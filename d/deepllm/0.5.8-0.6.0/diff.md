# Comparing `tmp/deepllm-0.5.8.tar.gz` & `tmp/deepllm-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepllm-0.5.8.tar", last modified: Thu Jul  6 02:52:10 2023, max compression
+gzip compressed data, was "deepllm-0.6.0.tar", last modified: Sat Jul  8 00:52:44 2023, max compression
```

## Comparing `deepllm-0.5.8.tar` & `deepllm-0.6.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.964865 deepllm-0.5.8/
--rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-0.5.8/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     4261 2023-07-06 02:52:10.964568 deepllm-0.5.8/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     3976 2023-07-06 02:19:27.000000 deepllm-0.5.8/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.952422 deepllm-0.5.8/deepllm/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2023-07-06 02:52:00.000000 deepllm-0.5.8/deepllm/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     1329 2023-07-05 04:00:30.000000 deepllm-0.5.8/deepllm/api.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.956106 deepllm-0.5.8/deepllm/apps/
--rw-r--r--   0 tarau      (503) staff       (20)       56 2023-07-03 02:58:46.000000 deepllm-0.5.8/deepllm/apps/README.md
--rw-r--r--   0 tarau      (503) staff       (20)     1296 2023-07-05 03:38:00.000000 deepllm-0.5.8/deepllm/apps/app.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-07-05 03:13:40.000000 deepllm-0.5.8/deepllm/apps/app.sh
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.8/deepllm/apps/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       10 2023-07-03 02:55:55.000000 deepllm-0.5.8/deepllm/apps/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      663 2023-07-03 00:54:44.000000 deepllm-0.5.8/deepllm/configurator.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.957883 deepllm-0.5.8/deepllm/demos/
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 02:44:58.000000 deepllm-0.5.8/deepllm/demos/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.8/deepllm/demos/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2121 2023-07-03 03:55:03.000000 deepllm-0.5.8/deepllm/demos/demo.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.8/deepllm/demos/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       36 2023-07-05 04:04:08.000000 deepllm-0.5.8/deepllm/demos/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1966 2023-07-03 03:39:42.000000 deepllm-0.5.8/deepllm/demos/wikifetch.py
--rw-r--r--   0 tarau      (503) staff       (20)     1864 2023-07-03 02:27:55.000000 deepllm-0.5.8/deepllm/embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)     3425 2023-07-03 00:41:21.000000 deepllm-0.5.8/deepllm/horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)     8737 2023-07-03 01:11:12.000000 deepllm-0.5.8/deepllm/interactors.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.960192 deepllm-0.5.8/deepllm/local_llms/
--rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-0.5.8/deepllm/local_llms/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.5.8/deepllm/local_llms/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.5.8/deepllm/local_llms/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-0.5.8/deepllm/local_llms/local_runs.py
--rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-0.5.8/deepllm/local_llms/requirements.txt
--rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-0.5.8/deepllm/local_llms/server.sh
--rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-07-03 02:43:39.000000 deepllm-0.5.8/deepllm/local_llms/test_vicuna.py
--rw-r--r--   0 tarau      (503) staff       (20)     3006 2023-07-06 02:11:51.000000 deepllm-0.5.8/deepllm/params.py
--rw-r--r--   0 tarau      (503) staff       (20)     6111 2023-07-05 03:41:23.000000 deepllm-0.5.8/deepllm/prompters.py
--rw-r--r--   0 tarau      (503) staff       (20)     6880 2023-07-06 02:50:36.000000 deepllm-0.5.8/deepllm/recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     4081 2023-07-05 03:23:11.000000 deepllm-0.5.8/deepllm/refiners.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.964072 deepllm-0.5.8/deepllm/tests/
--rw-r--r--   0 tarau      (503) staff       (20)       81 2023-07-03 02:47:31.000000 deepllm-0.5.8/deepllm/tests/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-0.5.8/deepllm/tests/__init__.py
--rwxr-xr-x   0 tarau      (503) staff       (20)      186 2023-07-03 04:38:48.000000 deepllm-0.5.8/deepllm/tests/test_all.sh
--rw-r--r--   0 tarau      (503) staff       (20)      571 2023-07-05 03:35:45.000000 deepllm-0.5.8/deepllm/tests/test_api.py
--rw-r--r--   0 tarau      (503) staff       (20)      365 2023-07-03 01:01:09.000000 deepllm-0.5.8/deepllm/tests/test_configurator.py
--rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 02:27:15.000000 deepllm-0.5.8/deepllm/tests/test_embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-0.5.8/deepllm/tests/test_horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 05:27:34.000000 deepllm-0.5.8/deepllm/tests/test_interactors.py
--rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-0.5.8/deepllm/tests/test_params.py
--rw-r--r--   0 tarau      (503) staff       (20)     1173 2023-07-03 03:45:12.000000 deepllm-0.5.8/deepllm/tests/test_recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     2246 2023-07-05 00:10:55.000000 deepllm-0.5.8/deepllm/tests/test_refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)     1205 2023-07-01 21:29:23.000000 deepllm-0.5.8/deepllm/tools.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-06 02:52:10.954271 deepllm-0.5.8/deepllm.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     4261 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     1256 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       28 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2023-07-06 02:52:10.000000 deepllm-0.5.8/deepllm.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2023-07-06 02:52:10.964981 deepllm-0.5.8/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      896 2023-07-04 20:51:34.000000 deepllm-0.5.8/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 00:52:44.201197 deepllm-0.6.0/
+-rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-0.6.0/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     4266 2023-07-08 00:52:44.200794 deepllm-0.6.0/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     3981 2023-07-07 22:49:34.000000 deepllm-0.6.0/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 00:52:44.182104 deepllm-0.6.0/deepllm/
+-rw-r--r--   0 tarau      (503) staff       (20)       23 2023-07-08 00:51:38.000000 deepllm-0.6.0/deepllm/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1322 2023-07-08 00:50:25.000000 deepllm-0.6.0/deepllm/api.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 00:52:44.186974 deepllm-0.6.0/deepllm/apps/
+-rw-r--r--   0 tarau      (503) staff       (20)       56 2023-07-03 02:58:46.000000 deepllm-0.6.0/deepllm/apps/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)     1299 2023-07-08 00:50:47.000000 deepllm-0.6.0/deepllm/apps/app.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-07-05 03:13:40.000000 deepllm-0.6.0/deepllm/apps/app.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.6.0/deepllm/apps/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       47 2023-07-07 23:04:29.000000 deepllm-0.6.0/deepllm/apps/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)      663 2023-07-03 00:54:44.000000 deepllm-0.6.0/deepllm/configurator.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 00:52:44.189593 deepllm-0.6.0/deepllm/demos/
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 02:44:58.000000 deepllm-0.6.0/deepllm/demos/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.6.0/deepllm/demos/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2121 2023-07-03 03:55:03.000000 deepllm-0.6.0/deepllm/demos/demo.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.6.0/deepllm/demos/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       36 2023-07-05 04:04:08.000000 deepllm-0.6.0/deepllm/demos/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1966 2023-07-03 03:39:42.000000 deepllm-0.6.0/deepllm/demos/wikifetch.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1864 2023-07-03 02:27:55.000000 deepllm-0.6.0/deepllm/embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3425 2023-07-03 00:41:21.000000 deepllm-0.6.0/deepllm/horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)     8737 2023-07-03 01:11:12.000000 deepllm-0.6.0/deepllm/interactors.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 00:52:44.193114 deepllm-0.6.0/deepllm/local_llms/
+-rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-0.6.0/deepllm/local_llms/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-0.6.0/deepllm/local_llms/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-0.6.0/deepllm/local_llms/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-0.6.0/deepllm/local_llms/local_runs.py
+-rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-0.6.0/deepllm/local_llms/requirements.txt
+-rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-0.6.0/deepllm/local_llms/server.sh
+-rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-07-03 02:43:39.000000 deepllm-0.6.0/deepllm/local_llms/test_vicuna.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3006 2023-07-06 05:21:46.000000 deepllm-0.6.0/deepllm/params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6111 2023-07-05 03:41:23.000000 deepllm-0.6.0/deepllm/prompters.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6880 2023-07-06 02:50:36.000000 deepllm-0.6.0/deepllm/recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     4081 2023-07-05 03:23:11.000000 deepllm-0.6.0/deepllm/refiners.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 00:52:44.199938 deepllm-0.6.0/deepllm/tests/
+-rw-r--r--   0 tarau      (503) staff       (20)       81 2023-07-03 02:47:31.000000 deepllm-0.6.0/deepllm/tests/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-0.6.0/deepllm/tests/__init__.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)      186 2023-07-03 04:38:48.000000 deepllm-0.6.0/deepllm/tests/test_all.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      571 2023-07-05 03:35:45.000000 deepllm-0.6.0/deepllm/tests/test_api.py
+-rw-r--r--   0 tarau      (503) staff       (20)      365 2023-07-03 01:01:09.000000 deepllm-0.6.0/deepllm/tests/test_configurator.py
+-rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 02:27:15.000000 deepllm-0.6.0/deepllm/tests/test_embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-0.6.0/deepllm/tests/test_horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)      498 2023-07-03 05:27:34.000000 deepllm-0.6.0/deepllm/tests/test_interactors.py
+-rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-0.6.0/deepllm/tests/test_params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1173 2023-07-03 03:45:12.000000 deepllm-0.6.0/deepllm/tests/test_recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2246 2023-07-05 00:10:55.000000 deepllm-0.6.0/deepllm/tests/test_refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1205 2023-07-01 21:29:23.000000 deepllm-0.6.0/deepllm/tools.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2023-07-08 00:52:44.184222 deepllm-0.6.0/deepllm.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     4266 2023-07-08 00:52:44.000000 deepllm-0.6.0/deepllm.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     1256 2023-07-08 00:52:44.000000 deepllm-0.6.0/deepllm.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-08 00:52:44.000000 deepllm-0.6.0/deepllm.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2023-07-08 00:52:44.000000 deepllm-0.6.0/deepllm.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       28 2023-07-08 00:52:44.000000 deepllm-0.6.0/deepllm.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2023-07-08 00:52:44.000000 deepllm-0.6.0/deepllm.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2023-07-08 00:52:44.201336 deepllm-0.6.0/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      896 2023-07-04 20:51:34.000000 deepllm-0.6.0/setup.py
```

### Comparing `deepllm-0.5.8/LICENSE` & `deepllm-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/PKG-INFO` & `deepllm-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 0.5.8
+Version: 0.6.0
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,15 +19,15 @@
 of a Horn Clause interpreter, except that we accommodate our logic engine to fit the natural language reasoning patterns LLMs have been trained on. Semantic similarity to ground-truth facts or oracle advice from another LLM instance is used to restrict the search space and validate the traces of justification steps returned as answers. At the end, the unique minimal model of a generated Horn Clause program collects the results of the reasoning process.
 
 As applications, we sketch implementations of consequence predictions, causal explanations,  recommendation systems and topic-focussed exploration of scientific literature.
 
 
 ### INSTALLATION and USAGE:
 
-#### Getting to OpenAI key:
+#### Getting the OpenAI key:
 
 As the code will use it, make sure you acquire it and have 
 
 ```
 export OPENAI_KEY=<your_key>
 ```
 
@@ -57,23 +57,22 @@
 
 #### API
 
 The DeepLLM [API](https://github.com/ptarau/recursors/blob/main/deepllm/api.py) exposes its high-level functions ready to embed in your application with something as simple as (assuming the your OPENAI_KEY is exported by your environment):
 
 ```
 for result in run_recursor(initiator='Using tactical nukes', prompter=conseq_prompter, lim=2):
-...   print(result)
+    print(result)
 ```
 
-Also, you can ask more interesting questions like in:
+Also, you can explore questions with less gruesome results like in:
 
 ```
-from deepllm.api import *
-1. for result in run_rrater(initiator='How to repair a flat tire', prompter=goal_prompter, lim=1):
-  print(result)
+for result in run_rater(initiator='Artificial General Intelligence', prompter=sci_prompter, lim=2, threshold=0.5):
+    print(result)
 ```
 
 #### Tests and demos 
 
 * Take a look at folder [deepllm/tests](https://github.com/ptarau/recursors/tree/main/deepllm/tests) for typical uses.
 
 * There are more extensive demos in folder  [deepllm/demos](https://github.com/ptarau/recursors/tree/main/deepllm/demos) .
```

### Comparing `deepllm-0.5.8/README.md` & `deepllm-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 of a Horn Clause interpreter, except that we accommodate our logic engine to fit the natural language reasoning patterns LLMs have been trained on. Semantic similarity to ground-truth facts or oracle advice from another LLM instance is used to restrict the search space and validate the traces of justification steps returned as answers. At the end, the unique minimal model of a generated Horn Clause program collects the results of the reasoning process.
 
 As applications, we sketch implementations of consequence predictions, causal explanations,  recommendation systems and topic-focussed exploration of scientific literature.
 
 
 ### INSTALLATION and USAGE:
 
-#### Getting to OpenAI key:
+#### Getting the OpenAI key:
 
 As the code will use it, make sure you acquire it and have 
 
 ```
 export OPENAI_KEY=<your_key>
 ```
 
@@ -46,23 +46,22 @@
 
 #### API
 
 The DeepLLM [API](https://github.com/ptarau/recursors/blob/main/deepllm/api.py) exposes its high-level functions ready to embed in your application with something as simple as (assuming the your OPENAI_KEY is exported by your environment):
 
 ```
 for result in run_recursor(initiator='Using tactical nukes', prompter=conseq_prompter, lim=2):
-...   print(result)
+    print(result)
 ```
 
-Also, you can ask more interesting questions like in:
+Also, you can explore questions with less gruesome results like in:
 
 ```
-from deepllm.api import *
-1. for result in run_rrater(initiator='How to repair a flat tire', prompter=goal_prompter, lim=1):
-  print(result)
+for result in run_rater(initiator='Artificial General Intelligence', prompter=sci_prompter, lim=2, threshold=0.5):
+    print(result)
 ```
 
 #### Tests and demos 
 
 * Take a look at folder [deepllm/tests](https://github.com/ptarau/recursors/tree/main/deepllm/tests) for typical uses.
 
 * There are more extensive demos in folder  [deepllm/demos](https://github.com/ptarau/recursors/tree/main/deepllm/demos) .
```

### Comparing `deepllm-0.5.8/deepllm/api.py` & `deepllm-0.6.0/deepllm/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from .refiners import Advisor, Rater, TruthRater, AbstractMaker
 
 def run_recursor(initiator=None, prompter=None, lim=None):
     assert None not in (prompter, initiator, lim)
     recursor = AndOrExplorer(initiator=initiator, prompter=prompter, lim=lim)
     yield from recursor.run()
 
-def run_adviser(initiator=None, prompter=None, lim=None):
+def run_advisor(initiator=None, prompter=None, lim=None):
     assert None not in (prompter, initiator, lim)
     recursor = Advisor(initiator=initiator, prompter=prompter, lim=lim)
     yield from recursor.run()
 
 def run_rater(initiator=None, prompter=None, lim=None, threshold=None):
     assert None not in (prompter, initiator, lim, threshold)
     recursor = Rater(initiator=initiator, prompter=prompter, lim=lim, threshold=threshold)
     yield from recursor.run()
 
 def run_truth_rater(initiator=None, prompter=None, truth_file=None, threshold=None, lim=None):
     assert None not in (initiator, prompter, truth_file, threshold, lim)
-    r = TruthRater(initiator=initiator, prompter=prompter, truth_file=truth_file, threshold=threshold, lim=lim)
-    yield from super().run()
+    rater = TruthRater(initiator=initiator, prompter=prompter, truth_file=truth_file, threshold=threshold, lim=lim)
+    yield from rater.run()
 
 def run_abstract_maker(topic=None,keywords=None):
-    assert None not in (prompter, initiator, lim)
+    assert None not in (topic, keywords)
     recursor = AbstractMaker(topic=topic,keywords=keywords)
     return recursor.run()
```

### Comparing `deepllm-0.5.8/deepllm/apps/app.py` & `deepllm-0.6.0/deepllm/apps/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,29 @@
 
 st.title('Streamlit-based DeepLLM Client')
 
 key = ensure_openai_api_key(
     st.sidebar.text_area("Unless it is in your environment, enter your OPENAI_API_KEY:", ""))
 
 d = prompter_dict()
-#st.write(d)
+# st.write(d)
 
 
 with st.sidebar:
     recursor = st.radio('LLM Agent:', ['Recursor', 'Advisor', 'Rater'])  # , 'Truth_rater'])
 
     threshold = st.slider('Threshold:', 0, 100, 50)
 
     lim = st.slider('Maximum depth', 1, 4, 1)
 
     initiator = st.text_area('Topic to explore:', value='Origin of COVID-19')
 
-
     prompter_name = st.radio('Prompter:', list(d.keys()))
 
-    prompter=eval(d[prompter_name])
+    prompter = eval(d[prompter_name])
 
     query_it = st.button('Activate LLM!')
 
 
 def do_query():
     if recursor == 'Recursor':
         g = run_recursor(initiator=initiator, prompter=prompter, lim=lim)
@@ -42,14 +41,14 @@
     else:
         assert recursor == 'Rater'
         g = run_rater(
             initiator=initiator, prompter=prompter, lim=lim, threshold=threshold)
 
     st.write('STARTING:')
     for x in g:
-        #st.write('.')
+        # st.write('.')
         st.write(*x)
     st.write('DONE:')
 
 
 if query_it:
     do_query()
```

### Comparing `deepllm-0.5.8/deepllm/configurator.py` & `deepllm-0.6.0/deepllm/configurator.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/demos/demo.py` & `deepllm-0.6.0/deepllm/demos/demo.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/demos/wikifetch.py` & `deepllm-0.6.0/deepllm/demos/wikifetch.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/embedders.py` & `deepllm-0.6.0/deepllm/embedders.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/horn_prover.py` & `deepllm-0.6.0/deepllm/horn_prover.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/interactors.py` & `deepllm-0.6.0/deepllm/interactors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/local_llms/local_runs.py` & `deepllm-0.6.0/deepllm/local_llms/local_runs.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/local_llms/test_vicuna.py` & `deepllm-0.6.0/deepllm/local_llms/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/params.py` & `deepllm-0.6.0/deepllm/params.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/prompters.py` & `deepllm-0.6.0/deepllm/prompters.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/recursors.py` & `deepllm-0.6.0/deepllm/recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/refiners.py` & `deepllm-0.6.0/deepllm/refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/tests/test_api.py` & `deepllm-0.6.0/deepllm/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/tests/test_recursors.py` & `deepllm-0.6.0/deepllm/tests/test_recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/tests/test_refiners.py` & `deepllm-0.6.0/deepllm/tests/test_refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm/tools.py` & `deepllm-0.6.0/deepllm/tools.py`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/deepllm.egg-info/PKG-INFO` & `deepllm-0.6.0/deepllm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 0.5.8
+Version: 0.6.0
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,15 +19,15 @@
 of a Horn Clause interpreter, except that we accommodate our logic engine to fit the natural language reasoning patterns LLMs have been trained on. Semantic similarity to ground-truth facts or oracle advice from another LLM instance is used to restrict the search space and validate the traces of justification steps returned as answers. At the end, the unique minimal model of a generated Horn Clause program collects the results of the reasoning process.
 
 As applications, we sketch implementations of consequence predictions, causal explanations,  recommendation systems and topic-focussed exploration of scientific literature.
 
 
 ### INSTALLATION and USAGE:
 
-#### Getting to OpenAI key:
+#### Getting the OpenAI key:
 
 As the code will use it, make sure you acquire it and have 
 
 ```
 export OPENAI_KEY=<your_key>
 ```
 
@@ -57,23 +57,22 @@
 
 #### API
 
 The DeepLLM [API](https://github.com/ptarau/recursors/blob/main/deepllm/api.py) exposes its high-level functions ready to embed in your application with something as simple as (assuming the your OPENAI_KEY is exported by your environment):
 
 ```
 for result in run_recursor(initiator='Using tactical nukes', prompter=conseq_prompter, lim=2):
-...   print(result)
+    print(result)
 ```
 
-Also, you can ask more interesting questions like in:
+Also, you can explore questions with less gruesome results like in:
 
 ```
-from deepllm.api import *
-1. for result in run_rrater(initiator='How to repair a flat tire', prompter=goal_prompter, lim=1):
-  print(result)
+for result in run_rater(initiator='Artificial General Intelligence', prompter=sci_prompter, lim=2, threshold=0.5):
+    print(result)
 ```
 
 #### Tests and demos 
 
 * Take a look at folder [deepllm/tests](https://github.com/ptarau/recursors/tree/main/deepllm/tests) for typical uses.
 
 * There are more extensive demos in folder  [deepllm/demos](https://github.com/ptarau/recursors/tree/main/deepllm/demos) .
```

### Comparing `deepllm-0.5.8/deepllm.egg-info/SOURCES.txt` & `deepllm-0.6.0/deepllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepllm-0.5.8/setup.py` & `deepllm-0.6.0/setup.py`

 * *Files identical despite different names*

