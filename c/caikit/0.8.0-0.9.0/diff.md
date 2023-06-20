# Comparing `tmp/caikit-0.8.0.tar.gz` & `tmp/caikit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.8.0.tar` & `caikit-0.9.0.tar`

### file list

```diff
@@ -1,304 +1,312 @@
--rw-r--r--   0        0        0       60 2023-06-14 15:11:43.801701 caikit-0.8.0/.coveragerc
--rw-r--r--   0        0        0      676 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1559 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1328 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1117 2023-06-14 15:11:43.801701 caikit-0.8.0/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      260 2023-06-14 15:11:43.801701 caikit-0.8.0/.gitignore
--rw-r--r--   0        0        0      324 2023-06-14 15:11:43.801701 caikit-0.8.0/.isort.cfg
--rw-r--r--   0        0        0      370 2023-06-14 15:11:43.801701 caikit-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-06-14 15:11:43.801701 caikit-0.8.0/.prettierignore
--rw-r--r--   0        0        0       12 2023-06-14 15:11:43.801701 caikit-0.8.0/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-06-14 15:11:43.801701 caikit-0.8.0/.pylintrc
--rw-r--r--   0        0        0      530 2023-06-14 15:11:43.801701 caikit-0.8.0/.readthedocs.yaml
--rw-r--r--   0        0        0       78 2023-06-14 15:11:43.801701 caikit-0.8.0/.whitesource
--rw-r--r--   0        0        0      368 2023-06-14 15:11:43.801701 caikit-0.8.0/CODEOWNERS
--rw-r--r--   0        0        0     7164 2023-06-14 15:11:43.801701 caikit-0.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-06-14 15:11:43.801701 caikit-0.8.0/LICENSE
--rw-r--r--   0        0        0     4448 2023-06-14 15:11:43.801701 caikit-0.8.0/README.md
--rw-r--r--   0        0        0      152 2023-06-14 15:11:43.801701 caikit-0.8.0/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit-overview.png
--rw-r--r--   0        0        0      427 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/config/__init__.py
--rw-r--r--   0        0        0     6052 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/config/config.py
--rw-r--r--   0        0        0     6388 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/config/config.yml
--rw-r--r--   0        0        0     1642 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0     1027 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    37893 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-06-14 15:11:43.801701 caikit-0.8.0/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2446 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     4997 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    15192 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4996 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     5127 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/json_dict.py
--rw-r--r--   0        0        0     1564 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40244 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21296 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/model_manager.py
--rw-r--r--   0        0        0      684 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2834 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4718 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2802 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     6002 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/module_backends/module_backend_config.py
--rw-r--r--   0        0        0      742 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/__init__.py
--rw-r--r--   0        0        0    30320 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/base.py
--rw-r--r--   0        0        0     6157 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/config.py
--rw-r--r--   0        0        0    11042 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/decorator.py
--rw-r--r--   0        0        0     4151 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/loader.py
--rw-r--r--   0        0        0     6013 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/meta.py
--rw-r--r--   0        0        0    13024 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/modules/saver.py
--rw-r--r--   0        0        0     3895 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/registries.py
--rw-r--r--   0        0        0      654 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10721 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4688 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8221 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/signature_parsing/parsers.py
--rw-r--r--   0        0        0    10558 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/task.py
--rw-r--r--   0        0        0      982 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21366 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     1648 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32206 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0      530 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1662 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14335 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    15629 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2606 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12089 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1480 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-06-14 15:11:43.805701 caikit-0.8.0/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0     9572 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     4229 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    13127 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     5613 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/protoable.py
--rw-r--r--   0        0        0    12397 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0     2216 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    11024 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    12451 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5440 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6810 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    12934 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0    11924 2023-06-14 15:11:43.809701 caikit-0.8.0/caikit/runtime/work_management/train_executors.py
--rw-r--r--   0        0        0      169 2023-06-14 15:11:43.809701 caikit-0.8.0/code-of-conduct.md
--rw-r--r--   0        0        0       90 2023-06-14 15:11:43.809701 caikit-0.8.0/docs-requirements.txt
--rw-r--r--   0        0        0      639 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/Makefile
--rw-r--r--   0        0        0     6860 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/001-module.md
--rw-r--r--   0        0        0     1610 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/architecture_club/README.md
--rw-r--r--   0        0        0      805 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/make.bat
--rw-r--r--   0        0        0     3053 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/source/conf.py
--rw-r--r--   0        0        0      225 2023-06-14 15:11:43.809701 caikit-0.8.0/docs/source/index.rst
--rw-r--r--   0        0        0      837 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1422 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      673 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       72 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      615 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      645 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3283 2023-06-14 15:11:43.809701 caikit-0.8.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
--rw-r--r--   0        0        0     1234 2023-06-14 15:11:47.085731 caikit-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2952 2023-06-14 15:11:43.809701 caikit-0.8.0/releases.md
--rwxr-xr-x   0        0        0      639 2023-06-14 15:11:43.809701 caikit-0.8.0/scripts/check_deps.sh
--rwxr-xr-x   0        0        0      720 2023-06-14 15:11:43.809701 caikit-0.8.0/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-06-14 15:11:43.809701 caikit-0.8.0/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     5240 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/base.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/config/__init__.py
--rw-r--r--   0        0        0     5358 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/config/test_configs.py
--rw-r--r--   0        0        0    10738 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:43.809701 caikit-0.8.0/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     5034 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26951 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    16237 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    25955 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     5083 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/test_enums.py
--rw-r--r--   0        0        0     2358 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/test_json_dict.py
--rw-r--r--   0        0        0     1104 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4378 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/helpers.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2320 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     6888 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/module_backends/test_module_backend_config.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/modules/__init__.py
--rw-r--r--   0        0        0    13033 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/modules/test_module.py
--rw-r--r--   0        0        0     6274 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/modules/test_module_metadata.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0     4872 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8595 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0      521 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/test_imports.py
--rw-r--r--   0        0        0    21743 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/test_model_manager.py
--rw-r--r--   0        0        0     1038 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     7497 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/test_task.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/__init__.py
--rw-r--r--   0        0        0     7967 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4997 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0     6782 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      591 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0      222 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0     1017 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module.zip
--rw-r--r--   0        0        0      675 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module/config.yml
--rw-r--r--   0        0        0      299 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module/data.json
--rw-r--r--   0        0        0       14 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module/data.pkl
--rw-r--r--   0        0        0      191 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_backend/config.yml
--rw-r--r--   0        0        0      179 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_foo/config.yml
--rw-r--r--   0        0        0      508 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_no_id/config.yml
--rw-r--r--   0        0        0      508 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_no_nesting.zip
--rw-r--r--   0        0        0      570 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_singleton/data.json
--rw-r--r--   0        0        0       14 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_module_singleton/data.pkl
--rw-r--r--   0        0        0      230 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0      326 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/dummy_streaming_module/config.yml
--rw-r--r--   0        0        0     3034 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      349 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      360 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      364 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      396 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0       24 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      294 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      296 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      176 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1474 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0      156 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/__init__.py
--rw-r--r--   0        0        0       89 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/other_task/__init__.py
--rw-r--r--   0        0        0     1946 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
--rw-r--r--   0        0        0      296 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/__init__.py
--rw-r--r--   0        0        0     1720 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
--rw-r--r--   0        0        0      902 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
--rw-r--r--   0        0        0     2463 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1410 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2720 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
--rw-r--r--   0        0        0     1514 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py
--rw-r--r--   0        0        0      364 2023-06-14 15:11:43.813701 caikit-0.8.0/tests/fixtures/sample_module/config.yml
--rw-r--r--   0        0        0        0 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3845 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14101 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10266 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17911 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     4035 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    17954 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     3105 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/test_protoable.py
--rw-r--r--   0        0        0     2345 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/test_rpcs.py
--rw-r--r--   0        0        0     1376 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     8381 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    16259 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     4088 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7776 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    36461 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0     5072 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    17337 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3819 2023-06-14 15:11:43.817701 caikit-0.8.0/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     2617 2023-06-14 15:11:43.817701 caikit-0.8.0/tox.ini
--rw-r--r--   0        0        0     5653 1970-01-01 00:00:00.000000 caikit-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-06-20 23:03:32.698051 caikit-0.9.0/.coveragerc
+-rw-r--r--   0        0        0      676 2023-06-20 23:03:32.702051 caikit-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-06-20 23:03:32.702051 caikit-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-06-20 23:03:32.702051 caikit-0.9.0/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-06-20 23:03:32.702051 caikit-0.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1689 2023-06-20 23:03:32.702051 caikit-0.9.0/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-06-20 23:03:32.702051 caikit-0.9.0/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1117 2023-06-20 23:03:32.702051 caikit-0.9.0/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      260 2023-06-20 23:03:32.702051 caikit-0.9.0/.gitignore
+-rw-r--r--   0        0        0      324 2023-06-20 23:03:32.702051 caikit-0.9.0/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-06-20 23:03:32.702051 caikit-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-06-20 23:03:32.702051 caikit-0.9.0/.prettierignore
+-rw-r--r--   0        0        0       12 2023-06-20 23:03:32.702051 caikit-0.9.0/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-06-20 23:03:32.702051 caikit-0.9.0/.pylintrc
+-rw-r--r--   0        0        0      599 2023-06-20 23:03:32.702051 caikit-0.9.0/.readthedocs.yaml
+-rw-r--r--   0        0        0       78 2023-06-20 23:03:32.702051 caikit-0.9.0/.whitesource
+-rw-r--r--   0        0        0      368 2023-06-20 23:03:32.702051 caikit-0.9.0/CODEOWNERS
+-rw-r--r--   0        0        0     7164 2023-06-20 23:03:32.702051 caikit-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-06-20 23:03:32.702051 caikit-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4448 2023-06-20 23:03:32.702051 caikit-0.9.0/README.md
+-rw-r--r--   0        0        0      152 2023-06-20 23:03:32.702051 caikit-0.9.0/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit-overview.png
+-rw-r--r--   0        0        0      427 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6052 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/config/config.py
+-rw-r--r--   0        0        0     6388 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/config/config.yml
+-rw-r--r--   0        0        0     1642 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0     1027 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    39670 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2446 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     4997 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    16828 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4996 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     5127 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/json_dict.py
+-rw-r--r--   0        0        0     1564 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40244 2023-06-20 23:03:32.702051 caikit-0.9.0/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21296 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/model_manager.py
+-rw-r--r--   0        0        0      684 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2834 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4718 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2880 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     6002 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/module_backends/module_backend_config.py
+-rw-r--r--   0        0        0      742 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/modules/__init__.py
+-rw-r--r--   0        0        0    30320 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/modules/base.py
+-rw-r--r--   0        0        0     6157 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/modules/config.py
+-rw-r--r--   0        0        0    11042 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/modules/decorator.py
+-rw-r--r--   0        0        0     4151 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/modules/loader.py
+-rw-r--r--   0        0        0     6013 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/modules/meta.py
+-rw-r--r--   0        0        0    13024 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/modules/saver.py
+-rw-r--r--   0        0        0     3895 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/registries.py
+-rw-r--r--   0        0        0      654 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10673 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4688 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8221 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/signature_parsing/parsers.py
+-rw-r--r--   0        0        0    10558 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/task.py
+-rw-r--r--   0        0        0      982 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21366 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     1648 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32206 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1056 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      618 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/nlp/__init__.py
+-rw-r--r--   0        0        0      809 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/nlp/data_model/__init__.py
+-rw-r--r--   0        0        0      740 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/nlp/data_model/package.py
+-rw-r--r--   0        0        0     2254 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/nlp/data_model/text_generation.py
+-rw-r--r--   0        0        0     1383 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/nlp/tasks.py
+-rw-r--r--   0        0        0      611 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1662 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14335 2023-06-20 23:03:32.706051 caikit-0.9.0/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    15629 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2606 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12089 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0     9572 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     4229 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    11983 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     6156 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/service_generation/protoable.py
+-rw-r--r--   0        0        0    12152 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0     2216 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    12655 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    12451 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5440 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6810 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    13825 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0    11924 2023-06-20 23:03:32.710052 caikit-0.9.0/caikit/runtime/work_management/train_executors.py
+-rw-r--r--   0        0        0      169 2023-06-20 23:03:32.710052 caikit-0.9.0/code-of-conduct.md
+-rw-r--r--   0        0        0      639 2023-06-20 23:03:32.710052 caikit-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0     6860 2023-06-20 23:03:32.710052 caikit-0.9.0/docs/adrs/001-module.md
+-rw-r--r--   0        0        0     1610 2023-06-20 23:03:32.710052 caikit-0.9.0/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-06-20 23:03:32.710052 caikit-0.9.0/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-06-20 23:03:32.710052 caikit-0.9.0/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-06-20 23:03:32.710052 caikit-0.9.0/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-06-20 23:03:32.710052 caikit-0.9.0/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-06-20 23:03:32.714052 caikit-0.9.0/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-06-20 23:03:32.714052 caikit-0.9.0/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      805 2023-06-20 23:03:32.714052 caikit-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0     3053 2023-06-20 23:03:32.714052 caikit-0.9.0/docs/source/conf.py
+-rw-r--r--   0        0        0      225 2023-06-20 23:03:32.714052 caikit-0.9.0/docs/source/index.rst
+-rw-r--r--   0        0        0      837 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1422 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      673 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      615 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      645 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3283 2023-06-20 23:03:32.714052 caikit-0.9.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
+-rw-r--r--   0        0        0     1900 2023-06-20 23:03:38.062036 caikit-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2952 2023-06-20 23:03:32.714052 caikit-0.9.0/releases.md
+-rwxr-xr-x   0        0        0      639 2023-06-20 23:03:32.714052 caikit-0.9.0/scripts/check_deps.sh
+-rwxr-xr-x   0        0        0      720 2023-06-20 23:03:32.714052 caikit-0.9.0/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-06-20 23:03:32.714052 caikit-0.9.0/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     5240 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/base.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/config/test_configs.py
+-rw-r--r--   0        0        0     4508 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     5034 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26951 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    16237 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    30195 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     2358 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/test_json_dict.py
+-rw-r--r--   0        0        0     1104 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4378 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2320 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     6888 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/module_backends/test_module_backend_config.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/modules/__init__.py
+-rw-r--r--   0        0        0    13033 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/modules/test_module.py
+-rw-r--r--   0        0        0     6274 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/modules/test_module_metadata.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     4872 2023-06-20 23:03:32.714052 caikit-0.9.0/tests/core/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8595 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0      521 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21743 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0     1038 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     7497 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/test_task.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     7967 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4997 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0     6782 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      591 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0      222 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0     1017 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module.zip
+-rw-r--r--   0        0        0      675 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module/config.yml
+-rw-r--r--   0        0        0      299 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module/data.json
+-rw-r--r--   0        0        0       14 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module/data.pkl
+-rw-r--r--   0        0        0      191 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module_backend/config.yml
+-rw-r--r--   0        0        0      179 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module_foo/config.yml
+-rw-r--r--   0        0        0      508 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module_no_id/config.yml
+-rw-r--r--   0        0        0      508 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module_no_nesting.zip
+-rw-r--r--   0        0        0      570 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_module_singleton/data.pkl
+-rw-r--r--   0        0        0      230 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0      326 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/dummy_streaming_module/config.yml
+-rw-r--r--   0        0        0     3034 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      349 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      360 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      364 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      396 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0       24 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      294 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      176 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1474 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0      156 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/modules/__init__.py
+-rw-r--r--   0        0        0       89 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/modules/other_task/__init__.py
+-rw-r--r--   0        0        0     1946 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
+-rw-r--r--   0        0        0      296 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/__init__.py
+-rw-r--r--   0        0        0     1720 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
+-rw-r--r--   0        0        0      902 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
+-rw-r--r--   0        0        0     2463 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     3401 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2720 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0     1514 2023-06-20 23:03:32.718052 caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py
+-rw-r--r--   0        0        0      364 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/fixtures/sample_module/config.yml
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/interfaces/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/interfaces/nlp/__init__.py
+-rw-r--r--   0        0        0     2859 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/interfaces/nlp/test_nlp_tasks.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/__init__.py
+-rw-r--r--   0        0        0     6754 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/conftest.py
+-rw-r--r--   0        0        0      756 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3845 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14101 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10266 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17911 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     4035 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    17954 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     3796 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/service_generation/test_protoable.py
+-rw-r--r--   0        0        0     2345 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1376 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     8875 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    16259 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     4088 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7776 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    38206 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0     5072 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    17329 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3819 2023-06-20 23:03:32.722052 caikit-0.9.0/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     2047 2023-06-20 23:03:32.722052 caikit-0.9.0/tox.ini
+-rw-r--r--   0        0        0     6672 1970-01-01 00:00:00.000000 caikit-0.9.0/PKG-INFO
```

### Comparing `caikit-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.9.0/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/.github/workflows/build-library.yml` & `caikit-0.9.0/.github/workflows/build-library.yml`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,17 @@
           - setup: '3.10'
             tox: 'py310'
           - setup: '3.11'
             tox: 'py311'
           # Special matrix entry to ensure protobuf 3 compatibility
           - setup: '3.8'
             tox: 'proto3'
+          # Special matrix entry to ensure core tests pass without optional deps
+          - setup: '3.8'
+            tox: 'core'
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version.setup }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version.setup }}
```

### Comparing `caikit-0.8.0/.github/workflows/lint-code.yml` & `caikit-0.9.0/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/.github/workflows/publish-library.yml` & `caikit-0.9.0/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/.pylintrc` & `caikit-0.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/.readthedocs.yaml` & `caikit-0.9.0/.readthedocs.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -14,8 +14,12 @@
 # Build documentation in the docs/source directory with Sphinx
 sphinx:
     configuration: docs/source/conf.py
 
 # Declare the Python requirements required to build your docs
 python:
     install:
-        - requirements: docs-requirements.txt
+        - method: pip
+          path: .
+          extra_requirements:
+              - all
+              - dev-docs
```

### Comparing `caikit-0.8.0/CONTRIBUTING.md` & `caikit-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/LICENSE` & `caikit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/README.md` & `caikit-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit-overview.png` & `caikit-0.9.0/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/config/__init__.py` & `caikit-0.9.0/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/config/config.py` & `caikit-0.9.0/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/config/config.yml` & `caikit-0.9.0/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/__init__.py` & `caikit-0.9.0/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/augmentors/__init__.py` & `caikit-0.9.0/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/augmentors/base.py` & `caikit-0.9.0/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.9.0/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.9.0/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/augmentors/schemes/base.py` & `caikit-0.9.0/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.9.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.9.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/__init__.py` & `caikit-0.9.0/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/base.py` & `caikit-0.9.0/caikit/core/data_model/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 
 # metaclass-generated field members cannot be detected by pylint
 # pylint: disable=no-member
 
 # Standard
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Dict, Optional, Type, Union
+from typing import Any, Dict, List, Optional, Type, Union
 import base64
 import json
 
 # Third Party
 from google.protobuf import json_format
-from google.protobuf.descriptor import Descriptor
+from google.protobuf.descriptor import Descriptor, FieldDescriptor, OneofDescriptor
 from google.protobuf.internal import type_checkers as proto_type_checkers
 from google.protobuf.message import Message as ProtoMessageType
 
 # First Party
 import alog
 
 # Local
@@ -62,14 +62,25 @@
     _FWD_DECL_FIELDS = "__fwd_decl_fields__"
 
     # Special instance attributes that an instance of a class derived from
     # DataBase may have. These are added to __slots__.
     _BACKEND_ATTR = "_backend"
     _WHICH_ONEOF_ATTR = "_which_oneof"
 
+    # When inferring which field in a oneof a given value should be used for
+    # based on the python type, we need to check types in order with bool first,
+    # ints next, then floats values that fit a "more flexible" type don't
+    # accidentally get assigned to the wrong field. These are the lists of int
+    # and bool type values in protobuf.
+    _PROTO_TYPE_ORDER = [FieldDescriptor.TYPE_BOOL] + [
+        val
+        for name, val in vars(FieldDescriptor).items()
+        if name.startswith("TYPE_") and "INT" in name
+    ]
+
     def __new__(mcs, name, bases, attrs):
         """When constructing a new data model class, we set the 'fields' class variable from the
         protobufs descriptor and then set the '__slots__' magic class attribute to fields.  This
         provides two benefits: (a) performance is improved since the classes only need to know
         about these attributes (b) it helps to enforce that all member variables in these classes
         are described in the protobufs.
 
@@ -182,16 +193,20 @@
             if field.enum_type is not None
         }
 
         # mapping of all oneofs and the fields that are part of them
         # NOTE: protobuf makes an interesting use of oneof to wrap types that
         #   should be explicitly optional. We don't want to consider these
         #   oneofs in the general oneof handling.
+
+        # Sort the names of the fields in this map to ensure that ordering is
+        # correct such that bool < int < float
+
         cls._fields_oneofs_map = {
-            oneof_name: [field.name for field in oneof.fields]
+            oneof_name: mcs._sorted_oneof_field_names(oneof)
             for oneof_name, oneof in cls._proto_class.DESCRIPTOR.oneofs_by_name.items()
             if len(oneof.fields) != 1 or oneof.name != f"_{oneof.fields[0].name}"
         }
         cls._fields_to_oneof = {
             field_name: oneof_name
             for (oneof_name, oneof_fields) in cls._fields_oneofs_map.items()
             for field_name in oneof_fields
@@ -405,14 +420,31 @@
                     ):
                         setattr(self, field_name, None)
 
         # Set docstring to the method explicitly
         setattr(__init__, "__doc__", docstring)
         return __init__
 
+    @classmethod
+    def _sorted_oneof_field_names(mcs, oneof: OneofDescriptor) -> List[str]:
+        """Helper to get the list of oneof fields while ensuring field names are
+        sorted such that bool < int < float. This ensures that when iterating
+        fields for which_oneof inference, lower-precedence types take
+        precedence.
+        """
+        return [
+            field.name
+            for field in sorted(
+                oneof.fields,
+                key=lambda fld: mcs._PROTO_TYPE_ORDER.index(fld.type)
+                if fld.type in mcs._PROTO_TYPE_ORDER
+                else len(mcs._PROTO_TYPE_ORDER),
+            )
+        ]
+
 
 class DataBase(metaclass=_DataBaseMetaClass):
     """Base class for all structures in the data model.
 
     Notes:
         All leaves in the hierarchy of derived classes should have a corresponding protobufs class
         defined in the interface definitions.  If not, an exception will be thrown at runtime.
@@ -514,14 +546,16 @@
     def _infer_which_oneof(cls, oneof_name: str, oneof_val: Any) -> Optional[str]:
         """Check each candidate field within the oneof to see if it's a type
         match
 
         NOTE: In the case where fields within a oneof have the same type, the
           first field whose type matches will be used!
         """
+        # NOTE: The list of field names are guaranteed to be sorted so that
+        #   bool < int < float
         for field_name in cls._fields_oneofs_map.get(oneof_name, []):
             if cls._is_valid_type_for_field(field_name, oneof_val):
                 return field_name
 
     def _get_which_oneof_dict(self) -> Dict[str, str]:
         which_oneof = getattr(self, _DataBaseMetaClass._WHICH_ONEOF_ATTR, None)
         if which_oneof is None:
@@ -552,14 +586,19 @@
         # a bad type
         if field_descriptor.type in [
             field_descriptor.TYPE_MESSAGE,
             field_descriptor.TYPE_ENUM,
         ]:
             return False
 
+        # If the field is a bool field, only accept python bools. Proto is ok to
+        # accept ints, but we are stricter than that.
+        if field_descriptor.type == field_descriptor.TYPE_BOOL:
+            return isinstance(val, bool)
+
         # If it's a primitive, use protobuf type checkers
         checker = proto_type_checkers.GetTypeChecker(field_descriptor)
         try:
             checker.CheckValue(val)
             return True
         except TypeError:
             pass
@@ -588,14 +627,15 @@
             proto:
                 A protocol buffer to serialize from.
 
         Returns:
             protobufs
                 A DataBase object.
         """
+        error.type_check("<COR45207671E>", ProtoMessageType, proto=proto)
         if cls._proto_class.DESCRIPTOR.name != proto.DESCRIPTOR.name:
             error(
                 "<COR71783894E>",
                 ValueError(
                     "class name `{}` does not match protobufs name `{}`".format(
                         cls._proto_class.DESCRIPTOR.name, proto.DESCRIPTOR.name
                     )
```

### Comparing `caikit-0.8.0/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.9.0/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/data_backends/base.py` & `caikit-0.9.0/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.9.0/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/dataobject.py` & `caikit-0.9.0/caikit/core/data_model/dataobject.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,26 @@
 """This module defines the @schema decorator which can be used to declare data
 model objects inline without manually defining the protobufs representation
 """
 
 
 # Standard
 from enum import Enum
-from typing import Any, Callable, List, Type, Union, get_args, get_origin
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Type,
+    Union,
+    get_args,
+    get_origin,
+)
 import dataclasses
 
 # Third Party
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import struct_pb2
 from google.protobuf.internal.enum_type_wrapper import EnumTypeWrapper
@@ -229,14 +240,61 @@
         interfaces_dir:  str
             The target directory (must already exist)
     """
     for proto_class in _AUTO_GEN_PROTO_CLASSES:
         proto_class.write_proto_file(interfaces_dir)
 
 
+def make_dataobject(
+    *,
+    name: str,
+    annotations: Dict[str, type],
+    bases: Optional[Iterable[type]] = None,
+    attrs: Optional[Dict[str, Any]] = None,
+    proto_name: Optional[str] = None,
+    **kwargs,
+) -> _DataObjectBaseMetaClass:
+    """Factory function for creating net-new dataobject classes
+
+    WARNING: This is a power-user feature that should be used with caution since
+        dynamically generated dataobject classes have portability issues due to
+        the use of global registries.
+
+    Kwargs:
+        name (str): The name of the class to create
+        annotations (Dict[str, type]): The type annotations for the class
+        bases (Optional[Iterable[type]]): Additional base classes beyond
+            DataObjectBase
+        attrs (Optional[Dict[str, Any]]): Additional class attributes beyond
+            __annotations__
+        proto_name (Optional[str]): Alternate name to use for the name of
+            protobuf message
+
+    Returns:
+        dataobject_class (_DataObjectBaseMetaClass): Programmatically created
+            class derived from DataObjectBase with the given name and
+            annotations
+    """
+    bases = tuple([DataObjectBase] + list(bases or []))
+    attrs = {
+        "__annotations__": annotations,
+        **(attrs or {}),
+    }
+    if proto_name is not None:
+        kwargs["name"] = proto_name
+    return dataobject(**kwargs)(
+        _DataObjectBaseMetaClass.__new__(
+            _DataObjectBaseMetaClass,
+            name=name,
+            bases=bases,
+            attrs=attrs,
+        )
+    )
+
+
 ## Implementation Details ######################################################
 
 
 def _dataobject_to_proto(*args, **kwargs):
     kwargs.setdefault("type_mapping", DATAOBJECT_PY_TO_PROTO_TYPES)
     return _DataobjectConverter(*args, **kwargs).descriptor
```

### Comparing `caikit-0.8.0/caikit/core/data_model/enums.py` & `caikit-0.9.0/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/json_dict.py` & `caikit-0.9.0/caikit/core/data_model/json_dict.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/producer.py` & `caikit-0.9.0/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.9.0/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/streams/__init__.py` & `caikit-0.9.0/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/streams/converter.py` & `caikit-0.9.0/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.9.0/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/streams/data_stream.py` & `caikit-0.9.0/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/streams/resolver.py` & `caikit-0.9.0/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/data_model/streams/validator.py` & `caikit-0.9.0/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/model_manager.py` & `caikit-0.9.0/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/module_backends/__init__.py` & `caikit-0.9.0/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/module_backends/backend_types.py` & `caikit-0.9.0/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/module_backends/base.py` & `caikit-0.9.0/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/module_backends/local_backend.py` & `caikit-0.9.0/caikit/core/module_backends/local_backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import alog
 
 # Local
 from ..modules.base import ModuleBase
 from ..modules.config import ModuleConfig
 from ..registries import module_registry
 from ..toolkit.errors import error_handler
+from ..toolkit.wip_decorator import TempDisableWIP
 from .backend_types import register_backend_type
 from .base import SharedLoadBackendBase, SharedTrainBackendBase
 
 log = alog.use_channel("LCLBKND")
 error = error_handler.get(log)
 
 
@@ -76,8 +77,9 @@
             "Could not load MODULE_ID %s with %s",
             module_id,
             self.backend_type,
         )
 
 
 # Register local backend
-register_backend_type(LocalBackend)
+with TempDisableWIP():
+    register_backend_type(LocalBackend)
```

### Comparing `caikit-0.8.0/caikit/core/module_backends/module_backend_config.py` & `caikit-0.9.0/caikit/core/module_backends/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/modules/__init__.py` & `caikit-0.9.0/caikit/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/modules/base.py` & `caikit-0.9.0/caikit/core/modules/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/modules/config.py` & `caikit-0.9.0/caikit/core/modules/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/modules/decorator.py` & `caikit-0.9.0/caikit/core/modules/decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/modules/loader.py` & `caikit-0.9.0/caikit/core/modules/loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/modules/meta.py` & `caikit-0.9.0/caikit/core/modules/meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/modules/saver.py` & `caikit-0.9.0/caikit/core/modules/saver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/registries.py` & `caikit-0.9.0/caikit/core/registries.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/signature_parsing/__init__.py` & `caikit-0.9.0/caikit/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/signature_parsing/docstrings.py` & `caikit-0.9.0/caikit/core/signature_parsing/docstrings.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,22 +208,20 @@
         if candidate_type is not None:
             valid_candidates.append(candidate_type)
             log.debug2(f"Found valid candidate type on sys.modules: {candidate_type}")
             continue
 
         # If the type was not fully qualified (like a `ProducerId`), look in a couple well known
         # places - the caikit core data model itself
-        candidate_type = _extract_type_from_pymodule(
-            caikit.interfaces.common.data_model, type_name
-        )
+        candidate_type = _extract_type_from_pymodule(caikit.core.data_model, type_name)
         if candidate_type is not None:
             valid_candidates.append(candidate_type)
             log.debug2(
                 # pylint: disable=line-too-long
-                f"Found valid candidate type on caikit.interfaces.common.data_model: {candidate_type}"
+                f"Found valid candidate type on caikit.core.data_model: {candidate_type}"
             )
             continue
         # ...And the data model within the interfaces, including those defined in library
         try:
             candidate_type = DataBase.get_class_for_name(type_name)
         except ValueError:
             log.debug2(f"Data model match failed on {candidate_type}, continuing")
```

### Comparing `caikit-0.8.0/caikit/core/signature_parsing/module_signature.py` & `caikit-0.9.0/caikit/core/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/signature_parsing/parsers.py` & `caikit-0.9.0/caikit/core/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/task.py` & `caikit-0.9.0/caikit/core/task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/toolkit/__init__.py` & `caikit-0.9.0/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/toolkit/compatibility.py` & `caikit-0.9.0/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/toolkit/errors/__init__.py` & `caikit-0.9.0/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.9.0/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.9.0/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/toolkit/fileio.py` & `caikit-0.9.0/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/toolkit/logging.py` & `caikit-0.9.0/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.9.0/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/toolkit/serializers.py` & `caikit-0.9.0/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/core/toolkit/wip_decorator.py` & `caikit-0.9.0/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/interfaces/common/__init__.py` & `caikit-0.9.0/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.9.0/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/interfaces/common/data_model/producer.py` & `caikit-0.9.0/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/interfaces/runtime/__init__.py` & `caikit-0.9.0/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.9.0/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.9.0/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/__init__.py` & `caikit-0.9.0/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/dump_services.py` & `caikit-0.9.0/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/grpc_server.py` & `caikit-0.9.0/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/interceptors/__init__.py` & `caikit-0.9.0/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.9.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/metrics/__init__.py` & `caikit-0.9.0/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.9.0/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/model_management/__init__.py` & `caikit-0.9.0/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/model_management/batcher.py` & `caikit-0.9.0/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/model_management/loaded_model.py` & `caikit-0.9.0/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/model_management/model_loader.py` & `caikit-0.9.0/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/model_management/model_manager.py` & `caikit-0.9.0/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/model_management/model_sizer.py` & `caikit-0.9.0/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/model_management/training_manager.py` & `caikit-0.9.0/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/protobufs/__init__.py` & `caikit-0.9.0/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.9.0/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.9.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.9.0/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.9.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.9.0/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.9.0/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.9.0/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.9.0/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.9.0/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/service_factory.py` & `caikit-0.9.0/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.9.0/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/service_generation/create_service.py` & `caikit-0.9.0/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.9.0/caikit/runtime/service_generation/data_stream_source.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,20 +23,15 @@
 
 # First Party
 from py_to_proto.dataclass_to_proto import Annotated, OneofField
 import alog
 
 # Local
 from caikit.core.data_model.base import DataBase
-from caikit.core.data_model.dataobject import (
-    DataObjectBase,
-    _DataObjectBaseMetaClass,
-    _make_oneof_init,
-    dataobject,
-)
+from caikit.core.data_model.dataobject import _make_oneof_init, make_dataobject
 from caikit.core.data_model.streams.data_stream import DataStream
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 import caikit
 
 # This global holds the mapping of element types to their respective
 # DataStreamSource wrappers so that the same message is not recreated
 # unnecessarily
@@ -198,89 +193,64 @@
 
         # Set up the "sub classes." In python, this is the same as creating a
         # standalone class with a __qualname__ that nests it under a parent
         # class. We do this outside the declaration of the parent class so that
         # these classes can be referenced within the Union annotation for the
         # outer class itself.
         package = "caikit_data_model.runtime"
-        JsonData = dataobject(package=package, name=f"{cls_name}JsonData")(
-            _DataObjectBaseMetaClass.__new__(
-                _DataObjectBaseMetaClass,
-                name="JsonData",
-                bases=(DataObjectBase,),
-                attrs={
-                    "__annotations__": {"data": List[data_element_type]},
-                    "__qualname__": f"{cls_name}.JsonData",
-                },
-            ),
-        )
-        File = dataobject(package=package, name=f"{cls_name}File")(
-            _DataObjectBaseMetaClass.__new__(
-                _DataObjectBaseMetaClass,
-                name="File",
-                bases=(DataObjectBase,),
-                attrs={
-                    "__annotations__": {"filename": str},
-                    "__qualname__": f"{cls_name}.File",
-                },
-            ),
-        )
-        ListOfFiles = dataobject(package=package, name=f"{cls_name}ListOfFiles")(
-            _DataObjectBaseMetaClass.__new__(
-                _DataObjectBaseMetaClass,
-                name="ListOfFiles",
-                bases=(DataObjectBase,),
-                attrs={
-                    "__annotations__": {"files": List[str]},
-                    "__qualname__": f"{cls_name}.ListOfFiles",
-                },
-            ),
-        )
-        Directory = dataobject(package=package, name=f"{cls_name}Directory")(
-            _DataObjectBaseMetaClass.__new__(
-                _DataObjectBaseMetaClass,
-                name="Directory",
-                bases=(DataObjectBase,),
-                attrs={
-                    "__annotations__": {
-                        "dirname": str,
-                        "extension": str,
-                    },
-                    "__qualname__": f"{cls_name}.Directory",
-                },
-            ),
+        JsonData = make_dataobject(
+            package=package,
+            proto_name=f"{cls_name}JsonData",
+            name="JsonData",
+            attrs={"__qualname__": f"{cls_name}.JsonData"},
+            annotations={"data": List[data_element_type]},
+        )
+        File = make_dataobject(
+            package=package,
+            proto_name=f"{cls_name}File",
+            name="File",
+            attrs={"__qualname__": f"{cls_name}.File"},
+            annotations={"filename": str},
+        )
+        ListOfFiles = make_dataobject(
+            package=package,
+            proto_name=f"{cls_name}ListOfFiles",
+            name="ListOfFiles",
+            attrs={"__qualname__": f"{cls_name}.ListOfFiles"},
+            annotations={"files": List[str]},
+        )
+        Directory = make_dataobject(
+            package=package,
+            proto_name=f"{cls_name}Directory",
+            name="Directory",
+            attrs={"__qualname__": f"{cls_name}.Directory"},
+            annotations={"dirname": str, "extension": str},
         )
 
         # Create the outer class that encapsulates the Union (oneof) or the
         # various types of input sources
-        data_object = dataobject(package=package)(
-            _DataObjectBaseMetaClass.__new__(
-                _DataObjectBaseMetaClass,
-                name=cls_name,
-                bases=(DataObjectBase, DataStreamSourceBase),
-                attrs={
-                    "ELEMENT_TYPE": data_element_type,
-                    JsonData.__name__: JsonData,
-                    File.__name__: File,
-                    ListOfFiles.__name__: ListOfFiles,
-                    Directory.__name__: Directory,
-                    "__annotations__": {
-                        "data_stream": Union[
-                            Annotated[JsonData, OneofField(JsonData.__name__.lower())],
-                            Annotated[File, OneofField(File.__name__.lower())],
-                            Annotated[
-                                ListOfFiles, OneofField(ListOfFiles.__name__.lower())
-                            ],
-                            Annotated[
-                                Directory, OneofField(Directory.__name__.lower())
-                            ],
-                        ],
-                    },
-                },
-            )
+        data_object = make_dataobject(
+            package=package,
+            name=cls_name,
+            bases=(DataStreamSourceBase,),
+            attrs={
+                "ELEMENT_TYPE": data_element_type,
+                JsonData.__name__: JsonData,
+                File.__name__: File,
+                ListOfFiles.__name__: ListOfFiles,
+                Directory.__name__: Directory,
+            },
+            annotations={
+                "data_stream": Union[
+                    Annotated[JsonData, OneofField(JsonData.__name__.lower())],
+                    Annotated[File, OneofField(File.__name__.lower())],
+                    Annotated[ListOfFiles, OneofField(ListOfFiles.__name__.lower())],
+                    Annotated[Directory, OneofField(Directory.__name__.lower())],
+                ],
+            },
         )
 
         # Add this data stream source to the common data model and the module
         # where it was declared
         setattr(
             caikit.interfaces.common.data_model,
             cls_name,
```

### Comparing `caikit-0.8.0/caikit/runtime/service_generation/protoable.py` & `caikit-0.9.0/caikit/runtime/service_generation/protoable.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,29 +120,40 @@
 
 def is_protoable_type(arg_type: Type) -> bool:
     """
     Returns True if arg_type is in PROTO_TYPE_MAP(float, int, bool, str, bytes)
     Or if it's an imported Caikit data model class.
     Or if it's a Union of at least one of those.
     Or if it's a List of one of those.
+    Or if it's a Dict of one of those.
     False otherwise"""
     proto_primitive_set = list(DATAOBJECT_PY_TO_PROTO_TYPES.keys())
-
+    protoable = False
     if arg_type in proto_primitive_set:
-        return True
-    if is_data_model_type(arg_type):
-        return True
-
-    if typing.get_origin(arg_type) == list:
+        protoable = True
+    elif is_data_model_type(arg_type):
+        protoable = True
+    elif typing.get_origin(arg_type) == list:
         log.debug2("Arg is List")
         if len(typing.get_args(arg_type)) == 0:
             log.debug2("List annotation has no type")
-            return False
-        return typing.get_args(arg_type)[0] in proto_primitive_set
-
-    if typing.get_origin(arg_type) == Union:
+            protoable = False
+        else:
+            protoable = typing.get_args(arg_type)[0] in proto_primitive_set
+    elif typing.get_origin(arg_type) == dict:
+        log.debug2("Arg is Dict")
+        if len(typing.get_args(arg_type)) == 0:
+            log.debug2("Dict annotation has no type")
+            protoable = False
+        else:
+            protoable = (
+                typing.get_args(arg_type)[0] in proto_primitive_set
+                and typing.get_args(arg_type)[1] in proto_primitive_set
+            )
+    elif typing.get_origin(arg_type) == Union:
         log.debug2("Arg is Union")
         # pylint: disable=use-a-generator
-        return any([is_protoable_type(arg) for arg in typing.get_args(arg_type)])
+        protoable = any([is_protoable_type(arg) for arg in typing.get_args(arg_type)])
 
-    log.debug2("Arg is not protoable, arg_type: %s", arg_type)
-    return False
+    if not protoable:
+        log.debug2("Arg is not protoable, arg_type: %s", arg_type)
+    return protoable
```

### Comparing `caikit-0.8.0/caikit/runtime/service_generation/rpcs.py` & `caikit-0.9.0/caikit/runtime/service_generation/rpcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,15 @@
 
 # Local
 from . import protoable, type_helpers
 from .compatibility_checker import ApiFieldNames
 from .data_stream_source import make_data_stream_source
 from caikit.core import ModuleBase, TaskBase
 from caikit.core.data_model.base import DataBase
-from caikit.core.data_model.dataobject import (
-    DataObjectBase,
-    _DataObjectBaseMetaClass,
-    dataobject,
-)
+from caikit.core.data_model.dataobject import make_dataobject
 from caikit.core.signature_parsing import CaikitMethodSignature, CustomSignature
 from caikit.interfaces.runtime.data_model import ModelPointer, TrainingJob
 
 log = alog.use_channel("RPC-SERIALIZERS")
 
 INDENT = "    "
 
@@ -70,33 +66,28 @@
         }
         optional_properties = {
             triple[1]: Annotated[Optional[triple[0]], FieldNumber(triple[2])]
             for triple in self.request.triples
             if triple[1] in self.request.default_map
         }
         attrs = copy.copy(self.request.default_map)
-        attrs["__annotations__"] = {**properties, **optional_properties}
 
         if not properties and not optional_properties:
             log.warning(
                 "No arguments found for request %s. Cannot generate rpc",
                 self.request.name,
             )
             return None
 
-        decorator = dataobject(package=package_name)
-        cls_ = _DataObjectBaseMetaClass.__new__(
-            _DataObjectBaseMetaClass,
+        return make_dataobject(
+            package=package_name,
             name=self.request.name,
-            bases=(DataObjectBase,),
             attrs=attrs,
+            annotations={**properties, **optional_properties},
         )
-        decorated_cls = decorator(cls_)
-
-        return decorated_cls
 
     def create_rpc_json(self, package_name: str) -> Dict:
         """Return json snippet for the service definition of this RPC"""
         if self.module_list[0].TASK_CLASS.is_output_streaming_task():
             output_type_name = (
                 typing.get_args(self.return_type)[0]
                 .get_proto_class()
```

### Comparing `caikit-0.8.0/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.9.0/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/servicers/__init__.py` & `caikit-0.9.0/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.9.0/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
+from contextlib import contextmanager
 from importlib.metadata import version
-from typing import Set
+from typing import Iterable, Optional, Set, Union
 import traceback
 
 # Third Party
 from google.protobuf.descriptor import FieldDescriptor
-from grpc import StatusCode
+from google.protobuf.message import Message as ProtobufMessage
+from grpc import ServicerContext, StatusCode
 from prometheus_client import Counter, Summary
 
 # First Party
 import alog
 
 # Local
 from caikit import get_config
 from caikit.core import ModuleBase
+from caikit.core.data_model import DataBase
 from caikit.runtime.metrics.rpc_meter import RPCMeter
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.service_factory import ServicePackage
 from caikit.runtime.service_generation.rpcs import TaskPredictRPC
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.import_util import clean_lib_names
 from caikit.runtime.utils.servicer_util import (
@@ -121,106 +124,151 @@
             "<RUN76884779I>",
             "Constructed inference service for library: %s, version: %s",
             library,
             lib_version,
         )
         super()
 
-    def Predict(self, request, context):
+    def Predict(
+        self,
+        request: ProtobufMessage,
+        context: ServicerContext,
+    ) -> Union[ProtobufMessage, Iterable[ProtobufMessage]]:
         """Global predict RPC -- Mocks the invocation of a Caikit Library module.run()
         method for a loaded Caikit Library model
 
         Args:
-            request(object):
+            request (ProtobufMessage):
                 A deserialized RPC request message
-            context(grpc.ServicerContext): Context object (contains request metadata, etc)
+            context (ServicerContext):
+                Context object (contains request metadata, etc)
 
         Returns:
-            response (object):
+            response (Union[ProtobufMessage, Iterable[ProtobufMessage]]):
                 A Caikit Library data model response object
         """
+        # Make sure the request has a model before doing anything
         request_name = request.DESCRIPTOR.name
-        outer_scope_name = "GlobalPredictServicer.Predict:%s" % request_name
-        inner_scope_name = (
-            "GlobalPredictServicer.Predict.caikit_library_run:%s" % request_name
-        )
-
-        try:
-            with alog.ContextLog(log.debug, outer_scope_name):
-                # Make sure the request has a model before doing anything
-                model_id = get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY)
+        model_id = get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY)
+        with self._handle_predict_exceptions(model_id, request_name):
+            with alog.ContextLog(
+                log.debug, "GlobalPredictServicer.Predict:%s", request_name
+            ):
                 # Retrieve the model from the model manager
                 log.debug("<RUN52259029D>", "Retrieving model '%s'", model_id)
                 model = self._model_manager.retrieve_model(model_id)
-
-                self._verify_model_task(model, request_name)
-
                 model_class = type(model)
                 # Unmarshall the request object into the required module run argument(s)
                 with PREDICT_FROM_PROTO_SUMMARY.labels(
                     grpc_request=request_name, model_id=model_id
                 ).time():
                     caikit_library_request = build_caikit_library_request_dict(
                         request,
                         model_class.RUN_SIGNATURE,
                     )
-
-                # NB: we previously recorded the size of the request, and timed this module to
-                # provide a rudimentary throughput metric of size / time
-                with alog.ContextLog(log.debug, inner_scope_name):
-                    with PREDICT_CAIKIT_LIBRARY_SUMMARY.labels(
-                        grpc_request=request_name, model_id=model_id
-                    ).time():
-                        if self.use_abortable_threads:
-                            work = AbortableAction(
-                                CallAborter(context),
-                                model.run,
-                                **caikit_library_request,
-                            )
-                            response = work.do()
-                        else:
-                            response = model.run(**caikit_library_request)
+                response = self.predict_model(
+                    request_name,
+                    model_id,
+                    aborter=CallAborter(context)
+                    if self.use_abortable_threads
+                    else None,
+                    **caikit_library_request,
+                )
 
                 # Marshall the response to the necessary return type
                 with PREDICT_TO_PROTO_SUMMARY.labels(
                     grpc_request=request_name, model_id=model_id
                 ).time():
                     if model.TASK_CLASS.is_output_streaming_task():
                         response_proto = build_proto_stream(response)
                     else:
                         response_proto = build_proto_response(response)
+                return response_proto
+
+    def predict_model(
+        self,
+        request_name: str,
+        model_id: str,
+        aborter: Optional[CallAborter] = None,
+        **kwargs,
+    ) -> Union[DataBase, Iterable[DataBase]]:
+        """Run a prediction against the given model using the raw arguments to
+        the model's run function.
+
+        Args:
+            request_name (str):
+                The name of the request message to validate the model's task
+            model_id (str):
+                The ID of the loaded model
+            aborter (Optional[CallAborter]):
+                If using abortable calls, this is the aborter to use
+            **kwargs:
+                Keyword arguments to pass to the model's run function
+
+        Returns:
+            response (Union[DataBase, Iterable[DataBase]]):
+                The object (unary) or objects (output stream) produced by the
+                inference request
+        """
+
+        with self._handle_predict_exceptions(model_id, request_name):
+            model = self._model_manager.retrieve_model(model_id)
+            self._verify_model_task(model, request_name)
+
+            # NB: we previously recorded the size of the request, and timed this module to
+            # provide a rudimentary throughput metric of size / time
+            with alog.ContextLog(
+                log.debug,
+                "GlobalPredictServicer.Predict.caikit_library_run:%s",
+                request_name,
+            ):
+                with PREDICT_CAIKIT_LIBRARY_SUMMARY.labels(
+                    grpc_request=request_name, model_id=model_id
+                ).time():
+                    if aborter is not None:
+                        work = AbortableAction(aborter, model.run, **kwargs)
+                        response = work.do()
+                    else:
+                        response = model.run(**kwargs)
 
             # Update Prometheus metrics
             PREDICT_RPC_COUNTER.labels(
                 grpc_request=request_name, code=StatusCode.OK.name, model_id=model_id
             ).inc()
             if get_config().runtime.metering.enabled:
                 self.rpc_meter.update_metrics(str(type(model)))
-            return response_proto
+            return response
+
+    ## Implementation Details ##################################################
+
+    @contextmanager
+    def _handle_predict_exceptions(self, model_id: str, request_name: str):
+        try:
+            yield
 
         except CaikitRuntimeException as e:
             log_dict = {
                 "log_code": "<RUN50530380W>",
                 "message": e.message,
-                "model_id": get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY),
+                "model_id": model_id,
                 "error_id": e.id,
             }
             log.warning({**log_dict, **e.metadata})
             PREDICT_RPC_COUNTER.labels(
                 grpc_request=request_name, code=e.status_code.name, model_id=model_id
             ).inc()
             raise e
 
         # Duplicate code in global_train_servicer
         # pylint: disable=duplicate-code
         except (TypeError, ValueError) as e:
             log_dict = {
                 "log_code": "<RUN490439039W>",
                 "message": repr(e),
-                "model_id": get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY),
+                "model_id": model_id,
                 "stack_trace": traceback.format_exc(),
             }
             log.warning(log_dict)
             PREDICT_RPC_COUNTER.labels(
                 grpc_request=request_name,
                 code=StatusCode.INVALID_ARGUMENT.name,
                 model_id=model_id,
@@ -230,15 +278,15 @@
                 f"Exception raised during inference. This may be a problem with your input: {e}",
             ) from e
 
         except Exception as e:
             log_dict = {
                 "log_code": "<RUN49049070W>",
                 "message": repr(e),
-                "model_id": get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY),
+                "model_id": model_id,
                 "stack_trace": traceback.format_exc(),
             }
             log.warning(log_dict)
             PREDICT_RPC_COUNTER.labels(
                 grpc_request=request_name,
                 code=StatusCode.INTERNAL.name,
                 model_id=model_id,
```

### Comparing `caikit-0.8.0/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.9.0/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.9.0/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.9.0/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.9.0/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/types/__init__.py` & `caikit-0.9.0/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/types/aborted_exception.py` & `caikit-0.9.0/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.9.0/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.9.0/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/utils/__init__.py` & `caikit-0.9.0/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/utils/import_util.py` & `caikit-0.9.0/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/utils/servicer_util.py` & `caikit-0.9.0/caikit/runtime/utils/servicer_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,16 +44,23 @@
 def validate_caikit_library_class_exists(cdm, class_name):
     try:
         # Attempt to instantiate a Caikit* CDM class of the specified
         # output type
         return getattr(cdm, class_name)
 
     except AttributeError as e:
-        log.error("<RUN24024010E>", "No Caikit Library CDM class for %s", class_name)
-        raise e
+        log.warning("<RUN24024050W>", "No Caikit Library CDM class for %s", class_name)
+        # Look up the data model class corresponding to the given name
+        dm_class_name = DataBase.get_class_for_name(class_name=class_name)
+        if not dm_class_name:
+            log.error(
+                "<RUN24024010E>", "No Caikit Library CDM class for %s", class_name
+            )
+            raise e
+        return dm_class_name
 
 
 def validate_caikit_library_class_method_exists(caikit_library_class, method_name):
     try:
         getattr(caikit_library_class, method_name)
 
     except AttributeError as e:
@@ -127,14 +134,17 @@
     if not isinstance(obj, FieldDescriptor):
         log.warning(
             "<RUN24033310D>",
             "Type [%s] should be FieldDescriptor",
             type(obj),
         )
         return False
+
+    if obj.type == FieldDescriptor.TYPE_MESSAGE and obj.message_type.name == "Struct":
+        return True
     return obj.type not in NON_PRIMITIVE_TYPES
 
 
 def get_metadata(context, key, required=True):
     """Retrieve a value from the gRPC ServicerContext invocation metadata
     dictionary with the given key
 
@@ -201,14 +211,25 @@
         input_proto_msg = method.input_type
 
         # Iterate over each field in this input RPC message...
         for field in input_proto_msg.fields:
             # and check to make that it is either a primitive protobufs type or that
             # we have a data model class that we can deserialize the protobufs with
             if not is_protobuf_primitive_field(field):
+
+                if field.message_type and field.message_type.GetOptions().map_entry:
+                    log.debug(
+                        "<RUN51658878D>",
+                        "Field: [%s] is a map of key type: [%s] and value type: [%s]",
+                        field.name,
+                        field.message_type.fields[0].type,
+                        field.message_type.fields[1].type,
+                    )
+                    continue
+
                 # ... or that we can get the field type name, e.g., RawDocument...
                 field_type = input_proto_msg.fields_by_name[
                     field.name
                 ].message_type.name
 
                 # ...and ensuring that we can load a corresponding object from the Caikit* CDM
                 caikit_library_class = validate_caikit_library_class_exists(
```

### Comparing `caikit-0.8.0/caikit/runtime/work_management/__init__.py` & `caikit-0.9.0/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/work_management/abortable_action.py` & `caikit-0.9.0/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/work_management/call_aborter.py` & `caikit-0.9.0/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.9.0/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/caikit/runtime/work_management/train_executors.py` & `caikit-0.9.0/caikit/runtime/work_management/train_executors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/docs/Makefile` & `caikit-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/docs/adrs/001-module.md` & `caikit-0.9.0/docs/adrs/001-module.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/docs/adrs/010-data-model-definition.md` & `caikit-0.9.0/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/docs/adrs/015-runtime-service-generation.md` & `caikit-0.9.0/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/docs/adrs/018-shared-backends.md` & `caikit-0.9.0/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/docs/adrs/019-loader-stack.md` & `caikit-0.9.0/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/docs/architecture_club/04-25-23.md` & `caikit-0.9.0/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/docs/make.bat` & `caikit-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/docs/source/conf.py` & `caikit-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/start_runtime_with_sample_lib.py` & `caikit-0.9.0/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/text-sentiment/README.md` & `caikit-0.9.0/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/text-sentiment/client.py` & `caikit-0.9.0/examples/text-sentiment/client.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.9.0/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/text-sentiment/start_runtime.py` & `caikit-0.9.0/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.9.0/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.9.0/examples/text-sentiment/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.9.0/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.9.0/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.9.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py` & `caikit-0.9.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/releases.md` & `caikit-0.9.0/releases.md`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/scripts/check_deps.sh` & `caikit-0.9.0/scripts/check_deps.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/scripts/fmt.sh` & `caikit-0.9.0/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/__init__.py` & `caikit-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/base.py` & `caikit-0.9.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/config/test_configs.py` & `caikit-0.9.0/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.9.0/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.9.0/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.9.0/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/data_model/streams/test_converter.py` & `caikit-0.9.0/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.9.0/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.9.0/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/data_model/streams/test_resolver.py` & `caikit-0.9.0/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/data_model/streams/test_validator.py` & `caikit-0.9.0/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/data_model/test_base.py` & `caikit-0.9.0/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/data_model/test_dataobject.py` & `caikit-0.9.0/tests/core/data_model/test_dataobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Tests for the @dataobject decorator"""
 
 # Standard
 from dataclasses import dataclass, field, is_dataclass
 from enum import Enum
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 import copy
 import json
 import os
 import tempfile
 
 # Third Party
 from google.protobuf import descriptor as _descriptor
@@ -38,14 +38,16 @@
     dataobject,
 )
 from caikit.core.data_model import enums
 from caikit.core.data_model.base import DataBase, _DataBaseMetaClass
 from caikit.core.data_model.data_backends.dict_backend import DictBackend
 from caikit.core.data_model.dataobject import (
     _AUTO_GEN_PROTO_CLASSES,
+    CAIKIT_DATA_MODEL,
+    make_dataobject,
     render_dataobject_protos,
 )
 from caikit.core.data_model.enums import isprotobufenum
 from caikit.core.data_model.json_dict import JsonDict
 
 ## Helpers #####################################################################
 
@@ -229,14 +231,36 @@
     class Foo(DataObjectBase):
         bar: List[str]
 
     assert check_field_type(Foo.get_proto_class(), "bar", "TYPE_STRING")
     assert check_field_label(Foo.get_proto_class(), "bar", "LABEL_REPEATED")
 
 
+def test_dataobject_simple_dict():
+    """Make sure simple dicts work as expected"""
+
+    @dataobject
+    class Foo(DataObjectBase):
+        bar: Dict[str, int]
+
+    assert check_field_type(Foo.get_proto_class(), "bar", "TYPE_MESSAGE")
+    assert (
+        Foo.get_proto_class()
+        .DESCRIPTOR.fields_by_name["bar"]
+        .message_type.GetOptions()
+        .map_entry
+    )
+
+    dict_input = {"foo": 1, "bar": 2}
+    foo = Foo(bar=dict_input)
+    assert foo.bar == dict_input
+
+    assert Foo.from_proto(foo.to_proto()).bar == dict_input
+
+
 def test_dataobject_obj_refs_no_opt_types():
     """Make sure that references to other data objects and enums work as
     expected
     """
 
     @dataobject
     class BarEnum(Enum):
@@ -541,14 +565,37 @@
     backend2 = DictBackend(data_dict2)
     msg2 = Foo.from_backend(backend2)
     assert msg2.foo == 1234
     assert msg2.foo_int == 1234
     assert msg2.which_oneof("foo") == "foo_int"
 
 
+def test_dataobject_oneof_numeric_type_precedence():
+    """Make sure that when inferring the which field from the python type, the
+    value of bool < int < float is respected
+    """
+
+    @dataobject
+    class Foo(DataObjectBase):
+        value: Union[
+            # NOTE: The order matters here. Since float is declared first, it
+            #   would naturally occur before int without correct sorting
+            Annotated[float, OneofField("float_val")],
+            Annotated[int, OneofField("int_val")],
+            Annotated[bool, OneofField("bool_val")],
+        ]
+
+    foo_bool = Foo(True)
+    assert foo_bool.which_oneof("value") == "bool_val"
+    foo_int = Foo(123)
+    assert foo_int.which_oneof("value") == "int_val"
+    foo_float = Foo(1.23)
+    assert foo_float.which_oneof("value") == "float_val"
+
+
 def test_dataobject_round_trip_json():
     """Make sure that a dataobject class can serialize to/from json"""
 
     @dataobject
     class BazObj(DataObjectBase):
         foo: str
         bar: int
@@ -874,14 +921,59 @@
     assert desc.fields_by_name["baz"].type == fld.TYPE_STRING
     inst = Derived(1, "asdf", "qwer")
     assert inst.foo == 1
     assert inst.bar == "asdf"
     assert inst.baz == "qwer"
 
 
+def test_dataobject_union_repeated():
+    """Make sure that a oneof with lists of primitive fields works correctly"""
+
+    # convert
+    @dataobject
+    class Foo(DataObjectBase):
+        foo: Union[List[str], List[int]]
+
+    # The above behaves the same way as this:
+
+    # @dataobject
+    # class Foo(DataObjectBase):
+    #     @dataobject
+    #     class IntSequence(DataObjectBase):
+    #         values: List[int]
+
+    #     @dataobject
+    #     class StrSequence(DataObjectBase):
+    #         values: List[str]
+
+    #     foo: Union[IntSequence, StrSequence]
+
+    # proto round trip
+    foo_int = Foo.IntSequence(values=[1, 2])
+    foo1 = Foo(foo=foo_int)
+    assert foo1.which_oneof("foo") == "foo_int_sequence"
+    proto_repr_foo = foo1.to_proto()
+    assert Foo.from_proto(proto=proto_repr_foo).to_proto() == proto_repr_foo
+
+    # dict test
+    assert foo1.to_dict() == {"foo_int_sequence": {"values": [1, 2]}}
+
+    # json round trip
+    json_repr_foo = foo1.to_json()
+    assert json.loads(json_repr_foo) == {"foo_int_sequence": {"values": [1, 2]}}
+    baz_from_json = Foo.from_json(json_repr_foo)
+    assert baz_from_json.to_json() == json_repr_foo
+
+    foo_str = Foo.StrSequence(values=["hello", "world"])
+    foo2 = Foo(foo=foo_str)
+    assert foo2.which_oneof("foo") == "foo_str_sequence"
+    proto_repr_foo2 = foo2.to_proto()
+    assert Foo.from_proto(proto=proto_repr_foo2).to_proto() == proto_repr_foo2
+
+
 def test_dataobject_function_inheritance(temp_dpool):
     """Make sure inheritance works to override functionality without changing
     the schema of the parent
     """
 
     @dataobject
     class Base(DataObjectBase):
@@ -896,7 +988,49 @@
             return self.foo * 3
 
     b_inst = Base(1)
     assert b_inst.doit() == 2
 
     d_inst = Derived(1)
     assert d_inst.doit() == 3
+
+
+def test_make_dataobject_no_optionals(temp_dpool):
+    """Test that dataobject classes can be created dynamically without optional
+    values given
+    """
+    data_object = make_dataobject(
+        name="FooBar",
+        annotations={"foo": str, "bar": int},
+    )
+
+    assert data_object.__name__ == "FooBar"
+    assert data_object.__annotations__ == {"foo": str, "bar": int}
+    assert issubclass(data_object, DataObjectBase)
+    assert data_object._proto_class.DESCRIPTOR.name == "FooBar"
+    assert data_object._proto_class.DESCRIPTOR.file.package == CAIKIT_DATA_MODEL
+
+
+def test_make_dataobject_with_optionals(temp_dpool):
+    """Test that dataobject classes can be created dynamically with optional
+    values given
+    """
+
+    class OtherBase:
+        pass
+
+    data_object = make_dataobject(
+        name="FooBar",
+        annotations={"foo": str, "bar": int},
+        bases=(OtherBase,),
+        attrs={"prop": "val"},
+        proto_name="SomeOtherFooBar",
+        package="foo.bar.baz",
+    )
+
+    assert data_object.__name__ == "FooBar"
+    assert data_object.__annotations__ == {"foo": str, "bar": int}
+    assert issubclass(data_object, DataObjectBase)
+    assert issubclass(data_object, OtherBase)
+    assert data_object.prop == "val"
+    assert data_object._proto_class.DESCRIPTOR.name == "SomeOtherFooBar"
+    assert data_object._proto_class.DESCRIPTOR.file.package == "foo.bar.baz"
```

### Comparing `caikit-0.8.0/tests/core/data_model/test_enums.py` & `caikit-0.9.0/tests/core/data_model/test_enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/data_model/test_json_dict.py` & `caikit-0.9.0/tests/core/data_model/test_json_dict.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/data_model/test_producer.py` & `caikit-0.9.0/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/helpers.py` & `caikit-0.9.0/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/module_backends/test_backend_types.py` & `caikit-0.9.0/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/module_backends/test_module_backend_config.py` & `caikit-0.9.0/tests/core/module_backends/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/modules/test_module.py` & `caikit-0.9.0/tests/core/modules/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/modules/test_module_metadata.py` & `caikit-0.9.0/tests/core/modules/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/signature_parsing/__init__.py` & `caikit-0.9.0/tests/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/signature_parsing/test_docstrings.py` & `caikit-0.9.0/tests/core/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/signature_parsing/test_parsers.py` & `caikit-0.9.0/tests/core/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/test_imports.py` & `caikit-0.9.0/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/test_model_manager.py` & `caikit-0.9.0/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/test_no_write_permissions.py` & `caikit-0.9.0/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/test_task.py` & `caikit-0.9.0/tests/core/test_task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/toolkit/test_compatibility.py` & `caikit-0.9.0/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/toolkit/test_error_handler.py` & `caikit-0.9.0/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/toolkit/test_fileio.py` & `caikit-0.9.0/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.9.0/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/toolkit/test_serializers.py` & `caikit-0.9.0/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.9.0/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/data_model_helpers.py` & `caikit-0.9.0/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/config/config.yml` & `caikit-0.9.0/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.9.0/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/dummy_module.zip` & `caikit-0.9.0/tests/fixtures/dummy_module.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/dummy_module/config.yml` & `caikit-0.9.0/tests/fixtures/dummy_module/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/dummy_module_singleton/config.yml` & `caikit-0.9.0/tests/fixtures/dummy_module_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/fixtures.py` & `caikit-0.9.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/invalid.zip` & `caikit-0.9.0/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/linux.txt` & `caikit-0.9.0/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.9.0/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py` & `caikit-0.9.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py` & `caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py` & `caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py` & `caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py` & `caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py` & `caikit-0.9.0/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/generated/__init__.py` & `caikit-0.9.0/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/metrics/__init__.py` & `caikit-0.9.0/tests/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.9.0/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/model_management/__init__.py` & `caikit-0.9.0/tests/interfaces/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/model_management/test_batcher.py` & `caikit-0.9.0/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/model_management/test_model_loader.py` & `caikit-0.9.0/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/model_management/test_model_manager.py` & `caikit-0.9.0/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.9.0/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/model_management/test_training_manager.py` & `caikit-0.9.0/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/service_generation/test_create_service.py` & `caikit-0.9.0/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.9.0/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/service_generation/test_protoable.py` & `caikit-0.9.0/tests/runtime/service_generation/test_protoable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Standard
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 # Third Party
 import pytest
 
 # Local
 from caikit.runtime.service_generation.protoable import (
     extract_data_model_type_from_union,
@@ -107,7 +107,37 @@
 
 
 def test_to_output_dm_type_with_union_optional_dm():
     assert (
         extract_data_model_type_from_union(Union[Optional[SampleOutputType], str])
         == SampleOutputType
     )
+
+
+def test_to_protoable_signature_dict():
+    assert to_protoable_signature(
+        signature={"name": Dict[str, int]},
+    ) == {"name": Dict[str, int]}
+
+
+def test_to_protoable_signature_dict_int_keys():
+    assert to_protoable_signature(
+        signature={"name": Dict[int, float]},
+    ) == {"name": Dict[int, float]}
+
+
+def test_to_protoable_signature_unsupported_dict():
+    assert (
+        to_protoable_signature(
+            signature={"name": Dict[str, NonProtoable]},
+        )
+        == {}
+    )
+
+
+def test_to_protoable_signature_dict_incomplete_type_hint():
+    assert (
+        to_protoable_signature(
+            signature={"name": dict},
+        )
+        == {}
+    )
```

### Comparing `caikit-0.8.0/tests/runtime/service_generation/test_rpcs.py` & `caikit-0.9.0/tests/runtime/service_generation/test_rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.9.0/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/servicers/__init__.py` & `caikit-0.9.0/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.9.0/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,35 +18,33 @@
     # Standard
     from test.support.threading_helper import catch_threading_exception
 except (NameError, ModuleNotFoundError):
     from tests.base import catch_threading_exception
 
 # Standard
 import json
-import os
-import tempfile
 import threading
 import time
-import uuid
 
 # Third Party
 import grpc
 import pytest
 
 # Local
 from caikit.runtime.servicers.global_predict_servicer import GlobalPredictServicer
 from caikit.runtime.types.aborted_exception import AbortedException
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from sample_lib.data_model import SampleInputType, SampleOutputType
 from sample_lib.modules.sample_task import SampleModule
 from tests.fixtures import Fixtures
-import sample_lib
 
-HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
-HAPPY_PATH_RESPONSE = SampleOutputType(greeting="Hello Gabe").to_proto()
+HAPPY_PATH_INPUT_DM = SampleInputType(name="Gabe")
+HAPPY_PATH_RESPONSE_DM = SampleOutputType(greeting="Hello Gabe")
+HAPPY_PATH_INPUT = HAPPY_PATH_INPUT_DM.to_proto()
+HAPPY_PATH_RESPONSE = HAPPY_PATH_RESPONSE_DM.to_proto()
 
 
 def test_calling_predict_should_raise_if_module_raises(
     sample_inference_service, sample_predict_servicer, sample_task_model_id
 ):
     with pytest.raises(CaikitRuntimeException) as context:
         # SampleModules will raise a RuntimeError if the throw flag is set
@@ -85,14 +83,28 @@
             sample_input=HAPPY_PATH_INPUT
         ),
         Fixtures.build_context(sample_task_model_id),
     )
     assert response == HAPPY_PATH_RESPONSE
 
 
+def test_global_predict_predict_model_direct(
+    sample_inference_service, sample_predict_servicer, sample_task_model_id
+):
+    """Test that the direct predict_model function can be called to bypass the
+    gRPC handler
+    """
+    response = sample_predict_servicer.predict_model(
+        request_name="SampleTaskRequest",
+        model_id=sample_task_model_id,
+        sample_input=HAPPY_PATH_INPUT_DM,
+    )
+    assert response == HAPPY_PATH_RESPONSE_DM
+
+
 def test_global_predict_aborts_long_running_predicts(
     sample_inference_service, sample_predict_servicer
 ):
     mock_manager = MagicMock()
 
     # return a dummy model from the mock model manager
     class UnresponsiveModel(SampleModule):
```

### Comparing `caikit-0.8.0/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.9.0/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.9.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.9.0/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.9.0/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/test_grpc_server.py` & `caikit-0.9.0/tests/runtime/test_grpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 import tls_test_tools
 
 # First Party
 import alog
 
 # Local
 from caikit import get_config
+from caikit.core.data_model.base import DataBase
 from caikit.interfaces.runtime.data_model import (
     TrainingInfoRequest,
     TrainingInfoResponse,
     TrainingJob,
     TrainingStatus,
 )
 from caikit.runtime.grpc_server import RuntimeGRPCServer
@@ -59,16 +60,17 @@
 from sample_lib import InnerModule
 from sample_lib.data_model import (
     OtherOutputType,
     SampleInputType,
     SampleOutputType,
     SampleTrainingType,
 )
-from tests.conftest import random_test_id, runtime_grpc_test_server, temp_config
+from tests.conftest import random_test_id, temp_config
 from tests.fixtures import Fixtures
+from tests.runtime.conftest import runtime_grpc_test_server
 import caikit
 import sample_lib
 
 ## Helpers #####################################################################
 
 log = alog.use_channel("TEST-SERVE-I")
 
@@ -401,14 +403,61 @@
     )
     expected_original_inference_response = OtherOutputType(
         farewell="goodbye: Gabe 42 times"
     ).to_proto()
     assert original_inference_response == expected_original_inference_response
 
 
+def test_train_primitive_model(
+    train_stub,
+    inference_stub,
+    training_management_stub,
+    sample_train_service,
+    sample_inference_service,
+):
+    """Test that we can make a successful training and inference call to the primitive module using primitive inputs"""
+
+    model_name = "primitive_trained_model"
+    train_request_class = DataBase.get_class_for_name(
+        "SampleTaskSamplePrimitiveModuleTrainRequest"
+    )
+    train_request = train_request_class(
+        model_name=model_name,
+        sample_input=SampleInputType(name="Gabe"),
+        simple_list=["hello", "world"],
+        union_list_str_sequence=train_request_class.StrSequence(
+            values=["str", "sequence"]
+        ),
+        training_params_json_dict={"foo": {"bar": [1, 2, 3]}},
+        training_params_dict={"layer_sizes": 100, "window_scaling": 200},
+        training_params_dict_int={1: 0.1, 2: 0.01},
+    ).to_proto()
+
+    training_response = train_stub.SampleTaskSamplePrimitiveModuleTrain(train_request)
+    is_good_train_response(
+        training_response,
+        HAPPY_PATH_TRAIN_RESPONSE,
+        model_name,
+        training_management_stub,
+    )
+
+    # make sure the trained model can run inference
+    predict_request = sample_inference_service.messages.SampleTaskRequest(
+        sample_input=HAPPY_PATH_INPUT
+    )
+
+    inference_response = inference_stub.SampleTaskPredict(
+        predict_request, metadata=[("mm-model-id", training_response.model_name)]
+    )
+    expected_inference_response = SampleOutputType(
+        greeting="hello: primitives! [1, 2, 3] 100"
+    ).to_proto()
+    assert inference_response == expected_inference_response
+
+
 ##### Test different datastream types #####
 def test_train_fake_module_ok_response_with_datastream_jsondata(
     train_stub,
     inference_stub,
     sample_train_service,
     sample_inference_service,
     training_management_stub,
```

### Comparing `caikit-0.8.0/tests/runtime/test_service_factory.py` & `caikit-0.9.0/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/utils/__init__.py` & `caikit-0.9.0/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/utils/test_import_util.py` & `caikit-0.9.0/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/utils/test_servicer_util.py` & `caikit-0.9.0/tests/runtime/utils/test_servicer_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         get_data_model(), "ProducerId"
     )
     assert validated_class == caikit.interfaces.common.data_model.producer.ProducerId
 
 
 def test_servicer_util_validate_caikit_library_class_exists_raises_for_garbage_input():
     """Test that validate_caikit_library_class_exists raises for garbage 'model'"""
-    with pytest.raises(AttributeError):
+    with pytest.raises(ValueError):
         validate_caikit_library_class_exists(get_data_model(), "NonExistentClass")
 
 
 # ---------------- Tests for validate_caikit_library_class_method_exists --------------------
 def test_service_util_validate_caikit_library_class_method_exists_doesnt_raise():
     """Test that validate_caikit_library_class_method_exists doesn't raise for valid methods"""
     try:
@@ -188,15 +188,15 @@
         validate_data_model(sample_inference_service.descriptor)
     except Exception as e:
         assert False, "Validation of interfaces failed for Predict!"
 
 
 def test_servicer_util_will_not_validate_arbitrary_service_descriptor():
     """Test that validate_data_model raises exception validating arbitrary ServiceDescriptor"""
-    with pytest.raises(AttributeError):
+    with pytest.raises(ValueError):
         validate_data_model(model_runtime_pb2._MODELRUNTIME)
 
 
 # ---------------- Tests for build_caikit_library_request_dict --------------------
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
```

### Comparing `caikit-0.8.0/tests/runtime/work_management/__init__.py` & `caikit-0.9.0/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.9.0/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.9.0/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.9.0/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.8.0/PKG-INFO` & `caikit-0.9.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,54 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.8.0
+Version: 0.9.0
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
 Requires-Dist: docstring-parser>=0.14.1,<0.16.0
-Requires-Dist: grpcio-health-checking>=1.35.0,<2.0
-Requires-Dist: grpcio-reflection>=1.35.0,<2.0
 Requires-Dist: grpcio>=1.35.0,<2.0,!=1.55.0
 Requires-Dist: ijson>=3.1.4,<3.3.0
-Requires-Dist: import-tracker>=3.1.5,<4
 Requires-Dist: munch>=2.5.0,<4.0
 Requires-Dist: numpy>=1.20,<2
-Requires-Dist: prometheus_client>=0.12.0,<1.0
 Requires-Dist: protobuf>=3.19.0,<5
-Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8
-Requires-Dist: py-to-proto>=0.3.0,<0.4.0,!=0.2.1
+Requires-Dist: py-to-proto>=0.3.1,<0.4.0,!=0.2.1
 Requires-Dist: PyYAML>=6.0,<7.0
-Requires-Dist: requests>=2.26.0,<3.0
 Requires-Dist: semver>=2.13.0,<4.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
+Requires-Dist: caikit[runtime-grpc] ; extra == "all"
+Requires-Dist: caikit[all, dev-test, dev-docs, dev-fmt, dev-build] ; extra == "all-dev"
+Requires-Dist: flit==3.8 ; extra == "dev-build"
+Requires-Dist: sphinx>=4.0.2,<8.0 ; extra == "dev-docs"
+Requires-Dist: sphinx-autoapi>=2.1.0 ; extra == "dev-docs"
+Requires-Dist: sphinx-rtd-theme~=1.2.1 ; extra == "dev-docs"
+Requires-Dist: pre-commit>=3.0.4,<4.0 ; extra == "dev-fmt"
+Requires-Dist: pylint>=2.16.2,<3.0 ; extra == "dev-fmt"
+Requires-Dist: pydeps==1.12.3 ; extra == "dev-fmt"
+Requires-Dist: pytest>=6.2.5,<7.0 ; extra == "dev-test"
+Requires-Dist: pytest-cov>=2.10.1,<3.0 ; extra == "dev-test"
+Requires-Dist: pytest-html>=3.1.1,<4.0 ; extra == "dev-test"
+Requires-Dist: tls_test_tools>=0.1.1 ; extra == "dev-test"
+Requires-Dist: wheel>=0.38.4 ; extra == "dev-test"
+Requires-Dist: grpcio-health-checking>=1.35.0,<2.0 ; extra == "runtime-grpc"
+Requires-Dist: grpcio-reflection>=1.35.0,<2.0 ; extra == "runtime-grpc"
+Requires-Dist: prometheus_client>=0.12.0,<1.0 ; extra == "runtime-grpc"
+Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8 ; extra == "runtime-grpc"
 Project-URL: Source, https://github.com/caikit/caikit
+Provides-Extra: all
+Provides-Extra: all-dev
+Provides-Extra: dev-build
+Provides-Extra: dev-docs
+Provides-Extra: dev-fmt
+Provides-Extra: dev-test
+Provides-Extra: runtime-grpc
 
 # Caikit
 
 [![Build Status](https://github.com/caikit/caikit/actions/workflows/build-library.yml/badge.svg?branch=main&label=tests)](https://github.com/caikit/caikit/actions)
 [![Minimum Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![Release](https://img.shields.io/github/v/release/caikit/caikit?include_prereleases&style=)](https://github.com/caikit/caikit/releases/)
 [![Read the Docs](https://img.shields.io/static/v1?label=readthedocs&message=reference&color=blue)](https://caikit.readthedocs.io/en/latest/)
```

