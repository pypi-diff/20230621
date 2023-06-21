# Comparing `tmp/nucliadb_node_binding-0.7.6.tar.gz` & `tmp/nucliadb_node_binding-0.7.7.tar.gz`

## Comparing `nucliadb_node_binding-0.7.6.tar` & `nucliadb_node_binding-0.7.7.tar`

### file list

```diff
@@ -1,212 +1,225 @@
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/Cargo.toml
--rw-r--r--   0        0        0       19 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/.gitignore
--rw-r--r--   0        0        0     2160 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/build.rs
--rw-r--r--   0        0        0     8365 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
--rw-r--r--   0        0        0     1025 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/lib.rs
--rw-r--r--   0        0        0    40864 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/reader.rs
--rw-r--r--   0        0        0     4464 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/schema.rs
--rw-r--r--   0        0        0    18383 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/search_query.rs
--rw-r--r--   0        0        0    12074 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/search_response.rs
--rw-r--r--   0        0        0    18426 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/writer.rs
--rw-r--r--   0        0        0     1496 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
--rw-r--r--   0        0        0     4724 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/stop_words/en.json
--rw-r--r--   0        0        0     4517 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/stop_words/es.json
--rw-r--r--   0        0        0     5233 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
--rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0        0        0     1045 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0        0        0      927 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0        0        0     1534 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0        0        0       72 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/entrypoint.sh
--rw-r--r--   0        0        0     1800 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0        0        0     3386 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0        0        0    15567 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0        0        0     2445 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/reader.py
--rw-r--r--   0        0        0     1961 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0        0        0     4132 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/servicer.py
--rw-r--r--   0        0        0     1657 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0        0        0     8485 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/shadow_shards.py
--rw-r--r--   0        0        0      854 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0        0        0     1082 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0        0        0     8625 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0        0        0     7770 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0        0        0     5131 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_shadow_shards.py
--rw-r--r--   0        0        0     1592 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_sidecar_servicer.py
--rw-r--r--   0        0        0     1866 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0        0        0     6015 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0        0        0     2181 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0        0        0       99 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0        0        0      214 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0        0        0      137 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0        0        0     1399 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0        0        0     2209 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/bin/payload_test.rs
--rw-r--r--   0        0        0     3460 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0        0        0    10193 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0        0        0     9014 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/env.rs
--rw-r--r--   0        0        0     1206 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0        0        0     1559 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0        0        0     1329 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0        0        0     5481 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0        0        0    18823 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/reader/grpc_driver.rs
--rw-r--r--   0        0        0    10688 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/reader/mod.rs
--rw-r--r--   0        0        0     1320 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/services/mod.rs
--rw-r--r--   0        0        0    25266 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/services/reader.rs
--rw-r--r--   0        0        0     9051 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/services/versions.rs
--rw-r--r--   0        0        0    21256 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/services/writer.rs
--rw-r--r--   0        0        0     4114 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/shard_metadata.rs
--rw-r--r--   0        0        0     4004 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0        0        0     2960 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0        0        0    25718 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/writer/grpc_driver.rs
--rw-r--r--   0        0        0     9476 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/writer/mod.rs
--rw-r--r--   0        0        0       43 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0        0        0     1454 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/common/constants.rs
--rw-r--r--   0        0        0     1162 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0        0        0     5487 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0        0        0    22733 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0        0        0     6891 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0        0        0     3451 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/Cargo.toml
--rw-r--r--   0        0        0       84 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/MANIFEST.in
--rw-r--r--   0        0        0     1302 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/Makefile
--rw-r--r--   0        0        0     5804 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/README.md
--rw-r--r--   0        0        0        7 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/VERSION
--rw-r--r--   0        0        0      921 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/__init__.py
--rw-r--r--   0        0        0    12339 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/batch_span.py
--rw-r--r--   0        0        0     1289 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/common.py
--rw-r--r--   0        0        0     3024 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/errors.py
--rw-r--r--   0        0        0     2929 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/__init__.py
--rw-r--r--   0        0        0     5603 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/metrics.py
--rw-r--r--   0        0        0    13481 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/tracing.py
--rw-r--r--   0        0        0    15218 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/grpc.py
--rw-r--r--   0        0        0     5384 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/grpc_metrics.py
--rw-r--r--   0        0        0     7420 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/jaeger.py
--rw-r--r--   0        0        0     8457 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/jetstream.py
--rw-r--r--   0        0        0     6457 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/logs.py
--rw-r--r--   0        0        0     7333 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/metrics.py
--rw-r--r--   0        0        0        0 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/py.typed
--rw-r--r--   0        0        0     1570 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/settings.py
--rw-r--r--   0        0        0      851 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/__init__.py
--rw-r--r--   0        0        0      984 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/conftest.py
--rw-r--r--   0        0        0      294 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/Makefile
--rw-r--r--   0        0        0      851 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/__init__.py
--rw-r--r--   0        0        0     1149 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld.proto
--rw-r--r--   0        0        0     2395 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.py
--rw-r--r--   0        0        0     1464 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.pyi
--rw-r--r--   0        0        0     2903 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.py
--rw-r--r--   0        0        0     1120 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.pyi
--rw-r--r--   0        0        0     1163 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld.proto
--rw-r--r--   0        0        0     2347 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2.py
--rw-r--r--   0        0        0     1235 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2.pyi
--rw-r--r--   0        0        0     2758 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.py
--rw-r--r--   0        0        0      990 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.pyi
--rw-r--r--   0        0        0     7421 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/integration/test_fastapi.py
--rw-r--r--   0        0        0     3376 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/integration/test_telemetry.py
--rw-r--r--   0        0        0    12955 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/telemetry.py
--rw-r--r--   0        0        0     3823 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_errors.py
--rw-r--r--   0        0        0     4646 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_logs.py
--rw-r--r--   0        0        0     6199 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_metrics.py
--rw-r--r--   0        0        0     3984 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tracerprovider.py
--rw-r--r--   0        0        0     5335 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/utils.py
--rw-r--r--   0        0        0      625 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/requirements.txt
--rw-r--r--   0        0        0      583 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/setup.cfg
--rw-r--r--   0        0        0     1670 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/setup.py
--rw-r--r--   0        0        0     2567 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/blocking.rs
--rw-r--r--   0        0        0     1247 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/lib.rs
--rw-r--r--   0        0        0     5080 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/payload.rs
--rw-r--r--   0        0        0    13230 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/sender.rs
--rw-r--r--   0        0        0     3272 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/sink.rs
--rw-r--r--   0        0        0     1915 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/sync.rs
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0        0        0       74 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0        0        0    10081 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0        0        0    15448 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0        0        0    12011 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0        0        0    11943 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0        0        0     4199 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0        0        0     7454 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0        0        0     4423 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point_provider/merge_worker.rs
--rw-r--r--   0        0        0     2995 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point_provider/merger.rs
--rw-r--r--   0        0        0     9056 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0        0        0    12089 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0        0        0     1477 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point_provider/work_flag.rs
--rw-r--r--   0        0        0     7142 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0        0        0    13871 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/key_value.rs
--rw-r--r--   0        0        0     2115 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0        0        0     6382 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0        0        0     3083 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0        0        0     4632 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0        0        0     5500 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0        0        0     4000 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/indexset/mod.rs
--rw-r--r--   0        0        0     4602 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/indexset/state.rs
--rw-r--r--   0        0        0     1632 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0        0        0     1301 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0        0        0    13579 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0        0        0    22224 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0        0        0     1488 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/context.rs
--rw-r--r--   0        0        0     5986 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0        0        0     4204 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0        0        0     3766 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0        0        0     2718 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/metrics/request_time.rs
--rw-r--r--   0        0        0     1976 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0        0        0     1647 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0        0        0     1852 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0        0        0     1781 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/Cargo.toml
--rw-r--r--   0        0        0     9600 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/bfs_engine.rs
--rw-r--r--   0        0        0     1812 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/errors.rs
--rw-r--r--   0        0        0    22269 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/graph_db.rs
--rw-r--r--   0        0        0     1895 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
--rw-r--r--   0        0        0    11054 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/index.rs
--rw-r--r--   0        0        0     1032 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/lib.rs
--rw-r--r--   0        0        0     5908 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/node_dictionary.rs
--rw-r--r--   0        0        0     5413 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/relations_io.rs
--rw-r--r--   0        0        0     2770 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/bfs.rs
--rw-r--r--   0        0        0      999 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/mod.rs
--rw-r--r--   0        0        0    15505 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/reader.rs
--rw-r--r--   0        0        0    14827 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/tests.rs
--rw-r--r--   0        0        0     3158 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/utils.rs
--rw-r--r--   0        0        0    11621 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/writer.rs
--rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0        0        0     2215 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0        0        0    26906 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0        0        0        0 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0        0        0     7067 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0        0        0     1321 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0        0        0    76517 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0        0        0     9975 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0        0        0    60235 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0        0        0    27367 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0        0        0     6040 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/Cargo.toml
--rw-r--r--   0        0        0      941 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/src/lib.rs
--rw-r--r--   0        0        0    30065 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/src/reader.rs
--rw-r--r--   0        0        0     2970 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/src/schema.rs
--rw-r--r--   0        0        0     7166 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/src/search_query.rs
--rw-r--r--   0        0        0    12671 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/src/writer.rs
--rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/Cargo.toml
--rw-r--r--   0        0        0      888 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/LICENSE-AGPL
--rw-r--r--   0        0        0      199 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/README.md
--rw-r--r--   0        0        0       81 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/entrypoint.sh
--rw-r--r--   0        0        0     7109 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/src/bin/manager.rs
--rw-r--r--   0        0        0      277 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/src/error.rs
--rw-r--r--   0        0        0      951 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/src/key.rs
--rw-r--r--   0        0        0      174 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/src/lib.rs
--rw-r--r--   0        0        0    15579 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/src/node.rs
--rw-r--r--   0        0        0     1227 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/src/register.rs
--rw-r--r--   0        0        0     1368 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/tests/cluster_reader.py
--rw-r--r--   0        0        0     7291 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/tests/integration.rs
--rw-r--r--   0        0        0     3277 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/tests/test2.py
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_ftp/Cargo.toml
--rw-r--r--   0        0        0     1549 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_ftp/README.md
--rw-r--r--   0        0        0     1172 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_ftp/src/error.rs
--rw-r--r--   0        0        0     7047 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_ftp/src/lib.rs
--rw-r--r--   0        0        0     4095 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_ftp/src/listener.rs
--rw-r--r--   0        0        0     2769 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_ftp/src/main.rs
--rw-r--r--   0        0        0     7315 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_ftp/src/publisher.rs
--rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/Cargo.toml
--rw-r--r--   0        0        0     1470 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/CHANGELOG.md
--rw-r--r--   0        0        0       53 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/README.md
--rw-r--r--   0        0        0     1192 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/pyproject.toml
--rw-r--r--   0        0        0    23646 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/src/lib.rs
--rw-r--r--   0        0        0     2097 2023-04-26 13:06:27.000000 nucliadb_node_binding-0.7.6/test.py
--rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     3127 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0        0        0     1045 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0        0        0      821 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0        0        0     1534 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0        0        0     1800 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0        0        0     3059 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0        0        0    12975 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0        0        0     2401 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/reader.py
+-rw-r--r--   0        0        0     1961 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0        0        0     2560 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/servicer.py
+-rw-r--r--   0        0        0     1500 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0        0        0      854 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0        0        0     1082 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0        0        0     8206 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0        0        0     6244 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0     1866 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0        0        0     4795 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0        0        0     2181 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0        0        0       99 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0        0        0      217 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0        0        0      268 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0        0        0     1501 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0        0        0     2217 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/bin/payload_test.rs
+-rw-r--r--   0        0        0     4081 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0        0        0    10514 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0        0        0     9598 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/env.rs
+-rw-r--r--   0        0        0     1205 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0        0        0     1559 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0        0        0     1371 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0        0        0     3145 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/middleware/debug.rs
+-rw-r--r--   0        0        0      980 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/middleware/mod.rs
+-rw-r--r--   0        0        0     4209 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/middleware/telemetry.rs
+-rw-r--r--   0        0        0     3327 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0        0        0    14848 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/reader/grpc_driver.rs
+-rw-r--r--   0        0        0     9310 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/reader/mod.rs
+-rw-r--r--   0        0        0     1320 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/services/mod.rs
+-rw-r--r--   0        0        0    25284 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/services/reader.rs
+-rw-r--r--   0        0        0     9051 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/services/versions.rs
+-rw-r--r--   0        0        0    21256 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/services/writer.rs
+-rw-r--r--   0        0        0     4114 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shard_metadata.rs
+-rw-r--r--   0        0        0     1248 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0        0        0     1969 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shards/shards_provider.rs
+-rw-r--r--   0        0        0     4223 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shards/unbounded_cache_provider/async_unbounded_reader.rs
+-rw-r--r--   0        0        0      869 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shards/unbounded_cache_provider/async_unbounded_writer.rs
+-rw-r--r--   0        0        0     1343 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shards/unbounded_cache_provider/mod.rs
+-rw-r--r--   0        0        0     3363 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shards/unbounded_cache_provider/unbounded_reader.rs
+-rw-r--r--   0        0        0      869 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shards/unbounded_cache_provider/unbounded_writer.rs
+-rw-r--r--   0        0        0     4245 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0        0        0     2184 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0        0        0    15249 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/writer/grpc_driver.rs
+-rw-r--r--   0        0        0     9466 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/writer/mod.rs
+-rw-r--r--   0        0        0       43 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0        0        0     1454 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/common/constants.rs
+-rw-r--r--   0        0        0     1162 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0        0        0     5681 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0        0        0    22733 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0        0        0     6891 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0        0        0     7438 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0        0        0       74 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0        0        0    10081 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0        0        0    16238 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0        0        0    12011 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0        0        0    12067 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0        0        0     4199 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0        0        0     7580 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0        0        0     4423 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point_provider/merge_worker.rs
+-rw-r--r--   0        0        0     2995 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point_provider/merger.rs
+-rw-r--r--   0        0        0    10205 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0        0        0    12464 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0        0        0     1477 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point_provider/work_flag.rs
+-rw-r--r--   0        0        0     7142 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0        0        0    13871 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/key_value.rs
+-rw-r--r--   0        0        0     2115 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0        0        0     6382 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0        0        0     3083 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0        0        0     4782 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0        0        0     6760 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0        0        0     4000 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/indexset/mod.rs
+-rw-r--r--   0        0        0     4602 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/indexset/state.rs
+-rw-r--r--   0        0        0     1702 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0        0        0     1301 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0        0        0    15077 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0        0        0    23293 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/Cargo.toml
+-rw-r--r--   0        0        0     9600 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/bfs_engine.rs
+-rw-r--r--   0        0        0     1812 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/errors.rs
+-rw-r--r--   0        0        0    22269 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/graph_db.rs
+-rw-r--r--   0        0        0     1895 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
+-rw-r--r--   0        0        0    11054 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/index.rs
+-rw-r--r--   0        0        0     1032 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/lib.rs
+-rw-r--r--   0        0        0     5908 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/node_dictionary.rs
+-rw-r--r--   0        0        0     5413 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/relations_io.rs
+-rw-r--r--   0        0        0     2770 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/bfs.rs
+-rw-r--r--   0        0        0      999 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/mod.rs
+-rw-r--r--   0        0        0    15505 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/reader.rs
+-rw-r--r--   0        0        0    14827 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/tests.rs
+-rw-r--r--   0        0        0     3158 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/utils.rs
+-rw-r--r--   0        0        0    11621 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/writer.rs
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0        0        0     2215 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0        0        0    26175 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0        0        0        0 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0        0        0     7067 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0        0        0     1321 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0        0        0    73759 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0        0        0     9895 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0        0        0    49810 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0        0        0    29641 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0        0        0     6040 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/Cargo.toml
+-rw-r--r--   0        0        0      888 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/LICENSE-AGPL
+-rw-r--r--   0        0        0      190 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/README.md
+-rw-r--r--   0        0        0     4233 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/src/bin/manager.rs
+-rw-r--r--   0        0        0      277 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/src/error.rs
+-rw-r--r--   0        0        0      951 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/src/key.rs
+-rw-r--r--   0        0        0      174 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/src/lib.rs
+-rw-r--r--   0        0        0    15579 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/src/node.rs
+-rw-r--r--   0        0        0     1227 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/src/register.rs
+-rw-r--r--   0        0        0     1368 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/tests/cluster_reader.py
+-rw-r--r--   0        0        0     7291 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/tests/integration.rs
+-rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/Cargo.toml
+-rw-r--r--   0        0        0      941 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/src/lib.rs
+-rw-r--r--   0        0        0    30065 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/src/reader.rs
+-rw-r--r--   0        0        0     2970 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/src/schema.rs
+-rw-r--r--   0        0        0     7166 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/src/search_query.rs
+-rw-r--r--   0        0        0    12956 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/src/writer.rs
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/Cargo.toml
+-rw-r--r--   0        0        0       84 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/MANIFEST.in
+-rw-r--r--   0        0        0     1182 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/Makefile
+-rw-r--r--   0        0        0     5804 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/README.md
+-rw-r--r--   0        0        0        8 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/VERSION
+-rw-r--r--   0        0        0      921 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/__init__.py
+-rw-r--r--   0        0        0    12339 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/batch_span.py
+-rw-r--r--   0        0        0     1289 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/common.py
+-rw-r--r--   0        0        0     2530 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/context.py
+-rw-r--r--   0        0        0     2855 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/errors.py
+-rw-r--r--   0        0        0     3127 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/__init__.py
+-rw-r--r--   0        0        0     1708 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/context.py
+-rw-r--r--   0        0        0     4087 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/metrics.py
+-rw-r--r--   0        0        0    13483 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/tracing.py
+-rw-r--r--   0        0        0     2426 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/utils.py
+-rw-r--r--   0        0        0    15377 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/grpc.py
+-rw-r--r--   0        0        0     5384 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/grpc_metrics.py
+-rw-r--r--   0        0        0     7420 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/jaeger.py
+-rw-r--r--   0        0        0     9674 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/jetstream.py
+-rw-r--r--   0        0        0     6952 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/logs.py
+-rw-r--r--   0        0        0     7981 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/metrics.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/py.typed
+-rw-r--r--   0        0        0     1570 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/settings.py
+-rw-r--r--   0        0        0      851 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/__init__.py
+-rw-r--r--   0        0        0      984 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/conftest.py
+-rw-r--r--   0        0        0      294 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/Makefile
+-rw-r--r--   0        0        0      851 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/__init__.py
+-rw-r--r--   0        0        0     1149 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld.proto
+-rw-r--r--   0        0        0     2395 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.py
+-rw-r--r--   0        0        0     1464 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.pyi
+-rw-r--r--   0        0        0     2903 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.py
+-rw-r--r--   0        0        0     1120 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1163 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld.proto
+-rw-r--r--   0        0        0     2347 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2.py
+-rw-r--r--   0        0        0     1235 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2.pyi
+-rw-r--r--   0        0        0     2758 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.py
+-rw-r--r--   0        0        0      990 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6424 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/integration/test_fastapi.py
+-rw-r--r--   0        0        0     3777 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/integration/test_telemetry.py
+-rw-r--r--   0        0        0    12955 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/telemetry.py
+-rw-r--r--   0        0        0      851 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1664 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/fastapi/test_context.py
+-rw-r--r--   0        0        0     1411 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/fastapi/test_utils.py
+-rw-r--r--   0        0        0     2254 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_context.py
+-rw-r--r--   0        0        0     3634 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_errors.py
+-rw-r--r--   0        0        0     5833 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_logs.py
+-rw-r--r--   0        0        0     7199 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_metrics.py
+-rw-r--r--   0        0        0     5324 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_tikv_instrumentation.py
+-rw-r--r--   0        0        0     5523 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tikv.py
+-rw-r--r--   0        0        0     3984 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tracerprovider.py
+-rw-r--r--   0        0        0     5088 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/utils.py
+-rw-r--r--   0        0        0      685 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/requirements.txt
+-rw-r--r--   0        0        0      583 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/setup.cfg
+-rw-r--r--   0        0        0     1670 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/setup.py
+-rw-r--r--   0        0        0     2567 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/blocking.rs
+-rw-r--r--   0        0        0     1249 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/lib.rs
+-rw-r--r--   0        0        0     5074 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/payload.rs
+-rw-r--r--   0        0        0    13230 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/sender.rs
+-rw-r--r--   0        0        0     3272 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/sink.rs
+-rw-r--r--   0        0        0     1915 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/sync.rs
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/Cargo.toml
+-rw-r--r--   0        0        0       19 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/.gitignore
+-rw-r--r--   0        0        0     2160 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/build.rs
+-rw-r--r--   0        0        0     8365 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
+-rw-r--r--   0        0        0     1025 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/lib.rs
+-rw-r--r--   0        0        0    40864 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/reader.rs
+-rw-r--r--   0        0        0     4464 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/schema.rs
+-rw-r--r--   0        0        0    18720 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/search_query.rs
+-rw-r--r--   0        0        0    12074 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/search_response.rs
+-rw-r--r--   0        0        0    18694 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/writer.rs
+-rw-r--r--   0        0        0     1496 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
+-rw-r--r--   0        0        0     4724 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/stop_words/en.json
+-rw-r--r--   0        0        0     4517 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/stop_words/es.json
+-rw-r--r--   0        0        0     5233 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0        0        0     5986 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0        0        0     4193 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0        0        0     1519 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/meters/console.rs
+-rw-r--r--   0        0        0     1456 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0        0        0     1262 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/meters/noop.rs
+-rw-r--r--   0        0        0     2928 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0        0        0     1551 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0        0        0     2708 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0        0        0    13774 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0        0        0     3010 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/middleware.rs
+-rw-r--r--   0        0        0     1561 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0        0        0     2407 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0        0        0     1976 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0        0        0     1647 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0        0        0     1852 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0        0        0     1781 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/Cargo.toml
+-rw-r--r--   0        0        0     1552 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/CHANGELOG.md
+-rw-r--r--   0        0        0       53 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/README.md
+-rw-r--r--   0        0        0     1192 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0    22938 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/src/lib.rs
+-rw-r--r--   0        0        0     2097 2023-06-21 10:26:02.000000 nucliadb_node_binding-0.7.7/test.py
+-rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 nucliadb_node_binding-0.7.7/PKG-INFO
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/build.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/lib.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/reader.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/reader.rs`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 use std::fmt::Debug;
 use std::fs;
 use std::time::SystemTime;
 
-use nucliadb_core::context;
+use nucliadb_core::metrics;
 use nucliadb_core::metrics::request_time;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::order_by::{OrderField, OrderType};
 use nucliadb_core::protos::{
     OrderBy, ParagraphItem, ParagraphSearchRequest, ParagraphSearchResponse, ResourceId,
     StreamRequest, SuggestRequest,
 };
@@ -71,15 +71,15 @@
         let id: Option<String> = None;
         let searcher = self.reader.searcher();
         let count = searcher.search(&AllQuery, &Count).unwrap_or_default();
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Ending at: {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::paragraphs("count".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(count)
     }
     #[tracing::instrument(skip_all)]
@@ -120,15 +120,15 @@
             if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
                 debug!("{id:?} - Trying fuzzy: ends at {v} ms");
             }
         }
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Ending at: {v} ms");
         }
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::paragraphs("suggest".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(ParagraphSearchResponse::from(SearchBm25Response {
             total: results.len(),
             top_docs: results,
@@ -240,15 +240,15 @@
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Producing results: starts at {v} ms");
         }
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Ending at: {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::paragraphs("search".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(response)
     }
     #[tracing::instrument(skip_all)]
@@ -265,15 +265,15 @@
             let Some(key) = searcher
                 .doc(addr)?
                 .get_first(self.schema.uuid)
                 .and_then(|i| i.as_text().map(String::from)) else { continue };
             keys.push(key);
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::paragraphs("stored_ids".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(keys)
     }
 }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/schema.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/search_query.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/search_query.rs`

 * *Files 1% similar despite different names*

```diff
@@ -407,14 +407,21 @@
         .flat_map(|facet_key| Facet::from_text(facet_key).ok().into_iter())
         .for_each(|facet| {
             let facet_term = Term::from_facet(schema.facets, &facet);
             let facet_term_query = TermQuery::new(facet_term, IndexRecordOption::Basic);
             fuzzies.push((Occur::Must, Box::new(facet_term_query.clone())));
             originals.push((Occur::Must, Box::new(facet_term_query)));
         });
+    // Keys
+    search.key_filters.iter().for_each(|uuid| {
+        let term = Term::from_field_text(schema.uuid, uuid);
+        let term_query = TermQuery::new(term, IndexRecordOption::Basic);
+        fuzzies.push((Occur::Must, Box::new(term_query.clone())));
+        originals.push((Occur::Must, Box::new(term_query)));
+    });
 
     if originals.len() == 1 && originals[0].1.is::<AllQuery>() {
         let original = originals.pop().unwrap().1;
         let fuzzy = Box::new(BooleanQuery::new(vec![]));
         (original, termc, fuzzy)
     } else {
         if processed.fuzzy_query.is_empty() {
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/search_response.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/src/writer.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/src/writer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fs;
 use std::time::SystemTime;
 
-use nucliadb_core::context;
+use nucliadb_core::metrics;
 use nucliadb_core::metrics::request_time;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::prost::Message;
 use nucliadb_core::protos::resource::ResourceStatus;
 use nucliadb_core::protos::{Resource, ResourceId};
 use nucliadb_core::tracing::{self, *};
 use regex::Regex;
@@ -75,15 +75,15 @@
         let reader = self.index.reader()?;
         let searcher = reader.searcher();
         let count = searcher.search(&AllQuery, &Count)?;
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Ending at: {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::paragraphs("count".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(count)
     }
     #[tracing::instrument(skip_all)]
@@ -115,15 +115,15 @@
             debug!("{id:?} - Commit: starts at {v} ms");
         }
         self.writer.commit()?;
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Commit: ends at {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::paragraphs("set_resource".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(())
     }
     #[tracing::instrument(skip_all)]
@@ -144,15 +144,15 @@
             debug!("{id:?} - Commit: starts at {v} ms");
         }
         self.writer.commit()?;
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Commit: ends at {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::paragraphs("delete_resource".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(())
     }
     #[tracing::instrument(skip_all)]
@@ -216,17 +216,27 @@
             index,
             writer,
             schema: paragraph_schema,
         })
     }
 
     fn index_paragraph(&mut self, resource: &Resource) -> tantivy::Result<()> {
-        let metadata = resource.metadata.as_ref().unwrap();
-        let modified = metadata.modified.as_ref().unwrap();
-        let created = metadata.created.as_ref().unwrap();
+        let metadata = resource
+            .metadata
+            .as_ref()
+            .expect("Missing resource metadata");
+        let modified = metadata
+            .modified
+            .as_ref()
+            .expect("Missing resource modified date in metadata");
+        let created = metadata
+            .created
+            .as_ref()
+            .expect("Missing resource created date in metadata");
+
         let empty_paragraph = HashMap::with_capacity(0);
         let inspect_paragraph = |field: &str| {
             resource
                 .paragraphs
                 .get(field)
                 .map_or_else(|| &empty_paragraph, |i| &i.paragraphs)
         };
@@ -260,15 +270,15 @@
                     .labels
                     .iter()
                     .map(Facet::from_text)
                     .collect::<Result<Vec<_>, _>>()
                     .map_err(|e| tantivy::TantivyError::InvalidArgument(e.to_string()))?;
 
                 let mut doc = doc!(
-                    self.schema.uuid => resource.resource.as_ref().unwrap().uuid.as_str(),
+                    self.schema.uuid => resource.resource.as_ref().expect("Missing resource details").uuid.as_str(),
                     self.schema.modified => timestamp_to_datetime_utc(modified),
                     self.schema.created => timestamp_to_datetime_utc(created),
                     self.schema.status => resource.status as u64,
                     self.schema.repeated_in_field => p.repeated_in_field as u64,
                 );
 
                 if let Some(ref metadata) = p.metadata {
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/stop_words/ca.json` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/stop_words/en.json` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/stop_words/es.json` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_paragraphs/stop_words/fr.json` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_paragraphs/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 uuid = { version = "1.1", features = ["serde", "v4"] }
 bincode = "1.3.3"
 async-trait = "0.1.51"
 time = "0.3.3"
 itertools = "0.10"
 anyhow = "1"
 http = "0.2"
+hyper = "0.14.26"
+tower = "0.4.13"
 thiserror = "1"
 opentelemetry = { version = "0.17", features = ["rt-tokio", "trace"] }
 tracing-opentelemetry = "0.17.2"
 reqwest = "0.11.16"
 
 # Test dependencies
 tempfile = "3.2.0"
@@ -67,15 +69,14 @@
 async-stream = "0.3.2"
 
 rand = "0.8.4"
 
 # nucliadb dependencies
 nucliadb_cluster = { path = "../nucliadb_cluster" }
 nucliadb_telemetry = { path = "../nucliadb_telemetry" }
-nucliadb_ftp = { path = "../nucliadb_ftp" }
 nucliadb_core = { path = "../nucliadb_core" }
 nucliadb_texts= { path = "../nucliadb_texts" }
 nucliadb_paragraphs= { path = "../nucliadb_paragraphs" }
 nucliadb_vectors= { path = "../nucliadb_vectors" }
 nucliadb_relations= { path = "../nucliadb_relations" }
 
 # test
@@ -85,14 +86,15 @@
 # sentry sdk
 sentry = "0.26.0"
 opentelemetry-jaeger = { version = "0.16.0", features = ["rt-tokio"] }
 tracing-subscriber = { version = "0.3.11", features = [
     "env-filter",
     "registry",
     "std",
+    "json",
 ] }
 dotenvy = "0.15.1"
 tracing-log = { version = "0.1.3", features = ["env_logger"] }
 opentelemetry-zipkin = "0.15.0"
 sentry-tracing = "0.27.0"
 
 parse_duration = "2.1.1"
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .PHONY: install-dev
 install-dev:
-## TODO: remove pip version install when pip is fixed. Right now it was making mypy fail.
-	pip install --upgrade "pip<23.1"
-	pip install -r ../test-requirements.txt
-	pip install -r ../code-requirements.txt
-	cd .. && pip install -r nucliadb_node/requirements-sources.txt
-	pip install -r requirements.txt
+	pip install --upgrade pip wheel
+	cd .. && pip install \
+		-r test-requirements.txt \
+		-r code-requirements.txt \
+		-r nucliadb_node/requirements-sources.txt \
+		-r nucliadb_node/requirements.txt
 	pip install -e .
 
 .PHONY: format
 format:
 	isort --profile black .
 	black .
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,29 +15,28 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 import asyncio
-import logging
-import sys
 import uuid
 
 import pkg_resources
 from nucliadb_telemetry import errors
+from nucliadb_telemetry.logs import setup_logging
 from nucliadb_telemetry.utils import setup_telemetry
 from nucliadb_utils.fastapi.run import serve_metrics
 from nucliadb_utils.run import run_until_exit
 
 from nucliadb_node import SERVICE_NAME, logger
 from nucliadb_node.pull import Worker
 from nucliadb_node.reader import Reader
 from nucliadb_node.service import start_grpc
-from nucliadb_node.settings import running_settings, settings
+from nucliadb_node.settings import settings
 from nucliadb_node.writer import Writer
 
 
 async def start_worker(writer: Writer, reader: Reader) -> Worker:
     if settings.force_host_id is None:  # pragma: no cover
         node = None
         i = 0
@@ -86,20 +85,12 @@
         reader.close,
     ]
 
     await run_until_exit(finalizers)
 
 
 def run():  # pragma: no cover
-    errors.setup_error_handling(pkg_resources.get_distribution("nucliadb_node").version)
-
-    logging.basicConfig(
-        level=logging.INFO,
-        format="[%(asctime)s.%(msecs)02d] [%(levelname)s] - %(name)s - %(message)s",
-        datefmt="%Y-%m-%d %H:%M:%S",
-        stream=sys.stderr,
-    )
+    setup_logging()
 
-    logger.setLevel(logging.getLevelName(running_settings.log_level.upper()))
-    logging.getLogger("asyncio").setLevel(logging.ERROR)
+    errors.setup_error_handling(pkg_resources.get_distribution("nucliadb_node").version)
 
     asyncio.run(main())
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,32 +25,24 @@
 import nats
 from grpc import StatusCode
 from grpc.aio import AioRpcError  # type: ignore
 from nats.aio.client import Msg
 from nats.aio.subscription import Subscription
 from nats.js.errors import NotFoundError as StreamNotFoundError
 from nucliadb_protos.noderesources_pb2 import Resource, ResourceID, ShardIds
-from nucliadb_protos.nodewriter_pb2 import (
-    IndexedMessage,
-    IndexMessage,
-    OpStatus,
-    TypeMessage,
-)
+from nucliadb_protos.nodewriter_pb2 import IndexMessage, OpStatus, TypeMessage
+from nucliadb_protos.writer_pb2 import Notification
 from nucliadb_telemetry import errors, metrics
+from nucliadb_utils import const
 from nucliadb_utils.nats import get_traced_jetstream
 from nucliadb_utils.storages.exceptions import IndexDataNotFound
 from nucliadb_utils.storages.storage import Storage
-from nucliadb_utils.utilities import (
-    Utility,
-    clean_utility,
-    get_storage,
-    get_transaction_utility,
-)
+from nucliadb_utils.utilities import get_pubsub, get_storage
 
-from nucliadb_node import SERVICE_NAME, logger, shadow_shards
+from nucliadb_node import SERVICE_NAME, logger
 from nucliadb_node.reader import Reader
 from nucliadb_node.settings import indexing_settings, settings
 from nucliadb_node.writer import Writer
 
 subscriber_observer = metrics.Observer(
     "message_processor",
     buckets=[
@@ -86,60 +78,53 @@
         self.reader = reader
         self.subscriptions = []
         self.ack_wait = 10 * 60
         self.lock = asyncio.Lock()
         self.event = asyncio.Event()
         self.node = node
         self.gc_task = None
-        self.ssm = shadow_shards.get_manager()
-        self.publisher = IndexedPublisher(
-            stream=indexing_settings.indexed_jetstream_stream,
-            subject=indexing_settings.indexed_jetstream_target,
-            auth=indexing_settings.index_jetstream_auth,
-            servers=indexing_settings.index_jetstream_servers,
-        )
+        self.publisher = IndexedPublisher()
         self.load_seqid()
+        self.brain: Optional[Resource] = None
 
     async def finalize(self):
         if self.gc_task:
             self.gc_task.cancel()
 
+        await self.publisher.finalize()
         await self.subscriber_finalize()
 
-        transaction_utility = get_transaction_utility()
-        if transaction_utility:
-            await transaction_utility.finalize()
-            clean_utility(Utility.TRANSACTION)
-
-        await self.publisher.finalize()
         await self.storage.finalize()
 
     async def disconnected_cb(self):
         logger.info("Got disconnected from NATS!")
 
     async def reconnected_cb(self):
         # See who we are connected to on reconnect
-        logger.info("Got reconnected to NATS {url}".format(url=self.nc.connected_url))
+        logger.warning(
+            f"Got reconnected to NATS {self.nc.connected_url}. Attempting reconnect"
+        )
+        await self.drain_subscriptions()
+        await self.subscribe()
 
     async def error_cb(self, e):
         errors.capture_exception(e)
         logger.error(
             "There was an error on the worker, check sentry: {}".format(e),
             exc_info=True,
         )
 
     async def closed_cb(self):
         logger.info("Connection is closed on NATS")
 
     async def initialize(self):
         self.storage = await get_storage(service_name=SERVICE_NAME)
-        await self.ssm.load()
         self.event.clear()
-        await self.subscriber_initialize()
         await self.publisher.initialize()
+        await self.subscriber_initialize()
         self.gc_task = asyncio.create_task(self.garbage())
 
     async def subscriber_initialize(self):
         options = {
             "error_cb": self.error_cb,
             "closed_cb": self.closed_cb,
             "reconnected_cb": self.reconnected_cb,
@@ -152,22 +137,24 @@
             options["servers"] = indexing_settings.index_jetstream_servers
 
         self.nc = await nats.connect(**options)
         self.js = get_traced_jetstream(self.nc, SERVICE_NAME)
         logger.info(f"Nats: Connected to {indexing_settings.index_jetstream_servers}")
         await self.subscribe()
 
-    async def subscriber_finalize(self):
+    async def drain_subscriptions(self) -> None:
         for subscription in self.subscriptions:
             try:
                 await subscription.drain()
             except nats.errors.ConnectionClosedError:
                 pass
         self.subscriptions = []
 
+    async def subscriber_finalize(self):
+        await self.drain_subscriptions()
         try:
             await self.nc.close()
         except (RuntimeError, AttributeError):  # pragma: no cover
             # RuntimeError: can be thrown if event loop is closed
             # AttributeError: can be thrown by nats-py when handling shutdown
             pass
 
@@ -208,39 +195,30 @@
         try:
             with open(f"{settings.data_path}/seqid", "r") as seqfile:
                 self.last_seqid = int(seqfile.read())
         except FileNotFoundError:
             # First time the consumer is started
             self.last_seqid = None
 
-    async def set_resource(self, pb: IndexMessage) -> Optional[OpStatus]:
-        brain: Resource = await self.storage.get_indexing(pb)
-        brain.shard_id = brain.resource.shard_id = pb.shard
-        is_shadow_shard = self.ssm.exists(pb.shard)
+    async def set_resource(self, pb: IndexMessage) -> OpStatus:
+        self.brain = await self.storage.get_indexing(pb)
+        self.brain.shard_id = self.brain.resource.shard_id = pb.shard
         logger.info(
-            f"Added [shadow={is_shadow_shard}] {brain.resource.uuid} at {brain.shard_id} otx:{pb.txid}"
+            f"Added {self.brain.resource.uuid} at {self.brain.shard_id} otx:{pb.txid}"
         )
-        status: Optional[OpStatus] = None
-        if is_shadow_shard:
-            await self.ssm.set_resource(brain, pb.shard, pb.txid)
-        else:
-            status = await self.writer.set_resource(brain)
+        status = await self.writer.set_resource(self.brain)
         logger.info(f"...done")
-        del brain
+        del self.brain
+        self.brain = None
         return status
 
-    async def delete_resource(self, pb: IndexMessage) -> Optional[OpStatus]:
-        is_shadow_shard = self.ssm.exists(pb.shard)
-        logger.info(f"Deleting [shadow={is_shadow_shard}] {pb.resource} otx:{pb.txid}")
-        status: Optional[OpStatus] = None
-        if is_shadow_shard:
-            await self.ssm.delete_resource(pb.resource, pb.shard, pb.txid)
-        else:
-            rid = ResourceID(uuid=pb.resource, shard_id=pb.shard)
-            status = await self.writer.delete_resource(rid)
+    async def delete_resource(self, pb: IndexMessage) -> OpStatus:
+        logger.info(f"Deleting {pb.resource} otx:{pb.txid}")
+        rid = ResourceID(uuid=pb.resource, shard_id=pb.shard)
+        status = await self.writer.delete_resource(rid)
         logger.info(f"...done")
         return status
 
     @subscriber_observer.wrap()
     async def subscription_worker(self, msg: Msg):
         subject = msg.subject
         reply = msg.reply
@@ -272,22 +250,28 @@
                 if grpc_error.code() == StatusCode.NOT_FOUND:
                     logger.error(f"Shard does not exist {pb.shard}")
                 else:
                     event_id = errors.capture_exception(grpc_error)
                     logger.error(
                         f"An error on subscription_worker. Check sentry for more details. Event id: {event_id}"
                     )
-                    raise grpc_error
+                    if (
+                        pb.typemessage == TypeMessage.CREATION
+                        and self.brain
+                        and self.brain.HasField("metadata")
+                    ):
+                        # Hard fail if we have the correct data
+                        raise grpc_error
 
             except IndexDataNotFound as storage_error:
                 # This should never happen now.
                 # Remove this block in the future once we're confident it's not needed.
                 errors.capture_exception(storage_error)
                 logger.warning(
-                    "Error retrieving the indexing payload we do not block as that means its already deleted"
+                    "Error retrieving the indexing payload we do not block as that means its already deleted!"
                 )
             except Exception as e:
                 event_id = errors.capture_exception(e)
                 logger.error(
                     f"An error on subscription_worker. Check sentry for more details. Event id: {event_id}"
                 )
                 raise e
@@ -302,116 +286,66 @@
                 f"An error on subscription_worker. Check sentry for more details."
             )
             raise e
 
     async def subscribe(self):
         logger.info(f"Last seqid {self.last_seqid}")
         try:
-            await self.js.stream_info(indexing_settings.index_jetstream_stream)
+            await self.js.stream_info(const.Streams.INDEX.name)
         except StreamNotFoundError:
             logger.info("Creating stream")
             res = await self.js.add_stream(
-                name=indexing_settings.index_jetstream_stream,
-                subjects=[indexing_settings.index_jetstream_target.format(node=">")],
+                name=const.Streams.INDEX.name,
+                subjects=[
+                    const.Streams.INDEX.subject.format(node=">"),
+                ],
             )
-            await self.js.stream_info(indexing_settings.index_jetstream_stream)
+            await self.js.stream_info(const.Streams.INDEX.name)
 
+        subject = const.Streams.INDEX.subject.format(node=self.node)
         res = await self.js.subscribe(
-            subject=indexing_settings.index_jetstream_target.format(node=self.node),
-            queue=indexing_settings.index_jetstream_group.format(node=self.node),
-            stream=indexing_settings.index_jetstream_stream,
+            subject=subject,
+            queue=const.Streams.INDEX.group.format(node=self.node),
+            stream=const.Streams.INDEX.name,
             flow_control=True,
             cb=self.subscription_worker,
             config=nats.js.api.ConsumerConfig(
                 deliver_policy=nats.js.api.DeliverPolicy.BY_START_SEQUENCE,
                 opt_start_seq=self.last_seqid or 1,
                 ack_policy=nats.js.api.AckPolicy.EXPLICIT,
                 max_deliver=10000,
                 max_ack_pending=1,
                 ack_wait=self.ack_wait,
                 idle_heartbeat=5,
             ),
         )
         self.subscriptions.append(res)
-        logger.info(
-            f"Subscribed to {indexing_settings.index_jetstream_target.format(node=self.node)} on \
-             stream {indexing_settings.index_jetstream_stream}"
-        )
+        logger.info(f"Subscribed to {subject} on stream {const.Streams.INDEX.name}")
 
 
 class IndexedPublisher:
-    def __init__(
-        self,
-        stream: str,
-        subject: str,
-        servers: List[str],
-        auth: Optional[str],
-    ):
-        self.stream = stream
-        self.subject = subject
-        self.auth: Optional[str] = auth
-        self.servers: List[str] = servers
-        self.js = None
-        self.nc = None
+    def __init__(self):
+        self.pubsub = None
 
     async def initialize(self):
-        options = dict(
-            closed_cb=self.on_connection_closed,
-            reconnected_cb=self.on_reconnection,
-        )
-        if self.auth is not None:
-            options["user_credentials"] = self.auth
-        if len(self.servers) > 0:
-            options["servers"] = self.servers
-        self.nc = await nats.connect(**options)
-        self.js = get_traced_jetstream(self.nc, SERVICE_NAME)
-        await self.create_stream_if_not_exists()
-
-    async def create_stream_if_not_exists(self):
-        try:
-            await self.js.stream_info(self.stream)
-        except StreamNotFoundError:
-            logger.info("Creating publisher stream")
-            await self.js.add_stream(
-                name=self.stream,
-                subjects=[self.subject.format(partition=">")],
-            )
-            await self.js.stream_info(self.stream)
-
-    async def on_reconnection(self):
-        logger.warning(
-            "Got reconnected to NATS {url}".format(url=self.nc.connected_url)
-        )
-
-    async def on_connection_closed(self):
-        logger.warning("Connection is closed on NATS")
+        self.pubsub = await get_pubsub()
 
     async def finalize(self):
-        if self.nc is not None:
-            try:
-                await self.nc.flush()
-                await self.nc.close()
-            except (RuntimeError, AttributeError):  # pragma: no cover
-                # RuntimeError: can be thrown if event loop is closed
-                # AttributeError: can be thrown by nats-py when handling shutdown
-                pass
-            self.nc = None
+        await self.pubsub.finalize()
 
     async def indexed(self, indexpb: IndexMessage):
-        if self.js is None:
-            raise RuntimeError("Not initialized")
-
         if not indexpb.HasField("partition"):
             logger.warning(f"Could not publish message without partition")
             return
 
-        indexedpb = IndexedMessage()
-        indexedpb.node = indexpb.node
-        indexedpb.shard = indexpb.shard
-        indexedpb.txid = indexpb.txid
-        indexedpb.resource = indexpb.resource
-        indexedpb.typemessage = indexpb.typemessage
-        indexedpb.reindex_id = indexpb.reindex_id
-        subject = self.subject.format(partition=indexpb.partition)
-        await self.js.publish(subject, indexedpb.SerializeToString())
-        logger.info(f"Published to indexed stream {subject}")
-        return
+        message = Notification(
+            partition=int(indexpb.partition),
+            seqid=indexpb.txid,
+            uuid=indexpb.resource,
+            kbid=indexpb.kbid,
+            action=Notification.INDEXED,
+        )
+
+        await self.pubsub.publish(
+            const.PubSubChannels.RESOURCE_NOTIFY.format(kbid=indexpb.kbid),
+            message.SerializeToString(),
+        )
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/reader.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 from nucliadb_node import SERVICE_NAME  # type: ignore
 
 CACHE = LRU(128)
 
 
 class Reader:
-    _stub: Optional[NodeReaderStub] = None
     lock: asyncio.Lock
 
     def __init__(self, grpc_reader_address: str):
         self.lock = asyncio.Lock()
         self.channel = get_traced_grpc_channel(grpc_reader_address, SERVICE_NAME)
         self.stub = NodeReaderStub(self.channel)
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/servicer.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/servicer.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,21 +33,18 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from nucliadb_protos import nodesidecar_pb2_grpc
-from nucliadb_protos.noderesources_pb2 import EmptyQuery, ShardId
-from nucliadb_protos.nodesidecar_pb2 import Counter, ShadowShardResponse
-from nucliadb_telemetry import errors
+from nucliadb_protos.noderesources_pb2 import ShardId
+from nucliadb_protos.nodesidecar_pb2 import Counter
 
-from nucliadb_node import logger, shadow_shards
 from nucliadb_node.reader import Reader
-from nucliadb_node.shadow_shards import ShadowShardNotFound, ShadowShardsManager
 from nucliadb_node.writer import Writer
 
 
 class SidecarServicer(nodesidecar_pb2_grpc.NodeSidecarServicer):
     def __init__(self, reader: Reader, writer: Writer):
         self.reader = reader
         self.writer = writer
@@ -61,41 +58,7 @@
     async def GetCount(self, request: ShardId, context) -> Counter:  # type: ignore
         response = Counter()
         shard = await self.reader.get_shard(request)
         if shard is not None:
             response.resources = shard.resources
             response.paragraphs = shard.paragraphs
         return response
-
-    async def CreateShadowShard(self, request: EmptyQuery, context) -> ShadowShardResponse:  # type: ignore
-        ssm: ShadowShardsManager = shadow_shards.get_manager()
-        await ssm.load()
-        response = ShadowShardResponse()
-        try:
-            shard_id = await ssm.create()
-            response.success = True
-            response.shard.id = shard_id
-        except Exception as exc:
-            errors.capture_exception(exc)
-            logger.warning(f"Error creating shadow shard: {shard_id}")
-        finally:
-            return response
-
-    async def DeleteShadowShard(self, request: ShardId, context) -> ShadowShardResponse:  # type: ignore
-        ssm = shadow_shards.get_manager()
-        await ssm.load()
-        response = ShadowShardResponse()
-        shard_id = request.id
-        try:
-            await ssm.delete(shard_id=shard_id)
-            response.success = True
-            response.shard.id = shard_id
-        except ShadowShardNotFound:
-            logger.warning(
-                f"Attempting to delete a shadow shard that does not exist: {shard_id}"
-            )
-            response.success = True
-        except Exception as exc:
-            errors.capture_exception(exc)
-            logger.warning(f"Error deleting shadow shard: {shard_id}")
-        finally:
-            return response
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,22 +31,15 @@
     reader_listen_address: str = "0.0.0.0:10001"
     sidecar_listen_address: str = "0.0.0.0:10002"
 
     data_path: Optional[str] = None
 
 
 settings = Settings()
-
-
-class IndexingSettings(utils_settings.IndexingSettings):
-    indexed_jetstream_target: str = "indexed.{partition}"
-    indexed_jetstream_stream: str = "indexed"
-
-
-indexing_settings = IndexingSettings()
+indexing_settings = utils_settings.IndexingSettings()
 
 
 class RunningSettings(BaseSettings):
     debug: bool = True
     log_level: str = "DEBUG"
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 from grpc import aio, insecure_channel  # type: ignore
 from grpc_health.v1 import health_pb2_grpc  # type: ignore
 from grpc_health.v1.health_pb2 import HealthCheckRequest  # type: ignore
 from nucliadb_protos.noderesources_pb2 import EmptyQuery, ShardCreated, ShardId
 from nucliadb_protos.nodesidecar_pb2_grpc import NodeSidecarStub
 from nucliadb_protos.nodewriter_pb2 import NewShardRequest
 from nucliadb_protos.nodewriter_pb2_grpc import NodeWriterStub
+from nucliadb_utils.cache.settings import settings as cache_settings
 from pytest_docker_fixtures import images  # type: ignore
 from pytest_docker_fixtures.containers._base import BaseImage  # type: ignore
 
-from nucliadb_node import shadow_shards
 from nucliadb_node.app import start_worker
 from nucliadb_node.pull import Worker
 from nucliadb_node.reader import Reader
 from nucliadb_node.service import start_grpc
 from nucliadb_node.settings import indexing_settings, settings
 from nucliadb_node.writer import Writer
 
@@ -206,14 +206,16 @@
     reader,
     writer,
     grpc_server,
 ) -> AsyncIterable[Worker]:
     settings.force_host_id = "node1"
     settings.data_path = data_path
     indexing_settings.index_jetstream_servers = [natsd]
+    cache_settings.cache_pubsub_driver = "nats"
+    cache_settings.cache_pubsub_nats_url = [natsd]
 
     worker = await start_worker(writer, reader)
     yield worker
 
     # Cleanup all shards to be ready for following tests
     shards = await writer_stub.ListShards(EmptyQuery())  # type: ignore
     for shard in shards.ids:  # pragma: no cover
@@ -240,32 +242,14 @@
 
 
 @pytest.fixture(scope="function")
 def data_path():
     with tempfile.TemporaryDirectory() as td:
         previous = os.environ.get("DATA_PATH")
         os.environ["DATA_PATH"] = str(td)
-        shadow_shards.MAIN.pop("manager", None)
 
         yield str(td)
 
         if previous is None:
             os.environ.pop("DATA_PATH")
         else:  # pragma: no cover
             os.environ["DATA_PATH"] = previous
-
-
-@pytest.fixture(scope="function")
-def shadow_folder(data_path) -> str:
-    return shadow_shards.SHADOW_SHARDS_FOLDER.format(data_path=data_path)
-
-
-@pytest.fixture(scope="function")
-async def shadow_shard(
-    sidecar_stub: NodeSidecarStub, shadow_folder: str
-) -> AsyncIterable[str]:
-    resp = await sidecar_stub.CreateShadowShard(EmptyQuery())  # type: ignore
-    assert resp.success
-
-    yield resp.shard.id
-
-    await sidecar_stub.DeleteShadowShard(resp.shard)  # type: ignore
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
+import uuid
 from datetime import datetime
 from typing import Optional
 
-import nats
 import pytest
 from grpc.aio import AioRpcError  # type: ignore
 from nucliadb_protos.noderesources_pb2 import Resource, Shard, ShardId
-from nucliadb_protos.nodewriter_pb2 import IndexedMessage, IndexMessage, TypeMessage
-from nucliadb_utils.utilities import get_storage
+from nucliadb_protos.nodewriter_pb2 import IndexMessage, TypeMessage
+from nucliadb_protos.writer_pb2 import Notification
+from nucliadb_utils import const
+from nucliadb_utils.utilities import get_pubsub, get_storage
 
-from nucliadb_node import SERVICE_NAME, shadow_shards
+from nucliadb_node import SERVICE_NAME
 from nucliadb_node.pull import Worker
-from nucliadb_node.settings import indexing_settings, settings
-from nucliadb_node.shadow_shards import OperationCode
+from nucliadb_node.settings import settings
 
 TEST_PARTITION = "111"
 
 
 @pytest.mark.asyncio
 async def test_indexing(worker, shard: str, reader):
     node = settings.force_host_id
@@ -83,69 +84,36 @@
     sipb.id = shard
 
     with pytest.raises(AioRpcError):
         await reader.get_shard(sipb)
 
 
 @pytest.mark.asyncio
-async def test_indexing_shadow_shard(data_path, worker, shadow_shard: str):
-    storage = await get_storage(service_name=SERVICE_NAME)
-    node_id = settings.force_host_id
-
-    # Add a set resource operation
-    pb = resource_payload(shadow_shard)
-    setpb = await create_indexing_message(pb, "kb", shadow_shard, node_id)  # type: ignore
-    await send_indexing_message(worker, setpb, node_id)  # type: ignore
-
-    # Add a delete operation
-    deletepb = delete_indexing_message("bar", shadow_shard, node_id)  # type: ignore
-    await send_indexing_message(worker, deletepb, node_id)  # type: ignore
-
-    # Check that they were stored in a shadow shard
-    ssm = shadow_shards.get_manager()
-
-    ops = []
-    for _ in range(10):
-        print("Waiting for sidecar to consume messages...")
-        await asyncio.sleep(1)
-        ops = [op async for op in ssm.iter_operations(shadow_shard)]
-        if len(ops) == 2:
-            break
-    assert len(ops) == 2
-    assert ops[0][0] == OperationCode.SET
-    assert ops[0][1] == pb
-    assert ops[1][0] == OperationCode.DELETE
-    assert ops[1][1] == "bar"
-
-    await asyncio.sleep(1)
-
-    assert await storage.get_indexing(setpb) is not None
-
-
-@pytest.mark.asyncio
 async def test_indexing_publishes_to_sidecar_index_stream(worker, shard: str, natsd):
     node_id = settings.force_host_id
     assert node_id
 
     indexpb = await create_indexing_message(
         resource_payload(shard), "kb", shard, node_id
     )
 
+    waiting_task = asyncio.create_task(wait_for_indexed_message("kb"))
+    await asyncio.sleep(0.1)
+
     await send_indexing_message(worker, indexpb, node_id)  # type: ignore
 
-    msg = await get_indexed_message(natsd)
+    msg = await waiting_task
 
-    assert msg.subject == f"indexed.{TEST_PARTITION}"
-    indexedpb = IndexedMessage()
-    indexedpb.ParseFromString(msg.data)
-    assert indexedpb.node == indexpb.node
-    assert indexedpb.shard == indexpb.shard
-    assert indexedpb.txid == indexpb.txid
-    assert indexedpb.typemessage == indexpb.typemessage
-    assert indexedpb.reindex_id == indexpb.reindex_id
+    assert msg.subject == const.PubSubChannels.RESOURCE_NOTIFY.format(kbid="kb")
+    notification = Notification()
+    notification.ParseFromString(msg.data)
+    assert notification.partition == int(indexpb.partition)
+    assert notification.seqid == indexpb.txid
+    assert notification.uuid == indexpb.resource
+    assert notification.kbid == indexpb.kbid
 
 
 def resource_payload(shard: str) -> Resource:
     pb = Resource()
     pb.shard_id = shard
     pb.resource.shard_id = shard
     pb.resource.uuid = "uuid"
@@ -185,43 +153,34 @@
     index.node = node
     index.shard = shard
     return index
 
 
 async def send_indexing_message(worker: Worker, index: IndexMessage, node: str):
     # Push on stream
-    assert indexing_settings.index_jetstream_target is not None
     await worker.js.publish(
-        indexing_settings.index_jetstream_target.format(node=node),
+        const.Streams.INDEX.subject.format(node=node),
         index.SerializeToString(),
     )
 
 
-async def get_indexed_message(natsd):
-    nc = await nats.connect(servers=[natsd])
-    future = asyncio.Future()
+async def wait_for_indexed_message(kbid: str):
+    pubsub = await get_pubsub()
+    future = asyncio.Future()  # type: ignore
+    request_id = str(uuid.uuid4())
 
     async def cb(msg):
         nonlocal future
         future.set_result(msg)
 
-    js = nc.jetstream()
-    await js.subscribe(
-        stream=indexing_settings.indexed_jetstream_stream,
-        subject=indexing_settings.indexed_jetstream_target.format(
-            partition=TEST_PARTITION
-        ),
-        queue="indexed-{partition}".format(partition=TEST_PARTITION),
-        cb=cb,
-        config=nats.js.api.ConsumerConfig(
-            deliver_policy=nats.js.api.DeliverPolicy.NEW,
-        ),
+    await pubsub.subscribe(
+        handler=cb,
+        key=const.PubSubChannels.RESOURCE_NOTIFY.format(kbid=kbid),
+        subscription_id=request_id,
     )
     msg = None
     try:
-        msg = await asyncio.wait_for(future, 1)
+        msg = await asyncio.wait_for(future, 10)
     except TimeoutError:  # pragma: no cover
         pass
     finally:
-        await nc.flush()
-        await nc.close()
         return msg
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_sidecar_servicer.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/fastapi/test_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,29 +12,45 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
+from unittest.mock import AsyncMock
 
 import pytest
-from nucliadb_protos.noderesources_pb2 import EmptyQuery, ShardId
-from nucliadb_protos.nodesidecar_pb2_grpc import NodeSidecarStub
+from fastapi import FastAPI
+
+from nucliadb_telemetry import context
+from nucliadb_telemetry.fastapi.context import ContextInjectorMiddleware
+
+app = FastAPI()
+
+
+@app.get("/api/v1/kb/{kbid}")
+def get_kb(kbid: str):
+    return {"kbid": kbid}
 
 
 @pytest.mark.asyncio
-async def test_create_delete_shadow_shards(
-    sidecar_stub: NodeSidecarStub, shadow_folder: str
-):
-    # Create a shadow shard
-    response = await sidecar_stub.CreateShadowShard(EmptyQuery())  # type: ignore
-    assert response.success
-
-    # Delete now
-    sipb = ShardId(id=response.shard.id)
-    response = await sidecar_stub.DeleteShadowShard(sipb)  # type: ignore
-    assert response.success
-
-    # Deleting again should succed (not found)
-    response = await sidecar_stub.DeleteShadowShard(sipb)  # type: ignore
-    assert response.success
+async def test_context_injected():
+    scope = {
+        "app": app,
+        "path": "/api/v1/kb/123",
+        "method": "GET",
+        "type": "http",
+    }
+
+    mdlw = ContextInjectorMiddleware(app)
+
+    found_ctx = {}
+
+    async def receive(*args, **kwargs):
+        found_ctx.update(context.get_context())
+        return {
+            "type": "http.disconnect",
+        }
+
+    await mdlw(scope, receive, AsyncMock())
+
+    assert found_ctx == {"kbid": "123"}
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,156 +15,117 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 import tempfile
 from unittest import mock
-from unittest.mock import AsyncMock, Mock
+from unittest.mock import AsyncMock, MagicMock, Mock
 
-import nats as natslib
 import pytest
 from nats.aio.client import Msg
 from nucliadb_protos.nodewriter_pb2 import IndexMessage, TypeMessage
+from nucliadb_utils import const
 
 from nucliadb_node.pull import IndexedPublisher, Worker
 from nucliadb_node.settings import settings
 
 
+@pytest.fixture(autouse=True)
+def pubsub():
+    pubsub = AsyncMock()
+    with mock.patch("nucliadb_node.pull.get_pubsub", return_value=pubsub):
+        yield pubsub
+
+
 class NatsConnectionTest:
     def __init__(self):
         self.js = AsyncMock()
         self.jetstream = Mock(return_value=self.js)
         self.close = AsyncMock()
         self.flush = AsyncMock()
 
 
 class NatsTest:
     def __init__(self, connection):
         self.connect = AsyncMock(return_value=connection)
 
 
 class TestIndexedPublisher:
-    stream = "stream"
-    target = "target.{partition}"
-    auth = "token"
-    servers = ["nats://localhost:4222"]
-
     @pytest.fixture(scope="function")
-    def publisher(self, nats_mock):
-        return IndexedPublisher(self.stream, self.target, self.servers, self.auth)
+    async def publisher(self):
+        pub = IndexedPublisher()
+        await pub.initialize()
+        yield pub
 
     @pytest.fixture(scope="function")
     def index_message(self):
         delpb = IndexMessage()
         delpb.node = "node"
         delpb.typemessage = TypeMessage.DELETION
         delpb.partition = "11"
         delpb.resource = "rid"
+        delpb.kbid = "kbid"
         return delpb
 
-    @pytest.fixture(scope="function")
-    def nats_connection(self):
-        return NatsConnectionTest()
-
-    @pytest.fixture(scope="function")
-    def nats_mock(self, nats_connection):
-        nats_test = NatsTest(nats_connection)
-        with mock.patch("nucliadb_node.pull.nats", nats_test):
-            yield nats_test
-
-    @pytest.mark.asyncio
-    async def test_initialize(self, nats_mock, nats_connection, publisher):
-        await publisher.initialize()
-
-        nats_mock.connect.assert_called_once_with(
-            **{
-                "closed_cb": publisher.on_connection_closed,
-                "reconnected_cb": publisher.on_reconnection,
-                "user_credentials": self.auth,
-                "servers": self.servers,
-            }
-        )
-        assert publisher.nc == nats_connection
-        assert publisher.js == nats_connection.js
-
     @pytest.mark.asyncio
-    async def test_initialize_creates_stream_if_not_found(
-        self, nats_connection, publisher
-    ):
-        nats_connection.js.stream_info.side_effect = [
-            natslib.js.errors.NotFoundError,
-            None,
-        ]
-        await publisher.initialize()
-
-        nats_connection.js.add_stream.assert_awaited_once()
+    async def test_initialize(self, publisher, pubsub):
+        assert publisher.pubsub == pubsub
 
     @pytest.mark.asyncio
-    async def test_initialize_creates_stream_only_if_not_found(
-        self, nats_connection, publisher
-    ):
-        nats_connection.js.stream_info.return_value = None
-        await publisher.initialize()
-
-        nats_connection.js.add_stream.assert_not_awaited()
-
-    @pytest.mark.asyncio
-    async def test_finalize(self, nats_connection, publisher):
-        await publisher.initialize()
-        await publisher.finalize()
+    async def test_finalize(self, publisher, pubsub):
         await publisher.finalize()
 
-        nats_connection.flush.assert_awaited_once()
-        nats_connection.close.assert_awaited_once()
+        pubsub.finalize.assert_awaited_once()
 
     @pytest.mark.asyncio
-    async def test_indexed(self, nats_connection, publisher, index_message):
-        await publisher.initialize()
-
+    async def test_indexed(self, publisher, index_message, pubsub):
         await publisher.indexed(index_message)
 
-        subject = self.target.format(partition=index_message.partition)
-        nats_connection.js.publish.assert_awaited_once()
-        assert nats_connection.js.publish.call_args[0][0] == subject
+        channel = const.PubSubChannels.RESOURCE_NOTIFY.format(kbid=index_message.kbid)
+        pubsub.publish.assert_awaited_once()
+        assert pubsub.publish.call_args[0][0] == channel
 
     @pytest.mark.asyncio
     async def test_indexed_skips_if_no_partition(
-        self, nats_connection, publisher, index_message
+        self, publisher, index_message, pubsub
     ):
-        await publisher.initialize()
         index_message.ClearField("partition")
 
         await publisher.indexed(index_message)
 
-        nats_connection.js.publish.assert_not_awaited()
-
-    @pytest.mark.asyncio
-    async def test_indexed_errors_if_not_initialized(self, publisher, index_message):
-        publisher.js = None
-        with pytest.raises(RuntimeError):
-            await publisher.indexed(index_message)
+        pubsub.publish.assert_not_awaited()
 
 
-class TestSubsciptionWorker:
+class TestSubscriptionWorker:
     @pytest.fixture(scope="function")
     def settings(self):
         previous = settings.data_path
         with tempfile.TemporaryDirectory() as td:
             settings.data_path = str(td)
             yield
         settings.data_path = previous
 
+    @pytest.fixture()
+    def nats_conn(self):
+        conn = MagicMock()
+        conn.jetstream.return_value = AsyncMock()
+        conn.drain = AsyncMock()
+        conn.close = AsyncMock()
+        with mock.patch("nucliadb_node.pull.nats.connect", return_value=conn):
+            yield conn
+
     @pytest.fixture(scope="function")
-    def worker(self, settings):
+    def worker(self, settings, nats_conn):
         writer = AsyncMock()
         reader = AsyncMock()
-        worker = Worker(writer, reader, "node")
-        worker.store_seqid = Mock()
-        yield worker
+        with mock.patch("nucliadb_node.pull.get_storage"):
+            worker = Worker(writer, reader, "node")
+            worker.store_seqid = Mock()
+            yield worker
 
     def get_msg(self, seqid):
         client = AsyncMock()
         reply = f"foo.bar.ba.blan.ca.{seqid}.bar"
         msg = Msg(client, "subject", reply)
         msg.ack = AsyncMock()
         return msg
@@ -174,7 +135,14 @@
         worker.last_seqid = 10
         msg = self.get_msg(seqid=9)
         await worker.subscription_worker(msg)
 
         # The message is acked and ignored
         msg.ack.assert_awaited_once()
         worker.store_seqid.assert_not_called()
+
+    @pytest.mark.asyncio
+    async def test_reconnected_cb(self, worker: Worker):
+        await worker.initialize()
+        await worker.reconnected_cb()
+
+        assert worker.nc.jetstream().subscribe.call_count == 2
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 
 setup(
     name="nucliadb_node",
     version=VERSION,
     long_description=README,
     classifiers=[
         "Development Status :: 4 - Beta",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     url="https://nuclia.com",
     license="BSD",
     setup_requires=[
         "pytest-runner",
     ],
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/bin/payload_test.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/bin/payload_test.rs`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
 use nucliadb_core::protos::*;
 use nucliadb_node::reader::NodeReaderService;
 use nucliadb_node::writer::NodeWriterService;
 use prost::Message;
 
 fn main() -> anyhow::Result<()> {
-    let mut writer = NodeWriterService::new();
+    let writer = NodeWriterService::new();
     let reader = NodeReaderService::new();
 
     let resources_dir = std::path::Path::new("/path/to/data");
-    let new_shard = writer.new_shard(&NewShardRequest::default())?;
+    let new_shard = NodeWriterService::new_shard(&NewShardRequest::default())?;
     let shard_id = ShardId { id: new_shard.id };
     assert!(resources_dir.exists());
     for file_path in std::fs::read_dir(resources_dir).unwrap() {
         let file_path = file_path.unwrap().path();
         println!("processing {file_path:?}");
         let content = std::fs::read(&file_path).unwrap();
         let resource = Resource::decode(&mut Cursor::new(content)).unwrap();
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files 19% similar despite different names*

```diff
@@ -15,41 +15,48 @@
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 use std::time::Instant;
 
+use nucliadb_core::metrics::middleware::MetricsLayer;
 use nucliadb_core::protos::node_reader_server::NodeReaderServer;
 use nucliadb_core::tracing::*;
 use nucliadb_core::NodeResult;
 use nucliadb_node::env;
 use nucliadb_node::http_server::{run_http_metrics_server, MetricsServerOptions};
-use nucliadb_node::reader::grpc_driver::NodeReaderGRPCDriver;
-use nucliadb_node::reader::NodeReaderService;
+use nucliadb_node::middleware::{GrpcDebugLogsLayer, GrpcInstrumentorLayer};
+use nucliadb_node::reader::grpc_driver::{GrpcReaderOptions, NodeReaderGRPCDriver};
+use nucliadb_node::shards::{AsyncReaderShardsProvider, AsyncUnboundedShardReaderCache};
 use nucliadb_node::telemetry::init_telemetry;
 use tokio::signal::unix::SignalKind;
 use tokio::signal::{ctrl_c, unix};
 use tonic::transport::Server;
 
 type GrpcServer = NodeReaderServer<NodeReaderGRPCDriver>;
 
 #[tokio::main]
 async fn main() -> Result<(), Box<dyn std::error::Error>> {
     eprintln!("NucliaDB Reader Node starting...");
     let _guard = init_telemetry()?;
     let start_bootstrap = Instant::now();
-    let mut node_reader_service = NodeReaderService::new();
+    let shards_provider = AsyncUnboundedShardReaderCache::new();
 
     std::fs::create_dir_all(env::shards_path())?;
     if !env::lazy_loading() {
-        node_reader_service.load_shards()?;
+        shards_provider.load_all().await?;
     }
 
-    let grpc_driver = NodeReaderGRPCDriver::from(node_reader_service);
+    let grpc_options = GrpcReaderOptions {
+        lazy_loading: env::lazy_loading(),
+    };
+    let grpc_driver = NodeReaderGRPCDriver::new(grpc_options);
+    grpc_driver.initialize().await?;
+
     let _grpc_task = tokio::spawn(start_grpc_service(grpc_driver));
     let metrics_task = tokio::spawn(run_http_metrics_server(MetricsServerOptions {
         default_http_port: 3031,
     }));
 
     info!("Bootstrap complete in: {:?}", start_bootstrap.elapsed());
     eprintln!("Running");
@@ -78,18 +85,24 @@
 }
 
 pub async fn start_grpc_service(grpc_driver: NodeReaderGRPCDriver) {
     let addr = env::reader_listen_address();
 
     info!("Reader listening for gRPC requests at: {:?}", addr);
 
-    let (mut health_reporter, health_service) = tonic_health::server::health_reporter();
+    let tracing_middleware = GrpcInstrumentorLayer::default();
+    let debug_logs_middleware = GrpcDebugLogsLayer::default();
+    let metrics_middleware = MetricsLayer::default();
 
+    let (mut health_reporter, health_service) = tonic_health::server::health_reporter();
     health_reporter.set_serving::<GrpcServer>().await;
 
     Server::builder()
+        .layer(tracing_middleware)
+        .layer(debug_logs_middleware)
+        .layer(metrics_middleware)
         .add_service(health_service)
         .add_service(GrpcServer::new(grpc_driver))
         .serve(addr)
         .await
         .expect("Error starting gRPC reader");
 }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -23,48 +23,47 @@
 use std::path::{Path, PathBuf};
 use std::str::FromStr;
 use std::time::Instant;
 
 use anyhow::{Context, Result};
 use futures::Stream;
 use nucliadb_cluster::{node, Key, Node, NodeHandle, NodeType};
+use nucliadb_core::metrics::middleware::MetricsLayer;
 use nucliadb_core::protos::node_writer_server::NodeWriterServer;
 use nucliadb_core::tracing::*;
-use nucliadb_core::NodeResult;
+use nucliadb_core::{metrics, NodeResult};
 use nucliadb_node::env;
 use nucliadb_node::http_server::{run_http_metrics_server, MetricsServerOptions};
+use nucliadb_node::middleware::{GrpcDebugLogsLayer, GrpcInstrumentorLayer};
 use nucliadb_node::node_metadata::NodeMetadata;
 use nucliadb_node::telemetry::init_telemetry;
 use nucliadb_node::writer::grpc_driver::{NodeWriterEvent, NodeWriterGRPCDriver};
 use nucliadb_node::writer::NodeWriterService;
 use tokio::signal::unix::SignalKind;
 use tokio::signal::{ctrl_c, unix};
 use tokio::sync::mpsc::{UnboundedReceiver, UnboundedSender};
 use tokio_stream::StreamExt;
 use tonic::transport::Server;
 use uuid::Uuid;
 
-const LOAD_SCORE_KEY: Key<f32> = Key::new("load_score");
 const SHARD_COUNT_KEY: Key<u64> = Key::new("shard_count");
 
 type GrpcServer = NodeWriterServer<NodeWriterGRPCDriver>;
 
 #[derive(Debug)]
 pub enum NodeUpdate {
     ShardCount(u64),
-    LoadScore(f32),
 }
 
 #[tokio::main]
 async fn main() -> NodeResult<()> {
     eprintln!("NucliaDB Writer Node starting...");
-    let _guard = init_telemetry()?;
-
     let start_bootstrap = Instant::now();
-
+    let _guard = init_telemetry()?;
+    let metrics = metrics::get_metrics();
     let metadata_path = env::metadata_path();
     let node_metadata = NodeMetadata::load_or_create(&metadata_path)?;
     let mut node_writer_service = NodeWriterService::new();
 
     std::fs::create_dir_all(env::shards_path())?;
     if !env::lazy_loading() {
         node_writer_service.load_shards()?;
@@ -84,32 +83,49 @@
     // Cluster
     let host_key = read_or_create_host_key(Path::new(&host_key_path))?;
     let node = Node::builder()
         .register_as(NodeType::Io)
         .on_local_network(chitchat_addr)
         .with_id(host_key.to_string())
         .with_seed_nodes(seed_nodes)
-        .insert_to_initial_state(LOAD_SCORE_KEY, node_metadata.load_score())
         .insert_to_initial_state(SHARD_COUNT_KEY, node_metadata.shard_count())
         .build()?;
     let node = node.start().await?;
     let cluster_watcher = node.cluster_watcher().await;
     let update_handle = node.clone();
 
     nucliadb_telemetry::sync::start_telemetry_loop();
 
     tokio::spawn(start_grpc_service(grpc_driver));
-    tokio::spawn(update_node_metadata(
-        update_sender,
-        metadata_receiver,
-        node_metadata,
-        metadata_path,
-    ));
+    {
+        let task = update_node_metadata(
+            update_sender,
+            metadata_receiver,
+            node_metadata,
+            metadata_path,
+        );
+        match metrics.task_monitor("UpdateNodeMetadata".to_string()) {
+            Some(monitor) => {
+                let instrumented = monitor.instrument(task);
+                tokio::spawn(instrumented)
+            }
+            None => tokio::spawn(task),
+        };
+    }
     let update_task = tokio::spawn(update_node_state(update_handle, update_receiver));
-    let monitor_task = tokio::spawn(monitor_cluster(cluster_watcher));
+    let monitor_task = {
+        let task = monitor_cluster(cluster_watcher);
+        match metrics.task_monitor("ClusterMonitor".to_string()) {
+            Some(monitor) => {
+                let instrumented = monitor.instrument(task);
+                tokio::spawn(instrumented)
+            }
+            None => tokio::spawn(task),
+        }
+    };
     let metrics_task = tokio::spawn(run_http_metrics_server(MetricsServerOptions {
         default_http_port: 3032,
     }));
 
     info!("Bootstrap complete in: {:?}", start_bootstrap.elapsed());
     eprintln!("Running");
 
@@ -145,19 +161,25 @@
 }
 
 pub async fn start_grpc_service(grpc_driver: NodeWriterGRPCDriver) {
     let addr = env::writer_listen_address();
 
     info!("Listening for gRPC requests at: {:?}", addr);
 
-    let (mut health_reporter, health_service) = tonic_health::server::health_reporter();
+    let tracing_middleware = GrpcInstrumentorLayer::default();
+    let debug_logs_middleware = GrpcDebugLogsLayer::default();
+    let metrics_middleware = MetricsLayer::default();
 
+    let (mut health_reporter, health_service) = tonic_health::server::health_reporter();
     health_reporter.set_serving::<GrpcServer>().await;
 
     Server::builder()
+        .layer(tracing_middleware)
+        .layer(debug_logs_middleware)
+        .layer(metrics_middleware)
         .add_service(health_service)
         .add_service(GrpcServer::new(grpc_driver))
         .serve(addr)
         .await
         .expect("Error starting gRPC service");
 }
 
@@ -185,17 +207,14 @@
     info!("Start node update task");
 
     while let Some(event) = metadata_receiver.recv().await {
         info!("Receive node update event: {event:?}");
 
         match event {
             NodeUpdate::ShardCount(count) => node.update_state(SHARD_COUNT_KEY, count).await,
-            NodeUpdate::LoadScore(load_score) => {
-                node.update_state(LOAD_SCORE_KEY, load_score).await
-            }
         }
     }
 }
 
 pub async fn update_node_metadata(
     update_sender: UnboundedSender<NodeUpdate>,
     mut metadata_receiver: UnboundedReceiver<NodeWriterEvent>,
@@ -204,29 +223,21 @@
 ) {
     info!("Start node update task");
 
     while let Some(event) = metadata_receiver.recv().await {
         debug!("Receive metadata update event: {event:?}");
 
         let result = match event {
-            NodeWriterEvent::ShardCreation(id, knowledge_box) => {
-                node_metadata.new_shard(id, knowledge_box, 0.0);
+            NodeWriterEvent::ShardCreation => {
+                node_metadata.new_shard();
                 update_sender.send(NodeUpdate::ShardCount(node_metadata.shard_count()))
             }
-            NodeWriterEvent::ShardDeletion(id) => {
-                node_metadata.delete_shard(id);
-                update_sender
-                    .send(NodeUpdate::ShardCount(node_metadata.shard_count()))
-                    .and_then(|_| {
-                        update_sender.send(NodeUpdate::LoadScore(node_metadata.load_score()))
-                    })
-            }
-            NodeWriterEvent::ParagraphCount(id, paragraph_count) => {
-                node_metadata.update_shard(id, paragraph_count);
-                update_sender.send(NodeUpdate::LoadScore(node_metadata.load_score()))
+            NodeWriterEvent::ShardDeletion => {
+                node_metadata.delete_shard();
+                update_sender.send(NodeUpdate::ShardCount(node_metadata.shard_count()))
             }
         };
 
         if let Err(e) = result {
             warn!("Cannot send node update: {e:?}");
         }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/env.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/env.rs`

 * *Files 3% similar despite different names*

```diff
@@ -200,24 +200,29 @@
             }
         },
         Err(_) => default,
     }
 }
 
 pub fn log_level() -> Vec<(String, Level)> {
-    let default = "nucliadb_node=WARN,nucliadb_cluster=WARN,nucliadb_cluster=WARN".to_string();
+    let default = "nucliadb_node=WARN,nucliadb_cluster=WARN".to_string();
     match env::var("RUST_LOG") {
         Ok(levels) => parse_log_level(&levels),
         Err(_) => {
             error!("RUST_LOG not defined. Defaulting to {default}");
             parse_log_level(&default)
         }
     }
 }
 
+pub fn span_levels() -> Vec<(String, Level)> {
+    let default = "nucliadb_node=INFO,nucliadb_cluster=INFO,nucliadb_core=INFO".to_string();
+    parse_log_level(&default)
+}
+
 pub fn get_sentry_env() -> &'static str {
     let default = SENTRY_DEV;
     match env::var("RUNNING_ENVIRONMENT") {
         Ok(sentry_env) if sentry_env.eq("prod") => SENTRY_PROD,
         Ok(sentry_env) if sentry_env.eq("stage") => SENTRY_DEV,
         Ok(_) => {
             error!("RUNNING_ENVIRONMENT defined incorrectly. Defaulting to {default}");
@@ -289,7 +294,22 @@
                 error!("METRICS_HTTP_PORT defined incorrectly. Defaulting to {default}");
                 default
             }
         }
         Err(_) => default,
     }
 }
+
+pub fn max_shards_per_node() -> usize {
+    let default = 800;
+    match env::var("MAX_NODE_REPLICAS") {
+        Ok(max_shards) => {
+            if let Ok(max_shards) = max_shards.parse() {
+                max_shards
+            } else {
+                error!("MAX_NODE_REPLICAS defined incorrectly. Using default: {default}");
+                default
+            }
+        }
+        Err(_) => default,
+    }
+}
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
-use nucliadb_core::{context, tracing};
+use nucliadb_core::{metrics, tracing};
 
 pub async fn metrics_service() -> String {
-    let metrics = context::get_metrics();
-    match metrics.collect() {
+    let metrics = metrics::get_metrics();
+    match metrics.export() {
         Ok(m) => m,
         Err(err) => {
             tracing::error!("Could not collect metrics due to {err:?}");
             Default::default()
         }
     }
 }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -35,9 +35,9 @@
     // Add routes to services
     let addr = SocketAddr::from(([0, 0, 0, 0], metrics_http_port(options.default_http_port)));
     let metrics = Router::new().route("/metrics", get(metrics_service::metrics_service));
     axum_server::bind(addr)
         // Services will be added here
         .serve(metrics.into_make_service())
         .await
-        .expect("Error starting the http server");
+        .expect("Error starting the HTTP server");
 }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 /// Shard metadata, defined at the moment of creation.
 mod shard_metadata;
 
 pub mod node_metadata;
 
 pub mod services;
 
+pub mod middleware;
+
+pub mod shards;
+
 /// Global configuration enviromental variables
 pub mod env;
 
 /// GRPC reading service
 pub mod reader;
 
 /// Utilities
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/reader/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/reader/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 pub mod grpc_driver;
 use std::collections::HashMap;
 
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::{
     DocumentSearchRequest, DocumentSearchResponse, EdgeList, GetShardRequest, IdCollection,
     ParagraphSearchRequest, ParagraphSearchResponse, RelationSearchRequest, RelationSearchResponse,
-    SearchRequest, SearchResponse, Shard as ShardPB, ShardId, ShardList, StreamRequest,
-    SuggestRequest, SuggestResponse, TypeList, VectorSearchRequest, VectorSearchResponse,
+    SearchRequest, SearchResponse, Shard as ShardPB, ShardId, StreamRequest, SuggestRequest,
+    SuggestResponse, TypeList, VectorSearchRequest, VectorSearchResponse,
 };
 use nucliadb_core::thread::*;
 use nucliadb_core::tracing::{self, *};
 
 use crate::env;
 use crate::services::reader::ShardReaderService;
 
@@ -51,25 +51,14 @@
     pub fn shutdown(&mut self) {
         for (shard_id, shard) in &mut self.cache {
             debug!("Stopping shard {}", shard_id);
             ShardReaderService::stop(shard);
         }
     }
 
-    #[tracing::instrument(skip_all)]
-    pub fn iter_shards(&self) -> NodeResult<impl Iterator<Item = NodeResult<ShardReaderService>>> {
-        let shards_path = env::shards_path();
-        Ok(std::fs::read_dir(shards_path)?.flatten().map(|entry| {
-            let file_name = entry.file_name().to_str().unwrap().to_string();
-            let shard_path = entry.path();
-            debug!("Opening {shard_path:?}");
-            ShardReaderService::new(file_name, &shard_path)
-        }))
-    }
-
     /// Load all shards on the shards memory structure
     #[tracing::instrument(skip_all)]
     pub fn load_shards(&mut self) -> NodeResult<()> {
         let shards_path = env::shards_path();
         debug!("Recovering shards from {shards_path:?}...");
         for entry in std::fs::read_dir(&shards_path)? {
             let entry = entry?;
@@ -95,48 +84,28 @@
             debug!("Shard {shard_path:?} is already on memory");
             return;
         }
         if !shard_path.is_dir() {
             error!("Shard {shard_path:?} is not on disk");
             return;
         }
-        let Ok(shard) = ShardReaderService::new(shard_name, &shard_path) else {
-            error!("Shard {shard_path:?} could not be loaded from disk");
-            return;
-        };
-        self.cache.insert(shard_id.id.clone(), shard);
-        debug!("{shard_path:?}: Shard loaded");
+        match ShardReaderService::new(shard_name, &shard_path) {
+            Err(err) => error!("Shard {shard_path:?} could not be loaded from disk: {err:?}"),
+            Ok(shard) => {
+                self.cache.insert(shard_id.id.clone(), shard);
+                debug!("{shard_path:?}: Shard loaded");
+            }
+        }
     }
 
     #[tracing::instrument(skip_all)]
     pub fn get_shard(&self, shard_id: &ShardId) -> Option<&ShardReaderService> {
         self.cache.get(&shard_id.id)
     }
-    #[tracing::instrument(skip_all)]
-    pub fn get_shards(&self) -> NodeResult<ShardList> {
-        use crate::telemetry::run_with_telemetry;
-        let span = tracing::Span::current();
-        let task = move |shard_id: &str, shard: &ShardReaderService| {
-            run_with_telemetry(info_span!(parent: &span, "get shards"), || {
-                shard.get_resources().map(|count| ShardPB {
-                    metadata: Some(shard.metadata.clone().into()),
-                    shard_id: shard_id.to_string(),
-                    resources: count as u64,
-                    paragraphs: 0_u64,
-                    sentences: 0_u64,
-                })
-            })
-        };
-        let shards = self
-            .cache
-            .par_iter()
-            .map(|(id, shard)| task(id, shard))
-            .collect::<Result<Vec<_>, _>>()?;
-        Ok(ShardList { shards })
-    }
+
     #[tracing::instrument(skip_all)]
     pub fn suggest(
         &self,
         shard_id: &ShardId,
         request: SuggestRequest,
     ) -> NodeResult<Option<SuggestResponse>> {
         let Some(shard) = self.get_shard(shard_id) else {
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/services/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/services/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/services/reader.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/services/reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 use std::path::Path;
 use std::sync::RwLock;
 use std::time::SystemTime;
 
-use nucliadb_core::context;
-use nucliadb_core::metrics::request_time;
+use nucliadb_core::metrics::{self, request_time};
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::shard_created::{
     DocumentService, ParagraphService, RelationService, VectorService,
 };
 use nucliadb_core::protos::{
     DocumentSearchRequest, DocumentSearchResponse, EdgeList, GetShardRequest,
     ParagraphSearchRequest, ParagraphSearchResponse, RelatedEntities, RelationPrefixSearchRequest,
@@ -115,15 +114,15 @@
         let mut vector_result = Ok(0);
         thread::scope(|s| {
             s.spawn(|_| text_result = text_task());
             s.spawn(|_| paragraph_result = paragraph_task());
             s.spawn(|_| vector_result = vector_task());
         });
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("reader/get_info".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(Shard {
             metadata: Some(self.metadata.clone().into()),
             shard_id: self.id.clone(),
@@ -160,18 +159,14 @@
         self.relation_reader.get_edges()
     }
     #[tracing::instrument(skip_all)]
     pub fn get_relations_types(&self) -> NodeResult<TypeList> {
         self.reload_policy(true);
         self.relation_reader.get_node_types()
     }
-    #[tracing::instrument(skip_all)]
-    pub fn get_resources(&self) -> NodeResult<usize> {
-        self.text_reader.count()
-    }
 
     #[tracing::instrument(skip_all)]
     pub fn new(id: String, shard_path: &Path) -> NodeResult<ShardReaderService> {
         let span = tracing::Span::current();
         let time = SystemTime::now();
 
         let metadata = ShardMetadata::open(&shard_path.join(METADATA_FILE))?;
@@ -218,15 +213,15 @@
             s.spawn(|_| relation_result = relation_task());
         });
         let fields = text_result.transpose()?;
         let paragraphs = paragraph_result.transpose()?;
         let vectors = vector_result.transpose()?;
         let relations = relation_result.transpose()?;
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("reader/new".to_string());
         metrics.record_request_time(metric, took);
         Ok(ShardReaderService {
             id,
             metadata,
             text_reader: fields.unwrap(),
@@ -286,15 +281,15 @@
         if let Err(e) = vector_result {
             error!("Error stopping the Vector reader service: {}", e);
         }
         if let Err(e) = relation_result {
             error!("Error stopping the Relation reader service: {}", e);
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("reader/stop".to_string());
         metrics.record_request_time(metric, took);
 
         debug!("Shard stopped {}...", { &self.id });
     }
 
@@ -367,15 +362,15 @@
                     .nodes
                     .iter()
                     .map(|relation_node| relation_node.value.clone())
                     .collect::<Vec<String>>()
             })
             .collect::<Vec<String>>();
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("reader/suggest".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(SuggestResponse {
             query: rparagraph.query,
             total: rparagraph.total,
@@ -433,14 +428,15 @@
             faceted: search_request.faceted.clone(),
             page_number: search_request.page_number,
             result_per_page: search_request.result_per_page,
             timestamps: search_request.timestamps.clone(),
             reload: search_request.reload,
             only_faceted: search_request.only_faceted,
             advanced_query: search_request.advanced_query.clone(),
+            key_filters: search_request.key_filters.clone(),
         };
         let paragraph_reader_service = self.paragraph_reader.clone();
         let paragraph_task = move || {
             if !skip_paragraphs {
                 Some(paragraph_reader_service.search(&paragraph_request))
             } else {
                 None
@@ -451,20 +447,22 @@
             id: "".to_string(),
             vector_set: search_request.vectorset.clone(),
             vector: search_request.vector.clone(),
             reload: search_request.reload,
             page_number: search_request.page_number,
             result_per_page: search_request.result_per_page,
             with_duplicates: true,
+            key_filters: search_request.key_filters.clone(),
             tags: search_request
                 .filter
                 .iter()
                 .flat_map(|f| f.tags.iter().cloned())
                 .chain(search_request.fields.iter().cloned())
                 .collect(),
+            min_score: search_request.min_score,
         };
         let vector_reader_service = self.vector_reader.clone();
         let vector_task = move || {
             if !skip_vectors {
                 Some(vector_reader_service.search(&vector_request))
             } else {
                 None
@@ -497,15 +495,15 @@
         thread::scope(|s| {
             s.spawn(|_| rtext = text_task());
             s.spawn(|_| rparagraph = paragraph_task());
             s.spawn(|_| rvector = vector_task());
             s.spawn(|_| rrelation = relation_task());
         });
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("reader/search".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(SearchResponse {
             document: rtext.transpose()?,
             paragraph: rparagraph.transpose()?,
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/services/versions.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/services/versions.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/services/writer.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/services/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     DocumentService, ParagraphService, RelationService, VectorService,
 };
 use nucliadb_core::protos::{
     DeleteGraphNodes, JoinGraph, NewShardRequest, OpStatus, Resource, ResourceId, VectorSetId,
     VectorSimilarity,
 };
 use nucliadb_core::tracing::{self, *};
-use nucliadb_core::{context, thread};
+use nucliadb_core::{metrics, thread};
 
 use super::shard_disk_structure::*;
 use crate::services::versions::Versions;
 use crate::shard_metadata::ShardMetadata;
 use crate::telemetry::run_with_telemetry;
 
 #[derive(Debug)]
@@ -191,15 +191,15 @@
         };
         let rsc = RelationConfig {
             path: path.join(RELATIONS_DIR),
         };
 
         metadata.serialize(&metadata_path)?;
         let result = ShardWriterService::initialize(id, path, metadata, tsc, psc, vsc, rsc);
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("writer/new".to_string());
         metrics.record_request_time(metric, took);
 
         result
     }
 
@@ -222,15 +222,15 @@
             path: path.join(VECTORS_DIR),
             vectorset: path.join(VECTORSET_DIR),
         };
         let rsc = RelationConfig {
             path: path.join(RELATIONS_DIR),
         };
         let result = ShardWriterService::initialize(id, path, metadata, tsc, psc, vsc, rsc);
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("writer/open".to_string());
         metrics.record_request_time(metric, took);
 
         result
     }
 
@@ -279,15 +279,15 @@
         if let Err(e) = vector_result {
             error!("Error stopping the Vector writer service: {}", e);
         }
         if let Err(e) = relation_result {
             error!("Error stopping the Relation writer service: {}", e);
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("writer/stop".to_string());
         metrics.record_request_time(metric, took);
 
         debug!("Shard stopped {}...", { &self.id });
     }
 
@@ -352,15 +352,15 @@
         thread::scope(|s| {
             s.spawn(|_| text_result = text_task());
             s.spawn(|_| paragraph_result = paragraph_task());
             s.spawn(|_| vector_result = vector_task());
             s.spawn(|_| relation_result = relation_task());
         });
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("writer/set_resource".to_string());
         metrics.record_request_time(metric, took);
 
         text_result?;
         paragraph_result?;
         vector_result?;
@@ -413,15 +413,15 @@
         thread::scope(|s| {
             s.spawn(|_| text_result = text_task());
             s.spawn(|_| paragraph_result = paragraph_task());
             s.spawn(|_| vector_result = vector_task());
             s.spawn(|_| relation_result = relation_task());
         });
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("writer/remove_resource".to_string());
         metrics.record_request_time(metric, took);
 
         text_result?;
         paragraph_result?;
         vector_result?;
@@ -450,15 +450,15 @@
         let mut vector_result = Ok(0);
         thread::scope(|s| {
             s.spawn(|_| text_result = text_task());
             s.spawn(|_| paragraph_result = paragraph_task());
             s.spawn(|_| vector_result = vector_task());
         });
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::shard("writer/get_opstatus".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(OpStatus {
             shard_id: self.id.clone(),
             count: text_result? as u64,
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/shard_metadata.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shard_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files 24% similar despite different names*

```diff
@@ -19,89 +19,102 @@
 
 use nucliadb_core::tracing::{Level, Span};
 use nucliadb_core::{Context, NodeResult};
 use opentelemetry::global;
 use opentelemetry::trace::TraceContextExt;
 use sentry::ClientInitGuard;
 use tracing_opentelemetry::OpenTelemetrySpanExt;
-use tracing_subscriber::filter::{FilterFn, Targets};
+use tracing_subscriber::filter::{FilterFn, LevelFilter, Targets};
 use tracing_subscriber::layer::SubscriberExt;
 use tracing_subscriber::util::SubscriberInitExt;
 use tracing_subscriber::{Layer, Registry};
 
 use crate::env;
 
 const TRACE_ID: &str = "trace-id";
 
 pub fn init_telemetry() -> NodeResult<ClientInitGuard> {
-    let log_levels = env::log_level();
-
     let mut layers = Vec::new();
 
+    let log_levels = env::log_level();
+    let stdout = stdout_layer(log_levels);
+    layers.push(stdout);
+
     if env::jaeger_enabled() {
-        layers.push(init_jaeger(log_levels.clone())?);
+        let span_levels = env::span_levels();
+        let jaeger = jaeger_layer(span_levels)?;
+        layers.push(jaeger);
     }
 
-    let stdout_layer = tracing_subscriber::fmt::layer()
-        .with_level(true)
-        .with_filter(Targets::new().with_targets(log_levels))
-        .boxed();
-
-    layers.push(stdout_layer);
-
-    let sentry_env = env::get_sentry_env();
-    let guard = sentry::init((
-        env::sentry_url(),
-        sentry::ClientOptions {
-            release: sentry::release_name!(),
-            environment: Some(sentry_env.into()),
-            ..Default::default()
-        },
-    ));
-    layers.push(sentry_tracing::layer().boxed());
+    let sentry_guard = setup_sentry(env::get_sentry_env(), env::sentry_url());
+    let sentry = sentry_layer();
+    layers.push(sentry);
 
     tracing_subscriber::registry()
         .with(layers)
         .try_init()
         .with_context(|| "trying to init tracing")?;
-    Ok(guard)
+
+    Ok(sentry_guard)
 }
 
-pub(crate) fn run_with_telemetry<F, R>(current: Span, f: F) -> R
-where F: FnOnce() -> R {
-    let tid = current.context().span().span_context().trace_id();
-    sentry::with_scope(|scope| scope.set_tag(TRACE_ID, tid), || current.in_scope(f))
+fn stdout_layer(log_levels: Vec<(String, Level)>) -> Box<dyn Layer<Registry> + Send + Sync> {
+    let format = tracing_subscriber::fmt::format().with_level(true).compact();
+
+    tracing_subscriber::fmt::layer()
+        .event_format(format)
+        .with_filter(Targets::new().with_targets(log_levels))
+        .boxed()
 }
 
-fn init_jaeger(
-    log_levels: Vec<(String, Level)>,
+fn jaeger_layer(
+    _span_levels: Vec<(String, Level)>,
 ) -> NodeResult<Box<dyn Layer<Registry> + Send + Sync>> {
+    global::set_text_map_propagator(opentelemetry_zipkin::Propagator::new());
+
     let agent_endpoint = env::jaeger_agent_endp();
     let tracer = opentelemetry_jaeger::new_pipeline()
         .with_agent_endpoint(agent_endpoint)
         .with_service_name("nucliadb_node")
         .with_auto_split_batch(true)
         .install_batch(opentelemetry::runtime::Tokio)?;
 
-    // This filter is needed because we want to keep logs in stdout and attach logs to jaeger
-    // spans in really rare cases So, basically it checks the source of event (allowed
-    // only from nucliadb_node crate) and filter out all events without special field
-    // For attaching log to jaeger span use this:
-    // tracing::event!(Level::INFO, trace_marker = true, "your logs for jaeger here: {}", foo =
-    // bar);
-    let filter = FilterFn::new(|metadata| {
-        metadata
-            .file()
-            .filter(|file| file.contains("nucliadb_node"))
-            .map(|_| metadata.is_event())
-            .map(|state| state && metadata.fields().field("trace_marker").is_none())
-            .map(|state| !state)
-            .unwrap_or_default()
+    // To avoid sending too much information to Jaeger, we filter out all events
+    // (as they are logged to stdout), spans from external instrumented crates
+    // (like tantivy, hyper, tower, mio...) and spans below INFO level (default
+    // span level).
+    let level_filter = LevelFilter::from_level(Level::INFO);
+    let span_filter = FilterFn::new(|metadata| {
+        metadata.is_span()
+            && metadata
+                .file()
+                .filter(|file| file.contains("nucliadb"))
+                .is_some()
     });
-    global::set_text_map_propagator(opentelemetry_zipkin::Propagator::new());
 
     Ok(tracing_opentelemetry::layer()
         .with_tracer(tracer)
-        .with_filter(Targets::new().with_targets(log_levels))
-        .with_filter(filter)
+        .with_filter(level_filter)
+        .with_filter(span_filter)
         .boxed())
 }
+
+fn setup_sentry(env: &'static str, sentry_url: String) -> ClientInitGuard {
+    sentry::init((
+        sentry_url,
+        sentry::ClientOptions {
+            release: sentry::release_name!(),
+            environment: Some(env.into()),
+            ..Default::default()
+        },
+    ))
+}
+
+fn sentry_layer() -> Box<dyn Layer<Registry> + Send + Sync> {
+    sentry_tracing::layer().boxed()
+}
+
+pub fn run_with_telemetry<F, R>(current: Span, f: F) -> R
+where F: FnOnce() -> R {
+    let tid = current.context().span().span_context().trace_id();
+    sentry::with_scope(|scope| scope.set_tag(TRACE_ID, tid), || current.in_scope(f))
+}
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files 19% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 //
 use std::net::{IpAddr, SocketAddr};
 use std::str::FromStr;
 use std::time::Duration;
 
 use http::Uri;
 use nucliadb_core::tracing::Level;
-use opentelemetry::propagation::Extractor;
 use tokio::net;
 use tokio::time::sleep;
 use tonic::transport::Endpoint;
 
 /// Prepares a socket addr for a grpc endpoint to connect to
 pub fn socket_to_endpoint(grpc_addr: SocketAddr) -> anyhow::Result<Endpoint> {
     let uri = Uri::builder()
@@ -36,36 +35,14 @@
         .path_and_query("/")
         .build()?;
     // Create a channel with connect_lazy to automatically reconnect to the node.
     let channel = Endpoint::from(uri);
     Ok(channel)
 }
 
-/// Metadata mapping
-pub struct MetadataMap<'a>(pub &'a tonic::metadata::MetadataMap);
-
-impl<'a> Extractor for MetadataMap<'a> {
-    /// Gets a value for a key from the MetadataMap.  If the value can't be converted to &str,
-    /// returns None
-    fn get(&self, key: &str) -> Option<&str> {
-        self.0.get(key).and_then(|metadata| metadata.to_str().ok())
-    }
-
-    /// Collect all the keys from the MetadataMap.
-    fn keys(&self) -> Vec<&str> {
-        self.0
-            .keys()
-            .map(|key| match key {
-                tonic::metadata::KeyRef::Ascii(v) => v.as_str(),
-                tonic::metadata::KeyRef::Binary(v) => v.as_str(),
-            })
-            .collect::<Vec<_>>()
-    }
-}
-
 pub async fn reliable_lookup_host(host: &str) -> IpAddr {
     let mut tries = 5;
     while tries != 0 {
         if let Ok(mut addr_iter) = net::lookup_host(host).await {
             if let Some(addr) = addr_iter.next() {
                 return addr.ip();
             }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/src/writer/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/writer/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -66,20 +66,21 @@
     pub fn load_shards(&mut self) -> NodeResult<()> {
         let shards_path = env::shards_path();
         debug!("Recovering shards from {shards_path:?}...");
         for entry in std::fs::read_dir(&shards_path)? {
             let entry = entry?;
             let file_name = entry.file_name().to_str().unwrap().to_string();
             let shard_path = entry.path();
-            let Ok(shard) = ShardWriterService::open(file_name.clone(), &shard_path) else {
-                error!("Shard {shard_path:?} could not be loaded from disk");
-                continue;
-            };
-            self.cache.insert(file_name, shard);
-            debug!("Shard loaded: {shard_path:?}");
+            match ShardWriterService::open(file_name.clone(), &shard_path) {
+                Err(err) => error!("Shard {shard_path:?} could not be loaded from disk: {err:?}"),
+                Ok(shard) => {
+                    debug!("{shard_path:?}: Shard loaded");
+                    self.cache.insert(file_name, shard);
+                }
+            }
         }
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     pub fn load_shard(&mut self, shard_id: &ShardId) {
         let shard_name = shard_id.id.clone();
@@ -88,44 +89,43 @@
             debug!("Shard {shard_path:?} is already on memory");
             return;
         }
         if !shard_path.is_dir() {
             error!("Shard {shard_path:?} is not on disk");
             return;
         }
-        let Ok(shard) = ShardWriterService::open(shard_name, &shard_path) else {
-            error!("Shard {shard_path:?} could not be loaded from disk");
-            return;
-        };
-        self.cache.insert(shard_id.id.clone(), shard);
-        debug!("{shard_path:?}: Shard loaded");
+        match ShardWriterService::open(shard_name, &shard_path) {
+            Err(err) => error!("Shard {shard_path:?} could not be loaded from disk: {err:?}"),
+            Ok(shard) => {
+                self.cache.insert(shard_id.id.clone(), shard);
+                debug!("{shard_path:?}: Shard loaded");
+            }
+        }
     }
     #[tracing::instrument(skip_all)]
     pub fn get_shard(&self, shard_id: &ShardId) -> Option<&ShardWriterService> {
         self.cache.get(&shard_id.id)
     }
     #[tracing::instrument(skip_all)]
     pub fn get_mut_shard(&mut self, shard_id: &ShardId) -> Option<&mut ShardWriterService> {
         self.cache.get_mut(&shard_id.id)
     }
 
     #[tracing::instrument(skip_all)]
-    pub fn new_shard(&mut self, request: &NewShardRequest) -> NodeResult<ShardCreated> {
+    pub fn new_shard(request: &NewShardRequest) -> NodeResult<ShardCreated> {
         let shard_id = Uuid::new_v4().to_string();
         let shard_path = env::shards_path_id(&shard_id);
         let new_shard = ShardWriterService::new(shard_id.clone(), &shard_path, request)?;
-        let data = ShardCreated {
-            id: new_shard.id.clone(),
+        Ok(ShardCreated {
+            id: shard_id,
             document_service: new_shard.document_version() as i32,
             paragraph_service: new_shard.paragraph_version() as i32,
             vector_service: new_shard.vector_version() as i32,
             relation_service: new_shard.relation_version() as i32,
-        };
-        self.cache.insert(shard_id, new_shard);
-        Ok(data)
+        })
     }
 
     #[tracing::instrument(skip_all)]
     pub fn delete_shard(&mut self, shard_id: &ShardId) -> NodeResult<()> {
         if shard_id.id.is_empty() {
             warn!("Shard id is empty");
             return Ok(());
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/common/constants.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/common/constants.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files 10% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 use std::sync::Arc;
 use std::time::Duration;
 
 use nucliadb_core::protos::node_reader_client::NodeReaderClient;
 use nucliadb_core::protos::node_reader_server::NodeReaderServer;
 use nucliadb_core::protos::node_writer_client::NodeWriterClient;
 use nucliadb_core::protos::node_writer_server::NodeWriterServer;
-use nucliadb_node::reader::grpc_driver::NodeReaderGRPCDriver;
-use nucliadb_node::reader::NodeReaderService;
+use nucliadb_node::reader::grpc_driver::{GrpcReaderOptions, NodeReaderGRPCDriver};
 use nucliadb_node::writer::grpc_driver::NodeWriterGRPCDriver;
 use nucliadb_node::writer::NodeWriterService;
 use once_cell::sync::Lazy;
 use tokio::sync::Mutex;
 use tonic::transport::{Channel, Server};
 
 use crate::common::{READER_ADDR, SERVER_STARTUP_TIMEOUT, WRITER_ADDR};
@@ -45,16 +44,21 @@
     Lazy::new(|| Arc::new(Mutex::new(false)));
 
 async fn start_reader(addr: SocketAddr) {
     let mut initialized_lock = READER_SERVER_INITIALIZED.lock().await;
 
     if !*initialized_lock {
         tokio::spawn(async move {
-            let reader_server =
-                NodeReaderServer::new(NodeReaderGRPCDriver::from(NodeReaderService::new()));
+            let options = GrpcReaderOptions { lazy_loading: true };
+            let grpc_driver = NodeReaderGRPCDriver::new(options);
+            grpc_driver
+                .initialize()
+                .await
+                .expect("Unable to initialize reader gRPC");
+            let reader_server = NodeReaderServer::new(grpc_driver);
             Server::builder()
                 .add_service(reader_server)
                 .serve(addr)
                 .await
                 .map_or_else(
                     |err| {
                         panic!("Error starting gRPC server: {err:?}");
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/Cargo.toml` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/Makefile` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 
 protos:
 	python -m grpc_tools.protoc ./nucliadb_telemetry/tests/grpc/helloworld.proto           -I ./ --python_out=./ --mypy_out=./ --grpc_python_out=./ --mypy_grpc_out=./
 	python -m grpc_tools.protoc ./nucliadb_telemetry/tests/grpc/hellostreamingworld.proto  -I ./ --python_out=./ --mypy_out=./ --grpc_python_out=./ --mypy_grpc_out=./
 
 .PHONY: install-dev
 install-dev:
-## TODO: remove pip version install when pip is fixed. Right now it was making mypy fail.
-	pip install --upgrade "pip<23.1"
-	pip install -r ../test-requirements.txt
-	pip install -r ../code-requirements.txt
-	pip install -r requirements.txt
+	pip install --upgrade pip wheel
+	pip install -r ../test-requirements.txt -r ../code-requirements.txt -r requirements.txt
 # utils dep required for test fixtures for nats
 # NEEDS TO BE DECOUPLED EVENTUALLY
 	pip install -e ../nucliadb_protos/python
 	pip install -e ../nucliadb_utils
 	pip install -e .
 
 .PHONY: format
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/README.md` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/__init__.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/batch_span.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/batch_span.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/common.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/common.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/errors.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 # abstract advanced error handling into its own module to prevent
 # code from handling sentry integration everywhere
-import logging
 from typing import Any, ContextManager, Optional
 
 import pydantic
 
 try:
     import sentry_sdk
     from sentry_sdk import Scope
-    from sentry_sdk.integrations.logging import LoggingIntegration
 
     SENTRY = True
 except ImportError:  # pragma: no cover
-    Scope = LoggingIntegration = sentry_sdk = None  # type: ignore
+    Scope = sentry_sdk = None  # type: ignore
     SENTRY = False
 
 
 def capture_exception(error: BaseException) -> Optional[str]:
     if SENTRY:
         return sentry_sdk.capture_exception(error)
     return None
@@ -71,29 +69,26 @@
 
 
 class ErrorHandlingSettings(pydantic.BaseSettings):
     sentry_url: Optional[str] = None
     environment: str = pydantic.Field(
         "local", env=["environment", "running_environment"]
     )
-    logging_integration: bool = False
 
 
 def setup_error_handling(version: str) -> None:
     settings = ErrorHandlingSettings()
 
     if settings.sentry_url:
-        enabled_integrations: list[Any] = []
-
-        if settings.logging_integration:
-            sentry_logging = LoggingIntegration(
-                level=logging.CRITICAL, event_level=logging.CRITICAL
-            )
-            enabled_integrations.append(sentry_logging)
+        # Disabled everywhere for now. Let's have less knobs to tweak.
+        # Either we use with with sentry or we don't.
+        # enabled_integrations: list[Any] = [
+        #     LoggingIntegration(level=logging.CRITICAL, event_level=logging.CRITICAL)
+        # ]
 
         sentry_sdk.init(
             release=version,
             environment=settings.environment,
             dsn=settings.sentry_url,
-            integrations=enabled_integrations,
+            integrations=[],
             default_integrations=False,
         )
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/__init__.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 from nucliadb_telemetry.fastapi.metrics import PrometheusMiddleware
 from nucliadb_telemetry.fastapi.tracing import (
     OpenTelemetryMiddleware,
     ServerRequestHookT,
 )
 
+from .context import ContextInjectorMiddleware
+
 try:
     from sentry_sdk.integrations.asgi import SentryAsgiMiddleware
 except ImportError:  # pragma: no cover
     SentryAsgiMiddleware = None  # type: ignore
 
 
 async def metrics_endpoint(request):
@@ -65,20 +67,24 @@
     excluded_urls: List[str],
     server_request_hook: ServerRequestHookT = None,
     tracer_provider=None,
     metrics=False,
 ):
     if metrics:
         # b/w compat
-        app.add_middleware(PrometheusMiddleware, filter_unhandled_paths=True)
-    if SentryAsgiMiddleware is not None:
-        app.add_middleware(SentryAsgiMiddleware)
+        app.add_middleware(PrometheusMiddleware)
 
     excluded_urls_obj = ExcludeList(excluded_urls)
 
+    app.add_middleware(ContextInjectorMiddleware)
     app.add_middleware(
         OpenTelemetryMiddleware,
         excluded_urls=excluded_urls_obj,
         default_span_details=_get_route_details,
         server_request_hook=server_request_hook,
         tracer_provider=tracer_provider,
     )
+
+    if SentryAsgiMiddleware is not None:
+        # add last to catch all exceptions
+        # `add_middleware` always adds to the beginning of the middleware list
+        app.add_middleware(SentryAsgiMiddleware)
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/tracing.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/fastapi/tracing.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,14 +306,15 @@
                     current_span,
                     span_name,
                     scope,
                     send,
                 )
 
                 await self.app(scope, receive, otel_send)
+
         finally:
             if token:
                 context.detach(token)
 
     def _get_otel_send(self, server_span, server_span_name, scope, send):
         @wraps(send)
         async def otel_send(message):
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/grpc.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import functools
 from collections import OrderedDict
 from concurrent import futures
 from contextlib import contextmanager
-from typing import Any, Awaitable, Callable, List, Optional
+from typing import Any, Awaitable, Callable, List, Optional, Tuple
 
 import grpc
 from grpc import ChannelCredentials, ClientCallDetails, aio  # type: ignore
 from grpc.experimental import wrap_server_method_handler  # type: ignore
 from opentelemetry.context import attach, detach
 from opentelemetry.propagate import extract, inject
 from opentelemetry.propagators.textmap import CarrierT, Setter  # type: ignore
@@ -356,19 +356,20 @@
         self.tracer_provider = tracer_provider
 
     def init_client(
         self,
         server_addr: str,
         max_send_message: int = 100,
         credentials: Optional[ChannelCredentials] = None,
+        options: Optional[List[Tuple[str, Any]]] = None,
     ):
         options = [
             ("grpc.max_receive_message_length", max_send_message * 1024 * 1024),
             ("grpc.max_send_message_length", max_send_message * 1024 * 1024),
-        ]
+        ] + (options or [])
         interceptors = (
             get_client_interceptors(self.service_name, self.tracer_provider)
             + grpc_metrics.CLIENT_INTERCEPTORS
         )
         if credentials is not None:
             channel = aio.secure_channel(
                 server_addr,
@@ -383,25 +384,26 @@
         return channel
 
     def init_server(
         self,
         concurrency: int = 4,
         max_receive_message: int = 100,
         interceptors: Optional[List[aio.ServerInterceptor]] = None,
+        options: Optional[List[Tuple[str, Any]]] = None,
     ):
         _interceptors = (
             get_server_interceptors(self.service_name, self.tracer_provider)
             + grpc_metrics.SERVER_INTERCEPTORS
         )
         if interceptors is not None:
             _interceptors.extend(interceptors)
         options = [
             ("grpc.max_send_message_length", max_receive_message * 1024 * 1024),
             ("grpc.max_receive_message_length", max_receive_message * 1024 * 1024),
-        ]
+        ] + (options or [])
         server = aio.server(
             futures.ThreadPoolExecutor(max_workers=concurrency),
             interceptors=_interceptors,
             options=options,
         )
         return server
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/grpc_metrics.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/grpc_metrics.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/jaeger.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/jaeger.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/jetstream.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/jetstream.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,30 +13,56 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+from datetime import datetime
 from functools import partial
 from typing import Any, Callable, Dict, List, Optional
 
 from nats.aio.client import Client
 from nats.aio.msg import Msg
 from nats.js.client import JetStreamContext
 from opentelemetry.context import attach
 from opentelemetry.propagate import extract, inject
 from opentelemetry.sdk.trace import TracerProvider  # type: ignore
 from opentelemetry.semconv.trace import SpanAttributes  # type: ignore
 from opentelemetry.trace import SpanKind  # type: ignore
 from opentelemetry.trace import Tracer  # type: ignore
 
-from nucliadb_telemetry import logger
+from nucliadb_telemetry import logger, metrics
 from nucliadb_telemetry.common import set_span_exception
 
+msg_time_histo = metrics.Histogram(
+    # time it takes from when msg was queue to when it finished processing
+    "nuclia_nats_msg_op_time",
+    labels={
+        "stream": "",
+        "consumer": "",
+        "acked": "no",
+    },
+    buckets=[
+        0.005,
+        0.025,
+        0.05,
+        0.1,
+        0.5,
+        1.0,
+        5.0,
+        10.0,
+        30.0,
+        60.0,
+        120.0,
+        600.0,
+        metrics.INF,
+    ],
+)
+
 
 def start_span_message_receiver(tracer: Tracer, msg: Msg):
     attributes = {
         SpanAttributes.MESSAGING_DESTINATION_KIND: "nats",
         SpanAttributes.MESSAGING_MESSAGE_PAYLOAD_SIZE_BYTES: len(msg.data),
         SpanAttributes.MESSAGING_MESSAGE_ID: msg.reply,
     }
@@ -94,14 +120,23 @@
 
             with start_span_message_receiver(tracer, msg) as span:
                 try:
                     await origin_cb(msg)
                 except Exception as error:
                     set_span_exception(span, error)
                     raise error
+                finally:
+                    msg_time_histo.observe(
+                        (datetime.now() - msg.metadata.timestamp).total_seconds(),
+                        {
+                            "stream": msg.metadata.stream,
+                            "consumer": msg.metadata.consumer or "",
+                            "acked": "yes" if msg._ackd else "no",  # type: ignore
+                        },
+                    )
 
         wrapped_cb = partial(wrapper, cb, tracer)
         return await self.js.subscribe(cb=wrapped_cb, **kwargs)
 
     async def publish(
         self,
         subject: str,
@@ -112,16 +147,15 @@
         tracer = self.tracer_provider.get_tracer(f"{self.service_name}_js_publisher")
         headers = {} if headers is None else headers
         inject(headers)
         with start_span_message_publisher(tracer, subject) as span:
             try:
                 result = await self.js.publish(subject, body, headers=headers, **kwargs)
             except Exception as error:
-                if type(error) != Exception:
-                    set_span_exception(span, error)
+                set_span_exception(span, error)
                 raise error
 
         return result
 
     # Just for convenience, to wrap all we use in the context of
     # telemetry-instrumented stuff using the JetStreamContextTelemetry class
 
@@ -154,14 +188,23 @@
 
         with start_span_message_receiver(tracer, message) as span:
             try:
                 return await cb(message)
             except Exception as error:
                 set_span_exception(span, error)
                 raise error
+            finally:
+                msg_time_histo.observe(
+                    (datetime.now() - message.metadata.timestamp).total_seconds(),
+                    {
+                        "stream": message.metadata.stream,
+                        "consumer": message.metadata.consumer or "",
+                        "acked": "yes" if message._ackd else "no",
+                    },
+                )
 
 
 class NatsClientTelemetry:
     def __init__(self, nc: Client, service_name: str, tracer_provider: TracerProvider):
         self.nc = nc
         self.service_name = service_name
         self.tracer_provider = tracer_provider
@@ -197,16 +240,15 @@
         headers = {} if headers is None else headers
         inject(headers)
 
         with start_span_message_publisher(tracer, subject) as span:
             try:
                 result = await self.nc.publish(subject, body, headers=headers, **kwargs)
             except Exception as error:
-                if type(error) != Exception:
-                    set_span_exception(span, error)
+                set_span_exception(span, error)
                 raise error
 
         return result
 
     async def request(
         self,
         subject: str,
@@ -220,12 +262,11 @@
         tracer = self.tracer_provider.get_tracer(f"{self.service_name}_nc_request")
         with start_span_message_publisher(tracer, subject) as span:
             try:
                 result = await self.nc.request(
                     subject, payload, timeout, old_style, headers  # type: ignore
                 )
             except Exception as error:
-                if type(error) != Exception:
-                    set_span_exception(span, error)
+                set_span_exception(span, error)
                 raise error
 
         return result
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/logs.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 import orjson
 import pydantic
 from opentelemetry import trace
 from opentelemetry.trace.span import INVALID_SPAN
 
 from nucliadb_telemetry.settings import LogLevel, LogSettings
 
+from . import context
+
 try:
     from uvicorn.logging import AccessFormatter  # type: ignore
 except ImportError:  # pragma: no cover
     AccessFormatter = logging.Formatter
 
 _BUILTIN_ATTRS = (
     # list of all possible args
@@ -96,14 +98,18 @@
         data["severity"] = record.levelname
         data["logging.googleapis.com/sourceLocation"] = {
             "file": record.pathname,
             "line": record.lineno,
             "function": record.funcName,
         }
 
+        current_ctx = context.get_context()
+        if len(current_ctx) > 0:
+            data["context"] = current_ctx
+
         current_span = trace.get_current_span()
         if current_span not in (INVALID_SPAN, None):
             span_context = current_span.get_span_context()
             # for us, this is opentelemetry trace_id/span_id
             # GCP has logging.googleapis.com/spanId but it's for it's own cloud tracing system
             data["trace_id"] = str(span_context.trace_id)
             data["span_id"] = str(span_context.span_id)
@@ -146,45 +152,57 @@
         )
         return super().format(recordcopy)
 
 
 _ACCESS_LOGGER_NAME = "uvicorn.access"
 
 
+_default_logger_levels = {
+    # some are too chatty
+    "uvicorn.error": LogLevel.WARNING,
+    "nucliadb_utils.utilities": LogLevel.WARNING,
+    # needed always for access logs
+    _ACCESS_LOGGER_NAME: LogLevel.INFO,
+}
+
+
 def setup_logging() -> None:
     settings = LogSettings()
 
     if settings.logger_levels is None:
         settings.logger_levels = {}
-    if _ACCESS_LOGGER_NAME not in settings.logger_levels:
-        settings.logger_levels[
-            _ACCESS_LOGGER_NAME
-        ] = LogLevel.INFO  # always have INFO here so we get access logs
 
-    formatter = JSONFormatter()
-    access_formatter = UvicornAccessFormatter()
+    for logger_name, level in _default_logger_levels.items():
+        if logger_name not in settings.logger_levels:
+            settings.logger_levels[logger_name] = level
 
+    formatter = JSONFormatter()
     json_handler = logging.StreamHandler()
     json_handler.setFormatter(formatter)
-    access_handler = logging.StreamHandler()
-    access_handler.setFormatter(access_formatter)
     stream_handler = logging.StreamHandler()
+    stream_handler.setFormatter(
+        logging.Formatter(
+            "[%(asctime)s.%(msecs)02d] [%(levelname)s] - %(name)s - %(message)s"
+        )
+    )
 
     root_logger = logging.getLogger()
     access_logger = logging.getLogger(_ACCESS_LOGGER_NAME)
     access_logger.handlers = []
     if not settings.debug:
         root_logger.addHandler(json_handler)
+        access_handler = logging.StreamHandler()
+        access_handler.setFormatter(UvicornAccessFormatter())
         access_logger.addHandler(access_handler)
     else:
         root_logger.addHandler(stream_handler)
         # regular stream access logs
-        access_log_handler = logging.StreamHandler()
-        access_log_handler.setFormatter(AccessFormatter())
-        access_logger.addHandler(stream_handler)
+        access_handler = logging.StreamHandler()
+        access_handler.setFormatter(AccessFormatter())  # not json based
+        access_logger.addHandler(access_handler)
 
     root_logger.setLevel(getattr(logging, settings.log_level.value))
 
     for logger_name, level in settings.logger_levels.items():
         log = logging.getLogger(logger_name)
         if logger_name != _ACCESS_LOGGER_NAME:
             if not settings.debug:
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/metrics.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 import asyncio
 import os
 import time
 from functools import wraps
+from inspect import isasyncgenfunction, isgeneratorfunction
 from typing import TYPE_CHECKING, Optional, Type, Union
 
 import prometheus_client
 
 if TYPE_CHECKING:  # pragma: no cover
     from traceback import StackSummary
 else:
@@ -79,14 +80,30 @@
             if asyncio.iscoroutinefunction(func):
 
                 @wraps(func)
                 async def inner(*args, **kwargs):
                     with ObserverRecorder(self, labels or {}):
                         return await func(*args, **kwargs)
 
+            elif isasyncgenfunction(func):
+
+                @wraps(func)
+                async def inner(*args, **kwargs):
+                    with ObserverRecorder(self, labels or {}):
+                        async for item in func(*args, **kwargs):
+                            yield item
+
+            elif isgeneratorfunction(func):
+
+                @wraps(func)
+                def inner(*args, **kwargs):
+                    with ObserverRecorder(self, labels or {}):
+                        for item in func(*args, **kwargs):
+                            yield item
+
             else:
 
                 @wraps(func)
                 def inner(*args, **kwargs):
                     with ObserverRecorder(self, labels or {}):
                         return func(*args, **kwargs)
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/settings.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/__init__.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/conftest.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/__init__.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld.proto` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.pyi` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.pyi` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld.proto` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2.pyi` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.pyi` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/integration/test_fastapi.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/integration/test_fastapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -157,44 +157,14 @@
             in metrics_text
         )
         assert (
             'starlette_requests_in_progress{method="GET",path_template="/metrics/"} 1.0'
             in metrics_text
         )
 
-    def test_unhandled_paths(self, client):
-        # Do a request
-        client.get("/any/unhandled/path")
-
-        # Get metrics
-        response = client.get("/metrics/")
-        metrics_text = response.content.decode()
-
-        # Asserts: Requests
-        assert (
-            'starlette_requests_total{method="GET",path_template="/any/unhandled/path"} 1.0'
-            in metrics_text
-        )
-
-        # Asserts: Responses
-        assert (
-            'starlette_responses_total{method="GET",path_template="/any/unhandled/path",status_code="404"} 1.0'
-            in metrics_text
-        )
-
-        # Asserts: Requests in progress
-        assert (
-            'starlette_requests_in_progress{method="GET",path_template="/any/unhandled/path"} 0.0'
-            in metrics_text
-        )
-        assert (
-            'starlette_requests_in_progress{method="GET",path_template="/metrics/"} 1.0'
-            in metrics_text
-        )
-
     def test_sub_path_match(self, client):
         # Do a request
         client.get("/sub/foobar/")
 
         # Get metrics
         response = client.get("/metrics/")
         metrics_text = response.content.decode()
@@ -206,15 +176,15 @@
         )
 
 
 class TestCasePrometheusMiddlewareFilterUnhandledPaths:
     @pytest.fixture(scope="class")
     def app(self):
         app_ = Starlette()
-        app_.add_middleware(PrometheusMiddleware, filter_unhandled_paths=True)
+        app_.add_middleware(PrometheusMiddleware)
         app_.add_route("/metrics/", metrics_endpoint)
 
         return app_
 
     @pytest.fixture
     def client(self, app):
         return TestClient(app)
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/integration/test_telemetry.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/integration/test_telemetry.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import asyncio
 import json
 
 import pytest
 from httpx import AsyncClient
 
 from nucliadb_telemetry import grpc_metrics
+from nucliadb_telemetry.jetstream import msg_time_histo
 from nucliadb_telemetry.settings import telemetry_settings
 from nucliadb_telemetry.tests.telemetry import Greeter
 
 
 def fmt_span(span):
     tags_by_key = {tag["key"]: tag["value"] for tag in span["tags"]}
     return {
@@ -92,7 +93,17 @@
     # debug_spans(resp.json()["data"][0]["spans"])
 
     assert len(resp.json()["data"][0]["spans"]) == expected_spans
     assert len(resp.json()["data"][0]["processes"]) == 3
 
     assert grpc_metrics.grpc_client_observer.histogram.collect()[0].samples  # type: ignore
     assert grpc_metrics.grpc_server_observer.histogram.collect()[0].samples  # type: ignore
+
+    assert msg_time_histo.histo.collect()[0].samples  # type: ignore
+
+    sample = [
+        sam.labels
+        for sam in msg_time_histo.histo.collect()[0].samples  # type: ignore
+        if sam.labels.get("le") == "0.005"
+    ][0]
+    sample.pop("consumer")
+    assert sample == {"stream": "testing", "acked": "no", "le": "0.005"}
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/telemetry.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/telemetry.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_errors.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from unittest.mock import ANY, patch
+from unittest.mock import patch
 
 from nucliadb_telemetry import errors
 
 
 def test_capture_exception() -> None:
     with patch("nucliadb_telemetry.errors.sentry_sdk") as mock_sentry_sdk, patch.object(
         errors, "SENTRY", True
@@ -55,28 +55,26 @@
     ) as mock_sentry_sdk:
         errors.capture_message("error_msg", "level", "scope")
         mock_sentry_sdk.capture_message.assert_not_called()
 
 
 def test_setup_error_handling(monkeypatch):
     monkeypatch.setenv("sentry_url", "sentry_url")
-    monkeypatch.setenv("logging_integration", "True")
     monkeypatch.setenv("environment", "environment")
     with patch("nucliadb_telemetry.errors.sentry_sdk") as mock_sentry_sdk, patch.object(
         errors, "SENTRY", True
-    ), patch("nucliadb_telemetry.errors.LoggingIntegration") as LoggingIntegration:
+    ):
         errors.setup_error_handling("1.0.0")
         mock_sentry_sdk.init.assert_called_once_with(
             release="1.0.0",
             environment="environment",
             dsn="sentry_url",
-            integrations=[ANY],
+            integrations=[],
             default_integrations=False,
         )
-        LoggingIntegration.assert_called_once()
 
 
 def test_setup_error_handling_no_sentry(monkeypatch):
     with patch("nucliadb_telemetry.errors.sentry_sdk") as mock_sentry_sdk:
         errors.setup_error_handling("1.0.0")
         mock_sentry_sdk.init.assert_not_called()
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_logs.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_logs.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,31 +13,33 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+import asyncio
 import logging
 from unittest.mock import MagicMock, patch
 
 import orjson
 import pydantic
+import pytest
 
-from nucliadb_telemetry import logs
+from nucliadb_telemetry import context, logs
 
 
 def test_setup_logging(monkeypatch):
     monkeypatch.setenv("LOG_LEVEL", "INFO")
     monkeypatch.setenv("LOGGER_LEVELS", '{"foo": "WARNING"}')
     with patch("nucliadb_telemetry.logs.logging") as logging:
         logs.setup_logging()
 
         logging.getLogger.assert_any_call("foo")
-        assert len(logging.getLogger().addHandler.mock_calls) == 3
+        assert len(logging.getLogger().addHandler.mock_calls) == 5
 
         logger = logging.getLogger()
         handler = logger.addHandler.mock_calls[0].args[0]
         assert isinstance(
             handler.setFormatter.mock_calls[0].args[0], logs.JSONFormatter
         )
 
@@ -144,7 +146,50 @@
     )
     with patch("nucliadb_telemetry.logs.trace.get_current_span", return_value=span):
         logger.error("foobar")
 
     assert len(outputted_records) == 1
     assert outputted_records[0]["trace_id"] == "9999999999999999999999"
     assert outputted_records[0]["span_id"] == "9999999999999999999999"
+
+
+@pytest.mark.asyncio
+async def test_logger_with_context(caplog):
+    logger = logging.getLogger("test.logger4")
+    formatter = logs.JSONFormatter()
+
+    outputted_records = []
+
+    class Handler(logging.Handler):
+        def emit(self, record):
+            msg = self.format(record)
+            data = orjson.loads(msg)
+            outputted_records.append(data)
+
+    handler = Handler()
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+
+    logger.setLevel(logging.ERROR)
+    logger.propagate = False
+
+    async def task2():
+        context.add_context({"task2": "value", "foo": "baz"})
+        logger.error("baz")
+
+    async def task1():
+        context.add_context({"task1": "value", "foo": "bar"})
+        logger.error("bar")
+        await asyncio.create_task(task2())
+
+    await asyncio.create_task(task1())
+    assert len(outputted_records) == 2
+
+    assert outputted_records[0]["context"] == {
+        "task1": "value",
+        "foo": "bar",
+    }
+    assert outputted_records[1]["context"] == {
+        "task1": "value",
+        "task2": "value",
+        "foo": "baz",
+    }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_metrics.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tests/unit/test_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
+import asyncio
+import time
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 from nucliadb_telemetry import metrics
 
 
@@ -85,14 +87,47 @@
             pass
 
         await my_func()
 
         histogram.observe.assert_called_once()
         counter.labels().inc.assert_called_once()
 
+    def test_gen_decorator(self, histogram, counter):
+        observer = metrics.Observer("my_metric")
+
+        @observer.wrap()
+        def my_func():
+            for i in range(1):
+                time.sleep(0.2)
+                yield i
+
+        for _ in my_func():
+            pass
+
+        histogram.observe.assert_called_once()
+        assert histogram.observe.call_args[0][0] >= 0.2
+        counter.labels().inc.assert_called_once()
+
+    @pytest.mark.asyncio
+    async def test_async_gen_decorator(self, histogram, counter):
+        observer = metrics.Observer("my_metric")
+
+        @observer.wrap()
+        async def my_func():
+            for i in range(1):
+                await asyncio.sleep(0.2)
+                yield i
+
+        async for _ in my_func():
+            pass
+
+        histogram.observe.assert_called_once()
+        assert histogram.observe.call_args[0][0] >= 0.2
+        counter.labels().inc.assert_called_once()
+
     def test_observer_with_env(self, histogram, counter, monkeypatch):
         monkeypatch.setenv("VERSION", "1.0.0")
         observer = metrics.Observer(
             "my_metric", buckets=[1, 2, 3], labels={"foo": "bar"}
         )
         with observer(labels={"foo": "baz"}):
             pass
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tracerprovider.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/tracerprovider.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/utils.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/nucliadb_telemetry/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,30 +15,34 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 import os
-from typing import Dict, Optional, Sequence, Union
+from typing import Dict, Optional
 
 from opentelemetry.propagate import set_global_textmap
 from opentelemetry.propagators.b3 import B3MultiFormat
 from opentelemetry.sdk.resources import SERVICE_NAME  # type: ignore
 from opentelemetry.sdk.resources import Resource  # type: ignore
-from opentelemetry.trace import get_current_span
 
 from nucliadb_telemetry.batch_span import BatchSpanProcessor
 from nucliadb_telemetry.jaeger import JaegerExporterAsync
 from nucliadb_telemetry.settings import telemetry_settings
+from nucliadb_telemetry.tikv import TiKVInstrumentor
 from nucliadb_telemetry.tracerprovider import (
     AsyncMultiSpanProcessor,
     AsyncTracerProvider,
 )
 
+from .context import set_info_on_span  # noqa: F401
+
+set_info_on_span  # b/w compatible import
+
 GLOBAL_PROVIDER: Dict[str, AsyncTracerProvider] = {}
 
 
 def get_telemetry(service_name: Optional[str] = None) -> Optional[AsyncTracerProvider]:
     if service_name is None:
         return None
     if service_name not in GLOBAL_PROVIDER and service_name is not None:
@@ -113,36 +117,17 @@
     """
     Setup telemetry for a service if it is enabled
     """
     tracer_provider = get_telemetry(service_name)
     if tracer_provider is not None:  # pragma: no cover
         await init_telemetry(tracer_provider)
         set_global_textmap(B3MultiFormat())
+        TiKVInstrumentor().instrument(tracer_provider=tracer_provider)
         try:
             from opentelemetry.instrumentation.aiohttp_client import (  # type: ignore
                 AioHttpClientInstrumentor,
             )
 
             AioHttpClientInstrumentor().instrument(tracer_provider=tracer_provider)
         except ImportError:
             pass
     return tracer_provider
-
-
-def set_info_on_span(
-    headers: Dict[
-        str,
-        Union[
-            str,
-            bool,
-            int,
-            float,
-            Sequence[str],
-            Sequence[bool],
-            Sequence[int],
-            Sequence[float],
-        ],
-    ]
-):
-    if telemetry_settings.jaeger_enabled:
-        span = get_current_span()
-        span.set_attributes(headers)
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/requirements.txt` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-nats-py[nkeys]==2.1.3
+nats-py[nkeys]==2.2.0
 httpx==0.23.0
 grpcio>=1.44.0
 grpcio-health-checking>=1.44.0
 grpcio-channelz>=1.44.0
 grpcio-status>=1.44.0
 grpcio-tools>=1.44.0
 grpcio-testing>=1.44.0
@@ -14,11 +14,14 @@
 opentelemetry-propagator-b3==1.11.1
 opentelemetry-instrumentation-fastapi==0.30b1
 opentelemetry-instrumentation-aiohttp-client>=0.30b1
 opentelemetry-semantic-conventions>=0.30b1
 pydantic
 requests
 fastapi
+tikv-client>=0.0.3
 types-protobuf>=3.19.5,<4.0
 types-requests
 prometheus-client>=0.12.0
-orjson>=3.6.7
+orjson>=3.6.7
+urllib3<1.27,>=1.21.1
+wrapt>=1.14.1
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/setup.cfg` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/setup.cfg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/setup.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/blocking.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/lib.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
+//
 
-#![allow(clippy::bool_assert_comparison)]
-pub mod payload;
-/// This crate contains  the code responsible for sending usage data to Nuclia's server.
-mod sender;
-pub(crate) mod sink;
+mod bfs;
+pub mod reader;
+#[cfg(test)]
+mod tests;
+mod utils;
+pub mod writer;
 
-pub mod blocking;
-pub mod sync;
-/// This environment variable can be set to disable sending telemetry events.
-pub const DISABLE_TELEMETRY_ENV_KEY: &str = "NUCLIADB_DISABLE_TELEMETRY";
+pub use reader::*;
+pub use writer::*;
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/payload.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/payload.rs`

 * *Files 2% similar despite different names*

```diff
@@ -122,17 +122,17 @@
 }
 
 fn hashed_host_username() -> String {
     let hostname = hostname::get()
         .map(|hostname| hostname.to_string_lossy().to_string())
         .unwrap_or_else(|_| "".to_string());
     let username = username::get_user_name().unwrap_or_else(|_| "".to_string());
-    let hashed_value = format!("{}:{}", hostname, username);
+    let hashed_value = format!("{hostname}:{username}");
     let digest = md5::compute(hashed_value.as_bytes());
-    format!("{:x}", digest)
+    format!("{digest:x}")
 }
 
 impl Default for ClientInformation {
     fn default() -> ClientInformation {
         ClientInformation {
             session_uuid: Uuid::new_v4(),
             nucliadb_version: env!("CARGO_PKG_VERSION").to_string(),
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/sender.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/sink.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_telemetry/src/sync.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_telemetry/src/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -105,40 +105,52 @@
 
 pub struct Retriever<'a, Dlog> {
     similarity: Similarity,
     no_nodes: usize,
     temp: &'a [u8],
     nodes: &'a Mmap,
     delete_log: &'a Dlog,
+    min_score: f32,
 }
 impl<'a, Dlog: DeleteLog> Retriever<'a, Dlog> {
     pub fn new(
         temp: &'a [u8],
         nodes: &'a Mmap,
         delete_log: &'a Dlog,
         similarity: Similarity,
+        min_score: f32,
     ) -> Retriever<'a, Dlog> {
         Retriever {
             temp,
             nodes,
             delete_log,
             similarity,
             no_nodes: key_value::get_no_elems(nodes),
+            min_score,
         }
     }
     fn find_node(&self, Address(x): Address) -> &[u8] {
         if x == self.no_nodes {
             self.temp
         } else {
             key_value::get_value(Node, self.nodes, x)
         }
     }
 }
 
 impl<'a, Dlog: DeleteLog> DataRetriever for Retriever<'a, Dlog> {
+    fn get_key(&self, x @ Address(addr): Address) -> &[u8] {
+        if addr == self.no_nodes {
+            &[]
+        } else {
+            let x = self.find_node(x);
+            Node::key(x)
+        }
+    }
+
     fn get_vector(&self, x @ Address(addr): Address) -> &[u8] {
         if addr == self.no_nodes {
             self.temp
         } else {
             let x = self.find_node(x);
             Node::vector(x)
         }
@@ -173,14 +185,18 @@
             let x = self.find_node(x);
             let y = self.find_node(y);
             let x = Node::vector(x);
             let y = Node::vector(y);
             self.similarity.compute(x, y)
         }
     }
+
+    fn min_score(&self) -> f32 {
+        self.min_score
+    }
 }
 
 #[derive(Clone, Debug)]
 pub struct LabelDictionary(Vec<u8>);
 impl Default for LabelDictionary {
     fn default() -> Self {
         LabelDictionary::new(vec![])
@@ -307,38 +323,54 @@
 impl AsRef<DataPoint> for DataPoint {
     fn as_ref(&self) -> &DataPoint {
         self
     }
 }
 
 impl DataPoint {
+    pub fn stored_len(&self) -> Option<u64> {
+        if key_value::get_no_elems(&self.nodes) == 0 {
+            return None;
+        }
+        let node = key_value::get_value(Node, &self.nodes, 0);
+        Some(vector::vector_len(Node::vector(node)))
+    }
     pub fn get_id(&self) -> DpId {
         self.journal.uid
     }
     pub fn meta(&self) -> Journal {
         self.journal
     }
     pub fn get_keys<Dlog: DeleteLog>(&self, delete_log: &Dlog) -> Vec<String> {
         key_value::get_keys(Node, &self.nodes)
             .filter(|k| !delete_log.is_deleted(k))
             .map(String::from_utf8_lossy)
             .map(|s| s.to_string())
             .collect()
     }
+
+    #[allow(clippy::too_many_arguments)]
     pub fn search<Dlog: DeleteLog>(
         &self,
         delete_log: &Dlog,
         query: &[f32],
         filter: &Formula,
         with_duplicates: bool,
         results: usize,
         similarity: Similarity,
+        min_score: f32,
     ) -> impl Iterator<Item = Neighbour> + '_ {
         let encoded_query = vector::encode_vector(query);
-        let tracker = Retriever::new(&encoded_query, &self.nodes, delete_log, similarity);
+        let tracker = Retriever::new(
+            &encoded_query,
+            &self.nodes,
+            delete_log,
+            similarity,
+            min_score,
+        );
         let ops = HnswOps::new(&tracker);
         let neighbours = ops.search(
             Address(self.journal.nodes),
             self.index.as_ref(),
             results,
             filter,
             with_duplicates,
@@ -385,15 +417,15 @@
             let mut node_buffer = BufWriter::new(&mut nodes);
             key_value::merge(&mut node_buffer, node_producers.collect())?;
             node_buffer.flush()?;
         }
 
         let nodes = unsafe { Mmap::map(&nodes)? };
         let no_nodes = key_value::get_no_elems(&nodes);
-        let tracker = Retriever::new(&[], &nodes, &NoDLog, similarity);
+        let tracker = Retriever::new(&[], &nodes, &NoDLog, similarity, -1.0);
         let mut ops = HnswOps::new(&tracker);
         let mut index = RAMHnsw::new();
         for id in 0..no_nodes {
             ops.insert(Address(id), &mut index)
         }
 
         {
@@ -486,15 +518,15 @@
             key_value::create_key_value(&mut nodesf_buffer, elems)?;
             nodesf_buffer.flush()?;
         }
         let nodes = unsafe { Mmap::map(&nodesf)? };
         let no_nodes = key_value::get_no_elems(&nodes);
 
         // Creating the HNSW using the mmaped nodes
-        let tracker = Retriever::new(&[], &nodes, &NoDLog, similarity);
+        let tracker = Retriever::new(&[], &nodes, &NoDLog, similarity, -1.0);
         let mut ops = HnswOps::new(&tracker);
         let mut index = RAMHnsw::new();
         for id in 0..no_nodes {
             ops.insert(Address(id), &mut index)
         }
 
         {
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,20 @@
         30
     }
     pub const fn ef_construction() -> usize {
         100
     }
 }
 pub trait DataRetriever: std::marker::Sync {
+    fn get_key(&self, _: Address) -> &[u8];
     fn is_deleted(&self, _: Address) -> bool;
     fn has_label(&self, _: Address, _: &[u8]) -> bool;
     fn similarity(&self, _: Address, _: Address) -> f32;
     fn get_vector(&self, _: Address) -> &[u8];
+    fn min_score(&self) -> f32;
 }
 
 pub trait Layer {
     type EdgeIt: Iterator<Item = (Address, Edge)>;
     fn get_out_edges(&self, node: Address) -> Self::EdgeIt;
 }
 
@@ -96,15 +98,15 @@
         mut candidates: Vec<(Address, Edge)>,
     ) -> Vec<(Address, Edge)> {
         candidates.sort_unstable_by_key(|(n, d)| std::cmp::Reverse(Cnx(*n, d.dist)));
         candidates.dedup_by_key(|(addr, _)| *addr);
         candidates.truncate(k_neighbours);
         candidates
     }
-    fn cosine_similarity(&self, x: Address, y: Address) -> f32 {
+    fn similarity(&self, x: Address, y: Address) -> f32 {
         self.tracker.similarity(x, y)
     }
     fn get_random_layer(&mut self) -> usize {
         let sample: f64 = self.layer_rng.sample(self.distribution);
         let picked_level = -sample.ln() * params::level_factor();
         picked_level.round() as usize
     }
@@ -114,35 +116,36 @@
         query: Address,
         layer: L,
         filter: &Formula,
         blocked_addresses: &HashSet<Address>,
         vec_counter: &RepCounter,
     ) -> Option<(Address, f32)> {
         let mut visited_nodes = HashSet::new();
-        let mut candidates = BinaryHeap::from([Cnx(x, self.cosine_similarity(x, query))]);
+        let mut candidates = BinaryHeap::from([Cnx(x, self.similarity(x, query))]);
         loop {
             match candidates.pop() {
                 None => break None,
+                Some(Cnx(_, score)) if score < self.tracker.min_score() => break None,
                 Some(Cnx(n, score))
                         // The vector was deleted at some point and will be removed in a future merge
                         if !self.tracker.is_deleted(n)
                         // A score may be invalid if the index contains zero vectors 
                         && !score.is_nan()
                         // The vector is blocked, meaning that its key is part of the current version of the solution
                         && !blocked_addresses.contains(&n)
                         // The number of times this vector appears is 0
                         && vec_counter.get(self.tracker.get_vector(n)) == 0
                         // The vector satisfies the given filter
                         && filter.run(n, self.tracker) =>
                 {
-                    break Some((n, self.cosine_similarity(n, query)));
+                    break Some((n, self.similarity(n, query)));
                 }
                 Some(Cnx(down, _)) => layer.get_out_edges(down).for_each(|(n, _)| {
                     if !visited_nodes.contains(&n) {
-                        candidates.push(Cnx(n, self.cosine_similarity(n, query)));
+                        candidates.push(Cnx(n, self.similarity(n, query)));
                         visited_nodes.insert(n);
                     }
                 }),
             }
         }
     }
     fn layer_search<L: Layer>(
@@ -153,27 +156,27 @@
         entry_points: &[Address],
     ) -> Neighbours {
         let mut visited = HashSet::new();
         let mut candidates = BinaryHeap::new();
         let mut ms_neighbours = BinaryHeap::new();
         for ep in entry_points.iter().copied() {
             visited.insert(ep);
-            let similarity = self.cosine_similarity(x, ep);
+            let similarity = self.similarity(x, ep);
             candidates.push(Cnx(ep, similarity));
             ms_neighbours.push(Reverse(Cnx(ep, similarity)));
         }
         loop {
             match (candidates.pop(), ms_neighbours.peek().cloned()) {
                 (None, _) => break,
                 (Some(Cnx(_, cs)), Some(Reverse(Cnx(_, ws)))) if cs < ws => break,
                 (Some(Cnx(cn, _)), Some(Reverse(Cnx(_, mut ws)))) => {
                     for (y, _) in layer.get_out_edges(cn) {
                         if !visited.contains(&y) {
                             visited.insert(y);
-                            let similarity = self.cosine_similarity(x, y);
+                            let similarity = self.similarity(x, y);
                             if similarity > ws || ms_neighbours.len() < k_neighbours {
                                 candidates.push(Cnx(y, similarity));
                                 ms_neighbours.push(Reverse(Cnx(y, similarity)));
                                 if ms_neighbours.len() > k_neighbours {
                                     ms_neighbours.pop();
                                 }
                                 ws = ms_neighbours.peek().map_or(ws, |Reverse(v)| v.1);
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 use std::collections::HashSet;
 
 use crate::data_point::{DataPoint, DeleteLog, Elem, LabelDictionary, Similarity};
-use crate::formula::{Formula, LabelClause};
+use crate::formula::{AtomClause, Formula};
 
 const SIMILARITY: Similarity = Similarity::Cosine;
 
 fn create_query() -> Vec<f32> {
     vec![rand::random::<f32>; 178]
         .into_iter()
         .map(|f| f())
@@ -43,15 +43,15 @@
 fn simple_flow() {
     let temp_dir = tempfile::tempdir().unwrap();
     let mut elems = vec![];
     let mut labels = vec![];
     let mut queries = vec![];
     for i in 0..50 {
         labels.push(format!("LABEL_{}", i));
-        queries.push(LabelClause::new(format!("LABEL_{}", i)));
+        queries.push(AtomClause::label(format!("LABEL_{}", i)));
     }
     let mut expected_keys = vec![];
     let label_dictionary = LabelDictionary::new(labels.clone());
     for i in 0..50 {
         let key = format!("KEY_{}", i);
         let vector = vec![rand::random::<f32>(); 8];
         let labels = label_dictionary.clone();
@@ -70,29 +70,30 @@
     let result = reader.search(
         &HashSet::new(),
         &query,
         &formula,
         true,
         no_results,
         Similarity::Cosine,
+        -1.0,
     );
     let got_keys = reader.get_keys(&HashSet::new());
     assert!(got_keys.iter().all(|k| expected_keys.contains(k)));
     assert_eq!(got_keys.len(), expected_keys.len());
     assert_eq!(result.count(), no_results);
 }
 
 #[test]
 fn accuracy_test() {
     let temp_dir = tempfile::tempdir().unwrap();
     let mut labels = vec![];
     let mut queries = vec![];
     for i in 0..50 {
         labels.push(format!("LABEL_{}", i));
-        queries.push(LabelClause::new(format!("LABEL_{}", i)));
+        queries.push(AtomClause::label(format!("LABEL_{}", i)));
     }
     let labels_dictionary = LabelDictionary::new(labels.clone());
     let mut elems = Vec::new();
     for i in 0..100 {
         let key = format!("KEY_{}", i);
         let vector = create_query();
         let labels = labels_dictionary.clone();
@@ -109,27 +110,29 @@
         .search(
             &HashSet::new(),
             &query,
             &formula,
             true,
             no_results,
             Similarity::Cosine,
+            -1.0,
         )
         .collect::<Vec<_>>();
     result_0.sort_by(|i, j| i.id().cmp(j.id()));
     let query: Vec<_> = query.into_iter().map(|v| v + 1.0).collect();
     let no_results = 10;
     let mut result_1 = reader
         .search(
             &HashSet::new(),
             &query,
             &formula,
             true,
             no_results,
             Similarity::Cosine,
+            -1.0,
         )
         .collect::<Vec<_>>();
     result_1.sort_by(|i, j| i.id().cmp(j.id()));
     assert_ne!(result_0, result_1)
 }
 
 #[test]
@@ -149,26 +152,28 @@
     let result = reader.search(
         &HashSet::from([key.clone()]),
         &vector,
         &formula,
         true,
         5,
         Similarity::Cosine,
+        -1.0,
     );
     assert_eq!(result.count(), 0);
 
     let reader = DataPoint::new(temp_dir.path(), elems, None, SIMILARITY).unwrap();
     let result = reader
         .search(
             &HashSet::new(),
             &vector,
             &formula,
             true,
             5,
             Similarity::Cosine,
+            -1.0,
         )
         .collect::<Vec<_>>();
     assert_eq!(result.len(), 1);
     assert!(result[0].score() >= 0.9);
     assert!(result[0].id() == key.as_bytes());
 }
 
@@ -208,27 +213,29 @@
         .search(
             &HashSet::new(),
             &vector1,
             &formula,
             true,
             1,
             Similarity::Cosine,
+            -1.0,
         )
         .collect();
     assert_eq!(result.len(), 1);
     assert!(result[0].score() >= 0.9);
     assert!(result[0].id() == key1.as_bytes());
     let result: Vec<_> = dp
         .search(
             &HashSet::new(),
             &vector0,
             &formula,
             true,
             1,
             Similarity::Cosine,
+            -1.0,
         )
         .collect();
     assert_eq!(result.len(), 1);
     assert!(result[0].score() >= 0.9);
     assert!(result[0].id() == key0.as_bytes());
     let dlog = HashSet::from([key1, key0]);
     let dp = DataPoint::merge(
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point_provider/merge_worker.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point_provider/merge_worker.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point_provider/merger.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point_provider/merger.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -36,24 +36,25 @@
 use state::*;
 use work_flag::MergerWriterSync;
 
 pub use crate::data_point::Neighbour;
 use crate::data_point::{DataPoint, DpId, Similarity};
 use crate::data_point_provider::merge_worker::Worker;
 use crate::formula::Formula;
-use crate::VectorR;
+use crate::{VectorErr, VectorR};
 pub type TemporalMark = SystemTime;
 
 const METADATA: &str = "metadata.json";
 
 pub trait SearchRequest {
     fn get_query(&self) -> &[f32];
     fn get_filter(&self) -> &Formula;
     fn no_results(&self) -> usize;
     fn with_duplicates(&self) -> bool;
+    fn min_score(&self) -> f32;
 }
 
 #[derive(Clone, Copy, Debug)]
 pub enum IndexCheck {
     None,
     Sanity,
 }
@@ -81,14 +82,15 @@
 
 pub struct Index {
     metadata: IndexMetadata,
     work_flag: MergerWriterSync,
     state: RwLock<State>,
     date: RwLock<Version>,
     location: PathBuf,
+    dimension_used: Option<u64>,
 }
 impl Index {
     fn read_state(&self) -> RwLockReadGuard<'_, State> {
         self.state.read().unwrap_or_else(|e| e.into_inner())
     }
     fn write_state(&self) -> RwLockWriteGuard<'_, State> {
         self.state.write().unwrap_or_else(|e| e.into_inner())
@@ -122,22 +124,24 @@
         );
         merger::send_merge_request(worker);
     }
     pub fn open(path: &Path, with_check: IndexCheck) -> VectorR<Index> {
         let lock = fs_state::shared_lock(path)?;
         let state = fs_state::load_state::<State>(&lock)?;
         let date = fs_state::crnt_version(&lock)?;
+        let dimension_used = state.stored_len(path)?;
         let metadata = IndexMetadata::open(path)?.map(Ok).unwrap_or_else(|| {
             // Old indexes may not have this file so in that case the
             // metadata file they should have is created.
             let metadata = IndexMetadata::default();
             metadata.write(path).map(|_| metadata)
         })?;
         let index = Index {
             metadata,
+            dimension_used,
             work_flag: MergerWriterSync::new(),
             state: RwLock::new(state),
             date: RwLock::new(date),
             location: path.to_path_buf(),
         };
         if let IndexCheck::Sanity = with_check {
             let mut state = index.write_state();
@@ -151,14 +155,15 @@
         fs_state::initialize_disk(path, State::new)?;
         metadata.write(path)?;
         let lock = fs_state::shared_lock(path)?;
         let state = fs_state::load_state::<State>(&lock)?;
         let date = fs_state::crnt_version(&lock)?;
         let index = Index {
             metadata,
+            dimension_used: None,
             work_flag: MergerWriterSync::new(),
             state: RwLock::new(state),
             date: RwLock::new(date),
             location: path.to_path_buf(),
         };
         Ok(index)
     }
@@ -166,16 +171,21 @@
         let mut state = self.write_state();
         state.remove(prefix.as_ref(), temporal_mark);
     }
     pub fn get_keys(&self, _: &Lock) -> VectorR<Vec<String>> {
         self.read_state().keys(&self.location)
     }
     pub fn search(&self, request: &dyn SearchRequest, _: &Lock) -> VectorR<Vec<Neighbour>> {
-        self.read_state()
-            .search(&self.location, request, self.metadata.similarity)
+        let state = self.read_state();
+        let given_len = request.get_query().len() as u64;
+        match self.dimension_used {
+            Some(expected) if expected != given_len => Err(VectorErr::InconsistentDimensions),
+            None => Ok(Vec::with_capacity(0)),
+            Some(_) => state.search(&self.location, request, self.metadata.similarity),
+        }
     }
     pub fn no_nodes(&self, _: &Lock) -> usize {
         self.read_state().no_nodes()
     }
     pub fn collect_garbage(&self, _: &Lock) -> VectorR<()> {
         use std::collections::HashSet;
         let work_flag = self.work_flag.try_to_start_working()?;
@@ -197,19 +207,35 @@
                 let Err(err)  = DataPoint::delete(&self.location, dpid) else { continue };
                 warn!("{name} is garbage and could not be deleted because of {err}");
             }
         }
         std::mem::drop(work_flag);
         Ok(())
     }
-    pub fn add(&self, dp: DataPoint, _: &ELock) {
+    pub fn add(&mut self, dp: DataPoint, _: &ELock) -> VectorR<()> {
         let mut state = self.write_state();
+        let Some(new_dp_vector_len) = dp.stored_len() else {
+            return Ok(());
+        };
+        let Some(state_vector_len) = self.dimension_used else {
+            // There is not a len in the state, therefore adding the datapoint can not
+            // create a merging requirement.
+            let dp_dimension = dp.stored_len();
+            let _ = state.add(dp);
+            std::mem::drop(state);
+            self.dimension_used = dp_dimension;
+            return Ok(());
+        };
+        if state_vector_len != new_dp_vector_len {
+            return Err(VectorErr::InconsistentDimensions);
+        }
         if state.add(dp) {
             self.notify_merger()
         }
+        Ok(())
     }
     pub fn commit(&self, lock: ELock) -> VectorR<()> {
         let state = self.read_state();
         let mut date = self.write_date();
         fs_state::persist_state::<State>(&lock, &state)?;
         *date = fs_state::crnt_version(&lock)?;
         Ok(())
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files 2% similar despite different names*

```diff
@@ -188,26 +188,28 @@
         request: &dyn SearchRequest,
         similarity: Similarity,
     ) -> VectorR<Vec<Neighbour>> {
         let query = request.get_query();
         let filter = request.get_filter();
         let with_duplicates = request.with_duplicates();
         let no_results = request.no_results();
+        let min_score = request.min_score();
         let mut ffsv = Fssc::new(request.no_results());
         for journal in self.data_point_iterator().copied() {
             let delete_log = self.delete_log(journal);
             let data_point = DataPoint::open(location, journal.id())?;
             data_point
                 .search(
                     &delete_log,
                     query,
                     filter,
                     with_duplicates,
                     no_results,
                     similarity,
+                    min_score,
                 )
                 .for_each(|candidate| ffsv.add(candidate));
         }
         Ok(ffsv.into())
     }
     pub fn remove(&mut self, id: &str, deleted_since: SystemTime) {
         self.delete_log.insert(id.as_bytes(), deleted_since);
@@ -266,14 +268,21 @@
     }
     pub fn work_stack_len(&mut self) -> usize {
         self.work_stack.len()
     }
     pub fn current_work_unit(&self) -> Option<&[Journal]> {
         self.work_stack.back().map(|wu| wu.load.as_slice())
     }
+    pub fn stored_len(&self, location: &Path) -> VectorR<Option<u64>> {
+        let Some(journal) = self.data_point_iterator().next() else {
+            return Ok(None);
+        };
+        let data_point = DataPoint::open(location, journal.id())?;
+        Ok(data_point.stored_len())
+    }
 }
 
 #[cfg(test)]
 mod test {
     use std::path::Path;
 
     use rand::random;
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_point_provider/work_flag.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_point_provider/work_flag.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/key_value.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/key_value.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 }
 fn encode_unit(mut buff: Vec<u8>, unit: Unit) -> Vec<u8> {
     buff.write_all(&unit.to_le_bytes()).unwrap();
     buff.flush().unwrap();
     buff
 }
 
+pub fn vector_len(mut x: &[u8]) -> u64 {
+    let mut buff_x = [0; 8];
+    x.read_exact(&mut buff_x).unwrap();
+    Len::from_le_bytes(buff_x)
+}
+
 pub fn cosine_similarity(mut x: &[u8], mut y: &[u8]) -> Dist {
     let mut buff_x = [0; 8];
     let mut buff_y = [0; 8];
     x.read_exact(&mut buff_x).unwrap();
     y.read_exact(&mut buff_y).unwrap();
     let len_x = Len::from_le_bytes(buff_x);
     let len_y = Len::from_le_bytes(buff_y);
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files 16% similar despite different names*

```diff
@@ -16,73 +16,96 @@
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 use crate::data_point::{Address, DataRetriever};
 
-/// Is a singleton clause formed by label. It will be satisfied only if the address
-/// is applied to has the label.
+#[derive(Debug, Clone, Copy)]
+pub enum AtomKind {
+    KeyPrefix,
+    Label,
+}
+
+/// Is a singleton clause.
 #[derive(Debug, Clone)]
-pub struct LabelClause {
+pub struct AtomClause {
+    kind: AtomKind,
     value: String,
 }
-impl LabelClause {
-    pub fn new(labels: String) -> LabelClause {
-        LabelClause { value: labels }
+impl AtomClause {
+    pub fn new(value: String, kind: AtomKind) -> AtomClause {
+        AtomClause { kind, value }
+    }
+    pub fn label(value: String) -> AtomClause {
+        AtomClause::new(value, AtomKind::Label)
+    }
+    pub fn key_prefix(value: String) -> AtomClause {
+        AtomClause::new(value, AtomKind::KeyPrefix)
     }
     fn run<D: DataRetriever>(&self, x: Address, retriever: &D) -> bool {
-        retriever.has_label(x, self.value.as_bytes())
+        match self.kind {
+            AtomKind::KeyPrefix => retriever.get_key(x).starts_with(self.value.as_bytes()),
+            AtomKind::Label => retriever.has_label(x, self.value.as_bytes()),
+        }
     }
 }
 
 /// Is a clause formed by the conjuction of several LabelClauses. Additionally this
-/// clause has a threshold that specifies the minimum number of LabelClauses that have to
+/// clause has a threshold that specifies the minimum number of AtomClauses that have to
 /// succeed in order for the overall conjuction to be satisfied.
 #[derive(Debug, Clone)]
 pub struct CompoundClause {
     threshold: usize,
-    labels: Vec<LabelClause>,
+    labels: Vec<AtomClause>,
 }
 impl CompoundClause {
-    pub fn new(threshold: usize, labels: Vec<LabelClause>) -> CompoundClause {
+    pub fn len(&self) -> usize {
+        self.labels.len()
+    }
+    pub fn is_empty(&self) -> bool {
+        self.labels.is_empty()
+    }
+    pub fn new(threshold: usize, labels: Vec<AtomClause>) -> CompoundClause {
         CompoundClause { threshold, labels }
     }
     fn run<D: DataRetriever>(&self, x: Address, retriever: &D) -> bool {
-        let number_of_subqueries = self.labels.len();
+        if self.is_empty() {
+            return true;
+        }
         let mut threshold = self.threshold;
         let mut i = 0;
-        while threshold > 0 && i <= number_of_subqueries {
+        while threshold > 0 && i < self.len() {
             let is_valid = self.labels[i].run(x, retriever);
             threshold -= is_valid as usize;
             i += 1;
         }
         threshold == 0
     }
 }
 
 /// Wrapper that unifies the different types of clauses a formula may have.
 #[derive(Debug, Clone)]
 pub enum Clause {
-    Label(LabelClause),
+    Atom(AtomClause),
     Compound(CompoundClause),
 }
 
 impl Clause {
     fn run<D: DataRetriever>(&self, x: Address, retriever: &D) -> bool {
         match self {
             Clause::Compound(q) => q.run(x, retriever),
-            Clause::Label(q) => q.run(x, retriever),
+            Clause::Atom(q) => q.run(x, retriever),
         }
     }
 }
 
-impl From<LabelClause> for Clause {
-    fn from(value: LabelClause) -> Self {
-        Clause::Label(value)
+impl From<AtomClause> for Clause {
+    fn from(value: AtomClause) -> Self {
+        Clause::Atom(value)
     }
 }
 
 impl From<CompoundClause> for Clause {
     fn from(value: CompoundClause) -> Self {
         Clause::Compound(value)
     }
@@ -112,51 +135,70 @@
 #[cfg(test)]
 mod tests {
     use std::collections::HashSet;
 
     use super::*;
     use crate::data_point::Address;
     struct DummyRetriever {
+        key: &'static [u8],
         labels: HashSet<&'static [u8]>,
     }
     impl DataRetriever for DummyRetriever {
+        fn get_key(&self, _: Address) -> &[u8] {
+            self.key
+        }
         fn has_label(&self, _: Address, label: &[u8]) -> bool {
             self.labels.contains(label)
         }
         fn is_deleted(&self, _: Address) -> bool {
             panic!("Not meant to be used")
         }
         fn similarity(&self, _: Address, _: Address) -> f32 {
             panic!("Not meant to be used")
         }
         fn get_vector(&self, _: Address) -> &[u8] {
             panic!("Not meant to be used")
         }
+        fn min_score(&self) -> f32 {
+            -1.0
+        }
     }
     #[test]
     fn test_query() {
+        const KEY: &str = "/This/is/a/key";
         const L1: &str = "Label1";
         const L2: &str = "Label2";
         const L3: &str = "Label3";
         const ADDRESS: Address = Address::dummy();
         let retriever = DummyRetriever {
+            key: KEY.as_bytes(),
             labels: [L1.as_bytes(), L3.as_bytes()].into_iter().collect(),
         };
         let mut formula = Formula::new();
-        formula.extend(LabelClause::new(L1.to_string()));
-        formula.extend(LabelClause::new(L3.to_string()));
+        formula.extend(AtomClause::label(L1.to_string()));
+        formula.extend(AtomClause::label(L3.to_string()));
         assert!(formula.run(ADDRESS, &retriever));
 
         let mut formula = Formula::new();
-        formula.extend(LabelClause::new(L1.to_string()));
-        formula.extend(LabelClause::new(L2.to_string()));
+        formula.extend(AtomClause::label(L1.to_string()));
+        formula.extend(AtomClause::label(L2.to_string()));
         assert!(!formula.run(ADDRESS, &retriever));
 
         let mut formula = Formula::new();
         let inner = vec![
-            LabelClause::new(L1.to_string()),
-            LabelClause::new(L2.to_string()),
+            AtomClause::label(L1.to_string()),
+            AtomClause::label(L2.to_string()),
         ];
         formula.extend(CompoundClause::new(1, inner));
         assert!(formula.run(ADDRESS, &retriever));
+
+        let mut formula = Formula::new();
+        let inner = vec![AtomClause::key_prefix("/This/is".to_string())];
+        formula.extend(CompoundClause::new(1, inner));
+        assert!(formula.run(ADDRESS, &retriever));
+        let mut formula = Formula::new();
+
+        let inner = vec![AtomClause::key_prefix("/This/is/not".to_string())];
+        formula.extend(CompoundClause::new(1, inner));
+        assert!(!formula.run(ADDRESS, &retriever));
     }
 }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/indexset/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/indexset/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/indexset/state.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/indexset/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -38,10 +38,12 @@
     WorkDelayed,
     #[error("Several writers are open at the same time ")]
     MultipleWriters,
     #[error("Merger is already initialized")]
     MergerAlreadyInitialized,
     #[error("Can not merge zero datapoints")]
     EmptyMerge,
+    #[error("Inconsistent dimensions")]
+    InconsistentDimensions,
 }
 
 pub type VectorR<O> = Result<O, VectorErr>;
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files 8% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 use std::fmt::Debug;
 use std::time::SystemTime;
 
-use nucliadb_core::context;
+use nucliadb_core::metrics;
 use nucliadb_core::metrics::request_time;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::prost::Message;
 use nucliadb_core::protos::{
     DocumentScored, DocumentVectorIdentifier, SentenceMetadata, VectorSearchRequest,
     VectorSearchResponse,
 };
 use nucliadb_core::tracing::{self, *};
 
 use crate::data_point_provider::*;
-use crate::formula::{Formula, LabelClause};
+use crate::formula::{AtomClause, CompoundClause, Formula};
 use crate::indexset::IndexSet;
 
 impl<'a> SearchRequest for (usize, &'a VectorSearchRequest, Formula) {
     fn with_duplicates(&self) -> bool {
         self.1.with_duplicates
     }
     fn get_filter(&self) -> &Formula {
@@ -43,14 +43,17 @@
     }
     fn get_query(&self) -> &[f32] {
         &self.1.vector
     }
     fn no_results(&self) -> usize {
         self.0
     }
+    fn min_score(&self) -> f32 {
+        self.1.min_score
+    }
 }
 
 pub struct VectorReaderService {
     index: Index,
     indexset: IndexSet,
 }
 impl Debug for VectorReaderService {
@@ -67,28 +70,28 @@
         let indexet_slock = self.indexset.get_slock()?;
         if vectorset.is_empty() {
             debug!("Id for the vectorset is empty");
             let index_slock = self.index.get_slock()?;
             let no_nodes = self.index.no_nodes(&index_slock);
             std::mem::drop(index_slock);
 
-            let metrics = context::get_metrics();
+            let metrics = metrics::get_metrics();
             let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
             let metric = request_time::RequestTimeKey::vectors("count".to_string());
             metrics.record_request_time(metric, took);
             debug!("Ending at {took} ms");
 
             Ok(no_nodes)
         } else if let Some(index) = self.indexset.get(vectorset, &indexet_slock)? {
             debug!("Counting nodes for {vectorset}");
             let lock = index.get_slock()?;
             let no_nodes = index.no_nodes(&lock);
             std::mem::drop(lock);
 
-            let metrics = context::get_metrics();
+            let metrics = metrics::get_metrics();
             let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
             let metric = request_time::RequestTimeKey::vectors("count".to_string());
             metrics.record_request_time(metric, took);
             debug!("Ending at {took} ms");
 
             Ok(no_nodes)
         } else {
@@ -111,21 +114,31 @@
         let id = Some(&request.id);
         let offset = request.result_per_page * request.page_number;
         let total_to_get = offset + request.result_per_page;
         let offset = offset as usize;
         let total_to_get = total_to_get as usize;
         let indexet_slock = self.indexset.get_slock()?;
         let index_slock = self.index.get_slock()?;
+
+        let key_filters = request
+            .key_filters
+            .iter()
+            .cloned()
+            .map(AtomClause::key_prefix);
         let mut formula = Formula::new();
         request
             .tags
             .iter()
             .cloned()
-            .map(LabelClause::new)
+            .map(AtomClause::label)
             .for_each(|c| formula.extend(c));
+        if key_filters.len() > 0 {
+            formula.extend(CompoundClause::new(1, key_filters.collect()));
+        }
+
         let search_request = (total_to_get, request, formula);
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Searching: starts at {v} ms");
         }
         let result = if request.vector_set.is_empty() {
             debug!("{id:?} - No vectorset specified, searching in the main index");
             self.index.search(&search_request, &index_slock)?
@@ -160,15 +173,15 @@
             .map(|(_, v)| v)
             .flat_map(DocumentScored::try_from)
             .collect::<Vec<_>>();
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Creating results: ends at {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::vectors("search".to_string());
         metrics.record_request_time(metric, took);
         debug!("{id:?} - Ending at {took} ms");
 
         Ok(VectorSearchResponse {
             documents,
@@ -339,27 +352,60 @@
             vector_set: "".to_string(),
             vector: vec![4.0, 6.0, 7.0],
             tags: vec!["1".to_string()],
             page_number: 0,
             result_per_page: 20,
             reload: false,
             with_duplicates: true,
+            ..Default::default()
         };
         let result = reader.search(&request).unwrap();
         assert_eq!(result.documents.len(), 4);
 
         let request = VectorSearchRequest {
             id: "".to_string(),
             vector_set: "".to_string(),
             vector: vec![4.0, 6.0, 7.0],
             tags: vec!["1".to_string()],
             page_number: 0,
             result_per_page: 20,
             reload: false,
             with_duplicates: false,
+            ..Default::default()
         };
         let result = reader.search(&request).unwrap();
         let no_nodes = reader.count("").unwrap();
         assert_eq!(no_nodes, 4);
         assert_eq!(result.documents.len(), 3);
+
+        // Check that min_score works
+        let request = VectorSearchRequest {
+            id: "".to_string(),
+            vector_set: "".to_string(),
+            vector: vec![4.0, 6.0, 7.0],
+            tags: vec!["1".to_string()],
+            page_number: 0,
+            result_per_page: 20,
+            reload: false,
+            with_duplicates: false,
+            min_score: 900.0,
+            ..Default::default()
+        };
+        let result = reader.search(&request).unwrap();
+        let no_nodes = reader.count("").unwrap();
+        assert_eq!(no_nodes, 4);
+        assert_eq!(result.documents.len(), 0);
+
+        let bad_request = VectorSearchRequest {
+            id: "".to_string(),
+            vector_set: "".to_string(),
+            vector: vec![4.0, 6.0],
+            tags: vec!["1".to_string()],
+            page_number: 0,
+            result_per_page: 20,
+            reload: false,
+            with_duplicates: false,
+            ..Default::default()
+        };
+        assert!(reader.search(&bad_request).is_err());
     }
 }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::time::SystemTime;
 
 use data_point::{Elem, LabelDictionary};
-use nucliadb_core::context;
+use nucliadb_core::metrics;
 use nucliadb_core::metrics::request_time;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::prost::Message;
 use nucliadb_core::protos::resource::ResourceStatus;
 use nucliadb_core::protos::{Resource, ResourceId, VectorSetId, VectorSimilarity};
 use nucliadb_core::tracing::{self, *};
 
@@ -57,15 +57,15 @@
         let time = SystemTime::now();
 
         let id: Option<String> = None;
         let mut collector = Vec::new();
         let indexset_slock = self.indexset.get_slock()?;
         self.indexset.index_keys(&mut collector, &indexset_slock);
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::vectors("list_vectorsets".to_string());
         metrics.record_request_time(metric, took);
 
         debug!("{id:?} - Ending at {took} ms");
         Ok(collector)
     }
@@ -82,15 +82,15 @@
         let indexid = setid.vectorset.as_str();
         let similarity = similarity.into();
         let indexset_elock = self.indexset.get_elock()?;
         self.indexset
             .get_or_create(indexid, similarity, &indexset_elock)?;
         self.indexset.commit(indexset_elock)?;
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::vectors("add_vectorset".to_string());
         metrics.record_request_time(metric, took);
         debug!("{id:?}/{set} - Ending at {took} ms");
 
         Ok(())
     }
@@ -101,15 +101,15 @@
         let id = setid.shard.as_ref().map(|s| &s.id);
         let set = &setid.vectorset;
         let indexid = &setid.vectorset;
         let indexset_elock = self.indexset.get_elock()?;
         self.indexset.remove_index(indexid, &indexset_elock)?;
         self.indexset.commit(indexset_elock)?;
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::vectors("remove_vectorset".to_string());
         metrics.record_request_time(metric, took);
         debug!("{id:?}/{set} - Ending at {took} ms");
 
         Ok(())
     }
@@ -125,15 +125,15 @@
         let time = SystemTime::now();
 
         let id: Option<String> = None;
         let lock = self.index.get_slock()?;
         let no_nodes = self.index.no_nodes(&lock);
         std::mem::drop(lock);
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::vectors("count".to_string());
         metrics.record_request_time(metric, took);
         debug!("{id:?} - Ending at {took} ms");
 
         Ok(no_nodes)
     }
@@ -143,15 +143,15 @@
 
         let id = Some(&resource_id.shard_id);
         let temporal_mark = TemporalMark::now();
         let lock = self.index.get_elock()?;
         self.index.delete(&resource_id.uuid, temporal_mark, &lock);
         self.index.commit(lock)?;
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::vectors("delete_resource".to_string());
         metrics.record_request_time(metric, took);
         debug!("{id:?} - Ending at {took} ms");
 
         Ok(())
     }
@@ -162,18 +162,19 @@
         let id = resource.resource.as_ref().map(|i| &i.shard_id);
         debug!("{id:?} - Updating main index");
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Creating elements for the main index: starts {v} ms");
         }
 
         let temporal_mark = TemporalMark::now();
+        let mut lengths: HashMap<usize, Vec<_>> = HashMap::new();
         let mut elems = Vec::new();
         if resource.status != ResourceStatus::Delete as i32 {
-            for (field, paragraph) in resource.paragraphs.iter() {
-                let field = &[field.clone()];
+            for (paragraph_field, paragraph) in resource.paragraphs.iter() {
+                let field = &[paragraph_field.clone()];
                 for index in paragraph.paragraphs.values() {
                     let labels = LabelDictionary::new(
                         resource
                             .labels
                             .iter()
                             .chain(index.labels.iter())
                             .chain(field.iter())
@@ -181,34 +182,39 @@
                             .collect(),
                     );
                     for (key, sentence) in index.sentences.iter().clone() {
                         let key = key.to_string();
                         let labels = labels.clone();
                         let vector = sentence.vector.clone();
                         let metadata = sentence.metadata.as_ref().map(|m| m.encode_to_vec());
+                        let bucket = lengths.entry(vector.len()).or_default();
                         elems.push(Elem::new(key, vector, labels, metadata));
+                        bucket.push(paragraph_field);
                     }
                 }
             }
         }
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Creating elements for the main index: ends {v} ms");
         }
 
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Datapoint creation: starts {v} ms");
         }
 
-        let similarity = self.index.metadata().similarity;
+        if lengths.len() > 1 {
+            return Ok(tracing::error!("{}", self.dimensions_report(lengths)));
+        }
+
         let new_dp = if !elems.is_empty() {
             Some(DataPoint::new(
                 self.index.location(),
                 elems,
                 Some(temporal_mark),
-                similarity,
+                self.index.metadata().similarity,
             )?)
         } else {
             None
         };
 
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Datapoint creation: ends {v} ms");
@@ -224,21 +230,17 @@
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Processing Sentences to delete: ends {v} ms");
         }
 
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Indexing datapoint: starts {v} ms");
         }
-        if let Some(new_dp) = new_dp {
-            debug!("{id:?} - The datapoint is not empty, adding it");
-            self.index.add(new_dp, &lock);
-            self.index.commit(lock)?;
-        } else {
-            debug!("{id:?} - The datapoint is empty, no need to add it");
-            self.index.commit(lock)?;
+        match new_dp.map(|i| self.index.add(i, &lock)).unwrap_or(Ok(())) {
+            Ok(_) => self.index.commit(lock)?,
+            Err(e) => tracing::error!("{id:?}/default could insert vectors: {e:?}"),
         }
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Indexing datapoint: ends {v} ms");
         }
 
         // Updating existing indexes
         // Perform delete operations over the vector set
@@ -276,36 +278,43 @@
             .keys()
             .map(|k| (k, self.indexset.get(k, &indexset_elock)))
             .map(|(key, index)| index.map(|index| (key, index)))
             .collect::<Result<HashMap<_, _>, _>>()?;
         self.indexset.commit(indexset_elock)?;
 
         // Inner indexes are updated
-        for (index_key, index) in indexes.into_iter().flat_map(|i| i.1.map(|j| (i.0, j))) {
+        for (index_key, mut index) in indexes.into_iter().flat_map(|i| i.1.map(|j| (i.0, j))) {
+            let mut lengths: HashMap<usize, Vec<_>> = HashMap::new();
             let mut elems = vec![];
-            for (key, user_vector) in resource.vectors[index_key].vectors.iter() {
-                let key = key.clone();
+            for (vectorset, user_vector) in resource.vectors[index_key].vectors.iter() {
+                let key = vectorset.clone();
                 let vector = user_vector.vector.clone();
+                let bucket = lengths.entry(vector.len()).or_default();
                 let labels = LabelDictionary::new(user_vector.labels.clone());
                 elems.push(Elem::new(key, vector, labels, None));
+                bucket.push(vectorset);
             }
-            if !elems.is_empty() {
+            if lengths.len() > 1 {
+                tracing::error!("vectorsets report: {}", self.dimensions_report(lengths));
+            } else if !elems.is_empty() {
                 let similarity = index.metadata().similarity;
-                let new_dp =
-                    DataPoint::new(index.location(), elems, Some(temporal_mark), similarity)?;
+                let location = index.location();
+                let new_dp = DataPoint::new(location, elems, Some(temporal_mark), similarity)?;
                 let lock = index.get_elock()?;
-                index.add(new_dp, &lock);
-                index.commit(lock)?;
+                match index.add(new_dp, &lock) {
+                    Ok(_) => index.commit(lock)?,
+                    Err(e) => tracing::error!("Could not insert at {id:?}/{index_key}: {e:?}"),
+                }
             }
         }
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Creating and geting indexes in the set: ends {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::vectors("set_resource".to_string());
         metrics.record_request_time(metric, took);
         debug!("{id:?} - Ending at {took} ms");
 
         Ok(())
     }
@@ -320,25 +329,34 @@
         for index_key in index_keys {
             let Some(index) = self.indexset.get(&index_key, &indexset_slock)? else {
                 return Err(node_error!("Unknown state for {index_key}"));
             };
             self.collect_garbage_for(&index)?;
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::vectors("garbage_collection".to_string());
         metrics.record_request_time(metric, took);
         debug!("Garbage collection {took} ms");
 
         Ok(())
     }
 }
 
 impl VectorWriterService {
+    fn dimensions_report<'a>(&'a self, dimensions: HashMap<usize, Vec<&'a String>>) -> String {
+        let mut report = String::new();
+        for (dimension, bucket) in dimensions {
+            let partial = format!("{dimension} : {bucket:?}\n");
+            report.push_str(&partial);
+        }
+        report.pop();
+        report
+    }
     fn collect_garbage_for(&self, index: &Index) -> NodeResult<()> {
         debug!("Collecting garbage for index: {:?}", index.location());
         let slock = index.get_slock()?;
         match index.collect_garbage(&slock) {
             Ok(_) => debug!("Garbage collected for main index"),
             Err(VectorErr::WorkDelayed) => debug!("Garbage collection delayed"),
             Err(e) => Err(e)?,
@@ -457,14 +475,15 @@
             vector_set: "4".to_string(),
             vector: vec![4.0, 6.0, 7.0],
             tags: vec!["4/label".to_string()],
             page_number: 0,
             result_per_page: 20,
             reload: false,
             with_duplicates: false,
+            ..Default::default()
         };
         let results = reader.search(&request).unwrap();
         let id = results.documents[0].doc_id.clone().unwrap().id;
         assert_eq!(results.documents.len(), 1);
         assert_eq!(id, "4/key");
 
         // Same set, but no label match
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/context.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files 13% similar despite different names*

```diff
@@ -9,38 +9,46 @@
 // published by the Free Software Foundation, either version 3 of the
 // License, or (at your option) any later version.
 //
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
+//
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+pub mod middleware;
+
+mod meters;
+mod metric;
+mod task_monitor;
+
 use std::sync::Arc;
 
 use lazy_static::lazy_static;
+pub use metric::request_time;
 
-use crate::metrics::{self, Metrics};
+use self::meters::Meter;
 
 lazy_static! {
-    static ref METRICS: Arc<dyn Metrics> = create_metrics();
+    static ref METRICS: Arc<dyn Meter> = create_metrics();
 }
 
 #[cfg(prometheus_metrics)]
-fn create_metrics() -> Arc<dyn Metrics> {
-    Arc::new(metrics::PrometheusMetrics::new())
+fn create_metrics() -> Arc<dyn Meter> {
+    Arc::new(meters::PrometheusMeter::new())
 }
 
 #[cfg(log_metrics)]
-fn create_metrics() -> Arc<dyn Metrics> {
-    Arc::new(metrics::ConsoleLogMetrics)
+fn create_metrics() -> Arc<dyn Meter> {
+    Arc::new(meters::ConsoleMeter)
 }
 
 #[cfg(not(any(prometheus_metrics, log_metrics)))]
-fn create_metrics() -> Arc<dyn Metrics> {
-    Arc::new(metrics::NoMetrics)
+fn create_metrics() -> Arc<dyn Meter> {
+    Arc::new(meters::NoOpMeter)
 }
 
-pub fn get_metrics() -> Arc<dyn Metrics> {
+pub fn get_metrics() -> Arc<dyn Meter> {
     Arc::clone(&METRICS)
 }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,23 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
-pub mod context;
 pub mod fs_state;
 pub mod metrics;
 pub mod paragraphs;
 pub mod relations;
 pub mod texts;
 pub mod vectors;
 use std::sync::{Arc, RwLock, RwLockReadGuard, RwLockWriteGuard};
 
-pub use anyhow::{anyhow as node_error, Context};
+pub use anyhow::{anyhow as node_error, Context, Error};
 use nucliadb_protos::{Resource, ResourceId};
 pub type NodeResult<O> = anyhow::Result<O>;
 
 pub fn paragraph_write(
     x: &paragraphs::ParagraphsWriterPointer,
 ) -> RwLockWriteGuard<'_, dyn paragraphs::ParagraphWriter + 'static> {
     x.write().unwrap_or_else(|l| l.into_inner())
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files 25% similar despite different names*

```diff
@@ -9,109 +9,80 @@
 // published by the Free Software Foundation, either version 3 of the
 // License, or (at your option) any later version.
 //
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
+//
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-use std::fmt::Debug;
-
 use prometheus_client::encoding;
 use prometheus_client::registry::Registry;
 
-use crate::{tracing, NodeResult};
-// metrics
-// Every metric must be define in its own module, which must fulfill the following requirements:
-// - The name of the module must be the name of the name of the metric.
-// - If the metric is called SomeName, then there must be a type 'SomeNameMetric' describing such
-//   metric.
-// - If the metric is called SomeName, a function 'register_some_name' must be defined and its job
-//   is to recive a registry, register there the metric and return such metric.
-// - If the metric is called SomeName, a struct 'SomeNameKey' must be defined.
-// - If the metric is called SomeName, a struct 'SomeNameValue' must be defined.
-pub mod request_time;
-
-pub trait Metrics: Send + Sync {
-    fn collect(&self) -> NodeResult<String>;
-    fn record_request_time(
-        &self,
-        metric: request_time::RequestTimeKey,
-        value: request_time::RequestTimeValue,
-    );
-}
+use crate::metrics::meters::Meter;
+use crate::metrics::metric::tokio_tasks::TaskLabels;
+use crate::metrics::metric::{request_time, tokio_tasks};
+use crate::metrics::task_monitor::{Monitor, MultiTaskMonitor, TaskId};
+use crate::NodeResult;
 
-pub struct PrometheusMetrics {
+pub struct PrometheusMeter {
     registry: Registry,
     request_time_metric: request_time::RequestTimeMetric,
+    tokio_task_metrics: tokio_tasks::TokioTaskMetrics,
+    tasks_monitor: MultiTaskMonitor,
 }
 
-impl Default for PrometheusMetrics {
+impl Default for PrometheusMeter {
     fn default() -> Self {
         Self::new()
     }
 }
 
-impl Metrics for PrometheusMetrics {
-    fn collect(&self) -> NodeResult<String> {
+impl Meter for PrometheusMeter {
+    fn export(&self) -> NodeResult<String> {
+        self.tasks_monitor
+            .export_all()
+            .for_each(|(task_id, metrics)| {
+                let labels = TaskLabels { request: task_id };
+                self.tokio_task_metrics.collect(labels, metrics.to_owned());
+            });
+
         let mut buf = String::new();
         encoding::text::encode(&mut buf, &self.registry)?;
         Ok(buf)
     }
+
     fn record_request_time(
         &self,
         metric: request_time::RequestTimeKey,
         value: request_time::RequestTimeValue,
     ) {
         self.request_time_metric
             .get_or_create(&metric)
             .observe(value);
     }
+
+    fn task_monitor(&self, task_id: TaskId) -> Option<Monitor> {
+        Some(self.tasks_monitor.task_monitor(task_id))
+    }
 }
 
-impl PrometheusMetrics {
-    pub fn new() -> PrometheusMetrics {
+impl PrometheusMeter {
+    pub fn new() -> PrometheusMeter {
         let mut registry = Registry::default();
 
         // This must be done for every metric
         let request_time_metric = request_time::register_request_time(&mut registry);
+        let tokio_task_metrics = tokio_tasks::register_tokio_task_metrics(&mut registry);
 
-        PrometheusMetrics {
+        let tasks_monitor = MultiTaskMonitor::new();
+
+        PrometheusMeter {
             registry,
             request_time_metric,
+            tokio_task_metrics,
+            tasks_monitor,
         }
     }
 }
-
-pub struct ConsoleLogMetrics;
-impl ConsoleLogMetrics {
-    fn record<Metric: Debug, Value: Debug>(&self, metric: Metric, value: Value) {
-        tracing::debug!("{metric:?} : {value:?}")
-    }
-}
-impl Metrics for ConsoleLogMetrics {
-    fn collect(&self) -> NodeResult<String> {
-        Ok(Default::default())
-    }
-    fn record_request_time(
-        &self,
-        metric: request_time::RequestTimeKey,
-        value: request_time::RequestTimeValue,
-    ) {
-        self.record(metric, value)
-    }
-}
-
-pub struct NoMetrics;
-impl Metrics for NoMetrics {
-    fn collect(&self) -> NodeResult<String> {
-        Ok(Default::default())
-    }
-    fn record_request_time(
-        &self,
-        _: request_time::RequestTimeKey,
-        _: request_time::RequestTimeValue,
-    ) {
-    }
-}
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/metrics/request_time.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 // published by the Free Software Foundation, either version 3 of the
 // License, or (at your option) any later version.
 //
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
+//
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 use prometheus_client::encoding::{EncodeLabelSet, EncodeLabelValue};
 use prometheus_client::metrics::family::Family;
 use prometheus_client::metrics::histogram::Histogram;
 use prometheus_client::registry::Registry;
@@ -55,20 +56,20 @@
         Self::new(RequestActor::Texts, request)
     }
     pub fn relations(request: String) -> RequestTimeKey {
         Self::new(RequestActor::Relations, request)
     }
 }
 
-pub(super) type RequestTimeMetric = Family<RequestTimeKey, Histogram>;
+pub type RequestTimeMetric = Family<RequestTimeKey, Histogram>;
 const BUCKETS: [f64; 12] = [
     0.005, 0.01, 0.025, 0.05, 0.1, 0.25, 0.5, 2.5, 5.0, 10.0, 30.0, 60.0,
 ];
 
-pub(super) fn register_request_time(registry: &mut Registry) -> RequestTimeMetric {
+pub fn register_request_time(registry: &mut Registry) -> RequestTimeMetric {
     let constructor = || Histogram::new(BUCKETS.iter().copied());
     let metric = RequestTimeMetric::new_with_constructor(constructor);
     registry.register(
         "node_requests",
         "Time an actor took to process the given request",
         metric.clone(),
     );
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/Cargo.toml` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/bfs_engine.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/bfs_engine.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/errors.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/graph_db.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/graph_db.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/graph_test_utils.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/graph_test_utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/index.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/index.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/lib.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/node_dictionary.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/node_dictionary.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/relations_io.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/relations_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/bfs.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/bfs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/mod.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shards/unbounded_cache_provider/async_unbounded_writer.rs`

 * *Files 12% similar despite different names*

```diff
@@ -12,18 +12,7 @@
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
-//
-
-mod bfs;
-pub mod reader;
-#[cfg(test)]
-mod tests;
-mod utils;
-pub mod writer;
-
-pub use reader::*;
-pub use writer::*;
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/reader.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 use std::collections::HashSet;
 use std::fmt::Debug;
 use std::time::SystemTime;
 
-use nucliadb_core::context;
+use nucliadb_core::metrics;
 use nucliadb_core::metrics::request_time;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::*;
 use nucliadb_core::tracing::{self, *};
 
 use super::bfs::GrpcGuide;
 use super::utils::*;
@@ -225,15 +225,15 @@
 
         let result = Ok(self
             .index
             .start_reading()
             .and_then(|reader| reader.no_nodes())
             .map(|v| v as usize)?);
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::relations("count".to_string());
         metrics.record_request_time(metric, took);
 
         result
     }
     #[tracing::instrument(skip_all)]
@@ -260,15 +260,15 @@
                 });
             }
         }
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Ending at {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::relations("get_edges".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(EdgeList { list: edges })
     }
     #[tracing::instrument(skip_all)]
@@ -295,15 +295,15 @@
                 });
             }
         }
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Ending at {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::relations("get_node_types".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(TypeList { list: types })
     }
 }
@@ -321,15 +321,15 @@
         let time = SystemTime::now();
 
         let result = Ok(RelationSearchResponse {
             subgraph: self.graph_search(request)?,
             prefix: self.prefix_search(request)?,
         });
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::relations("search".to_string());
         metrics.record_request_time(metric, took);
 
         result
     }
     #[tracing::instrument(skip_all)]
@@ -340,15 +340,15 @@
         let ids = reader
             .iter_node_ids()?
             .filter_map(|node| node.ok())
             .filter_map(|id| reader.get_node(id).ok())
             .map(|s| format!("{s:?}"))
             .collect();
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::relations("stored_ids".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(ids)
     }
     #[tracing::instrument(skip_all)]
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/tests.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/utils.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_relations/src/service/writer.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_relations/src/service/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 use std::collections::HashMap;
 use std::time::SystemTime;
 
-use nucliadb_core::context;
+use nucliadb_core::metrics;
 use nucliadb_core::metrics::request_time;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::resource::ResourceStatus;
 use nucliadb_core::protos::{DeleteGraphNodes, JoinGraph, Resource, ResourceId};
 use nucliadb_core::tracing::{self, *};
 
 use super::utils::*;
@@ -68,15 +68,15 @@
             let node = IoNode::new(name, xtype.to_string(), subtype.map(|s| s.to_string()));
             if let Some(id) = writer.get_node_id(node.hash())? {
                 self.delete_node(&mut writer, id)?;
             }
         }
         let result = Ok(writer.commit(&mut self.wmode)?);
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::relations("delete_nodes".to_string());
         metrics.record_request_time(metric, took);
         debug!("{id:?} - Ending at {took} ms");
 
         result
     }
@@ -127,15 +127,15 @@
         }
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("Ending at {v} ms")
         }
 
         let result = Ok(writer.commit(&mut self.wmode)?);
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::relations("join_graph".to_string());
         metrics.record_request_time(metric, took);
 
         result
     }
 }
@@ -162,15 +162,15 @@
             .index
             .start_reading()
             .and_then(|reader| reader.no_nodes())?;
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("Ending at {v} ms")
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::relations("count".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(count as usize)
     }
     #[tracing::instrument(skip_all)]
@@ -183,15 +183,15 @@
         if let Some(id) = writer.get_node_id(node.hash())? {
             self.delete_node(&mut writer, id)?;
         }
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Ending at {v} ms")
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::relations("delete_resource".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(())
     }
     #[tracing::instrument(skip_all)]
@@ -233,15 +233,15 @@
                 debug!("{id:?} - Populating the graph: ends {v} ms");
             }
         }
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Ending at {v} ms")
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::relations("set_resource".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(())
     }
     fn garbage_collection(&mut self) -> NodeResult<()> {
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/Cargo.toml` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,16 @@
     #[prost(int64, tag="34")]
     pub account_seq: i64,
     #[prost(message, repeated, tag="35")]
     pub user_vectors: ::prost::alloc::vec::Vec<super::resources::UserVectorsWrapper>,
     /// If true, force reindex all paragraphs in a resource
     #[prost(bool, tag="36")]
     pub reindex: bool,
+    #[prost(message, optional, tag="37")]
+    pub extra: ::core::option::Option<super::resources::Extra>,
 }
 /// Nested message and enum types in `BrokerMessage`.
 pub mod broker_message {
     #[derive(Clone, Copy, Debug, PartialEq, Eq, Hash, PartialOrd, Ord, ::prost::Enumeration)]
     #[repr(i32)]
     pub enum MessageType {
         Autocommit = 0,
@@ -454,22 +456,35 @@
     pub uuid: ::prost::alloc::string::String,
     #[prost(string, tag="4")]
     pub kbid: ::prost::alloc::string::String,
     #[prost(int64, tag="5")]
     pub seqid: i64,
     #[prost(enumeration="notification::Action", tag="6")]
     pub action: i32,
+    #[prost(enumeration="notification::WriteType", tag="7")]
+    pub write_type: i32,
+    #[prost(message, optional, tag="8")]
+    pub message: ::core::option::Option<BrokerMessage>,
 }
 /// Nested message and enum types in `Notification`.
 pub mod notification {
     #[derive(Clone, Copy, Debug, PartialEq, Eq, Hash, PartialOrd, Ord, ::prost::Enumeration)]
     #[repr(i32)]
     pub enum Action {
         Commit = 0,
         Abort = 1,
+        Indexed = 2,
+    }
+    #[derive(Clone, Copy, Debug, PartialEq, Eq, Hash, PartialOrd, Ord, ::prost::Enumeration)]
+    #[repr(i32)]
+    pub enum WriteType {
+        Unset = 0,
+        Created = 1,
+        Modified = 2,
+        Deleted = 3,
     }
 }
 //// The member information.
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct Member {
     //// Member ID.　A string of the UUID.
     #[prost(string, tag="1")]
@@ -484,14 +499,15 @@
     //// Io, Ingest, Search, Train.
     #[prost(enumeration="member::Type", tag="4")]
     pub r#type: i32,
     //// Dummy Member
     #[prost(bool, tag="5")]
     pub dummy: bool,
     //// The load score of the member.
+    #[deprecated]
     #[prost(float, tag="6")]
     pub load_score: f32,
     //// The number of shards in the node.
     #[prost(uint32, tag="7")]
     pub shard_count: u32,
 }
 /// Nested message and enum types in `Member`.
@@ -511,28 +527,19 @@
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct ListMembersResponse {
     #[prost(message, repeated, tag="1")]
     pub members: ::prost::alloc::vec::Vec<Member>,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
-pub struct ShadowShard {
-    #[prost(message, optional, tag="1")]
-    pub shard: ::core::option::Option<super::noderesources::ShardId>,
-    #[prost(string, tag="2")]
-    pub node: ::prost::alloc::string::String,
-}
-#[derive(Clone, PartialEq, ::prost::Message)]
 pub struct ShardReplica {
     #[prost(message, optional, tag="1")]
     pub shard: ::core::option::Option<super::noderesources::ShardCreated>,
     #[prost(string, tag="2")]
     pub node: ::prost::alloc::string::String,
-    #[prost(message, optional, tag="3")]
-    pub shadow_replica: ::core::option::Option<ShadowShard>,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct ShardObject {
     #[prost(string, tag="1")]
     pub shard: ::prost::alloc::string::String,
     #[prost(message, repeated, tag="3")]
     pub replicas: ::prost::alloc::vec::Vec<ShardReplica>,
@@ -654,38 +661,14 @@
         Payload(::prost::alloc::vec::Vec<u8>),
     }
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct FileUploaded {
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
-pub struct CreateShadowShardRequest {
-    #[prost(string, tag="1")]
-    pub kbid: ::prost::alloc::string::String,
-    #[prost(message, optional, tag="2")]
-    pub replica: ::core::option::Option<super::noderesources::ShardId>,
-    /// node where the shadow shard is created
-    #[prost(string, tag="3")]
-    pub node: ::prost::alloc::string::String,
-}
-#[derive(Clone, PartialEq, ::prost::Message)]
-pub struct DeleteShadowShardRequest {
-    #[prost(string, tag="1")]
-    pub kbid: ::prost::alloc::string::String,
-    #[prost(message, optional, tag="2")]
-    pub replica: ::core::option::Option<super::noderesources::ShardId>,
-}
-#[derive(Clone, PartialEq, ::prost::Message)]
-pub struct ShadowShardResponse {
-    #[prost(message, optional, tag="1")]
-    pub shadow_shard: ::core::option::Option<ShadowShard>,
-    #[prost(bool, tag="2")]
-    pub success: bool,
-}
-#[derive(Clone, PartialEq, ::prost::Message)]
 pub struct SynonymsRequest {
     #[prost(string, tag="1")]
     pub kbid: ::prost::alloc::string::String,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct SetSynonymsRequest {
     #[prost(message, optional, tag="1")]
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files 4% similar despite different names*

```diff
@@ -130,14 +130,16 @@
     pub reload: bool,
     #[prost(bool, tag="14")]
     pub with_duplicates: bool,
     #[prost(bool, tag="15")]
     pub only_faceted: bool,
     #[prost(string, optional, tag="16")]
     pub advanced_query: ::core::option::Option<::prost::alloc::string::String>,
+    #[prost(string, repeated, tag="17")]
+    pub key_filters: ::prost::alloc::vec::Vec<::prost::alloc::string::String>,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct ResultScore {
     #[prost(float, tag="1")]
     pub bm25: f32,
     /// In the case of two equal bm25 scores, booster 
     /// decides
@@ -232,34 +234,38 @@
     pub ematches: ::prost::alloc::vec::Vec<::prost::alloc::string::String>,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct VectorSearchRequest {
     ///Shard ID
     #[prost(string, tag="1")]
     pub id: ::prost::alloc::string::String,
-    /// ID for the vector set.
-    /// Empty for searching on the original index
-    #[prost(string, tag="15")]
-    pub vector_set: ::prost::alloc::string::String,
     /// Embedded vector search.
     #[prost(float, repeated, tag="2")]
     pub vector: ::prost::alloc::vec::Vec<f32>,
     /// tags to filter
     #[prost(string, repeated, tag="3")]
     pub tags: ::prost::alloc::vec::Vec<::prost::alloc::string::String>,
     /// What page is the answer.
     #[prost(int32, tag="4")]
     pub page_number: i32,
     /// How many results are in this page.
     #[prost(int32, tag="5")]
     pub result_per_page: i32,
-    #[prost(bool, tag="14")]
-    pub with_duplicates: bool,
     #[prost(bool, tag="13")]
     pub reload: bool,
+    #[prost(bool, tag="14")]
+    pub with_duplicates: bool,
+    /// ID for the vector set.
+    /// Empty for searching on the original index
+    #[prost(string, tag="15")]
+    pub vector_set: ::prost::alloc::string::String,
+    #[prost(string, repeated, tag="16")]
+    pub key_filters: ::prost::alloc::vec::Vec<::prost::alloc::string::String>,
+    #[prost(float, tag="17")]
+    pub min_score: f32,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct DocumentVectorIdentifier {
     #[prost(string, tag="1")]
     pub id: ::prost::alloc::string::String,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
@@ -417,14 +423,18 @@
     #[deprecated]
     #[prost(message, optional, tag="19")]
     pub relations: ::core::option::Option<RelationSearchRequest>,
     #[prost(message, optional, tag="20")]
     pub relation_prefix: ::core::option::Option<RelationPrefixSearchRequest>,
     #[prost(message, optional, tag="21")]
     pub relation_subgraph: ::core::option::Option<EntitiesSubgraphRequest>,
+    #[prost(string, repeated, tag="22")]
+    pub key_filters: ::prost::alloc::vec::Vec<::prost::alloc::string::String>,
+    #[prost(float, tag="23")]
+    pub min_score: f32,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct SuggestRequest {
     #[prost(string, tag="1")]
     pub shard: ::prost::alloc::string::String,
     #[prost(string, tag="2")]
     pub body: ::prost::alloc::string::String,
@@ -611,36 +621,14 @@
                 })?;
             let codec = tonic::codec::ProstCodec::default();
             let path = http::uri::PathAndQuery::from_static(
                 "/nodereader.NodeReader/GetShard",
             );
             self.inner.unary(request.into_request(), path, codec).await
         }
-        pub async fn get_shards(
-            &mut self,
-            request: impl tonic::IntoRequest<super::super::noderesources::EmptyQuery>,
-        ) -> Result<
-            tonic::Response<super::super::noderesources::ShardList>,
-            tonic::Status,
-        > {
-            self.inner
-                .ready()
-                .await
-                .map_err(|e| {
-                    tonic::Status::new(
-                        tonic::Code::Unknown,
-                        format!("Service was not ready: {}", e.into()),
-                    )
-                })?;
-            let codec = tonic::codec::ProstCodec::default();
-            let path = http::uri::PathAndQuery::from_static(
-                "/nodereader.NodeReader/GetShards",
-            );
-            self.inner.unary(request.into_request(), path, codec).await
-        }
         pub async fn document_search(
             &mut self,
             request: impl tonic::IntoRequest<super::DocumentSearchRequest>,
         ) -> Result<tonic::Response<super::DocumentSearchResponse>, tonic::Status> {
             self.inner
                 .ready()
                 .await
@@ -919,21 +907,14 @@
     ///Generated trait containing gRPC methods that should be implemented for use with NodeReaderServer.
     #[async_trait]
     pub trait NodeReader: Send + Sync + 'static {
         async fn get_shard(
             &self,
             request: tonic::Request<super::GetShardRequest>,
         ) -> Result<tonic::Response<super::super::noderesources::Shard>, tonic::Status>;
-        async fn get_shards(
-            &self,
-            request: tonic::Request<super::super::noderesources::EmptyQuery>,
-        ) -> Result<
-            tonic::Response<super::super::noderesources::ShardList>,
-            tonic::Status,
-        >;
         async fn document_search(
             &self,
             request: tonic::Request<super::DocumentSearchRequest>,
         ) -> Result<tonic::Response<super::DocumentSearchResponse>, tonic::Status>;
         async fn paragraph_search(
             &self,
             request: tonic::Request<super::ParagraphSearchRequest>,
@@ -1077,55 +1058,14 @@
                         let codec = tonic::codec::ProstCodec::default();
                         let mut grpc = tonic::server::Grpc::new(codec)
                             .apply_compression_config(
                                 accept_compression_encodings,
                                 send_compression_encodings,
                             );
                         let res = grpc.unary(method, req).await;
-                        Ok(res)
-                    };
-                    Box::pin(fut)
-                }
-                "/nodereader.NodeReader/GetShards" => {
-                    #[allow(non_camel_case_types)]
-                    struct GetShardsSvc<T: NodeReader>(pub Arc<T>);
-                    impl<
-                        T: NodeReader,
-                    > tonic::server::UnaryService<
-                        super::super::noderesources::EmptyQuery,
-                    > for GetShardsSvc<T> {
-                        type Response = super::super::noderesources::ShardList;
-                        type Future = BoxFuture<
-                            tonic::Response<Self::Response>,
-                            tonic::Status,
-                        >;
-                        fn call(
-                            &mut self,
-                            request: tonic::Request<
-                                super::super::noderesources::EmptyQuery,
-                            >,
-                        ) -> Self::Future {
-                            let inner = self.0.clone();
-                            let fut = async move { (*inner).get_shards(request).await };
-                            Box::pin(fut)
-                        }
-                    }
-                    let accept_compression_encodings = self.accept_compression_encodings;
-                    let send_compression_encodings = self.send_compression_encodings;
-                    let inner = self.inner.clone();
-                    let fut = async move {
-                        let inner = inner.0;
-                        let method = GetShardsSvc(inner);
-                        let codec = tonic::codec::ProstCodec::default();
-                        let mut grpc = tonic::server::Grpc::new(codec)
-                            .apply_compression_config(
-                                accept_compression_encodings,
-                                send_compression_encodings,
-                            );
-                        let res = grpc.unary(method, req).await;
                         Ok(res)
                     };
                     Box::pin(fut)
                 }
                 "/nodereader.NodeReader/DocumentSearch" => {
                     #[allow(non_camel_case_types)]
                     struct DocumentSearchSvc<T: NodeReader>(pub Arc<T>);
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files 1% similar despite different names*

```diff
@@ -92,19 +92,14 @@
     pub resources: u64,
     #[prost(uint64, tag="3")]
     pub paragraphs: u64,
     #[prost(uint64, tag="4")]
     pub sentences: u64,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
-pub struct ShardList {
-    #[prost(message, repeated, tag="1")]
-    pub shards: ::prost::alloc::vec::Vec<Shard>,
-}
-#[derive(Clone, PartialEq, ::prost::Message)]
 pub struct EmptyResponse {
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct EmptyQuery {
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct Position {
@@ -234,33 +229,37 @@
     #[repr(i32)]
     pub enum ResourceStatus {
         Processed = 0,
         Empty = 1,
         Error = 2,
         Delete = 3,
         Pending = 4,
+        Blocked = 5,
+        Expired = 6,
     }
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct ShardMetadata {
     #[prost(string, tag="1")]
     pub kbid: ::prost::alloc::string::String,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct NodeMetadata {
+    #[deprecated]
     #[prost(float, tag="1")]
     pub load_score: f32,
     #[prost(uint64, tag="2")]
     pub shard_count: u64,
     #[prost(map="string, message", tag="3")]
     pub shards: ::std::collections::HashMap<::prost::alloc::string::String, node_metadata::ShardMetadata>,
 }
 /// Nested message and enum types in `NodeMetadata`.
 pub mod node_metadata {
     #[derive(Clone, PartialEq, ::prost::Message)]
     pub struct ShardMetadata {
         #[prost(string, tag="1")]
         pub kbid: ::prost::alloc::string::String,
+        #[deprecated]
         #[prost(float, tag="2")]
         pub load_score: f32,
     }
 }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files 7% similar despite different names*

```diff
@@ -38,29 +38,16 @@
     pub typemessage: i32,
     #[prost(string, tag="6")]
     pub reindex_id: ::prost::alloc::string::String,
     #[prost(string, optional, tag="7")]
     pub partition: ::core::option::Option<::prost::alloc::string::String>,
     #[prost(string, tag="8")]
     pub storage_key: ::prost::alloc::string::String,
-}
-#[derive(Clone, PartialEq, ::prost::Message)]
-pub struct IndexedMessage {
-    #[prost(string, tag="1")]
-    pub node: ::prost::alloc::string::String,
-    #[prost(string, tag="2")]
-    pub shard: ::prost::alloc::string::String,
-    #[prost(uint64, tag="3")]
-    pub txid: u64,
-    #[prost(string, tag="4")]
-    pub resource: ::prost::alloc::string::String,
-    #[prost(enumeration="TypeMessage", tag="5")]
-    pub typemessage: i32,
-    #[prost(string, tag="6")]
-    pub reindex_id: ::prost::alloc::string::String,
+    #[prost(string, tag="9")]
+    pub kbid: ::prost::alloc::string::String,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct SetGraph {
     #[prost(message, optional, tag="1")]
     pub shard_id: ::core::option::Option<super::noderesources::ShardId>,
     #[prost(message, optional, tag="2")]
     pub graph: ::core::option::Option<super::utils::JoinGraph>,
@@ -69,30 +56,14 @@
 pub struct DeleteGraphNodes {
     #[prost(message, optional, tag="2")]
     pub shard_id: ::core::option::Option<super::noderesources::ShardId>,
     #[prost(message, repeated, tag="1")]
     pub nodes: ::prost::alloc::vec::Vec<super::utils::RelationNode>,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
-pub struct MoveShardRequest {
-    #[prost(message, optional, tag="1")]
-    pub shard_id: ::core::option::Option<super::noderesources::ShardId>,
-    #[prost(string, tag="2")]
-    pub address: ::prost::alloc::string::String,
-}
-#[derive(Clone, PartialEq, ::prost::Message)]
-pub struct AcceptShardRequest {
-    #[prost(message, optional, tag="1")]
-    pub shard_id: ::core::option::Option<super::noderesources::ShardId>,
-    #[prost(uint32, tag="2")]
-    pub port: u32,
-    #[prost(bool, tag="3")]
-    pub override_shard: bool,
-}
-#[derive(Clone, PartialEq, ::prost::Message)]
 pub struct NewShardRequest {
     #[prost(enumeration="super::utils::VectorSimilarity", tag="1")]
     pub similarity: i32,
     #[prost(string, tag="2")]
     pub kbid: ::prost::alloc::string::String,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
@@ -170,36 +141,14 @@
         }
         /// Enable decompressing responses with `gzip`.
         #[must_use]
         pub fn accept_gzip(mut self) -> Self {
             self.inner = self.inner.accept_gzip();
             self
         }
-        pub async fn get_shard(
-            &mut self,
-            request: impl tonic::IntoRequest<super::super::noderesources::ShardId>,
-        ) -> Result<
-            tonic::Response<super::super::noderesources::ShardId>,
-            tonic::Status,
-        > {
-            self.inner
-                .ready()
-                .await
-                .map_err(|e| {
-                    tonic::Status::new(
-                        tonic::Code::Unknown,
-                        format!("Service was not ready: {}", e.into()),
-                    )
-                })?;
-            let codec = tonic::codec::ProstCodec::default();
-            let path = http::uri::PathAndQuery::from_static(
-                "/nodewriter.NodeWriter/GetShard",
-            );
-            self.inner.unary(request.into_request(), path, codec).await
-        }
         pub async fn new_shard(
             &mut self,
             request: impl tonic::IntoRequest<super::NewShardRequest>,
         ) -> Result<
             tonic::Response<super::super::noderesources::ShardCreated>,
             tonic::Status,
         > {
@@ -436,58 +385,14 @@
                 })?;
             let codec = tonic::codec::ProstCodec::default();
             let path = http::uri::PathAndQuery::from_static(
                 "/nodewriter.NodeWriter/ListVectorSets",
             );
             self.inner.unary(request.into_request(), path, codec).await
         }
-        pub async fn move_shard(
-            &mut self,
-            request: impl tonic::IntoRequest<super::MoveShardRequest>,
-        ) -> Result<
-            tonic::Response<super::super::noderesources::EmptyResponse>,
-            tonic::Status,
-        > {
-            self.inner
-                .ready()
-                .await
-                .map_err(|e| {
-                    tonic::Status::new(
-                        tonic::Code::Unknown,
-                        format!("Service was not ready: {}", e.into()),
-                    )
-                })?;
-            let codec = tonic::codec::ProstCodec::default();
-            let path = http::uri::PathAndQuery::from_static(
-                "/nodewriter.NodeWriter/MoveShard",
-            );
-            self.inner.unary(request.into_request(), path, codec).await
-        }
-        pub async fn accept_shard(
-            &mut self,
-            request: impl tonic::IntoRequest<super::AcceptShardRequest>,
-        ) -> Result<
-            tonic::Response<super::super::noderesources::EmptyResponse>,
-            tonic::Status,
-        > {
-            self.inner
-                .ready()
-                .await
-                .map_err(|e| {
-                    tonic::Status::new(
-                        tonic::Code::Unknown,
-                        format!("Service was not ready: {}", e.into()),
-                    )
-                })?;
-            let codec = tonic::codec::ProstCodec::default();
-            let path = http::uri::PathAndQuery::from_static(
-                "/nodewriter.NodeWriter/AcceptShard",
-            );
-            self.inner.unary(request.into_request(), path, codec).await
-        }
         pub async fn get_metadata(
             &mut self,
             request: impl tonic::IntoRequest<super::super::noderesources::EmptyQuery>,
         ) -> Result<
             tonic::Response<super::super::noderesources::NodeMetadata>,
             tonic::Status,
         > {
@@ -511,21 +416,14 @@
 /// Generated server implementations.
 pub mod node_writer_server {
     #![allow(unused_variables, dead_code, missing_docs, clippy::let_unit_value)]
     use tonic::codegen::*;
     ///Generated trait containing gRPC methods that should be implemented for use with NodeWriterServer.
     #[async_trait]
     pub trait NodeWriter: Send + Sync + 'static {
-        async fn get_shard(
-            &self,
-            request: tonic::Request<super::super::noderesources::ShardId>,
-        ) -> Result<
-            tonic::Response<super::super::noderesources::ShardId>,
-            tonic::Status,
-        >;
         async fn new_shard(
             &self,
             request: tonic::Request<super::NewShardRequest>,
         ) -> Result<
             tonic::Response<super::super::noderesources::ShardCreated>,
             tonic::Status,
         >;
@@ -584,28 +482,14 @@
         async fn list_vector_sets(
             &self,
             request: tonic::Request<super::super::noderesources::ShardId>,
         ) -> Result<
             tonic::Response<super::super::noderesources::VectorSetList>,
             tonic::Status,
         >;
-        async fn move_shard(
-            &self,
-            request: tonic::Request<super::MoveShardRequest>,
-        ) -> Result<
-            tonic::Response<super::super::noderesources::EmptyResponse>,
-            tonic::Status,
-        >;
-        async fn accept_shard(
-            &self,
-            request: tonic::Request<super::AcceptShardRequest>,
-        ) -> Result<
-            tonic::Response<super::super::noderesources::EmptyResponse>,
-            tonic::Status,
-        >;
         async fn get_metadata(
             &self,
             request: tonic::Request<super::super::noderesources::EmptyQuery>,
         ) -> Result<
             tonic::Response<super::super::noderesources::NodeMetadata>,
             tonic::Status,
         >;
@@ -653,52 +537,14 @@
             _cx: &mut Context<'_>,
         ) -> Poll<Result<(), Self::Error>> {
             Poll::Ready(Ok(()))
         }
         fn call(&mut self, req: http::Request<B>) -> Self::Future {
             let inner = self.inner.clone();
             match req.uri().path() {
-                "/nodewriter.NodeWriter/GetShard" => {
-                    #[allow(non_camel_case_types)]
-                    struct GetShardSvc<T: NodeWriter>(pub Arc<T>);
-                    impl<
-                        T: NodeWriter,
-                    > tonic::server::UnaryService<super::super::noderesources::ShardId>
-                    for GetShardSvc<T> {
-                        type Response = super::super::noderesources::ShardId;
-                        type Future = BoxFuture<
-                            tonic::Response<Self::Response>,
-                            tonic::Status,
-                        >;
-                        fn call(
-                            &mut self,
-                            request: tonic::Request<super::super::noderesources::ShardId>,
-                        ) -> Self::Future {
-                            let inner = self.0.clone();
-                            let fut = async move { (*inner).get_shard(request).await };
-                            Box::pin(fut)
-                        }
-                    }
-                    let accept_compression_encodings = self.accept_compression_encodings;
-                    let send_compression_encodings = self.send_compression_encodings;
-                    let inner = self.inner.clone();
-                    let fut = async move {
-                        let inner = inner.0;
-                        let method = GetShardSvc(inner);
-                        let codec = tonic::codec::ProstCodec::default();
-                        let mut grpc = tonic::server::Grpc::new(codec)
-                            .apply_compression_config(
-                                accept_compression_encodings,
-                                send_compression_encodings,
-                            );
-                        let res = grpc.unary(method, req).await;
-                        Ok(res)
-                    };
-                    Box::pin(fut)
-                }
                 "/nodewriter.NodeWriter/NewShard" => {
                     #[allow(non_camel_case_types)]
                     struct NewShardSvc<T: NodeWriter>(pub Arc<T>);
                     impl<
                         T: NodeWriter,
                     > tonic::server::UnaryService<super::NewShardRequest>
                     for NewShardSvc<T> {
@@ -1168,92 +1014,14 @@
                         let codec = tonic::codec::ProstCodec::default();
                         let mut grpc = tonic::server::Grpc::new(codec)
                             .apply_compression_config(
                                 accept_compression_encodings,
                                 send_compression_encodings,
                             );
                         let res = grpc.unary(method, req).await;
-                        Ok(res)
-                    };
-                    Box::pin(fut)
-                }
-                "/nodewriter.NodeWriter/MoveShard" => {
-                    #[allow(non_camel_case_types)]
-                    struct MoveShardSvc<T: NodeWriter>(pub Arc<T>);
-                    impl<
-                        T: NodeWriter,
-                    > tonic::server::UnaryService<super::MoveShardRequest>
-                    for MoveShardSvc<T> {
-                        type Response = super::super::noderesources::EmptyResponse;
-                        type Future = BoxFuture<
-                            tonic::Response<Self::Response>,
-                            tonic::Status,
-                        >;
-                        fn call(
-                            &mut self,
-                            request: tonic::Request<super::MoveShardRequest>,
-                        ) -> Self::Future {
-                            let inner = self.0.clone();
-                            let fut = async move { (*inner).move_shard(request).await };
-                            Box::pin(fut)
-                        }
-                    }
-                    let accept_compression_encodings = self.accept_compression_encodings;
-                    let send_compression_encodings = self.send_compression_encodings;
-                    let inner = self.inner.clone();
-                    let fut = async move {
-                        let inner = inner.0;
-                        let method = MoveShardSvc(inner);
-                        let codec = tonic::codec::ProstCodec::default();
-                        let mut grpc = tonic::server::Grpc::new(codec)
-                            .apply_compression_config(
-                                accept_compression_encodings,
-                                send_compression_encodings,
-                            );
-                        let res = grpc.unary(method, req).await;
-                        Ok(res)
-                    };
-                    Box::pin(fut)
-                }
-                "/nodewriter.NodeWriter/AcceptShard" => {
-                    #[allow(non_camel_case_types)]
-                    struct AcceptShardSvc<T: NodeWriter>(pub Arc<T>);
-                    impl<
-                        T: NodeWriter,
-                    > tonic::server::UnaryService<super::AcceptShardRequest>
-                    for AcceptShardSvc<T> {
-                        type Response = super::super::noderesources::EmptyResponse;
-                        type Future = BoxFuture<
-                            tonic::Response<Self::Response>,
-                            tonic::Status,
-                        >;
-                        fn call(
-                            &mut self,
-                            request: tonic::Request<super::AcceptShardRequest>,
-                        ) -> Self::Future {
-                            let inner = self.0.clone();
-                            let fut = async move {
-                                (*inner).accept_shard(request).await
-                            };
-                            Box::pin(fut)
-                        }
-                    }
-                    let accept_compression_encodings = self.accept_compression_encodings;
-                    let send_compression_encodings = self.send_compression_encodings;
-                    let inner = self.inner.clone();
-                    let fut = async move {
-                        let inner = inner.0;
-                        let method = AcceptShardSvc(inner);
-                        let codec = tonic::codec::ProstCodec::default();
-                        let mut grpc = tonic::server::Grpc::new(codec)
-                            .apply_compression_config(
-                                accept_compression_encodings,
-                                send_compression_encodings,
-                            );
-                        let res = grpc.unary(method, req).await;
                         Ok(res)
                     };
                     Box::pin(fut)
                 }
                 "/nodewriter.NodeWriter/GetMetadata" => {
                     #[allow(non_camel_case_types)]
                     struct GetMetadataSvc<T: NodeWriter>(pub Arc<T>);
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files 5% similar despite different names*

```diff
@@ -126,14 +126,19 @@
     pub enum Source {
         Web = 0,
         Desktop = 1,
         Api = 2,
     }
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
+pub struct Extra {
+    #[prost(message, optional, tag="1")]
+    pub metadata: ::core::option::Option<::prost_types::Struct>,
+}
+#[derive(Clone, PartialEq, ::prost::Message)]
 pub struct Relations {
     #[prost(message, repeated, tag="1")]
     pub relations: ::prost::alloc::vec::Vec<super::utils::Relation>,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct MessageContent {
     #[prost(string, tag="1")]
@@ -162,26 +167,43 @@
     pub who: ::prost::alloc::string::String,
     #[prost(string, repeated, tag="3")]
     pub to: ::prost::alloc::vec::Vec<::prost::alloc::string::String>,
     #[prost(message, optional, tag="4")]
     pub content: ::core::option::Option<MessageContent>,
     #[prost(string, tag="5")]
     pub ident: ::prost::alloc::string::String,
+    #[prost(enumeration="message::MessageType", tag="6")]
+    pub r#type: i32,
+}
+/// Nested message and enum types in `Message`.
+pub mod message {
+    #[derive(Clone, Copy, Debug, PartialEq, Eq, Hash, PartialOrd, Ord, ::prost::Enumeration)]
+    #[repr(i32)]
+    pub enum MessageType {
+        Unset = 0,
+        Question = 1,
+        Answer = 2,
+    }
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct Conversation {
     #[prost(message, repeated, tag="1")]
     pub messages: ::prost::alloc::vec::Vec<Message>,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct FieldConversation {
+    /// Total number of pages
     #[prost(int32, tag="1")]
     pub pages: i32,
+    /// Max page size
     #[prost(int32, tag="2")]
     pub size: i32,
+    /// Total number of messages
+    #[prost(int32, tag="3")]
+    pub total: i32,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct NestedPosition {
     #[prost(int64, tag="1")]
     pub start: i64,
     #[prost(int64, tag="2")]
     pub end: i64,
@@ -242,14 +264,16 @@
     pub link_image: ::core::option::Option<CloudFile>,
     #[prost(string, tag="10")]
     pub description: ::prost::alloc::string::String,
     #[prost(string, tag="11")]
     pub r#type: ::prost::alloc::string::String,
     #[prost(string, tag="12")]
     pub embed: ::prost::alloc::string::String,
+    #[prost(message, optional, tag="13")]
+    pub pdf_structure: ::core::option::Option<PageStructure>,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct ExtractedTextWrapper {
     #[prost(message, optional, tag="3")]
     pub field: ::core::option::Option<FieldId>,
     #[prost(oneof="extracted_text_wrapper::FileOrData", tags="1, 2")]
     pub file_or_data: ::core::option::Option<extracted_text_wrapper::FileOrData>,
@@ -437,14 +461,15 @@
     #[derive(Clone, Copy, Debug, PartialEq, Eq, Hash, PartialOrd, Ord, ::prost::Enumeration)]
     #[repr(i32)]
     pub enum Format {
         Plain = 0,
         Html = 1,
         Rst = 2,
         Markdown = 3,
+        Json = 4,
     }
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct Block {
     #[prost(int32, tag="1")]
     pub x: i32,
     #[prost(int32, tag="2")]
@@ -653,19 +678,62 @@
 pub struct PagePositions {
     #[prost(int64, tag="1")]
     pub start: i64,
     #[prost(int64, tag="2")]
     pub end: i64,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
+pub struct PageStructurePage {
+    #[prost(int64, tag="1")]
+    pub width: i64,
+    #[prost(int64, tag="2")]
+    pub height: i64,
+}
+#[derive(Clone, PartialEq, ::prost::Message)]
+pub struct PageStructureToken {
+    #[deprecated]
+    #[prost(int64, tag="1")]
+    pub x_deprecated: i64,
+    #[deprecated]
+    #[prost(int64, tag="2")]
+    pub y_deprecated: i64,
+    #[deprecated]
+    #[prost(int64, tag="3")]
+    pub width_deprecated: i64,
+    #[deprecated]
+    #[prost(int64, tag="4")]
+    pub height_deprecated: i64,
+    #[prost(float, tag="7")]
+    pub x: f32,
+    #[prost(float, tag="8")]
+    pub y: f32,
+    #[prost(float, tag="9")]
+    pub width: f32,
+    #[prost(float, tag="10")]
+    pub height: f32,
+    #[prost(string, tag="5")]
+    pub text: ::prost::alloc::string::String,
+    #[prost(float, tag="6")]
+    pub line: f32,
+}
+#[derive(Clone, PartialEq, ::prost::Message)]
+pub struct PageStructure {
+    #[prost(message, optional, tag="1")]
+    pub page: ::core::option::Option<PageStructurePage>,
+    #[prost(message, repeated, tag="2")]
+    pub tokens: ::prost::alloc::vec::Vec<PageStructureToken>,
+}
+#[derive(Clone, PartialEq, ::prost::Message)]
 pub struct FilePages {
     #[prost(message, repeated, tag="1")]
     pub pages: ::prost::alloc::vec::Vec<CloudFile>,
     #[prost(message, repeated, tag="2")]
     pub positions: ::prost::alloc::vec::Vec<PagePositions>,
+    #[prost(message, repeated, tag="3")]
+    pub structures: ::prost::alloc::vec::Vec<PageStructure>,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct RowsPreview {
     #[prost(map="string, message", tag="1")]
     pub sheets: ::std::collections::HashMap<::prost::alloc::string::String, rows_preview::Sheet>,
 }
 /// Nested message and enum types in `RowsPreview`.
@@ -687,14 +755,19 @@
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct FieldId {
     #[prost(enumeration="FieldType", tag="1")]
     pub field_type: i32,
     #[prost(string, tag="2")]
     pub field: ::prost::alloc::string::String,
 }
+#[derive(Clone, PartialEq, ::prost::Message)]
+pub struct AllFieldIDs {
+    #[prost(message, repeated, tag="1")]
+    pub fields: ::prost::alloc::vec::Vec<FieldId>,
+}
 #[derive(Clone, Copy, Debug, PartialEq, Eq, Hash, PartialOrd, Ord, ::prost::Enumeration)]
 #[repr(i32)]
 pub enum FieldType {
     File = 0,
     Link = 1,
     Datetime = 2,
     Keywordset = 3,
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/src/lib.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/src/reader.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/src/reader.rs`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 //
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fs;
 use std::time::*;
 
 use itertools::Itertools;
-use nucliadb_core::context;
+use nucliadb_core::metrics;
 use nucliadb_core::metrics::request_time;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::order_by::{OrderField, OrderType};
 use nucliadb_core::protos::{
     DocumentItem, DocumentResult, DocumentSearchRequest, DocumentSearchResponse, FacetResult,
     FacetResults, OrderBy, ResourceId, ResultScore, StreamRequest,
 };
@@ -128,15 +128,15 @@
     }
     #[tracing::instrument(skip_all)]
     fn search(&self, request: &Self::Request) -> NodeResult<Self::Response> {
         let time = SystemTime::now();
 
         let result = self.do_search(request);
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::texts("search".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(result?)
     }
     #[tracing::instrument(skip_all)]
@@ -153,15 +153,15 @@
             let Some(key) = searcher
                 .doc(addr)?
                 .get_first(self.schema.uuid)
                 .and_then(|i| i.as_text().map(String::from)) else { continue };
             keys.push(key);
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::texts("stored_ids".to_string());
         metrics.record_request_time(metric, took);
 
         Ok(keys)
     }
 }
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/src/schema.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/src/search_query.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_texts/src/writer.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_texts/src/writer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 use std::fmt::Debug;
 use std::fs;
 use std::time::SystemTime;
 
-use nucliadb_core::context;
+use nucliadb_core::metrics;
 use nucliadb_core::metrics::request_time;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::resource::ResourceStatus;
 use nucliadb_core::protos::{Resource, ResourceId};
 use nucliadb_core::tracing::{self, *};
 use tantivy::collector::Count;
 use tantivy::query::AllQuery;
@@ -64,28 +64,28 @@
         let time = SystemTime::now();
 
         let id: Option<String> = None;
         let reader = self.index.reader()?;
         let searcher = reader.searcher();
         let count = searcher.search(&AllQuery, &Count)?;
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::texts("count".to_string());
         metrics.record_request_time(metric, took);
         debug!("{id:?} - Ending at {took}");
 
         Ok(count)
     }
     #[tracing::instrument(skip_all)]
     fn set_resource(&mut self, resource: &Resource) -> NodeResult<()> {
         let time = SystemTime::now();
 
         let id = Some(&resource.shard_id);
-        let resource_id = resource.resource.as_ref().unwrap();
+        let resource_id = resource.resource.as_ref().expect("Missing resource ID");
 
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Delete existing uuid: starts at {v} ms");
         }
         let uuid_field = self.schema.uuid;
         let uuid_term = Term::from_field_text(uuid_field, &resource_id.uuid);
         self.writer.delete_term(uuid_term);
@@ -107,15 +107,15 @@
             debug!("{id:?} - Commit: starts at {v} ms");
         }
         self.writer.commit()?;
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Commit: ends at {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::texts("set_resource".to_string());
         metrics.record_request_time(metric, took);
         debug!("{id:?} - Ending at {took}");
 
         Ok(())
     }
@@ -138,15 +138,15 @@
             debug!("{id:?} - Commit: starts at {v} ms");
         }
         self.writer.commit()?;
         if let Ok(v) = time.elapsed().map(|s| s.as_millis()) {
             debug!("{id:?} - Commit: ends at {v} ms");
         }
 
-        let metrics = context::get_metrics();
+        let metrics = metrics::get_metrics();
         let took = time.elapsed().map(|i| i.as_secs_f64()).unwrap_or(f64::NAN);
         let metric = request_time::RequestTimeKey::texts("delete_resource".to_string());
         metrics.record_request_time(metric, took);
         debug!("{id:?} - Ending at {took}");
 
         Ok(())
     }
@@ -208,21 +208,29 @@
             index,
             writer,
             schema: field_schema,
         })
     }
 
     fn index_document(&mut self, resource: &Resource) {
-        let metadata = resource.metadata.as_ref().unwrap();
-
-        let modified = metadata.modified.as_ref().unwrap();
-        let created = metadata.created.as_ref().unwrap();
+        let metadata = resource
+            .metadata
+            .as_ref()
+            .expect("Missing resource metadata");
+        let modified = metadata
+            .modified
+            .as_ref()
+            .expect("Missing resource modified date in metadata");
+        let created = metadata
+            .created
+            .as_ref()
+            .expect("Missing resource created date in metadata");
 
         let mut doc = doc!(
-            self.schema.uuid => resource.resource.as_ref().unwrap().uuid.as_str(),
+            self.schema.uuid => resource.resource.as_ref().expect("Missing resource details").uuid.as_str(),
             self.schema.modified => timestamp_to_datetime_utc(modified),
             self.schema.created => timestamp_to_datetime_utc(created),
             self.schema.status => resource.status as u64,
         );
 
         #[allow(clippy::iter_cloned_collect)]
         let resource_labels: Vec<String> = resource.labels.iter().cloned().collect();
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/Cargo.toml` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,22 +24,21 @@
 tracing = "0.1"
 uuid = { version = "1.1", features = ["v4"] }
 log = "0.4.14"
 env_logger = "0.9.0"
 chitchat = "0.5.0"
 dockertest = "0.3.0"
 bytes = "1.1.0"
-crc32fast = "1.3.2"
-rand = "0.8.5"
 strum = { version = "0.24.1", features = ["derive"] }
 clap = { version = "4.0.29", features = ["derive", "env"] }
 parse_duration = "2.1.1"
 derive_builder = "0.12.0"
 derive_more = { version = "0.99.17", default-features = false, features = ["display", "deref", "deref_mut"] }
 futures = "0.3.25"
+reqwest = { version = "0.11.17", default-features = true,  features = ["json"] }
 
 [dev-dependencies]
 serde_test = "1.0.150"
 serial_test = "0.10.0"
 
 [[test]]
 name = "integration"
```

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/LICENSE-AGPL` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/LICENSE-AGPL`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/src/key.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/src/key.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/src/node.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/src/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/src/register.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/src/register.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/tests/cluster_reader.py` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/tests/cluster_reader.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_cluster/tests/integration.rs` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_cluster/tests/integration.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-0.7.6/local_dependencies/nucliadb_ftp/src/error.rs` & `nucliadb_node_binding-0.7.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-// Copyright (C) 2021 Bosutech XXI S.L.
-//
-// nucliadb is offered under the AGPL v3.0 and as commercial software.
-// For commercial licensing, contact us at info@nuclia.com.
-//
-// AGPL:
-// This program is free software: you can redistribute it and/or modify
-// it under the terms of the GNU Affero General Public License as
-// published by the Free Software Foundation, either version 3 of the
-// License, or (at your option) any later version.
-//
-// This program is distributed in the hope that it will be useful,
-// but WITHOUT ANY WARRANTY; without even the implied warranty of
-// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-// GNU Affero General Public License for more details.
-//
-// You should have received a copy of the GNU Affero General Public License
-// along with this program. If not, see <http://www.gnu.org/licenses/>.
-//
+# Copyright (C) 2021 Bosutech XXI S.L.
+#
+# nucliadb is offered under the AGPL v3.0 and as commercial software.
+# For commercial licensing, contact us at info@nuclia.com.
+#
+# AGPL:
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-use std::io;
+[build-system]
+requires = ["maturin>=0.12,<0.13"]
+build-backend = "maturin"
 
-use thiserror::Error;
-
-/// The error that may occur when publishing/receiving files/directories.
-#[derive(Debug, Error)]
-pub enum Error {
-    #[error("invalid path '{0}': {1}")]
-    InvalidPath(String, String),
-    #[error(transparent)]
-    IoError(#[from] io::Error),
-}
+[project]
+name = "nucliadb_node_binding"
+requires-python = ">=3.6"
+classifiers = [
+    "Programming Language :: Rust",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+]
```

### Comparing `nucliadb_node_binding-0.7.6/Cargo.toml` & `nucliadb_node_binding-0.7.7/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "0.7.6"
+version = "0.7.7"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-0.7.6/CHANGELOG.md` & `nucliadb_node_binding-0.7.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 # Changelog
+
+## 0.7.7
+
+- Be able to filter paragraph and vectors search results by keys
+
 ## 0.7.6
 
 - Properly compute total search results for document and paragaph
 
 ## 0.7.5
 
 - Fully remove stop-words from paragraphs
```

### Comparing `nucliadb_node_binding-0.7.6/pyproject.toml` & `nucliadb_node_binding-0.7.7/local_dependencies/nucliadb_node/src/shards/unbounded_cache_provider/unbounded_writer.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,18 @@
-# Copyright (C) 2021 Bosutech XXI S.L.
-#
-# nucliadb is offered under the AGPL v3.0 and as commercial software.
-# For commercial licensing, contact us at info@nuclia.com.
-#
-# AGPL:
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
-
-[build-system]
-requires = ["maturin>=0.12,<0.13"]
-build-backend = "maturin"
-
-[project]
-name = "nucliadb_node_binding"
-requires-python = ">=3.6"
-classifiers = [
-    "Programming Language :: Rust",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
-]
+// Copyright (C) 2021 Bosutech XXI S.L.
+//
+// nucliadb is offered under the AGPL v3.0 and as commercial software.
+// For commercial licensing, contact us at info@nuclia.com.
+//
+// AGPL:
+// This program is free software: you can redistribute it and/or modify
+// it under the terms of the GNU Affero General Public License as
+// published by the Free Software Foundation, either version 3 of the
+// License, or (at your option) any later version.
+//
+// This program is distributed in the hope that it will be useful,
+// but WITHOUT ANY WARRANTY; without even the implied warranty of
+// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+// GNU Affero General Public License for more details.
+//
+// You should have received a copy of the GNU Affero General Public License
+// along with this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `nucliadb_node_binding-0.7.6/src/lib.rs` & `nucliadb_node_binding-0.7.7/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -131,21 +131,14 @@
         match self.reader.get_info(shard_id, request).transpose() {
             Some(Ok(shard)) => Ok(PyList::new(py, shard.encode_to_vec())),
             Some(Err(e)) => Err(exceptions::PyTypeError::new_err(e.to_string())),
             None => Err(exceptions::PyTypeError::new_err("Error loading shard")),
         }
     }
 
-    pub fn get_shards<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
-        match self.reader.get_shards() {
-            Ok(r) => Ok(PyList::new(py, r.encode_to_vec())),
-            Err(e) => Err(exceptions::PyTypeError::new_err(e.to_string())),
-        }
-    }
-
     pub fn search<'p>(&mut self, request: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
         let search_request = SearchRequest::decode(&mut Cursor::new(request)).unwrap();
         let shard_id = ShardId {
             id: search_request.shard.clone(),
         };
         self.reader.load_shard(&shard_id);
         let response = self.reader.search(&shard_id, search_request);
@@ -284,27 +277,18 @@
     #[staticmethod]
     pub fn new() -> NodeWriter {
         NodeWriter {
             writer: RustWriterService::new(),
         }
     }
 
-    pub fn get_shard<'p>(&mut self, shard_id: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
-        let shard_id = ShardId::decode(&mut Cursor::new(shard_id)).unwrap();
-        self.writer.load_shard(&shard_id);
-        match self.writer.get_shard(&shard_id) {
-            Some(_) => Ok(PyList::new(py, shard_id.encode_to_vec())),
-            None => Err(exceptions::PyTypeError::new_err("Not found")),
-        }
-    }
-
-    pub fn new_shard<'p>(&mut self, metadata: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
+    pub fn new_shard<'p>(&self, metadata: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
         send_telemetry_event(TelemetryEvent::Create);
         let request = NewShardRequest::decode(&mut Cursor::new(metadata)).unwrap();
-        match self.writer.new_shard(&request) {
+        match RustWriterService::new_shard(&request) {
             Ok(shard) => Ok(PyList::new(py, shard.encode_to_vec())),
             Err(e) => Err(exceptions::PyTypeError::new_err(e.to_string())),
         }
     }
 
     pub fn delete_shard<'p>(&mut self, shard_id: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
         send_telemetry_event(TelemetryEvent::Delete);
```

### Comparing `nucliadb_node_binding-0.7.6/test.py` & `nucliadb_node_binding-0.7.7/test.py`

 * *Files identical despite different names*

