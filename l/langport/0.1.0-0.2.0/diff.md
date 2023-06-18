# Comparing `tmp/langport-0.1.0.tar.gz` & `tmp/langport-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langport-0.1.0.tar", last modified: Fri Jun 16 07:21:30 2023, max compression
+gzip compressed data, was "langport-0.2.0.tar", last modified: Sun Jun 18 13:12:05 2023, max compression
```

## Comparing `langport-0.1.0.tar` & `langport-0.2.0.tar`

### file list

```diff
@@ -1,138 +1,136 @@
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.127148 langport-0.1.0/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.1.0/LICENSE
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5396 2023-06-16 07:21:30.127148 langport-0.1.0/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4916 2023-06-16 07:20:16.000000 langport-0.1.0/README.md
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.115149 langport-0.1.0/langport/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.1.0/langport/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.1.0/langport/constants.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.115149 langport-0.1.0/langport/core/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.1.0/langport/core/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.1.0/langport/core/base_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.1.0/langport/core/cluster_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.1.0/langport/core/cluster_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.1.0/langport/core/dispatch.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.115149 langport-0.1.0/langport/data/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.1.0/langport/data/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.115149 langport-0.1.0/langport/data/conversation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5684 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/conversation_settings.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.119149 langport-0.1.0/langport/data/conversation/settings/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/dolly.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/h2ogpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      271 2023-06-16 07:20:16.000000 langport-0.1.0/langport/data/conversation/settings/llama_cpp.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/mpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/one_shot.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/redpajama.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/stablelm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/zero_shot.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.119149 langport-0.1.0/langport/model/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.1.0/langport/model/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/model/adapters/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.1.0/langport/model/adapters/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/adapters/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/adapters/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      280 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/chatglm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/codegen.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/dolly_v2.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/adapters/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/adapters/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1377 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/llama_cpp.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/stable_lm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/starcoder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/t5.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/text2vec.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7171 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/compression.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/model/executor/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/executor/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/executor/base.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/model/executor/embedding/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/executor/embedding/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5816 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/embedding/huggingface.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/model/executor/generation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/generation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/executor/generation/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    15561 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/generation/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4463 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/generation/llamacpp.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7037 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      909 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/llamacpp.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/model_adapter.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1272 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/model_args.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/model/models/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.1.0/langport/model/models/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.1.0/langport/model/models/rwkv_model.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/monkey_patch_non_inplace.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/protocol/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.1.0/langport/protocol/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.1.0/langport/protocol/huggingface_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4477 2023-05-14 15:31:14.000000 langport-0.1.0/langport/protocol/openai_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.1.0/langport/protocol/tabby_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2726 2023-06-12 17:00:54.000000 langport-0.1.0/langport/protocol/worker_protocol.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/routers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/routers/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.1.0/langport/routers/gateway/common.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16376 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/gateway/openai_compatible.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/routers/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.1.0/langport/routers/server/core_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/server/embedding_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3486 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/server/generation_node.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/service/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.1.0/langport/service/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.127148 langport-0.1.0/langport/service/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/service/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/cluster_monitor.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/cluster_monitor_app.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/fauxpilot_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/graphite_feeder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/huggingface_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5714 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/openai_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/tabby_api.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.127148 langport-0.1.0/langport/service/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/service/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2187 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/server/chatgpt_generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/server/dummy_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/server/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2610 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/server/generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2830 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/server/ggml_generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.127148 langport-0.1.0/langport/utils/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7261 2023-06-16 07:20:16.000000 langport-0.1.0/langport/utils/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.1.0/langport/utils/cache_state.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.1.0/langport/utils/evaluation.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.1.0/langport/utils/http_pool.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.1.0/langport/utils/interval_timer.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       27 2023-06-16 07:20:16.000000 langport-0.1.0/langport/version.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.127148 langport-0.1.0/langport/workers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/workers/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.1.0/langport/workers/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3176 2023-06-16 07:20:16.000000 langport-0.1.0/langport/workers/generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.115149 langport-0.1.0/langport.egg-info/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5396 2023-06-16 07:21:30.000000 langport-0.1.0/langport.egg-info/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4266 2023-06-16 07:21:30.000000 langport-0.1.0/langport.egg-info/SOURCES.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-06-16 07:21:30.000000 langport-0.1.0/langport.egg-info/dependency_links.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-16 07:21:30.000000 langport-0.1.0/langport.egg-info/requires.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-06-16 07:21:30.000000 langport-0.1.0/langport.egg-info/top_level.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1089 2023-06-16 07:21:09.000000 langport-0.1.0/pyproject.toml
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-06-16 07:21:30.127148 langport-0.1.0/setup.cfg
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.902785 langport-0.2.0/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.2.0/LICENSE
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5591 2023-06-18 13:12:05.902785 langport-0.2.0/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5115 2023-06-18 13:11:45.000000 langport-0.2.0/README.md
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.2.0/langport/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.2.0/langport/constants.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport/core/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.2.0/langport/core/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.2.0/langport/core/base_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.2.0/langport/core/cluster_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.2.0/langport/core/cluster_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.2.0/langport/core/dispatch.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport/data/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.2.0/langport/data/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport/data/conversation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5684 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/conversation_settings.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport/data/conversation/settings/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/dolly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/h2ogpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/mpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/one_shot.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/redpajama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/stablelm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.2.0/langport/data/conversation/settings/zero_shot.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.2.0/langport/model/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/adapters/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.2.0/langport/model/adapters/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/adapters/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/adapters/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      280 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/codegen.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/dolly_v2.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/adapters/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/adapters/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/stable_lm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/starcoder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/t5.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/text2vec.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/adapters/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7171 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/compression.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/executor/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/executor/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/executor/base.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/executor/embedding/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/executor/embedding/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5816 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/executor/embedding/huggingface.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/executor/generation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/executor/generation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/executor/generation/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4247 2023-06-18 13:11:45.000000 langport-0.2.0/langport/model/executor/generation/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    15561 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/executor/generation/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2110 2023-06-18 13:11:45.000000 langport-0.2.0/langport/model/executor/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7037 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/executor/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/model_adapter.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1272 2023-06-16 07:20:16.000000 langport-0.2.0/langport/model/model_args.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/model/models/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.2.0/langport/model/models/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.2.0/langport/model/models/rwkv_model.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.2.0/langport/model/monkey_patch_non_inplace.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/protocol/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.2.0/langport/protocol/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.2.0/langport/protocol/huggingface_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4477 2023-05-14 15:31:14.000000 langport-0.2.0/langport/protocol/openai_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.2.0/langport/protocol/tabby_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2726 2023-06-12 17:00:54.000000 langport-0.2.0/langport/protocol/worker_protocol.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/routers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/routers/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.2.0/langport/routers/gateway/common.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16376 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/gateway/openai_compatible.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/routers/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.2.0/langport/routers/server/core_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/server/embedding_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3486 2023-06-12 17:00:54.000000 langport-0.2.0/langport/routers/server/generation_node.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.898785 langport-0.2.0/langport/service/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.2.0/langport/service/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.902785 langport-0.2.0/langport/service/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/service/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/cluster_monitor.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/cluster_monitor_app.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/fauxpilot_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/graphite_feeder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/huggingface_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5714 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/openai_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/gateway/tabby_api.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.902785 langport-0.2.0/langport/service/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/service/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2187 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/server/chatgpt_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/server/dummy_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/server/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2610 2023-06-16 07:20:16.000000 langport-0.2.0/langport/service/server/generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2911 2023-06-18 13:11:45.000000 langport-0.2.0/langport/service/server/ggml_generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.902785 langport-0.2.0/langport/utils/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7261 2023-06-16 07:20:16.000000 langport-0.2.0/langport/utils/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.2.0/langport/utils/cache_state.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.2.0/langport/utils/evaluation.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.2.0/langport/utils/http_pool.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.2.0/langport/utils/interval_timer.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       27 2023-06-18 13:11:45.000000 langport-0.2.0/langport/version.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.902785 langport-0.2.0/langport/workers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.0/langport/workers/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.2.0/langport/workers/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3176 2023-06-16 07:20:16.000000 langport-0.2.0/langport/workers/generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-18 13:12:05.894785 langport-0.2.0/langport.egg-info/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5591 2023-06-18 13:12:05.000000 langport-0.2.0/langport.egg-info/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4172 2023-06-18 13:12:05.000000 langport-0.2.0/langport.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-06-18 13:12:05.000000 langport-0.2.0/langport.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      237 2023-06-18 13:12:05.000000 langport-0.2.0/langport.egg-info/requires.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-06-18 13:12:05.000000 langport-0.2.0/langport.egg-info/top_level.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1082 2023-06-18 13:11:45.000000 langport-0.2.0/pyproject.toml
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-06-18 13:12:05.902785 langport-0.2.0/setup.cfg
```

### Comparing `langport-0.1.0/LICENSE` & `langport-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/PKG-INFO` & `langport-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: langport
-Version: 0.1.0
+Version: 0.2.0
 Summary: A large language model serving platform.
 Project-URL: Homepage, https://github.com/vtuber-plan/langport
 Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: llamacpp
+Provides-Extra: ggml
 License-File: LICENSE
 
 <div align="center">
 
 # LangPort
 
 <a href="https://github.com/vtuber-plan/langport">
@@ -29,14 +29,16 @@
 
 LangPort is a open-source large language model serving platform.
 Our goal is to build a super fast LLM inference service.
 
 This project is inspired by [lmsys/fastchat](https://github.com/lm-sys/FastChat), we hope that the serving platform is lightweight and fast, but fastchat includes other features such as training and evaluation make it complicated.
 
 The core features include:
+- Huggingface transformers support.
+- ggml (llama.cpp) support.
 - A distributed serving system for state-of-the-art models.
 - Streaming generation support with various decoding strategies.
 - Batch inference for higher throughput.
 - Support for encoder-only, decoder-only and encoder-decoder models.
 - OpenAI-compatible RESTful APIs.
 - FauxPilot-compatible RESTful APIs.
 - HuggingFace-compatible RESTful APIs.
@@ -46,14 +48,15 @@
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 
 ## News
+- [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
 - [2023/05/22] New distributed architecture.
 - [2023/05/14] Batch inference supported.
@@ -61,26 +64,31 @@
 
 
 ## Install
 
 ### Method 1: With pip
 
 ```bash
-pip3 install langport
+pip install langport
 ```
 
 or:
 
 ```bash
-pip3 install git+https://github.com/vtuber-plan/langport.git 
+pip install git+https://github.com/vtuber-plan/langport.git 
 ```
 
-If you need llamacpp generation worker, use this command:
+If you need ggml generation worker, use this command:
 ```bash
-pip3 install langport[llamacpp]
+pip install langport[ggml]
+```
+
+If you wanna use GPU:
+```bash
+CT_CUBLAS=1 pip install langport[ggml]
 ```
 
 ### Method 2: From source
 
 1. Clone this repository
 ```bash
 git clone https://github.com/vtuber-plan/langport.git
@@ -124,18 +132,18 @@
 Run text generation with multi GPUs:
 
 ``` bash
 python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpus 0,1 --num-gpus 2
 python -m langport.service.gateway.openai_api
 ```
 
-Run text generation with LLama.cpp worker:
+Run text generation with ggml worker:
 
 ```bash
-python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --n-gpu-layers <num layer to gpu (resize this for your VRAM)>
+python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
 ```
 
 ## License
 
 langport is released under the Apache Software License.
```

#### html2text {}

```diff
@@ -1,43 +1,46 @@
-Metadata-Version: 2.1 Name: langport Version: 0.1.0 Summary: A large language
+Metadata-Version: 2.1 Name: langport Version: 0.2.0 Summary: A large language
 model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
 langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: llamacpp
-License-File: LICENSE
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml License-
+File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
                                architecture.jpg)
 LangPort is a open-source large language model serving platform. Our goal is to
 build a super fast LLM inference service. This project is inspired by [lmsys/
 fastchat](https://github.com/lm-sys/FastChat), we hope that the serving
 platform is lightweight and fast, but fastchat includes other features such as
-training and evaluation make it complicated. The core features include: - A
-distributed serving system for state-of-the-art models. - Streaming generation
-support with various decoding strategies. - Batch inference for higher
-throughput. - Support for encoder-only, decoder-only and encoder-decoder
-models. - OpenAI-compatible RESTful APIs. - FauxPilot-compatible RESTful APIs.
-- HuggingFace-compatible RESTful APIs. - Tabby-compatible RESTful APIs. ##
-Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
-V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
-server, and the following figure shows the Queries Per Second (QPS) and Tokens
-Per Second (TPS) of FastChat and LangPort with different max model concurrency
-settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/09]
-Add LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding
-worker support. - [2023/06/01] Add HuggingFace text generation API support. -
-[2023/06/01] Add tabby API support. - [2023/05/23] Add chat throughput test
-script. - [2023/05/22] New distributed architecture. - [2023/05/14] Batch
-inference supported. - [2023/05/10] Langport project started. ## Install ###
-Method 1: With pip ```bash pip3 install langport ``` or: ```bash pip3 install
-git+https://github.com/vtuber-plan/langport.git ``` If you need llamacpp
-generation worker, use this command: ```bash pip3 install langport[llamacpp]
-``` ### Method 2: From source 1. Clone this repository ```bash git clone https:
-//github.com/vtuber-plan/langport.git cd langport ``` 2. Install the Package
-```bash pip install --upgrade pip pip install -e . ``` ## Start the server It
-is simple to start a single node chat API service: ``` bash python -
+training and evaluation make it complicated. The core features include: -
+Huggingface transformers support. - ggml (llama.cpp) support. - A distributed
+serving system for state-of-the-art models. - Streaming generation support with
+various decoding strategies. - Batch inference for higher throughput. - Support
+for encoder-only, decoder-only and encoder-decoder models. - OpenAI-compatible
+RESTful APIs. - FauxPilot-compatible RESTful APIs. - HuggingFace-compatible
+RESTful APIs. - Tabby-compatible RESTful APIs. ## Benchmark We use single
+RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16
+setting. We create 32 threads to submit chat tasks to the server, and the
+following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS)
+of FastChat and LangPort with different max model concurrency settings. !
+[benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18] Add ggml
+(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
+LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
+support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
+06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
+[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
+supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
+With pip ```bash pip install langport ``` or: ```bash pip install git+https://
+github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
+this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
+```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
+Clone this repository ```bash git clone https://github.com/vtuber-plan/
+langport.git cd langport ``` 2. Install the Package ```bash pip install --
+upgrade pip pip install -e . ``` ## Start the server It is simple to start a
+single node chat API service: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  python -
 m langport.service.gateway.openai_api ``` If you need the embeddings API or
 other features, you can deploy a distributed inference cluster: ``` bash python
 -m langport.service.server.dummy_worker --port 21001 python -
 m langport.service.server.generation_worker --model-path  --neighbors http://
 localhost:21001 python -m langport.service.server.embedding_worker --model-path
 --neighbors http://localhost:21001 python -
@@ -54,16 +57,16 @@
 neighbors http://localhost:21001 http://localhost:21004 python -
 m langport.service.gateway.openai_api --controller-address http://localhost:
 21003 # 21003 is OK! python -m langport.service.gateway.openai_api --
 controller-address http://localhost:21002 # Any worker is also OK! ``` Run text
 generation with multi GPUs: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  --gpus
 0,1 --num-gpus 2 python -m langport.service.gateway.openai_api ``` Run text
-generation with LLama.cpp worker: ```bash python -
-m langport.service.server.generation_worker --port 21001 --model-path  --n-gpu-
+generation with ggml worker: ```bash python -
+m langport.service.server.generation_worker --port 21001 --model-path  --gpu-
 layers
 resize this for your VRAM)> ``` ## License langport is released under the
 Apache Software License. ## See also - [langport-docs](https://github.com/
 vtuber-plan/langport/tree/main/docs) - [langport-source](https://github.com/
 vtuber-plan/langport) ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=vtuber-plan/langport&type=Date)](https://star-
 history.com/#vtuber-plan/langport&Date)
```

### Comparing `langport-0.1.0/README.md` & `langport-0.2.0/langport.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: langport
+Version: 0.2.0
+Summary: A large language model serving platform.
+Project-URL: Homepage, https://github.com/vtuber-plan/langport
+Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: ggml
+License-File: LICENSE
+
 <div align="center">
 
 # LangPort
 
 <a href="https://github.com/vtuber-plan/langport">
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/vtuber-plan/langport?style=social">
 </a>
@@ -15,14 +29,16 @@
 
 LangPort is a open-source large language model serving platform.
 Our goal is to build a super fast LLM inference service.
 
 This project is inspired by [lmsys/fastchat](https://github.com/lm-sys/FastChat), we hope that the serving platform is lightweight and fast, but fastchat includes other features such as training and evaluation make it complicated.
 
 The core features include:
+- Huggingface transformers support.
+- ggml (llama.cpp) support.
 - A distributed serving system for state-of-the-art models.
 - Streaming generation support with various decoding strategies.
 - Batch inference for higher throughput.
 - Support for encoder-only, decoder-only and encoder-decoder models.
 - OpenAI-compatible RESTful APIs.
 - FauxPilot-compatible RESTful APIs.
 - HuggingFace-compatible RESTful APIs.
@@ -32,14 +48,15 @@
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 
 ## News
+- [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
 - [2023/05/22] New distributed architecture.
 - [2023/05/14] Batch inference supported.
@@ -47,26 +64,31 @@
 
 
 ## Install
 
 ### Method 1: With pip
 
 ```bash
-pip3 install langport
+pip install langport
 ```
 
 or:
 
 ```bash
-pip3 install git+https://github.com/vtuber-plan/langport.git 
+pip install git+https://github.com/vtuber-plan/langport.git 
+```
+
+If you need ggml generation worker, use this command:
+```bash
+pip install langport[ggml]
 ```
 
-If you need llamacpp generation worker, use this command:
+If you wanna use GPU:
 ```bash
-pip3 install langport[llamacpp]
+CT_CUBLAS=1 pip install langport[ggml]
 ```
 
 ### Method 2: From source
 
 1. Clone this repository
 ```bash
 git clone https://github.com/vtuber-plan/langport.git
@@ -110,18 +132,18 @@
 Run text generation with multi GPUs:
 
 ``` bash
 python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpus 0,1 --num-gpus 2
 python -m langport.service.gateway.openai_api
 ```
 
-Run text generation with LLama.cpp worker:
+Run text generation with ggml worker:
 
 ```bash
-python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --n-gpu-layers <num layer to gpu (resize this for your VRAM)>
+python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
 ```
 
 ## License
 
 langport is released under the Apache Software License.
```

#### html2text {}

```diff
@@ -1,36 +1,46 @@
+Metadata-Version: 2.1 Name: langport Version: 0.2.0 Summary: A large language
+model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
+langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
+issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml License-
+File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
                                architecture.jpg)
 LangPort is a open-source large language model serving platform. Our goal is to
 build a super fast LLM inference service. This project is inspired by [lmsys/
 fastchat](https://github.com/lm-sys/FastChat), we hope that the serving
 platform is lightweight and fast, but fastchat includes other features such as
-training and evaluation make it complicated. The core features include: - A
-distributed serving system for state-of-the-art models. - Streaming generation
-support with various decoding strategies. - Batch inference for higher
-throughput. - Support for encoder-only, decoder-only and encoder-decoder
-models. - OpenAI-compatible RESTful APIs. - FauxPilot-compatible RESTful APIs.
-- HuggingFace-compatible RESTful APIs. - Tabby-compatible RESTful APIs. ##
-Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
-V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
-server, and the following figure shows the Queries Per Second (QPS) and Tokens
-Per Second (TPS) of FastChat and LangPort with different max model concurrency
-settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/09]
-Add LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding
-worker support. - [2023/06/01] Add HuggingFace text generation API support. -
-[2023/06/01] Add tabby API support. - [2023/05/23] Add chat throughput test
-script. - [2023/05/22] New distributed architecture. - [2023/05/14] Batch
-inference supported. - [2023/05/10] Langport project started. ## Install ###
-Method 1: With pip ```bash pip3 install langport ``` or: ```bash pip3 install
-git+https://github.com/vtuber-plan/langport.git ``` If you need llamacpp
-generation worker, use this command: ```bash pip3 install langport[llamacpp]
-``` ### Method 2: From source 1. Clone this repository ```bash git clone https:
-//github.com/vtuber-plan/langport.git cd langport ``` 2. Install the Package
-```bash pip install --upgrade pip pip install -e . ``` ## Start the server It
-is simple to start a single node chat API service: ``` bash python -
+training and evaluation make it complicated. The core features include: -
+Huggingface transformers support. - ggml (llama.cpp) support. - A distributed
+serving system for state-of-the-art models. - Streaming generation support with
+various decoding strategies. - Batch inference for higher throughput. - Support
+for encoder-only, decoder-only and encoder-decoder models. - OpenAI-compatible
+RESTful APIs. - FauxPilot-compatible RESTful APIs. - HuggingFace-compatible
+RESTful APIs. - Tabby-compatible RESTful APIs. ## Benchmark We use single
+RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16
+setting. We create 32 threads to submit chat tasks to the server, and the
+following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS)
+of FastChat and LangPort with different max model concurrency settings. !
+[benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18] Add ggml
+(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
+LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
+support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
+06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
+[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
+supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
+With pip ```bash pip install langport ``` or: ```bash pip install git+https://
+github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
+this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
+```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
+Clone this repository ```bash git clone https://github.com/vtuber-plan/
+langport.git cd langport ``` 2. Install the Package ```bash pip install --
+upgrade pip pip install -e . ``` ## Start the server It is simple to start a
+single node chat API service: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  python -
 m langport.service.gateway.openai_api ``` If you need the embeddings API or
 other features, you can deploy a distributed inference cluster: ``` bash python
 -m langport.service.server.dummy_worker --port 21001 python -
 m langport.service.server.generation_worker --model-path  --neighbors http://
 localhost:21001 python -m langport.service.server.embedding_worker --model-path
 --neighbors http://localhost:21001 python -
@@ -47,16 +57,16 @@
 neighbors http://localhost:21001 http://localhost:21004 python -
 m langport.service.gateway.openai_api --controller-address http://localhost:
 21003 # 21003 is OK! python -m langport.service.gateway.openai_api --
 controller-address http://localhost:21002 # Any worker is also OK! ``` Run text
 generation with multi GPUs: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  --gpus
 0,1 --num-gpus 2 python -m langport.service.gateway.openai_api ``` Run text
-generation with LLama.cpp worker: ```bash python -
-m langport.service.server.generation_worker --port 21001 --model-path  --n-gpu-
+generation with ggml worker: ```bash python -
+m langport.service.server.generation_worker --port 21001 --model-path  --gpu-
 layers
 resize this for your VRAM)> ``` ## License langport is released under the
 Apache Software License. ## See also - [langport-docs](https://github.com/
 vtuber-plan/langport/tree/main/docs) - [langport-source](https://github.com/
 vtuber-plan/langport) ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=vtuber-plan/langport&type=Date)](https://star-
 history.com/#vtuber-plan/langport&Date)
```

### Comparing `langport-0.1.0/langport/constants.py` & `langport-0.2.0/langport/constants.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/core/base_node.py` & `langport-0.2.0/langport/core/base_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/core/cluster_node.py` & `langport-0.2.0/langport/core/cluster_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/core/cluster_worker.py` & `langport-0.2.0/langport/core/cluster_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/data/conversation/__init__.py` & `langport-0.2.0/langport/data/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/data/conversation/conversation_settings.py` & `langport-0.2.0/langport/data/conversation/conversation_settings.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/baize.py` & `langport-0.2.0/langport/model/adapters/baize.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/bard.py` & `langport-0.2.0/langport/model/adapters/bard.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/billa.py` & `langport-0.2.0/langport/model/adapters/billa.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/chatgpt.py` & `langport-0.2.0/langport/model/adapters/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/claude.py` & `langport-0.2.0/langport/model/adapters/claude.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/dolly_v2.py` & `langport-0.2.0/langport/model/adapters/dolly_v2.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/falcon.py` & `langport-0.2.0/langport/model/adapters/falcon.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/koala.py` & `langport-0.2.0/langport/model/adapters/koala.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/llama_cpp.py` & `langport-0.2.0/langport/model/adapters/openbuddy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+import os
 from langport.data.conversation import ConversationHistory
 from langport.data.conversation.conversation_settings import get_conv_settings
 from langport.model.model_adapter import BaseAdapter
 
-
-class LlamaCppAdapter(BaseAdapter):
-    """The model adapter for LlamaCpp"""
+class OpenBuddyAdapter(BaseAdapter):
+    """The model adapter for OpenBuddy"""
 
     def match(self, model_path: str):
-        return "ggml" in model_path
+        if model_path.endswith('/'):
+            model_path = model_path[:-1]
+        dir_name = os.path.basename(model_path)
+        parent_name = os.path.dirname(model_path)
+        return dir_name.startswith('openbuddy') or parent_name.startswith('openbuddy')
 
     def get_default_conv_template(self, model_path: str) -> ConversationHistory:
-        settings = get_conv_settings("llama_cpp")
+        settings = get_conv_settings("openbuddy")
         return ConversationHistory(
-            system=f"""Consider a conversation between User (a human) and Assistant (named Buddy).
-Buddy is an INTP-T, a friendly, intelligent and multilingual AI assistant, based on LLaMA Transformers architecture, by OpenBuddy team on GitHub.
+            system="""Consider a conversation between User (a human) and Assistant (named Buddy).
+Buddy is an INTP-T, a friendly, intelligent and multilingual AI assistant, by OpenBuddy team. GitHub: https://github.com/OpenBuddy/OpenBuddy
 Buddy cannot access the Internet.
 Buddy can fluently speak the user's language (e.g. English, Chinese).
 Buddy can generate poems, stories, code, essays, songs, parodies, and more.
 Buddy possesses vast knowledge about the world, history, and culture.
 Buddy's responses are always safe, creative, high-quality, human-like, and interesting.
-Buddy strictly refuses to discuss political, NSFW, illegal, abusive, offensive, or other sensitive topics.
+Buddy strictly refuses to discuss political, NSFW, or other unsafe topics.
 
 User: Hi.
 Assistant: Hi, I'm Buddy, your AI assistant. How can I help you today?""",
             messages=[],
             offset=0,
             settings=settings,
         )
```

### Comparing `langport-0.1.0/langport/model/adapters/oasst_pythia.py` & `langport-0.2.0/langport/model/adapters/oasst_pythia.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/phoenix.py` & `langport-0.2.0/langport/model/adapters/phoenix.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/rwkv.py` & `langport-0.2.0/langport/model/adapters/rwkv.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/stable_lm.py` & `langport-0.2.0/langport/model/adapters/stable_lm.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/adapters/vicuna.py` & `langport-0.2.0/langport/model/adapters/vicuna.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/compression.py` & `langport-0.2.0/langport/model/compression.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/executor/base.py` & `langport-0.2.0/langport/model/executor/base.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/executor/embedding/__init__.py` & `langport-0.2.0/langport/model/executor/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/executor/embedding/huggingface.py` & `langport-0.2.0/langport/model/executor/embedding/huggingface.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/executor/generation/__init__.py` & `langport-0.2.0/langport/model/executor/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/executor/generation/chatgpt.py` & `langport-0.2.0/langport/model/executor/generation/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/executor/generation/huggingface.py` & `langport-0.2.0/langport/model/executor/generation/huggingface.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/executor/generation/llamacpp.py` & `langport-0.2.0/langport/model/executor/generation/ggml.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 from typing import List, Optional
-
-from llama_cpp import Llama, LlamaTokenizer
-
-from langport.model.executor.llamacpp import LlamaCppExecutor
-from langport.model.model_adapter import get_model_adapter
-from langport.model.executor.base import BaseModelExecutor, LocalModelExecutor
+from langport.model.executor.ggml import GgmlExecutor, GgmlTokenizer
+from ctransformers import LLM
 from langport.protocol.worker_protocol import BaseWorkerResult, GenerationTask, GenerationWorkerResult, UsageInfo
 from langport.workers.generation_worker import GenerationModelWorker
 
 
-def batch_generation(
-    model: Llama,
-    tokenizer: LlamaTokenizer,
+def stream_generation(
+    model: LLM,
+    tokenizer: GgmlTokenizer,
     stream_interval: int,
     tasks: List[GenerationTask],
 ):
     batch_size = len(tasks)
     if batch_size == 0:
         return
 
     # todo: add stop words support
     for i, task in enumerate(tasks):
-
         output = ""
 
         if task.echo:
             output = task.prompt
         else:
-            tokens = tokenizer.encode(" " + task.prompt + " ")
+            tokens = tokenizer.encode(task.prompt)
             prompt_length = len(tokens)
             output_ids = []
 
-            for j, token in enumerate(model.generate(tokens, top_k=40, top_p=task.top_p, 
-                                                  temp=task.temperature, repeat_penalty=1.17647)):
+            # Compatible with some models
+            top_k = 40 if task.top_k <= 1 else task.top_k
+            repetition_penalty = 1.17647 if task.repetition_penalty == 0.0 else task.repetition_penalty
+
+            for j, token in enumerate(model.generate(tokens, top_k=top_k, top_p=task.top_p,
+                                                  temperature=task.temperature, repetition_penalty=repetition_penalty)):
                 output_ids.append(token)
-                if token == model.token_eos() or len(tokens) + j == task.max_tokens - 1:
+                if tokenizer.is_eos_token(token) or prompt_length + j == task.max_tokens - 1:
                     output = tokenizer.decode(output_ids)
-                    if token == model.token_eos():
+                    if tokenizer.is_eos_token(token):
                         finish_reason = "stop"
                     else:
                         finish_reason = "length"
                     yield GenerationWorkerResult(
                         task_id=task.task_id,
                         type="finish",
                         text=output,
@@ -67,39 +66,37 @@
                         total_tokens=prompt_length + j,
                         completion_tokens=j,
                     ),
                     finish_reason=None,
                 )
 
 
-class LlamaCppGenerationExecutor(LlamaCppExecutor):
+class GgmlGenerationExecutor(GgmlExecutor):
     def __init__(
         self,
         model_name: str,
         model_path: str,
-        n_ctx: int,
-        n_gpu_layers: int,
-        seed: int,
-        n_batch: int,
-        last_n_tokens_size: int
+        context_length: int,
+        gpu_layers: int,
+        model_type: str = "llama",
+        lib: Optional[str] = None,
     ) -> None:
-        super(LlamaCppGenerationExecutor, self).__init__(
+        n_gpu = 1 if gpu_layers > 0 else 0
+        super(GgmlGenerationExecutor, self).__init__(
             model_name=model_name,
             model_path=model_path,
             device="cpu",
-            num_gpus=1,
+            num_gpus=n_gpu,
             max_gpu_memory=None,
+            gpu_layers=gpu_layers,
+            lib=lib,
+            model_type=model_type,
         )
-        self.n_ctx = n_ctx
-        self.adapter = get_model_adapter(model_path)
-        self.model, self.tokenizer = self.load_model(model_path, {"n_ctx":n_ctx,
-                                                                          "n_gpu_layers":n_gpu_layers, 
-                                                                          "seed":seed, 
-                                                                          "n_batch":n_batch, 
-                                                                          "last_n_tokens_size":last_n_tokens_size,})
+        self.n_ctx = context_length
+        self.adapter, self.model, self.tokenizer = self.load_model(model_path, from_pretrained_kwargs={})
 
     @property
     def context_length(self) -> int:
         return self.n_ctx
 
     def tokenize(self, text: str) -> List[int]:
         return self.tokenizer.encode(text)
@@ -110,15 +107,15 @@
 
         tasks = worker.fetch_tasks()
         batch_size = len(tasks)
         if batch_size == 0:
             return
 
         # batch inference
-        for chunk in batch_generation(
+        for chunk in stream_generation(
             self.model,
             self.tokenizer,
             worker.stream_interval,
             tasks,
         ):
             worker.push_task_result(chunk.task_id, chunk)
```

### Comparing `langport-0.1.0/langport/model/executor/huggingface.py` & `langport-0.2.0/langport/model/executor/huggingface.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/model_adapter.py` & `langport-0.2.0/langport/model/model_adapter.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/model_args.py` & `langport-0.2.0/langport/model/model_args.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/models/rwkv_model.py` & `langport-0.2.0/langport/model/models/rwkv_model.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/model/monkey_patch_non_inplace.py` & `langport-0.2.0/langport/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/protocol/huggingface_api_protocol.py` & `langport-0.2.0/langport/protocol/huggingface_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/protocol/openai_api_protocol.py` & `langport-0.2.0/langport/protocol/openai_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/protocol/tabby_api_protocol.py` & `langport-0.2.0/langport/protocol/tabby_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/protocol/worker_protocol.py` & `langport-0.2.0/langport/protocol/worker_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/routers/gateway/common.py` & `langport-0.2.0/langport/routers/gateway/common.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/routers/gateway/openai_compatible.py` & `langport-0.2.0/langport/routers/gateway/openai_compatible.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/routers/server/core_node.py` & `langport-0.2.0/langport/routers/server/core_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/routers/server/embedding_node.py` & `langport-0.2.0/langport/routers/server/embedding_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/routers/server/generation_node.py` & `langport-0.2.0/langport/routers/server/generation_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/gateway/cluster_monitor.py` & `langport-0.2.0/langport/service/gateway/cluster_monitor.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/gateway/cluster_monitor_app.py` & `langport-0.2.0/langport/service/gateway/cluster_monitor_app.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/gateway/fauxpilot_api.py` & `langport-0.2.0/langport/service/gateway/fauxpilot_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/gateway/graphite_feeder.py` & `langport-0.2.0/langport/service/gateway/graphite_feeder.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/gateway/huggingface_api.py` & `langport-0.2.0/langport/service/gateway/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/gateway/openai_api.py` & `langport-0.2.0/langport/service/gateway/openai_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/gateway/tabby_api.py` & `langport-0.2.0/langport/service/gateway/tabby_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/server/chatgpt_generation_worker.py` & `langport-0.2.0/langport/service/server/chatgpt_generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/server/dummy_worker.py` & `langport-0.2.0/langport/service/server/dummy_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/server/embedding_worker.py` & `langport-0.2.0/langport/service/server/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/server/generation_worker.py` & `langport-0.2.0/langport/service/server/generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/service/server/ggml_generation_worker.py` & `langport-0.2.0/langport/service/server/ggml_generation_worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,19 +20,18 @@
 
     add_model_args(parser)
     parser.add_argument("--model-name", type=str, help="Optional display name")
     parser.add_argument("--limit-model-concurrency", type=int, default=8)
     parser.add_argument("--batch", type=int, default=1)
     parser.add_argument("--stream-interval", type=int, default=2)
 
-    parser.add_argument("--n-ctx", type=int, default=2048)
-    parser.add_argument("--n-gpu-layers", type=int, default=24)
-    parser.add_argument("--seed", type=int, default=42)
-    parser.add_argument("--n-batch", type=int, default=1024)
-    parser.add_argument("--last-n-tokens-size", type=int, default=1024)
+    parser.add_argument("--context-length", type=int, default=2048)
+    parser.add_argument("--gpu-layers", type=int, default=0)
+    parser.add_argument("--lib", type=str, default=None, choices=["avx2", "avx", "basic"], help="The path to a shared library or one of avx2, avx, basic.")
+    parser.add_argument("--model-type", type=str, default="llama", choices=["llama", "gpt2", "dolly-v2", "starcoder"], help="The type of model to use.")
     args = parser.parse_args()
 
     node_id = str(uuid.uuid4())
     logger = build_logger("ggml_generation_worker", f"ggml_generation_worker_{node_id}.log")
     logger.info(f"args: {args}")
 
     if args.gpus:
@@ -47,23 +46,22 @@
 
     if args.worker_address is None:
         args.worker_address = f"http://{args.host}:{args.port}"
     
     if args.model_name is None:
         args.model_name = os.path.basename(os.path.normpath(args.model_path))
     
-    from langport.model.executor.generation.llamacpp import LlamaCppGenerationExecutor
-    executor = LlamaCppGenerationExecutor(
+    from langport.model.executor.generation.ggml import GgmlGenerationExecutor
+    executor = GgmlGenerationExecutor(
         model_name=args.model_name,
         model_path=args.model_path,
-        n_ctx=args.n_ctx,
-        n_gpu_layers=args.n_gpu_layers,
-        seed=args.seed,
-        n_batch=args.n_batch,
-        last_n_tokens_size=args.last_n_tokens_size
+        context_length=args.context_length,
+        gpu_layers=args.gpu_layers,
+        lib=args.lib,
+        model_type=args.model_type,
     )
 
     app.node = GenerationModelWorker(
         node_addr=args.worker_address,
         node_id=node_id,
         init_neighborhoods_addr=args.neighbors,
         executor=executor,
```

### Comparing `langport-0.1.0/langport/utils/__init__.py` & `langport-0.2.0/langport/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/utils/evaluation.py` & `langport-0.2.0/langport/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/utils/http_pool.py` & `langport-0.2.0/langport/utils/http_pool.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/utils/interval_timer.py` & `langport-0.2.0/langport/utils/interval_timer.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/workers/embedding_worker.py` & `langport-0.2.0/langport/workers/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport/workers/generation_worker.py` & `langport-0.2.0/langport/workers/generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.1.0/langport.egg-info/PKG-INFO` & `langport-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: langport
-Version: 0.1.0
-Summary: A large language model serving platform.
-Project-URL: Homepage, https://github.com/vtuber-plan/langport
-Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: llamacpp
-License-File: LICENSE
-
 <div align="center">
 
 # LangPort
 
 <a href="https://github.com/vtuber-plan/langport">
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/vtuber-plan/langport?style=social">
 </a>
@@ -29,14 +15,16 @@
 
 LangPort is a open-source large language model serving platform.
 Our goal is to build a super fast LLM inference service.
 
 This project is inspired by [lmsys/fastchat](https://github.com/lm-sys/FastChat), we hope that the serving platform is lightweight and fast, but fastchat includes other features such as training and evaluation make it complicated.
 
 The core features include:
+- Huggingface transformers support.
+- ggml (llama.cpp) support.
 - A distributed serving system for state-of-the-art models.
 - Streaming generation support with various decoding strategies.
 - Batch inference for higher throughput.
 - Support for encoder-only, decoder-only and encoder-decoder models.
 - OpenAI-compatible RESTful APIs.
 - FauxPilot-compatible RESTful APIs.
 - HuggingFace-compatible RESTful APIs.
@@ -46,14 +34,15 @@
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 
 ## News
+- [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
 - [2023/05/22] New distributed architecture.
 - [2023/05/14] Batch inference supported.
@@ -61,26 +50,31 @@
 
 
 ## Install
 
 ### Method 1: With pip
 
 ```bash
-pip3 install langport
+pip install langport
 ```
 
 or:
 
 ```bash
-pip3 install git+https://github.com/vtuber-plan/langport.git 
+pip install git+https://github.com/vtuber-plan/langport.git 
+```
+
+If you need ggml generation worker, use this command:
+```bash
+pip install langport[ggml]
 ```
 
-If you need llamacpp generation worker, use this command:
+If you wanna use GPU:
 ```bash
-pip3 install langport[llamacpp]
+CT_CUBLAS=1 pip install langport[ggml]
 ```
 
 ### Method 2: From source
 
 1. Clone this repository
 ```bash
 git clone https://github.com/vtuber-plan/langport.git
@@ -124,18 +118,18 @@
 Run text generation with multi GPUs:
 
 ``` bash
 python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpus 0,1 --num-gpus 2
 python -m langport.service.gateway.openai_api
 ```
 
-Run text generation with LLama.cpp worker:
+Run text generation with ggml worker:
 
 ```bash
-python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --n-gpu-layers <num layer to gpu (resize this for your VRAM)>
+python -m langport.service.server.generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
 ```
 
 ## License
 
 langport is released under the Apache Software License.
```

#### html2text {}

```diff
@@ -1,43 +1,39 @@
-Metadata-Version: 2.1 Name: langport Version: 0.1.0 Summary: A large language
-model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
-langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
-issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: llamacpp
-License-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
                                architecture.jpg)
 LangPort is a open-source large language model serving platform. Our goal is to
 build a super fast LLM inference service. This project is inspired by [lmsys/
 fastchat](https://github.com/lm-sys/FastChat), we hope that the serving
 platform is lightweight and fast, but fastchat includes other features such as
-training and evaluation make it complicated. The core features include: - A
-distributed serving system for state-of-the-art models. - Streaming generation
-support with various decoding strategies. - Batch inference for higher
-throughput. - Support for encoder-only, decoder-only and encoder-decoder
-models. - OpenAI-compatible RESTful APIs. - FauxPilot-compatible RESTful APIs.
-- HuggingFace-compatible RESTful APIs. - Tabby-compatible RESTful APIs. ##
-Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
-V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
-server, and the following figure shows the Queries Per Second (QPS) and Tokens
-Per Second (TPS) of FastChat and LangPort with different max model concurrency
-settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/09]
-Add LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding
-worker support. - [2023/06/01] Add HuggingFace text generation API support. -
-[2023/06/01] Add tabby API support. - [2023/05/23] Add chat throughput test
-script. - [2023/05/22] New distributed architecture. - [2023/05/14] Batch
-inference supported. - [2023/05/10] Langport project started. ## Install ###
-Method 1: With pip ```bash pip3 install langport ``` or: ```bash pip3 install
-git+https://github.com/vtuber-plan/langport.git ``` If you need llamacpp
-generation worker, use this command: ```bash pip3 install langport[llamacpp]
-``` ### Method 2: From source 1. Clone this repository ```bash git clone https:
-//github.com/vtuber-plan/langport.git cd langport ``` 2. Install the Package
-```bash pip install --upgrade pip pip install -e . ``` ## Start the server It
-is simple to start a single node chat API service: ``` bash python -
+training and evaluation make it complicated. The core features include: -
+Huggingface transformers support. - ggml (llama.cpp) support. - A distributed
+serving system for state-of-the-art models. - Streaming generation support with
+various decoding strategies. - Batch inference for higher throughput. - Support
+for encoder-only, decoder-only and encoder-decoder models. - OpenAI-compatible
+RESTful APIs. - FauxPilot-compatible RESTful APIs. - HuggingFace-compatible
+RESTful APIs. - Tabby-compatible RESTful APIs. ## Benchmark We use single
+RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16
+setting. We create 32 threads to submit chat tasks to the server, and the
+following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS)
+of FastChat and LangPort with different max model concurrency settings. !
+[benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18] Add ggml
+(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
+LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
+support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
+06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
+[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
+supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
+With pip ```bash pip install langport ``` or: ```bash pip install git+https://
+github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
+this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
+```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
+Clone this repository ```bash git clone https://github.com/vtuber-plan/
+langport.git cd langport ``` 2. Install the Package ```bash pip install --
+upgrade pip pip install -e . ``` ## Start the server It is simple to start a
+single node chat API service: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  python -
 m langport.service.gateway.openai_api ``` If you need the embeddings API or
 other features, you can deploy a distributed inference cluster: ``` bash python
 -m langport.service.server.dummy_worker --port 21001 python -
 m langport.service.server.generation_worker --model-path  --neighbors http://
 localhost:21001 python -m langport.service.server.embedding_worker --model-path
 --neighbors http://localhost:21001 python -
@@ -54,16 +50,16 @@
 neighbors http://localhost:21001 http://localhost:21004 python -
 m langport.service.gateway.openai_api --controller-address http://localhost:
 21003 # 21003 is OK! python -m langport.service.gateway.openai_api --
 controller-address http://localhost:21002 # Any worker is also OK! ``` Run text
 generation with multi GPUs: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  --gpus
 0,1 --num-gpus 2 python -m langport.service.gateway.openai_api ``` Run text
-generation with LLama.cpp worker: ```bash python -
-m langport.service.server.generation_worker --port 21001 --model-path  --n-gpu-
+generation with ggml worker: ```bash python -
+m langport.service.server.generation_worker --port 21001 --model-path  --gpu-
 layers
 resize this for your VRAM)> ``` ## License langport is released under the
 Apache Software License. ## See also - [langport-docs](https://github.com/
 vtuber-plan/langport/tree/main/docs) - [langport-source](https://github.com/
 vtuber-plan/langport) ## Star History [![Star History Chart](https://api.star-
 history.com/svg?repos=vtuber-plan/langport&type=Date)](https://star-
 history.com/#vtuber-plan/langport&Date)
```

### Comparing `langport-0.1.0/langport.egg-info/SOURCES.txt` & `langport-0.2.0/langport.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 langport/data/conversation/settings/billa.py
 langport/data/conversation/settings/chatgpt.py
 langport/data/conversation/settings/claude.py
 langport/data/conversation/settings/dolly.py
 langport/data/conversation/settings/falcon.py
 langport/data/conversation/settings/h2ogpt.py
 langport/data/conversation/settings/koala.py
-langport/data/conversation/settings/llama_cpp.py
 langport/data/conversation/settings/mpt.py
 langport/data/conversation/settings/oasst_pythia.py
 langport/data/conversation/settings/one_shot.py
 langport/data/conversation/settings/openbuddy.py
 langport/data/conversation/settings/phoenix.py
 langport/data/conversation/settings/redpajama.py
 langport/data/conversation/settings/rwkv.py
@@ -50,34 +49,33 @@
 langport/model/adapters/chatglm.py
 langport/model/adapters/chatgpt.py
 langport/model/adapters/claude.py
 langport/model/adapters/codegen.py
 langport/model/adapters/dolly_v2.py
 langport/model/adapters/falcon.py
 langport/model/adapters/koala.py
-langport/model/adapters/llama_cpp.py
 langport/model/adapters/oasst_pythia.py
 langport/model/adapters/openbuddy.py
 langport/model/adapters/phoenix.py
 langport/model/adapters/rwkv.py
 langport/model/adapters/stable_lm.py
 langport/model/adapters/starcoder.py
 langport/model/adapters/t5.py
 langport/model/adapters/text2vec.py
 langport/model/adapters/vicuna.py
 langport/model/executor/__init__.py
 langport/model/executor/base.py
+langport/model/executor/ggml.py
 langport/model/executor/huggingface.py
-langport/model/executor/llamacpp.py
 langport/model/executor/embedding/__init__.py
 langport/model/executor/embedding/huggingface.py
 langport/model/executor/generation/__init__.py
 langport/model/executor/generation/chatgpt.py
+langport/model/executor/generation/ggml.py
 langport/model/executor/generation/huggingface.py
-langport/model/executor/generation/llamacpp.py
 langport/model/models/__init__.py
 langport/model/models/rwkv_model.py
 langport/protocol/__init__.py
 langport/protocol/huggingface_api_protocol.py
 langport/protocol/openai_api_protocol.py
 langport/protocol/tabby_api_protocol.py
 langport/protocol/worker_protocol.py
```

### Comparing `langport-0.1.0/pyproject.toml` & `langport-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langport"
-version = "0.1.0"
+version = "0.2.0"
 description = "A large language model serving platform."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
@@ -17,15 +17,15 @@
     "rich>=10.0.0", "sentencepiece",
     "shortuuid", "shortuuid", "tokenizers>=0.12.1", "torch",
     "transformers>=4.28.0,<4.29.0", "uvicorn", "wandb", "tenacity>=8.2.2",
 ]
 
 [project.optional-dependencies]
 dev = ["black==23.3.0", "pylint==2.8.2"]
-llamacpp = ["llama-cpp-python"]
+ggml = ["ctransformers"]
 
 [project.urls]
 "Homepage" = "https://github.com/vtuber-plan/langport"
 "Bug Tracker" = "https://github.com/vtuber-plan/langport/issues"
 
 [tool.setuptools.packages.find]
 exclude = ["assets*", "benchmark*", "docs", "dist*", "playground*", "scripts*", "tests*"]
```

