# Comparing `tmp/neptune-1.3.1.tar.gz` & `tmp/neptune-1.3.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune-1.3.1.tar", max compression
+gzip compressed data, was "neptune-1.3.2rc0.tar", max compression
```

## Comparing `neptune-1.3.1.tar` & `neptune-1.3.2rc0.tar`

### file list

```diff
@@ -1,324 +1,327 @@
--rw-r--r--   0        0        0    25802 2023-06-15 17:45:30.384708 neptune-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-06-15 17:45:30.384708 neptune-1.3.1/LICENSE
--rw-r--r--   0        0        0    13935 2023-06-15 17:45:30.384708 neptune-1.3.1/README.md
--rw-r--r--   0        0        0     5399 2023-06-15 17:45:42.472976 neptune-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     3532 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/__init__.py
--rw-r--r--   0        0        0     1218 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3048 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2121 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     1788 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     1704 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     2395 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2658 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2159 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2723 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     2642 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4266 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     1949 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4292 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2656 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6003 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3498 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2627 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2157 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1017 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0      866 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/cli/abstract_backend_runner.py
--rw-r--r--   0        0        0     3436 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5574 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/cli/commands.py
--rw-r--r--   0        0        0     2814 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/cli/container_manager.py
--rw-r--r--   0        0        0     1947 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3899 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/cli/status.py
--rw-r--r--   0        0        0     9995 2023-06-15 17:45:30.384708 neptune-1.3.1/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5028 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/cli/utils.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/__init__.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/backends/__init__.py
--rw-r--r--   0        0        0     1038 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/backends/api_model.py
--rw-r--r--   0        0        0     4230 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/backends/utils.py
--rw-r--r--   0        0        0      859 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/envs.py
--rw-r--r--   0        0        0    14106 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/exceptions.py
--rw-r--r--   0        0        0      629 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/experiments.py
--rw-r--r--   0        0        0     2490 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/git_info.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/__init__.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3212 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/constants.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1554 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2023 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1766 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1748 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2568 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3490 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1679 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      947 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2309 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2504 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/hardware/system/system_monitor.py
--rw-r--r--   0        0        0     4772 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/oauth.py
--rw-r--r--   0        0        0      884 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/patches/__init__.py
--rw-r--r--   0        0        0     2731 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/patches/bravado.py
--rw-r--r--   0        0        0      726 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/patterns.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/storage/__init__.py
--rw-r--r--   0        0        0     3223 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/storage/datastream.py
--rw-r--r--   0        0        0     7335 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/storage/storage_utils.py
--rw-r--r--   0        0        0     7075 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/utils.py
--rw-r--r--   0        0        0     2206 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/warnings.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/websockets/__init__.py
--rw-r--r--   0        0        0     3589 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2693 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/common/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0      985 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/constants.py
--rw-r--r--   0        0        0     1863 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/envs.py
--rw-r--r--   0        0        0    41966 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/exceptions.py
--rw-r--r--   0        0        0    29698 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      973 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0     1014 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      985 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      976 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      993 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      985 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0      989 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3084 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0     1006 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/pytorch/__init__.py
--rw-r--r--   0        0        0     1042 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      985 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      989 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0     1038 2023-06-15 17:45:30.388708 neptune-1.3.1/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0     1032 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0     1164 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      989 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4810 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     4017 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2318 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     7169 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     6700 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     5942 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    17136 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    40705 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     8506 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    31714 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     1942 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     4471 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3946 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5003 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13841 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1619 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5246 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0     8765 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1381 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1035 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      350 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2345 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0     8468 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/disk_queue.py
--rw-r--r--   0        0        0      689 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2466 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     4997 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      933 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0      796 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1572 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1831 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0    17310 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    10851 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     2177 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     2136 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     1140 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1998 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/operation_processors/operation_storage.py
--rw-r--r--   0        0        0     1577 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     2483 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     3724 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      776 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/state.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     2418 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     3567 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4584 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     1665 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0     4856 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     1171 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/utils/dependency_tracking.py
--rw-r--r--   0        0        0     2114 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2374 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     5888 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0      849 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0     9732 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1288 2023-06-15 17:45:30.392708 neptune-1.3.1/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     3053 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/json_file_splitter.py
--rw-r--r--   0        0        0     1633 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     1488 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1042 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0     2049 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1564 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1207 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1340 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2270 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     1457 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/sync_offset_file.py
--rw-r--r--   0        0        0     1927 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2426 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     4462 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     5188 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1229 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0    13821 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/__init__.py
--rw-r--r--   0        0        0    11218 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/api_exceptions.py
--rw-r--r--   0        0        0     4710 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/backend.py
--rw-r--r--   0        0        0      737 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/checkpoint.py
--rw-r--r--   0        0        0      859 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/constants.py
--rw-r--r--   0        0        0      860 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/envs.py
--rw-r--r--   0        0        0    12780 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/exceptions.py
--rw-r--r--   0        0        0    42888 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/experiments.py
--rw-r--r--   0        0        0      663 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/git_info.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/__init__.py
--rw-r--r--   0        0        0     1999 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/abort.py
--rw-r--r--   0        0        0      888 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/api_clients/__init__.py
--rw-r--r--   0        0        0     1148 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/api_clients/backend_factory.py
--rw-r--r--   0        0        0     1826 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/api_clients/client_config.py
--rw-r--r--   0        0        0     3103 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/api_clients/credentials.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
--rw-r--r--   0        0        0    46556 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
--rw-r--r--   0        0        0     8710 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
--rw-r--r--   0        0        0     4456 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
--rw-r--r--   0        0        0     3857 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
--rw-r--r--   0        0        0     4631 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/api_clients/offline_backend.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/backends/__init__.py
--rw-r--r--   0        0        0      776 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/channels/__init__.py
--rw-r--r--   0        0        0     3903 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/channels/channels.py
--rw-r--r--   0        0        0     7087 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/channels/channels_values_sender.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/execution/__init__.py
--rw-r--r--   0        0        0     6126 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/execution/execution_context.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/experiments/__init__.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1510 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1711 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/streams/__init__.py
--rw-r--r--   0        0        0     2805 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/streams/channel_writer.py
--rw-r--r--   0        0        0     1945 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/streams/stdstream_uploader.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/threads/__init__.py
--rw-r--r--   0        0        0     2363 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/threads/aborting_thread.py
--rw-r--r--   0        0        0     1816 2023-06-15 17:45:30.396708 neptune-1.3.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
--rw-r--r--   0        0        0     1334 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/threads/neptune_thread.py
--rw-r--r--   0        0        0     1556 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/threads/ping_thread.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/utils/__init__.py
--rw-r--r--   0        0        0     8091 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/utils/alpha_integration.py
--rw-r--r--   0        0        0      997 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2597 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/utils/http.py
--rw-r--r--   0        0        0     2597 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/utils/http_utils.py
--rw-r--r--   0        0        0     2990 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/utils/image.py
--rw-r--r--   0        0        0     3145 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/utils/source_code.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/websockets/message.py
--rw-r--r--   0        0        0     1097 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
--rw-r--r--   0        0        0     1228 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py
--rw-r--r--   0        0        0     3938 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/model.py
--rw-r--r--   0        0        0     2807 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/notebook.py
--rw-r--r--   0        0        0      691 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/oauth.py
--rw-r--r--   0        0        0      678 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/patterns.py
--rw-r--r--   0        0        0    26377 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/projects.py
--rw-r--r--   0        0        0     8992 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/sessions.py
--rw-r--r--   0        0        0     1162 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/legacy/utils.py
--rw-r--r--   0        0        0      660 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/logging/__init__.py
--rw-r--r--   0        0        0      976 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/logging/logger.py
--rw-r--r--   0        0        0     4454 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     6943 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    36941 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     2013 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      995 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/metadata_containers/__init__.py
--rw-r--r--   0        0        0     2063 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/metadata_containers/abstract.py
--rw-r--r--   0        0        0    20007 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/metadata_containers/metadata_container.py
--rw-r--r--   0        0        0     9194 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/metadata_containers/metadata_containers_table.py
--rw-r--r--   0        0        0    12337 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/metadata_containers/model.py
--rw-r--r--   0        0        0    11428 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/metadata_containers/model_version.py
--rw-r--r--   0        0        0    15433 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/metadata_containers/project.py
--rw-r--r--   0        0        0    23734 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/metadata_containers/run.py
--rw-r--r--   0        0        0     2606 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/_compatibility.py
--rw-r--r--   0        0        0      974 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/constants.py
--rw-r--r--   0        0        0     1378 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/envs.py
--rw-r--r--   0        0        0     5846 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/exceptions.py
--rw-r--r--   0        0        0      655 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/handler.py
--rw-r--r--   0        0        0      694 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/project.py
--rw-r--r--   0        0        0     1672 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/run.py
--rw-r--r--   0        0        0     1426 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/runs_table.py
--rw-r--r--   0        0        0      681 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/utils.py
--rw-r--r--   0        0        0      696 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/new/version.py
--rw-r--r--   0        0        0     1071 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    11695 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1144 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     2447 2023-06-15 17:45:30.400708 neptune-1.3.1/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     2553 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1221 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     2601 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0      698 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/typing.py
--rw-r--r--   0        0        0     1755 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     2228 2023-06-15 17:45:30.404708 neptune-1.3.1/src/neptune/version.py
--rw-r--r--   0        0        0    18357 1970-01-01 00:00:00.000000 neptune-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    26074 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/LICENSE
+-rw-r--r--   0        0        0    13935 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/README.md
+-rw-r--r--   0        0        0     5404 2023-06-21 15:38:26.668585 neptune-1.3.2rc0/pyproject.toml
+-rw-r--r--   0        0        0     3532 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/api/__init__.py
+-rw-r--r--   0        0        0     1229 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/api/exceptions_utils.py
+-rw-r--r--   0        0        0      992 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/api/requests_utils.py
+-rw-r--r--   0        0        0     1218 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3048 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2121 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     1788 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     1704 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2395 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2658 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2159 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2723 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     2642 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4266 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     1949 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4292 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2656 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6003 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3498 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2627 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2157 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1017 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0      866 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/cli/abstract_backend_runner.py
+-rw-r--r--   0        0        0     3436 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5574 2023-06-21 15:38:13.268452 neptune-1.3.2rc0/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0     2814 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/cli/container_manager.py
+-rw-r--r--   0        0        0     1947 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3899 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     9995 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5028 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/backends/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/backends/api_model.py
+-rw-r--r--   0        0        0     5615 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/backends/utils.py
+-rw-r--r--   0        0        0      859 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/envs.py
+-rw-r--r--   0        0        0    14676 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/exceptions.py
+-rw-r--r--   0        0        0      629 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/experiments.py
+-rw-r--r--   0        0        0     2490 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/git_info.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3212 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/constants.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1554 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2023 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1766 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1748 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2568 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3490 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1679 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      947 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2309 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2504 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0     4772 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/oauth.py
+-rw-r--r--   0        0        0      884 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/patches/bravado.py
+-rw-r--r--   0        0        0      726 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/patterns.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/storage/__init__.py
+-rw-r--r--   0        0        0     3223 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/storage/datastream.py
+-rw-r--r--   0        0        0     7335 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/storage/storage_utils.py
+-rw-r--r--   0        0        0     7514 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/utils.py
+-rw-r--r--   0        0        0     2206 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/warnings.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/websockets/__init__.py
+-rw-r--r--   0        0        0     3589 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2693 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/common/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0      985 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/constants.py
+-rw-r--r--   0        0        0     1863 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/envs.py
+-rw-r--r--   0        0        0    41966 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    29698 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      973 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0     1014 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      976 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      993 2023-06-21 15:38:13.272452 neptune-1.3.2rc0/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0      989 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3084 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0     1006 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0     1042 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      989 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0     1032 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0     1164 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      989 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4810 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     4017 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2318 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     7169 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     6700 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     6232 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    17136 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    40705 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0     8506 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    31714 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     1942 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     4471 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3946 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5003 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13841 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1619 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5184 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0     8765 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1537 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1154 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      350 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2345 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0     8543 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/disk_queue.py
+-rw-r--r--   0        0        0      689 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2466 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     5101 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      933 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0      796 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1572 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1831 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0    17310 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    10682 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     2177 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     2136 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     1253 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1998 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/operation_processors/operation_storage.py
+-rw-r--r--   0        0        0     1577 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     2483 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     3724 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      776 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/state.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2023 2023-06-21 15:38:13.276452 neptune-1.3.2rc0/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     3041 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     5476 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4584 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     1665 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0     4856 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1171 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/dependency_tracking.py
+-rw-r--r--   0        0        0     2114 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2374 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     5888 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0      849 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0     9732 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1288 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     3053 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/json_file_splitter.py
+-rw-r--r--   0        0        0     1633 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     1488 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1042 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0     2188 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1564 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1207 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1340 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2270 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     1457 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/sync_offset_file.py
+-rw-r--r--   0        0        0     1998 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2426 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     4462 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     5334 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1229 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0    13821 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/__init__.py
+-rw-r--r--   0        0        0    11218 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/api_exceptions.py
+-rw-r--r--   0        0        0     4710 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/backend.py
+-rw-r--r--   0        0        0      737 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/checkpoint.py
+-rw-r--r--   0        0        0      859 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/constants.py
+-rw-r--r--   0        0        0      860 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/envs.py
+-rw-r--r--   0        0        0    12780 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/exceptions.py
+-rw-r--r--   0        0        0    42888 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/experiments.py
+-rw-r--r--   0        0        0      663 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/git_info.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/__init__.py
+-rw-r--r--   0        0        0     1999 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/abort.py
+-rw-r--r--   0        0        0      888 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/__init__.py
+-rw-r--r--   0        0        0     1148 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/backend_factory.py
+-rw-r--r--   0        0        0     1826 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/client_config.py
+-rw-r--r--   0        0        0     3103 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/credentials.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
+-rw-r--r--   0        0        0    46556 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
+-rw-r--r--   0        0        0     8710 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
+-rw-r--r--   0        0        0     4456 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
+-rw-r--r--   0        0        0     3857 2023-06-21 15:38:13.280452 neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
+-rw-r--r--   0        0        0     4631 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/offline_backend.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/backends/__init__.py
+-rw-r--r--   0        0        0      776 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/channels/__init__.py
+-rw-r--r--   0        0        0     3903 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/channels/channels.py
+-rw-r--r--   0        0        0     7087 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/channels/channels_values_sender.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/execution/__init__.py
+-rw-r--r--   0        0        0     6126 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/execution/execution_context.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/experiments/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1711 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2805 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/streams/channel_writer.py
+-rw-r--r--   0        0        0     1945 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/streams/stdstream_uploader.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/threads/__init__.py
+-rw-r--r--   0        0        0     2363 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/threads/aborting_thread.py
+-rw-r--r--   0        0        0     1816 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
+-rw-r--r--   0        0        0     1334 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/threads/neptune_thread.py
+-rw-r--r--   0        0        0     1556 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/threads/ping_thread.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/utils/__init__.py
+-rw-r--r--   0        0        0     8091 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/utils/alpha_integration.py
+-rw-r--r--   0        0        0      997 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2597 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/utils/http.py
+-rw-r--r--   0        0        0     2597 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/utils/http_utils.py
+-rw-r--r--   0        0        0     2990 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/utils/image.py
+-rw-r--r--   0        0        0     3145 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/utils/source_code.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/websockets/message.py
+-rw-r--r--   0        0        0     1097 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
+-rw-r--r--   0        0        0     1228 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/internal/websockets/websocket_message_processor.py
+-rw-r--r--   0        0        0     3938 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/model.py
+-rw-r--r--   0        0        0     2807 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/notebook.py
+-rw-r--r--   0        0        0      691 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/oauth.py
+-rw-r--r--   0        0        0      678 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/patterns.py
+-rw-r--r--   0        0        0    26377 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/projects.py
+-rw-r--r--   0        0        0     8992 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/sessions.py
+-rw-r--r--   0        0        0     1162 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/legacy/utils.py
+-rw-r--r--   0        0        0      660 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/logging/__init__.py
+-rw-r--r--   0        0        0      976 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/logging/logger.py
+-rw-r--r--   0        0        0     4454 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     6943 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    36941 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2013 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      995 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/metadata_containers/__init__.py
+-rw-r--r--   0        0        0     2063 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/metadata_containers/abstract.py
+-rw-r--r--   0        0        0    21692 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/metadata_containers/metadata_container.py
+-rw-r--r--   0        0        0     9194 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/metadata_containers/metadata_containers_table.py
+-rw-r--r--   0        0        0    12337 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/metadata_containers/model.py
+-rw-r--r--   0        0        0    11428 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/metadata_containers/model_version.py
+-rw-r--r--   0        0        0    15433 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/metadata_containers/project.py
+-rw-r--r--   0        0        0    23734 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/metadata_containers/run.py
+-rw-r--r--   0        0        0     2606 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/new/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/new/_compatibility.py
+-rw-r--r--   0        0        0      974 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/new/constants.py
+-rw-r--r--   0        0        0     1378 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/new/envs.py
+-rw-r--r--   0        0        0     5846 2023-06-21 15:38:13.284452 neptune-1.3.2rc0/src/neptune/new/exceptions.py
+-rw-r--r--   0        0        0      655 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/new/handler.py
+-rw-r--r--   0        0        0      694 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/new/project.py
+-rw-r--r--   0        0        0     1672 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/new/run.py
+-rw-r--r--   0        0        0     1426 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/new/runs_table.py
+-rw-r--r--   0        0        0      681 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/new/utils.py
+-rw-r--r--   0        0        0      696 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/new/version.py
+-rw-r--r--   0        0        0     1071 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    11695 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1144 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2447 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     2553 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0      698 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/typing.py
+-rw-r--r--   0        0        0     1755 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     2228 2023-06-21 15:38:13.288452 neptune-1.3.2rc0/src/neptune/version.py
+-rw-r--r--   0        0        0    18360 1970-01-01 00:00:00.000000 neptune-1.3.2rc0/PKG-INFO
```

### Comparing `neptune-1.3.1/CHANGELOG.md` & `neptune-1.3.2rc0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+## [UNRELEASED] neptune 1.3.2
+
+### Changes
+- Added support of writing to archived project exception ([#1355](https://github.com/neptune-ai/neptune-client/pull/1355))
+
 ## neptune 1.3.1
 
 ### Fixes
 - Fix ImportError when git is missing ([#1359](https://github.com/neptune-ai/neptune-client/pull/1359))
 
 ## neptune 1.3.0
 
 ### Features
 - Added automatic tracking of dependencies ([#1345](https://github.com/neptune-ai/neptune-client/pull/1345))
 - Added automatic tracking of uncommitted changes ([#1350]https://github.com/neptune-ai/neptune-client/pull/1350)
 
 ### Fixes
 - Added support of project visibility exception ([#1343](https://github.com/neptune-ai/neptune-client/pull/1343))
+- Fix SSL errors after forking process ([#1353](https://github.com/neptune-ai/neptune-client/pull/1353))
 
 ### Changes
 - Added support of active projects limit exception ([#1348](https://github.com/neptune-ai/neptune-client/pull/1348))
 
 ## neptune 1.2.0
 
 ### Changes
```

### Comparing `neptune-1.3.1/LICENSE` & `neptune-1.3.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/README.md` & `neptune-1.3.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/pyproject.toml` & `neptune-1.3.2rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 repository = "https://github.com/neptune-ai/neptune-client"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune"
 readme = "README.md"
-version = "1.3.1"
+version = "1.3.2-rc.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune-1.3.1/src/neptune/__init__.py` & `neptune-1.3.2rc0/src/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/__init__.py` & `neptune-1.3.2rc0/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/__init__.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/artifact.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/atom.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/boolean.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/copiable_atom.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/datetime.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/file.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/float.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/git_ref.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/integer.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/notebook_ref.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/run_state.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/atoms/string.py` & `neptune-1.3.2rc0/src/neptune/attributes/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/attribute.py` & `neptune-1.3.2rc0/src/neptune/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/constants.py` & `neptune-1.3.2rc0/src/neptune/attributes/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/file_set.py` & `neptune-1.3.2rc0/src/neptune/attributes/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/namespace.py` & `neptune-1.3.2rc0/src/neptune/attributes/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/series/__init__.py` & `neptune-1.3.2rc0/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/series/fetchable_series.py` & `neptune-1.3.2rc0/src/neptune/attributes/series/fetchable_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/series/file_series.py` & `neptune-1.3.2rc0/src/neptune/attributes/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/series/float_series.py` & `neptune-1.3.2rc0/src/neptune/attributes/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/series/series.py` & `neptune-1.3.2rc0/src/neptune/attributes/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/series/string_series.py` & `neptune-1.3.2rc0/src/neptune/attributes/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/sets/__init__.py` & `neptune-1.3.2rc0/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/sets/set.py` & `neptune-1.3.2rc0/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/sets/string_set.py` & `neptune-1.3.2rc0/src/neptune/attributes/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/attributes/utils.py` & `neptune-1.3.2rc0/src/neptune/attributes/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/cli/__init__.py` & `neptune-1.3.2rc0/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/cli/__main__.py` & `neptune-1.3.2rc0/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/cli/abstract_backend_runner.py` & `neptune-1.3.2rc0/src/neptune/cli/abstract_backend_runner.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/cli/clear.py` & `neptune-1.3.2rc0/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/cli/commands.py` & `neptune-1.3.2rc0/src/neptune/cli/commands.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/cli/container_manager.py` & `neptune-1.3.2rc0/src/neptune/cli/container_manager.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/cli/path_option.py` & `neptune-1.3.2rc0/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/cli/status.py` & `neptune-1.3.2rc0/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/cli/sync.py` & `neptune-1.3.2rc0/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/cli/utils.py` & `neptune-1.3.2rc0/src/neptune/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/backends/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/backends/api_model.py` & `neptune-1.3.2rc0/src/neptune/common/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/backends/utils.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,121 +1,111 @@
 #
-# Copyright (c) 2022, Neptune Labs Sp. z o.o.
+# Copyright (c) 2023, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["with_api_exceptions_handler"]
 
-import itertools
 import logging
-import os
 import time
 
 import requests
 from bravado.exception import (
     BravadoConnectionError,
     BravadoTimeoutError,
     HTTPBadGateway,
-    HTTPClientError,
     HTTPForbidden,
     HTTPGatewayTimeout,
     HTTPInternalServerError,
     HTTPRequestTimeout,
     HTTPServiceUnavailable,
     HTTPTooManyRequests,
     HTTPUnauthorized,
 )
 from urllib3.exceptions import NewConnectionError
 
-from neptune.common.envs import NEPTUNE_RETRIES_TIMEOUT_ENV
-from neptune.common.exceptions import (
-    ClientHttpError,
+from neptune.legacy.api_exceptions import (
+    ConnectionLost,
     Forbidden,
-    NeptuneAuthTokenExpired,
-    NeptuneConnectionLostException,
-    NeptuneInvalidApiTokenException,
     NeptuneSSLVerificationError,
+    ServerError,
     Unauthorized,
 )
 
 _logger = logging.getLogger(__name__)
 
-MAX_RETRY_TIME = 30
-retries_timeout = int(os.getenv(NEPTUNE_RETRIES_TIMEOUT_ENV, "60"))
 
-
-def with_api_exceptions_handler(func):
+def legacy_with_api_exceptions_handler(func):
     def wrapper(*args, **kwargs):
-        last_exception = None
-        start_time = time.monotonic()
-        for retry in itertools.count(0):
-            if time.monotonic() - start_time > retries_timeout:
-                break
-
+        retries = 11
+        retry = 0
+        while retry < retries:
             try:
                 return func(*args, **kwargs)
-            except requests.exceptions.InvalidHeader as e:
-                if "X-Neptune-Api-Token" in e.args[0]:
-                    raise NeptuneInvalidApiTokenException()
-                raise
-            except requests.exceptions.SSLError as e:
-                raise NeptuneSSLVerificationError() from e
+            except requests.exceptions.SSLError:
+                raise NeptuneSSLVerificationError()
+            except HTTPServiceUnavailable:
+                if retry >= 6:
+                    _logger.warning("Experiencing connection interruptions. Reestablishing communication with Neptune.")
+                time.sleep(2**retry)
+                retry += 1
+                continue
             except (
                 BravadoConnectionError,
                 BravadoTimeoutError,
                 requests.exceptions.ConnectionError,
                 requests.exceptions.Timeout,
                 HTTPRequestTimeout,
-                HTTPServiceUnavailable,
                 HTTPGatewayTimeout,
                 HTTPBadGateway,
                 HTTPTooManyRequests,
                 HTTPInternalServerError,
                 NewConnectionError,
-            ) as e:
-                time.sleep(min(2 ** min(10, retry), MAX_RETRY_TIME))
-                last_exception = e
-                continue
-            except NeptuneAuthTokenExpired:
+            ):
+                if retry >= 6:
+                    _logger.warning("Experiencing connection interruptions. Reestablishing communication with Neptune.")
+                time.sleep(2**retry)
+                retry += 1
                 continue
             except HTTPUnauthorized:
                 raise Unauthorized()
             except HTTPForbidden:
                 raise Forbidden()
-            except HTTPClientError as e:
-                raise ClientHttpError(e.status_code, e.response.text) from e
             except requests.exceptions.RequestException as e:
                 if e.response is None:
                     raise
                 status_code = e.response.status_code
                 if status_code in (
                     HTTPRequestTimeout.status_code,
                     HTTPBadGateway.status_code,
                     HTTPServiceUnavailable.status_code,
                     HTTPGatewayTimeout.status_code,
                     HTTPTooManyRequests.status_code,
                     HTTPInternalServerError.status_code,
                 ):
-                    time.sleep(min(2 ** min(10, retry), MAX_RETRY_TIME))
-                    last_exception = e
+                    if retry >= 6:
+                        _logger.warning(
+                            "Experiencing connection interruptions. Reestablishing communication with Neptune."
+                        )
+                    time.sleep(2**retry)
+                    retry += 1
                     continue
+                elif status_code >= HTTPInternalServerError.status_code:
+                    raise ServerError()
                 elif status_code == HTTPUnauthorized.status_code:
                     raise Unauthorized()
                 elif status_code == HTTPForbidden.status_code:
                     raise Forbidden()
-                elif 400 <= status_code < 500:
-                    raise ClientHttpError(status_code, e.response.text) from e
                 else:
                     raise
-        raise NeptuneConnectionLostException(last_exception) from last_exception
+        raise ConnectionLost()
 
     return wrapper
```

### Comparing `neptune-1.3.1/src/neptune/common/envs.py` & `neptune-1.3.2rc0/src/neptune/common/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/exceptions.py` & `neptune-1.3.2rc0/src/neptune/common/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,7 +404,22 @@
     def __init__(self, path):
         super(NotAFile, self).__init__("Path {} is not a file.".format(path))
 
 
 class NotADirectory(NeptuneException):
     def __init__(self, path):
         super(NotADirectory, self).__init__("Path {} is not a directory.".format(path))
+
+
+class WritingToArchivedProjectException(NeptuneException):
+    def __init__(self):
+        message = """
+{h1}
+----WritingToArchivedProjectException-----------------------------------------------------------------------
+{end}
+You're trying to write to a project that was archived.
+
+Set the project as active again or use mode="read-only" at initialization to fetch metadata from it.
+
+{correct}Need help?{end}-> https://docs.neptune.ai/help/error_writing_to_archived_project/
+"""
+        super(WritingToArchivedProjectException, self).__init__(message.format(**STYLES))
```

### Comparing `neptune-1.3.1/src/neptune/common/experiments.py` & `neptune-1.3.2rc0/src/neptune/common/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/git_info.py` & `neptune-1.3.2rc0/src/neptune/common/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/cgroup/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/cgroup/cgroup_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/constants.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/gauges/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/gauges/cpu.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/gauges/cpu.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/gauges/gauge.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/gauges/gauge_factory.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/gauges/gauge_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/gauges/gauge_mode.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/gauges/gpu.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/gauges/gpu.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/gauges/memory.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/gauges/memory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/gpu/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/gpu/gpu_monitor.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/metric.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/metrics_container.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/metrics_factory.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/metrics_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/reports/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/reports/metric_report.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/reports/metric_reporter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/service/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/service/metric_service.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/metrics/service/metric_service_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/resources/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/resources/system_resource_info.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/resources/system_resource_info_factory.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/resources/system_resource_info_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/system/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/hardware/system/system_monitor.py` & `neptune-1.3.2rc0/src/neptune/common/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/oauth.py` & `neptune-1.3.2rc0/src/neptune/common/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/patches/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/patches/bravado.py` & `neptune-1.3.2rc0/src/neptune/common/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/patterns.py` & `neptune-1.3.2rc0/src/neptune/common/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/storage/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/storage/datastream.py` & `neptune-1.3.2rc0/src/neptune/common/storage/datastream.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/storage/storage_utils.py` & `neptune-1.3.2rc0/src/neptune/common/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/utils.py` & `neptune-1.3.2rc0/src/neptune/common/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import functools
 import glob as globlib
 import logging
 import math
 import os
 import re
+import ssl
 import sys
 
 import numpy as np
 import pandas as pd
 
 from neptune.common import envs
 from neptune.common.exceptions import (
@@ -39,14 +40,24 @@
 
 _logger = logging.getLogger(__name__)
 
 IS_WINDOWS = sys.platform == "win32"
 IS_MACOS = sys.platform == "darwin"
 
 
+def reset_internal_ssl_state():
+    """
+    OpenSSL's internal random number generator does not properly handle forked processes.
+    Applications must change the PRNG state of the parent process if they use any SSL feature with os.fork().
+    Any successful call of RAND_add(), RAND_bytes() or RAND_pseudo_bytes() is sufficient.
+    https://docs.python.org/3/library/ssl.html#multi-processing
+    """
+    ssl.RAND_bytes(100)
+
+
 def map_values(f_value, dictionary):
     return dict((k, f_value(v)) for k, v in dictionary.items())
 
 
 def map_keys(f_key, dictionary):
     return dict((f_key(k), v) for k, v in dictionary.items())
```

### Comparing `neptune-1.3.1/src/neptune/common/warnings.py` & `neptune-1.3.2rc0/src/neptune/common/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/websockets/__init__.py` & `neptune-1.3.2rc0/src/neptune/common/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/websockets/reconnecting_websocket.py` & `neptune-1.3.2rc0/src/neptune/common/websockets/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/common/websockets/websocket_client_adapter.py` & `neptune-1.3.2rc0/src/neptune/common/websockets/websocket_client_adapter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/constants.py` & `neptune-1.3.2rc0/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/envs.py` & `neptune-1.3.2rc0/src/neptune/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/exceptions.py` & `neptune-1.3.2rc0/src/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/handler.py` & `neptune-1.3.2rc0/src/neptune/handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/aws/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/detectron2/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/detectron2/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/fastai/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/kedro/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/lightgbm/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/optuna/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/optuna/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/prophet/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/python_logger.py` & `neptune-1.3.2rc0/src/neptune/integrations/python_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/pytorch/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/sacred/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/sklearn/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/transformers/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/utils.py` & `neptune-1.3.2rc0/src/neptune/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/integrations/xgboost/__init__.py` & `neptune-1.3.2rc0/src/neptune/integrations/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/artifacts/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/artifacts/drivers/local.py` & `neptune-1.3.2rc0/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/artifacts/drivers/s3.py` & `neptune-1.3.2rc0/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/artifacts/file_hasher.py` & `neptune-1.3.2rc0/src/neptune/internal/artifacts/file_hasher.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune-1.3.2rc0/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/artifacts/types.py` & `neptune-1.3.2rc0/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/artifacts/utils.py` & `neptune-1.3.2rc0/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/api_model.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/factory.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/hosted_client.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/hosted_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import os
 import platform
 from typing import (
     Dict,
     Tuple,
 )
 
+import requests
 from bravado.http_client import HttpClient
 from bravado.requests_client import RequestsClient
 
 from neptune.common.backends.utils import with_api_exceptions_handler
 from neptune.common.oauth import NeptuneAuthenticator
 from neptune.envs import NEPTUNE_REQUEST_TIMEOUT
 from neptune.exceptions import NeptuneClientUpgradeRequiredError
@@ -61,18 +62,27 @@
         "connect_timeout": CONNECT_TIMEOUT,
         "timeout": REQUEST_TIMEOUT,
         "headers": {"X-Neptune-LegacyClient": "false"},
     }
 }
 
 
+def _close_connections_on_fork(session: requests.Session):
+    try:
+        os.register_at_fork(before=session.close, after_in_child=session.close, after_in_parent=session.close)
+    except AttributeError:
+        pass
+
+
 def create_http_client(ssl_verify: bool, proxies: Dict[str, str]) -> RequestsClient:
     http_client = RequestsClient(ssl_verify=ssl_verify, response_adapter_class=NeptuneResponseAdapter)
     http_client.session.verify = ssl_verify
 
+    _close_connections_on_fork(http_client.session)
+
     update_session_proxies(http_client.session, proxies)
 
     user_agent = "neptune-client/{lib_version} ({system}, python {python_version})".format(
         lib_version=neptune_client_version,
         system=platform.platform(),
         python_version=platform.python_version(),
     )
```

### Comparing `neptune-1.3.1/src/neptune/internal/backends/hosted_file_operations.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/neptune_backend.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/nql.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/nql.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/offline_neptune_backend.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/offline_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/operations_preprocessor.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/project_name_lookup.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backends/swagger_client_wrapper.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/swagger_client_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 from collections.abc import Callable
 from typing import Optional
 
 from bravado.client import SwaggerClient
 from bravado.exception import HTTPError
 
+from neptune.api.exceptions_utils import handle_json_errors
+from neptune.api.requests_utils import ensure_json_response
 from neptune.common.exceptions import NeptuneAuthTokenExpired
 from neptune.exceptions import (
     NeptuneFieldCountLimitExceedException,
     NeptuneLimitExceedException,
 )
 
 
@@ -42,19 +44,14 @@
             ProjectKeyInvalid,
             ProjectNameCollision,
             ProjectNameInvalid,
             ProjectPrivacyRestrictedException,
             ProjectsLimitReached,
         )
 
-        try:
-            body = response.json() or dict()
-        except Exception:
-            body = {}
-
         error_processors: dict[str, Callable[[dict], Exception]] = {
             "ATTRIBUTES_PER_EXPERIMENT_LIMIT_EXCEEDED": lambda response_body: NeptuneFieldCountLimitExceedException(
                 limit=response_body.get("limit", "<unknown limit>"),
                 container_type=response_body.get("experimentType", "object"),
                 identifier=response_body.get("experimentQualifiedName", "<unknown identifier>"),
             ),
             "AUTHORIZATION_TOKEN_EXPIRED": lambda _: NeptuneAuthTokenExpired(),
@@ -84,20 +81,19 @@
                 reason=response_body.get("title", "Unknown reason")
             ),
             "LIMIT_OF_ACTIVE_PROJECTS_REACHED": lambda response_body: ActiveProjectsLimitReachedException(
                 currentQuota=response_body.get("currentQuota", "<unknown quota>")
             ),
         }
 
-        error_type: Optional[str] = body.get("errorType")
-        error_processor = error_processors.get(error_type)
-        if error_processor:
-            raise error_processor(body) from exception
-        elif exception:
-            raise exception
+        handle_json_errors(
+            content=ensure_json_response(response),
+            error_processors=error_processors,
+            source_exception=exception,
+        )
 
     def __call__(self, *args, **kwargs):
         try:
             future = self._api_method(*args, **kwargs)
             return FinishedApiResponseFuture(future.response())  # wait synchronously
         except HTTPError as e:
             self.handle_neptune_http_errors(e.response, exception=e)
```

### Comparing `neptune-1.3.1/src/neptune/internal/backends/utils.py` & `neptune-1.3.2rc0/src/neptune/internal/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/backgroud_job_list.py` & `neptune-1.3.2rc0/src/neptune/internal/backgroud_job_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,7 +41,15 @@
             job.stop()
 
     def join(self, seconds: Optional[float] = None):
         ts = time.time()
         for job in self._jobs:
             sec_left = None if seconds is None else seconds - (time.time() - ts)
             job.join(sec_left)
+
+    def pause(self):
+        for job in self._jobs:
+            job.pause()
+
+    def resume(self):
+        for job in self._jobs:
+            job.resume()
```

### Comparing `neptune-1.3.1/src/neptune/internal/background_job.py` & `neptune-1.3.2rc0/src/neptune/internal/background_job.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,7 +33,15 @@
     @abc.abstractmethod
     def stop(self):
         pass
 
     @abc.abstractmethod
     def join(self, seconds: Optional[float] = None):
         pass
+
+    @abc.abstractmethod
+    def pause(self):
+        pass
+
+    @abc.abstractmethod
+    def resume(self):
+        pass
```

### Comparing `neptune-1.3.1/src/neptune/internal/container_structure.py` & `neptune-1.3.2rc0/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/container_type.py` & `neptune-1.3.2rc0/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/credentials.py` & `neptune-1.3.2rc0/src/neptune/internal/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/disk_queue.py` & `neptune-1.3.2rc0/src/neptune/internal/disk_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,19 @@
 
     def _remove_data(self):
         path = self._dir_path
         shutil.rmtree(path, ignore_errors=True)
 
         parent = path.parent
 
-        files = os.listdir(parent)
+        try:
+            files = os.listdir(parent)
+        except FileNotFoundError:
+            files = []
+
         if len(files) == 0:
             try:
                 os.rmdir(parent)
             except OSError:
                 _logger.info(f"Cannot remove directory: {parent}")
 
     def wait_for_empty(self, seconds: Optional[float] = None) -> bool:
```

### Comparing `neptune-1.3.1/src/neptune/internal/exceptions.py` & `neptune-1.3.2rc0/src/neptune/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/hardware/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/hardware/gpu/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/hardware/gpu/gpu_monitor.py` & `neptune-1.3.2rc0/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune-1.3.2rc0/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,20 @@
         self._started = True
 
     def stop(self):
         if not self._started:
             return
         self._thread.interrupt()
 
+    def pause(self):
+        self._thread.pause()
+
+    def resume(self):
+        self._thread.resume()
+
     def join(self, seconds: Optional[float] = None):
         if not self._started:
             return
         self._thread.join(seconds)
 
     def get_attribute_name(self, resource_type, gauge_name) -> str:
         gauges_count = self._gauges_in_resource.get(resource_type, None)
```

### Comparing `neptune-1.3.1/src/neptune/internal/id_formats.py` & `neptune-1.3.2rc0/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/init/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/init/parameters.py` & `neptune-1.3.2rc0/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/notebooks/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/notebooks/comm.py` & `neptune-1.3.2rc0/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/notebooks/notebooks.py` & `neptune-1.3.2rc0/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/operation.py` & `neptune-1.3.2rc0/src/neptune/internal/operation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/operation_processors/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune-1.3.2rc0/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ("AsyncOperationProcessor",)
 
 import logging
 import os
-import sys
 import threading
 from datetime import datetime
 from time import (
     monotonic,
     time,
 )
 from typing import (
@@ -73,39 +72,27 @@
         self._container_id = container_id
         self._container_type = container_type
         self._backend = backend
         self._batch_size = batch_size
         self._last_version = 0
         self._consumed_version = 0
         self._consumer = self.ConsumerThread(self, sleep_time, batch_size)
-        self._drop_operations = False
 
         # Caller is responsible for taking this lock
         self._waiting_cond = threading.Condition(lock=lock)
 
-        if sys.version_info >= (3, 7):
-            try:
-                os.register_at_fork(after_in_child=self._handle_fork_in_child)
-            except AttributeError:
-                pass
-
     @staticmethod
     def _init_data_path(container_id: UniqueId, container_type: ContainerType):
         now = datetime.now()
         container_dir = f"{NEPTUNE_DATA_DIRECTORY}/{ASYNC_DIRECTORY}/{container_type.create_dir_name(container_id)}"
-        data_path = f"{container_dir}/exec-{now.timestamp()}-{now.strftime('%Y-%m-%d_%H.%M.%S.%f')}"
+        data_path = f"{container_dir}/exec-{now.timestamp()}-{now.strftime('%Y-%m-%d_%H.%M.%S.%f')}-{os.getpid()}"
         data_path = data_path.replace(" ", "_").replace(":", ".")
         return data_path
 
-    def _handle_fork_in_child(self):
-        self._drop_operations = True
-
     def enqueue_operation(self, op: Operation, *, wait: bool) -> None:
-        if self._drop_operations:
-            return
         self._last_version = self._queue.put(op)
         if self._queue.size() > self._batch_size / 2:
             self._consumer.wake_up()
         if wait:
             self.wait()
 
     def wait(self):
@@ -123,14 +110,21 @@
 
     def flush(self):
         self._queue.flush()
 
     def start(self):
         self._consumer.start()
 
+    def pause(self):
+        self._consumer.pause()
+        self._queue.flush()
+
+    def resume(self):
+        self._consumer.resume()
+
     def _wait_for_queue_empty(self, initial_queue_size: int, seconds: Optional[float]):
         waiting_start = monotonic()
         time_elapsed = 0
         max_reconnect_wait_time = self.STOP_QUEUE_MAX_TIME_NO_CONNECTION_SECONDS if seconds is None else seconds
         if initial_queue_size > 0:
             if self._consumer.last_backoff_time > 0:
                 logger.warning(
@@ -209,14 +203,17 @@
             self._consumer.wake_up()
             self._wait_for_queue_empty(initial_queue_size=self._queue.size(), seconds=seconds)
             self._consumer.interrupt()
         sec_left = None if seconds is None else seconds - (time() - ts)
         self._consumer.join(sec_left)
         self._queue.close()
 
+    def close(self):
+        self._queue.close()
+
     class ConsumerThread(Daemon):
         def __init__(
             self,
             processor: "AsyncOperationProcessor",
             sleep_time: float,
             batch_size: int,
         ):
```

### Comparing `neptune-1.3.1/src/neptune/internal/operation_processors/factory.py` & `neptune-1.3.2rc0/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune-1.3.2rc0/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/operation_processors/operation_processor.py` & `neptune-1.3.2rc0/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,10 +34,19 @@
     def flush(self):
         pass
 
     @abc.abstractmethod
     def start(self):
         pass
 
+    def pause(self):
+        pass
+
+    def resume(self):
+        pass
+
     @abc.abstractmethod
     def stop(self, seconds: Optional[float] = None):
         pass
+
+    def close(self):
+        self.stop()
```

### Comparing `neptune-1.3.1/src/neptune/internal/operation_processors/operation_storage.py` & `neptune-1.3.2rc0/src/neptune/internal/operation_processors/operation_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune-1.3.2rc0/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune-1.3.2rc0/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/operation_visitor.py` & `neptune-1.3.2rc0/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/state.py` & `neptune-1.3.2rc0/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/streams/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/streams/std_capture_background_job.py` & `neptune-1.3.2rc0/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 
     def start(self, container: "MetadataContainer"):
         self._logger = StdoutCaptureLogger(container, self._attribute_name)
 
     def stop(self):
         self._logger.close()
 
+    def pause(self):
+        self._logger.pause()
+
+    def resume(self):
+        self._logger.resume()
+
     def join(self, seconds: Optional[float] = None):
         pass
 
 
 class StderrCaptureBackgroundJob(BackgroundJob):
     def __init__(self, attribute_name: str):
         self._attribute_name = attribute_name
@@ -52,9 +58,15 @@
 
     def start(self, container: "MetadataContainer"):
         self._logger = StderrCaptureLogger(container, self._attribute_name)
 
     def stop(self):
         self._logger.close()
 
+    def pause(self):
+        self._logger.pause()
+
+    def resume(self):
+        self._logger.resume()
+
     def join(self, seconds: Optional[float] = None):
         pass
```

### Comparing `neptune-1.3.1/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune-1.3.2rc0/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,46 +16,62 @@
 __all__ = ["StdoutCaptureLogger", "StderrCaptureLogger"]
 
 import sys
 import threading
 from queue import Queue
 from typing import TextIO
 
+from neptune.internal.threading.daemon import Daemon
 from neptune.logging import Logger as NeptuneLogger
 from neptune.metadata_containers import MetadataContainer
 
 
 class StdStreamCaptureLogger:
     def __init__(self, container: MetadataContainer, attribute_name: str, stream: TextIO):
         self._logger = NeptuneLogger(container, attribute_name)
         self.stream = stream
         self._thread_local = threading.local()
         self.enabled = True
         self._log_data_queue = Queue()
-        self._logging_thread = threading.Thread(target=self.__proces_logs, daemon=True)
+        self._logging_thread = self.ReportingThread(self, "NeptuneThread_" + attribute_name)
         self._logging_thread.start()
 
+    def pause(self):
+        self._log_data_queue.put_nowait(None)
+        self._logging_thread.pause()
+
+    def resume(self):
+        self._logging_thread.resume()
+
     def write(self, data: str):
         self.stream.write(data)
         self._log_data_queue.put_nowait(data)
 
     def __getattr__(self, attr):
         return getattr(self.stream, attr)
 
     def close(self):
+        if self.enabled:
+            self._logging_thread.interrupt()
         self.enabled = False
         self._log_data_queue.put_nowait(None)
         self._logging_thread.join()
 
-    def __proces_logs(self):
-        while True:
-            data = self._log_data_queue.get()
-            if data is None:
-                break
-            self._logger.log(data)
+    class ReportingThread(Daemon):
+        def __init__(self, logger: "StdStreamCaptureLogger", name: str):
+            super().__init__(sleep_time=0, name=name)
+            self._logger = logger
+
+        @Daemon.ConnectionRetryWrapper(kill_message="Killing Neptune STD capturing thread.")
+        def work(self) -> None:
+            while True:
+                data = self._logger._log_data_queue.get()
+                if data is None:
+                    break
+                self._logger._logger.log(data)
 
 
 class StdoutCaptureLogger(StdStreamCaptureLogger):
     def __init__(self, container: MetadataContainer, attribute_name: str):
         super().__init__(container, attribute_name, sys.stdout)
         sys.stdout = self
```

### Comparing `neptune-1.3.1/src/neptune/internal/threading/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/types/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/types/file_types.py` & `neptune-1.3.2rc0/src/neptune/internal/types/file_types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/types/stringify_value.py` & `neptune-1.3.2rc0/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/dependency_tracking.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/dependency_tracking.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/deprecation.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/git.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/git.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/hashing.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/images.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/images.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/iteration.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/json_file_splitter.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/limits.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/logger.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/paths.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/ping_background_job.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/ping_background_job.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,27 +29,33 @@
 
 _logger = logging.getLogger(__name__)
 
 
 class PingBackgroundJob(BackgroundJob):
     def __init__(self, period: float = 10):
         self._period = period
-        self._thread = None
+        self._thread: PingBackgroundJob.ReportingThread = None
         self._started = False
 
     def start(self, container: "MetadataContainer"):
         self._thread = self.ReportingThread(self._period, container)
         self._thread.start()
         self._started = True
 
     def stop(self):
         if not self._started:
             return
         self._thread.interrupt()
 
+    def pause(self):
+        self._thread.pause()
+
+    def resume(self):
+        self._thread.resume()
+
     def join(self, seconds: Optional[float] = None):
         if not self._started:
             return
         self._thread.join(seconds)
 
     class ReportingThread(Daemon):
         def __init__(self, period: float, container: "MetadataContainer"):
```

### Comparing `neptune-1.3.1/src/neptune/internal/utils/process_killer.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/run_state.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/runningmode.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/s3.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/source_code.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/sync_offset_file.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/utils/traceback_job.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/traceback_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,7 +54,13 @@
         self._started = True
 
     def stop(self):
         traceback_handler.unregister(self._uuid)
 
     def join(self, seconds: Optional[float] = None):
         pass
+
+    def pause(self):
+        pass
+
+    def resume(self):
+        pass
```

### Comparing `neptune-1.3.1/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune-1.3.2rc0/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/value_to_attribute_visitor.py` & `neptune-1.3.2rc0/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/websockets/__init__.py` & `neptune-1.3.2rc0/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune-1.3.2rc0/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,21 @@
 
     def stop(self):
         if not self._started:
             return
         self._thread.interrupt()
         self._thread.shutdown_ws_client()
 
+    def pause(self):
+        self._thread.shutdown_ws_client()
+        self._thread.pause()
+
+    def resume(self):
+        self._thread.resume()
+
     def join(self, seconds: Optional[float] = None):
         if not self._started or threading.get_ident() == self._thread.ident:
             return
         self._thread.join(seconds)
         # Just in case. There is possible race condition when connection can be reestablished after being shutdown.
         self._thread.shutdown_ws_client()
```

### Comparing `neptune-1.3.1/src/neptune/internal/websockets/websockets_factory.py` & `neptune-1.3.2rc0/src/neptune/internal/websockets/websockets_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/api_exceptions.py` & `neptune-1.3.2rc0/src/neptune/legacy/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/backend.py` & `neptune-1.3.2rc0/src/neptune/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/checkpoint.py` & `neptune-1.3.2rc0/src/neptune/legacy/checkpoint.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/constants.py` & `neptune-1.3.2rc0/src/neptune/legacy/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/envs.py` & `neptune-1.3.2rc0/src/neptune/legacy/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/exceptions.py` & `neptune-1.3.2rc0/src/neptune/legacy/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/experiments.py` & `neptune-1.3.2rc0/src/neptune/legacy/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/git_info.py` & `neptune-1.3.2rc0/src/neptune/legacy/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/abort.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/abort.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/api_clients/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/api_clients/backend_factory.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/backend_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/api_clients/client_config.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/client_config.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/api_clients/credentials.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/api_clients/offline_backend.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/api_clients/offline_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/backends/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/channels/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/channels/channels.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/channels/channels.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/channels/channels_values_sender.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/channels/channels_values_sender.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/execution/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/execution/execution_context.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/experiments/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/notebooks/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/notebooks/comm.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/notebooks/notebooks.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/streams/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/streams/channel_writer.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/streams/channel_writer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/streams/stdstream_uploader.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/streams/stdstream_uploader.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/threads/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/threads/aborting_thread.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/threads/aborting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/threads/neptune_thread.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/threads/neptune_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/threads/ping_thread.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/threads/ping_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/utils/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/utils/alpha_integration.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/utils/alpha_integration.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/utils/deprecation.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/utils/http.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/utils/http.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/utils/http_utils.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/utils/image.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/utils/image.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/utils/source_code.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/websockets/__init__.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/websockets/message.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/websockets/message.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py` & `neptune-1.3.2rc0/src/neptune/legacy/internal/websockets/websocket_message_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/model.py` & `neptune-1.3.2rc0/src/neptune/legacy/model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/notebook.py` & `neptune-1.3.2rc0/src/neptune/legacy/notebook.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/oauth.py` & `neptune-1.3.2rc0/src/neptune/legacy/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/patterns.py` & `neptune-1.3.2rc0/src/neptune/legacy/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/projects.py` & `neptune-1.3.2rc0/src/neptune/legacy/projects.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/sessions.py` & `neptune-1.3.2rc0/src/neptune/legacy/sessions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/legacy/utils.py` & `neptune-1.3.2rc0/src/neptune/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/logging/__init__.py` & `neptune-1.3.2rc0/src/neptune/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/logging/logger.py` & `neptune-1.3.2rc0/src/neptune/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/management/__init__.py` & `neptune-1.3.2rc0/src/neptune/management/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/management/exceptions.py` & `neptune-1.3.2rc0/src/neptune/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/management/internal/__init__.py` & `neptune-1.3.2rc0/src/neptune/management/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/management/internal/api.py` & `neptune-1.3.2rc0/src/neptune/management/internal/api.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/management/internal/dto.py` & `neptune-1.3.2rc0/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/management/internal/types.py` & `neptune-1.3.2rc0/src/neptune/management/internal/types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/management/internal/utils.py` & `neptune-1.3.2rc0/src/neptune/management/internal/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/metadata_containers/__init__.py` & `neptune-1.3.2rc0/src/neptune/metadata_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/metadata_containers/abstract.py` & `neptune-1.3.2rc0/src/neptune/metadata_containers/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/metadata_containers/metadata_container.py` & `neptune-1.3.2rc0/src/neptune/metadata_containers/metadata_container.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 #
 __all__ = ["MetadataContainer"]
 
 import abc
 import atexit
 import itertools
+import os
 import threading
 import time
 import traceback
 from contextlib import AbstractContextManager
 from functools import wraps
 from typing import (
     Any,
@@ -33,14 +34,15 @@
 )
 
 from neptune.attributes import create_attribute_from_type
 from neptune.attributes.attribute import Attribute
 from neptune.attributes.namespace import Namespace as NamespaceAttr
 from neptune.attributes.namespace import NamespaceBuilder
 from neptune.common.exceptions import UNIX_STYLES
+from neptune.common.utils import reset_internal_ssl_state
 from neptune.common.warnings import warn_about_unsupported_type
 from neptune.exceptions import (
     MetadataInconsistency,
     NeptunePossibleLegacyUsageException,
 )
 from neptune.handler import Handler
 from neptune.internal.backends.api_model import (
@@ -103,14 +105,15 @@
         verify_type("project", project, (str, type(None)))
         verify_type("api_token", api_token, (str, type(None)))
         verify_type("mode", mode, Mode)
         verify_type("flush_period", flush_period, (int, float))
         verify_type("proxies", proxies, (dict, type(None)))
 
         self._mode: Mode = mode
+        self._flush_period = flush_period
         self._lock: threading.RLock = threading.RLock()
         self._state: ContainerState = ContainerState.CREATED
 
         self._backend: NeptuneBackend = get_backend(mode=mode, api_token=api_token, proxies=proxies)
 
         self._project_qualified_name: Optional[str] = conform_optional(project, QualifiedName)
         self._project_api_object: Project = project_name_lookup(
@@ -139,14 +142,59 @@
             self.sync(wait=False)
 
         if self._mode != Mode.READ_ONLY:
             self._write_initial_attributes()
 
         self._startup(debug_mode=mode == Mode.DEBUG)
 
+        try:
+            os.register_at_fork(
+                before=self._before_fork,
+                after_in_child=self._handle_fork_in_child,
+                after_in_parent=self._handle_fork_in_parent,
+            )
+        except AttributeError:
+            pass
+
+    """
+    OpenSSL's internal random number generator does not properly handle forked processes.
+    Applications must change the PRNG state of the parent process if they use any SSL feature with os.fork().
+    Any successful call of RAND_add(), RAND_bytes() or RAND_pseudo_bytes() is sufficient.
+    https://docs.python.org/3/library/ssl.html#multi-processing
+
+    On Linux it looks like it does not help much but does not break anything either.
+    """
+
+    def _handle_fork_in_parent(self):
+        reset_internal_ssl_state()
+        self._op_processor.resume()
+        self._bg_job.resume()
+
+    def _handle_fork_in_child(self):
+        reset_internal_ssl_state()
+        self._op_processor.close()
+        self._op_processor = get_operation_processor(
+            mode=self._mode,
+            container_id=self._id,
+            container_type=self.container_type,
+            backend=self._backend,
+            lock=self._lock,
+            flush_period=self._flush_period,
+        )
+
+        # TODO: Every implementation of background job should handle fork by itself.
+        self._bg_job = BackgroundJobList([])
+
+        if self._state == ContainerState.STARTED:
+            self._op_processor.start()
+
+    def _before_fork(self):
+        self._bg_job.pause()
+        self._op_processor.pause()
+
     def _prepare_background_jobs_if_non_read_only(self) -> BackgroundJobList:
         if self._mode != Mode.READ_ONLY:
             return self._prepare_background_jobs()
         return BackgroundJobList([])
 
     @abc.abstractmethod
     def _get_or_create_api_object(self) -> ApiExperiment:
```

### Comparing `neptune-1.3.1/src/neptune/metadata_containers/metadata_containers_table.py` & `neptune-1.3.2rc0/src/neptune/metadata_containers/metadata_containers_table.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/metadata_containers/model.py` & `neptune-1.3.2rc0/src/neptune/metadata_containers/model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/metadata_containers/model_version.py` & `neptune-1.3.2rc0/src/neptune/metadata_containers/model_version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/metadata_containers/project.py` & `neptune-1.3.2rc0/src/neptune/metadata_containers/project.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/metadata_containers/run.py` & `neptune-1.3.2rc0/src/neptune/metadata_containers/run.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/__init__.py` & `neptune-1.3.2rc0/src/neptune/new/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/_compatibility.py` & `neptune-1.3.2rc0/src/neptune/new/_compatibility.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/constants.py` & `neptune-1.3.2rc0/src/neptune/new/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/envs.py` & `neptune-1.3.2rc0/src/neptune/new/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/exceptions.py` & `neptune-1.3.2rc0/src/neptune/new/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/handler.py` & `neptune-1.3.2rc0/src/neptune/new/handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/project.py` & `neptune-1.3.2rc0/src/neptune/new/project.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/run.py` & `neptune-1.3.2rc0/src/neptune/new/run.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/runs_table.py` & `neptune-1.3.2rc0/src/neptune/new/runs_table.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/utils.py` & `neptune-1.3.2rc0/src/neptune/new/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/new/version.py` & `neptune-1.3.2rc0/src/neptune/new/version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/__init__.py` & `neptune-1.3.2rc0/src/neptune/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/atoms/__init__.py` & `neptune-1.3.2rc0/src/neptune/types/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/atoms/artifact.py` & `neptune-1.3.2rc0/src/neptune/types/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/atoms/atom.py` & `neptune-1.3.2rc0/src/neptune/types/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/atoms/boolean.py` & `neptune-1.3.2rc0/src/neptune/types/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/atoms/datetime.py` & `neptune-1.3.2rc0/src/neptune/types/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/atoms/file.py` & `neptune-1.3.2rc0/src/neptune/types/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/atoms/float.py` & `neptune-1.3.2rc0/src/neptune/types/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/atoms/git_ref.py` & `neptune-1.3.2rc0/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/atoms/integer.py` & `neptune-1.3.2rc0/src/neptune/types/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/atoms/string.py` & `neptune-1.3.2rc0/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/file_set.py` & `neptune-1.3.2rc0/src/neptune/types/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/mode.py` & `neptune-1.3.2rc0/src/neptune/types/mode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/model_version_stage.py` & `neptune-1.3.2rc0/src/neptune/types/model_version_stage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/namespace.py` & `neptune-1.3.2rc0/src/neptune/types/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/series/__init__.py` & `neptune-1.3.2rc0/src/neptune/types/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/series/file_series.py` & `neptune-1.3.2rc0/src/neptune/types/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/series/float_series.py` & `neptune-1.3.2rc0/src/neptune/types/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/series/series.py` & `neptune-1.3.2rc0/src/neptune/types/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/series/series_value.py` & `neptune-1.3.2rc0/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/series/string_series.py` & `neptune-1.3.2rc0/src/neptune/types/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/sets/__init__.py` & `neptune-1.3.2rc0/src/neptune/types/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/sets/set.py` & `neptune-1.3.2rc0/src/neptune/types/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/sets/string_set.py` & `neptune-1.3.2rc0/src/neptune/types/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/type_casting.py` & `neptune-1.3.2rc0/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/value.py` & `neptune-1.3.2rc0/src/neptune/types/value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/value_copy.py` & `neptune-1.3.2rc0/src/neptune/types/value_copy.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/types/value_visitor.py` & `neptune-1.3.2rc0/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/typing.py` & `neptune-1.3.2rc0/src/neptune/typing.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/utils.py` & `neptune-1.3.2rc0/src/neptune/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/vendor/lib_programname.py` & `neptune-1.3.2rc0/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/vendor/pynvml.py` & `neptune-1.3.2rc0/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/src/neptune/version.py` & `neptune-1.3.2rc0/src/neptune/version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.3.1/PKG-INFO` & `neptune-1.3.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune
-Version: 1.3.1
+Version: 1.3.2rc0
 Summary: Neptune Client
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
```

