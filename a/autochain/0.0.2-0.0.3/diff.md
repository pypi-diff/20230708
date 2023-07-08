# Comparing `tmp/autochain-0.0.2.tar.gz` & `tmp/autochain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autochain-0.0.2.tar", max compression
+gzip compressed data, was "autochain-0.0.3.tar", max compression
```

## Comparing `autochain-0.0.2.tar` & `autochain-0.0.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1069 2023-06-27 17:21:47.749193 autochain-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     6830 2023-07-08 21:25:57.129750 autochain-0.0.2/README.md
--rw-r--r--   0        0        0       22 2023-06-27 17:21:47.758861 autochain-0.0.2/autochain/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.947303 autochain-0.0.2/autochain/agent/__init__.py
--rw-r--r--   0        0        0     3843 2023-07-03 18:01:35.208652 autochain-0.0.2/autochain/agent/base_agent.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.947544 autochain-0.0.2/autochain/agent/conversational_agent/__init__.py
--rw-r--r--   0        0        0     9365 2023-07-03 18:01:35.209140 autochain-0.0.2/autochain/agent/conversational_agent/conversational_agent.py
--rw-r--r--   0        0        0     1723 2023-06-27 17:21:47.796089 autochain-0.0.2/autochain/agent/conversational_agent/output_parser.py
--rw-r--r--   0        0        0     2300 2023-07-08 21:24:43.160600 autochain-0.0.2/autochain/agent/conversational_agent/prompt.py
--rw-r--r--   0        0        0      192 2023-06-27 17:21:47.864519 autochain-0.0.2/autochain/agent/conversational_agent/readme.md
--rw-r--r--   0        0        0     2988 2023-07-03 18:01:35.209804 autochain-0.0.2/autochain/agent/message.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:47.713048 autochain-0.0.2/autochain/agent/openai_funtions_agent/__init__.py
--rw-r--r--   0        0        0     2866 2023-07-03 18:01:35.210284 autochain-0.0.2/autochain/agent/openai_funtions_agent/openai_functions_agent.py
--rw-r--r--   0        0        0      718 2023-06-27 17:21:47.846783 autochain-0.0.2/autochain/agent/openai_funtions_agent/output_parser.py
--rw-r--r--   0        0        0      226 2023-06-27 17:21:47.847035 autochain-0.0.2/autochain/agent/openai_funtions_agent/readme.md
--rw-r--r--   0        0        0      842 2023-06-27 17:21:47.864856 autochain-0.0.2/autochain/agent/prompt_formatter.py
--rw-r--r--   0        0        0     2633 2023-07-03 18:01:35.210734 autochain-0.0.2/autochain/agent/structs.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.948601 autochain-0.0.2/autochain/chain/__init__.py
--rw-r--r--   0        0        0     7175 2023-07-03 18:05:28.426791 autochain-0.0.2/autochain/chain/base_chain.py
--rw-r--r--   0        0        0     4352 2023-07-03 18:01:35.211429 autochain-0.0.2/autochain/chain/chain.py
--rw-r--r--   0        0        0      149 2023-06-27 17:21:47.715223 autochain-0.0.2/autochain/chain/constants.py
--rw-r--r--   0        0        0     1183 2023-07-03 18:01:35.211793 autochain-0.0.2/autochain/chain/langchain_wrapper_chain.py
--rw-r--r--   0        0        0      554 2023-06-27 17:21:43.949077 autochain-0.0.2/autochain/errors.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.949163 autochain-0.0.2/autochain/examples/__init__.py
--rw-r--r--   0        0        0      978 2023-07-08 21:24:43.160949 autochain-0.0.2/autochain/examples/get_weather_with_conversational_agent.py
--rw-r--r--   0        0        0     1292 2023-07-08 21:24:43.161287 autochain-0.0.2/autochain/examples/get_weather_with_openai_function_agent.py
--rw-r--r--   0        0        0      445 2023-06-27 20:00:44.804353 autochain-0.0.2/autochain/examples/readme.md
--rw-r--r--   0        0        0      820 2023-07-08 21:24:43.161595 autochain-0.0.2/autochain/examples/upsale_goal_conversational_agent.py
--rw-r--r--   0        0        0      620 2023-07-08 21:24:43.162082 autochain-0.0.2/autochain/examples/write_poem_with_conversational_agent.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.949446 autochain-0.0.2/autochain/memory/__init__.py
--rw-r--r--   0        0        0     1145 2023-06-27 17:21:47.715981 autochain-0.0.2/autochain/memory/base.py
--rw-r--r--   0        0        0     1321 2023-07-03 18:01:35.212974 autochain-0.0.2/autochain/memory/buffer_memory.py
--rw-r--r--   0        0        0       16 2023-07-03 18:05:28.427082 autochain-0.0.2/autochain/memory/constants.py
--rw-r--r--   0        0        0     2358 2023-07-03 18:01:35.213321 autochain-0.0.2/autochain/memory/long_term_memory.py
--rw-r--r--   0        0        0     2834 2023-07-08 03:23:01.738016 autochain-0.0.2/autochain/memory/redis_memory.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.949725 autochain-0.0.2/autochain/models/__init__.py
--rw-r--r--   0        0        0     2024 2023-06-27 17:21:47.759100 autochain-0.0.2/autochain/models/ada_embedding.py
--rw-r--r--   0        0        0     4762 2023-06-27 17:21:47.759372 autochain-0.0.2/autochain/models/base.py
--rw-r--r--   0        0        0     7669 2023-07-03 18:01:35.213652 autochain-0.0.2/autochain/models/chat_openai.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950002 autochain-0.0.2/autochain/py.typed
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950070 autochain-0.0.2/autochain/tools/__init__.py
--rw-r--r--   0        0        0     3829 2023-07-03 18:01:35.214111 autochain-0.0.2/autochain/tools/base.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950229 autochain-0.0.2/autochain/tools/google_search/__init__.py
--rw-r--r--   0        0        0      728 2023-06-27 17:21:43.950338 autochain-0.0.2/autochain/tools/google_search/tool.py
--rw-r--r--   0        0        0     4900 2023-06-27 17:21:43.950442 autochain-0.0.2/autochain/tools/google_search/util.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950493 autochain-0.0.2/autochain/tools/internal_search/__init__.py
--rw-r--r--   0        0        0     2201 2023-06-27 17:21:47.835514 autochain-0.0.2/autochain/tools/internal_search/chromadb_tool.py
--rw-r--r--   0        0        0     2226 2023-06-27 17:21:47.848764 autochain-0.0.2/autochain/tools/internal_search/pinecone_tool.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950648 autochain-0.0.2/autochain/tools/simple_handoff/__init__.py
--rw-r--r--   0        0        0      303 2023-07-08 21:24:43.162458 autochain-0.0.2/autochain/tools/simple_handoff/tool.py
--rw-r--r--   0        0        0     1595 2023-07-08 21:24:43.162779 autochain-0.0.2/autochain/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950856 autochain-0.0.2/autochain/workflows_evaluation/__init__.py
--rw-r--r--   0        0        0     7038 2023-07-08 21:24:43.163350 autochain-0.0.2/autochain/workflows_evaluation/base_test.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:47.865309 autochain-0.0.2/autochain/workflows_evaluation/conversational_agent_eval/__init__.py
--rw-r--r--   0        0        0     3772 2023-07-08 21:24:43.163698 autochain-0.0.2/autochain/workflows_evaluation/conversational_agent_eval/change_shipping_address_test.py
--rw-r--r--   0        0        0     3206 2023-07-08 21:24:43.164014 autochain-0.0.2/autochain/workflows_evaluation/conversational_agent_eval/generate_ads_test.py
--rw-r--r--   0        0        0        0 2023-06-27 17:21:47.739513 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/__init__.py
--rw-r--r--   0        0        0     3355 2023-07-08 21:24:43.164441 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/change_shipping_address_test.py
--rw-r--r--   0        0        0     1150 2023-07-08 03:23:01.739765 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/custom_langchain_output_parser.py
--rw-r--r--   0        0        0     3520 2023-07-08 21:24:43.164777 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/generate_ads_test.py
--rw-r--r--   0        0        0     1546 2023-07-08 03:23:01.740220 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/langchain_test_utils.py
--rw-r--r--   0        0        0      704 2023-07-08 03:23:01.740419 autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/readme.md
--rw-r--r--   0        0        0        0 2023-06-27 17:21:47.716600 autochain-0.0.2/autochain/workflows_evaluation/openai_function_agent_eval/__init__.py
--rw-r--r--   0        0        0     3986 2023-07-08 21:24:43.165214 autochain-0.0.2/autochain/workflows_evaluation/openai_function_agent_eval/change_shipping_address_test.py
--rw-r--r--   0        0        0     3513 2023-07-08 21:24:43.165568 autochain-0.0.2/autochain/workflows_evaluation/openai_function_agent_eval/generate_ads_test.py
--rw-r--r--   0        0        0     1531 2023-07-08 21:24:43.165898 autochain-0.0.2/autochain/workflows_evaluation/test_utils.py
--rw-r--r--   0        0        0     2712 2023-07-08 21:31:58.610782 autochain-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8947 1970-01-01 00:00:00.000000 autochain-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-27 17:21:47.749193 autochain-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     6830 2023-07-08 21:25:57.129750 autochain-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2023-06-27 17:21:47.758861 autochain-0.0.3/autochain/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.947303 autochain-0.0.3/autochain/agent/__init__.py
+-rw-r--r--   0        0        0     3843 2023-07-03 18:01:35.208652 autochain-0.0.3/autochain/agent/base_agent.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.947544 autochain-0.0.3/autochain/agent/conversational_agent/__init__.py
+-rw-r--r--   0        0        0     9365 2023-07-03 18:01:35.209140 autochain-0.0.3/autochain/agent/conversational_agent/conversational_agent.py
+-rw-r--r--   0        0        0     1723 2023-06-27 17:21:47.796089 autochain-0.0.3/autochain/agent/conversational_agent/output_parser.py
+-rw-r--r--   0        0        0     2300 2023-07-08 21:24:43.160600 autochain-0.0.3/autochain/agent/conversational_agent/prompt.py
+-rw-r--r--   0        0        0      192 2023-06-27 17:21:47.864519 autochain-0.0.3/autochain/agent/conversational_agent/readme.md
+-rw-r--r--   0        0        0     2988 2023-07-03 18:01:35.209804 autochain-0.0.3/autochain/agent/message.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:47.713048 autochain-0.0.3/autochain/agent/openai_funtions_agent/__init__.py
+-rw-r--r--   0        0        0     2866 2023-07-03 18:01:35.210284 autochain-0.0.3/autochain/agent/openai_funtions_agent/openai_functions_agent.py
+-rw-r--r--   0        0        0      718 2023-06-27 17:21:47.846783 autochain-0.0.3/autochain/agent/openai_funtions_agent/output_parser.py
+-rw-r--r--   0        0        0      226 2023-06-27 17:21:47.847035 autochain-0.0.3/autochain/agent/openai_funtions_agent/readme.md
+-rw-r--r--   0        0        0      842 2023-06-27 17:21:47.864856 autochain-0.0.3/autochain/agent/prompt_formatter.py
+-rw-r--r--   0        0        0     2633 2023-07-03 18:01:35.210734 autochain-0.0.3/autochain/agent/structs.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.948601 autochain-0.0.3/autochain/chain/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-03 18:05:28.426791 autochain-0.0.3/autochain/chain/base_chain.py
+-rw-r--r--   0        0        0     4352 2023-07-03 18:01:35.211429 autochain-0.0.3/autochain/chain/chain.py
+-rw-r--r--   0        0        0      149 2023-06-27 17:21:47.715223 autochain-0.0.3/autochain/chain/constants.py
+-rw-r--r--   0        0        0     1183 2023-07-03 18:01:35.211793 autochain-0.0.3/autochain/chain/langchain_wrapper_chain.py
+-rw-r--r--   0        0        0      554 2023-06-27 17:21:43.949077 autochain-0.0.3/autochain/errors.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.949163 autochain-0.0.3/autochain/examples/__init__.py
+-rw-r--r--   0        0        0      978 2023-07-08 21:24:43.160949 autochain-0.0.3/autochain/examples/get_weather_with_conversational_agent.py
+-rw-r--r--   0        0        0     1292 2023-07-08 21:24:43.161287 autochain-0.0.3/autochain/examples/get_weather_with_openai_function_agent.py
+-rw-r--r--   0        0        0      445 2023-06-27 20:00:44.804353 autochain-0.0.3/autochain/examples/readme.md
+-rw-r--r--   0        0        0      820 2023-07-08 21:24:43.161595 autochain-0.0.3/autochain/examples/upsale_goal_conversational_agent.py
+-rw-r--r--   0        0        0      620 2023-07-08 21:24:43.162082 autochain-0.0.3/autochain/examples/write_poem_with_conversational_agent.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.949446 autochain-0.0.3/autochain/memory/__init__.py
+-rw-r--r--   0        0        0     1145 2023-06-27 17:21:47.715981 autochain-0.0.3/autochain/memory/base.py
+-rw-r--r--   0        0        0     1321 2023-07-03 18:01:35.212974 autochain-0.0.3/autochain/memory/buffer_memory.py
+-rw-r--r--   0        0        0       16 2023-07-03 18:05:28.427082 autochain-0.0.3/autochain/memory/constants.py
+-rw-r--r--   0        0        0     2358 2023-07-03 18:01:35.213321 autochain-0.0.3/autochain/memory/long_term_memory.py
+-rw-r--r--   0        0        0     2834 2023-07-08 03:23:01.738016 autochain-0.0.3/autochain/memory/redis_memory.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.949725 autochain-0.0.3/autochain/models/__init__.py
+-rw-r--r--   0        0        0     2024 2023-06-27 17:21:47.759100 autochain-0.0.3/autochain/models/ada_embedding.py
+-rw-r--r--   0        0        0     4651 2023-07-08 21:35:34.978707 autochain-0.0.3/autochain/models/base.py
+-rw-r--r--   0        0        0     7669 2023-07-03 18:01:35.213652 autochain-0.0.3/autochain/models/chat_openai.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950002 autochain-0.0.3/autochain/py.typed
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950070 autochain-0.0.3/autochain/tools/__init__.py
+-rw-r--r--   0        0        0     3829 2023-07-03 18:01:35.214111 autochain-0.0.3/autochain/tools/base.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950229 autochain-0.0.3/autochain/tools/google_search/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-27 17:21:43.950338 autochain-0.0.3/autochain/tools/google_search/tool.py
+-rw-r--r--   0        0        0     4900 2023-06-27 17:21:43.950442 autochain-0.0.3/autochain/tools/google_search/util.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950493 autochain-0.0.3/autochain/tools/internal_search/__init__.py
+-rw-r--r--   0        0        0     2201 2023-06-27 17:21:47.835514 autochain-0.0.3/autochain/tools/internal_search/chromadb_tool.py
+-rw-r--r--   0        0        0     2226 2023-06-27 17:21:47.848764 autochain-0.0.3/autochain/tools/internal_search/pinecone_tool.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950648 autochain-0.0.3/autochain/tools/simple_handoff/__init__.py
+-rw-r--r--   0        0        0      303 2023-07-08 21:24:43.162458 autochain-0.0.3/autochain/tools/simple_handoff/tool.py
+-rw-r--r--   0        0        0     1595 2023-07-08 21:24:43.162779 autochain-0.0.3/autochain/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:43.950856 autochain-0.0.3/autochain/workflows_evaluation/__init__.py
+-rw-r--r--   0        0        0     7038 2023-07-08 21:24:43.163350 autochain-0.0.3/autochain/workflows_evaluation/base_test.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:47.865309 autochain-0.0.3/autochain/workflows_evaluation/conversational_agent_eval/__init__.py
+-rw-r--r--   0        0        0     3772 2023-07-08 21:24:43.163698 autochain-0.0.3/autochain/workflows_evaluation/conversational_agent_eval/change_shipping_address_test.py
+-rw-r--r--   0        0        0     3206 2023-07-08 21:24:43.164014 autochain-0.0.3/autochain/workflows_evaluation/conversational_agent_eval/generate_ads_test.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:47.739513 autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/__init__.py
+-rw-r--r--   0        0        0     3355 2023-07-08 21:24:43.164441 autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/change_shipping_address_test.py
+-rw-r--r--   0        0        0     1150 2023-07-08 03:23:01.739765 autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/custom_langchain_output_parser.py
+-rw-r--r--   0        0        0     3520 2023-07-08 21:24:43.164777 autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/generate_ads_test.py
+-rw-r--r--   0        0        0     1546 2023-07-08 03:23:01.740220 autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/langchain_test_utils.py
+-rw-r--r--   0        0        0      704 2023-07-08 03:23:01.740419 autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/readme.md
+-rw-r--r--   0        0        0        0 2023-06-27 17:21:47.716600 autochain-0.0.3/autochain/workflows_evaluation/openai_function_agent_eval/__init__.py
+-rw-r--r--   0        0        0     3986 2023-07-08 21:24:43.165214 autochain-0.0.3/autochain/workflows_evaluation/openai_function_agent_eval/change_shipping_address_test.py
+-rw-r--r--   0        0        0     3513 2023-07-08 21:24:43.165568 autochain-0.0.3/autochain/workflows_evaluation/openai_function_agent_eval/generate_ads_test.py
+-rw-r--r--   0        0        0     1531 2023-07-08 21:24:43.165898 autochain-0.0.3/autochain/workflows_evaluation/test_utils.py
+-rw-r--r--   0        0        0     2732 2023-07-08 21:38:32.925414 autochain-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8988 1970-01-01 00:00:00.000000 autochain-0.0.3/PKG-INFO
```

### Comparing `autochain-0.0.2/LICENSE.txt` & `autochain-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/README.md` & `autochain-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/agent/base_agent.py` & `autochain-0.0.3/autochain/agent/base_agent.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/agent/conversational_agent/conversational_agent.py` & `autochain-0.0.3/autochain/agent/conversational_agent/conversational_agent.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/agent/conversational_agent/output_parser.py` & `autochain-0.0.3/autochain/agent/conversational_agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/agent/conversational_agent/prompt.py` & `autochain-0.0.3/autochain/agent/conversational_agent/prompt.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/agent/message.py` & `autochain-0.0.3/autochain/agent/message.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/agent/openai_funtions_agent/openai_functions_agent.py` & `autochain-0.0.3/autochain/agent/openai_funtions_agent/openai_functions_agent.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/agent/openai_funtions_agent/output_parser.py` & `autochain-0.0.3/autochain/agent/openai_funtions_agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/agent/prompt_formatter.py` & `autochain-0.0.3/autochain/agent/prompt_formatter.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/agent/structs.py` & `autochain-0.0.3/autochain/agent/structs.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/chain/base_chain.py` & `autochain-0.0.3/autochain/chain/base_chain.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/chain/chain.py` & `autochain-0.0.3/autochain/chain/chain.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/chain/langchain_wrapper_chain.py` & `autochain-0.0.3/autochain/chain/langchain_wrapper_chain.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/errors.py` & `autochain-0.0.3/autochain/errors.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/examples/get_weather_with_conversational_agent.py` & `autochain-0.0.3/autochain/examples/get_weather_with_conversational_agent.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/examples/get_weather_with_openai_function_agent.py` & `autochain-0.0.3/autochain/examples/get_weather_with_openai_function_agent.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/examples/upsale_goal_conversational_agent.py` & `autochain-0.0.3/autochain/examples/upsale_goal_conversational_agent.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/examples/write_poem_with_conversational_agent.py` & `autochain-0.0.3/autochain/examples/write_poem_with_conversational_agent.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/memory/base.py` & `autochain-0.0.3/autochain/memory/base.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/memory/buffer_memory.py` & `autochain-0.0.3/autochain/memory/buffer_memory.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/memory/long_term_memory.py` & `autochain-0.0.3/autochain/memory/long_term_memory.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/memory/redis_memory.py` & `autochain-0.0.3/autochain/memory/redis_memory.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/models/ada_embedding.py` & `autochain-0.0.3/autochain/models/ada_embedding.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/models/base.py` & `autochain-0.0.3/autochain/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from __future__ import annotations
 
-import enum
-import inspect
 import logging
-import re
 from abc import abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from pydantic import Extra, Field, BaseModel
 from tenacity import (
     before_sleep_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
 from autochain.agent.message import BaseMessage
-from autochain.agent.message import UserMessage, AIMessage, SystemMessage
 from autochain.tools.base import Tool
 
 logger = logging.getLogger(__name__)
 
 
 class Generation(BaseModel):
     """Output of a single generation."""
```

### Comparing `autochain-0.0.2/autochain/models/chat_openai.py` & `autochain-0.0.3/autochain/models/chat_openai.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/tools/base.py` & `autochain-0.0.3/autochain/tools/base.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/tools/google_search/tool.py` & `autochain-0.0.3/autochain/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/tools/google_search/util.py` & `autochain-0.0.3/autochain/tools/google_search/util.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/tools/internal_search/chromadb_tool.py` & `autochain-0.0.3/autochain/tools/internal_search/chromadb_tool.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/tools/internal_search/pinecone_tool.py` & `autochain-0.0.3/autochain/tools/internal_search/pinecone_tool.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/utils.py` & `autochain-0.0.3/autochain/utils.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/base_test.py` & `autochain-0.0.3/autochain/workflows_evaluation/base_test.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/conversational_agent_eval/change_shipping_address_test.py` & `autochain-0.0.3/autochain/workflows_evaluation/conversational_agent_eval/change_shipping_address_test.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/conversational_agent_eval/generate_ads_test.py` & `autochain-0.0.3/autochain/workflows_evaluation/conversational_agent_eval/generate_ads_test.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/change_shipping_address_test.py` & `autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/change_shipping_address_test.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/custom_langchain_output_parser.py` & `autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/custom_langchain_output_parser.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/generate_ads_test.py` & `autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/generate_ads_test.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/langchain_test_utils.py` & `autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/langchain_test_utils.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/langchain_eval/readme.md` & `autochain-0.0.3/autochain/workflows_evaluation/langchain_eval/readme.md`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/openai_function_agent_eval/change_shipping_address_test.py` & `autochain-0.0.3/autochain/workflows_evaluation/openai_function_agent_eval/change_shipping_address_test.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/openai_function_agent_eval/generate_ads_test.py` & `autochain-0.0.3/autochain/workflows_evaluation/openai_function_agent_eval/generate_ads_test.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/autochain/workflows_evaluation/test_utils.py` & `autochain-0.0.3/autochain/workflows_evaluation/test_utils.py`

 * *Files identical despite different names*

### Comparing `autochain-0.0.2/pyproject.toml` & `autochain-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autochain"
-version = "0.0.2"
+version = "0.0.3"
 description = "AutoChain: Build lightweight, extensible, and testable LLM Agents"
 # TODO: add URLs, homepage, documentation
 authors = [
     "Yi Lu <yi.lu@forethought.ai>",
     "Forethought Engineering <eng-oss@forethought.ai>",
 ]
 readme = "README.md"
@@ -46,14 +46,15 @@
 pandas = ">=2.0.2"
 openai = ">=0.27.8"
 types-colorama = ">=0.4.15.11"
 pytest = "^7.3.2"
 redis = "^4.6.0"
 pinecone-client = "^2.2.2"
 mkdocs-git-authors-plugin = "^0.7.2"
+tenacity = "^8.2.2"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 black = "^23.3.0"
 ruff = "^0.0.272"
 mkdocs = "^1.4.2"
```

### Comparing `autochain-0.0.2/PKG-INFO` & `autochain-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autochain
-Version: 0.0.2
+Version: 0.0.3
 Summary: AutoChain: Build lightweight, extensible, and testable LLM Agents
 Author: Yi Lu
 Author-email: yi.lu@forethought.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
@@ -39,14 +39,15 @@
 Requires-Dist: mkdocs-git-authors-plugin (>=0.7.2,<0.8.0)
 Requires-Dist: openai (>=0.27.8)
 Requires-Dist: pandas (>=2.0.2)
 Requires-Dist: pinecone-client (>=2.2.2,<3.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Requires-Dist: redis (>=4.6.0,<5.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: types-colorama (>=0.4.15.11)
 Description-Content-Type: text/markdown
 
 # AutoChain
 
 Large language models (LLMs) have shown huge success in different text generation tasks and
 enable developers to build generative agents based on natural language objectives.
```

