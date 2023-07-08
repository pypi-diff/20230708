# Comparing `tmp/swarms-0.7.9.tar.gz` & `tmp/swarms-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.7.9.tar", last modified: Thu Jul  6 23:22:12 2023, max compression
+gzip compressed data, was "swarms-0.8.0.tar", last modified: Sat Jul  8 21:37:13 2023, max compression
```

## Comparing `swarms-0.7.9.tar` & `swarms-0.8.0.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.975728 swarms-0.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 23:22:00.000000 swarms-0.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 23:22:12.971727 swarms-0.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-07-06 23:22:00.000000 swarms-0.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.959727 swarms-0.7.9/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:01.000000 swarms-0.7.9/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-06 23:22:01.000000 swarms-0.7.9/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-06 23:22:01.000000 swarms-0.7.9/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-06 23:22:01.000000 swarms-0.7.9/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 23:22:12.975728 swarms-0.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-06 23:22:01.000000 swarms-0.7.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.959727 swarms-0.7.9/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.959727 swarms-0.7.9/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.959727 swarms-0.7.9/swarms/agents/boss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/boss/babyagi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/boss/boss_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.963727 swarms-0.7.9/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/auto_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/metaprompt_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.963727 swarms-0.7.9/swarms/agents/workers/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.963727 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.963727 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.963727 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.963727 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.963727 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.963727 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.967727 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.967727 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.967727 swarms-0.7.9/swarms/agents/workers/models/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.967727 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.971727 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.971727 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/models/segment_anything/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.971727 swarms-0.7.9/swarms/agents/workers/multi_modal_workers/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/multi_modal_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.971727 swarms-0.7.9/swarms/agents/workers/multi_modal_workers/omni_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    45882 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/omni_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/visual_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/agents/workers/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.971727 swarms-0.7.9/swarms/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.971727 swarms-0.7.9/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/tools/agent_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    71905 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.971727 swarms-0.7.9/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-06 23:22:01.000000 swarms-0.7.9/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:22:12.959727 swarms-0.7.9/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 23:22:12.000000 swarms-0.7.9/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-06 23:22:12.000000 swarms-0.7.9/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:22:12.000000 swarms-0.7.9/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-06 23:22:12.000000 swarms-0.7.9/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 23:22:12.000000 swarms-0.7.9/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.283095 swarms-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 21:37:03.000000 swarms-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-08 21:37:13.283095 swarms-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17658 2023-07-08 21:37:03.000000 swarms-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.251095 swarms-0.8.0/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-08 21:37:03.000000 swarms-0.8.0/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-08 21:37:03.000000 swarms-0.8.0/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-08 21:37:03.000000 swarms-0.8.0/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:37:13.283095 swarms-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-08 21:37:03.000000 swarms-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.251095 swarms-0.8.0/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.255095 swarms-0.8.0/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.255095 swarms-0.8.0/swarms/agents/boss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/boss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/boss/babyagi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/boss/boss_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.259095 swarms-0.8.0/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/auto_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/metaprompt_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.259095 swarms-0.8.0/swarms/agents/workers/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.259095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.259095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.259095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.263095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.263095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.267095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.267095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.271095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.271095 swarms-0.8.0/swarms/agents/workers/models/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.275095 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.275095 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.279095 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.279095 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.279095 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45882 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/omni_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/visual_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/worker_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.279095 swarms-0.8.0/swarms/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20151 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.283095 swarms-0.8.0/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/tools/agent_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71643 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.283095 swarms-0.8.0/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/utils/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.255095 swarms-0.8.0/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-08 21:37:13.000000 swarms-0.8.0/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-08 21:37:13.000000 swarms-0.8.0/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:37:13.000000 swarms-0.8.0/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-08 21:37:13.000000 swarms-0.8.0/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 21:37:13.000000 swarms-0.8.0/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.7.9/LICENSE` & `swarms-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/PKG-INFO` & `swarms-0.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.7.9
+Version: 0.8.0
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.7.9/README.md` & `swarms-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,33 +40,22 @@
 # Method1
 * Pip install `python3 -m pip install swarms`
 
 * Create new python file and unleash superintelligence
 
 ```python
 
-from swarms import Swarms
+from swarms import swarm
 
-# Retrieve your API key from the environment or replace with your actual key
-api_key = "sksdsds"
-
-# Initialize Swarms with your API key
-swarm = Swarms(openai_api_key=api_key)
+api_key = "api key for openai"
 
-# Define an objective
-objective = """
-Please develop and serve a simple community web service. 
-People can signup, login, post, comment. 
-Post and comment should be visible at once. 
-I want it to have neumorphism-style. 
-The ports you can use are 4500 and 6500.
-"""
+objective = "What is the capital of the Uk"
 
-# Run Swarms
-swarm.run_swarms(objective)
+result = swarm(api_key, objective)
+print(result)
 ```
 
 # Method 2
 Download via Github, and install requirements. Simple example by:
 
 * `git cloning https://github.com/kyegomez/swarms.git`
 
@@ -127,28 +116,37 @@
 
 # Open Source Roadmap
 
 Here is the detailed roadmap of our priorities and planned features for the near term:
 
 ## TODO
 
+
+* Make sure that the boss agent successfully calls the worker agent if when it's finished makinng a plan
+
+* Make sure the worker agent can access tools like web browser, terminal, and code editor, and multi-modal agents
+
+* Make sure inputs and outputs from boss to worker are well defined and are collaborating if not then readjust prompt
+
 * Create a tool that creates other tools with access to write code, debug, and an architectural argent that creates the architecture and then another agent that creates the code[Architecter(with code examples), code generator (with access to writing code and terminalrools)] -- The Compiler?
 
 * Create a screenshot tool that takes a screen shot and then passes it to a worker multi-modal agent for visual context.
 
 * API endroute in FASTAPI
 
 * Develop Conversational UI with Gradio
 
 * Integrate omni agent as a worker tool
 
 * Integrate Ocean Database as primary vectorstore
 
 * Integrate visual agent
 
+* Integrate quantized hf models as base models with langchain huggingface
+
 1. **Multi-Agent Debate Integration**: Integrate multi-agent debate frameworks ([Multi Agent debate](https://github.com/Skytliang/Multi-Agents-Debate) and [Multi agent2 debate](https://github.com/composable-models/llm_multiagent_debate)) to improve decision-making.
 
 2. **Meta Prompting Integration**: Include meta prompting across all worker agents to guide their actions.
 
 3. **Swarms Class**: Create a main swarms class `swarms('Increase sales by 40$', workers=4)` for managing and coordinating multiple worker nodes.
 
 4. **Integration of Additional Tools**: Integrate [Jarvis](https://github.com/microsoft/JARVIS) as worker nodes, add text to speech and text to script tools ([whisper x](https://github.com/kyegomez/youtubeURL-to-text)), and integrate Hugging Face agents and other external tools.
```

### Comparing `swarms-0.7.9/api/container.py` & `swarms-0.8.0/api/container.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-
 import os
 import re
 from pathlib import Path
 from typing import Dict, List
 
 from fastapi.templating import Jinja2Templates
 
-from swarms.agents.workers.agents import AgentManager
+from swarms import Swarms
 from swarms.utils.utils import BaseHandler, FileHandler, FileType, StaticUploader, CsvToDataframe
 
 from swarms.tools.main import BaseToolSet, ExitConversation, RequestsGet, CodeEditor, Terminal
 
-from env import settings
-
 
 BASE_DIR = Path(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-os.chdir(BASE_DIR / os.getenv["PLAYGROUND_DIR"])
+os.chdir(BASE_DIR / os.getenv("PLAYGROUND_DIR"))
 
+api_key = os.getenv("OPENAI_API_KEY")
 
 toolsets: List[BaseToolSet] = [
     Terminal(),
     CodeEditor(),
     RequestsGet(),
     ExitConversation(),
 ]
 handlers: Dict[FileType, BaseHandler] = {FileType.DATAFRAME: CsvToDataframe()}
 
-if os.getenv["USE_GPU"]:
+if os.getenv("USE_GPU") == "True":
     import torch
 
     from swarms.tools.main import ImageCaptioning
     from swarms.tools.main import (
         ImageEditing,
         InstructPix2Pix,
         Text2Image,
@@ -44,18 +42,20 @@
                 ImageEditing("cuda"),
                 InstructPix2Pix("cuda"),
                 VisualQuestionAnswering("cuda"),
             ]
         )
         handlers[FileType.IMAGE] = ImageCaptioning("cuda")
 
-agent_manager = AgentManager.create(toolsets=toolsets)
+swarms = Swarms(api_key)
 
 file_handler = FileHandler(handlers=handlers, path=BASE_DIR)
 
 templates = Jinja2Templates(directory=BASE_DIR / "api" / "templates")
 
-uploader = StaticUploader.from_settings(
-    settings, path=BASE_DIR / "static", endpoint="static"
+uploader = StaticUploader(
+    static_dir=BASE_DIR / "static",
+    endpoint="static",
+    public_url=os.getenv("PUBLIC_URL")
 )
 
-reload_dirs = [BASE_DIR / "swarms", BASE_DIR / "api"]
+reload_dirs = [BASE_DIR / "swarms", BASE_DIR / "api"]
```

### Comparing `swarms-0.7.9/api/worker.py` & `swarms-0.8.0/api/worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from celery import Celery
 from celery.result import AsyncResult
 
-from api.container import agent_manager
-# from env import settings
+from api.container import swarms
 
-celery_broker = os.environ["CELERY_BROKER_URL"]
+celery_broker = os.getenv("CELERY_BROKER_URL", "")
 
 
 celery_app = Celery(__name__)
 celery_app.conf.broker_url = celery_broker
 celery_app.conf.result_backend = celery_broker
 celery_app.conf.update(
     task_track_started=True,
@@ -18,15 +17,15 @@
     result_serializer="json",
     enable_utc=True,
 )
 
 
 @celery_app.task(name="task_execute", bind=True)
 def task_execute(self, session: str, prompt: str):
-    executor = agent_manager.create_executor(session, self)
+    executor = swarms.create_executor(session, self)
     response = executor({"input": prompt})
     result = {"output": response["output"]}
 
     previous = AsyncResult(self.request.id)
     if previous and previous.info:
         result.update(previous.info)
 
@@ -39,8 +38,8 @@
 
 def start_worker():
     celery_app.worker_main(
         [
             "worker",
             "--loglevel=INFO",
         ]
-    )
+    )
```

### Comparing `swarms-0.7.9/setup.py` & `swarms-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.7.9',
+  version = '0.8.0',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.7.9/swarms/agents/boss/babyagi_agent.py` & `swarms-0.8.0/swarms/agents/boss/babyagi_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/boss/boss_agent.py` & `swarms-0.8.0/swarms/agents/boss/boss_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/agents.py` & `swarms-0.8.0/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/auto_worker.py` & `swarms-0.8.0/swarms/agents/workers/auto_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/metaprompt_worker.py` & `swarms-0.8.0/swarms/agents/workers/metaprompt_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/GroundingDINO/setup.py` & `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/__init__.py` & `swarms-0.8.0/swarms/agents/workers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/models/segment_anything/setup.py` & `swarms-0.8.0/swarms/agents/workers/models/segment_anything/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py` & `swarms-0.8.0/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py` & `swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py` & `swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py` & `swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/omni_worker.py` & `swarms-0.8.0/swarms/agents/workers/omni_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/agents/workers/visual_worker.py` & `swarms-0.8.0/swarms/agents/workers/visual_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/prompts/prompts.py` & `swarms-0.8.0/swarms/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms/swarms.py` & `swarms-0.8.0/swarms/swarms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from swarms.tools.agent_tools import *
-from swarms.agents.workers.worker import WorkerNode
+from swarms.agents.workers.worker_agent import WorkerNode
 from swarms.agents.boss.boss_agent import BossNode
 # from swarms.agents.workers.omni_worker import OmniWorkerAgent
 # from swarms.tools.main import RequestsGet, ExitConversation
 # visual agent
 
-from swarms.agents.workers.worker import worker_tool
+from swarms.agents.workers.worker_agent import worker_tool
 import logging
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
 class Swarms:
     def __init__(self, openai_api_key):
         self.openai_api_key = openai_api_key
@@ -118,14 +118,169 @@
 
 
 
 
 
 
 
+# usage
+def swarm(api_key, objective):
+    swarms = Swarms(api_key)
+    return swarms.run_swarms(objective)
+
+# # Use the function
+# api_key = "APIKEY"
+# objective = "What is the capital of the UK?"
+# result = swarm(api_key, objective)
+# print(result)  # Prints: "The capital of the UK is London."
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+# class Swarms:
+#     def __init__(self, openai_api_key):
+#         self.openai_api_key = openai_api_key
+
+#     def initialize_llm(self, llm_class, temperature=0.5):
+#         # Initialize language model
+#         return llm_class(openai_api_key=self.openai_api_key, temperature=temperature)
+
+#     def initialize_tools(self, llm_class):
+#         llm = self.initialize_llm(llm_class)
+#         # Initialize tools
+#         web_search = DuckDuckGoSearchRun()
+#         tools = [
+#             web_search,
+#             WriteFileTool(root_dir=ROOT_DIR),
+#             ReadFileTool(root_dir=ROOT_DIR),
+
+#             process_csv,
+#             WebpageQATool(qa_chain=load_qa_with_sources_chain(llm)),
+
+#             # RequestsGet()
+#             Tool(name="RequestsGet", func=RequestsGet.get, description="A portal to the internet, Use this when you need to get specific content from a website. Input should be a  url (i.e. https://www.google.com). The output will be the text response of the GET request."),
+
+            
+#             # CodeEditor,
+#             # Terminal,
+#             # RequestsGet,
+#             # ExitConversation
+
+#             #code editor + terminal editor + visual agent
+#             # Give the worker node itself as a tool
+
+#         ]
+#         assert tools is not None, "tools is not initialized"
+#         return tools
+
+#     def initialize_vectorstore(self):
+#         # Initialize vector store
+#         embeddings_model = OpenAIEmbeddings(openai_api_key=self.openai_api_key)
+#         embedding_size = 1536
+#         index = faiss.IndexFlatL2(embedding_size)
+#         return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
+
+#     def initialize_worker_node(self, worker_tools, vectorstore):
+#         # Initialize worker node
+#         llm = self.initialize_llm(ChatOpenAI)
+#         worker_node = WorkerNode(llm=llm, tools=worker_tools, vectorstore=vectorstore)
+#         worker_node.create_agent(ai_name="Swarm Worker AI Assistant", ai_role="Assistant", human_in_the_loop=False, search_kwargs={})
+#         worker_node_tool = Tool(name="WorkerNode AI Agent", func=worker_node.run, description="Input: an objective with a todo list for that objective. Output: your task completed: Please be very clear what the objective and task instructions are. The Swarm worker agent is Useful for when you need to spawn an autonomous agent instance as a worker to accomplish any complex tasks, it can search the internet or write code or spawn child multi-modality models to process and generate images and text or audio and so on")
+#         return worker_node_tool
+
+#     def initialize_boss_node(self, vectorstore, worker_node):
+#         # Initialize boss node
+#         llm = self.initialize_llm(OpenAI)
+#         todo_prompt = PromptTemplate.from_template("You are a boss planer in a swarm who is an expert at coming up with a todo list for a given objective and then creating an worker to help you accomplish your task. Come up with a todo list for this objective: {objective} and then spawn a worker agent to complete the task for you. Always spawn an worker agent after creating a plan and pass the objective and plan to the worker agent.")
+#         todo_chain = LLMChain(llm=llm, prompt=todo_prompt)
+#         tools = [
+#             Tool(name="TODO", func=todo_chain.run, description="useful for when you need to come up with todo lists. Input: an objective to create a todo list for. Output: a todo list for that objective. Please be very clear what the objective is!"),
+#             worker_node
+#         ]
+#         suffix = """Question: {task}\n{agent_scratchpad}"""
+#         prefix = """You are an Boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n """
+#         prompt = ZeroShotAgent.create_prompt(tools, prefix=prefix, suffix=suffix, input_variables=["objective", "task", "context", "agent_scratchpad"],)
+#         llm_chain = LLMChain(llm=llm, prompt=prompt)
+#         agent = ZeroShotAgent(llm_chain=llm_chain, allowed_tools=[tool.name for tool in tools])
+#         agent_executor = AgentExecutor.from_agent_and_tools(agent=agent, tools=tools, verbose=True)
+#         # return BossNode(return BossNode(llm, vectorstore, agent_executor, max_iterations=5)
+#         return BossNode(llm, vectorstore, agent_executor, max_iterations=5)
+
+
+#     def run_swarms(self, objective, run_as=None):
+#         try:
+#             # Run the swarm with the given objective
+#             worker_tools = self.initialize_tools(OpenAI)
+#             assert worker_tools is not None, "worker_tools is not initialized"
+
+#             vectorstore = self.initialize_vectorstore()
+#             worker_node = self.initialize_worker_node(worker_tools, vectorstore)
+
+#             if run_as.lower() == 'worker':
+#                 tool_input = {'prompt': objective}
+#                 return worker_node.run(tool_input)
+#             else:
+#                 boss_node = self.initialize_boss_node(vectorstore, worker_node)
+#                 task = boss_node.create_task(objective)
+#                 return boss_node.execute_task(task)
+#         except Exception as e:
+#             logging.error(f"An error occurred in run_swarms: {e}")
+#             raise
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 
 
 
 
 
 
 
@@ -209,29 +364,14 @@
 #         task = boss_node.create_task(objective)
 #         boss_node.execute_task(task)
 #         worker_node.run_agent(objective)
 
 
 
 
-# usage
-def swarm(api_key, objective):
-    swarms = Swarms(api_key)
-    return swarms.run_swarms(objective)
-
-# # Use the function
-# api_key = "APIKEY"
-# objective = "What is the capital of the UK?"
-# result = swarm(api_key, objective)
-# print(result)  # Prints: "The capital of the UK is London."
-
-
-
-
-
```

### Comparing `swarms-0.7.9/swarms/tools/main.py` & `swarms-0.8.0/swarms/tools/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,32 +13,23 @@
 from langchain.chat_models import ChatOpenAI
 
 
 import requests
 from bs4 import BeautifulSoup
 
 
-# import llama_index
-# from llama_index import GPTVectorStoreIndex
-# from llama_index.readers.database import DatabaseReader
-
-# from logger import logger
 
 from swarms.utils.logger import logger
 class ToolScope(Enum):
     GLOBAL = "global"
     SESSION = "session"
 
 
 SessionGetter = Callable[[], Tuple[str, AgentExecutor]]
 
-# openai_api_key = os.environ["OPENAI_API_KEY"]
-# llm = ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key=openai_api_key)
-
-
 def tool(
     name: str,
     description: str,
     scope: ToolScope = ToolScope.GLOBAL,
 ):
     def decorator(func):
         func.name = name
@@ -87,21 +78,21 @@
         ]
         return [ToolWrapper(m.name, m.description, m.scope, m) for m in methods]
     
 
 
 
 class RequestsGet(BaseToolSet):
-    @tool(
-        name="Requests Get",
-        description="A portal to the internet. "
-        "Use this when you need to get specific content from a website."
-        "Input should be a  url (i.e. https://www.google.com)."
-        "The output will be the text response of the GET request.",
-    )
+    # @tool(
+    #     name="Requests Get",
+    #     description="A portal to the internet. "
+    #     "Use this when you need to get specific content from a website."
+    #     "Input should be a  url (i.e. https://www.google.com)."
+    #     "The output will be the text response of the GET request.",
+    # )
     def get(self, url: str) -> str:
         """Run the tool."""
         html = requests.get(url).text
         soup = BeautifulSoup(html)
         non_readable_tags = soup.find_all(
             ["script", "style", "header", "footer", "form"]
         )
@@ -1064,15 +1055,15 @@
     @tool(
         name="CodeEditor.DELETE",
         description="Delete code in file for a new start. "
         "Input should be filename."
         "ex. test.py "
         "Output will be success or error message.",
     )
-    def delete(self, inputs: str) -> str:
+    def delete(self, inputs: str, filepath: str) -> str:
         try:
             with open(filepath, "w") as f:
                 f.write("")
             output = "success"
         except Exception as e:
             output = str(e)
```

### Comparing `swarms-0.7.9/swarms/utils/utils.py` & `swarms-0.8.0/swarms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.7.9/swarms.egg-info/PKG-INFO` & `swarms-0.8.0/swarms.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.7.9
+Version: 0.8.0
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.7.9/swarms.egg-info/SOURCES.txt` & `swarms-0.8.0/swarms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 swarms/agents/boss/boss_agent.py
 swarms/agents/workers/__init__.py
 swarms/agents/workers/agents.py
 swarms/agents/workers/auto_worker.py
 swarms/agents/workers/metaprompt_worker.py
 swarms/agents/workers/omni_worker.py
 swarms/agents/workers/visual_worker.py
-swarms/agents/workers/worker.py
+swarms/agents/workers/worker_agent.py
 swarms/agents/workers/models/__init__.py
 swarms/agents/workers/models/GroundingDINO/__init__.py
 swarms/agents/workers/models/GroundingDINO/setup.py
 swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
 swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
 swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
 swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
@@ -84,9 +84,10 @@
 swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
 swarms/prompts/__init__.py
 swarms/prompts/prompts.py
 swarms/tools/__init__.py
 swarms/tools/agent_tools.py
 swarms/tools/main.py
 swarms/utils/__init__.py
+swarms/utils/llm.py
 swarms/utils/logger.py
 swarms/utils/utils.py
```

### Comparing `swarms-0.7.9/swarms.egg-info/requires.txt` & `swarms-0.8.0/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

