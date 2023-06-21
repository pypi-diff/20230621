# Comparing `tmp/langport-0.2.0.tar.gz` & `tmp/langport-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langport-0.2.0.tar", last modified: Sun Jun 18 13:12:05 2023, max compression
+gzip compressed data, was "langport-0.2.1.tar", last modified: Wed Jun 21 04:12:11 2023, max compression
```

## Comparing `langport-0.2.0.tar` & `langport-0.2.1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.902785 langport-0.2.0/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.2.0/LICENSE
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5591 2023-06-18 13:12:05.902785 langport-0.2.0/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5115 2023-06-18 13:11:45.000000 langport-0.2.0/README.md
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.2.0/langport/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.2.0/langport/constants.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport/core/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.2.0/langport/core/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.2.0/langport/core/base_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.2.0/langport/core/cluster_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.2.0/langport/core/cluster_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.2.0/langport/core/dispatch.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport/data/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.2.0/langport/data/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport/data/conversation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5684 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/conversation_settings.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport/data/conversation/settings/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/dolly.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/h2ogpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/mpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/one_shot.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/redpajama.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/stablelm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/zero_shot.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.2.0/langport/model/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/adapters/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.2.0/langport/model/adapters/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/adapters/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/adapters/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      280 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/chatglm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/codegen.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/dolly_v2.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/adapters/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/adapters/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/stable_lm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/starcoder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/t5.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/text2vec.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7171 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/compression.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/executor/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/executor/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/executor/base.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/executor/embedding/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/executor/embedding/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5816 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/executor/embedding/huggingface.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/executor/generation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/executor/generation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/executor/generation/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4247 2023-06-18 13:11:45.000000 langport-0.2.0/langport/model/executor/generation/ggml.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    15561 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/executor/generation/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2110 2023-06-18 13:11:45.000000 langport-0.2.0/langport/model/executor/ggml.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7037 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/executor/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/model_adapter.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1272 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/model_args.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/models/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.2.0/langport/model/models/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.2.0/langport/model/models/rwkv_model.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/monkey_patch_non_inplace.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/protocol/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.2.0/langport/protocol/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.2.0/langport/protocol/huggingface_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4477 2023-05-14 15:31:14.000000 langport-0.2.0/langport/protocol/openai_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.2.0/langport/protocol/tabby_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2726 2023-06-12 17:00:54.000000 langport-0.2.0/langport/protocol/worker_protocol.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/routers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/routers/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.2.0/langport/routers/gateway/common.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16376 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/gateway/openai_compatible.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/routers/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.2.0/langport/routers/server/core_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/server/embedding_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3486 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/server/generation_node.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/service/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.2.0/langport/service/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.902785 langport-0.2.0/langport/service/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/service/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/cluster_monitor.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/cluster_monitor_app.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/fauxpilot_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/graphite_feeder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/huggingface_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5714 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/openai_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/tabby_api.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.902785 langport-0.2.0/langport/service/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/service/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2187 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/server/chatgpt_generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/server/dummy_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/server/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2610 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/server/generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2911 2023-06-18 13:11:45.000000 langport-0.2.0/langport/service/server/ggml_generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.902785 langport-0.2.0/langport/utils/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7261 2023-06-16 07:20:16.000000 langport-0.2.0/langport/utils/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.2.0/langport/utils/cache_state.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.2.0/langport/utils/evaluation.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.2.0/langport/utils/http_pool.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.2.0/langport/utils/interval_timer.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       27 2023-06-18 13:11:45.000000 langport-0.2.0/langport/version.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.902785 langport-0.2.0/langport/workers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/workers/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.2.0/langport/workers/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3176 2023-06-16 07:20:16.000000 langport-0.2.0/langport/workers/generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport.egg-info/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5591 2023-06-18 13:12:05.000000 langport-0.2.0/langport.egg-info/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4172 2023-06-18 13:12:05.000000 langport-0.2.0/langport.egg-info/SOURCES.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-06-18 13:12:05.000000 langport-0.2.0/langport.egg-info/dependency_links.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      237 2023-06-18 13:12:05.000000 langport-0.2.0/langport.egg-info/requires.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-06-18 13:12:05.000000 langport-0.2.0/langport.egg-info/top_level.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1082 2023-06-18 13:11:45.000000 langport-0.2.0/pyproject.toml
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-06-18 13:12:05.902785 langport-0.2.0/setup.cfg
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.2.1/LICENSE
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5596 2023-06-21 04:12:11.779040 langport-0.2.1/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5120 2023-06-21 04:11:50.000000 langport-0.2.1/README.md
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.771040 langport-0.2.1/langport/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.2.1/langport/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.2.1/langport/constants.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.771040 langport-0.2.1/langport/core/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.2.1/langport/core/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.2.1/langport/core/base_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.2.1/langport/core/cluster_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.2.1/langport/core/cluster_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.2.1/langport/core/dispatch.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.771040 langport-0.2.1/langport/data/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.2.1/langport/data/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.771040 langport-0.2.1/langport/data/conversation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5684 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/conversation_settings.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/data/conversation/settings/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/dolly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/h2ogpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/mpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/one_shot.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/redpajama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/stablelm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/zero_shot.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.2.1/langport/model/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/adapters/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.2.1/langport/model/adapters/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/adapters/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/adapters/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      280 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/codegen.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/dolly_v2.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/adapters/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/adapters/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/stable_lm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/starcoder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/t5.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/text2vec.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7171 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/compression.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/executor/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/executor/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/executor/base.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/executor/embedding/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/executor/embedding/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5816 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/executor/embedding/huggingface.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/executor/generation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/executor/generation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/executor/generation/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5000 2023-06-21 04:11:50.000000 langport-0.2.1/langport/model/executor/generation/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    15698 2023-06-21 04:11:50.000000 langport-0.2.1/langport/model/executor/generation/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2110 2023-06-18 13:11:45.000000 langport-0.2.1/langport/model/executor/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7037 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/executor/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/model_adapter.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1272 2023-06-19 18:47:41.000000 langport-0.2.1/langport/model/model_args.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/models/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.2.1/langport/model/models/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.2.1/langport/model/models/rwkv_model.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/monkey_patch_non_inplace.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/protocol/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.2.1/langport/protocol/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.2.1/langport/protocol/huggingface_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4477 2023-05-14 15:31:14.000000 langport-0.2.1/langport/protocol/openai_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.2.1/langport/protocol/tabby_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2726 2023-06-12 17:00:54.000000 langport-0.2.1/langport/protocol/worker_protocol.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/routers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/routers/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.2.1/langport/routers/gateway/common.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16376 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/gateway/openai_compatible.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/routers/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.2.1/langport/routers/server/core_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/server/embedding_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3486 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/server/generation_node.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/service/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.2.1/langport/service/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/service/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/service/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/cluster_monitor.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/cluster_monitor_app.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/fauxpilot_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/graphite_feeder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/huggingface_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4920 2023-06-21 04:11:50.000000 langport-0.2.1/langport/service/gateway/openai_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/tabby_api.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/service/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/service/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2187 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/server/chatgpt_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/server/dummy_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/server/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2610 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/server/generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2911 2023-06-18 13:11:45.000000 langport-0.2.1/langport/service/server/ggml_generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/utils/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7261 2023-06-21 04:11:44.000000 langport-0.2.1/langport/utils/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.2.1/langport/utils/cache_state.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.2.1/langport/utils/evaluation.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.2.1/langport/utils/http_pool.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.2.1/langport/utils/interval_timer.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       27 2023-06-21 04:11:50.000000 langport-0.2.1/langport/version.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/workers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/workers/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.2.1/langport/workers/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3176 2023-06-16 07:20:16.000000 langport-0.2.1/langport/workers/generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.771040 langport-0.2.1/langport.egg-info/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5596 2023-06-21 04:12:11.000000 langport-0.2.1/langport.egg-info/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4172 2023-06-21 04:12:11.000000 langport-0.2.1/langport.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-06-21 04:12:11.000000 langport-0.2.1/langport.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      237 2023-06-21 04:12:11.000000 langport-0.2.1/langport.egg-info/requires.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-06-21 04:12:11.000000 langport-0.2.1/langport.egg-info/top_level.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1082 2023-06-21 04:11:50.000000 langport-0.2.1/pyproject.toml
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-06-21 04:12:11.779040 langport-0.2.1/setup.cfg
```

### Comparing `langport-0.2.0/LICENSE` & `langport-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/PKG-INFO` & `langport-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langport
-Version: 0.2.0
+Version: 0.2.1
 Summary: A large language model serving platform.
 Project-URL: Homepage, https://github.com/vtuber-plan/langport
 Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -135,15 +135,15 @@
 python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpus 0,1 --num-gpus 2
 python -m langport.service.gateway.openai_api
 ```
 
 Run text generation with ggml worker:
 
 ```bash
-python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
+python -m langport.service.server.ggml_generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
 ```
 
 ## License
 
 langport is released under the Apache Software License.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langport Version: 0.2.0 Summary: A large language
+Metadata-Version: 2.1 Name: langport Version: 0.2.1 Summary: A large language
 model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
 langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml License-
 File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
@@ -58,15 +58,15 @@
 m langport.service.gateway.openai_api --controller-address http://localhost:
 21003 # 21003 is OK! python -m langport.service.gateway.openai_api --
 controller-address http://localhost:21002 # Any worker is also OK! ``` Run text
 generation with multi GPUs: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  --gpus
 0,1 --num-gpus 2 python -m langport.service.gateway.openai_api ``` Run text
 generation with ggml worker: ```bash python -
-m langport.service.server.generation_worker --port 21001 --model-path  --gpu-
-layers
+m langport.service.server.ggml_generation_worker --port 21001 --model-path  --
+gpu-layers
 resize this for your VRAM)> ``` ## License langport is released under the
 Apache Software License. ## See also - [langport-docs](https://github.com/
 vtuber-plan/langport/tree/main/docs) - [langport-source](https://github.com/
 vtuber-plan/langport) ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=vtuber-plan/langport&type=Date)](https://star-
 history.com/#vtuber-plan/langport&Date)
```

### Comparing `langport-0.2.0/README.md` & `langport-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpus 0,1 --num-gpus 2
 python -m langport.service.gateway.openai_api
 ```
 
 Run text generation with ggml worker:
 
 ```bash
-python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
+python -m langport.service.server.ggml_generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
 ```
 
 ## License
 
 langport is released under the Apache Software License.
```

#### html2text {}

```diff
@@ -51,15 +51,15 @@
 m langport.service.gateway.openai_api --controller-address http://localhost:
 21003 # 21003 is OK! python -m langport.service.gateway.openai_api --
 controller-address http://localhost:21002 # Any worker is also OK! ``` Run text
 generation with multi GPUs: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  --gpus
 0,1 --num-gpus 2 python -m langport.service.gateway.openai_api ``` Run text
 generation with ggml worker: ```bash python -
-m langport.service.server.generation_worker --port 21001 --model-path  --gpu-
-layers
+m langport.service.server.ggml_generation_worker --port 21001 --model-path  --
+gpu-layers
 resize this for your VRAM)> ``` ## License langport is released under the
 Apache Software License. ## See also - [langport-docs](https://github.com/
 vtuber-plan/langport/tree/main/docs) - [langport-source](https://github.com/
 vtuber-plan/langport) ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=vtuber-plan/langport&type=Date)](https://star-
 history.com/#vtuber-plan/langport&Date)
```

### Comparing `langport-0.2.0/langport/constants.py` & `langport-0.2.1/langport/constants.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/core/base_node.py` & `langport-0.2.1/langport/core/base_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/core/cluster_node.py` & `langport-0.2.1/langport/core/cluster_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/core/cluster_worker.py` & `langport-0.2.1/langport/core/cluster_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/data/conversation/__init__.py` & `langport-0.2.1/langport/data/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/data/conversation/conversation_settings.py` & `langport-0.2.1/langport/data/conversation/conversation_settings.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/baize.py` & `langport-0.2.1/langport/model/adapters/baize.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/bard.py` & `langport-0.2.1/langport/model/adapters/bard.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/billa.py` & `langport-0.2.1/langport/model/adapters/billa.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/chatgpt.py` & `langport-0.2.1/langport/model/adapters/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/claude.py` & `langport-0.2.1/langport/model/adapters/claude.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/dolly_v2.py` & `langport-0.2.1/langport/model/adapters/dolly_v2.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/falcon.py` & `langport-0.2.1/langport/model/adapters/falcon.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/koala.py` & `langport-0.2.1/langport/model/adapters/koala.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/oasst_pythia.py` & `langport-0.2.1/langport/model/adapters/oasst_pythia.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/openbuddy.py` & `langport-0.2.1/langport/model/adapters/openbuddy.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/phoenix.py` & `langport-0.2.1/langport/model/adapters/phoenix.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/rwkv.py` & `langport-0.2.1/langport/model/adapters/rwkv.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/stable_lm.py` & `langport-0.2.1/langport/model/adapters/stable_lm.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/adapters/vicuna.py` & `langport-0.2.1/langport/model/adapters/vicuna.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/compression.py` & `langport-0.2.1/langport/model/compression.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/executor/base.py` & `langport-0.2.1/langport/model/executor/base.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/executor/embedding/__init__.py` & `langport-0.2.1/langport/model/executor/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/executor/embedding/huggingface.py` & `langport-0.2.1/langport/model/executor/embedding/huggingface.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/executor/generation/__init__.py` & `langport-0.2.1/langport/model/executor/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/executor/generation/chatgpt.py` & `langport-0.2.1/langport/model/executor/generation/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/executor/generation/ggml.py` & `langport-0.2.1/langport/model/executor/generation/ggml.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import threading
 from typing import List, Optional
 from langport.model.executor.ggml import GgmlExecutor, GgmlTokenizer
 from ctransformers import LLM
 from langport.protocol.worker_protocol import BaseWorkerResult, GenerationTask, GenerationWorkerResult, UsageInfo
 from langport.workers.generation_worker import GenerationModelWorker
 
 
@@ -26,53 +27,69 @@
             prompt_length = len(tokens)
             output_ids = []
 
             # Compatible with some models
             top_k = 40 if task.top_k <= 1 else task.top_k
             repetition_penalty = 1.17647 if task.repetition_penalty == 0.0 else task.repetition_penalty
 
-            for j, token in enumerate(model.generate(tokens, top_k=top_k, top_p=task.top_p,
-                                                  temperature=task.temperature, repetition_penalty=repetition_penalty)):
+            finish_reason = "stop"
+            n_tokens = 0
+            for token in model.generate(
+                            tokens, top_k=top_k, top_p=task.top_p, batch_size=512,
+                            temperature=task.temperature, repetition_penalty=repetition_penalty):
+                n_tokens += 1
                 output_ids.append(token)
-                if tokenizer.is_eos_token(token) or prompt_length + j == task.max_tokens - 1:
+                if n_tokens == task.max_tokens:
                     output = tokenizer.decode(output_ids)
-                    if tokenizer.is_eos_token(token):
-                        finish_reason = "stop"
-                    else:
-                        finish_reason = "length"
+                    finish_reason = "length"
                     yield GenerationWorkerResult(
                         task_id=task.task_id,
                         type="finish",
                         text=output,
                         usage=UsageInfo(
                             prompt_tokens=prompt_length,
-                            total_tokens=prompt_length + j,
-                            completion_tokens=j,
+                            total_tokens=prompt_length + n_tokens,
+                            completion_tokens=n_tokens,
                         ),
                         finish_reason=finish_reason,
                     )
                     break
 
-                if j%stream_interval!=0:
+                if n_tokens % stream_interval != 0:
                     continue
                 output = tokenizer.decode(output_ids)
 
                 # yield result
                 yield GenerationWorkerResult(
                     task_id=task.task_id,
                     type="data",
                     text=output,
                     usage=UsageInfo(
                         prompt_tokens=prompt_length,
-                        total_tokens=prompt_length + j,
-                        completion_tokens=j,
+                        total_tokens=prompt_length + n_tokens,
+                        completion_tokens=n_tokens,
                     ),
                     finish_reason=None,
                 )
 
+            # token == eos is checked in model.generate
+            if finish_reason == "stop":
+                output = tokenizer.decode(output_ids)
+                yield GenerationWorkerResult(
+                    task_id=task.task_id,
+                    type="finish",
+                    text=output,
+                    usage=UsageInfo(
+                        prompt_tokens=prompt_length,
+                        total_tokens=prompt_length + n_tokens,
+                        completion_tokens=n_tokens,
+                    ),
+                    finish_reason="stop",
+                )
+
 
 class GgmlGenerationExecutor(GgmlExecutor):
     def __init__(
         self,
         model_name: str,
         model_path: str,
         context_length: int,
@@ -89,14 +106,15 @@
             max_gpu_memory=None,
             gpu_layers=gpu_layers,
             lib=lib,
             model_type=model_type,
         )
         self.n_ctx = context_length
         self.adapter, self.model, self.tokenizer = self.load_model(model_path, from_pretrained_kwargs={})
+        self.lock = threading.Lock()
 
     @property
     def context_length(self) -> int:
         return self.n_ctx
 
     def tokenize(self, text: str) -> List[int]:
         return self.tokenizer.encode(text)
@@ -105,22 +123,27 @@
         if not worker.online:
             return
 
         tasks = worker.fetch_tasks()
         batch_size = len(tasks)
         if batch_size == 0:
             return
+        
+        self.lock.acquire()
 
         # batch inference
-        for chunk in stream_generation(
-            self.model,
-            self.tokenizer,
-            worker.stream_interval,
-            tasks,
-        ):
-            worker.push_task_result(chunk.task_id, chunk)
-
-        for task in tasks:
-            worker.push_task_result(
-                task.task_id, BaseWorkerResult(task_id=task.task_id, type="done")
-            )
+        try:
+            for chunk in stream_generation(
+                self.model,
+                self.tokenizer,
+                worker.stream_interval,
+                tasks,
+            ):
+                worker.push_task_result(chunk.task_id, chunk)
+
+            for task in tasks:
+                worker.push_task_result(
+                    task.task_id, BaseWorkerResult(task_id=task.task_id, type="done")
+                )
+        finally:
+            self.lock.release()
```

### Comparing `langport-0.2.0/langport/model/executor/generation/huggingface.py` & `langport-0.2.1/langport/model/executor/generation/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             self.batch_tokens_cache[i].append(token)
 
             # auto check stop
             if token == self.tokenizer.eos_token_id:
                 self.set_stop(i)
             if self.tasks[i].stop_token_ids is not None and token in self.tasks[i].stop_token_ids:
                 self.set_stop(i)
-            if self.get_prompt_length(i) + self.get_generated_length(i) >= self.max_tokens[i]:
+            if self.get_generated_length(i) == self.max_tokens[i]:
                 self.set_stop(i)
                 
     def set_stop(self, idx:int):
         self._check_idx(idx)
         self.stop[idx] = True
     
     def is_stop(self, idx:int):
@@ -256,15 +256,19 @@
                 decoder_input_ids_list = [new_ids_tensor]
             else:
                 decoder_input_ids = inputs(return_attention_mask=False)
                 decoder_input_ids_list = [decoder_input_ids]
 
             if all(inputs.stop):
                 break
-
+        
+        # stop all
+        for i in range(inputs.batch_size):
+            if not inputs.is_stop(i):
+                inputs.set_stop(i)
         if streamer:
             streamer.end()
 
         del past_key_values
 
 class GenerationWorkerStreamer(BaseStreamer):
     def __init__(self,
@@ -288,15 +292,15 @@
             stop_pos = stop_by_stopwords(text, 0, task.stop)
             if stop_pos != -1:
                 self.task_batch.set_stop(i)
                 text = text[:stop_pos]
             prompt_len = self.task_batch.get_prompt_length(i)
 
             if self.task_batch.is_stop(i):
-                if prompt_len + generated_len >= self.task_batch.max_tokens[i]:
+                if generated_len == self.task_batch.max_tokens[i]:
                     finish_reason = "length"
                 else:
                     finish_reason = "stop"
                 self.worker.push_task_result(task.task_id,
                     GenerationWorkerResult(
                         task_id=task.task_id,
                         type="finish",
@@ -325,15 +329,16 @@
                             completion_tokens=generated_len,
                         ),
                         finish_reason=None,
                     )
                 )
 
     def end(self):
-        pass
+        # check all done
+        self.put(None)
             
 
 def stop_by_stopwords(
     output: str, rfind_start: int, stop: Optional[Union[str, List[str]]]
 ) -> int:
     if stop is not None:
         if isinstance(stop, str):
```

### Comparing `langport-0.2.0/langport/model/executor/ggml.py` & `langport-0.2.1/langport/model/executor/ggml.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/executor/huggingface.py` & `langport-0.2.1/langport/model/executor/huggingface.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/model_adapter.py` & `langport-0.2.1/langport/model/model_adapter.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/model_args.py` & `langport-0.2.1/langport/model/model_args.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/models/rwkv_model.py` & `langport-0.2.1/langport/model/models/rwkv_model.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/model/monkey_patch_non_inplace.py` & `langport-0.2.1/langport/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/protocol/huggingface_api_protocol.py` & `langport-0.2.1/langport/protocol/huggingface_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/protocol/openai_api_protocol.py` & `langport-0.2.1/langport/protocol/openai_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/protocol/tabby_api_protocol.py` & `langport-0.2.1/langport/protocol/tabby_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/protocol/worker_protocol.py` & `langport-0.2.1/langport/protocol/worker_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/routers/gateway/common.py` & `langport-0.2.1/langport/routers/gateway/common.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/routers/gateway/openai_compatible.py` & `langport-0.2.1/langport/routers/gateway/openai_compatible.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/routers/server/core_node.py` & `langport-0.2.1/langport/routers/server/core_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/routers/server/embedding_node.py` & `langport-0.2.1/langport/routers/server/embedding_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/routers/server/generation_node.py` & `langport-0.2.1/langport/routers/server/generation_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/service/gateway/cluster_monitor.py` & `langport-0.2.1/langport/service/gateway/cluster_monitor.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/service/gateway/cluster_monitor_app.py` & `langport-0.2.1/langport/service/gateway/cluster_monitor_app.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/service/gateway/fauxpilot_api.py` & `langport-0.2.1/langport/service/gateway/fauxpilot_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/service/gateway/graphite_feeder.py` & `langport-0.2.1/langport/service/gateway/graphite_feeder.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/service/gateway/huggingface_api.py` & `langport-0.2.1/langport/service/gateway/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/service/gateway/openai_api.py` & `langport-0.2.1/langport/service/gateway/tabby_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import argparse
 import json
 import logging
 
-from typing import Optional
+from typing import Optional, Union
 
 import fastapi
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse
 from starlette.middleware.base import BaseHTTPMiddleware, DispatchFunction
 from starlette.types import ASGIApp
 import uvicorn
 
 from langport.constants import ErrorCode
 from fastapi.exceptions import RequestValidationError
-from langport.protocol.openai_api_protocol import (
-    ChatCompletionRequest,
+from langport.protocol.tabby_api_protocol import (
+    Choice,
     CompletionRequest,
-    EmbeddingsRequest,
+    CompletionResponse,
+    ChoiceEvent,
+    CompletionEvent,
+    EventTypeMapping,
+    HTTPValidationError,
+    LanguagePresets,
 )
-from langport.routers.gateway.common import AppSettings, create_error_response
-from langport.routers.gateway.openai_compatible import api_chat_completions, api_completions, api_embeddings, api_models
+from langport.protocol.openai_api_protocol import CompletionRequest as OpenAICompletionRequest
+
+from langport.routers.gateway.common import AppSettings, check_model, create_error_response
+from langport.routers.gateway.openai_compatible import completions_non_stream, get_gen_params
 
 logger = logging.getLogger(__name__)
 
 app = fastapi.FastAPI(debug=False)
 
 class BaseAuthorizationMiddleware(BaseHTTPMiddleware):
     def __init__(self, app: ASGIApp, sk:str, dispatch: Optional[DispatchFunction] = None) -> None:
@@ -41,75 +48,86 @@
                 status_code=401,
                 content={"msg":"Not authenticated"},
                 headers={"WWW-Authenticate": "Bearer"},
             )
         return await call_next(request)
 
 
-class RedirectModelMiddleware(BaseHTTPMiddleware):
-    def __init__(self, app: ASGIApp,  redirect_rules:list, dispatch: Optional[DispatchFunction] = None) -> None:
-        super().__init__(app, dispatch)
-        self.redirect_rules = redirect_rules
-        self.receive_ = None
-
-    async def dispatch(self, request, call_next):
-        if "content-type" not in request.headers or request.headers["content-type"] != "application/json":
-            return await call_next(request)
-        
-        try:
-            await self.set_body(request)
-            data = await request.json()
-            if "model" in data:
-                for rule in self.redirect_rules:
-                    from_model_name, to_model_name = rule.split(":")
-                    if data["model"] == from_model_name:
-                        data["model"] = to_model_name
-                        self.receive_['body'] = json.dumps(data).encode("utf-8")
-                        break
-        except Exception as e:
-            logger.error(f"RedirectModelMiddleware: {e}")
-        return await call_next(request)
-    
-    async def set_body(self, request):
-        self.receive_ = await request._receive()
-        async def receive():
-            return self.receive_
-        request._receive = receive
-
-
 @app.exception_handler(RequestValidationError)
 async def validation_exception_handler(request, exc):
     return create_error_response(ErrorCode.VALIDATION_TYPE_ERROR, str(exc))
 
+def trim_with_stop_words(output: str, stopwords: list) -> str:
+    for w in sorted(stopwords, key=len, reverse=True):
+        index = output.find(w)
+        if index != -1:
+            output = output[:index]
+    return output
+
+@app.post("/v1/events")
+async def events(e: Union[ChoiceEvent, CompletionEvent]):
+    if isinstance(e, EventTypeMapping[e.type]):
+        # events_lib.log_event(e)
+        return JSONResponse(content="ok")
+    else:
+        print(type(e))
+        return JSONResponse(content="invalid event", status_code=422)
 
-@app.get("/v1/models")
-async def models():
-    return await api_models(app.app_settings)
-
-
-@app.post("/v1/chat/completions")
-async def chat_completions(request: ChatCompletionRequest):
-    return await api_chat_completions(app.app_settings, request)
 
 @app.post("/v1/completions")
 async def completions(request: CompletionRequest):
-    return await api_completions(app.app_settings, request)
-
-
-@app.post("/v1/embeddings")
-async def embeddings(request: EmbeddingsRequest):
-    return await api_embeddings(app.app_settings, request)
-
+    error_check_ret = await check_model(app.app_settings, request, "generation", app.model_name)
+    if error_check_ret is not None:
+        return error_check_ret
+    
+    preset = LanguagePresets.get(request.language, None)
+    if preset is None:
+        return CompletionResponse()
+
+    # print(request.prompt)
+    payload = get_gen_params(
+        app.model_name,
+        request.prompt,
+        temperature=0.7,
+        top_p=1.0,
+        max_tokens=preset.max_length,
+        echo=False,
+        stream=False,
+        stop=preset.stop_words,
+    )
+    N = 1
+    response = await completions_non_stream(
+        app.app_settings,
+        payload,
+        OpenAICompletionRequest(
+            model=app.model_name,
+            prompt=request.prompt,
+            n=N,
+        )
+    )
+    if isinstance(response, JSONResponse):
+        print(response.body)
+        return CompletionResponse()
+
+    # print(response.choices[0].text.replace("\n", "\\n"))
+    return CompletionResponse(choices=[
+        Choice(
+            index=i,
+            text=response.choices[i].text
+        )
+        for i in range(len(response.choices))
+    ])
 
-if __name__ in ["__main__", "langport.service.gateway.openai_api"]:
+if __name__ in ["__main__", "langport.service.gateway.tabby_api"]:
     parser = argparse.ArgumentParser(
-        description="Langport openai-compatible RESTful API server."
+        description="Langport tabby-compatible RESTful API server."
     )
     parser.add_argument("--host", type=str, default="localhost", help="host name")
     parser.add_argument("--port", type=int, default=8000, help="port number")
+    parser.add_argument("--model-name", type=str, default="J-350M", help="default tabby model name")
     parser.add_argument("--sk", type=str, default=None, help="security key")
     parser.add_argument(
         "--controller-address", type=str, default="http://localhost:21001"
     )
     parser.add_argument(
         "--allow-credentials", action="store_true", help="allow credentials"
     )
@@ -118,40 +136,35 @@
     )
     parser.add_argument(
         "--allowed-methods", type=json.loads, default=["*"], help="allowed methods"
     )
     parser.add_argument(
         "--allowed-headers", type=json.loads, default=["*"], help="allowed headers"
     )
-    parser.add_argument("--redirect", action="append", required=False, help="redirect model_name to another model_name, e.g. --redirect model_name1:model_name2")
     args = parser.parse_args()
 
     app.add_middleware(
         CORSMiddleware,
         allow_origins=args.allowed_origins,
         allow_credentials=args.allow_credentials,
         allow_methods=args.allowed_methods,
         allow_headers=args.allowed_headers,
     )
-    if args.redirect is not None:
-        app.add_middleware(
-            RedirectModelMiddleware,
-            redirect_rules=args.redirect,
-        )
     if args.sk is not None:
         app.add_middleware(
             BaseAuthorizationMiddleware,
             sk=args.sk,
         )
+    app.model_name = args.model_name
     app.app_settings = AppSettings(controller_address=args.controller_address)
 
     logger.debug(f"==== args ====\n{args}")
 
     # don't delete this line, otherwise the middleware won't work with reload==True
     if __name__ == "__main__":
         uvicorn.run(
-            "langport.service.gateway.openai_api:app",
+            "langport.service.gateway.tabby_api:app",
             host=args.host,
             port=args.port,
             log_level="info",
             reload=True,
         )
```

### Comparing `langport-0.2.0/langport/service/server/chatgpt_generation_worker.py` & `langport-0.2.1/langport/service/server/chatgpt_generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/service/server/dummy_worker.py` & `langport-0.2.1/langport/service/server/dummy_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/service/server/embedding_worker.py` & `langport-0.2.1/langport/service/server/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/service/server/generation_worker.py` & `langport-0.2.1/langport/service/server/generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/service/server/ggml_generation_worker.py` & `langport-0.2.1/langport/service/server/ggml_generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/utils/__init__.py` & `langport-0.2.1/langport/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/utils/evaluation.py` & `langport-0.2.1/langport/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/utils/http_pool.py` & `langport-0.2.1/langport/utils/http_pool.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/utils/interval_timer.py` & `langport-0.2.1/langport/utils/interval_timer.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/workers/embedding_worker.py` & `langport-0.2.1/langport/workers/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport/workers/generation_worker.py` & `langport-0.2.1/langport/workers/generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/langport.egg-info/PKG-INFO` & `langport-0.2.1/langport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langport
-Version: 0.2.0
+Version: 0.2.1
 Summary: A large language model serving platform.
 Project-URL: Homepage, https://github.com/vtuber-plan/langport
 Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -135,15 +135,15 @@
 python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpus 0,1 --num-gpus 2
 python -m langport.service.gateway.openai_api
 ```
 
 Run text generation with ggml worker:
 
 ```bash
-python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
+python -m langport.service.server.ggml_generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
 ```
 
 ## License
 
 langport is released under the Apache Software License.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langport Version: 0.2.0 Summary: A large language
+Metadata-Version: 2.1 Name: langport Version: 0.2.1 Summary: A large language
 model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
 langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml License-
 File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
@@ -58,15 +58,15 @@
 m langport.service.gateway.openai_api --controller-address http://localhost:
 21003 # 21003 is OK! python -m langport.service.gateway.openai_api --
 controller-address http://localhost:21002 # Any worker is also OK! ``` Run text
 generation with multi GPUs: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  --gpus
 0,1 --num-gpus 2 python -m langport.service.gateway.openai_api ``` Run text
 generation with ggml worker: ```bash python -
-m langport.service.server.generation_worker --port 21001 --model-path  --gpu-
-layers
+m langport.service.server.ggml_generation_worker --port 21001 --model-path  --
+gpu-layers
 resize this for your VRAM)> ``` ## License langport is released under the
 Apache Software License. ## See also - [langport-docs](https://github.com/
 vtuber-plan/langport/tree/main/docs) - [langport-source](https://github.com/
 vtuber-plan/langport) ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=vtuber-plan/langport&type=Date)](https://star-
 history.com/#vtuber-plan/langport&Date)
```

### Comparing `langport-0.2.0/langport.egg-info/SOURCES.txt` & `langport-0.2.1/langport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langport-0.2.0/pyproject.toml` & `langport-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langport"
-version = "0.2.0"
+version = "0.2.1"
 description = "A large language model serving platform."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
```

