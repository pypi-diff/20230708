# Comparing `tmp/alphawave-0.3.4.tar.gz` & `tmp/alphawave-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.3.4.tar", last modified: Thu Jul  6 15:48:34 2023, max compression
+gzip compressed data, was "alphawave-0.3.5.tar", last modified: Sat Jul  8 01:28:53 2023, max compression
```

## Comparing `alphawave-0.3.4.tar` & `alphawave-0.3.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 15:48:34.564322 alphawave-0.3.4/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.4/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-06 15:48:34.564322 alphawave-0.3.4/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.4/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1006 2023-07-06 15:48:27.000000 alphawave-0.3.4/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-06 15:48:34.564322 alphawave-0.3.4/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 15:48:34.560323 alphawave-0.3.4/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 15:48:34.560323 alphawave-0.3.4/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10039 2023-07-06 15:34:18.000000 alphawave-0.3.4/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.4/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.4/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8159 2023-07-06 15:36:35.000000 alphawave-0.3.4/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.4/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.3.4/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8917 2023-06-30 21:13:15.000000 alphawave-0.3.4/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.3.4/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.4/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6501 2023-07-04 18:20:06.000000 alphawave-0.3.4/src/alphawave/TOMLResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.4/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.4/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.4/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.3.4/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.4/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.4/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 15:48:34.560323 alphawave-0.3.4/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-06 15:48:34.000000 alphawave-0.3.4/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1777 2023-07-06 15:48:34.000000 alphawave-0.3.4/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-06 15:48:34.000000 alphawave-0.3.4/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      191 2023-07-06 15:48:34.000000 alphawave-0.3.4/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-06 15:48:34.000000 alphawave-0.3.4/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 15:48:34.560323 alphawave-0.3.4/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    16573 2023-07-06 03:45:52.000000 alphawave-0.3.4/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1721 2023-07-05 23:26:34.000000 alphawave-0.3.4/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7215 2023-07-06 15:43:30.000000 alphawave-0.3.4/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-06-30 18:31:20.000000 alphawave-0.3.4/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.4/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.4/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-01 22:34:34.000000 alphawave-0.3.4/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1512 2023-07-05 23:30:15.000000 alphawave-0.3.4/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3239 2023-06-30 02:09:36.000000 alphawave-0.3.4/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7944 2023-07-05 23:46:12.000000 alphawave-0.3.4/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.4/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.4/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.4/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.4/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 15:48:34.560323 alphawave-0.3.4/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.4/src/alphawave_pyexts/FsInference.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6391 2023-07-05 18:56:38.000000 alphawave-0.3.4/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2731 2023-07-03 19:26:44.000000 alphawave-0.3.4/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.4/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.4/src/alphawave_pyexts/configuration_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    22234 2023-07-05 22:51:49.000000 alphawave-0.3.4/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.4/src/alphawave_pyexts/handler.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 15:48:34.560323 alphawave-0.3.4/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14219 2023-07-04 18:53:15.000000 alphawave-0.3.4/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-07-06 15:45:53.000000 alphawave-0.3.4/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.4/src/alphawave_pyexts/modelling_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.4/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6901 2023-07-03 18:25:59.000000 alphawave-0.3.4/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-06 15:48:34.564322 alphawave-0.3.4/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.4/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.4/tests/testOpenAiClient.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.409691 alphawave-0.3.5/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.5/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-08 01:28:53.409691 alphawave-0.3.5/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.5/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1006 2023-07-08 01:27:21.000000 alphawave-0.3.5/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-08 01:28:53.409691 alphawave-0.3.5/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.405691 alphawave-0.3.5/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.405691 alphawave-0.3.5/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9544 2023-07-07 19:02:32.000000 alphawave-0.3.5/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.5/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.5/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8159 2023-07-06 15:36:35.000000 alphawave-0.3.5/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.5/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7128 2023-07-07 19:01:47.000000 alphawave-0.3.5/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8917 2023-06-30 21:13:15.000000 alphawave-0.3.5/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.3.5/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.5/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6501 2023-07-04 18:20:06.000000 alphawave-0.3.5/src/alphawave/TOMLResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.5/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.5/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.5/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1373 2023-07-06 17:42:19.000000 alphawave-0.3.5/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.5/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.5/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.405691 alphawave-0.3.5/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-08 01:28:53.000000 alphawave-0.3.5/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1777 2023-07-08 01:28:53.000000 alphawave-0.3.5/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-08 01:28:53.000000 alphawave-0.3.5/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      191 2023-07-08 01:28:53.000000 alphawave-0.3.5/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-08 01:28:53.000000 alphawave-0.3.5/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.405691 alphawave-0.3.5/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    16573 2023-07-06 03:45:52.000000 alphawave-0.3.5/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1721 2023-07-05 23:26:34.000000 alphawave-0.3.5/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6829 2023-07-07 18:03:47.000000 alphawave-0.3.5/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-06-30 18:31:20.000000 alphawave-0.3.5/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.5/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.5/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-01 22:34:34.000000 alphawave-0.3.5/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1512 2023-07-05 23:30:15.000000 alphawave-0.3.5/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3239 2023-06-30 02:09:36.000000 alphawave-0.3.5/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7944 2023-07-05 23:46:12.000000 alphawave-0.3.5/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.5/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.5/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.5/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.5/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.405691 alphawave-0.3.5/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.5/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6391 2023-07-05 18:56:38.000000 alphawave-0.3.5/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2731 2023-07-03 19:26:44.000000 alphawave-0.3.5/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.5/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.5/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    22900 2023-07-07 17:34:06.000000 alphawave-0.3.5/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.5/src/alphawave_pyexts/handler.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.409691 alphawave-0.3.5/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14219 2023-07-04 18:53:15.000000 alphawave-0.3.5/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-07-06 15:45:53.000000 alphawave-0.3.5/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.5/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.5/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6901 2023-07-03 18:25:59.000000 alphawave-0.3.5/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.409691 alphawave-0.3.5/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.5/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.5/tests/testOpenAiClient.py
```

### Comparing `alphawave-0.3.4/LICENSE` & `alphawave-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/PKG-INFO` & `alphawave-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.4
+Version: 0.3.5
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.4/README.md` & `alphawave-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/pyproject.toml` & `alphawave-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave-py - Functions for smaller Large Language Models (sLLMs)"
```

### Comparing `alphawave-0.3.4/src/alphawave/AlphaWave.py` & `alphawave-0.3.5/src/alphawave/AlphaWave.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     prompt: Prompt = None
     prompt_options: PromptCompletionOptions = None
     memory: PromptMemory = VolatileMemory()
     functions: PromptFunctions = FunctionRegistry()
     history_variable: str = 'history'
     input_variable: str = 'input'
     max_history_messages: int = 6
-    max_repair_attempts: int =2
+    max_repair_attempts: int =3
     tokenizer: Tokenizer = GPT3Tokenizer()
     validator: DefaultResponseValidator = DefaultResponseValidator()
     logRepairs: bool = False
 
 def update_dataclass(instance, **kwargs):
     for key, value in kwargs.items():
         if hasattr(instance, key):
@@ -75,31 +75,27 @@
             input = ''
 
         try:
             self.emit('beforePrompt', memory, functions, tokenizer, prompt, prompt_options)
             response = await client.completePrompt(memory, functions, tokenizer, prompt, prompt_options)
             self.emit('afterPrompt', memory, functions, tokenizer, prompt, prompt_options, response)
             if response['status'] != 'success':
-                #print(f'***** Alphawave client completePrompt failure {response}')
                 return response
 
             if not isinstance(response['message'], dict):
-                #print(f'***** Alphawave making sure message is a dict with key content')
                 response['message'] = {'role': 'assistant', 'content': response['message'] or ''}
 
             self.emit('beforeValidation', memory, functions, tokenizer, response, max_repair_attempts)
-            #print(f'***** Alphawave before validation ')
             validation = validator.validate_response(memory, functions, tokenizer, response, max_repair_attempts)
             self.emit('afterValidation', memory, functions, tokenizer, response, max_repair_attempts, validation)
             if 'coroutine' in str(type(validation)).lower():
                 validation = await validation
             if validation['valid']:
                 if 'value' in validation:
                     response['message']['content'] = validation['value']
-                    #print(f"***** Alphawave post validation picking up value {response}\n note response['message']['content'] must exist!")
         
                 self.addInputToHistory(memory, history_variable, input)
                 self.addResponseToHistory(memory, history_variable, response['message'])
                 return response
 
             if self.options.logRepairs:
                 print(Colorize.title('REPAIRING RESPONSE:'))
@@ -151,19 +147,19 @@
             else:
                 history[-1]['content']=message
             if len(history) > self.options.max_history_messages:
                 history = history[int(self.options.max_history_messages/2):]
             memory.set(variable, history)
 
     async def repairResponse(self, fork, functions, tokenizer, response, validation, remaining_attempts):
-        client, prompt, prompt_options, memory, functions, history_variable, input_variable, max_history_messages, max_repair_attempts, tokenizer, validator, log_repairs = get_values(self.options, ('client', 'prompt', 'prompt_options', 'memory', 'functions', 'history_variable', 'input_variable', 'max_history_messages', 'max_repair_attempts', 'tokenizer', 'validator', 'log_repairs'))
+        client, prompt, prompt_options, memory, history_variable, validator, log_repairs = get_values(self.options, ('client', 'prompt', 'prompt_options', 'memory',  'history_variable', 'validator', 'log_repairs'))
 
-        # Are we out of attempts?
+        # Are we out of attemp ts?
         feedback = validation.get('feedback', 'The response was invalid. Try another strategy.')
-            
+        #print(f'remaining_repair {remaining_attempts}')    
         if remaining_attempts <= 0:
             return {
                 'status': 'invalid_response',
                 'message': feedback
             }
 
         # Add response and feedback to repair history
```

### Comparing `alphawave-0.3.4/src/alphawave/Colorize.py` & `alphawave-0.3.5/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.3.5/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/JSONResponseValidator.py` & `alphawave-0.3.5/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/MemoryFork.py` & `alphawave-0.3.5/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/OSClient.py` & `alphawave-0.3.5/src/alphawave/OSClient.py`

 * *Files 17% similar despite different names*

```diff
@@ -82,65 +82,39 @@
                                               frequency_penalty = argoptions['frequency_penalty']
                                               )
         startTime = time.time()
         max_input_tokens = 1500
         if hasattr(options, 'max_input_tokens') and getattr(options, 'max_input_tokens') is not None:
             max_input_tokens = options.max_input_tokens
         
-        if hasattr(options, 'completion_type') and options.completion_type == 'text':
-            result = prompt.renderAsText(memory, functions, tokenizer, max_input_tokens)
-            if result.tooLong:
-                return {'status': 'too_long', 'message': f"The generated text completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
-            if self.options.logRequests:
-                print(Colorize.title('PROMPT:'))
-                for msg in result.output:
-                    if not isinstance(msg, dict):
-                        msg = msg.__dict__
-                    print(Colorize.output(json.dumps(msg, indent=2)), end='')
-                print()
-            request = self.copyOptionsToRequest(CreateCompletionRequest({
-                'model': optionsmodel,
-                'prompt': result.output,
-            }), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
-            response = self.createCompletion(request)
-            if self.options.logRequests:
-                print(Colorize.title('RESPONSE:'))
-                print(Colorize.value('status', response.status))
-                print(Colorize.value('duration', time.time() - startTime, 'ms'))
-                print(Colorize.output(response.message))
-
-            if response.status == 'success':
-                completion = response.message
-                return {'status': 'success', 'message': completion}
-            else:
-                return {'status': 'error', 'message': f"The text completion API returned an error status of {response.status}: {response.message}"}
+        result = await prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
+        
+        if result.tooLong:
+            return {'status': 'too_long', 'message': f"The generated chat completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
+        if self.options.logRequests:
+            print(Colorize.title('CHAT PROMPT:'))
+            for msg in result.output:
+                if not isinstance(msg, dict):
+                    print(Colorize.output(msg))
+                    msg = msg.__dict__
+                print(Colorize.output(json.dumps(msg, indent=2)), end='')
+            print()
+        request = self.copyOptionsToRequest(CreateChatCompletionRequest(model = options.model, messages =  result.output), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
+        response = self.createChatCompletion(request)
+        if self.options.logRequests:
+            print(Colorize.title('CHAT RESPONSE:'))
+            print(Colorize.value('status', response.status))
+            print(Colorize.value('duration', time.time() - startTime, 'ms'))
+            print(Colorize.output(response.message))
+        
+        if response.status == 'success':
+            completion = response.message
+            return {'status': 'success', 'message': completion}
         else:
-            result = await prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
-            if result.tooLong:
-                return {'status': 'too_long', 'message': f"The generated chat completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
-            if self.options.logRequests:
-                print(Colorize.title('CHAT PROMPT:'))
-                for msg in result.output:
-                    if not isinstance(msg, dict):
-                        msg = msg.__dict__
-                    print(Colorize.output(json.dumps(msg, indent=2)), end='')
-                print()
-            request = self.copyOptionsToRequest(CreateChatCompletionRequest(model = options.model, messages =  result.output), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
-            response = self.createChatCompletion(request)
-            if self.options.logRequests:
-                print(Colorize.title('CHAT RESPONSE:'))
-                print(Colorize.value('status', response.status))
-                print(Colorize.value('duration', time.time() - startTime, 'ms'))
-                print(Colorize.output(response.message))
-
-            if response.status == 'success':
-                completion = response.message
-                return {'status': 'success', 'message': completion}
-            else:
-                return {'status': 'error', 'message': f"The chat completion API returned an error status of {response.status}: {response.message}"}
+            return {'status': 'error', 'message': f"The chat completion API returned an error status of {response.status}: {response.message}"}
 
     def addRequestHeaders(self, headers: Dict[str, str], options: OSClientOptions):
         headers['Authorization'] = f"Bearer {options.apiKey}"
         if options.organization:
             headers['OS-Organization'] = options.organization
 
     def copyOptionsToRequest(self, target: Dict[str, Any], src: Any, fields: list) -> Dict[str, Any]:
```

### Comparing `alphawave-0.3.4/src/alphawave/OpenAIClient.py` & `alphawave-0.3.5/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/RepairTestClient.py` & `alphawave-0.3.5/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/Response.py` & `alphawave-0.3.5/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/TOMLResponseValidator.py` & `alphawave-0.3.5/src/alphawave/TOMLResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/TestClient.py` & `alphawave-0.3.5/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/TestClientTest.py` & `alphawave-0.3.5/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/alphawaveTypes.py` & `alphawave-0.3.5/src/alphawave/alphawaveTypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 class PromptResponseValidator:
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: 'PromptResponse', remaining_attempts: int) -> 'Promise[Validation]':
         pass
 
 @dataclass
 class PromptCompletionOptions:
-    completion_type: str  # 'text' | 'chat'
-    model: str
+    completion_type: str  = 'chat' # 'text' | 'chat'
+    model: str = ''
     max_input_tokens: int =2000
     temperature: float = 0.7
     top_p: float = 1.0
     max_tokens: int = 500
     stop: str = None
     presence_penalty: float = 1.0
     frequency_penalty: float = 1.0
```

### Comparing `alphawave-0.3.4/src/alphawave/internalTypes.py` & `alphawave-0.3.5/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave/jsonParser.py` & `alphawave-0.3.5/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.3.5/src/alphawave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.4
+Version: 0.3.5
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.4/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.3.5/src/alphawave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/Agent.py` & `alphawave-0.3.5/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.3.5/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.3.5/src/alphawave_agents/AgentCommandValidator.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         #print(f"***** AgentCommandValidator generic exit fail {thought['command']['name']}")
         return {
             'type': 'Validation',
             'valid': False,
             'feedback': f'The command validation failed. try again {str(e)}'
                 }
 
+    ### interesting experiment, set aside for now
     async def repair_args(self, command, fail_thought):
         #print(f"***** AgentCommandValidator recovery attempt keys {list(self._memory._memory.keys())}")
         args_validator = JSONResponseValidator(command.schema, "invalid command inputs syntax, use: {command.one_shot()\n}")
         fork = MemoryFork(self._memory)
         prompt_options=PromptCompletionOptions(completion_type='chat', model=self._model, temperature=0.1)
         args_prompt=Prompt([ConversationHistory(self._history_variable),
                             UserMessage(f'invalid command args: {fail_args}, repair using this format: {command.schema["properties"]}')])
@@ -120,14 +121,7 @@
             return args
         #print(f"***** AgentCommandValidator recovery returning fail_args {fail_args}")
         return fail_args
 
 
 from alphawave.OSClient import OSClient
 
-if __name__ == '__main__':
-    memory=VolatileMemory()
-    memory.set('history', {'role': 'assistant', 'content': {"command":{"name":"math", "inputs":{"abc":"xyz"}}}})
-    acv = AgentCommandValidator(commands={"math":MathCommand()}, client=OSClient(logRequests=True), model='vicuna_v1.1', syntax='JSON', memory=memory)
-    #print('acv created')
-    result = asyncio.run(acv.repair_args(MathCommand(), {'abc':'xyz'}))
-    #print(result)
```

### Comparing `alphawave-0.3.4/src/alphawave_agents/AskCommand.py` & `alphawave-0.3.5/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.3.5/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.3.5/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.3.5/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/MathCommand.py` & `alphawave-0.3.5/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/PromptCommand.py` & `alphawave-0.3.5/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.3.5/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.3.5/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.3.5/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_agents/agentTypes.py` & `alphawave-0.3.5/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/FsInference.py` & `alphawave-0.3.5/src/alphawave_pyexts/FsInference.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.3.5/src/alphawave_pyexts/LLMClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.3.5/src/alphawave_pyexts/SearchCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/chat.py` & `alphawave-0.3.5/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/configuration_RW.py` & `alphawave-0.3.5/src/alphawave_pyexts/configuration_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/conversation.py` & `alphawave-0.3.5/src/alphawave_pyexts/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,28 +675,39 @@
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="",
     )
 )
 register_conv_template(Conversation(
-        name="wizardLM",
+        name="wizardLM2",
         system="",
         roles=("### Input", "### Response"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="\n",
     )
 )
 register_conv_template(Conversation(
-        name="wizardLM2",
+        name="wizardCoder",
+        system="Below is an instruction that describes a task. Write a response that appropriately completes the request",
+        roles=("### Instruction", "### Response"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_TWO,
+        sep="\n",
+        sep2="<|end|>",
+    )
+)
+register_conv_template(Conversation(
+        name="wizardLM",
         system="",
-        roles=("User", "Assistant"),
+        roles=("USER", "ASSISTANT"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="\n",
     )
 )
@@ -736,14 +747,27 @@
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ROBIN,
         sep="\n\n",
         stop_str="###",
     )
 )
+# tigerbot template
+register_conv_template(
+    Conversation(
+        name="xgen",
+        system="",
+        roles=("### Human", "### Assistant"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_SINGLE,
+        sep="\n\n",
+        stop_str="###",
+    )
+)
 
 
 if __name__ == "__main__":
     conv = get_conv_template("vicuna_v1.1")
     conv.append_message(conv.roles[0], "Hello!")
     conv.append_message(conv.roles[1], "Hi!")
     conv.append_message(conv.roles[0], "How are you?")
```

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/handler.py` & `alphawave-0.3.5/src/alphawave_pyexts/handler.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.3.5/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.3.5/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/modelling_RW.py` & `alphawave-0.3.5/src/alphawave_pyexts/modelling_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/serverUtils.py` & `alphawave-0.3.5/src/alphawave_pyexts/serverUtils.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.3.5/src/alphawave_pyexts/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/tests/testOSClient.py` & `alphawave-0.3.5/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.4/tests/testOpenAiClient.py` & `alphawave-0.3.5/tests/testOpenAiClient.py`

 * *Files identical despite different names*

