# Comparing `tmp/autochain-0.0.1.tar.gz` & `tmp/autochain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autochain-0.0.1.tar", max compression
+gzip compressed data, was "autochain-0.0.2.tar", max compression
```

## Comparing `autochain-0.0.1.tar` & `autochain-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,68 @@
--rw-r--r--   0        0        0        0 2023-06-16 17:31:51.700852 autochain-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-16 17:31:51.700794 autochain-0.0.1/autochain/__init__.py
--rw-r--r--   0        0        0      433 2023-06-16 17:32:30.350171 autochain-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 autochain-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-27 17:21:47.749193 autochain-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     6830 2023-07-08 21:25:57.129750 autochain-0.0.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-27 17:21:47.758861 autochain-0.0.2/autochain/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.947303 autochain-0.0.2/autochain/agent/__init__.py
+-rw-r--r--   0        0        0     3843 2023-07-03 18:01:35.208652 autochain-0.0.2/autochain/agent/base_agent.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.947544 autochain-0.0.2/autochain/agent/conversational_agent/__init__.py
+-rw-r--r--   0        0        0     9365 2023-07-03 18:01:35.209140 autochain-0.0.2/autochain/agent/conversational_agent/conversational_agent.py
+-rw-r--r--   0        0        0     1723 2023-06-27 17:21:47.796089 autochain-0.0.2/autochain/agent/conversational_agent/output_parser.py
+-rw-r--r--   0        0        0     2300 2023-07-08 21:24:43.160600 autochain-0.0.2/autochain/agent/conversational_agent/prompt.py
+-rw-r--r--   0        0        0      192 2023-06-27 17:21:47.864519 autochain-0.0.2/autochain/agent/conversational_agent/readme.md
+-rw-r--r--   0        0        0     2988 2023-07-03 18:01:35.209804 autochain-0.0.2/autochain/agent/message.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:47.713048 autochain-0.0.2/autochain/agent/openai_funtions_agent/__init__.py
+-rw-r--r--   0        0        0     2866 2023-07-03 18:01:35.210284 autochain-0.0.2/autochain/agent/openai_funtions_agent/openai_functions_agent.py
+-rw-r--r--   0        0        0      718 2023-06-27 17:21:47.846783 autochain-0.0.2/autochain/agent/openai_funtions_agent/output_parser.py
+-rw-r--r--   0        0        0      226 2023-06-27 17:21:47.847035 autochain-0.0.2/autochain/agent/openai_funtions_agent/readme.md
+-rw-r--r--   0        0        0      842 2023-06-27 17:21:47.864856 autochain-0.0.2/autochain/agent/prompt_formatter.py
+-rw-r--r--   0        0        0     2633 2023-07-03 18:01:35.210734 autochain-0.0.2/autochain/agent/structs.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.948601 autochain-0.0.2/autochain/chain/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-03 18:05:28.426791 autochain-0.0.2/autochain/chain/base_chain.py
+-rw-r--r--   0        0        0     4352 2023-07-03 18:01:35.211429 autochain-0.0.2/autochain/chain/chain.py
+-rw-r--r--   0        0        0      149 2023-06-27 17:21:47.715223 autochain-0.0.2/autochain/chain/constants.py
+-rw-r--r--   0        0        0     1183 2023-07-03 18:01:35.211793 autochain-0.0.2/autochain/chain/langchain_wrapper_chain.py
+-rw-r--r--   0        0        0      554 2023-06-27 17:21:43.949077 autochain-0.0.2/autochain/errors.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.949163 autochain-0.0.2/autochain/examples/__init__.py
+-rw-r--r--   0        0        0      978 2023-07-08 21:24:43.160949 autochain-0.0.2/autochain/examples/get_weather_with_conversational_agent.py
+-rw-r--r--   0        0        0     1292 2023-07-08 21:24:43.161287 autochain-0.0.2/autochain/examples/get_weather_with_openai_function_agent.py
+-rw-r--r--   0        0        0      445 2023-06-27 20:00:44.804353 autochain-0.0.2/autochain/examples/readme.md
+-rw-r--r--   0        0        0      820 2023-07-08 21:24:43.161595 autochain-0.0.2/autochain/examples/upsale_goal_conversational_agent.py
+-rw-r--r--   0        0        0      620 2023-07-08 21:24:43.162082 autochain-0.0.2/autochain/examples/write_poem_with_conversational_agent.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.949446 autochain-0.0.2/autochain/memory/__init__.py
+-rw-r--r--   0        0        0     1145 2023-06-27 17:21:47.715981 autochain-0.0.2/autochain/memory/base.py
+-rw-r--r--   0        0        0     1321 2023-07-03 18:01:35.212974 autochain-0.0.2/autochain/memory/buffer_memory.py
+-rw-r--r--   0        0        0       16 2023-07-03 18:05:28.427082 autochain-0.0.2/autochain/memory/constants.py
+-rw-r--r--   0        0        0     2358 2023-07-03 18:01:35.213321 autochain-0.0.2/autochain/memory/long_term_memory.py
+-rw-r--r--   0        0        0     2834 2023-07-08 03:23:01.738016 autochain-0.0.2/autochain/memory/redis_memory.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.949725 autochain-0.0.2/autochain/models/__init__.py
+-rw-r--r--   0        0        0     2024 2023-06-27 17:21:47.759100 autochain-0.0.2/autochain/models/ada_embedding.py
+-rw-r--r--   0        0        0     4762 2023-06-27 17:21:47.759372 autochain-0.0.2/autochain/models/base.py
+-rw-r--r--   0        0        0     7669 2023-07-03 18:01:35.213652 autochain-0.0.2/autochain/models/chat_openai.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950002 autochain-0.0.2/autochain/py.typed
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950070 autochain-0.0.2/autochain/tools/__init__.py
+-rw-r--r--   0        0        0     3829 2023-07-03 18:01:35.214111 autochain-0.0.2/autochain/tools/base.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950229 autochain-0.0.2/autochain/tools/google_search/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-27 17:21:43.950338 autochain-0.0.2/autochain/tools/google_search/tool.py
+-rw-r--r--   0        0        0     4900 2023-06-27 17:21:43.950442 autochain-0.0.2/autochain/tools/google_search/util.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950493 autochain-0.0.2/autochain/tools/internal_search/__init__.py
+-rw-r--r--   0        0        0     2201 2023-06-27 17:21:47.835514 autochain-0.0.2/autochain/tools/internal_search/chromadb_tool.py
+-rw-r--r--   0        0        0     2226 2023-06-27 17:21:47.848764 autochain-0.0.2/autochain/tools/internal_search/pinecone_tool.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950648 autochain-0.0.2/autochain/tools/simple_handoff/__init__.py
+-rw-r--r--   0        0        0      303 2023-07-08 21:24:43.162458 autochain-0.0.2/autochain/tools/simple_handoff/tool.py
+-rw-r--r--   0        0        0     1595 2023-07-08 21:24:43.162779 autochain-0.0.2/autochain/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950856 autochain-0.0.2/autochain/workflows_evaluation/__init__.py
+-rw-r--r--   0        0        0     7038 2023-07-08 21:24:43.163350 autochain-0.0.2/autochain/workflows_evaluation/base_test.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:47.865309 autochain-0.0.2/autochain/workflows_evaluation/conversational_agent_eval/__init__.py
+-rw-r--r--   0        0        0     3772 2023-07-08 21:24:43.163698 autochain-0.0.2/autochain/workflows_evaluation/conversational_agent_eval/change_shipping_address_test.py
+-rw-r--r--   0        0        0     3206 2023-07-08 21:24:43.164014 autochain-0.0.2/autochain/workflows_evaluation/conversational_agent_eval/generate_ads_test.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:47.739513 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/__init__.py
+-rw-r--r--   0        0        0     3355 2023-07-08 21:24:43.164441 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/change_shipping_address_test.py
+-rw-r--r--   0        0        0     1150 2023-07-08 03:23:01.739765 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/custom_langchain_output_parser.py
+-rw-r--r--   0        0        0     3520 2023-07-08 21:24:43.164777 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/generate_ads_test.py
+-rw-r--r--   0        0        0     1546 2023-07-08 03:23:01.740220 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/langchain_test_utils.py
+-rw-r--r--   0        0        0      704 2023-07-08 03:23:01.740419 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/readme.md
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:47.716600 autochain-0.0.2/autochain/workflows_evaluation/openai_function_agent_eval/__init__.py
+-rw-r--r--   0        0        0     3986 2023-07-08 21:24:43.165214 autochain-0.0.2/autochain/workflows_evaluation/openai_function_agent_eval/change_shipping_address_test.py
+-rw-r--r--   0        0        0     3513 2023-07-08 21:24:43.165568 autochain-0.0.2/autochain/workflows_evaluation/openai_function_agent_eval/generate_ads_test.py
+-rw-r--r--   0        0        0     1531 2023-07-08 21:24:43.165898 autochain-0.0.2/autochain/workflows_evaluation/test_utils.py
+-rw-r--r--   0        0        0     2712 2023-07-08 21:31:58.610782 autochain-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8947 1970-01-01 00:00:00.000000 autochain-0.0.2/PKG-INFO
```

