# Comparing `tmp/daisyfl-0.1.3.tar.gz` & `tmp/daisyfl-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daisyfl-0.1.3.tar", max compression
+gzip compressed data, was "daisyfl-0.4.5.tar", max compression
```

## Comparing `daisyfl-0.1.3.tar` & `daisyfl-0.4.5.tar`

### file list

```diff
@@ -1,118 +1,83 @@
--rw-r--r--   0        0        0    11358 2022-11-10 02:16:06.346918 daisyfl-0.1.3/LICENSE
--rw-r--r--   0        0        0     8480 2022-11-10 02:16:06.346918 daisyfl-0.1.3/README.md
--rw-r--r--   0        0        0     3697 2022-11-17 06:54:49.064119 daisyfl-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1115 2022-11-10 02:16:06.490918 daisyfl-0.1.3/src/py/daisyfl/__init__.py
--rw-r--r--   0        0        0     1231 2022-11-10 02:16:06.490918 daisyfl-0.1.3/src/py/daisyfl/client/__init__.py
--rw-r--r--   0        0        0    11297 2022-11-14 11:47:10.076943 daisyfl-0.1.3/src/py/daisyfl/client/app.py
--rw-r--r--   0        0        0     3733 2022-11-10 02:16:06.490918 daisyfl-0.1.3/src/py/daisyfl/client/client.py
--rw-r--r--   0        0        0     3367 2022-11-10 02:16:06.490918 daisyfl-0.1.3/src/py/daisyfl/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      714 2022-11-10 02:16:06.490918 daisyfl-0.1.3/src/py/daisyfl/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4671 2022-11-14 11:53:47.028855 daisyfl-0.1.3/src/py/daisyfl/client/grpc_client/connection.py
--rw-r--r--   0        0        0     7218 2022-11-10 02:16:06.490918 daisyfl-0.1.3/src/py/daisyfl/client/grpc_client/message_handler.py
--rw-r--r--   0        0        0     5084 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/client/numpy_client.py
--rw-r--r--   0        0        0     1625 2022-11-14 11:47:56.296948 daisyfl-0.1.3/src/py/daisyfl/client/zone_client.py
--rw-r--r--   0        0        0     3967 2022-11-14 01:44:01.776230 daisyfl-0.1.3/src/py/daisyfl/common/__init__.py
--rw-r--r--   0        0        0     1830 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/common/dp.py
--rw-r--r--   0        0        0     3483 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/common/logger.py
--rw-r--r--   0        0        0     3938 2022-11-14 08:26:17.346839 daisyfl-0.1.3/src/py/daisyfl/common/parameter.py
--rw-r--r--   0        0        0    15254 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/common/serde.py
--rw-r--r--   0        0        0     3844 2022-11-11 07:40:12.258882 daisyfl-0.1.3/src/py/daisyfl/common/typing.py
--rw-r--r--   0        0        0       53 2022-11-10 10:21:08.678229 daisyfl-0.1.3/src/py/daisyfl/operation/__init__.py
--rw-r--r--   0        0        0      323 2022-11-10 10:17:01.271000 daisyfl-0.1.3/src/py/daisyfl/operation/base/__init__.py
--rw-r--r--   0        0        0     1870 2022-11-11 04:51:34.688156 daisyfl-0.1.3/src/py/daisyfl/operation/base/client_logic.py
--rw-r--r--   0        0        0     3908 2022-11-10 10:03:34.138067 daisyfl-0.1.3/src/py/daisyfl/operation/base/server_logic.py
--rw-r--r--   0        0        0     1397 2022-11-10 05:01:51.234283 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/__init__.py
--rw-r--r--   0        0        0     2533 2022-11-10 05:01:51.390282 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/aggregate.py
--rw-r--r--   0        0        0     4537 2022-11-10 05:03:10.906201 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     4895 2022-11-10 05:03:27.882183 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5987 2022-11-10 05:01:51.734282 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6846 2022-11-10 05:01:51.874282 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7096 2022-11-10 05:01:51.950282 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedadam.py
--rw-r--r--   0        0        0    11239 2022-11-10 05:01:52.174282 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedavg.py
--rw-r--r--   0        0        0    10028 2022-11-10 05:01:52.018282 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8998 2022-11-10 05:01:52.318282 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedavgm.py
--rw-r--r--   0        0        0     5366 2022-11-10 05:01:52.390282 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedopt.py
--rw-r--r--   0        0        0     7116 2022-11-10 05:01:52.466281 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedyogi.py
--rw-r--r--   0        0        0    10756 2022-11-10 05:01:52.538281 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/qfedavg.py
--rw-r--r--   0        0        0     7493 2022-11-10 05:01:52.622281 daisyfl-0.1.3/src/py/daisyfl/operation/strategy/strategy.py
--rw-r--r--   0        0        0      563 2022-11-10 05:27:38.816483 daisyfl-0.1.3/src/py/daisyfl/operation/utils/__init__.py
--rw-r--r--   0        0        0     4410 2022-11-10 05:18:39.703607 daisyfl-0.1.3/src/py/daisyfl/operation/utils/op_tools.py
--rw-r--r--   0        0        0       94 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/__init__.py
--rw-r--r--   0        0        0      128 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/base/__init__.py
--rw-r--r--   0        0        0     1861 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/base/client_logic.py
--rw-r--r--   0        0        0     4181 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/base/server_logic.py
--rw-r--r--   0        0        0      276 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/msg_demo/__init__.py
--rw-r--r--   0        0        0     2606 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/msg_demo/client_logic.py
--rw-r--r--   0        0        0      291 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/msg_demo/common/__init__.py
--rw-r--r--   0        0        0      378 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/msg_demo/common/msg.py
--rw-r--r--   0        0        0     5558 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/msg_demo/server_logic.py
--rw-r--r--   0        0        0     1865 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/msg_demo/zone_client_logic.py
--rw-r--r--   0        0        0     5423 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/msg_demo/zone_server_logic.py
--rw-r--r--   0        0        0      894 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/__init__.py
--rw-r--r--   0        0        0    12032 2022-11-14 01:45:35.799770 daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/client_logic.py
--rw-r--r--   0        0        0        0 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/common/__init__.py
--rw-r--r--   0        0        0     1827 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/common/typing.py
--rw-r--r--   0        0        0    19456 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/server_logic.py
--rw-r--r--   0        0        0        0 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/utils/__init__.py
--rw-r--r--   0        0        0    10071 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/utils/primitives.py
--rw-r--r--   0        0        0      676 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/__init__.py
--rw-r--r--   0        0        0     9965 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/driver_pb2.py
--rw-r--r--   0        0        0     3138 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5747 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1670 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     6773 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/fleet_pb2.py
--rw-r--r--   0        0        0     1962 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4103 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1172 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     3160 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/task_pb2.py
--rw-r--r--   0        0        0      986 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    62902 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/transport_pb2.py
--rw-r--r--   0        0        0    23142 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2601 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      781 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/py.typed
--rw-r--r--   0        0        0     1249 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/__init__.py
--rw-r--r--   0        0        0    11969 2022-11-14 11:50:20.472935 daisyfl-0.1.3/src/py/daisyfl/server/app.py
--rw-r--r--   0        0        0     4801 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/client_manager.py
--rw-r--r--   0        0        0     2213 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/client_proxy.py
--rw-r--r--   0        0        0     1058 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/criterion.py
--rw-r--r--   0        0        0      705 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/driver/__init__.py
--rw-r--r--   0        0        0     1928 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/fleet/__init__.py
--rw-r--r--   0        0        0     1458 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/fleet/fleet_servicer.py
--rw-r--r--   0        0        0      714 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/grpc_server/__init__.py
--rw-r--r--   0        0        0     5596 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
--rw-r--r--   0        0        0     6418 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/grpc_server/grpc_bridge.py
--rw-r--r--   0        0        0     4632 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
--rw-r--r--   0        0        0    11530 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/grpc_server/grpc_server.py
--rw-r--r--   0        0        0     3626 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/history.py
--rw-r--r--   0        0        0    16970 2022-11-14 01:40:37.229373 daisyfl-0.1.3/src/py/daisyfl/server/server.py
--rw-r--r--   0        0        0      120 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/shutdown.py
--rw-r--r--   0        0        0      702 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/state/__init__.py
--rw-r--r--   0        0        0     1397 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/__init__.py
--rw-r--r--   0        0        0     2533 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4534 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     4892 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5987 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6846 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7096 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11239 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/fedavg.py
--rw-r--r--   0        0        0    10028 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8998 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     5366 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7116 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/fedyogi.py
--rw-r--r--   0        0        0    10756 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7493 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/strategy/strategy.py
--rw-r--r--   0        0        0      701 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/server/task/__init__.py
--rw-r--r--   0        0        0     7334 2022-11-14 11:51:06.728922 daisyfl-0.1.3/src/py/daisyfl/server/task_manager.py
--rw-r--r--   0        0        0     1273 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/simulation/__init__.py
--rw-r--r--   0        0        0     7557 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/simulation/app.py
--rw-r--r--   0        0        0      727 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     4661 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0      936 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/utils/__init__.py
--rw-r--r--   0        0        0      121 2022-11-11 05:58:21.362104 daisyfl-0.1.3/src/py/daisyfl/utils/dynamic_loader.py
--rw-r--r--   0        0        0     5121 2022-11-10 02:16:06.494918 daisyfl-0.1.3/src/py/daisyfl/utils/tensorboard.py
--rw-r--r--   0        0        0    10326 2022-11-17 06:57:21.539226 daisyfl-0.1.3/setup.py
--rw-r--r--   0        0        0    10477 2022-11-17 06:57:21.539572 daisyfl-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-13 11:19:33.755489 daisyfl-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1158 2023-06-13 11:19:33.755489 daisyfl-0.4.5/README.md
+-rw-r--r--   0        0        0     3661 2023-06-21 00:25:20.622196 daisyfl-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1093 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/__init__.py
+-rw-r--r--   0        0        0     1171 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/__init__.py
+-rw-r--r--   0        0        0     9951 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/app.py
+-rw-r--r--   0        0        0     3733 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/client.py
+-rw-r--r--   0        0        0     1363 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/client_api_handler.py
+-rw-r--r--   0        0        0     3780 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/client_operator_manager.py
+-rw-r--r--   0        0        0     3367 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      714 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0    10038 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/connection.py
+-rw-r--r--   0        0        0     6704 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/message_handler.py
+-rw-r--r--   0        0        0     5084 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/numpy_client.py
+-rw-r--r--   0        0        0     4998 2023-06-17 09:18:06.051724 daisyfl-0.4.5/src/py/daisyfl/client/trainer.py
+-rw-r--r--   0        0        0     1663 2023-06-17 09:18:15.943647 daisyfl-0.4.5/src/py/daisyfl/client/zone_client.py
+-rw-r--r--   0        0        0     5644 2023-06-19 11:07:59.531140 daisyfl-0.4.5/src/py/daisyfl/common/__init__.py
+-rw-r--r--   0        0        0     1830 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/dp.py
+-rw-r--r--   0        0        0     3482 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/logger.py
+-rw-r--r--   0        0        0     1421 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/metadata.py
+-rw-r--r--   0        0        0     3938 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/parameter.py
+-rw-r--r--   0        0        0    16903 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/serde.py
+-rw-r--r--   0        0        0     4044 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/typing.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/base/__init__.py
+-rw-r--r--   0        0        0     1162 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/base/client_logic.py
+-rw-r--r--   0        0        0     5700 2023-06-19 13:00:12.324689 daisyfl-0.4.5/src/py/daisyfl/operator/base/server_logic.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/base_async/__init__.py
+-rw-r--r--   0        0        0     1162 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/base_async/client_logic.py
+-rw-r--r--   0        0        0     5383 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/base_async/server_logic.py
+-rw-r--r--   0        0        0     1987 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/client_logic.py
+-rw-r--r--   0        0        0      381 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/msg.py
+-rw-r--r--   0        0        0     5483 2023-06-17 11:11:34.557702 daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/server_logic.py
+-rw-r--r--   0        0        0      961 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
+-rw-r--r--   0        0        0     5848 2023-06-17 11:17:34.761761 daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
+-rw-r--r--   0        0        0    12137 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/client_logic.py
+-rw-r--r--   0        0        0     1755 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/common.py
+-rw-r--r--   0        0        0    10070 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/primitives.py
+-rw-r--r--   0        0        0    22268 2023-06-19 13:47:16.702565 daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/server_logic.py
+-rw-r--r--   0        0        0     1456 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/__init__.py
+-rw-r--r--   0        0        0     3016 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/aggregate.py
+-rw-r--r--   0        0        0     4538 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     5095 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     6134 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6993 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7245 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedadam.py
+-rw-r--r--   0        0        0    13054 2023-06-19 06:30:37.042075 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedasync.py
+-rw-r--r--   0        0        0    12396 2023-06-19 06:31:01.209923 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavg.py
+-rw-r--r--   0        0        0    10915 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     9115 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavgm.py
+-rw-r--r--   0        0        0     5513 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedopt.py
+-rw-r--r--   0        0        0     7263 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedyogi.py
+-rw-r--r--   0        0        0    10952 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7867 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/strategy.py
+-rw-r--r--   0        0        0      826 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/utils/__init__.py
+-rw-r--r--   0        0        0     6979 2023-06-19 13:28:40.804096 daisyfl-0.4.5/src/py/daisyfl/operator/utils/op_tools.py
+-rw-r--r--   0        0        0      676 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/proto/__init__.py
+-rw-r--r--   0        0        0    70900 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2.py
+-rw-r--r--   0        0        0    25816 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2631 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      781 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1064 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/__init__.py
+-rw-r--r--   0        0        0     5085 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/app.py
+-rw-r--r--   0        0        0     7809 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/client_manager.py
+-rw-r--r--   0        0        0     2371 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/client_proxy.py
+-rw-r--r--   0        0        0      714 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/__init__.py
+-rw-r--r--   0        0        0    12768 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
+-rw-r--r--   0        0        0     6827 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_bridge.py
+-rw-r--r--   0        0        0     4459 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11290 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0     3626 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/history.py
+-rw-r--r--   0        0        0    11835 2023-06-16 07:31:46.690912 daisyfl-0.4.5/src/py/daisyfl/server/server.py
+-rw-r--r--   0        0        0     6432 2023-06-19 12:57:16.218211 daisyfl-0.4.5/src/py/daisyfl/server/server_api_handler.py
+-rw-r--r--   0        0        0     4560 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/server_operator_manager.py
+-rw-r--r--   0        0        0    13571 2023-06-19 13:21:30.207305 daisyfl-0.4.5/src/py/daisyfl/server/task_manager.py
+-rw-r--r--   0        0        0     1273 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/simulation/__init__.py
+-rw-r--r--   0        0        0     7335 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     4661 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0      859 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/utils/dynamic_loader.py
+-rw-r--r--   0        0        0     2765 2023-06-21 00:25:31.476601 daisyfl-0.4.5/setup.py
+-rw-r--r--   0        0        0     3286 2023-06-21 00:25:31.476952 daisyfl-0.4.5/PKG-INFO
```

### Comparing `daisyfl-0.1.3/LICENSE` & `daisyfl-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/pyproject.toml` & `daisyfl-0.4.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "daisyfl"
-version = "0.1.3"
+version = "0.4.5"
 description = "Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing"
 license = "Apache-2.0"
 authors = ["tcfwbper <b05208031@ntu.edu.tw>"]
 readme = "README.md"
 homepage = "https://github.com/Intelligent-Systems-Lab/daisy"
 repository = "https://github.com/Intelligent-Systems-Lab/daisy"
 documentation = "https://github.com/Intelligent-Systems-Lab/daisy/tree/main/doc/daisy"
@@ -50,14 +50,17 @@
 grpcio = "^1.43.0"
 protobuf = "^3.19.0"
 importlib-metadata = { version = "^4.0.0", markers = "python_version < '3.8'" }
 iterators = "^0.0.2"
 dataclasses-json = "^0.5.7"
 # Optional dependencies
 ray = { extras = ["default"], version = "~2.0.0", optional = true }
+Flask = "^2.2.2"
+pycryptodome = "^3.16.0"
+cryptography = "^38.0.4"
 
 [tool.poetry.extras]
 simulation = ["ray"]
 
 [tool.poetry.dev-dependencies]
 types-protobuf = "==3.19.18"
 types-setuptools = "==57.4.14"
@@ -88,43 +91,38 @@
 [tool.isort]
 line_length = 88
 indent = "    "
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
-known_first_party = ["daisyfl", "flwr_experimental", "flwr_tool"]
+known_first_party = ["daisyfl", "daisy_tools"]
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310"]
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = "bad-continuation,duplicate-code,too-few-public-methods,useless-import-alias"
 
 [tool.pytest.ini_options]
 minversion = "6.2"
 addopts = "-qq"
 testpaths = [
     "src/py/daisyfl",
-    "src/py/flwr_tool",
+    "src/py/daisy_tools",
 ]
 
 [tool.mypy]
 plugins = [
     "numpy.typing.mypy_plugin",
 ]
 ignore_missing_imports = true
 strict = true
 
-[[tool.mypy.overrides]]
-module = [
-    "flwr_example.*",
-    "flwr_experimental.*",
-]
 ignore_errors = true
 
 [[tool.mypy.overrides]]
 module = [
     "importlib.metadata.*",
     "importlib_metadata.*",
 ]
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/__init__.py` & `daisyfl-0.4.5/src/py/daisyfl/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower main package."""
 
 import sys
 
-from . import client, server, simulation, plugin
+from . import client, server, simulation
 
 __all__ = [
-    "plugin",
     "client",
     "server",
     "simulation",
 ]
 
 # pylint: disable=import-error, no-name-in-module
 if sys.version_info < (3, 8):
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/client/__init__.py` & `daisyfl-0.4.5/src/py/daisyfl/client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,25 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower client."""
 
 
 from .app import ClientLike as ClientLike
-from .app import run_client as run_client
 from .app import start_client as start_client
 from .app import start_numpy_client as start_numpy_client
 from .app import to_client as to_client
 from .client import Client as Client
 from .numpy_client import NumPyClient as NumPyClient
 from .zone_client import ZoneClient as ZoneClient
 
 __all__ = [
     "Client",
     "ClientLike",
     "NumPyClient",
     "ZoneClient"
-    "run_client",
     "start_client",
     "start_numpy_client",
     "to_client",
 ]
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/client/app.py` & `daisyfl-0.4.5/src/py/daisyfl/client/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,29 +11,36 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower client app."""
 
 
-import time
-from logging import INFO
-from typing import Callable, Dict, Optional, Union
+from queue import Queue
+from logging import INFO, ERROR, WARNING
+from typing import Callable, Dict, Optional, Union, Tuple, List
+import threading
+import uuid
 
 from daisyfl.common import (
     GRPC_MAX_MESSAGE_LENGTH,
     CURRENT_ROUND,
     FIT_SAMPLES,
     EVALUATE_SAMPLES,
     LOSS,
     METRICS,
+    CLIENT_OPERATOR,
+    ZONE_CLIENT_OPERATOR,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
-    ###
-    USER_DEFINED_PLUGIN,
+    IS_ZONE,
+    CREDENTIAL,
+    metadata_to_dict,
+    dict_to_metadata,
+    CID,
 )
 from daisyfl.common.logger import log
 from daisyfl.common.typing import (
     Code,
     EvaluateIns,
     EvaluateRes,
     FitIns,
@@ -44,16 +51,19 @@
     GetPropertiesRes,
     NDArrays,
     Status,
     Report,
 )
 
 from .client import Client
-from .grpc_client.connection import grpc_connection
-from .grpc_client.message_handler import handle
+from .client_api_handler import ClientListener
+from .trainer import Trainer
+from .grpc_client.connection import gRPCConnection
+from .grpc_client.message_handler import set_client_operator_manager
+from daisyfl.client.client_operator_manager import ClientOperatorManager
 from .numpy_client import NumPyClient
 from .numpy_client import has_evaluate as numpyclient_has_evaluate
 from .numpy_client import has_fit as numpyclient_has_fit
 from .numpy_client import has_get_parameters as numpyclient_has_get_parameters
 from .numpy_client import has_get_properties as numpyclient_has_get_properties
 
 EXCEPTION_MESSAGE_WRONG_RETURN_TYPE_FIT = """
@@ -88,152 +98,109 @@
 
 def start_client(
     *,
     parent_address: str,
     client: Client,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[bytes] = None,
-    config: Dict = {},
+    api_ip: str = None,
+    api_port: int = None,
+    metadata: Tuple = None,
+    _zone: bool = False,
 ) -> None:
-    """Start a Flower Client which connects to a gRPC server.
+    # client_operator_manager
+    client_operator_manager = ClientOperatorManager(client=client)
+    operator_key = ZONE_CLIENT_OPERATOR if _zone else CLIENT_OPERATOR
+    client_operator_manager.set_operator_key(key=operator_key)
+    set_client_operator_manager(client_operator_manager)
+
+    # check metadata
+    if metadata is None:
+        metadata = ()
+    ## zone: process metadata
+    if _zone:
+        metadata_dict = metadata_to_dict(metadata=metadata, _check_required=False)
+        metadata_dict[IS_ZONE] = "is_zone"
+        if metadata_dict.__contains__(CREDENTIAL):
+            log(WARNING, "CREDENTIAL is defined in the metadata of a zone. It will be ignored.")
+            del metadata_dict[CREDENTIAL]
+        if not metadata_dict.__contains__(CID):
+            metadata_dict[CID] = str(uuid.uuid4())
+        metadata = dict_to_metadata(metadata_dict)
+    ## client: check metadata
+    else:
+        metadata_dict = metadata_to_dict(metadata=metadata)
+        metadata = dict_to_metadata(metadata_dict)
+
+    # declare instances: Trainer, gRPCConnection, ClientListener
+    trainer = Trainer()
+    connector = gRPCConnection(
+        parent_address=parent_address,
+        max_message_length=grpc_max_message_length,
+        root_certificates=root_certificates,
+        metadata=metadata,
+        trainer=trainer,
+    )
+    listener = ClientListener(
+        ip=api_ip,
+        port=api_port,
+        connector=connector,
+        trainer=trainer,
+    )
+    trainer.set_connector(connector=connector)
 
-    Parameters
-    ----------
-        parent_address: str. The IPv6 address of the server. If the Flower
-            server runs on the same machine on port 8080, then `parent_address`
-            would be `"[::]:8080"`.
-        client: flwr.client.Client. An implementation of the abstract base
-            class `flwr.client.Client`.
-        grpc_max_message_length: int (default: 536_870_912, this equals 512MB).
-            The maximum length of gRPC messages that can be exchanged with the
-            Flower server. The default should be sufficient for most models.
-            Users who train very large models might need to increase this
-            value. Note that the Flower server needs to be started with the
-            same value (see `flwr.server.start_server`), otherwise it will not
-            know about the increased limit and block larger messages.
-        root_certificates: bytes (default: None)
-            The PEM-encoded root certificates as a byte string. If provided, a secure
-            connection using the certificates will be established to a
-            SSL-enabled Flower server.
-
-    Returns
-    -------
-        None
-
-    Examples
-    --------
-    Starting a client with insecure server connection:
-
-    >>> start_client(
-    >>>     parent_address=localhost:8080,
-    >>>     client=FlowerClient(),
-    >>> )
-
-    Starting a SSL-enabled client:
-
-    >>> from pathlib import Path
-    >>> start_client(
-    >>>     parent_address=localhost:8080,
-    >>>     client=FlowerClient(),
-    >>>     root_certificates=Path("/crts/root.pem").read_bytes(),
-    >>> )
-    """
-    # wrap client according to plugin configuration
-    if config.__contains__(USER_DEFINED_PLUGIN):
-        client = config[USER_DEFINED_PLUGIN](client)
-
-    while True:
-        sleep_duration: int = 0
-        with grpc_connection(
-            parent_address,
-            max_message_length=grpc_max_message_length,
-            root_certificates=root_certificates,
-        ) as conn:
-            receive, send = conn
-
-            while True:
-                server_message = receive()
-                client_message, sleep_duration, keep_going = handle(
-                    client, server_message
-                )
-                send(client_message)
-                if not keep_going:
-                    break
-        if sleep_duration == 0:
-            log(INFO, "Disconnect and shut down")
-            break
-        # Sleep and reconnect afterwards
-        log(
-            INFO,
-            "Disconnect, then re-establish connection after %s second(s)",
-            sleep_duration,
-        )
-        time.sleep(sleep_duration)
+    # start threads: ClientListener, gRPCConnection, Trainer
+    
+    ## ClientListener
+    listener_thread = threading.Thread(target=listener.run, args=())
+    listener_thread.setDaemon(True)
+    listener_thread.start()
+    ## gRPCConnection
+    connector_thread = threading.Thread(target=connector.run, args=())
+    connector_thread.setDaemon(True)
+    connector_thread.start()
+    ### check
+    threading.Event().wait(timeout=1)
+    if not listener_thread.is_alive():
+        log(ERROR, "ClientListener failed")
+        exit(1)
+    if not connector_thread.is_alive():
+        log(ERROR, "gRPCConnection failed")
+        exit(1)
+    ## Trainer
+    trainer.run()
 
 
 def start_numpy_client(
     *,
     parent_address: str,
     client: NumPyClient,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[bytes] = None,
-    config: Dict = {},
+    api_ip: str = None,
+    api_port: int = None,
+    metadata: Tuple = None,
+    _zone: bool = False
 ) -> None:
-    """Start a Flower NumPyClient which connects to a gRPC server.
-
-    Parameters
-    ----------
-    parent_address : str
-        The IPv6 address of the server. If the Flower server runs on the same
-        machine on port 8080, then `parent_address` would be `"[::]:8080"`.
-    client : flwr.client.NumPyClient
-        An implementation of the abstract base class `flwr.client.NumPyClient`.
-    grpc_max_message_length : int (default: 536_870_912, this equals 512MB)
-        The maximum length of gRPC messages that can be exchanged with the
-        Flower server. The default should be sufficient for most models.
-        Users who train very large models might need to increase this
-        value. Note that the Flower server needs to be started with the
-        same value (see `flwr.server.start_server`), otherwise it will not
-        know about the increased limit and block larger messages.
-    root_certificates : bytes (default: None)
-        The PEM-encoded root certificates a byte string. If provided, a secure
-        connection using the certificates will be established to a
-        SSL-enabled Flower server.
-
-    Examples
-    --------
-    Starting a client with an insecure server connection:
-
-    >>> start_client(
-    >>>     parent_address=localhost:8080,
-    >>>     client=FlowerClient(),
-    >>> )
-
-    Starting a SSL-enabled client:
-
-    >>> from pathlib import Path
-    >>> start_client(
-    >>>     parent_address=localhost:8080,
-    >>>     client=FlowerClient(),
-    >>>     root_certificates=Path("/crts/root.pem").read_bytes(),
-    >>> )
-    """
-
     # Start
     start_client(
         parent_address=parent_address,
         client=_wrap_numpy_client(client=client),
         grpc_max_message_length=grpc_max_message_length,
         root_certificates=root_certificates,
-        config=config,
+        api_ip=api_ip,
+        api_port=api_port,
+        metadata=metadata,
+        _zone=_zone,
     )
-    if hasattr(client, "stop_zone_server"):
-        client.stop_zone_server()
+    if _zone:
+        client.shutdown()
 
 
+# wrap numpy_client to client
 def to_client(client_like: ClientLike) -> Client:
     """Take any Client-like object and return it as a Client."""
     if isinstance(client_like, NumPyClient):
         return _wrap_numpy_client(client=client_like)
     return client_like
 
 
@@ -271,21 +238,22 @@
         len(results) == 3
         and isinstance(results[0], list)
         and isinstance(results[1], int)
         and isinstance(results[2], dict)
     ):
         raise Exception(EXCEPTION_MESSAGE_WRONG_RETURN_TYPE_FIT)
     # results -> Report.config
-    parameters_prime, num_examples, metrics = results
+    parameters_prime, num_examples, config = results
     parameters_prime_proto = ndarrays_to_parameters(parameters_prime)
-    config = {
-        CURRENT_ROUND: ins.config[CURRENT_ROUND],
-        FIT_SAMPLES: num_examples,
-        METRICS: metrics,
-    }
+    if not config.__contains__(CURRENT_ROUND):
+        config[CURRENT_ROUND] = ins.config[CURRENT_ROUND]
+    if not config.__contains__(FIT_SAMPLES):
+        config[FIT_SAMPLES] = num_examples
+    if not config.__contains__(METRICS):
+        config[METRICS] = {}
    
     # Return FitRes
     return FitRes(
         status=Status(code=Code.OK, message="Success"),
         parameters=parameters_prime_proto,
         config=config,
     )
@@ -301,21 +269,23 @@
         and isinstance(results[0], float)
         and isinstance(results[1], int)
         and isinstance(results[2], dict)
     ):
         raise Exception(EXCEPTION_MESSAGE_WRONG_RETURN_TYPE_EVALUATE)
 
     # results -> Report.config
-    loss, num_examples, metrics = results
-    config = {
-        CURRENT_ROUND: ins.config[CURRENT_ROUND],
-        EVALUATE_SAMPLES: num_examples,
-        LOSS: loss,
-        METRICS: metrics,
-    }
+    loss, num_examples, config = results
+    if not config.__contains__(CURRENT_ROUND):
+        config[CURRENT_ROUND] = ins.config[CURRENT_ROUND]
+    if not config.__contains__(LOSS):
+        config[LOSS] = loss
+    if not config.__contains__(EVALUATE_SAMPLES):
+        config[EVALUATE_SAMPLES] = num_examples
+    if not config.__contains__(METRICS):
+        config[METRICS] = {}
     
     # Return EvaluateRes
     return EvaluateRes(
         status=Status(code=Code.OK, message="Success"),
         config=config,
     )
 
@@ -340,13 +310,7 @@
         member_dict["evaluate"] = _evaluate
 
     # Create wrapper class
     wrapper_class = type("NumPyClientWrapper", (Client,), member_dict)
 
     # Create and return an instance of the newly created class
     return wrapper_class(numpy_client=client)  # type: ignore
-
-
-def run_client() -> None:
-    """Run Flower client."""
-    log(INFO, "Running Flower client...")
-    time.sleep(3)
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/client/client.py` & `daisyfl-0.4.5/src/py/daisyfl/client/client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/src/py/daisyfl/client/dpfedavg_numpy_client.py` & `daisyfl-0.4.5/src/py/daisyfl/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/src/py/daisyfl/client/grpc_client/__init__.py` & `daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/src/py/daisyfl/client/grpc_client/message_handler.py` & `daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/message_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,28 +20,31 @@
 from daisyfl.client.client import (
     Client,
     has_evaluate,
     has_fit,
     has_get_parameters,
     has_get_properties,
 )
+from daisyfl.client.client_operator_manager import ClientOperatorManager
 from daisyfl.common import serde, typing
 from daisyfl.common.typing import Parameters
 from daisyfl.proto.transport_pb2 import ClientMessage, Reason, ServerMessage
 
 # pylint: disable=missing-function-docstring
 
 
 class UnknownServerMessage(Exception):
     """Signifies that the received message is unknown."""
 
 
+_client_operator_manager: ClientOperatorManager = None
+
 def handle(
-    client: Client, server_msg: ServerMessage
-) -> Tuple[ClientMessage, int, bool]:
+    server_msg: ServerMessage
+) -> ClientMessage:
     """Handle incoming messages from the server.
 
     Parameters
     ----------
     client : Client
         The Client instance provided by the user.
 
@@ -54,44 +57,50 @@
     keep_going : bool
         Flag that indicates whether the client should continue to process the
         next message from the server (True) or disconnect and optionally
         reconnect later (False).
     """
     field = server_msg.WhichOneof("msg")
     if field == "reconnect_ins":
-        disconnect_msg, sleep_duration = _reconnect(server_msg.reconnect_ins)
-        return disconnect_msg, sleep_duration, False
+        return _reconnect(server_msg.reconnect_ins)
     if field == "get_properties_ins":
-        return _get_properties(client, server_msg.get_properties_ins), 0, True
+        return _get_properties(server_msg.get_properties_ins)
     if field == "get_parameters_ins":
-        return _get_parameters(client, server_msg.get_parameters_ins), 0, True
+        return _get_parameters(server_msg.get_parameters_ins)
     if field == "fit_ins":
-        return _fit(client, server_msg.fit_ins), 0, True
+        return _fit(server_msg.fit_ins)
     if field == "evaluate_ins":
-        return _evaluate(client, server_msg.evaluate_ins), 0, True
+        return _evaluate(server_msg.evaluate_ins)
     raise UnknownServerMessage()
 
 
 def _reconnect(
     reconnect_msg: ServerMessage.ReconnectIns,
 ) -> Tuple[ClientMessage, int]:
+    # TODO:
     # Determine the reason for sending DisconnectRes message
     reason = Reason.ACK
     sleep_duration = None
     if reconnect_msg.seconds is not None:
         reason = Reason.RECONNECT
         sleep_duration = reconnect_msg.seconds
     # Build DisconnectRes message
     disconnect_res = ClientMessage.DisconnectRes(reason=reason)
-    return ClientMessage(disconnect_res=disconnect_res), sleep_duration
+
+    client_operator_manager = get_client_operator_manager()
+    client_operator_manager.disconnect()
+    # TODO: reconnect request
+    return ClientMessage(disconnect_res=disconnect_res)
 
 
 def _get_properties(
-    client: Client, get_properties_msg: ServerMessage.GetPropertiesIns
+    get_properties_msg: ServerMessage.GetPropertiesIns
 ) -> ClientMessage:
+    client = get_client_operator_manager().get_client()
+
     # Check if client overrides get_properties
     if not has_get_properties(client=client):
         # If client does not override get_properties, don't call it
         get_properties_res = typing.GetPropertiesRes(
             status=typing.Status(
                 code=typing.Code.GET_PROPERTIES_NOT_IMPLEMENTED,
                 message="Client does not implement `get_properties`",
@@ -107,16 +116,18 @@
     get_properties_res = client.get_properties(get_properties_ins)
     # Serialize response
     get_properties_res_proto = serde.get_properties_res_to_proto(get_properties_res)
     return ClientMessage(get_properties_res=get_properties_res_proto)
 
 
 def _get_parameters(
-    client: Client, get_parameters_msg: ServerMessage.GetParametersIns
+    get_parameters_msg: ServerMessage.GetParametersIns
 ) -> ClientMessage:
+    client = get_client_operator_manager().get_client()
+
     # Check if client overrides get_parameters
     if not has_get_parameters(client=client):
         # If client does not override get_parameters, don't call it
         get_parameters_res = typing.GetParametersRes(
             status=typing.Status(
                 code=typing.Code.GET_PARAMETERS_NOT_IMPLEMENTED,
                 message="Client does not implement `get_parameters`",
@@ -131,55 +142,39 @@
     # Request parameters
     get_parameters_res = client.get_parameters(get_parameters_ins)
     # Serialize response
     get_parameters_res_proto = serde.get_parameters_res_to_proto(get_parameters_res)
     return ClientMessage(get_parameters_res=get_parameters_res_proto)
 
 
-def _fit(client: Client, fit_msg: ServerMessage.FitIns) -> ClientMessage:
-    # Check if client overrides fit
-    if not has_fit(client=client):
-        # If client does not override fit, don't call it
-        fit_res = typing.FitRes(
-            status=typing.Status(
-                code=typing.Code.FIT_NOT_IMPLEMENTED,
-                message="Client does not implement `fit`",
-            ),
-            parameters=Parameters(tensor_type="", tensors=[]),
-            num_examples=0,
-            metrics={},
-        )
-        fit_res_proto = serde.fit_res_to_proto(fit_res)
-        return ClientMessage(fit_res=fit_res_proto)
+def _fit(fit_msg: ServerMessage.FitIns) -> ClientMessage:
+    client_operator_manager = get_client_operator_manager()
 
     # Deserialize fit instruction
     fit_ins = serde.fit_ins_from_proto(fit_msg)
     # Perform fit
-    fit_res = client.fit(fit_ins)
+    fit_res = client_operator_manager.fit(fit_ins)
     # Serialize fit result
     fit_res_proto = serde.fit_res_to_proto(fit_res)
     return ClientMessage(fit_res=fit_res_proto)
 
 
-def _evaluate(client: Client, evaluate_msg: ServerMessage.EvaluateIns) -> ClientMessage:
-    # Check if client overrides evaluate
-    if not has_evaluate(client=client):
-        # If client does not override evaluate, don't call it
-        evaluate_res = typing.EvaluateRes(
-            status=typing.Status(
-                code=typing.Code.EVALUATE_NOT_IMPLEMENTED,
-                message="Client does not implement `evaluate`",
-            ),
-            loss=0.0,
-            num_examples=0,
-            metrics={},
-        )
-        evaluate_res_proto = serde.evaluate_res_to_proto(evaluate_res)
-        return ClientMessage(evaluate_res=evaluate_res_proto)
-
+def _evaluate(evaluate_msg: ServerMessage.EvaluateIns) -> ClientMessage:
+    client_operator_manager = get_client_operator_manager()
+    
     # Deserialize evaluate instruction
     evaluate_ins = serde.evaluate_ins_from_proto(evaluate_msg)
     # Perform evaluation
-    evaluate_res = client.evaluate(evaluate_ins)
+    evaluate_res = client_operator_manager.evaluate(evaluate_ins)
     # Serialize evaluate result
     evaluate_res_proto = serde.evaluate_res_to_proto(evaluate_res)
     return ClientMessage(evaluate_res=evaluate_res_proto)
+
+
+# client_operator_manager
+def set_client_operator_manager(client_operator_manager: ClientOperatorManager):
+    global _client_operator_manager
+    _client_operator_manager = client_operator_manager
+
+def get_client_operator_manager() -> ClientOperatorManager:
+    global _client_operator_manager
+    return _client_operator_manager
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/client/numpy_client.py` & `daisyfl-0.4.5/src/py/daisyfl/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/src/py/daisyfl/common/dp.py` & `daisyfl-0.4.5/src/py/daisyfl/common/dp.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/src/py/daisyfl/common/logger.py` & `daisyfl-0.4.5/src/py/daisyfl/common/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Flower Logger."""
 import logging
 from logging import LogRecord
 from logging.handlers import HTTPHandler
 from typing import Any, Dict, Optional, Tuple
 
 # Create logger
-LOGGER_NAME = "flower"
+LOGGER_NAME = "daisy"
 FLOWER_LOGGER = logging.getLogger(LOGGER_NAME)
 FLOWER_LOGGER.setLevel(logging.DEBUG)
 
 DEFAULT_FORMATTER = logging.Formatter(
     "%(levelname)s %(name)s %(asctime)s | %(filename)s:%(lineno)d | %(message)s"
 )
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/common/parameter.py` & `daisyfl-0.4.5/src/py/daisyfl/common/parameter.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/src/py/daisyfl/common/serde.py` & `daisyfl-0.4.5/src/py/daisyfl/common/serde.py`

 * *Files 8% similar despite different names*

```diff
@@ -218,28 +218,32 @@
         code = Code.GET_PROPERTIES_NOT_IMPLEMENTED
     if status.code == typing.Code.GET_PARAMETERS_NOT_IMPLEMENTED:
         code = Code.GET_PARAMETERS_NOT_IMPLEMENTED
     if status.code == typing.Code.FIT_NOT_IMPLEMENTED:
         code = Code.FIT_NOT_IMPLEMENTED
     if status.code == typing.Code.EVALUATE_NOT_IMPLEMENTED:
         code = Code.EVALUATE_NOT_IMPLEMENTED
+    if status.code == typing.Code.MESSAGE_LOST:
+        code = Code.MESSAGE_LOST
     return Status(code=code, message=status.message)
 
 
 def status_from_proto(msg: Status) -> typing.Status:
     """Deserialize Code from ProtoBuf message."""
     code = typing.Code.OK
     if msg.code == Code.GET_PROPERTIES_NOT_IMPLEMENTED:
         code = typing.Code.GET_PROPERTIES_NOT_IMPLEMENTED
     if msg.code == Code.GET_PARAMETERS_NOT_IMPLEMENTED:
         code = typing.Code.GET_PARAMETERS_NOT_IMPLEMENTED
     if msg.code == Code.FIT_NOT_IMPLEMENTED:
         code = typing.Code.FIT_NOT_IMPLEMENTED
     if msg.code == Code.EVALUATE_NOT_IMPLEMENTED:
         code = typing.Code.EVALUATE_NOT_IMPLEMENTED
+    if msg.code == Code.MESSAGE_LOST:
+        code = typing.Code.MESSAGE_LOST
     return typing.Status(code=code, message=msg.message)
 
 
 # === Evaluate messages ===
 
 
 def evaluate_ins_to_proto(ins: typing.EvaluateIns) -> ServerMessage.EvaluateIns:
@@ -274,14 +278,54 @@
     config = None if msg.config is None else inner_map_from_proto(msg.config)
     return typing.EvaluateRes(
         status=status,
         config=config,
     )
 
 
+#  === ClientStatus ===
+
+
+def client_status_to_proto(res: typing.ClientStatus) -> ClientMessage.ClientStatus:
+    """Serialize ClientStatus to ProtoBuf message."""
+    return ClientMessage.ClientStatus(status=res.status)
+
+
+def client_status_from_proto(msg: ClientMessage.ClientStatus) -> typing.ClientStatus:
+    """Deserialize ProtoBuf message to ClientStatus."""
+    return typing.ClientStatus(status=msg.status)
+
+
+# === SRS, CRS ===
+
+
+def server_received_signal_to_proto(ins: typing.ServerReceivedSignal) -> ServerMessage.ServerReceivedSignal:
+    """Serialize SRS to ProtoBuf message."""
+    status_proto = status_to_proto(ins.status)
+    return ServerMessage.ServerReceivedSignal(status=status_proto)
+
+
+def server_received_signal_from_proto(msg: ServerMessage.ServerReceivedSignal) -> typing.ServerReceivedSignal:
+    """Deserialize ProtoBug message to SRS"""
+    status = status_from_proto(msg.status)
+    return typing.ServerReceivedSignal(status=status)
+
+
+def client_received_signal_to_proto(res: typing.ClientReceivedSignal) -> ClientMessage.ClientReceivedSignal:
+    """Serialize CRS to ProtoBuf message."""
+    status_proto = status_to_proto(res.status)
+    return ClientMessage.ClientReceivedSignal(status=status_proto)
+
+
+def client_received_signal_from_proto(msg: ClientMessage.ClientReceivedSignal) -> typing.ClientReceivedSignal:
+    """Deserialize ProtoBug message to CRS"""
+    status = status_from_proto(msg.status)
+    return typing.ClientReceivedSignal(status=status)
+
+
 # === Properties messages ===
 
 
 def properties_to_proto(properties: typing.Properties) -> Any:
     """Serialize... ."""
     proto = {}
     for key in properties:
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/common/typing.py` & `daisyfl-0.4.5/src/py/daisyfl/common/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Flower type definitions."""
 
 
 from dataclasses import dataclass
 from dataclasses_json import dataclass_json
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union, TypedDict
-
+from threading import Condition
 import numpy.typing as npt
 
 NDArray = npt.NDArray[Any]
 NDArrays = List[NDArray]
 
 # The following union type contains Python types corresponding to ProtoBuf types that
 # ProtoBuf considers to be "Scalar Value Types", even though some of them arguably do
@@ -44,14 +44,15 @@
     """Client status codes."""
 
     OK = 0
     GET_PROPERTIES_NOT_IMPLEMENTED = 1
     GET_PARAMETERS_NOT_IMPLEMENTED = 2
     FIT_NOT_IMPLEMENTED = 3
     EVALUATE_NOT_IMPLEMENTED = 4
+    MESSAGE_LOST = 5
 
 
 @dataclass
 class Status:
     """Client status."""
 
     code: Code
@@ -141,28 +142,20 @@
 
     reason: str
 
 @dataclass
 class Task:
     """Input a task when calling server API."""
     config: TypedDict
+    # TID: str
     # NUM_ROUNDS: int
     # CURRENT_ROUND: int
     # EVALUATE: bool
     # TIMEOUT: int
 
-@dataclass
-class MetaTask:
-    """Input a task when calling server API."""
-    tid: int
-    start_time: float
-    task: Task
-    parameters: Parameters
-    configured_tasks: List[Task]
-    # on_configure_task_fn: Callable
 
 @dataclass
 class Report:
     """After complete a task, return a report."""
     config: TypedDict
     # CURRENT_ROUND: int
     # FIT_SAMPLES: int
@@ -170,8 +163,38 @@
     # LOSS: float
     # METRICS: Metrics
 
 class Type(Enum):
     """Type of the task manager."""
     
     MASTER = 1
-    ZONE = 2
+    ZONE = 2
+
+
+class CheckResults(Enum):
+    OK = 0
+    FAIL = 1
+    CONTINUE = 2
+
+
+@dataclass
+class CurrentReturns:
+    selected: int
+    results_num: int
+    failures_num: int
+    cnd: Condition
+
+
+@dataclass
+class ClientStatus:
+    status: str
+
+
+@dataclass
+class ServerReceivedSignal:
+    status: Status
+
+
+@dataclass
+class ClientReceivedSignal:
+    status: Status
+
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/__init__.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 from .fedadam import FedAdam as FedAdam
 from .fedavg import FedAvg as FedAvg
 from .fedavg_android import FedAvgAndroid as FedAvgAndroid
 from .fedavgm import FedAvgM as FedAvgM
 from .fedopt import FedOpt as FedOpt
 from .fedyogi import FedYogi as FedYogi
 from .qfedavg import QFedAvg as QFedAvg
+from .fedasync import FedAsync as FedAsync
 from .strategy import Strategy as Strategy
 
 __all__ = [
     "FaultTolerantFedAvg",
     "FedAdagrad",
     "FedAdam",
     "FedAvg",
     "FedAvgAndroid",
     "FedAvgM",
     "FedOpt",
     "FedYogi",
     "QFedAvg",
+    "FedAsync",
     "Strategy",
 ]
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/aggregate.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/aggregate.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Aggregation functions for strategy implementations."""
 
 
 from functools import reduce
-from typing import List, Tuple
+from typing import List, Tuple, Callable
 
 import numpy as np
 
 from daisyfl.common import NDArrays
 
 
 def aggregate(results: List[Tuple[NDArrays, int]]) -> NDArrays:
@@ -60,7 +60,20 @@
     for i in range(len(deltas[0])):
         tmp = scaled_deltas[0][i]
         for j in range(1, len(deltas)):
             tmp += scaled_deltas[j][i]
         updates.append(tmp)
     new_parameters = [(u - v) * 1.0 for u, v in zip(parameters, updates)]
     return new_parameters
+
+def aggregate_fedasync(
+    global_model: NDArrays,
+    local_model: NDArrays,
+    alpha: float,
+) -> NDArrays:
+    weighted_global_model = [layer * (1 - alpha) for layer in global_model]
+    weighted_local_model = [layer * alpha for layer in local_model]
+    nd_arrays_list = [weighted_global_model, weighted_local_model]
+    new_global_model: NDArrays = [
+        reduce(np.add, layer_updates) for layer_updates in zip(*nd_arrays_list)
+    ]
+    return new_global_model
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/dpfedavg_adaptive.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 from daisyfl.common import FitIns, FitRes, Parameters, Scalar
 from daisyfl.server.client_manager import ClientManager
 from daisyfl.server.client_proxy import ClientProxy
-from daisyfl.server.strategy.dpfedavg_fixed import DPFedAvgFixed
-from daisyfl.operation.strategy.strategy import Strategy
+from daisyfl.operator.strategy.dpfedavg_fixed import DPFedAvgFixed
+from daisyfl.operator.strategy.strategy import Strategy
 
 
 class DPFedAvgAdaptive(DPFedAvgFixed):
     """Wrapper for configuring a Strategy for DP with Adaptive Clipping."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/dpfedavg_fixed.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 """DP-FedAvg [McMahan et al., 2018] strategy.
 
 Paper: https://arxiv.org/pdf/1710.06963.pdf
 """
 
 from typing import Dict, List, Optional, Tuple, Union
 
-from daisyfl.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar
+from daisyfl.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar, CURRENT_ROUND, CurrentReturns, CheckResults
 from daisyfl.common.dp import add_gaussian_noise
 from daisyfl.common.parameter import ndarrays_to_parameters, parameters_to_ndarrays
-from daisyfl.server.client_manager import ClientManager
+from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
-from daisyfl.operation.strategy.strategy import Strategy
+from daisyfl.operator.strategy.strategy import Strategy
 
 
 class DPFedAvgFixed(Strategy):
     """Wrapper for configuring a Strategy for DP with Fixed Clipping."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
@@ -60,43 +60,51 @@
 
     def _calc_client_noise_stddev(self) -> float:
         return float(
             self.noise_multiplier * self.clip_norm / (self.num_sampled_clients ** (0.5))
         )
 
     def initialize_parameters(
-        self, client_manager: ClientManager
+        self, server: Server
     ) -> Optional[Parameters]:
-        return self.strategy.initialize_parameters(client_manager)
+        return self.strategy.initialize_parameters(server)
 
     def configure_fit(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self,
+        server_round: int,
+        parameters: Parameters,
+        server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
 
         additional_config = {"dpfedavg_clip_norm": self.clip_norm}
         if not self.server_side_noising:
             additional_config[
                 "dpfedavg_noise_stddev"
             ] = self._calc_client_noise_stddev()
 
         client_instructions = self.strategy.configure_fit(
-            server_round, parameters, client_manager
+            server_round, parameters, server, credential,
         )
 
         for _, fit_ins in client_instructions:
             fit_ins.config.update(additional_config)
 
         return client_instructions
 
     def configure_evaluate(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self,
+        server_round: int,
+        parameters: Parameters,
+        server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         return self.strategy.configure_evaluate(
-            server_round, parameters, client_manager
+            server_round, parameters, server, credential,
         )
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
         failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
@@ -123,7 +131,12 @@
     ) -> Tuple[Optional[float], Dict[str, Scalar]]:
         return self.strategy.aggregate_evaluate(server_round, results, failures)
 
     def evaluate(
         self, server_round: int, parameters: Parameters
     ) -> Optional[Tuple[float, Dict[str, Scalar]]]:
         return self.strategy.evaluate(server_round, parameters)
+    
+    def check_results(
+        self, current_returns: CurrentReturns,
+    ) -> CheckResults:
+        return
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fault_tolerant_fedavg.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 1,
         min_evaluate_clients: int = 1,
         min_available_clients: int = 1,
+        min_result: int = 1,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -60,17 +62,19 @@
         initial_parameters: Optional[Parameters] = None,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
     ) -> None:
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=True,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedadagrad.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedadagrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -106,17 +108,19 @@
             eta_l (float, optional): Client-side learning rate. Defaults to 1e-1.
             tau (float, optional): Controls the algorithm's degree of adaptability.
                 Defaults to 1e-9.
         """
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedadam.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedadam.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,17 +46,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: float = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -109,17 +111,19 @@
             beta_2 (float, optional): Second moment parameter. Defaults to 0.99.
             tau (float, optional): Controls the algorithm's degree of adaptability.
                 Defaults to 1e-9.
         """
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedavg.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavg.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,31 +14,34 @@
 # ==============================================================================
 """Federated Averaging (FedAvg) [McMahan et al., 2016] strategy.
 
 Paper: https://arxiv.org/abs/1602.05629
 """
 
 
-from logging import WARNING
+from logging import WARNING, INFO
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 from daisyfl.common import (
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
+    CheckResults,
+    CurrentReturns,
+    ACCURACY,
 )
 from daisyfl.common.logger import log
-from daisyfl.server.client_manager import ClientManager
+from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate, weighted_loss_avg
 from .strategy import Strategy
 
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
@@ -53,17 +56,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 0.8,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -115,17 +120,19 @@
             min_fit_clients > min_available_clients
             or min_evaluate_clients > min_available_clients
         ):
             log(WARNING, WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW)
 
         self.fraction_fit = fraction_fit
         self.fraction_evaluate = fraction_evaluate
+        self.fraction_result = fraction_result
         self.min_fit_clients = min_fit_clients
         self.min_evaluate_clients = min_evaluate_clients
         self.min_available_clients = min_available_clients
+        self.min_result = min_result
         self.evaluate_fn = evaluate_fn
         self.on_fit_config_fn = on_fit_config_fn
         self.on_evaluate_config_fn = on_evaluate_config_fn
         self.accept_failures = accept_failures
         self.initial_parameters = initial_parameters
         self.fit_metrics_aggregation_fn = fit_metrics_aggregation_fn
         self.evaluate_metrics_aggregation_fn = evaluate_metrics_aggregation_fn
@@ -142,15 +149,15 @@
 
     def num_evaluation_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Use a fraction of available clients for evaluation."""
         num_clients = int(num_available_clients * self.fraction_evaluate)
         return max(num_clients, self.min_evaluate_clients), self.min_available_clients
 
     def initialize_parameters(
-        self, client_manager: ClientManager
+        self, server: Server
     ) -> Optional[Parameters]:
         """Initialize global model parameters."""
         initial_parameters = self.initial_parameters
         self.initial_parameters = None  # Don't keep initial parameters in memory
         return initial_parameters
 
     def evaluate(
@@ -164,36 +171,41 @@
         eval_res = self.evaluate_fn(server_round, parameters_ndarrays, {})
         if eval_res is None:
             return None
         loss, metrics = eval_res
         return loss, metrics
 
     def configure_fit(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self,
+        server_round: int,
+        parameters: Parameters,
+        server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
         config = {}
         if self.on_fit_config_fn is not None:
             # Custom fit config function provided
             config = self.on_fit_config_fn(server_round)
         fit_ins = FitIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_fit_clients(
-            client_manager.num_available()
-        )
-        clients = client_manager.sample(
-            num_clients=sample_size, min_num_clients=min_num_clients
+            server.num_available(credential=credential)
         )
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # Return client/config pairs
         return [(client, fit_ins) for client in clients]
 
     def configure_evaluate(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self, server_round: int,
+        parameters: Parameters,
+        server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation."""
         # Do not configure federated evaluation if fraction eval is 0.
         if self.fraction_evaluate == 0.0:
             return []
 
         # Parameters and config
@@ -201,19 +213,17 @@
         if self.on_evaluate_config_fn is not None:
             # Custom evaluation config function provided
             config = self.on_evaluate_config_fn(server_round)
         evaluate_ins = EvaluateIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_evaluation_clients(
-            client_manager.num_available()
-        )
-        clients = client_manager.sample(
-            num_clients=sample_size, min_num_clients=min_num_clients
+            server.num_available(credential=credential)
         )
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # Return client/config pairs
         return [(client, evaluate_ins) for client in clients]
 
     def aggregate_fit(
         self,
         server_round: int,
@@ -235,15 +245,15 @@
         parameters_aggregated = ndarrays_to_parameters(aggregate(weights_results))
 
         # Aggregate custom metrics if aggregation fn was provided
         metrics_aggregated = {}
         if self.fit_metrics_aggregation_fn:
             fit_metrics = [(res.num_examples, res.metrics) for _, res in results]
             metrics_aggregated = self.fit_metrics_aggregation_fn(fit_metrics)
-        elif server_round == 1:  # Only log this warning once
+        elif server_round == 0:  # Only log this warning once
             log(WARNING, "No fit_metrics_aggregation_fn provided")
 
         return parameters_aggregated, metrics_aggregated
 
     def aggregate_evaluate(
         self,
         server_round: int,
@@ -263,14 +273,31 @@
                 (evaluate_res.num_examples, evaluate_res.loss)
                 for _, evaluate_res in results
             ]
         )
 
         # Aggregate custom metrics if aggregation fn was provided
         metrics_aggregated = {}
+        eval_metrics = [(res.num_examples, res.metrics) for _, res in results]
         if self.evaluate_metrics_aggregation_fn:
-            eval_metrics = [(res.num_examples, res.metrics) for _, res in results]
             metrics_aggregated = self.evaluate_metrics_aggregation_fn(eval_metrics)
-        elif server_round == 1:  # Only log this warning once
-            log(WARNING, "No evaluate_metrics_aggregation_fn provided")
+        else:
+            log(INFO, "Using default evaluate_metrics_aggregation_fn")
+            # Multiply accuracy of each client by number of examples used
+            accuracies = [num_examples * m[ACCURACY] for num_examples, m in eval_metrics]
+            examples = [num_examples for num_examples, _ in eval_metrics]
+            metrics_aggregated = {ACCURACY: sum(accuracies) / sum(examples)}
 
         return loss_aggregated, metrics_aggregated
+
+    def check_results(
+        self, current_returns: CurrentReturns,
+    ) -> CheckResults:
+        if current_returns is None:
+            return CheckResults.FAIL
+        if ((self.fraction_result * current_returns.selected <= current_returns.results_num) and \
+            (self.min_result <= current_returns.results_num)):
+            return CheckResults.OK
+        if ((self.fraction_result * current_returns.selected) <= (current_returns.selected - current_returns.failures_num)) \
+            and (self.min_result <= (current_returns.selected - current_returns.failures_num)):
+            return CheckResults.CONTINUE
+        return CheckResults.FAIL
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedavg_android.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavg_android.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,18 @@
     EvaluateRes,
     FitIns,
     FitRes,
     NDArray,
     NDArrays,
     Parameters,
     Scalar,
+    CurrentReturns,
+    CheckResults,
 )
-from daisyfl.server.client_manager import ClientManager
+from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate, weighted_loss_avg
 from .strategy import Strategy
 
 
 class FedAvgAndroid(Strategy):
@@ -45,17 +47,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -95,16 +99,18 @@
             containing failures. Defaults to True.
         initial_parameters : Optional[Parameters]
             Initial global model parameters.
         """
         super().__init__()
         self.min_fit_clients = min_fit_clients
         self.min_evaluate_clients = min_evaluate_clients
+        self.min_result = min_result
         self.fraction_fit = fraction_fit
         self.fraction_evaluate = fraction_evaluate
+        self.fraction_result = fraction_result
         self.min_available_clients = min_available_clients
         self.evaluate_fn = evaluate_fn
         self.on_fit_config_fn = on_fit_config_fn
         self.on_evaluate_config_fn = on_evaluate_config_fn
         self.accept_failures = accept_failures
         self.initial_parameters = initial_parameters
 
@@ -120,15 +126,15 @@
 
     def num_evaluation_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Use a fraction of available clients for evaluation."""
         num_clients = int(num_available_clients * self.fraction_evaluate)
         return max(num_clients, self.min_evaluate_clients), self.min_available_clients
 
     def initialize_parameters(
-        self, client_manager: ClientManager
+        self, server: Server
     ) -> Optional[Parameters]:
         """Initialize global model parameters."""
         initial_parameters = self.initial_parameters
         self.initial_parameters = None  # Don't keep initial parameters in memory
         return initial_parameters
 
     def evaluate(
@@ -142,36 +148,42 @@
         eval_res = self.evaluate_fn(server_round, weights, {})
         if eval_res is None:
             return None
         loss, metrics = eval_res
         return loss, metrics
 
     def configure_fit(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self,
+        server_round: int,
+        parameters: Parameters,
+        server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
         config = {}
         if self.on_fit_config_fn is not None:
             # Custom fit config function provided
             config = self.on_fit_config_fn(server_round)
         fit_ins = FitIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_fit_clients(
-            client_manager.num_available()
-        )
-        clients = client_manager.sample(
-            num_clients=sample_size, min_num_clients=min_num_clients
+            server.num_available(credential=credential)
         )
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # Return client/config pairs
         return [(client, fit_ins) for client in clients]
 
     def configure_evaluate(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self,
+        server_round: int,
+        parameters: Parameters,
+        server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation."""
         # Do not configure federated evaluation if fraction_evaluate is 0
         if self.fraction_evaluate == 0.0:
             return []
 
         # Parameters and config
@@ -179,19 +191,17 @@
         if self.on_evaluate_config_fn is not None:
             # Custom evaluation config function provided
             config = self.on_evaluate_config_fn(server_round)
         evaluate_ins = EvaluateIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_evaluation_clients(
-            client_manager.num_available()
-        )
-        clients = client_manager.sample(
-            num_clients=sample_size, min_num_clients=min_num_clients
+            server.num_available(credential=credential)
         )
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # Return client/config pairs
         return [(client, evaluate_ins) for client in clients]
 
     def aggregate_fit(
         self,
         server_round: int,
@@ -246,7 +256,21 @@
         return ndarray.tobytes()
 
     # pylint: disable=R0201
     def bytes_to_ndarray(self, tensor: bytes) -> NDArray:
         """Deserialize NumPy array from bytes."""
         ndarray_deserialized = np.frombuffer(tensor, dtype=np.float32)  # type: ignore
         return cast(NDArray, ndarray_deserialized)
+
+    def check_results(
+        self, current_returns: CurrentReturns,
+    ) -> CheckResults:
+        if current_returns is None:
+            return CheckResults.FAIL
+        if ((self.fraction_result * current_returns.selected <= current_returns.results_num) and \
+            (self.min_result <= current_returns.results_num)):
+            return CheckResults.OK
+        if ((self.fraction_result * current_returns.selected) <= (current_returns.selected - current_returns.failures_num)) \
+            and (self.min_result <= (current_returns.selected - current_returns.failures_num)):
+            return CheckResults.CONTINUE
+        return CheckResults.FAIL
+
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedavgm.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavgm.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
 from daisyfl.common.logger import log
-from daisyfl.server.client_manager import ClientManager
+from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate
 from .fedavg import FedAvg
 
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
@@ -50,17 +50,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -115,17 +117,19 @@
             or min_evaluate_clients > min_available_clients
         ):
             log(WARNING, WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW)
 
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
@@ -140,15 +144,15 @@
         self.evaluate_metrics_aggregation_fn = evaluate_metrics_aggregation_fn
 
     def __repr__(self) -> str:
         rep = f"FedAvgM(accept_failures={self.accept_failures})"
         return rep
 
     def initialize_parameters(
-        self, client_manager: ClientManager
+        self, server: Server
     ) -> Optional[Parameters]:
         """Initialize global model parameters."""
         return self.initial_parameters
 
     def aggregate_fit(
         self,
         server_round: int,
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedopt.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedopt.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -101,17 +103,19 @@
         beta_2 (float, optional): Second moment parameter. Defaults to 0.0.
         tau (float, optional): Controls the algorithm's degree of adaptability.
             Defaults to 1e-9.
         """
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/fedyogi.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedyogi.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,17 +46,19 @@
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        min_result: int = 2,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -109,17 +111,19 @@
             beta_2 (float, optional): Second moment parameter. Defaults to 0.99.
             tau (float, optional): Controls the algorithm's degree of adaptability.
                 Defaults to 1e-9.
         """
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/qfedavg.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/qfedavg.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
 from daisyfl.common.logger import log
-from daisyfl.server.client_manager import ClientManager
+from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate_qffl, weighted_loss_avg
 from .fedavg import FedAvg
 
 
 # pylint: disable=too-many-locals
@@ -51,17 +51,19 @@
     def __init__(
         self,
         *,
         q_param: float = 0.2,
         qffl_learning_rate: float = 0.1,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
+        fraction_result: float = 1.0,
         min_fit_clients: int = 1,
         min_evaluate_clients: int = 1,
         min_available_clients: int = 1,
+        min_result: int = 1,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
@@ -70,17 +72,19 @@
         initial_parameters: Optional[Parameters] = None,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
     ) -> None:
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
+            fraction_result=fraction_result,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
+            min_result=min_result,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
@@ -114,39 +118,45 @@
 
     def num_evaluation_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Use a fraction of available clients for evaluation."""
         num_clients = int(num_available_clients * self.fraction_evaluate)
         return max(num_clients, self.min_evaluate_clients), self.min_available_clients
 
     def configure_fit(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self,
+        server_round: int,
+        parameters: Parameters,
+        server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
         weights = parameters_to_ndarrays(parameters)
         self.pre_weights = weights
         parameters = ndarrays_to_parameters(weights)
         config = {}
         if self.on_fit_config_fn is not None:
             # Custom fit config function provided
             config = self.on_fit_config_fn(server_round)
         fit_ins = FitIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_fit_clients(
-            client_manager.num_available()
-        )
-        clients = client_manager.sample(
-            num_clients=sample_size, min_num_clients=min_num_clients
+            server.num_available(credential=credential)
         )
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # Return client/config pairs
         return [(client, fit_ins) for client in clients]
 
     def configure_evaluate(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self,
+        server_round: int,
+        parameters: Parameters,
+        server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation."""
         # Do not configure federated evaluation if fraction_evaluate is 0
         if self.fraction_evaluate == 0.0:
             return []
 
         # Parameters and config
@@ -154,19 +164,17 @@
         if self.on_evaluate_config_fn is not None:
             # Custom evaluation config function provided
             config = self.on_evaluate_config_fn(server_round)
         evaluate_ins = EvaluateIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_evaluation_clients(
-            client_manager.num_available()
-        )
-        clients = client_manager.sample(
-            num_clients=sample_size, min_num_clients=min_num_clients
+            server.num_available(credential=credential)
         )
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # Return client/config pairs
         return [(client, evaluate_ins) for client in clients]
 
     def aggregate_fit(
         self,
         server_round: int,
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/operation/strategy/strategy.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 # ==============================================================================
 """Flower server strategy."""
 
 
 from abc import ABC, abstractmethod
 from typing import Dict, List, Optional, Tuple, Union
 
-from daisyfl.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar
-from daisyfl.server.client_manager import ClientManager
+from daisyfl.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar, CheckResults, CurrentReturns
+from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
 
 class Strategy(ABC):
     """Abstract base class for server strategy implementations."""
 
     @abstractmethod
     def initialize_parameters(
-        self, client_manager: ClientManager
+        self, server: Server,
     ) -> Optional[Parameters]:
         """Initialize the (global) model parameters.
 
         Parameters
         ----------
         client_manager : ClientManager
             The client manager which holds all currently connected clients.
@@ -42,15 +42,16 @@
         parameters : Optional[Parameters]
             If parameters are returned, then the server will treat these as the
             initial global model parameters.
         """
 
     @abstractmethod
     def configure_fit(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self, server_round: int, parameters: Parameters, server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training.
 
         Parameters
         ----------
         server_round : int
             The current round of federated learning.
@@ -103,15 +104,16 @@
             results) then the server will no update the previous model
             parameters, the updates received in this round are discarded, and
             the global model parameters remain the same.
         """
 
     @abstractmethod
     def configure_evaluate(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self, server_round: int, parameters: Parameters, server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation.
 
         Parameters
         ----------
         server_round : int
             The current round of federated learning.
@@ -179,7 +181,18 @@
 
         Returns
         -------
         evaluation_result : Optional[Tuple[float, Dict[str, Scalar]]]
             The evaluation result, usually a Tuple containing loss and a
             dictionary containing task-specific metrics (e.g., accuracy).
         """
+    
+    @abstractmethod
+    def check_results(
+        self, current_returns: CurrentReturns,
+    ) -> CheckResults:
+        """Check if there are enough results
+        Query CurrentReturns instance from Server
+        Call op_tools.wait_for_results
+        wait until this function returns CheckResults.OK or CheckResults.FAIL
+        """
+
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/plugin/base/server_logic.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/base_async/server_logic.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,117 +8,145 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from logging import INFO, WARNING
-from typing import Dict, List, Optional, Tuple, TypedDict
-from daisyfl.server import Server as BaseServer
-from daisyfl.server.client_manager import ClientManager
-from daisyfl.server.strategy import Strategy
+from logging import INFO, WARNING, ERROR
+from typing import Dict, List, Optional, Tuple, TypedDict, Callable
+from queue import Queue
+from threading import Event
+from daisyfl.operator.strategy import Strategy
 from daisyfl.common import (
-    FitIns,
-    FitRes,
     Parameters,
-    Scalar,
     Report,
     Task,
     CURRENT_ROUND,
     TIMEOUT,
-    FIT_SAMPLES,
-    METRICS,
-    parameters_to_ndarrays,
-    ndarrays_to_parameters,
-    NDArrays,
+    PERIOD,
+    CREDENTIAL,
 )
-
-from daisyfl.server.client_proxy import ClientProxy
-
 from daisyfl.common.logger import log
 
-FitResultsAndFailures = Tuple[List[Tuple[ClientProxy, FitRes]], List[BaseException]]
+from daisyfl.operator.utils import (
+    get_configure_fit,
+    aggregate_fit,
+    generate_fit_report,
+    get_configure_evaluate,
+    aggregate_evaluate,
+    generate_evaluate_report,
+    wait_for_results,
+)
 
-class Server(BaseServer):
-    """Wrapper which adds SecAgg methods."""
 
-    def __init__(
-        self,
-        s: BaseServer,
+class ServerLogic():
+    def __init__(self,
+        server,
+        strategy: Strategy,
     ) -> None:
-        self.server = s
-
-    def disconnect_all_clients(self, timeout: Optional[float]) -> None:
-        """Send shutdown signal to all clients."""
-        self.server.disconnect_all_clients(timeout)
+        self.server = server
+        self.strategy: Strategy = strategy
+        self.subtasks = {}
 
     def fit_round(
         self,
         parameters: Parameters,
         task: Task,
     ) -> Optional[
         Tuple[Optional[Parameters], Optional[Report]]
     ]:
         """Perform a single round fit."""
         # Get clients and their respective instructions from strategy
-        client_instructions = self.server.get_configure_fit(
+        ## credential
+        if CREDENTIAL in task.config:
+            credential = task.config[CREDENTIAL]
+        else:
+            log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
+        ## get_clients
+        client_instructions = get_configure_fit(
+            strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             parameters=parameters,
-            client_manager=self.server.get_client_manager(),
+            server=self.server,
             config=task.config,
+            credential=credential,
         )
         # Collect `fit` results from all clients participating in this round
-        results, failures = self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
         )
+        self.subtasks[subtask_id] = subtask_id
+        Event().wait(timeout=task.config[PERIOD])
+        # check
+        results = []
+        for stid in list(self.subtasks.values()):
+            results = results + self.server.get_results(stid)
+        if len(results) == 0:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
         # Aggregate training results
-        parameters_aggregated, samples, metrics_aggregated  = self.server.aggregate_fit(
-            task.config[CURRENT_ROUND],
-            results,
-            failures,
+        parameters_aggregated, samples, metrics_aggregated = aggregate_fit(
+            strategy=self.strategy,
+            server_round=task.config[CURRENT_ROUND],
+            results=results,
+            failures=[],
         )
         # Get report
-        report = self.server.generate_fit_report(
-            task.config[CURRENT_ROUND],
-            samples,
-            metrics_aggregated,
+        report = generate_fit_report(
+            server_round=task.config[CURRENT_ROUND],
+            samples=samples,
+            metrics_aggregated=metrics_aggregated,
         )
 
         return parameters_aggregated, report
 
     def evaluate_round(
-        self, 
+        self,
         parameters: Parameters,
         task: Task,
     ) -> Optional[Report]:
         """Validate current global model on a number of clients."""
         # Get clients and their respective instructions from strategy
-        client_instructions = self.server.get_configure_evaluate(
+        ## credential
+        if CREDENTIAL in task.config:
+            credential = task.config[CREDENTIAL]
+        else:
+            log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
+        ## get_clients
+        client_instructions = get_configure_evaluate(
+            strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             parameters=parameters,
-            client_manager=self.server.get_client_manager(),
+            server=self.server,
             config=task.config,
+            credential=credential,
         )
         # Collect `evaluate` results from all clients participating in this round
-        results, failures = self.server.evaluate_clients(
-            client_instructions,
+        subtask_id = self.server.evaluate_clients(
+            client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
         )
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_evaluate_report(task.config[CURRENT_ROUND], 0, 9999.0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
         # Aggregate the evaluation results
-        loss_aggregated, samples, metrics_aggregated = self.server.aggregate_evaluate(
-            task.config[CURRENT_ROUND],
-            results,
-            failures,
+        loss_aggregated, samples, metrics_aggregated = aggregate_evaluate(
+            strategy=self.strategy,
+            server_round=task.config[CURRENT_ROUND],
+            results=results,
+            failures=[],
         )
         # Get report
-        report = self.server.generate_evaluate_report(
-            task.config[CURRENT_ROUND],
-            samples,
-            loss_aggregated,
-            metrics_aggregated,
+        report = generate_evaluate_report(
+            server_round=task.config[CURRENT_ROUND],
+            samples=samples,
+            loss_aggregated=loss_aggregated,
+            metrics_aggregated=metrics_aggregated,
         )
 
-        return report
+        return report
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/plugin/msg_demo/client_logic.py` & `daisyfl-0.4.5/src/py/daisyfl/server/client_proxy.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,79 +8,81 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-import numpy as np
-from typing import Dict, List, Tuple, TypedDict
+"""Flower client (abstract base class)."""
+
+
+from abc import ABC, abstractmethod
+from typing import Optional, Union, Callable
+
 from daisyfl.common import (
-    ndarrays_to_parameters,
-    parameters_to_ndarrays,
-    Status,
-    Code,
+    DisconnectRes,
+    EvaluateIns,
+    EvaluateRes,
     FitIns,
     FitRes,
     GetParametersIns,
     GetParametersRes,
     GetPropertiesIns,
     GetPropertiesRes,
-    EvaluateIns,
-    EvaluateRes,
-    NDArrays,
-)
-from daisyfl.common.logger import log
-from logging import DEBUG, ERROR, INFO, WARNING
-from daisyfl.client import Client as BaseClient
-from daisyfl.plugin.msg_demo.common import (
-    WHO_CREATE_THIS_DEMO,
-    TIME,
-    STUDENT,
-    Time,
-    Student,
+    Properties,
+    ReconnectIns,
 )
+from daisyfl.proto.transport_pb2 import ClientMessage
 
-class Client(BaseClient):
-    """Wrapper which adds SecAgg methods."""
-    
-    def __init__(self, c: BaseClient) -> None:
-        self.client = c
-    
-    def get_parameters(self, ins: GetParametersIns) -> GetParametersRes:
+
+class ClientProxy(ABC):
+    """Abstract base class for Flower client proxies."""
+
+    def __init__(self, cid: str):
+        self.cid = cid
+        self.properties: Properties = {}
+
+    @abstractmethod
+    def get_properties(
+        self,
+        ins: GetPropertiesIns,
+    ) -> None:
+        """Returns the client's properties."""
+
+    @abstractmethod
+    def get_parameters(
+        self,
+        ins: GetParametersIns,
+    ) -> None:
         """Return the current local model parameters."""
-        return self.client.get_parameters(ins)
-    
-    def get_properties(self, ins: GetPropertiesIns) -> GetPropertiesRes:
-        """Return set of client's properties."""
-        return self.client.get_properties(ins)
-    
+
+    @abstractmethod
     def fit(
-        self, ins: FitIns,
-    ) -> FitRes:
-        stage = Time(ins.config[TIME])
-        if stage == Time.SAY_HI:
-            return _say_hi(self, ins)
-        elif stage == Time.FIT:
-            return _fit(self, ins)
-        else:
-            raise ValueError("Invalid stage received")
+        self,
+        ins: FitIns,
+    ) -> None:
+        """Refine the provided parameters using the locally held dataset."""
 
+    @abstractmethod
     def evaluate(
-        self, ins: EvaluateIns,
-    ) -> EvaluateRes:
-        return self.client.evaluate(ins)
-
-def _say_hi(client, ins: FitIns) -> FitRes:
-    log(INFO,
-        "\nHello, %s.\nI am %s.\nNice to meet you.",
-        ins.config[WHO_CREATE_THIS_DEMO],
-        ins.config[STUDENT]["name"],
-    )
-    return FitRes(
-        status=Status(code=Code.OK, message="Success"),
-        parameters=ins.parameters,
-        config=ins.config,
-    )
+        self,
+        ins: EvaluateIns,
+    ) -> None:
+        """Evaluate the provided parameters using the locally held dataset."""
+
+    @abstractmethod
+    def reconnect(
+        self,
+        ins: ReconnectIns,
+    ) -> None:
+        """Disconnect and (optionally) reconnect later."""
+    
+    @abstractmethod
+    def submit_client_message(
+        self,
+        client_message: ClientMessage,
+    ) -> None:
+        """Receive, deserialize, and submit"""
 
-def _fit(client, ins: FitIns) -> FitRes:
-    return client.client.fit(ins)
+    @abstractmethod
+    def set_submit_subtask_fn(self, submit_subtask: Callable) -> None:
+        """Set callback function"""
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/plugin/msg_demo/server_logic.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/server_logic.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,136 +8,131 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from logging import INFO, WARNING
-from typing import Dict, List, Optional, Tuple, TypedDict
-from daisyfl.server import Server as BaseServer
+from logging import INFO, WARNING, ERROR
+from queue import Queue
+from typing import Dict, List, Optional, Tuple, TypedDict, Callable
+from daisyfl.operator.strategy import Strategy
 from daisyfl.common import (
-    FitIns,
-    FitRes,
     Parameters,
     Report,
     Task,
     CURRENT_ROUND,
     TIMEOUT,
+    PERIOD,
+    CREDENTIAL,
 )
-from daisyfl.plugin.msg_demo.common import (
+from .msg import (
     WHO_CREATE_THIS_DEMO,
     TIME,
     STUDENT,
     Time,
     Student,
 )
-from daisyfl.server.client_proxy import ClientProxy
 from daisyfl.common.logger import log
 
-FitResultsAndFailures = Tuple[List[Tuple[ClientProxy, FitRes]], List[BaseException]]
+from daisyfl.operator.utils import (
+    get_configure_fit,
+    aggregate_fit,
+    generate_fit_report,
+    get_clients_from_list,
+    get_configure_evaluate,
+    aggregate_evaluate,
+    generate_evaluate_report,
+    wait_for_results,
+)
+from daisyfl.server import Server
 
-class Server(BaseServer):
-    """Wrapper which adds SecAgg methods."""
+from daisyfl.operator.base.server_logic import ServerLogic as BaseServerLogic
 
-    def __init__(
-        self,
-        s: BaseServer,
-    ) -> None:
-        self.server = s
 
-    def disconnect_all_clients(self, timeout: Optional[float]) -> None:
-        """Send shutdown signal to all clients."""
-        self.server.disconnect_all_clients(timeout)
+class ServerLogic(BaseServerLogic):
+    def __init__(self,
+        server: Server,
+        strategy: Strategy,
+    ) -> None:
+        self.server: Server = server
+        self.strategy: Strategy = strategy
 
     def fit_round(
         self,
         parameters: Parameters,
         task: Task,
     ) -> Optional[
         Tuple[Optional[Parameters], Optional[Report]]
     ]:
         """Perform a single round fit."""
         # SAY_HI
         ## Get clients and their respective instructions from strategy
-        client_instructions = self.server.get_configure_fit(
+        ### credential
+        if CREDENTIAL in task.config:
+            credential = task.config[CREDENTIAL]
+        else:
+            log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
+        ### get_clients
+        client_instructions = get_configure_fit(
+            strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             parameters=parameters,
-            client_manager=self.server.get_client_manager(),
+            server=self.server,
             config=task.config,
+            credential=credential,
         )
         config = task.config
         config = _setup_info(config, "Tsung-Han Chang", "Alice", 18, False)
         config = _transition(config)
         client_instructions = _set_config(config, client_instructions)
         ## Collect `fit` results from all clients participating in this round
-        results, failures = self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
         )
-        
-        # FIT
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
+        # TRAIN
         config = _transition(config)
+        client_instructions = get_clients_from_list(server=self.server, clients=client_instructions, timeout=3, credential=credential,)
         client_instructions = _set_config(config, client_instructions)
         ## Collect `fit` results from all clients participating in this round
-        results, failures = self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
         )
-        # Aggregate training results
-        parameters_aggregated, samples, metrics_aggregated  = self.server.aggregate_fit(
-            task.config[CURRENT_ROUND],
-            results,
-            failures,
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
+        ## Aggregate training results
+        parameters_aggregated, samples, metrics_aggregated  = aggregate_fit(
+            strategy=self.strategy,
+            server_round=task.config[CURRENT_ROUND],
+            results=results,
+            failures=[],
         )
-        # Get report
-        report = self.server.generate_fit_report(
-            task.config[CURRENT_ROUND],
-            samples,
-            metrics_aggregated,
+        ## Get report
+        report = generate_fit_report(
+            server_round=task.config[CURRENT_ROUND],
+            samples=samples,
+            metrics_aggregated=metrics_aggregated,
         )
 
         return parameters_aggregated, report
 
-    def evaluate_round(
-        self, 
-        parameters: Parameters,
-        task: Task,
-    ) -> Optional[Report]:
-        """Validate current global model on a number of clients."""
-        # Get clients and their respective instructions from strategy
-        client_instructions = self.server.get_configure_evaluate(
-            server_round=task.config[CURRENT_ROUND],
-            parameters=parameters,
-            client_manager=self.server.get_client_manager(),
-            config=task.config,
-        )
-        # Collect `evaluate` results from all clients participating in this round
-        results, failures = self.server.evaluate_clients(
-            client_instructions,
-            max_workers=self.server.get_max_workers(),
-            timeout=task.config[TIMEOUT],
-        )
-        # Aggregate the evaluation results
-        loss_aggregated, samples, metrics_aggregated = self.server.aggregate_evaluate(
-            task.config[CURRENT_ROUND],
-            results,
-            failures,
-        )
-        # Get report
-        report = self.server.generate_evaluate_report(
-            task.config[CURRENT_ROUND],
-            samples,
-            loss_aggregated,
-            metrics_aggregated,
-        )
-
-        return report
 
 def _setup_info(
     config: TypedDict,
     author: str,
     stu_name: str,
     stu_age: int,
     stu_graduate: bool
@@ -157,14 +152,12 @@
         config[TIME] = Time((config[TIME] + 1) % Time.__len__()).value
     else:
         config[TIME] = Time(0).value
     return config
 
 def _set_config(
     config: TypedDict,
-    client_instructions: List[Tuple[ClientProxy, FitIns]],
-) -> List[Tuple[ClientProxy, FitIns]]:
+    client_instructions,
+):
     for i in range(len(client_instructions)):
         client_instructions[i][1].config = config.copy()
     return client_instructions
-
-
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/plugin/msg_demo/zone_server_logic.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/zone_server_logic.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,160 +8,158 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from logging import INFO, WARNING
-from typing import Dict, List, Optional, Tuple, TypedDict
-from daisyfl.server import Server as BaseServer
+from logging import INFO, WARNING, ERROR
+from typing import Dict, List, Optional, Tuple, TypedDict, Callable
+from threading import Timer, Condition, Event
+from queue import Queue
+from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.operator.strategy import Strategy
 from daisyfl.common import (
-    FitIns,
-    FitRes,
     Parameters,
     Report,
     Task,
     CURRENT_ROUND,
     TIMEOUT,
+    PERIOD,
+    CREDENTIAL,
+    FitIns,
 )
-from daisyfl.plugin.msg_demo.common import (
+from .msg import (
     TIME,
     Time,
 )
-from daisyfl.server.client_proxy import ClientProxy
 from daisyfl.common.logger import log
 
-FitResultsAndFailures = Tuple[List[Tuple[ClientProxy, FitRes]], List[BaseException]]
+from daisyfl.operator.utils import (
+    get_configure_fit,
+    aggregate_fit,
+    generate_fit_report,
+    get_configure_evaluate,
+    aggregate_evaluate,
+    generate_evaluate_report,
+    wait_for_results,
+    get_clients_from_list,
+)
+from daisyfl.server import Server
+from daisyfl.operator.base.server_logic import ServerLogic as BaseServerLogic
 
-class ZoneServer(BaseServer):
-    """Wrapper which adds SecAgg methods."""
 
-    def __init__(
-        self,
-        s: BaseServer,
+class ZoneServerLogic(BaseServerLogic):
+    def __init__(self,
+        server: Server,
+        strategy: Strategy,
     ) -> None:
-        self.server = s
-
-    def disconnect_all_clients(self, timeout: Optional[float]) -> None:
-        """Send shutdown signal to all clients."""
-        self.server.disconnect_all_clients(timeout)
+        self.server: Server = server
+        self.strategy: Strategy = strategy
 
     def fit_round(
         self,
         parameters: Parameters,
         task: Task,
     ) -> Optional[
         Tuple[Optional[Parameters], Optional[Report]]
     ]:
         """Perform a single round fit."""
         stage = Time(task.config[TIME])
         if stage == Time.SAY_HI:
-            return _say_hi(self, parameters, task)
-        elif stage == Time.FIT:
-            return _fit(self, parameters, task)
+            parameters, report, client_instructions = _say_hi(self, parameters, task,)
+            self.clients = client_instructions
+            return parameters, report
+        elif stage == Time.TRAIN:
+            return _fit(self, parameters, task, self.clients)
         else:
             raise ValueError("Invalid stage received")
 
-    def evaluate_round(
-        self, 
-        parameters: Parameters,
-        task: Task,
-    ) -> Optional[Report]:
-        """Validate current global model on a number of clients."""
-        # Get clients and their respective instructions from strategy
-        client_instructions = self.server.get_configure_evaluate(
-            server_round=task.config[CURRENT_ROUND],
-            parameters=parameters,
-            client_manager=self.server.get_client_manager(),
-            config=task.config,
-        )
-        # Collect `evaluate` results from all clients participating in this round
-        results, failures = self.server.evaluate_clients(
-            client_instructions,
-            max_workers=self.server.get_max_workers(),
-            timeout=task.config[TIMEOUT],
-        )
-        # Aggregate the evaluation results
-        loss_aggregated, samples, metrics_aggregated = self.server.aggregate_evaluate(
-            task.config[CURRENT_ROUND],
-            results,
-            failures,
-        )
-        # Get report
-        report = self.server.generate_evaluate_report(
-            task.config[CURRENT_ROUND],
-            samples,
-            loss_aggregated,
-            metrics_aggregated,
-        )
-
-        return report
-
 
 def _say_hi(
-    server,
+    server_logic: ZoneServerLogic,
     parameters: Parameters,
     task: Task,
 ) -> Optional[
     Tuple[Optional[Parameters], Optional[Report]]
 ]:
     ## Get clients and their respective instructions from strategy
-    client_instructions = server.server.get_configure_fit(
+    ### credential
+    if CREDENTIAL in task.config:
+        credential = task.config[CREDENTIAL]
+    else:
+        log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
+    ### get_clients
+    client_instructions = get_configure_fit(
+        strategy=server_logic.strategy,
         server_round=task.config[CURRENT_ROUND],
         parameters=parameters,
-        client_manager=server.server.get_client_manager(),
+        server=server_logic.server,
         config=task.config,
+        credential=credential,
     )
     ## Collect `fit` results from all clients participating in this round
-    results, failures = server.server.fit_clients(
+    subtask_id = server_logic.server.fit_clients(
         client_instructions=client_instructions,
-        max_workers=server.server.get_max_workers(),
+        max_workers=server_logic.server.get_max_workers(),
         timeout=task.config[TIMEOUT],
     )
+    # check
+    success = wait_for_results(strategy=server_logic.strategy, current_returns=server_logic.server.get_current_returns(subtask_id))
+    if not success:
+        return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+    results = server_logic.server.get_results(subtask_id)
+    server_logic.server.finish_subtask(subtask_id)
     # Get report
-    report = server.server.generate_fit_report(
-        task.config[CURRENT_ROUND],
-        0,
-        {},
+    report = generate_fit_report(
+        server_round=task.config[CURRENT_ROUND],
+        samples=0,
+        metrics_aggregated={},
     )
         
-    return parameters, report
+    return parameters, report, client_instructions
 
-def _fit(server, parameters, task):
-        ## Get clients and their respective instructions from strategy
-    client_instructions = server.server.get_configure_fit(
+def _fit(server_logic: ZoneServerLogic, parameters: Parameters, task: Task, client_instructions: List[Tuple[ClientProxy, FitIns]]):
+    """Perform a single round fit."""
+    # Get clients and their respective instructions from strategy
+    ### credential
+    if CREDENTIAL in task.config:
+        credential = task.config[CREDENTIAL]
+    else:
+        log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
+    ### get_clients
+    client_instructions = get_clients_from_list(server=server_logic.server, clients=client_instructions, timeout=0, credential=credential,)
+    client_instructions = get_configure_fit(
+        strategy=server_logic.strategy,
         server_round=task.config[CURRENT_ROUND],
         parameters=parameters,
-        client_manager=server.server.get_client_manager(),
+        server=server_logic.server,
         config=task.config,
+        credential=credential,
     )
-    ## Collect `fit` results from all clients participating in this round
-    results, failures = server.server.fit_clients(
+    # Collect `fit` results from all clients participating in this round
+    subtask_id = server_logic.server.fit_clients(
         client_instructions=client_instructions,
-        max_workers=server.server.get_max_workers(),
+        max_workers=server_logic.server.get_max_workers(),
         timeout=task.config[TIMEOUT],
     )
+    # check
+    success = wait_for_results(strategy=server_logic.strategy, current_returns=server_logic.server.get_current_returns(subtask_id))
+    if not success:
+        return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+    results = server_logic.server.get_results(subtask_id)
+    server_logic.server.finish_subtask(subtask_id)
     # Aggregate training results
-    parameters_aggregated, samples, metrics_aggregated  = server.server.aggregate_fit(
-        task.config[CURRENT_ROUND],
-        results,
-        failures,
+    parameters_aggregated, samples, metrics_aggregated  = aggregate_fit(
+        strategy=server_logic.strategy,
+        server_round=task.config[CURRENT_ROUND],
+        results=results,
+        failures=[],
     )
     # Get report
-    report = server.server.generate_fit_report(
-        task.config[CURRENT_ROUND],
-        samples,
-        metrics_aggregated,
+    report = generate_fit_report(
+        server_round=task.config[CURRENT_ROUND],
+        samples=samples,
+        metrics_aggregated=metrics_aggregated,
     )
-        
-    return parameters_aggregated, report
-
-def _set_config(
-    config: TypedDict,
-    client_instructions: List[Tuple[ClientProxy, FitIns]],
-) -> List[Tuple[ClientProxy, FitIns]]:
-    for i in range(len(client_instructions)):
-        client_instructions[i][1].config = config.copy()
-    return client_instructions
-
 
+    return parameters_aggregated, report
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/__init__.py` & `daisyfl-0.4.5/src/py/daisyfl/simulation/ray_transport/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Contains server side utilities to be used in combination with various
-components."""
-
-from .client_logic import Client as Client
-from .server_logic import Server as Server
-
-__all__ = [
-    "Client",
-    "Server",
-]
+"""Ray-based Flower ClientProxy implementation."""
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/client_logic.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/client_logic.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-import numpy as np
-from daisyfl.plugin.sec_agg.utils import primitives
 from typing import Dict, List, Tuple, TypedDict
 from daisyfl.common import (
     ndarrays_to_parameters,
     parameters_to_ndarrays,
     Status,
     Code,
     FitIns,
@@ -27,15 +25,15 @@
     GetPropertiesIns,
     GetPropertiesRes,
     EvaluateIns,
     EvaluateRes,
     NDArrays,
     FIT_SAMPLES,
 )
-from daisyfl.plugin.sec_agg.common.typing import (
+from .common import (
     PROTO_KEY,
     SEC_AGG_PARAM_DICT,
     PUBLIC_KEYS,
     PUBLIC_KEYS_LIST,
     SHARE_KEYS_PACKETS,
     FORWARD_PACKETS,
     SHARE_REQUEST,
@@ -44,29 +42,23 @@
     PublicKeys,
     ShareKeysPacket,
     ShareRequest,
     ShareResponse,
 )
 from daisyfl.common.logger import log
 from logging import DEBUG, ERROR, INFO, WARNING
-from daisyfl.client import Client as BaseClient
+from daisyfl.client import Client
+from daisyfl.operator.base.client_logic import ClientLogic as BaseClientLogic
+from . import primitives
 
-class Client(BaseClient):
+class ClientLogic(BaseClientLogic):
     """Wrapper which adds SecAgg methods."""
     
-    def __init__(self, c: BaseClient) -> None:
-        self.client = c
-    
-    def get_parameters(self, ins: GetParametersIns) -> GetParametersRes:
-        """Return the current local model parameters."""
-        return self.client.get_parameters(ins)
-    
-    def get_properties(self, ins: GetPropertiesIns) -> GetPropertiesRes:
-        """Return set of client's properties."""
-        return self.client.get_properties(ins)
+    def __init__(self, client: Client) -> None:
+        self.client: Client = client
     
     def fit(
         self, ins: FitIns,
     ) -> FitRes:
         stage = Proto(ins.config[PROTO_KEY])
         if stage == Proto.SETUP:
             return setup_param(self, ins)
@@ -77,231 +69,227 @@
         elif stage == Proto.ASK_VECTORS:
             return ask_vectors(self, ins)
         elif stage == Proto.UNMASK_VECTORS:
             return unmask_vectors(self, ins)
         else:
             raise ValueError("Invalid stage Proto received") 
 
-    def evaluate(
-        self, ins: EvaluateIns,
-    ) -> EvaluateRes:
-        return self.client.evaluate(ins)
 
-def setup_param(client, ins: FitIns) -> FitRes:
+def setup_param(client_logic: ClientLogic, ins: FitIns) -> FitRes:
     # Assigning parameter values to object fields
     sec_agg_param_dict = ins.config[SEC_AGG_PARAM_DICT]
-    client.sample_num = sec_agg_param_dict['sample_num']
-    client.sec_agg_id = sec_agg_param_dict['sec_agg_id']
-    client.share_num = sec_agg_param_dict['share_num']
-    client.threshold = sec_agg_param_dict['threshold']
-    client.clipping_range = sec_agg_param_dict['clipping_range']
-    client.target_range = sec_agg_param_dict['target_range']
-    client.mod_range = sec_agg_param_dict['mod_range']
-    client.max_weights_factor = sec_agg_param_dict['max_weights_factor']
+    client_logic.sample_num = sec_agg_param_dict['sample_num']
+    client_logic.sec_agg_id = sec_agg_param_dict['sec_agg_id']
+    client_logic.share_num = sec_agg_param_dict['share_num']
+    client_logic.threshold = sec_agg_param_dict['threshold']
+    client_logic.clipping_range = sec_agg_param_dict['clipping_range']
+    client_logic.target_range = sec_agg_param_dict['target_range']
+    client_logic.mod_range = sec_agg_param_dict['mod_range']
+    client_logic.max_weights_factor = sec_agg_param_dict['max_weights_factor']
 
     # key is another client's id
     # value is the secret share we possess that contributes to the client's secret (bytes)
-    client.b_share_dict = {}
-    client.sk1_share_dict = {}
-    client.shared_key_2_dict = {}
+    client_logic.b_share_dict = {}
+    client_logic.sk1_share_dict = {}
+    client_logic.shared_key_2_dict = {}
     log(INFO, "SecAgg Stage 0 Completed: Parameters Set Up")
     return FitRes(
         status=Status(code=Code.OK, message="Success"),
         parameters=ins.parameters,
         config={},
     )
 
 
-def ask_keys(client, ins: FitIns) -> FitRes:
+def ask_keys(client_logic: ClientLogic, ins: FitIns) -> FitRes:
     # Create 2 sets private public key pairs
     # One for creating pairwise masks
     # One for encrypting message to distribute shares
-    client.sk1, client.pk1 = primitives.generate_key_pairs()
-    client.sk2, client.pk2 = primitives.generate_key_pairs()
+    client_logic.sk1, client_logic.pk1 = primitives.generate_key_pairs()
+    client_logic.sk2, client_logic.pk2 = primitives.generate_key_pairs()
     log(INFO, "SecAgg Stage 1 Completed: Created Key Pairs")
     config = {}
     config[PUBLIC_KEYS] = PublicKeys(
-        pk1=primitives.public_key_to_bytes(client.pk1),
-        pk2=primitives.public_key_to_bytes(client.pk2),
+        pk1=primitives.public_key_to_bytes(client_logic.pk1),
+        pk2=primitives.public_key_to_bytes(client_logic.pk2),
     ).to_dict()
 
     return FitRes(
         status=Status(code=Code.OK, message="Success"),
         parameters=ins.parameters,
         config=config,
     )
 
 
-def share_keys(client, ins: FitIns) -> FitRes:
+def share_keys(client_logic: ClientLogic, ins: FitIns) -> FitRes:
     # Distribute shares for private mask seed and first private key
-    client.public_keys_dict = ins.config[PUBLIC_KEYS_LIST]
+    client_logic.public_keys_dict = ins.config[PUBLIC_KEYS_LIST]
     # check size is larger than threshold
-    if len(client.public_keys_dict) < client.threshold:
+    if len(client_logic.public_keys_dict) < client_logic.threshold:
+        print(len(client_logic.public_keys_dict))
+        print(client_logic.threshold)
         raise Exception("Available neighbours number smaller than threshold")
     # check if all public keys received are unique
     pk_list: List[bytes] = []
-    for i in client.public_keys_dict.values():
+    for i in client_logic.public_keys_dict.values():
         pk_list.append(i["pk1"])
         pk_list.append(i["pk2"])
     if len(set(pk_list)) != len(pk_list):
         raise Exception("Some public keys are identical")
     # sanity check that own public keys are correct in dict
-    if client.public_keys_dict[client.sec_agg_id]["pk1"] != primitives.public_key_to_bytes(client.pk1) \
-        or client.public_keys_dict[client.sec_agg_id]["pk2"] != primitives.public_key_to_bytes(client.pk2):
+    if client_logic.public_keys_dict[client_logic.sec_agg_id]["pk1"] != primitives.public_key_to_bytes(client_logic.pk1) \
+        or client_logic.public_keys_dict[client_logic.sec_agg_id]["pk2"] != primitives.public_key_to_bytes(client_logic.pk2):
         raise Exception(
             "Own public keys are displayed in dict incorrectly, should not happen!")
     # Generate private mask seed
-    client.b = primitives.rand_bytes(32)
+    client_logic.b = primitives.rand_bytes(32)
 
     # Create shares
     b_shares = primitives.create_shares(
-        client.b, client.threshold, client.share_num
+        client_logic.b, client_logic.threshold, client_logic.share_num
     )
     sk1_shares = primitives.create_shares(
         primitives.private_key_to_bytes(
-            client.sk1), client.threshold, client.share_num
+            client_logic.sk1), client_logic.threshold, client_logic.share_num
     )
     share_keys_res = []
 
-    for idx, p in enumerate(client.public_keys_dict.items()):
+    for idx, p in enumerate(client_logic.public_keys_dict.items()):
         client_sec_agg_id, client_public_keys = p
-        if client_sec_agg_id == client.sec_agg_id:
-            client.b_share_dict[client.sec_agg_id] = b_shares[idx]
-            client.sk1_share_dict[client.sec_agg_id] = sk1_shares[idx]
+        if client_sec_agg_id == client_logic.sec_agg_id:
+            client_logic.b_share_dict[client_logic.sec_agg_id] = b_shares[idx]
+            client_logic.sk1_share_dict[client_logic.sec_agg_id] = sk1_shares[idx]
         else:
             shared_key = primitives.generate_shared_key(
-                client.sk2, primitives.bytes_to_public_key(client_public_keys["pk2"])
+                client_logic.sk2, primitives.bytes_to_public_key(client_public_keys["pk2"])
             )
-            client.shared_key_2_dict[client_sec_agg_id] = shared_key
+            client_logic.shared_key_2_dict[client_sec_agg_id] = shared_key
             plaintext = primitives.share_keys_plaintext_concat(
-                client.sec_agg_id, client_sec_agg_id, b_shares[idx], sk1_shares[idx]
+                client_logic.sec_agg_id, client_sec_agg_id, b_shares[idx], sk1_shares[idx]
             )
             ciphertext = primitives.encrypt(shared_key, plaintext)
             share_keys_packet_dict = ShareKeysPacket(
-                source=client.sec_agg_id, destination=client_sec_agg_id, ciphertext=ciphertext
+                source=client_logic.sec_agg_id, destination=client_sec_agg_id, ciphertext=ciphertext
             ).to_dict()
             share_keys_res.append(share_keys_packet_dict)
     ins.config[SHARE_KEYS_PACKETS] = share_keys_res
 
     log(INFO, "SecAgg Stage 2 Completed: Sent Shares via Packets")
     return FitRes(
         status=Status(code=Code.OK, message="Success"),
         parameters=ins.parameters,
         config=ins.config,
     )
 
 
-def ask_vectors(
-    client, ins: FitIns
-) -> FitRes:
+def ask_vectors(client_logic: ClientLogic, ins: FitIns) -> FitRes:
     # Receive shares and fit model
     packet_list = ins.config[FORWARD_PACKETS]
     available_clients: List[int] = []
 
-    if len(packet_list) + 1 < client.threshold:
+    if len(packet_list) + 1 < client_logic.threshold:
         raise Exception("Available neighbours number smaller than threshold")
 
     # decode all packets and verify all packets are valid. Save shares received
     for packet in packet_list:
         source = packet["source"]
         available_clients.append(source)
         destination = packet["destination"]
         ciphertext = packet["ciphertext"]
-        if destination != client.sec_agg_id:
+        if destination != client_logic.sec_agg_id:
             raise Exception(
                 "Received packet meant for another user. Not supposed to happen")
-        shared_key = client.shared_key_2_dict[source]
+        shared_key = client_logic.shared_key_2_dict[source]
         plaintext = primitives.decrypt(shared_key, ciphertext)
         try:
             plaintext_source, plaintext_destination, plaintext_b_share, plaintext_sk1_share = \
                 primitives.share_keys_plaintext_separate(plaintext)
         except:
             raise Exception(
                 "Decryption of ciphertext failed. Not supposed to happen")
         if plaintext_source != source:
             raise Exception(
                 "Received packet source is different from intended source. Not supposed to happen")
         if plaintext_destination != destination:
             raise Exception(
                 "Received packet destination is different from intended destination. Not supposed to happen")
-        client.b_share_dict[source] = plaintext_b_share
-        client.sk1_share_dict[source] = plaintext_sk1_share
+        client_logic.b_share_dict[source] = plaintext_b_share
+        client_logic.sk1_share_dict[source] = plaintext_sk1_share
 
     # fit client
     del ins.config[FORWARD_PACKETS]
-    res: FitRes = client.client.fit(FitIns(
+    res: FitRes = client_logic.client.fit(FitIns(
         parameters=ins.parameters, 
         config=ins.config
     ))
     parameters = parameters_to_ndarrays(res.parameters)
     for key, value in res.config.items():
         ins.config[key] = value
     weights_factor = ins.config[FIT_SAMPLES]
 
     # Quantize weight update vector
     quantized_weights = primitives.quantize(
-        parameters, client.clipping_range, client.target_range)
+        parameters, client_logic.clipping_range, client_logic.target_range)
 
     # weights factor cannoot exceed maximum
-    if weights_factor > client.max_weights_factor:
-        weights_factor = client.max_weights_factor
+    if weights_factor > client_logic.max_weights_factor:
+        weights_factor = client_logic.max_weights_factor
         log(WARNING, "weights_factor exceeds allowed range and has been clipped. Either increase max_weights_factor, or train with fewer data. (Or server is performing unweighted aggregation)")
 
     quantized_weights = primitives.weights_multiply(
         quantized_weights, weights_factor)
     quantized_weights = primitives.factor_weights_combine(
         weights_factor, quantized_weights)
 
     dimensions_list: List[Tuple] = [a.shape for a in quantized_weights]
 
     # add private mask
     private_mask = primitives.pseudo_rand_gen(
-        client.b, client.mod_range, dimensions_list)
+        client_logic.b, client_logic.mod_range, dimensions_list)
     quantized_weights = primitives.weights_addition(
         quantized_weights, private_mask)
 
     for client_id in available_clients:
         # add pairwise mask
         shared_key = primitives.generate_shared_key(
-            client.sk1, primitives.bytes_to_public_key(client.public_keys_dict[client_id]["pk1"]))
+            client_logic.sk1, primitives.bytes_to_public_key(client_logic.public_keys_dict[client_id]["pk1"]))
         pairwise_mask = primitives.pseudo_rand_gen(
-            shared_key, client.mod_range, dimensions_list)
-        if client.sec_agg_id > client_id:
+            shared_key, client_logic.mod_range, dimensions_list)
+        if client_logic.sec_agg_id > client_id:
             quantized_weights = primitives.weights_addition(
                 quantized_weights, pairwise_mask)
         else:
             quantized_weights = primitives.weights_subtraction(
                 quantized_weights, pairwise_mask)
 
     # Take mod of final weight update vector and return to server
     quantized_weights = primitives.weights_mod(
-        quantized_weights, client.mod_range)
+        quantized_weights, client_logic.mod_range)
     log(INFO, "SecAgg Stage 3 Completed: Sent Vectors")
     parameters = ndarrays_to_parameters(quantized_weights)
 
     return FitRes(
         status=res.status,
         parameters=parameters,
         config=ins.config,
     )
 
 
-def unmask_vectors(client, ins: FitIns) -> FitRes:
+def unmask_vectors(client_logic: ClientLogic, ins: FitIns) -> FitRes:
     # Send private mask seed share for every avaliable client (including itclient)
     # Send first private key share for building pairwise mask for every dropped client
     available_clients = ins.config[SHARE_REQUEST]["survivals"]
-    if len(available_clients) < client.threshold:
+    if len(available_clients) < client_logic.threshold:
         raise Exception("Available neighbours number smaller than threshold")
 
     dropout_clients = ins.config[SHARE_REQUEST]["dropouts"]
     share_dict: Dict[int, bytes] = {}
     for idx in available_clients:
-        share_dict[idx] = client.b_share_dict[idx]
+        share_dict[idx] = client_logic.b_share_dict[idx]
     for idx in dropout_clients:
-        share_dict[idx] = client.sk1_share_dict[idx]
+        share_dict[idx] = client_logic.sk1_share_dict[idx]
     log(INFO, "SecAgg Stage 4 Completed: Sent Shares for Unmasking")
     ins.config[SHARE_RESPONSE] = ShareResponse(share_dict=share_dict).to_dict()
     return FitRes(
         status=Status(code=Code.OK, message="Success"),
         parameters=ins.parameters,
         config=ins.config,
     )
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/common/typing.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 # Copyright 2020 Adap GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,16 +16,14 @@
 # ==============================================================================
 """Flower type definitions."""
 
 
 from dataclasses import dataclass
 from dataclasses_json import dataclass_json
 from typing import Dict, List
-from daisyfl.common import Scalar, Parameters, FitIns
-import numpy as np
 from enum import Enum
 
 # check stage
 PROTO_KEY = "PROTO_KEY"
 # stage 0 ins
 SEC_AGG_PARAM_DICT = "SEC_AGG_PARAM_DICT"
 # stage 1 res
@@ -67,8 +67,8 @@
 class ShareRequest:
     survivals: List[int]
     dropouts: List[int]
     
 @dataclass_json
 @dataclass
 class ShareResponse:
-    share_dict: Dict[int, bytes]
+    share_dict: Dict[int, bytes]
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/server_logic.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/server_logic.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,186 +8,234 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from logging import INFO, WARNING
-from typing import Dict, List, Optional, Tuple, TypedDict
+from logging import INFO, WARNING, ERROR
+from typing import Dict, List, Optional, Tuple, TypedDict, Callable
+from queue import Queue
 from daisyfl.common.typing import NDArrays
-from daisyfl.server import Server as BaseServer
-from daisyfl.server.client_manager import ClientManager
-from daisyfl.server.strategy import Strategy
+from daisyfl.operator.strategy import Strategy
 from daisyfl.common import (
     FitIns,
     FitRes,
     Parameters,
     Scalar,
     Report,
     Task,
     CURRENT_ROUND,
     TIMEOUT,
     FIT_SAMPLES,
     METRICS,
+    PERIOD,
+    CREDENTIAL,
     parameters_to_ndarrays,
     ndarrays_to_parameters,
+    PARTICIPATION,
+    SUBTASK_RETURNS_FAILURES,
+    SUBTASK_RETURNS_RESULTS,
+    SUBTASK_RETURNS_SELECTED,
 )
-from daisyfl.plugin.sec_agg.common.typing import (
+from .common import (
     Proto,
     PROTO_KEY,
     SEC_AGG_PARAM_DICT,
     PUBLIC_KEYS,
     PUBLIC_KEYS_LIST,
     ShareKeysPacket,
     SHARE_KEYS_PACKETS,
     FORWARD_PACKETS,
     ShareRequest,
     SHARE_REQUEST,
     SHARE_RESPONSE,
 )
+from . import primitives
+from daisyfl.operator.base.server_logic import ServerLogic as BaseServerLogic
+from daisyfl.server import Server
+from threading import Event, Condition, Timer
+from daisyfl.server.server import FitResultsAndFailures
 from daisyfl.server.client_proxy import ClientProxy
-from daisyfl.plugin.sec_agg.utils import primitives
-
+from daisyfl.operator.utils import (
+    get_configure_fit,
+    generate_fit_report,
+    wait_for_results,
+    get_clients_from_list,
+)
 from daisyfl.common.logger import log
 
-FitResultsAndFailures = Tuple[List[Tuple[ClientProxy, FitRes]], List[BaseException]]
 
-class Server(BaseServer):
+class ServerLogic(BaseServerLogic):
     """Wrapper which adds SecAgg methods."""
 
     def __init__(
         self,
-        s: BaseServer,
+        server: Server,
+        strategy: Strategy,
     ) -> None:
-        self.server = s
-
-    def disconnect_all_clients(self, timeout: Optional[float]) -> None:
-        """Send shutdown signal to all clients."""
-        self.server.disconnect_all_clients(timeout)
+        self.server: Server = server
+        self.strategy: Strategy = strategy
 
     def fit_round(
         self,
         parameters: Parameters,
         task: Task,
     ) -> Optional[
         Tuple[Optional[Parameters], Optional[Report]]
     ]:
         """Perform a single round fit."""
         # Get clients and their respective instructions from strategy
-        client_instructions = self.server.get_configure_fit(
+        ## credential
+        if CREDENTIAL in task.config:
+            credential = task.config[CREDENTIAL]
+        else:
+            log(ERROR, "\"{}\" is a required key in a Task.".format(CREDENTIAL))
+        ## get_clients
+        client_instructions = get_configure_fit(
+            strategy=self.strategy,
             server_round=task.config[CURRENT_ROUND],
             parameters=parameters,
-            client_manager=self.server.get_client_manager(),
+            server=self.server,
             config=task.config,
+            credential=credential,
         )
 
-        # TODO: stages to APIs
         # === Stage 0: Setup ===
         log(INFO, "SecAgg Stage 0: Setting up Params")
         sec_agg_param_dict = get_sec_agg_param_dict(task,len(client_instructions))
         setup_dict: Dict[int, Tuple[ClientProxy, FitIns]] = \
             initialize_ins_dict(client_instructions)
         setup_dict = set_ins_stage(setup_dict, Proto.SETUP.value)
         setup_dict = set_sec_agg_param_dict(setup_dict, sec_agg_param_dict)
         # pass dummy parameters via gRPC
         setup_dict = set_ins_parameters(setup_dict, Parameters(tensors=[], tensor_type=""))
         client_instructions = client_ins_from_ins_dict(setup_dict)
 
-        results_and_failures: FitResultsAndFailures = self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
         )
-        results = results_and_failures[0]
-        check_num_survivals(results, sec_agg_param_dict)
-        
+        # check
+        current_returns = self.server.get_current_returns(subtask_id)
+        success = wait_for_results(strategy=self.strategy, current_returns=current_returns)
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        # (Optional) drop out metrics
+        selected_num = current_returns.selected
+        # get results and finish subtask
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
+
         # === Stage 1: Ask Public Keys ===
         log(INFO, "SecAgg Stage 1: Asking Keys")
         ask_keys_dict: Dict[int, Tuple[ClientProxy, FitIns]] = \
             next_ins_dict(setup_dict, results)
         ask_keys_dict = set_ins_stage(ask_keys_dict, Proto.ASK_KEYS.value)
         client_instructions = client_ins_from_ins_dict(ask_keys_dict)
+        client_instructions = get_clients_from_list(server=self.server, clients=client_instructions, timeout=3, credential=credential,)
 
-        results_and_failures: FitResultsAndFailures = self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
         )
-        results = results_and_failures[0]
-        check_num_survivals(results, sec_agg_param_dict)
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
 
         # === Stage 2: Share Keys ===
         log(INFO, "SecAgg Stage 2: Sharing Keys")
         share_keys_dict: Dict[int, Tuple[ClientProxy, FitIns]] = \
             next_ins_dict(ask_keys_dict, results)
         share_keys_dict = set_ins_stage(share_keys_dict, Proto.SHARE_KEYS.value)
         share_keys_dict = set_pks_dict(share_keys_dict, results)
         client_instructions = client_ins_from_ins_dict(share_keys_dict)
+        client_instructions = get_clients_from_list(server=self.server, clients=client_instructions, timeout=3, credential=credential,)
 
-        results_and_failures: FitResultsAndFailures = self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
         )
-        results = results_and_failures[0]
-        check_num_survivals(results, sec_agg_param_dict)
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
 
         # === Stage 3: Ask Vectors ===
         log(INFO, "SecAgg Stage 3: Asking Vectors")
         ask_vectors_dict = next_ins_dict(share_keys_dict, results)
         ask_vectors_dict = set_ins_stage(ask_vectors_dict, Proto.ASK_VECTORS.value)
         ask_vectors_dict = set_packet_list(ask_vectors_dict, results)
         # parameters for training
         ask_vectors_dict = set_ins_parameters(ask_vectors_dict, parameters)
         client_instructions = client_ins_from_ins_dict(ask_vectors_dict)
+        client_instructions = get_clients_from_list(server=self.server, clients=client_instructions, timeout=3, credential=credential,)
 
-        results_and_failures: FitResultsAndFailures = self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
         )
-        results = results_and_failures[0]
-        check_num_survivals(results, sec_agg_param_dict)
+        # check
+        success = wait_for_results(strategy=self.strategy, current_returns=self.server.get_current_returns(subtask_id))
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
 
         # === Stage 4: Unmask Vectors ===
         log(INFO, "SecAgg Stage 4: Unmasking Vectors")
         unmask_vectors_dict = next_ins_dict(ask_vectors_dict, results)
         unmask_vectors_dict = set_ins_stage(unmask_vectors_dict, Proto.UNMASK_VECTORS.value)
         masked_vectors, num_examples, metrics = aggregate_fit(results)
         unmask_vectors_dict = set_surviving_info(unmask_vectors_dict, ask_vectors_dict)
         # pass dummy parameters via gRPC
         unmask_vectors_dict = set_ins_parameters(unmask_vectors_dict, Parameters(tensors=[], tensor_type=""))
         client_instructions = client_ins_from_ins_dict(unmask_vectors_dict)
+        client_instructions = get_clients_from_list(server=self.server, clients=client_instructions, timeout=3, credential=credential,)
         
-        results_and_failures: FitResultsAndFailures = self.server.fit_clients(
+        subtask_id = self.server.fit_clients(
             client_instructions=client_instructions,
             max_workers=self.server.get_max_workers(),
             timeout=task.config[TIMEOUT],
         )
-        results = results_and_failures[0]
-        check_num_survivals(results, sec_agg_param_dict)
+        # check
+        current_returns = self.server.get_current_returns(subtask_id)
+        success = wait_for_results(strategy=self.strategy, current_returns=current_returns)
+        if not success:
+            return parameters, generate_fit_report(task.config[CURRENT_ROUND], 0, {},)
+        # (Optional) drop out metrics
+        results_num = current_returns.results_num
+        failures_num = selected_num - results_num
+        # get results and finish subtask
+        results = self.server.get_results(subtask_id)
+        self.server.finish_subtask(subtask_id)
 
         parameters_aggregated = unmask_vector(unmask_vectors_dict, ask_vectors_dict, masked_vectors, results, sec_agg_param_dict)
 
-        # (parameters, num_examples, metrics) -> Parameters, Report
-        report = Report(config={
-            CURRENT_ROUND: task.config[CURRENT_ROUND],
-            FIT_SAMPLES: num_examples,
-            METRICS: metrics,
-        })
+        metrics[PARTICIPATION][SUBTASK_RETURNS_SELECTED] += selected_num
+        metrics[PARTICIPATION][SUBTASK_RETURNS_RESULTS] += results_num
+        metrics[PARTICIPATION][SUBTASK_RETURNS_FAILURES] += failures_num
+        
+        report = generate_fit_report(
+            server_round=task.config[CURRENT_ROUND],
+            samples=num_examples,
+            metrics_aggregated=metrics,
+        )
 
         return parameters_aggregated, report
 
-    def evaluate_round(
-        self, 
-        parameters: Parameters,
-        task: Task,
-    ) -> Optional[Report]:
-        return self.server.evaluate_round(parameters, task)
 
 def set_ins_parameters(
     ins_dict: Dict[int, Tuple[ClientProxy, FitIns]],
     parameters = Parameters,
 ) -> Dict[int, Tuple[ClientProxy, FitIns]]:
     for key, _ in ins_dict.items():
         ins_dict[key][1].parameters = parameters
@@ -233,15 +281,15 @@
 
     if 'threshold' not in sec_agg_param_dict:
         sec_agg_param_dict['threshold'] = max(
             2, int(sec_agg_param_dict['share_num'] * 0.9))
 
     # Maximum number of example trained set to 1000
     if 'max_weights_factor' not in sec_agg_param_dict:
-        sec_agg_param_dict['max_weights_factor'] = 50000
+        sec_agg_param_dict['max_weights_factor'] = 1000
 
     # Quantization parameters
     if 'clipping_range' not in sec_agg_param_dict:
         sec_agg_param_dict['clipping_range'] = 3
 
     if 'target_range' not in sec_agg_param_dict:
         sec_agg_param_dict['target_range'] = 10000
@@ -280,15 +328,15 @@
 
 def next_ins_dict(
     ins_dict: Dict[int, Tuple[ClientProxy, FitIns]],
     results: List[Tuple[ClientProxy, FitRes]],
 ) -> Dict[int, Tuple[ClientProxy, FitIns]]:
     next_ins_dict = {}
     for idx, ins in ins_dict.items():
-        if ins[0] in [result[0] for result in results]:
+        if ins[0].cid in [result[0].cid for result in results]:
             next_ins_dict[idx] = ins
             for i in [
                 SEC_AGG_PARAM_DICT,
                 PUBLIC_KEYS,
                 PUBLIC_KEYS_LIST,
                 SHARE_KEYS_PACKETS,
                 FORWARD_PACKETS,
@@ -302,21 +350,14 @@
     return next_ins_dict
 
 def client_ins_from_ins_dict(
     ins_dict: Dict[int, Tuple[ClientProxy, FitIns]],
 ) -> List[Tuple[ClientProxy, FitIns]]:
     return [ins for _, ins in ins_dict.items()]
 
-def check_num_survivals(
-    results: List[Tuple[ClientProxy, FitRes]],
-    sec_agg_param_dict: Dict,
-) -> None:
-    if len(results) < sec_agg_param_dict['min_num']:
-        raise Exception("Not enough available clients")
-
 def check_enough_shares(
     share_list: List[bytes],
     sec_agg_param_dict: Dict,
 ) -> None:
     if len(share_list) < sec_agg_param_dict['threshold']:
         raise Exception(
             "Not enough shares to recover secret in unmask vectors stage"
@@ -344,29 +385,29 @@
 def set_pks_dict(
     ins_dict: Dict[int, Tuple[ClientProxy, FitIns]],
     results: List[Tuple[ClientProxy, FitRes]],
 ) -> Dict[int, Tuple[ClientProxy, FitIns]]:
     pks_dict = {}
     for result in results:
         for idx, ins in ins_dict.items():    
-            if ins[0] == result[0]:
+            if ins[0].cid == result[0].cid:
                 pks_dict[idx] = result[1].config[PUBLIC_KEYS]
                 break
     for key, _ in ins_dict.items():
         ins_dict[key][1].config[PUBLIC_KEYS_LIST] = pks_dict
 
     return ins_dict
 
 def set_packet_list(
     ins_dict: Dict[int, Tuple[ClientProxy, FitIns]],
     results: List[Tuple[ClientProxy, FitRes]],
 ) -> Dict[int, Tuple[ClientProxy, FitIns]]:
     total_packet_list: List[dict] = []
     for _, ins in ins_dict.items():
-        pos = [result[0] for result in results].index(ins[0])
+        pos = [result[0].cid for result in results].index(ins[0].cid)
         packet_list = results[pos][1].config[SHARE_KEYS_PACKETS]
         total_packet_list += packet_list
     
     for idx, _ in ins_dict.items():
         ins_dict[idx][1].config[FORWARD_PACKETS] = []
 
     for packet in total_packet_list:
@@ -380,24 +421,34 @@
     results: List[Tuple[ClientProxy, FitRes]],
 ) -> Tuple[NDArrays, int, TypedDict]:
     # Get shape of vector sent by first client
     masked_vectors = primitives.weights_zero_generate(
         [i.shape for i in parameters_to_ndarrays(results[0][1].parameters)]
     )
     total_examples = 0
+    participation = {
+        SUBTASK_RETURNS_SELECTED: 0,
+        SUBTASK_RETURNS_RESULTS: 0,
+        SUBTASK_RETURNS_FAILURES: 0,
+    }
     for result in results:
         masked_vectors = primitives.weights_addition(
             masked_vectors, parameters_to_ndarrays(result[1].parameters)
         )
         num_examples = result[1].config[FIT_SAMPLES]
         total_examples = total_examples + num_examples
 
-    avg_examples = int(total_examples / len(results))
+        if result[1].config[METRICS].__contains__(PARTICIPATION):
+            participation[SUBTASK_RETURNS_SELECTED] += result[1].config[METRICS][PARTICIPATION][SUBTASK_RETURNS_SELECTED] - 1
+            participation[SUBTASK_RETURNS_RESULTS] += result[1].config[METRICS][PARTICIPATION][SUBTASK_RETURNS_RESULTS] - 1
+            participation[SUBTASK_RETURNS_FAILURES] += result[1].config[METRICS][PARTICIPATION][SUBTASK_RETURNS_FAILURES]
+
+    avg_examples = int(total_examples)
     
-    return masked_vectors, avg_examples, {}
+    return masked_vectors, avg_examples, {PARTICIPATION: participation}
 
 def set_surviving_info(
     survivals_dict: Dict[int, Tuple[ClientProxy, FitIns]],
     participants_dict: Dict[int, Tuple[ClientProxy, FitIns]],
 ) -> Dict[int, Tuple[ClientProxy, FitIns]]:
     survivals = [idx for idx, _ in survivals_dict.items()]
     dropouts = []
@@ -475,8 +526,8 @@
     )
     total_weights_factor, masked_vectors = primitives.factor_weights_extract(masked_vectors)
     masked_vectors = primitives.weights_divide(masked_vectors, total_weights_factor)
     aggregated_vector = primitives.reverse_quantize(
         masked_vectors, sec_agg_param_dict['clipping_range'], sec_agg_param_dict['target_range']
     )
     aggregated_parameters = ndarrays_to_parameters(aggregated_vector)
-    return aggregated_parameters
+    return aggregated_parameters
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/plugin/sec_agg/utils/primitives.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/primitives.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -297,8 +297,8 @@
 def weights_multiply(a: NDArrays, b: int) -> NDArrays:
     return [a[idx] * b for idx in range(len(a))]
 
 # Divide weight by an integer
 
 
 def weights_divide(a: NDArrays, b: int) -> NDArrays:
-    return [a[idx] / b for idx in range(len(a))]
+    return [a[idx] / b for idx in range(len(a))]
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/proto/__init__.py` & `daisyfl-0.4.5/src/py/daisyfl/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/src/py/daisyfl/proto/transport_pb2.py` & `daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flwr/proto/transport.proto
+# source: daisyfl/proto/transport.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='flwr/proto/transport.proto',
-  package='flwr.proto',
+  name='daisyfl/proto/transport.proto',
+  package='daisyfl.proto',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1a\x66lwr/proto/transport.proto\x12\nflwr.proto\"9\n\x06Status\x12\x1e\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x10.flwr.proto.Code\x12\x0f\n\x07message\x18\x02 \x01(\t\"2\n\nParameters\x12\x0f\n\x07tensors\x18\x01 \x03(\x0c\x12\x13\n\x0btensor_type\x18\x02 \x01(\t\"i\n\x06Scalar\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x42\x08\n\x06scalar\"4\n\tInnerList\x12\'\n\ninner_list\x18\x01 \x03(\x0b\x32\x13.flwr.proto.Element\"\x87\x01\n\x08InnerMap\x12\x35\n\tinner_map\x18\x01 \x03(\x0b\x32\".flwr.proto.InnerMap.InnerMapEntry\x1a\x44\n\rInnerMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.flwr.proto.Element:\x02\x38\x01\"\x97\x01\n\x0bInnerMapInt\x12?\n\rinner_map_int\x18\x01 \x03(\x0b\x32(.flwr.proto.InnerMapInt.InnerMapIntEntry\x1aG\n\x10InnerMapIntEntry\x12\x0b\n\x03key\x18\x01 \x01(\x03\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.flwr.proto.Element:\x02\x38\x01\"\xf5\x01\n\x07\x45lement\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x12)\n\tinner_map\x18\x10 \x01(\x0b\x32\x14.flwr.proto.InnerMapH\x00\x12\x30\n\rinner_map_int\x18\x11 \x01(\x0b\x32\x17.flwr.proto.InnerMapIntH\x00\x12+\n\ninner_list\x18\x12 \x01(\x0b\x32\x15.flwr.proto.InnerListH\x00\x42\t\n\x07\x65lement\"\xfd\x06\n\rServerMessage\x12?\n\rreconnect_ins\x18\x01 \x01(\x0b\x32&.flwr.proto.ServerMessage.ReconnectInsH\x00\x12H\n\x12get_properties_ins\x18\x02 \x01(\x0b\x32*.flwr.proto.ServerMessage.GetPropertiesInsH\x00\x12H\n\x12get_parameters_ins\x18\x03 \x01(\x0b\x32*.flwr.proto.ServerMessage.GetParametersInsH\x00\x12\x33\n\x07\x66it_ins\x18\x04 \x01(\x0b\x32 .flwr.proto.ServerMessage.FitInsH\x00\x12=\n\x0c\x65valuate_ins\x18\x05 \x01(\x0b\x32%.flwr.proto.ServerMessage.EvaluateInsH\x00\x1a\x1f\n\x0cReconnectIns\x12\x0f\n\x07seconds\x18\x01 \x01(\x03\x1a\x9d\x01\n\x10GetPropertiesIns\x12\x46\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x36.flwr.proto.ServerMessage.GetPropertiesIns.ConfigEntry\x1a\x41\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.flwr.proto.Scalar:\x02\x38\x01\x1a\x9d\x01\n\x10GetParametersIns\x12\x46\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x36.flwr.proto.ServerMessage.GetParametersIns.ConfigEntry\x1a\x41\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.flwr.proto.Scalar:\x02\x38\x01\x1aZ\n\x06\x46itIns\x12*\n\nparameters\x18\x01 \x01(\x0b\x32\x16.flwr.proto.Parameters\x12$\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x14.flwr.proto.InnerMap\x1a_\n\x0b\x45valuateIns\x12*\n\nparameters\x18\x01 \x01(\x0b\x32\x16.flwr.proto.Parameters\x12$\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x14.flwr.proto.InnerMapB\x05\n\x03msg\"\xa3\x07\n\rClientMessage\x12\x41\n\x0e\x64isconnect_res\x18\x01 \x01(\x0b\x32\'.flwr.proto.ClientMessage.DisconnectResH\x00\x12H\n\x12get_properties_res\x18\x02 \x01(\x0b\x32*.flwr.proto.ClientMessage.GetPropertiesResH\x00\x12H\n\x12get_parameters_res\x18\x03 \x01(\x0b\x32*.flwr.proto.ClientMessage.GetParametersResH\x00\x12\x33\n\x07\x66it_res\x18\x04 \x01(\x0b\x32 .flwr.proto.ClientMessage.FitResH\x00\x12=\n\x0c\x65valuate_res\x18\x05 \x01(\x0b\x32%.flwr.proto.ClientMessage.EvaluateResH\x00\x1a\x33\n\rDisconnectRes\x12\"\n\x06reason\x18\x01 \x01(\x0e\x32\x12.flwr.proto.Reason\x1a\xcd\x01\n\x10GetPropertiesRes\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.flwr.proto.Status\x12N\n\nproperties\x18\x02 \x03(\x0b\x32:.flwr.proto.ClientMessage.GetPropertiesRes.PropertiesEntry\x1a\x45\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.flwr.proto.Scalar:\x02\x38\x01\x1a\x62\n\x10GetParametersRes\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.flwr.proto.Status\x12*\n\nparameters\x18\x02 \x01(\x0b\x32\x16.flwr.proto.Parameters\x1a~\n\x06\x46itRes\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.flwr.proto.Status\x12*\n\nparameters\x18\x02 \x01(\x0b\x32\x16.flwr.proto.Parameters\x12$\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x14.flwr.proto.InnerMap\x1aW\n\x0b\x45valuateRes\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.flwr.proto.Status\x12$\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x14.flwr.proto.InnerMapB\x05\n\x03msg*\x8d\x01\n\x04\x43ode\x12\x06\n\x02OK\x10\x00\x12\"\n\x1eGET_PROPERTIES_NOT_IMPLEMENTED\x10\x01\x12\"\n\x1eGET_PARAMETERS_NOT_IMPLEMENTED\x10\x02\x12\x17\n\x13\x46IT_NOT_IMPLEMENTED\x10\x03\x12\x1c\n\x18\x45VALUATE_NOT_IMPLEMENTED\x10\x04*[\n\x06Reason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tRECONNECT\x10\x01\x12\x16\n\x12POWER_DISCONNECTED\x10\x02\x12\x14\n\x10WIFI_UNAVAILABLE\x10\x03\x12\x07\n\x03\x41\x43K\x10\x04\x32S\n\rFlowerService\x12\x42\n\x04Join\x12\x19.flwr.proto.ClientMessage\x1a\x19.flwr.proto.ServerMessage\"\x00(\x01\x30\x01\x62\x06proto3'
+  serialized_pb=b'\n\x1d\x64\x61isyfl/proto/transport.proto\x12\rdaisyfl.proto\"<\n\x06Status\x12!\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x13.daisyfl.proto.Code\x12\x0f\n\x07message\x18\x02 \x01(\t\"2\n\nParameters\x12\x0f\n\x07tensors\x18\x01 \x03(\x0c\x12\x13\n\x0btensor_type\x18\x02 \x01(\t\"i\n\x06Scalar\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x42\x08\n\x06scalar\"7\n\tInnerList\x12*\n\ninner_list\x18\x01 \x03(\x0b\x32\x16.daisyfl.proto.Element\"\x8d\x01\n\x08InnerMap\x12\x38\n\tinner_map\x18\x01 \x03(\x0b\x32%.daisyfl.proto.InnerMap.InnerMapEntry\x1aG\n\rInnerMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.daisyfl.proto.Element:\x02\x38\x01\"\x9d\x01\n\x0bInnerMapInt\x12\x42\n\rinner_map_int\x18\x01 \x03(\x0b\x32+.daisyfl.proto.InnerMapInt.InnerMapIntEntry\x1aJ\n\x10InnerMapIntEntry\x12\x0b\n\x03key\x18\x01 \x01(\x03\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.daisyfl.proto.Element:\x02\x38\x01\"\xfe\x01\n\x07\x45lement\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x12,\n\tinner_map\x18\x10 \x01(\x0b\x32\x17.daisyfl.proto.InnerMapH\x00\x12\x33\n\rinner_map_int\x18\x11 \x01(\x0b\x32\x1a.daisyfl.proto.InnerMapIntH\x00\x12.\n\ninner_list\x18\x12 \x01(\x0b\x32\x18.daisyfl.proto.InnerListH\x00\x42\t\n\x07\x65lement\"\xb8\x08\n\rServerMessage\x12\x42\n\rreconnect_ins\x18\x01 \x01(\x0b\x32).daisyfl.proto.ServerMessage.ReconnectInsH\x00\x12K\n\x12get_properties_ins\x18\x02 \x01(\x0b\x32-.daisyfl.proto.ServerMessage.GetPropertiesInsH\x00\x12K\n\x12get_parameters_ins\x18\x03 \x01(\x0b\x32-.daisyfl.proto.ServerMessage.GetParametersInsH\x00\x12\x36\n\x07\x66it_ins\x18\x04 \x01(\x0b\x32#.daisyfl.proto.ServerMessage.FitInsH\x00\x12@\n\x0c\x65valuate_ins\x18\x05 \x01(\x0b\x32(.daisyfl.proto.ServerMessage.EvaluateInsH\x00\x12S\n\x16server_received_signal\x18\x06 \x01(\x0b\x32\x31.daisyfl.proto.ServerMessage.ServerReceivedSignalH\x00\x1a\x1f\n\x0cReconnectIns\x12\x0f\n\x07seconds\x18\x01 \x01(\x03\x1a\xa3\x01\n\x10GetPropertiesIns\x12I\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x39.daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry\x1a\x44\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1a\xa3\x01\n\x10GetParametersIns\x12I\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x39.daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry\x1a\x44\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1a`\n\x06\x46itIns\x12-\n\nparameters\x18\x01 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a\x65\n\x0b\x45valuateIns\x12-\n\nparameters\x18\x01 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a=\n\x14ServerReceivedSignal\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.StatusB\x05\n\x03msg\"\xcc\t\n\rClientMessage\x12\x44\n\x0e\x64isconnect_res\x18\x01 \x01(\x0b\x32*.daisyfl.proto.ClientMessage.DisconnectResH\x00\x12K\n\x12get_properties_res\x18\x02 \x01(\x0b\x32-.daisyfl.proto.ClientMessage.GetPropertiesResH\x00\x12K\n\x12get_parameters_res\x18\x03 \x01(\x0b\x32-.daisyfl.proto.ClientMessage.GetParametersResH\x00\x12\x36\n\x07\x66it_res\x18\x04 \x01(\x0b\x32#.daisyfl.proto.ClientMessage.FitResH\x00\x12@\n\x0c\x65valuate_res\x18\x05 \x01(\x0b\x32(.daisyfl.proto.ClientMessage.EvaluateResH\x00\x12\x42\n\rclient_status\x18\x06 \x01(\x0b\x32).daisyfl.proto.ClientMessage.ClientStatusH\x00\x12S\n\x16\x63lient_received_signal\x18\x07 \x01(\x0b\x32\x31.daisyfl.proto.ClientMessage.ClientReceivedSignalH\x00\x1a\x36\n\rDisconnectRes\x12%\n\x06reason\x18\x01 \x01(\x0e\x32\x15.daisyfl.proto.Reason\x1a\xd6\x01\n\x10GetPropertiesRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12Q\n\nproperties\x18\x02 \x03(\x0b\x32=.daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry\x1aH\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1ah\n\x10GetParametersRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12-\n\nparameters\x18\x02 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x1a\x87\x01\n\x06\x46itRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12-\n\nparameters\x18\x02 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a]\n\x0b\x45valuateRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a\x1e\n\x0c\x43lientStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x1a=\n\x14\x43lientReceivedSignal\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.StatusB\x05\n\x03msg*\x9f\x01\n\x04\x43ode\x12\x06\n\x02OK\x10\x00\x12\"\n\x1eGET_PROPERTIES_NOT_IMPLEMENTED\x10\x01\x12\"\n\x1eGET_PARAMETERS_NOT_IMPLEMENTED\x10\x02\x12\x17\n\x13\x46IT_NOT_IMPLEMENTED\x10\x03\x12\x1c\n\x18\x45VALUATE_NOT_IMPLEMENTED\x10\x04\x12\x10\n\x0cMESSAGE_LOST\x10\x05*[\n\x06Reason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tRECONNECT\x10\x01\x12\x16\n\x12POWER_DISCONNECTED\x10\x02\x12\x14\n\x10WIFI_UNAVAILABLE\x10\x03\x12\x07\n\x03\x41\x43K\x10\x04\x32Y\n\rFlowerService\x12H\n\x04Join\x12\x1c.daisyfl.proto.ClientMessage\x1a\x1c.daisyfl.proto.ServerMessage\"\x00(\x01\x30\x01\x62\x06proto3'
 )
 
 _CODE = _descriptor.EnumDescriptor(
   name='Code',
-  full_name='flwr.proto.Code',
+  full_name='daisyfl.proto.Code',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
       name='OK', index=0, number=0,
       serialized_options=None,
@@ -51,26 +51,31 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='EVALUATE_NOT_IMPLEMENTED', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='MESSAGE_LOST', index=5, number=5,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2685,
-  serialized_end=2826,
+  serialized_start=3202,
+  serialized_end=3361,
 )
 _sym_db.RegisterEnumDescriptor(_CODE)
 
 Code = enum_type_wrapper.EnumTypeWrapper(_CODE)
 _REASON = _descriptor.EnumDescriptor(
   name='Reason',
-  full_name='flwr.proto.Reason',
+  full_name='daisyfl.proto.Reason',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
       name='UNKNOWN', index=0, number=0,
       serialized_options=None,
@@ -95,50 +100,51 @@
       name='ACK', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2828,
-  serialized_end=2919,
+  serialized_start=3363,
+  serialized_end=3454,
 )
 _sym_db.RegisterEnumDescriptor(_REASON)
 
 Reason = enum_type_wrapper.EnumTypeWrapper(_REASON)
 OK = 0
 GET_PROPERTIES_NOT_IMPLEMENTED = 1
 GET_PARAMETERS_NOT_IMPLEMENTED = 2
 FIT_NOT_IMPLEMENTED = 3
 EVALUATE_NOT_IMPLEMENTED = 4
+MESSAGE_LOST = 5
 UNKNOWN = 0
 RECONNECT = 1
 POWER_DISCONNECTED = 2
 WIFI_UNAVAILABLE = 3
 ACK = 4
 
 
 
 _STATUS = _descriptor.Descriptor(
   name='Status',
-  full_name='flwr.proto.Status',
+  full_name='daisyfl.proto.Status',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='code', full_name='flwr.proto.Status.code', index=0,
+      name='code', full_name='daisyfl.proto.Status.code', index=0,
       number=1, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='message', full_name='flwr.proto.Status.message', index=1,
+      name='message', full_name='daisyfl.proto.Status.message', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -148,36 +154,36 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=42,
-  serialized_end=99,
+  serialized_start=48,
+  serialized_end=108,
 )
 
 
 _PARAMETERS = _descriptor.Descriptor(
   name='Parameters',
-  full_name='flwr.proto.Parameters',
+  full_name='daisyfl.proto.Parameters',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='tensors', full_name='flwr.proto.Parameters.tensors', index=0,
+      name='tensors', full_name='daisyfl.proto.Parameters.tensors', index=0,
       number=1, type=12, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='tensor_type', full_name='flwr.proto.Parameters.tensor_type', index=1,
+      name='tensor_type', full_name='daisyfl.proto.Parameters.tensor_type', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -187,57 +193,57 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=101,
-  serialized_end=151,
+  serialized_start=110,
+  serialized_end=160,
 )
 
 
 _SCALAR = _descriptor.Descriptor(
   name='Scalar',
-  full_name='flwr.proto.Scalar',
+  full_name='daisyfl.proto.Scalar',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='double', full_name='flwr.proto.Scalar.double', index=0,
+      name='double', full_name='daisyfl.proto.Scalar.double', index=0,
       number=1, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='sint64', full_name='flwr.proto.Scalar.sint64', index=1,
+      name='sint64', full_name='daisyfl.proto.Scalar.sint64', index=1,
       number=8, type=18, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bool', full_name='flwr.proto.Scalar.bool', index=2,
+      name='bool', full_name='daisyfl.proto.Scalar.bool', index=2,
       number=13, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='string', full_name='flwr.proto.Scalar.string', index=3,
+      name='string', full_name='daisyfl.proto.Scalar.string', index=3,
       number=14, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bytes', full_name='flwr.proto.Scalar.bytes', index=4,
+      name='bytes', full_name='daisyfl.proto.Scalar.bytes', index=4,
       number=15, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=b"",
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -247,34 +253,34 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
-      name='scalar', full_name='flwr.proto.Scalar.scalar',
+      name='scalar', full_name='daisyfl.proto.Scalar.scalar',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=153,
-  serialized_end=258,
+  serialized_start=162,
+  serialized_end=267,
 )
 
 
 _INNERLIST = _descriptor.Descriptor(
   name='InnerList',
-  full_name='flwr.proto.InnerList',
+  full_name='daisyfl.proto.InnerList',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='inner_list', full_name='flwr.proto.InnerList.inner_list', index=0,
+      name='inner_list', full_name='daisyfl.proto.InnerList.inner_list', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -284,36 +290,36 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=260,
-  serialized_end=312,
+  serialized_start=269,
+  serialized_end=324,
 )
 
 
 _INNERMAP_INNERMAPENTRY = _descriptor.Descriptor(
   name='InnerMapEntry',
-  full_name='flwr.proto.InnerMap.InnerMapEntry',
+  full_name='daisyfl.proto.InnerMap.InnerMapEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='flwr.proto.InnerMap.InnerMapEntry.key', index=0,
+      name='key', full_name='daisyfl.proto.InnerMap.InnerMapEntry.key', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='flwr.proto.InnerMap.InnerMapEntry.value', index=1,
+      name='value', full_name='daisyfl.proto.InnerMap.InnerMapEntry.value', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -323,28 +329,28 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=382,
-  serialized_end=450,
+  serialized_start=397,
+  serialized_end=468,
 )
 
 _INNERMAP = _descriptor.Descriptor(
   name='InnerMap',
-  full_name='flwr.proto.InnerMap',
+  full_name='daisyfl.proto.InnerMap',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='inner_map', full_name='flwr.proto.InnerMap.inner_map', index=0,
+      name='inner_map', full_name='daisyfl.proto.InnerMap.inner_map', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -354,36 +360,36 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=315,
-  serialized_end=450,
+  serialized_start=327,
+  serialized_end=468,
 )
 
 
 _INNERMAPINT_INNERMAPINTENTRY = _descriptor.Descriptor(
   name='InnerMapIntEntry',
-  full_name='flwr.proto.InnerMapInt.InnerMapIntEntry',
+  full_name='daisyfl.proto.InnerMapInt.InnerMapIntEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='flwr.proto.InnerMapInt.InnerMapIntEntry.key', index=0,
+      name='key', full_name='daisyfl.proto.InnerMapInt.InnerMapIntEntry.key', index=0,
       number=1, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='flwr.proto.InnerMapInt.InnerMapIntEntry.value', index=1,
+      name='value', full_name='daisyfl.proto.InnerMapInt.InnerMapIntEntry.value', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -393,28 +399,28 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=533,
-  serialized_end=604,
+  serialized_start=554,
+  serialized_end=628,
 )
 
 _INNERMAPINT = _descriptor.Descriptor(
   name='InnerMapInt',
-  full_name='flwr.proto.InnerMapInt',
+  full_name='daisyfl.proto.InnerMapInt',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='inner_map_int', full_name='flwr.proto.InnerMapInt.inner_map_int', index=0,
+      name='inner_map_int', full_name='daisyfl.proto.InnerMapInt.inner_map_int', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -424,78 +430,78 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=453,
-  serialized_end=604,
+  serialized_start=471,
+  serialized_end=628,
 )
 
 
 _ELEMENT = _descriptor.Descriptor(
   name='Element',
-  full_name='flwr.proto.Element',
+  full_name='daisyfl.proto.Element',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='double', full_name='flwr.proto.Element.double', index=0,
+      name='double', full_name='daisyfl.proto.Element.double', index=0,
       number=1, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='sint64', full_name='flwr.proto.Element.sint64', index=1,
+      name='sint64', full_name='daisyfl.proto.Element.sint64', index=1,
       number=8, type=18, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bool', full_name='flwr.proto.Element.bool', index=2,
+      name='bool', full_name='daisyfl.proto.Element.bool', index=2,
       number=13, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='string', full_name='flwr.proto.Element.string', index=3,
+      name='string', full_name='daisyfl.proto.Element.string', index=3,
       number=14, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bytes', full_name='flwr.proto.Element.bytes', index=4,
+      name='bytes', full_name='daisyfl.proto.Element.bytes', index=4,
       number=15, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=b"",
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='inner_map', full_name='flwr.proto.Element.inner_map', index=5,
+      name='inner_map', full_name='daisyfl.proto.Element.inner_map', index=5,
       number=16, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='inner_map_int', full_name='flwr.proto.Element.inner_map_int', index=6,
+      name='inner_map_int', full_name='daisyfl.proto.Element.inner_map_int', index=6,
       number=17, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='inner_list', full_name='flwr.proto.Element.inner_list', index=7,
+      name='inner_list', full_name='daisyfl.proto.Element.inner_list', index=7,
       number=18, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -505,34 +511,34 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
-      name='element', full_name='flwr.proto.Element.element',
+      name='element', full_name='daisyfl.proto.Element.element',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=607,
-  serialized_end=852,
+  serialized_start=631,
+  serialized_end=885,
 )
 
 
 _SERVERMESSAGE_RECONNECTINS = _descriptor.Descriptor(
   name='ReconnectIns',
-  full_name='flwr.proto.ServerMessage.ReconnectIns',
+  full_name='daisyfl.proto.ServerMessage.ReconnectIns',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='seconds', full_name='flwr.proto.ServerMessage.ReconnectIns.seconds', index=0,
+      name='seconds', full_name='daisyfl.proto.ServerMessage.ReconnectIns.seconds', index=0,
       number=1, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -542,35 +548,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1201,
-  serialized_end=1232,
+  serialized_start=1334,
+  serialized_end=1365,
 )
 
 _SERVERMESSAGE_GETPROPERTIESINS_CONFIGENTRY = _descriptor.Descriptor(
   name='ConfigEntry',
-  full_name='flwr.proto.ServerMessage.GetPropertiesIns.ConfigEntry',
+  full_name='daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='flwr.proto.ServerMessage.GetPropertiesIns.ConfigEntry.key', index=0,
+      name='key', full_name='daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry.key', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='flwr.proto.ServerMessage.GetPropertiesIns.ConfigEntry.value', index=1,
+      name='value', full_name='daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry.value', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -580,28 +586,28 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1327,
-  serialized_end=1392,
+  serialized_start=1463,
+  serialized_end=1531,
 )
 
 _SERVERMESSAGE_GETPROPERTIESINS = _descriptor.Descriptor(
   name='GetPropertiesIns',
-  full_name='flwr.proto.ServerMessage.GetPropertiesIns',
+  full_name='daisyfl.proto.ServerMessage.GetPropertiesIns',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ServerMessage.GetPropertiesIns.config', index=0,
+      name='config', full_name='daisyfl.proto.ServerMessage.GetPropertiesIns.config', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -611,35 +617,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1235,
-  serialized_end=1392,
+  serialized_start=1368,
+  serialized_end=1531,
 )
 
 _SERVERMESSAGE_GETPARAMETERSINS_CONFIGENTRY = _descriptor.Descriptor(
   name='ConfigEntry',
-  full_name='flwr.proto.ServerMessage.GetParametersIns.ConfigEntry',
+  full_name='daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='flwr.proto.ServerMessage.GetParametersIns.ConfigEntry.key', index=0,
+      name='key', full_name='daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry.key', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='flwr.proto.ServerMessage.GetParametersIns.ConfigEntry.value', index=1,
+      name='value', full_name='daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry.value', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -649,28 +655,28 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1327,
-  serialized_end=1392,
+  serialized_start=1463,
+  serialized_end=1531,
 )
 
 _SERVERMESSAGE_GETPARAMETERSINS = _descriptor.Descriptor(
   name='GetParametersIns',
-  full_name='flwr.proto.ServerMessage.GetParametersIns',
+  full_name='daisyfl.proto.ServerMessage.GetParametersIns',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ServerMessage.GetParametersIns.config', index=0,
+      name='config', full_name='daisyfl.proto.ServerMessage.GetParametersIns.config', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -680,35 +686,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1395,
-  serialized_end=1552,
+  serialized_start=1534,
+  serialized_end=1697,
 )
 
 _SERVERMESSAGE_FITINS = _descriptor.Descriptor(
   name='FitIns',
-  full_name='flwr.proto.ServerMessage.FitIns',
+  full_name='daisyfl.proto.ServerMessage.FitIns',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='parameters', full_name='flwr.proto.ServerMessage.FitIns.parameters', index=0,
+      name='parameters', full_name='daisyfl.proto.ServerMessage.FitIns.parameters', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ServerMessage.FitIns.config', index=1,
+      name='config', full_name='daisyfl.proto.ServerMessage.FitIns.config', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -718,35 +724,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1554,
-  serialized_end=1644,
+  serialized_start=1699,
+  serialized_end=1795,
 )
 
 _SERVERMESSAGE_EVALUATEINS = _descriptor.Descriptor(
   name='EvaluateIns',
-  full_name='flwr.proto.ServerMessage.EvaluateIns',
+  full_name='daisyfl.proto.ServerMessage.EvaluateIns',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='parameters', full_name='flwr.proto.ServerMessage.EvaluateIns.parameters', index=0,
+      name='parameters', full_name='daisyfl.proto.ServerMessage.EvaluateIns.parameters', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ServerMessage.EvaluateIns.config', index=1,
+      name='config', full_name='daisyfl.proto.ServerMessage.EvaluateIns.config', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -756,93 +762,131 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1646,
-  serialized_end=1741,
+  serialized_start=1797,
+  serialized_end=1898,
+)
+
+_SERVERMESSAGE_SERVERRECEIVEDSIGNAL = _descriptor.Descriptor(
+  name='ServerReceivedSignal',
+  full_name='daisyfl.proto.ServerMessage.ServerReceivedSignal',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='status', full_name='daisyfl.proto.ServerMessage.ServerReceivedSignal.status', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1900,
+  serialized_end=1961,
 )
 
 _SERVERMESSAGE = _descriptor.Descriptor(
   name='ServerMessage',
-  full_name='flwr.proto.ServerMessage',
+  full_name='daisyfl.proto.ServerMessage',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='reconnect_ins', full_name='flwr.proto.ServerMessage.reconnect_ins', index=0,
+      name='reconnect_ins', full_name='daisyfl.proto.ServerMessage.reconnect_ins', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='get_properties_ins', full_name='flwr.proto.ServerMessage.get_properties_ins', index=1,
+      name='get_properties_ins', full_name='daisyfl.proto.ServerMessage.get_properties_ins', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='get_parameters_ins', full_name='flwr.proto.ServerMessage.get_parameters_ins', index=2,
+      name='get_parameters_ins', full_name='daisyfl.proto.ServerMessage.get_parameters_ins', index=2,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='fit_ins', full_name='flwr.proto.ServerMessage.fit_ins', index=3,
+      name='fit_ins', full_name='daisyfl.proto.ServerMessage.fit_ins', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='evaluate_ins', full_name='flwr.proto.ServerMessage.evaluate_ins', index=4,
+      name='evaluate_ins', full_name='daisyfl.proto.ServerMessage.evaluate_ins', index=4,
       number=5, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='server_received_signal', full_name='daisyfl.proto.ServerMessage.server_received_signal', index=5,
+      number=6, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_SERVERMESSAGE_RECONNECTINS, _SERVERMESSAGE_GETPROPERTIESINS, _SERVERMESSAGE_GETPARAMETERSINS, _SERVERMESSAGE_FITINS, _SERVERMESSAGE_EVALUATEINS, ],
+  nested_types=[_SERVERMESSAGE_RECONNECTINS, _SERVERMESSAGE_GETPROPERTIESINS, _SERVERMESSAGE_GETPARAMETERSINS, _SERVERMESSAGE_FITINS, _SERVERMESSAGE_EVALUATEINS, _SERVERMESSAGE_SERVERRECEIVEDSIGNAL, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
-      name='msg', full_name='flwr.proto.ServerMessage.msg',
+      name='msg', full_name='daisyfl.proto.ServerMessage.msg',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=855,
-  serialized_end=1748,
+  serialized_start=888,
+  serialized_end=1968,
 )
 
 
 _CLIENTMESSAGE_DISCONNECTRES = _descriptor.Descriptor(
   name='DisconnectRes',
-  full_name='flwr.proto.ClientMessage.DisconnectRes',
+  full_name='daisyfl.proto.ClientMessage.DisconnectRes',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='reason', full_name='flwr.proto.ClientMessage.DisconnectRes.reason', index=0,
+      name='reason', full_name='daisyfl.proto.ClientMessage.DisconnectRes.reason', index=0,
       number=1, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -852,35 +896,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2099,
-  serialized_end=2150,
+  serialized_start=2487,
+  serialized_end=2541,
 )
 
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY = _descriptor.Descriptor(
   name='PropertiesEntry',
-  full_name='flwr.proto.ClientMessage.GetPropertiesRes.PropertiesEntry',
+  full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='flwr.proto.ClientMessage.GetPropertiesRes.PropertiesEntry.key', index=0,
+      name='key', full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry.key', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='flwr.proto.ClientMessage.GetPropertiesRes.PropertiesEntry.value', index=1,
+      name='value', full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry.value', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -890,35 +934,35 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2289,
-  serialized_end=2358,
+  serialized_start=2686,
+  serialized_end=2758,
 )
 
 _CLIENTMESSAGE_GETPROPERTIESRES = _descriptor.Descriptor(
   name='GetPropertiesRes',
-  full_name='flwr.proto.ClientMessage.GetPropertiesRes',
+  full_name='daisyfl.proto.ClientMessage.GetPropertiesRes',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='status', full_name='flwr.proto.ClientMessage.GetPropertiesRes.status', index=0,
+      name='status', full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.status', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='properties', full_name='flwr.proto.ClientMessage.GetPropertiesRes.properties', index=1,
+      name='properties', full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.properties', index=1,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -928,35 +972,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2153,
-  serialized_end=2358,
+  serialized_start=2544,
+  serialized_end=2758,
 )
 
 _CLIENTMESSAGE_GETPARAMETERSRES = _descriptor.Descriptor(
   name='GetParametersRes',
-  full_name='flwr.proto.ClientMessage.GetParametersRes',
+  full_name='daisyfl.proto.ClientMessage.GetParametersRes',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='status', full_name='flwr.proto.ClientMessage.GetParametersRes.status', index=0,
+      name='status', full_name='daisyfl.proto.ClientMessage.GetParametersRes.status', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='parameters', full_name='flwr.proto.ClientMessage.GetParametersRes.parameters', index=1,
+      name='parameters', full_name='daisyfl.proto.ClientMessage.GetParametersRes.parameters', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -966,42 +1010,42 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2360,
-  serialized_end=2458,
+  serialized_start=2760,
+  serialized_end=2864,
 )
 
 _CLIENTMESSAGE_FITRES = _descriptor.Descriptor(
   name='FitRes',
-  full_name='flwr.proto.ClientMessage.FitRes',
+  full_name='daisyfl.proto.ClientMessage.FitRes',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='status', full_name='flwr.proto.ClientMessage.FitRes.status', index=0,
+      name='status', full_name='daisyfl.proto.ClientMessage.FitRes.status', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='parameters', full_name='flwr.proto.ClientMessage.FitRes.parameters', index=1,
+      name='parameters', full_name='daisyfl.proto.ClientMessage.FitRes.parameters', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ClientMessage.FitRes.config', index=2,
+      name='config', full_name='daisyfl.proto.ClientMessage.FitRes.config', index=2,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -1011,35 +1055,35 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2460,
-  serialized_end=2586,
+  serialized_start=2867,
+  serialized_end=3002,
 )
 
 _CLIENTMESSAGE_EVALUATERES = _descriptor.Descriptor(
   name='EvaluateRes',
-  full_name='flwr.proto.ClientMessage.EvaluateRes',
+  full_name='daisyfl.proto.ClientMessage.EvaluateRes',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='status', full_name='flwr.proto.ClientMessage.EvaluateRes.status', index=0,
+      name='status', full_name='daisyfl.proto.ClientMessage.EvaluateRes.status', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='config', full_name='flwr.proto.ClientMessage.EvaluateRes.config', index=1,
+      name='config', full_name='daisyfl.proto.ClientMessage.EvaluateRes.config', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -1049,80 +1093,156 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2588,
-  serialized_end=2675,
+  serialized_start=3004,
+  serialized_end=3097,
+)
+
+_CLIENTMESSAGE_CLIENTSTATUS = _descriptor.Descriptor(
+  name='ClientStatus',
+  full_name='daisyfl.proto.ClientMessage.ClientStatus',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='status', full_name='daisyfl.proto.ClientMessage.ClientStatus.status', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3099,
+  serialized_end=3129,
+)
+
+_CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL = _descriptor.Descriptor(
+  name='ClientReceivedSignal',
+  full_name='daisyfl.proto.ClientMessage.ClientReceivedSignal',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='status', full_name='daisyfl.proto.ClientMessage.ClientReceivedSignal.status', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3131,
+  serialized_end=3192,
 )
 
 _CLIENTMESSAGE = _descriptor.Descriptor(
   name='ClientMessage',
-  full_name='flwr.proto.ClientMessage',
+  full_name='daisyfl.proto.ClientMessage',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='disconnect_res', full_name='flwr.proto.ClientMessage.disconnect_res', index=0,
+      name='disconnect_res', full_name='daisyfl.proto.ClientMessage.disconnect_res', index=0,
       number=1, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='get_properties_res', full_name='flwr.proto.ClientMessage.get_properties_res', index=1,
+      name='get_properties_res', full_name='daisyfl.proto.ClientMessage.get_properties_res', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='get_parameters_res', full_name='flwr.proto.ClientMessage.get_parameters_res', index=2,
+      name='get_parameters_res', full_name='daisyfl.proto.ClientMessage.get_parameters_res', index=2,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='fit_res', full_name='flwr.proto.ClientMessage.fit_res', index=3,
+      name='fit_res', full_name='daisyfl.proto.ClientMessage.fit_res', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='evaluate_res', full_name='flwr.proto.ClientMessage.evaluate_res', index=4,
+      name='evaluate_res', full_name='daisyfl.proto.ClientMessage.evaluate_res', index=4,
       number=5, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='client_status', full_name='daisyfl.proto.ClientMessage.client_status', index=5,
+      number=6, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='client_received_signal', full_name='daisyfl.proto.ClientMessage.client_received_signal', index=6,
+      number=7, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_CLIENTMESSAGE_DISCONNECTRES, _CLIENTMESSAGE_GETPROPERTIESRES, _CLIENTMESSAGE_GETPARAMETERSRES, _CLIENTMESSAGE_FITRES, _CLIENTMESSAGE_EVALUATERES, ],
+  nested_types=[_CLIENTMESSAGE_DISCONNECTRES, _CLIENTMESSAGE_GETPROPERTIESRES, _CLIENTMESSAGE_GETPARAMETERSRES, _CLIENTMESSAGE_FITRES, _CLIENTMESSAGE_EVALUATERES, _CLIENTMESSAGE_CLIENTSTATUS, _CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
-      name='msg', full_name='flwr.proto.ClientMessage.msg',
+      name='msg', full_name='daisyfl.proto.ClientMessage.msg',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=1751,
-  serialized_end=2682,
+  serialized_start=1971,
+  serialized_end=3199,
 )
 
 _STATUS.fields_by_name['code'].enum_type = _CODE
 _SCALAR.oneofs_by_name['scalar'].fields.append(
   _SCALAR.fields_by_name['double'])
 _SCALAR.fields_by_name['double'].containing_oneof = _SCALAR.oneofs_by_name['scalar']
 _SCALAR.oneofs_by_name['scalar'].fields.append(
@@ -1182,19 +1302,22 @@
 _SERVERMESSAGE_GETPARAMETERSINS.containing_type = _SERVERMESSAGE
 _SERVERMESSAGE_FITINS.fields_by_name['parameters'].message_type = _PARAMETERS
 _SERVERMESSAGE_FITINS.fields_by_name['config'].message_type = _INNERMAP
 _SERVERMESSAGE_FITINS.containing_type = _SERVERMESSAGE
 _SERVERMESSAGE_EVALUATEINS.fields_by_name['parameters'].message_type = _PARAMETERS
 _SERVERMESSAGE_EVALUATEINS.fields_by_name['config'].message_type = _INNERMAP
 _SERVERMESSAGE_EVALUATEINS.containing_type = _SERVERMESSAGE
+_SERVERMESSAGE_SERVERRECEIVEDSIGNAL.fields_by_name['status'].message_type = _STATUS
+_SERVERMESSAGE_SERVERRECEIVEDSIGNAL.containing_type = _SERVERMESSAGE
 _SERVERMESSAGE.fields_by_name['reconnect_ins'].message_type = _SERVERMESSAGE_RECONNECTINS
 _SERVERMESSAGE.fields_by_name['get_properties_ins'].message_type = _SERVERMESSAGE_GETPROPERTIESINS
 _SERVERMESSAGE.fields_by_name['get_parameters_ins'].message_type = _SERVERMESSAGE_GETPARAMETERSINS
 _SERVERMESSAGE.fields_by_name['fit_ins'].message_type = _SERVERMESSAGE_FITINS
 _SERVERMESSAGE.fields_by_name['evaluate_ins'].message_type = _SERVERMESSAGE_EVALUATEINS
+_SERVERMESSAGE.fields_by_name['server_received_signal'].message_type = _SERVERMESSAGE_SERVERRECEIVEDSIGNAL
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['reconnect_ins'])
 _SERVERMESSAGE.fields_by_name['reconnect_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['get_properties_ins'])
 _SERVERMESSAGE.fields_by_name['get_properties_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
@@ -1202,14 +1325,17 @@
 _SERVERMESSAGE.fields_by_name['get_parameters_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['fit_ins'])
 _SERVERMESSAGE.fields_by_name['fit_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['evaluate_ins'])
 _SERVERMESSAGE.fields_by_name['evaluate_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
+_SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
+  _SERVERMESSAGE.fields_by_name['server_received_signal'])
+_SERVERMESSAGE.fields_by_name['server_received_signal'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE_DISCONNECTRES.fields_by_name['reason'].enum_type = _REASON
 _CLIENTMESSAGE_DISCONNECTRES.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY.fields_by_name['value'].message_type = _SCALAR
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY.containing_type = _CLIENTMESSAGE_GETPROPERTIESRES
 _CLIENTMESSAGE_GETPROPERTIESRES.fields_by_name['status'].message_type = _STATUS
 _CLIENTMESSAGE_GETPROPERTIESRES.fields_by_name['properties'].message_type = _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY
 _CLIENTMESSAGE_GETPROPERTIESRES.containing_type = _CLIENTMESSAGE
@@ -1219,19 +1345,24 @@
 _CLIENTMESSAGE_FITRES.fields_by_name['status'].message_type = _STATUS
 _CLIENTMESSAGE_FITRES.fields_by_name['parameters'].message_type = _PARAMETERS
 _CLIENTMESSAGE_FITRES.fields_by_name['config'].message_type = _INNERMAP
 _CLIENTMESSAGE_FITRES.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE_EVALUATERES.fields_by_name['status'].message_type = _STATUS
 _CLIENTMESSAGE_EVALUATERES.fields_by_name['config'].message_type = _INNERMAP
 _CLIENTMESSAGE_EVALUATERES.containing_type = _CLIENTMESSAGE
+_CLIENTMESSAGE_CLIENTSTATUS.containing_type = _CLIENTMESSAGE
+_CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL.fields_by_name['status'].message_type = _STATUS
+_CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE.fields_by_name['disconnect_res'].message_type = _CLIENTMESSAGE_DISCONNECTRES
 _CLIENTMESSAGE.fields_by_name['get_properties_res'].message_type = _CLIENTMESSAGE_GETPROPERTIESRES
 _CLIENTMESSAGE.fields_by_name['get_parameters_res'].message_type = _CLIENTMESSAGE_GETPARAMETERSRES
 _CLIENTMESSAGE.fields_by_name['fit_res'].message_type = _CLIENTMESSAGE_FITRES
 _CLIENTMESSAGE.fields_by_name['evaluate_res'].message_type = _CLIENTMESSAGE_EVALUATERES
+_CLIENTMESSAGE.fields_by_name['client_status'].message_type = _CLIENTMESSAGE_CLIENTSTATUS
+_CLIENTMESSAGE.fields_by_name['client_received_signal'].message_type = _CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['disconnect_res'])
 _CLIENTMESSAGE.fields_by_name['disconnect_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['get_properties_res'])
 _CLIENTMESSAGE.fields_by_name['get_properties_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
@@ -1239,14 +1370,20 @@
 _CLIENTMESSAGE.fields_by_name['get_parameters_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['fit_res'])
 _CLIENTMESSAGE.fields_by_name['fit_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['evaluate_res'])
 _CLIENTMESSAGE.fields_by_name['evaluate_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
+_CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
+  _CLIENTMESSAGE.fields_by_name['client_status'])
+_CLIENTMESSAGE.fields_by_name['client_status'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
+_CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
+  _CLIENTMESSAGE.fields_by_name['client_received_signal'])
+_CLIENTMESSAGE.fields_by_name['client_received_signal'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 DESCRIPTOR.message_types_by_name['Status'] = _STATUS
 DESCRIPTOR.message_types_by_name['Parameters'] = _PARAMETERS
 DESCRIPTOR.message_types_by_name['Scalar'] = _SCALAR
 DESCRIPTOR.message_types_by_name['InnerList'] = _INNERLIST
 DESCRIPTOR.message_types_by_name['InnerMap'] = _INNERMAP
 DESCRIPTOR.message_types_by_name['InnerMapInt'] = _INNERMAPINT
 DESCRIPTOR.message_types_by_name['Element'] = _ELEMENT
@@ -1254,215 +1391,239 @@
 DESCRIPTOR.message_types_by_name['ClientMessage'] = _CLIENTMESSAGE
 DESCRIPTOR.enum_types_by_name['Code'] = _CODE
 DESCRIPTOR.enum_types_by_name['Reason'] = _REASON
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Status = _reflection.GeneratedProtocolMessageType('Status', (_message.Message,), {
   'DESCRIPTOR' : _STATUS,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.Status)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.Status)
   })
 _sym_db.RegisterMessage(Status)
 
 Parameters = _reflection.GeneratedProtocolMessageType('Parameters', (_message.Message,), {
   'DESCRIPTOR' : _PARAMETERS,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.Parameters)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.Parameters)
   })
 _sym_db.RegisterMessage(Parameters)
 
 Scalar = _reflection.GeneratedProtocolMessageType('Scalar', (_message.Message,), {
   'DESCRIPTOR' : _SCALAR,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.Scalar)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.Scalar)
   })
 _sym_db.RegisterMessage(Scalar)
 
 InnerList = _reflection.GeneratedProtocolMessageType('InnerList', (_message.Message,), {
   'DESCRIPTOR' : _INNERLIST,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.InnerList)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.InnerList)
   })
 _sym_db.RegisterMessage(InnerList)
 
 InnerMap = _reflection.GeneratedProtocolMessageType('InnerMap', (_message.Message,), {
 
   'InnerMapEntry' : _reflection.GeneratedProtocolMessageType('InnerMapEntry', (_message.Message,), {
     'DESCRIPTOR' : _INNERMAP_INNERMAPENTRY,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.InnerMap.InnerMapEntry)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.InnerMap.InnerMapEntry)
     })
   ,
   'DESCRIPTOR' : _INNERMAP,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.InnerMap)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.InnerMap)
   })
 _sym_db.RegisterMessage(InnerMap)
 _sym_db.RegisterMessage(InnerMap.InnerMapEntry)
 
 InnerMapInt = _reflection.GeneratedProtocolMessageType('InnerMapInt', (_message.Message,), {
 
   'InnerMapIntEntry' : _reflection.GeneratedProtocolMessageType('InnerMapIntEntry', (_message.Message,), {
     'DESCRIPTOR' : _INNERMAPINT_INNERMAPINTENTRY,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.InnerMapInt.InnerMapIntEntry)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.InnerMapInt.InnerMapIntEntry)
     })
   ,
   'DESCRIPTOR' : _INNERMAPINT,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.InnerMapInt)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.InnerMapInt)
   })
 _sym_db.RegisterMessage(InnerMapInt)
 _sym_db.RegisterMessage(InnerMapInt.InnerMapIntEntry)
 
 Element = _reflection.GeneratedProtocolMessageType('Element', (_message.Message,), {
   'DESCRIPTOR' : _ELEMENT,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.Element)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.Element)
   })
 _sym_db.RegisterMessage(Element)
 
 ServerMessage = _reflection.GeneratedProtocolMessageType('ServerMessage', (_message.Message,), {
 
   'ReconnectIns' : _reflection.GeneratedProtocolMessageType('ReconnectIns', (_message.Message,), {
     'DESCRIPTOR' : _SERVERMESSAGE_RECONNECTINS,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.ReconnectIns)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.ReconnectIns)
     })
   ,
 
   'GetPropertiesIns' : _reflection.GeneratedProtocolMessageType('GetPropertiesIns', (_message.Message,), {
 
     'ConfigEntry' : _reflection.GeneratedProtocolMessageType('ConfigEntry', (_message.Message,), {
       'DESCRIPTOR' : _SERVERMESSAGE_GETPROPERTIESINS_CONFIGENTRY,
-      '__module__' : 'flwr.proto.transport_pb2'
-      # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.GetPropertiesIns.ConfigEntry)
+      '__module__' : 'daisyfl.proto.transport_pb2'
+      # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry)
       })
     ,
     'DESCRIPTOR' : _SERVERMESSAGE_GETPROPERTIESINS,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.GetPropertiesIns)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.GetPropertiesIns)
     })
   ,
 
   'GetParametersIns' : _reflection.GeneratedProtocolMessageType('GetParametersIns', (_message.Message,), {
 
     'ConfigEntry' : _reflection.GeneratedProtocolMessageType('ConfigEntry', (_message.Message,), {
       'DESCRIPTOR' : _SERVERMESSAGE_GETPARAMETERSINS_CONFIGENTRY,
-      '__module__' : 'flwr.proto.transport_pb2'
-      # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.GetParametersIns.ConfigEntry)
+      '__module__' : 'daisyfl.proto.transport_pb2'
+      # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry)
       })
     ,
     'DESCRIPTOR' : _SERVERMESSAGE_GETPARAMETERSINS,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.GetParametersIns)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.GetParametersIns)
     })
   ,
 
   'FitIns' : _reflection.GeneratedProtocolMessageType('FitIns', (_message.Message,), {
     'DESCRIPTOR' : _SERVERMESSAGE_FITINS,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.FitIns)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.FitIns)
     })
   ,
 
   'EvaluateIns' : _reflection.GeneratedProtocolMessageType('EvaluateIns', (_message.Message,), {
     'DESCRIPTOR' : _SERVERMESSAGE_EVALUATEINS,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage.EvaluateIns)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.EvaluateIns)
+    })
+  ,
+
+  'ServerReceivedSignal' : _reflection.GeneratedProtocolMessageType('ServerReceivedSignal', (_message.Message,), {
+    'DESCRIPTOR' : _SERVERMESSAGE_SERVERRECEIVEDSIGNAL,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.ServerReceivedSignal)
     })
   ,
   'DESCRIPTOR' : _SERVERMESSAGE,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.ServerMessage)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage)
   })
 _sym_db.RegisterMessage(ServerMessage)
 _sym_db.RegisterMessage(ServerMessage.ReconnectIns)
 _sym_db.RegisterMessage(ServerMessage.GetPropertiesIns)
 _sym_db.RegisterMessage(ServerMessage.GetPropertiesIns.ConfigEntry)
 _sym_db.RegisterMessage(ServerMessage.GetParametersIns)
 _sym_db.RegisterMessage(ServerMessage.GetParametersIns.ConfigEntry)
 _sym_db.RegisterMessage(ServerMessage.FitIns)
 _sym_db.RegisterMessage(ServerMessage.EvaluateIns)
+_sym_db.RegisterMessage(ServerMessage.ServerReceivedSignal)
 
 ClientMessage = _reflection.GeneratedProtocolMessageType('ClientMessage', (_message.Message,), {
 
   'DisconnectRes' : _reflection.GeneratedProtocolMessageType('DisconnectRes', (_message.Message,), {
     'DESCRIPTOR' : _CLIENTMESSAGE_DISCONNECTRES,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.DisconnectRes)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.DisconnectRes)
     })
   ,
 
   'GetPropertiesRes' : _reflection.GeneratedProtocolMessageType('GetPropertiesRes', (_message.Message,), {
 
     'PropertiesEntry' : _reflection.GeneratedProtocolMessageType('PropertiesEntry', (_message.Message,), {
       'DESCRIPTOR' : _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY,
-      '__module__' : 'flwr.proto.transport_pb2'
-      # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.GetPropertiesRes.PropertiesEntry)
+      '__module__' : 'daisyfl.proto.transport_pb2'
+      # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry)
       })
     ,
     'DESCRIPTOR' : _CLIENTMESSAGE_GETPROPERTIESRES,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.GetPropertiesRes)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.GetPropertiesRes)
     })
   ,
 
   'GetParametersRes' : _reflection.GeneratedProtocolMessageType('GetParametersRes', (_message.Message,), {
     'DESCRIPTOR' : _CLIENTMESSAGE_GETPARAMETERSRES,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.GetParametersRes)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.GetParametersRes)
     })
   ,
 
   'FitRes' : _reflection.GeneratedProtocolMessageType('FitRes', (_message.Message,), {
     'DESCRIPTOR' : _CLIENTMESSAGE_FITRES,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.FitRes)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.FitRes)
     })
   ,
 
   'EvaluateRes' : _reflection.GeneratedProtocolMessageType('EvaluateRes', (_message.Message,), {
     'DESCRIPTOR' : _CLIENTMESSAGE_EVALUATERES,
-    '__module__' : 'flwr.proto.transport_pb2'
-    # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage.EvaluateRes)
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.EvaluateRes)
+    })
+  ,
+
+  'ClientStatus' : _reflection.GeneratedProtocolMessageType('ClientStatus', (_message.Message,), {
+    'DESCRIPTOR' : _CLIENTMESSAGE_CLIENTSTATUS,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.ClientStatus)
+    })
+  ,
+
+  'ClientReceivedSignal' : _reflection.GeneratedProtocolMessageType('ClientReceivedSignal', (_message.Message,), {
+    'DESCRIPTOR' : _CLIENTMESSAGE_CLIENTRECEIVEDSIGNAL,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.ClientReceivedSignal)
     })
   ,
   'DESCRIPTOR' : _CLIENTMESSAGE,
-  '__module__' : 'flwr.proto.transport_pb2'
-  # @@protoc_insertion_point(class_scope:flwr.proto.ClientMessage)
+  '__module__' : 'daisyfl.proto.transport_pb2'
+  # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage)
   })
 _sym_db.RegisterMessage(ClientMessage)
 _sym_db.RegisterMessage(ClientMessage.DisconnectRes)
 _sym_db.RegisterMessage(ClientMessage.GetPropertiesRes)
 _sym_db.RegisterMessage(ClientMessage.GetPropertiesRes.PropertiesEntry)
 _sym_db.RegisterMessage(ClientMessage.GetParametersRes)
 _sym_db.RegisterMessage(ClientMessage.FitRes)
 _sym_db.RegisterMessage(ClientMessage.EvaluateRes)
+_sym_db.RegisterMessage(ClientMessage.ClientStatus)
+_sym_db.RegisterMessage(ClientMessage.ClientReceivedSignal)
 
 
 _INNERMAP_INNERMAPENTRY._options = None
 _INNERMAPINT_INNERMAPINTENTRY._options = None
 _SERVERMESSAGE_GETPROPERTIESINS_CONFIGENTRY._options = None
 _SERVERMESSAGE_GETPARAMETERSINS_CONFIGENTRY._options = None
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY._options = None
 
 _FLOWERSERVICE = _descriptor.ServiceDescriptor(
   name='FlowerService',
-  full_name='flwr.proto.FlowerService',
+  full_name='daisyfl.proto.FlowerService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=2921,
-  serialized_end=3004,
+  serialized_start=3456,
+  serialized_end=3545,
   methods=[
   _descriptor.MethodDescriptor(
     name='Join',
-    full_name='flwr.proto.FlowerService.Join',
+    full_name='daisyfl.proto.FlowerService.Join',
     index=0,
     containing_service=None,
     input_type=_CLIENTMESSAGE,
     output_type=_SERVERMESSAGE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/proto/transport_pb2.pyi` & `daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 class _CodeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Code.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     OK: _Code.ValueType  # 0
     GET_PROPERTIES_NOT_IMPLEMENTED: _Code.ValueType  # 1
     GET_PARAMETERS_NOT_IMPLEMENTED: _Code.ValueType  # 2
     FIT_NOT_IMPLEMENTED: _Code.ValueType  # 3
     EVALUATE_NOT_IMPLEMENTED: _Code.ValueType  # 4
+    MESSAGE_LOST: _Code.ValueType  # 5
 class Code(_Code, metaclass=_CodeEnumTypeWrapper):
     pass
 
 OK: Code.ValueType  # 0
 GET_PROPERTIES_NOT_IMPLEMENTED: Code.ValueType  # 1
 GET_PARAMETERS_NOT_IMPLEMENTED: Code.ValueType  # 2
 FIT_NOT_IMPLEMENTED: Code.ValueType  # 3
 EVALUATE_NOT_IMPLEMENTED: Code.ValueType  # 4
+MESSAGE_LOST: Code.ValueType  # 5
 global___Code = Code
 
 
 class _Reason:
     ValueType = typing.NewType('ValueType', builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 class _ReasonEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Reason.ValueType], builtins.type):
@@ -331,40 +333,56 @@
             *,
             parameters: typing.Optional[global___Parameters] = ...,
             config: typing.Optional[global___InnerMap] = ...,
             ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["config",b"config","parameters",b"parameters"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["config",b"config","parameters",b"parameters"]) -> None: ...
 
+    class ServerReceivedSignal(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        STATUS_FIELD_NUMBER: builtins.int
+        @property
+        def status(self) -> global___Status: ...
+        def __init__(self,
+            *,
+            status: typing.Optional[global___Status] = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["status",b"status"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
+
     RECONNECT_INS_FIELD_NUMBER: builtins.int
     GET_PROPERTIES_INS_FIELD_NUMBER: builtins.int
     GET_PARAMETERS_INS_FIELD_NUMBER: builtins.int
     FIT_INS_FIELD_NUMBER: builtins.int
     EVALUATE_INS_FIELD_NUMBER: builtins.int
+    SERVER_RECEIVED_SIGNAL_FIELD_NUMBER: builtins.int
     @property
     def reconnect_ins(self) -> global___ServerMessage.ReconnectIns: ...
     @property
     def get_properties_ins(self) -> global___ServerMessage.GetPropertiesIns: ...
     @property
     def get_parameters_ins(self) -> global___ServerMessage.GetParametersIns: ...
     @property
     def fit_ins(self) -> global___ServerMessage.FitIns: ...
     @property
     def evaluate_ins(self) -> global___ServerMessage.EvaluateIns: ...
+    @property
+    def server_received_signal(self) -> global___ServerMessage.ServerReceivedSignal: ...
     def __init__(self,
         *,
         reconnect_ins: typing.Optional[global___ServerMessage.ReconnectIns] = ...,
         get_properties_ins: typing.Optional[global___ServerMessage.GetPropertiesIns] = ...,
         get_parameters_ins: typing.Optional[global___ServerMessage.GetParametersIns] = ...,
         fit_ins: typing.Optional[global___ServerMessage.FitIns] = ...,
         evaluate_ins: typing.Optional[global___ServerMessage.EvaluateIns] = ...,
+        server_received_signal: typing.Optional[global___ServerMessage.ServerReceivedSignal] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["reconnect_ins","get_properties_ins","get_parameters_ins","fit_ins","evaluate_ins"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins","server_received_signal",b"server_received_signal"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins","server_received_signal",b"server_received_signal"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["reconnect_ins","get_properties_ins","get_parameters_ins","fit_ins","evaluate_ins","server_received_signal"]]: ...
 global___ServerMessage = ServerMessage
 
 class ClientMessage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     class DisconnectRes(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
         REASON_FIELD_NUMBER: builtins.int
@@ -454,34 +472,64 @@
             *,
             status: typing.Optional[global___Status] = ...,
             config: typing.Optional[global___InnerMap] = ...,
             ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["config",b"config","status",b"status"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["config",b"config","status",b"status"]) -> None: ...
 
+    class ClientStatus(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        STATUS_FIELD_NUMBER: builtins.int
+        status: typing.Text
+        def __init__(self,
+            *,
+            status: typing.Text = ...,
+            ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
+
+    class ClientReceivedSignal(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        STATUS_FIELD_NUMBER: builtins.int
+        @property
+        def status(self) -> global___Status: ...
+        def __init__(self,
+            *,
+            status: typing.Optional[global___Status] = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["status",b"status"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
+
     DISCONNECT_RES_FIELD_NUMBER: builtins.int
     GET_PROPERTIES_RES_FIELD_NUMBER: builtins.int
     GET_PARAMETERS_RES_FIELD_NUMBER: builtins.int
     FIT_RES_FIELD_NUMBER: builtins.int
     EVALUATE_RES_FIELD_NUMBER: builtins.int
+    CLIENT_STATUS_FIELD_NUMBER: builtins.int
+    CLIENT_RECEIVED_SIGNAL_FIELD_NUMBER: builtins.int
     @property
     def disconnect_res(self) -> global___ClientMessage.DisconnectRes: ...
     @property
     def get_properties_res(self) -> global___ClientMessage.GetPropertiesRes: ...
     @property
     def get_parameters_res(self) -> global___ClientMessage.GetParametersRes: ...
     @property
     def fit_res(self) -> global___ClientMessage.FitRes: ...
     @property
     def evaluate_res(self) -> global___ClientMessage.EvaluateRes: ...
+    @property
+    def client_status(self) -> global___ClientMessage.ClientStatus: ...
+    @property
+    def client_received_signal(self) -> global___ClientMessage.ClientReceivedSignal: ...
     def __init__(self,
         *,
         disconnect_res: typing.Optional[global___ClientMessage.DisconnectRes] = ...,
         get_properties_res: typing.Optional[global___ClientMessage.GetPropertiesRes] = ...,
         get_parameters_res: typing.Optional[global___ClientMessage.GetParametersRes] = ...,
         fit_res: typing.Optional[global___ClientMessage.FitRes] = ...,
         evaluate_res: typing.Optional[global___ClientMessage.EvaluateRes] = ...,
+        client_status: typing.Optional[global___ClientMessage.ClientStatus] = ...,
+        client_received_signal: typing.Optional[global___ClientMessage.ClientReceivedSignal] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","msg",b"msg"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","msg",b"msg"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["disconnect_res","get_properties_res","get_parameters_res","fit_res","evaluate_res"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["client_received_signal",b"client_received_signal","client_status",b"client_status","disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","msg",b"msg"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["client_received_signal",b"client_received_signal","client_status",b"client_status","disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","msg",b"msg"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["disconnect_res","get_properties_res","get_parameters_res","fit_res","evaluate_res","client_status","client_received_signal"]]: ...
 global___ClientMessage = ClientMessage
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/proto/transport_pb2_grpc.py` & `daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2_grpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from daisyfl.proto import transport_pb2 as flwr_dot_proto_dot_transport__pb2
+from daisyfl.proto import transport_pb2 as daisyfl_dot_proto_dot_transport__pb2
 
 
 class FlowerServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Join = channel.stream_stream(
-                '/flwr.proto.FlowerService/Join',
-                request_serializer=flwr_dot_proto_dot_transport__pb2.ClientMessage.SerializeToString,
-                response_deserializer=flwr_dot_proto_dot_transport__pb2.ServerMessage.FromString,
+                '/daisyfl.proto.FlowerService/Join',
+                request_serializer=daisyfl_dot_proto_dot_transport__pb2.ClientMessage.SerializeToString,
+                response_deserializer=daisyfl_dot_proto_dot_transport__pb2.ServerMessage.FromString,
                 )
 
 
 class FlowerServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Join(self, request_iterator, context):
@@ -31,20 +31,20 @@
         raise NotImplementedError('Method not implemented!')
 
 
 def add_FlowerServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Join': grpc.stream_stream_rpc_method_handler(
                     servicer.Join,
-                    request_deserializer=flwr_dot_proto_dot_transport__pb2.ClientMessage.FromString,
-                    response_serializer=flwr_dot_proto_dot_transport__pb2.ServerMessage.SerializeToString,
+                    request_deserializer=daisyfl_dot_proto_dot_transport__pb2.ClientMessage.FromString,
+                    response_serializer=daisyfl_dot_proto_dot_transport__pb2.ServerMessage.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'flwr.proto.FlowerService', rpc_method_handlers)
+            'daisyfl.proto.FlowerService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class FlowerService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -55,12 +55,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_stream(request_iterator, target, '/flwr.proto.FlowerService/Join',
-            flwr_dot_proto_dot_transport__pb2.ClientMessage.SerializeToString,
-            flwr_dot_proto_dot_transport__pb2.ServerMessage.FromString,
+        return grpc.experimental.stream_stream(request_iterator, target, '/daisyfl.proto.FlowerService/Join',
+            daisyfl_dot_proto_dot_transport__pb2.ClientMessage.SerializeToString,
+            daisyfl_dot_proto_dot_transport__pb2.ServerMessage.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/proto/transport_pb2_grpc.pyi` & `daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/src/py/daisyfl/server/criterion.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/zone_client_logic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,24 @@
+
+
 # Copyright 2020 Adap GmbH. All Rights Reserved.
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
 # ==============================================================================
-"""Abstract class for criterion sampling."""
-
-
-from abc import ABC, abstractmethod
-
-from .client_proxy import ClientProxy
-
-
-class Criterion(ABC):
-    """Abstract class which allows subclasses to implement criterion
-    sampling."""
-
-    @abstractmethod
-    def select(self, client: ClientProxy) -> bool:
-        """Decide whether a client should be eligible for sampling or not."""
+from daisyfl.operator.base.client_logic import ClientLogic as BaseClientLogic
+from daisyfl.client import Client
+class ZoneClientLogic(BaseClientLogic):
+    """Wrapper which adds SecAgg methods."""
+    
+    def __init__(self, client) -> None:
+        self.client: Client = client
+
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/server/driver/__init__.py` & `daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright 2022 Adap GmbH. All Rights Reserved.
+# Copyright 2020 Adap GmbH. All Rights Reserved.
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
 # ==============================================================================
-"""Flower driver service."""
+"""Server-side networking package."""
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/server/fleet/__init__.py` & `daisyfl-0.4.5/src/py/daisyfl/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,24 @@
-# Copyright 2022 Adap GmbH. All Rights Reserved.
+# Copyright 2020 Adap GmbH. All Rights Reserved.
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
 # ==============================================================================
-"""Flower fleet service."""
+"""Contains server side utilities to be used in combination with various
+components."""
+
+
+from .dynamic_loader import dynamic_load as dynamic_load
+
+
+__all__ = [
+    "dynamic_load",
+]
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/server/grpc_server/grpc_bridge.py` & `daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_bridge.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,64 +13,50 @@
 # limitations under the License.
 # ==============================================================================
 """Provides class GRPCBridge."""
 
 from dataclasses import dataclass
 from enum import Enum
 from threading import Condition
-from typing import Iterator, Optional
+from typing import Iterator, Optional, Tuple, Callable
 
 from daisyfl.proto.transport_pb2 import ClientMessage, ServerMessage
 
 
-@dataclass
-class InsWrapper:
-    """Instruction wrapper class for a single server message."""
-
-    server_message: ServerMessage
-    timeout: Optional[float]
-
-
-@dataclass
-class ResWrapper:
-    """Result wrapper class for a single client message."""
-
-    client_message: ClientMessage
-
-
 class GRPCBridgeClosed(Exception):
     """Error signaling that GRPCBridge is closed."""
 
 
 class Status(Enum):
     """Status through which the bridge can transition."""
 
-    AWAITING_INS_WRAPPER = 1
-    INS_WRAPPER_AVAILABLE = 2
-    AWAITING_RES_WRAPPER = 3
-    RES_WRAPPER_AVAILABLE = 4
+    AWAITING_SERVER_MESSAGE = 1
+    SERVER_MESSAGE_AVAILABLE = 2
+    AWAITING_CLIENT_MESSAGE = 3
+    CLIENT_MESSAGE_AVAILABLE = 4
     CLOSED = 5
 
 
 class GRPCBridge:
-    """GRPCBridge holding res_wrapper and ins_wrapper.
+    """GRPCBridge holding ServerMessage and ClientMessage.
 
     For understanding this class it is recommended to understand how
     the threading.Condition class works. See here:
     - https://docs.python.org/3/library/threading.html#condition-objects
     """
 
-    def __init__(self) -> None:
+    def __init__(self, client_idling: bool = True) -> None:
         """Init bridge."""
         # Disable all unsubscriptable-object violations in __init__ method
         # pylint: disable=unsubscriptable-object
         self._cv = Condition()  # cv stands for condition variable
-        self._status = Status.AWAITING_INS_WRAPPER
-        self._ins_wrapper: Optional[InsWrapper] = None
-        self._res_wrapper: Optional[ResWrapper] = None
+        self._status = Status.AWAITING_SERVER_MESSAGE if client_idling else Status.AWAITING_CLIENT_MESSAGE
+        self._server_message: Optional[ServerMessage] = None
+        self._client_message: Optional[ClientMessage] = None
+        self.submit_client_message = None
 
     def _is_closed(self) -> bool:
         """Return True if closed and False otherwise."""
         return self._status == Status.CLOSED
 
     def _raise_if_closed(self) -> None:
         if self._status == Status.CLOSED:
@@ -81,106 +67,116 @@
 
         The caller of the transition method will have to aquire
         conditional variable.
         """
         if next_status == Status.CLOSED:
             self._status = next_status
         elif (
-            self._status == Status.AWAITING_INS_WRAPPER
-            and next_status == Status.INS_WRAPPER_AVAILABLE
-            and self._ins_wrapper is not None
-            and self._res_wrapper is None
+            self._status == Status.AWAITING_SERVER_MESSAGE
+            and next_status == Status.SERVER_MESSAGE_AVAILABLE
+            and self._server_message is not None
+            and self._client_message is None
         ):
             self._status = next_status
         elif (
-            self._status == Status.INS_WRAPPER_AVAILABLE
-            and next_status == Status.AWAITING_RES_WRAPPER
-            and self._ins_wrapper is None
-            and self._res_wrapper is None
+            self._status == Status.SERVER_MESSAGE_AVAILABLE
+            and next_status == Status.AWAITING_CLIENT_MESSAGE
+            and self._server_message is None
+            and self._client_message is None
         ):
             self._status = next_status
         elif (
-            self._status == Status.AWAITING_RES_WRAPPER
-            and next_status == Status.RES_WRAPPER_AVAILABLE
-            and self._ins_wrapper is None
-            and self._res_wrapper is not None
+            self._status == Status.AWAITING_CLIENT_MESSAGE
+            and next_status == Status.CLIENT_MESSAGE_AVAILABLE
+            and self._server_message is None
+            and self._client_message is not None
         ):
             self._status = next_status
         elif (
-            self._status == Status.RES_WRAPPER_AVAILABLE
-            and next_status == Status.AWAITING_INS_WRAPPER
-            and self._ins_wrapper is None
-            and self._res_wrapper is None
+            self._status == Status.CLIENT_MESSAGE_AVAILABLE
+            and next_status == Status.AWAITING_SERVER_MESSAGE
+            and self._server_message is None
+            and self._client_message is None
         ):
             self._status = next_status
         else:
             raise Exception(f"Invalid transition: {self._status} to {next_status}")
 
         self._cv.notify_all()
 
     def close(self) -> None:
         """Set bridge status to closed."""
         with self._cv:
             self._transition(Status.CLOSED)
 
-    def request(self, ins_wrapper: InsWrapper) -> ResWrapper:
-        """Set ins_wrapper and wait for res_wrapper."""
-        # Set ins_wrapper and transition to INS_WRAPPER_AVAILABLE
+    def request(self, server_message: ServerMessage) -> None:
+        """Set server_message."""
+        # Set ServerMessage and transition to SERVER_MESSAGE_AVAILABLE
         with self._cv:
             self._raise_if_closed()
 
-            if self._status != Status.AWAITING_INS_WRAPPER:
+            if self._status != Status.AWAITING_SERVER_MESSAGE:
                 raise Exception("This should not happen")
 
-            self._ins_wrapper = ins_wrapper  # Write
-            self._transition(Status.INS_WRAPPER_AVAILABLE)
+            self._server_message = server_message  # Write
+            self._transition(Status.SERVER_MESSAGE_AVAILABLE)
+            return
 
-        # Read res_wrapper and transition to AWAITING_INS_WRAPPER
-        with self._cv:
-            self._cv.wait_for(
-                lambda: self._status in [Status.CLOSED, Status.RES_WRAPPER_AVAILABLE]
-            )
-
-            self._raise_if_closed()
-            res_wrapper = self._res_wrapper  # Read
-            self._res_wrapper = None  # Reset
-            self._transition(Status.AWAITING_INS_WRAPPER)
-
-        if res_wrapper is None:
-            raise Exception("ResWrapper can not be None")
-
-        return res_wrapper
-
-    def ins_wrapper_iterator(self) -> Iterator[InsWrapper]:
-        """Return iterator over ins_wrapper objects."""
+    def server_message_iterator(self) -> Iterator[ServerMessage]:
+        """Return iterator over server_message objects."""
         while not self._is_closed():
             with self._cv:
                 self._cv.wait_for(
                     lambda: self._status
-                    in [Status.CLOSED, Status.INS_WRAPPER_AVAILABLE]
+                    in [Status.CLOSED, Status.SERVER_MESSAGE_AVAILABLE]
                 )
 
                 self._raise_if_closed()
 
-                ins_wrapper = self._ins_wrapper  # Read
-                self._ins_wrapper = None  # Reset
+                server_message = self._server_message  # Read
+                self._server_message = None  # Reset
 
                 # Transition before yielding as after the yield the execution of this
                 # function is paused and will resume when next is called again.
                 # Also release condition variable by exiting the context
-                self._transition(Status.AWAITING_RES_WRAPPER)
+                self._transition(Status.AWAITING_CLIENT_MESSAGE)
 
-            if ins_wrapper is None:
-                raise Exception("InsWrapper can not be None")
+            if server_message is None:
+                raise Exception("server_message can not be None")
 
-            yield ins_wrapper
+            yield server_message
 
-    def set_res_wrapper(self, res_wrapper: ResWrapper) -> None:
-        """Set res_wrapper for consumption."""
+    def set_client_message(self, client_message: ClientMessage) -> None:
+        """Set client_message for consumption."""
         with self._cv:
             self._raise_if_closed()
 
-            if self._status != Status.AWAITING_RES_WRAPPER:
+            if self._status != Status.AWAITING_CLIENT_MESSAGE:
                 raise Exception("This should not happen")
 
-            self._res_wrapper = res_wrapper  # Write
-            self._transition(Status.RES_WRAPPER_AVAILABLE)
+            self._client_message = client_message  # Write
+
+            self._transition(Status.CLIENT_MESSAGE_AVAILABLE)
+
+        with self._cv:
+            self._cv.wait_for(
+                lambda: self._status in [Status.CLOSED, Status.CLIENT_MESSAGE_AVAILABLE]
+            )
+
+            self._raise_if_closed()
+            client_message = self._client_message  # Read
+            self._client_message = None  # Reset
+            # NOTE: if connection will break after receving client_message, don't transfer to AWAITING_SERVER_MESSAGE
+            # self._transition(Status.AWAITING_SERVER_MESSAGE)
+
+        if client_message is None:
+            raise Exception("client_message can not be None")
+        
+        self.submit_client_message(client_message)
+
+    def client_available(self,) -> bool:
+        if self._status == Status.AWAITING_SERVER_MESSAGE:
+            return True
+        return False
+    
+    def set_submit_client_message_fn(self, submit_client_message: Callable) -> None:
+        self.submit_client_message = submit_client_message
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py` & `daisyfl-0.4.5/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,118 +8,126 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""gRPC-based Flower ClientProxy implementation."""
+"""Ray-based Flower ClientProxy implementation."""
 
-from typing import Optional
+
+from typing import Callable, Dict, Optional, cast
+
+import ray
 
 from daisyfl import common
-from daisyfl.common import serde
-from daisyfl.proto.transport_pb2 import ClientMessage, ServerMessage
+from daisyfl.client import Client, ClientLike, to_client
 from daisyfl.server.client_proxy import ClientProxy
-from daisyfl.server.grpc_server.grpc_bridge import GRPCBridge, InsWrapper, ResWrapper
+
+ClientFn = Callable[[str], ClientLike]
 
 
-class GrpcClientProxy(ClientProxy):
-    """Flower client proxy which delegates over the network using gRPC."""
+class RayClientProxy(ClientProxy):
+    """Flower client proxy which delegates work using Ray."""
 
-    def __init__(
-        self,
-        cid: str,
-        bridge: GRPCBridge,
-    ):
+    def __init__(self, client_fn: ClientFn, cid: str, resources: Dict[str, int]):
         super().__init__(cid)
-        self.bridge = bridge
+        self.client_fn = client_fn
+        self.resources = resources
 
     def get_properties(
-        self,
-        ins: common.GetPropertiesIns,
-        timeout: Optional[float],
+        self, ins: common.GetPropertiesIns, timeout: Optional[float]
     ) -> common.GetPropertiesRes:
-        """Requests client's set of internal properties."""
-        get_properties_msg = serde.get_properties_ins_to_proto(ins)
-        res_wrapper: ResWrapper = self.bridge.request(
-            ins_wrapper=InsWrapper(
-                server_message=ServerMessage(get_properties_ins=get_properties_msg),
-                timeout=timeout,
-            )
+        """Returns client's properties."""
+        future_get_properties_res = launch_and_get_properties.options(  # type: ignore
+            **self.resources,
+        ).remote(self.client_fn, self.cid, ins)
+        res = ray.get(future_get_properties_res, timeout=timeout)
+        return cast(
+            common.GetPropertiesRes,
+            res,
         )
-        client_msg: ClientMessage = res_wrapper.client_message
-        get_properties_res = serde.get_properties_res_from_proto(
-            client_msg.get_properties_res
-        )
-        return get_properties_res
 
     def get_parameters(
-        self,
-        ins: common.GetParametersIns,
-        timeout: Optional[float],
+        self, ins: common.GetParametersIns, timeout: Optional[float]
     ) -> common.GetParametersRes:
         """Return the current local model parameters."""
-        get_parameters_msg = serde.get_parameters_ins_to_proto(ins)
-        res_wrapper: ResWrapper = self.bridge.request(
-            ins_wrapper=InsWrapper(
-                server_message=ServerMessage(get_parameters_ins=get_parameters_msg),
-                timeout=timeout,
-            )
-        )
-        client_msg: ClientMessage = res_wrapper.client_message
-        get_parameters_res = serde.get_parameters_res_from_proto(
-            client_msg.get_parameters_res
+        future_paramseters_res = launch_and_get_parameters.options(  # type: ignore
+            **self.resources,
+        ).remote(self.client_fn, self.cid, ins)
+        res = ray.get(future_paramseters_res, timeout=timeout)
+        return cast(
+            common.GetParametersRes,
+            res,
+        )
+
+    def fit(self, ins: common.FitIns, timeout: Optional[float]) -> common.FitRes:
+        """Train model parameters on the locally held dataset."""
+        future_fit_res = launch_and_fit.options(  # type: ignore
+            **self.resources,
+        ).remote(self.client_fn, self.cid, ins)
+        res = ray.get(future_fit_res, timeout=timeout)
+        return cast(
+            common.FitRes,
+            res,
         )
-        return get_parameters_res
-
-    def fit(
-        self,
-        ins: common.FitIns,
-        timeout: Optional[float],
-    ) -> common.FitRes:
-        """Refine the provided parameters using the locally held dataset."""
-        fit_ins_msg = serde.fit_ins_to_proto(ins)
-
-        res_wrapper: ResWrapper = self.bridge.request(
-            ins_wrapper=InsWrapper(
-                server_message=ServerMessage(fit_ins=fit_ins_msg),
-                timeout=timeout,
-            )
-        )
-        client_msg: ClientMessage = res_wrapper.client_message
-        fit_res = serde.fit_res_from_proto(client_msg.fit_res)
-        return fit_res
 
     def evaluate(
-        self,
-        ins: common.EvaluateIns,
-        timeout: Optional[float],
+        self, ins: common.EvaluateIns, timeout: Optional[float]
     ) -> common.EvaluateRes:
-        """Evaluate the provided parameters using the locally held dataset."""
-        evaluate_msg = serde.evaluate_ins_to_proto(ins)
-        res_wrapper: ResWrapper = self.bridge.request(
-            ins_wrapper=InsWrapper(
-                server_message=ServerMessage(evaluate_ins=evaluate_msg),
-                timeout=timeout,
-            )
+        """Evaluate model parameters on the locally held dataset."""
+        future_evaluate_res = launch_and_evaluate.options(  # type: ignore
+            **self.resources,
+        ).remote(self.client_fn, self.cid, ins)
+        res = ray.get(future_evaluate_res, timeout=timeout)
+        return cast(
+            common.EvaluateRes,
+            res,
         )
-        client_msg: ClientMessage = res_wrapper.client_message
-        evaluate_res = serde.evaluate_res_from_proto(client_msg.evaluate_res)
-        return evaluate_res
 
     def reconnect(
-        self,
-        ins: common.ReconnectIns,
-        timeout: Optional[float],
+        self, ins: common.ReconnectIns, timeout: Optional[float]
     ) -> common.DisconnectRes:
         """Disconnect and (optionally) reconnect later."""
-        reconnect_ins_msg = serde.reconnect_ins_to_proto(ins)
-        res_wrapper: ResWrapper = self.bridge.request(
-            ins_wrapper=InsWrapper(
-                server_message=ServerMessage(reconnect_ins=reconnect_ins_msg),
-                timeout=timeout,
-            )
-        )
-        client_msg: ClientMessage = res_wrapper.client_message
-        disconnect = serde.disconnect_res_from_proto(client_msg.disconnect_res)
-        return disconnect
+        return common.DisconnectRes(reason="")  # Nothing to do here (yet)
+
+
+@ray.remote
+def launch_and_get_properties(
+    client_fn: ClientFn, cid: str, get_properties_ins: common.GetPropertiesIns
+) -> common.GetPropertiesRes:
+    """Exectue get_properties remotely."""
+    client: Client = _create_client(client_fn, cid)
+    return client.get_properties(get_properties_ins)
+
+
+@ray.remote
+def launch_and_get_parameters(
+    client_fn: ClientFn, cid: str, get_parameters_ins: common.GetParametersIns
+) -> common.GetParametersRes:
+    """Exectue get_parameters remotely."""
+    client: Client = _create_client(client_fn, cid)
+    return client.get_parameters(get_parameters_ins)
+
+
+@ray.remote
+def launch_and_fit(
+    client_fn: ClientFn, cid: str, fit_ins: common.FitIns
+) -> common.FitRes:
+    """Exectue fit remotely."""
+    client: Client = _create_client(client_fn, cid)
+    return client.fit(fit_ins)
+
+
+@ray.remote
+def launch_and_evaluate(
+    client_fn: ClientFn, cid: str, evaluate_ins: common.EvaluateIns
+) -> common.EvaluateRes:
+    """Exectue evaluate remotely."""
+    client: Client = _create_client(client_fn, cid)
+    return client.evaluate(evaluate_ins)
+
+
+def _create_client(client_fn: ClientFn, cid: str) -> Client:
+    """Create a client instance."""
+    client_like: ClientLike = client_fn(cid)
+    return to_client(client_like=client_like)
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/server/grpc_server/grpc_server.py` & `daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 
 import grpc
 
 from daisyfl.common import GRPC_MAX_MESSAGE_LENGTH
 from daisyfl.common.logger import log
 from daisyfl.proto.transport_pb2_grpc import add_FlowerServiceServicer_to_server
 from daisyfl.server.client_manager import ClientManager
-from daisyfl.server.driver.driver_servicer import DriverServicer
-from daisyfl.server.fleet.fleet_servicer import FleetServicer
 from daisyfl.server.grpc_server.flower_service_servicer import FlowerServiceServicer
 
 INVALID_CERTIFICATES_ERR_MSG = """
     When setting any of root_certificate, certificate, or private_key,
     all of them need to be set.
 """
 
@@ -127,15 +125,15 @@
     >>>         Path("/crts/root.pem").read_bytes(),
     >>>         Path("/crts/localhost.crt").read_bytes(),
     >>>         Path("/crts/localhost.key").read_bytes(),
     >>>     ),
     >>> )
     """
 
-    servicer = FlowerServiceServicer(client_manager)
+    servicer = FlowerServiceServicer(client_manager, server_address)
     add_servicer_to_server_fn = add_FlowerServiceServicer_to_server
 
     server = generic_create_grpc_server(
         servicer_and_add_fn=(servicer, add_servicer_to_server_fn),
         server_address=server_address,
         max_concurrent_workers=max_concurrent_workers,
         max_message_length=max_message_length,
@@ -145,19 +143,15 @@
 
     server.start()
 
     return server
 
 
 def generic_create_grpc_server(  # pylint: disable=too-many-arguments
-    servicer_and_add_fn: Union[
-        Tuple[FleetServicer, AddServicerToServerFn],
-        Tuple[FlowerServiceServicer, AddServicerToServerFn],
-        Tuple[DriverServicer, AddServicerToServerFn],
-    ],
+    servicer_and_add_fn: Tuple[FlowerServiceServicer, AddServicerToServerFn],
     server_address: str,
     max_concurrent_workers: int = 1000,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     keepalive_time_ms: int = 210000,
     certificates: Optional[Tuple[bytes, bytes, bytes]] = None,
 ) -> grpc.Server:
     """Generic function to create a gRPC server with a single servicer.
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/server/history.py` & `daisyfl-0.4.5/src/py/daisyfl/server/history.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/src/py/daisyfl/server/state/__init__.py` & `daisyfl-0.4.5/src/py/daisyfl/server/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,30 @@
-# Copyright 2022 Adap GmbH. All Rights Reserved.
+# Copyright 2020 Adap GmbH. All Rights Reserved.
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
 # ==============================================================================
-"""Flower fleet state."""
+"""Flower server."""
+
+
+from .app import start_server as start_server
+from .client_manager import ClientManager as ClientManager
+from .client_manager import SimpleClientManager as SimpleClientManager
+from .history import History as History
+from .server import Server as Server
+
+__all__ = [
+    "ClientManager",
+    "History",
+    "Server",
+    "SimpleClientManager",
+    "start_server",
+]
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/server/strategy/dpfedavg_adaptive.py` & `daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,113 +8,109 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""DP-FedAvg [Andrew et al., 2019] with adaptive clipping.
+"""gRPC-based Flower ClientProxy implementation."""
 
-Paper: https://arxiv.org/pdf/1905.03871.pdf
-"""
+from typing import Optional, Dict, Union, Callable
 
-
-import math
-from typing import Dict, List, Optional, Tuple, Union
-
-import numpy as np
-
-from daisyfl.common import FitIns, FitRes, Parameters, Scalar
-from daisyfl.server.client_manager import ClientManager
+from daisyfl import common
+from daisyfl.common import serde
+from daisyfl.proto.transport_pb2 import ClientMessage, ServerMessage
 from daisyfl.server.client_proxy import ClientProxy
-from daisyfl.server.strategy.dpfedavg_fixed import DPFedAvgFixed
-from daisyfl.server.strategy.strategy import Strategy
+from daisyfl.server.grpc_server.grpc_bridge import GRPCBridge
+from daisyfl.common.logger import log
+from logging import WARNING, INFO, ERROR
 
+class GrpcClientProxy(ClientProxy):
+    """Flower client proxy which delegates over the network using gRPC."""
 
-class DPFedAvgAdaptive(DPFedAvgFixed):
-    """Wrapper for configuring a Strategy for DP with Adaptive Clipping."""
-
-    # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
-        strategy: Strategy,
-        num_sampled_clients: int,
-        init_clip_norm: float = 0.1,
-        noise_multiplier: float = 1,
-        server_side_noising: bool = True,
-        clip_norm_lr: float = 0.2,
-        clip_norm_target_quantile: float = 0.5,
-        clip_count_stddev: Optional[float] = None,
-    ) -> None:
-        super().__init__(
-            strategy=strategy,
-            num_sampled_clients=num_sampled_clients,
-            clip_norm=init_clip_norm,
-            noise_multiplier=noise_multiplier,
-            server_side_noising=server_side_noising,
-        )
-        self.clip_norm_lr = clip_norm_lr
-        self.clip_norm_target_quantile = clip_norm_target_quantile
-        self.clip_count_stddev = clip_count_stddev
-        if self.clip_count_stddev is None:
-            self.clip_count_stddev = 0
-            if noise_multiplier > 0:
-                self.clip_count_stddev = self.num_sampled_clients / 20.0
-
-        if noise_multiplier:
-            self.noise_multiplier = (
-                self.noise_multiplier ** (-2) - (2 * self.clip_count_stddev) ** (-2)
-            ) ** (-0.5)
-
-    def __repr__(self) -> str:
-        rep = "Strategy with DP with Adaptive Clipping enabled."
-        return rep
-
-    def configure_fit(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
-    ) -> List[Tuple[ClientProxy, FitIns]]:
-        """Configure the next round of training."""
-
-        additional_config = {"dpfedavg_adaptive_clip_enabled": True}
+        cid: str,
+        bridge: GRPCBridge,
+        metadata_dict: Dict,
+    ):
+        super().__init__(cid)
+        self.bridge = bridge
+        self.metadata_dict: Dict = metadata_dict
+        self.submit_subtask = None
+        self.bridge.set_submit_client_message_fn(self.submit_client_message)
 
-        client_instructions = super().configure_fit(
-            server_round, parameters, client_manager
+    def get_properties(
+        self,
+        ins: common.GetPropertiesIns,
+    ) -> None:
+        """Requests client's set of internal properties."""
+        get_properties_msg = serde.get_properties_ins_to_proto(ins)
+        self.bridge.request(
+            ServerMessage(get_properties_ins=get_properties_msg),
         )
 
-        for _, fit_ins in client_instructions:
-            fit_ins.config.update(additional_config)
-
-        return client_instructions
+    def get_parameters(
+        self,
+        ins: common.GetParametersIns,
+    ) -> None:
+        """Return the current local model parameters."""
+        get_parameters_msg = serde.get_parameters_ins_to_proto(ins)
+        self.bridge.request(
+            ServerMessage(get_parameters_ins=get_parameters_msg),
+        )
 
-    def _update_clip_norm(self, results: List[Tuple[ClientProxy, FitRes]]) -> None:
-        # Calculating number of clients which set the norm indicator bit
-        norm_bit_set_count = 0
-        for client_proxy, fit_res in results:
-            if "dpfedavg_norm_bit" not in fit_res.metrics:
-                raise Exception(
-                    f"Indicator bit not returned by client with id {client_proxy.cid}."
-                )
-            if fit_res.metrics["dpfedavg_norm_bit"]:
-                norm_bit_set_count += 1
-        # Noising the count
-        noised_norm_bit_set_count = float(
-            np.random.normal(norm_bit_set_count, self.clip_count_stddev)
+    def fit(
+        self,
+        ins: common.FitIns,
+    ) -> None:
+        """Refine the provided parameters using the locally held dataset."""
+        fit_ins_msg = serde.fit_ins_to_proto(ins)
+        self.bridge.request(
+            ServerMessage(fit_ins=fit_ins_msg),
         )
 
-        noised_norm_bit_set_fraction = noised_norm_bit_set_count / len(results)
-        # Geometric update
-        self.clip_norm *= math.exp(
-            -self.clip_norm_lr
-            * (noised_norm_bit_set_fraction - self.clip_norm_target_quantile)
+    def evaluate(
+        self,
+        ins: common.EvaluateIns,
+    ) -> None:
+        """Evaluate the provided parameters using the locally held dataset."""
+        evaluate_msg = serde.evaluate_ins_to_proto(ins)
+        self.bridge.request(
+            ServerMessage(evaluate_ins=evaluate_msg),    
         )
 
-    def aggregate_fit(
+    def reconnect(
         self,
-        server_round: int,
-        results: List[Tuple[ClientProxy, FitRes]],
-        failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
-    ) -> Tuple[Optional[Parameters], Dict[str, Scalar]]:
-        if failures:
-            return None, {}
-        new_global_model = super().aggregate_fit(server_round, results, failures)
-        self._update_clip_norm(results)
-        return new_global_model
+        ins: common.ReconnectIns,
+    ) -> None:
+        """Disconnect and (optionally) reconnect later."""
+        reconnect_ins_msg = serde.reconnect_ins_to_proto(ins)
+        self.bridge.request(
+            ServerMessage(reconnect_ins=reconnect_ins_msg),
+        )
+
+    def submit_client_message(
+        self, client_message: ClientMessage
+    ) -> None:
+        field = client_message.WhichOneof("msg")
+        if field == "disconnect_res":
+            disconnect = serde.disconnect_res_from_proto(client_message.disconnect_res)
+            log(INFO, "Will not return {} type of message to Server".format(field))
+        elif field == "get_properties_res":
+            get_properties_res = serde.get_properties_res_from_proto(client_message.get_properties_res)
+            log(INFO, "Will not return {} type of message to Server".format(field))
+        elif field == "get_parameters_res":
+            get_parameters_res = serde.get_parameters_res_from_proto(client_message.get_parameters_res)
+            log(INFO, "Will not return {} type of message to Server".format(field))
+        elif field == "fit_res":
+            fit_res = serde.fit_res_from_proto(client_message.fit_res)
+            self.submit_subtask((self, fit_res))
+        elif field == "evaluate_res":
+            evaluate_res = serde.evaluate_res_from_proto(client_message.evaluate_res)
+            self.submit_subtask((self, evaluate_res))
+        else:
+            log(INFO, "Will not return {} type of message to Server".format(field))
+
+    def set_submit_subtask_fn(self, submit_subtask: Callable) -> None:
+        self.submit_subtask = submit_subtask
+
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/server/strategy/fedavg.py` & `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedasync.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,72 +14,82 @@
 # ==============================================================================
 """Federated Averaging (FedAvg) [McMahan et al., 2016] strategy.
 
 Paper: https://arxiv.org/abs/1602.05629
 """
 
 
-from logging import WARNING
+from logging import WARNING, INFO
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 from daisyfl.common import (
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
+    CURRENT_ROUND,
+    CurrentReturns,
+    CheckResults,
+    ACCURACY,
 )
 from daisyfl.common.logger import log
-from daisyfl.server.client_manager import ClientManager
+from daisyfl.server.server import Server
 from daisyfl.server.client_proxy import ClientProxy
 
-from .aggregate import aggregate, weighted_loss_avg
+from .aggregate import aggregate, weighted_loss_avg, aggregate_fedasync
 from .strategy import Strategy
 
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
 `min_evaluate_clients` can cause the server to fail when there are too few clients
 connected to the server. `min_available_clients` must be set to a value larger
 than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
 """
 
 
-class FedAvg(Strategy):
+class FedAsync(Strategy):
     """Configurable FedAvg strategy implementation."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
-        min_fit_clients: int = 2,
-        min_evaluate_clients: int = 2,
-        min_available_clients: int = 2,
+        fraction_result: float = 1.0,
+        min_fit_clients: int = 1,
+        min_evaluate_clients: int = 1,
+        min_available_clients: int = 1,
+        min_result: int = 1,
+        # NOTE:
+        alpha: float = 0.9,
+        staleness_fn: Callable = None,
+        # NOTE:
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         on_evaluate_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         accept_failures: bool = True,
         initial_parameters: Optional[Parameters] = None,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
     ) -> None:
-        """Federated Averaging strategy.
+        """Asynchronous Federated Optimization(FedAsync).
 
-        Implementation based on https://arxiv.org/abs/1602.05629
+        Implementation based on https://arxiv.org/pdf/1903.03934.pdf
 
         Parameters
         ----------
         fraction_fit : float, optional
             Fraction of clients used during training. Defaults to 1.0.
         fraction_evaluate : float, optional
             Fraction of clients used during validation. Defaults to 1.0.
@@ -115,24 +125,30 @@
             min_fit_clients > min_available_clients
             or min_evaluate_clients > min_available_clients
         ):
             log(WARNING, WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW)
 
         self.fraction_fit = fraction_fit
         self.fraction_evaluate = fraction_evaluate
+        self.fraction_result = fraction_result
         self.min_fit_clients = min_fit_clients
         self.min_evaluate_clients = min_evaluate_clients
         self.min_available_clients = min_available_clients
+        self.min_result = min_result
         self.evaluate_fn = evaluate_fn
         self.on_fit_config_fn = on_fit_config_fn
         self.on_evaluate_config_fn = on_evaluate_config_fn
         self.accept_failures = accept_failures
         self.initial_parameters = initial_parameters
         self.fit_metrics_aggregation_fn = fit_metrics_aggregation_fn
         self.evaluate_metrics_aggregation_fn = evaluate_metrics_aggregation_fn
+        # NOTE:
+        self.alpha = alpha
+        self.staleness_fn = staleness_fn
+        # NOTE:
 
     def __repr__(self) -> str:
         rep = f"FedAvg(accept_failures={self.accept_failures})"
         return rep
 
     def num_fit_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Return the sample size and the required number of available
@@ -142,15 +158,15 @@
 
     def num_evaluation_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Use a fraction of available clients for evaluation."""
         num_clients = int(num_available_clients * self.fraction_evaluate)
         return max(num_clients, self.min_evaluate_clients), self.min_available_clients
 
     def initialize_parameters(
-        self, client_manager: ClientManager
+        self, server: Server
     ) -> Optional[Parameters]:
         """Initialize global model parameters."""
         initial_parameters = self.initial_parameters
         self.initial_parameters = None  # Don't keep initial parameters in memory
         return initial_parameters
 
     def evaluate(
@@ -164,36 +180,42 @@
         eval_res = self.evaluate_fn(server_round, parameters_ndarrays, {})
         if eval_res is None:
             return None
         loss, metrics = eval_res
         return loss, metrics
 
     def configure_fit(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self,
+        server_round: int,
+        parameters: Parameters,
+        server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
         config = {}
         if self.on_fit_config_fn is not None:
             # Custom fit config function provided
             config = self.on_fit_config_fn(server_round)
         fit_ins = FitIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_fit_clients(
-            client_manager.num_available()
-        )
-        clients = client_manager.sample(
-            num_clients=sample_size, min_num_clients=min_num_clients
+            server.num_available(credential=credential)
         )
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # Return client/config pairs
         return [(client, fit_ins) for client in clients]
 
     def configure_evaluate(
-        self, server_round: int, parameters: Parameters, client_manager: ClientManager
+        self,
+        server_round: int,
+        parameters: Parameters,
+        server: Server,
+        credential: str,
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation."""
         # Do not configure federated evaluation if fraction eval is 0.
         if self.fraction_evaluate == 0.0:
             return []
 
         # Parameters and config
@@ -201,19 +223,17 @@
         if self.on_evaluate_config_fn is not None:
             # Custom evaluation config function provided
             config = self.on_evaluate_config_fn(server_round)
         evaluate_ins = EvaluateIns(parameters, config)
 
         # Sample clients
         sample_size, min_num_clients = self.num_evaluation_clients(
-            client_manager.num_available()
-        )
-        clients = client_manager.sample(
-            num_clients=sample_size, min_num_clients=min_num_clients
+            server.num_available(credential=credential)
         )
+        clients = server.get_available_clients(min_num_clients=min_num_clients, credential=credential,)
 
         # Return client/config pairs
         return [(client, evaluate_ins) for client in clients]
 
     def aggregate_fit(
         self,
         server_round: int,
@@ -224,26 +244,32 @@
         if not results:
             return None, {}
         # Do not aggregate if there are failures and failures are not accepted
         if not self.accept_failures and failures:
             return None, {}
 
         # Convert results
-        weights_results = [
-            (parameters_to_ndarrays(fit_res.parameters), fit_res.num_examples)
-            for _, fit_res in results
-        ]
-        parameters_aggregated = ndarrays_to_parameters(aggregate(weights_results))
+        parameters_aggregated = results[0][1].prime
+        for i in range(len(results)):
+            _, fit_res = results[i]
+            weights_prime = parameters_to_ndarrays(parameters_aggregated)
+            weights_result = parameters_to_ndarrays(fit_res.parameters)
+            if self.staleness_fn is not None:
+                staleness = server_round - fit_res.config[CURRENT_ROUND]
+                alpha = self.staleness_fn(self.alpha, staleness)
+            else:
+                alpha = self.alpha
+            parameters_aggregated = ndarrays_to_parameters(aggregate_fedasync(weights_prime, weights_result, alpha))
 
         # Aggregate custom metrics if aggregation fn was provided
         metrics_aggregated = {}
         if self.fit_metrics_aggregation_fn:
             fit_metrics = [(res.num_examples, res.metrics) for _, res in results]
             metrics_aggregated = self.fit_metrics_aggregation_fn(fit_metrics)
-        elif server_round == 1:  # Only log this warning once
+        elif server_round == 0:  # Only log this warning once
             log(WARNING, "No fit_metrics_aggregation_fn provided")
 
         return parameters_aggregated, metrics_aggregated
 
     def aggregate_evaluate(
         self,
         server_round: int,
@@ -263,14 +289,32 @@
                 (evaluate_res.num_examples, evaluate_res.loss)
                 for _, evaluate_res in results
             ]
         )
 
         # Aggregate custom metrics if aggregation fn was provided
         metrics_aggregated = {}
+        eval_metrics = [(res.num_examples, res.metrics) for _, res in results]
         if self.evaluate_metrics_aggregation_fn:
-            eval_metrics = [(res.num_examples, res.metrics) for _, res in results]
             metrics_aggregated = self.evaluate_metrics_aggregation_fn(eval_metrics)
-        elif server_round == 1:  # Only log this warning once
-            log(WARNING, "No evaluate_metrics_aggregation_fn provided")
+        else:
+            log(INFO, "Using default evaluate_metrics_aggregation_fn")
+            # Multiply accuracy of each client by number of examples used
+            accuracies = [num_examples * m[ACCURACY] for num_examples, m in eval_metrics]
+            examples = [num_examples for num_examples, _ in eval_metrics]
+            metrics_aggregated = {ACCURACY: sum(accuracies) / sum(examples)}
 
         return loss_aggregated, metrics_aggregated
+
+    def check_results(
+        self, current_returns: CurrentReturns,
+    ) -> CheckResults:
+        if current_returns is None:
+            return CheckResults.FAIL
+        if ((self.fraction_result * current_returns.selected <= current_returns.results_num) and \
+            (self.min_result <= current_returns.results_num)):
+            return CheckResults.OK
+        if ((self.fraction_result * current_returns.selected) <= (current_returns.selected - current_returns.failures_num)) \
+            and (self.min_result <= (current_returns.selected - current_returns.failures_num)):
+            return CheckResults.CONTINUE
+        return CheckResults.FAIL
+
```

### Comparing `daisyfl-0.1.3/src/py/daisyfl/simulation/__init__.py` & `daisyfl-0.4.5/src/py/daisyfl/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.1.3/src/py/daisyfl/simulation/app.py` & `daisyfl-0.4.5/src/py/daisyfl/simulation/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,17 @@
 from typing import Any, Callable, Dict, List, Optional
 
 import ray
 
 from daisyfl.client.client import Client
 from daisyfl.common.logger import log
 from daisyfl.server import Server
-from daisyfl.server.app import ServerConfig, _fl, _init_defaults
+from daisyfl.server.app import _init_defaults
 from daisyfl.server.client_manager import ClientManager
 from daisyfl.server.history import History
-from daisyfl.server.strategy import Strategy
 from daisyfl.simulation.ray_transport.ray_client_proxy import RayClientProxy
 
 INVALID_ARGUMENTS_START_SIMULATION = """
 INVALID ARGUMENTS ERROR
 
 Invalid Arguments in method:
 
@@ -61,16 +60,16 @@
 def start_simulation(  # pylint: disable=too-many-arguments
     *,
     client_fn: Callable[[str], Client],
     num_clients: Optional[int] = None,
     clients_ids: Optional[List[str]] = None,
     client_resources: Optional[Dict[str, int]] = None,
     server: Optional[Server] = None,
-    config: Optional[ServerConfig] = None,
-    strategy: Optional[Strategy] = None,
+    config = None,
+    strategy = None,
     client_manager: Optional[ClientManager] = None,
     ray_init_args: Optional[Dict[str, Any]] = None,
     keep_initialised: Optional[bool] = False,
 ) -> History:
     """Start a Ray-based Flower simulation server.
 
     Parameters
@@ -185,14 +184,8 @@
         client_proxy = RayClientProxy(
             client_fn=client_fn,
             cid=cid,
             resources=resources,
         )
         initialized_server.client_manager().register(client=client_proxy)
 
-    # Start training
-    hist = _fl(
-        server=initialized_server,
-        config=initialized_config,
-    )
-
-    return hist
+    return None
```

