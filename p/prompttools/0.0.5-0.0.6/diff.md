# Comparing `tmp/prompttools-0.0.5.tar.gz` & `tmp/prompttools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompttools-0.0.5.tar", last modified: Thu Jul  6 22:49:45 2023, max compression
+gzip compressed data, was "prompttools-0.0.6.tar", last modified: Sat Jul  8 01:07:06 2023, max compression
```

## Comparing `prompttools-0.0.5.tar` & `prompttools-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,60 @@
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 22:49:45.693602 prompttools-0.0.5/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2102 2023-07-05 23:51:56.000000 prompttools-0.0.5/LICENSE
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5109 2023-07-06 22:49:45.693301 prompttools-0.0.5/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     4508 2023-07-05 23:52:26.000000 prompttools-0.0.5/README.md
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 22:49:45.692923 prompttools-0.0.5/prompttools.egg-info/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5109 2023-07-06 22:49:45.000000 prompttools-0.0.5/prompttools.egg-info/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      278 2023-07-06 22:49:45.000000 prompttools-0.0.5/prompttools.egg-info/SOURCES.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 22:49:45.000000 prompttools-0.0.5/prompttools.egg-info/dependency_links.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-04 19:41:18.000000 prompttools-0.0.5/prompttools.egg-info/not-zip-safe
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-06 22:49:45.000000 prompttools-0.0.5/prompttools.egg-info/requires.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 22:49:45.000000 prompttools-0.0.5/prompttools.egg-info/top_level.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      698 2023-07-06 22:48:41.000000 prompttools-0.0.5/pyproject.toml
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-05 21:42:59.000000 prompttools-0.0.5/requirements.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-07-06 22:49:45.693707 prompttools-0.0.5/setup.cfg
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3737 2023-07-06 22:49:34.000000 prompttools-0.0.5/setup.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-07-06 22:48:45.000000 prompttools-0.0.5/version.txt
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.733103 prompttools-0.0.6/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2102 2023-07-05 23:51:56.000000 prompttools-0.0.6/LICENSE
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5647 2023-07-08 01:07:06.732721 prompttools-0.0.6/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5046 2023-07-08 00:44:14.000000 prompttools-0.0.6/README.md
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.694342 prompttools-0.0.6/prompttools/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:50:24.000000 prompttools-0.0.6/prompttools/__init__.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.705756 prompttools-0.0.6/prompttools/experiment/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-04 19:36:44.000000 prompttools-0.0.6/prompttools/experiment/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      315 2023-07-08 00:40:21.000000 prompttools-0.0.6/prompttools/experiment/error.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)    12162 2023-07-08 00:38:48.000000 prompttools-0.0.6/prompttools/experiment/experiment.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2614 2023-07-08 00:35:30.000000 prompttools-0.0.6/prompttools/experiment/openai_chat_experiment.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2977 2023-07-08 00:35:30.000000 prompttools-0.0.6/prompttools/experiment/openai_completion_experiment.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      184 2023-07-05 16:26:17.000000 prompttools-0.0.6/prompttools/experiment/openai_function_experiment.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      184 2023-07-05 16:26:43.000000 prompttools-0.0.6/prompttools/experiment/vector_database_experiment.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.709756 prompttools-0.0.6/prompttools/experiment/widgets/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:20.000000 prompttools-0.0.6/prompttools/experiment/widgets/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2540 2023-07-05 19:53:43.000000 prompttools-0.0.6/prompttools/experiment/widgets/comparison.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2773 2023-07-05 18:58:31.000000 prompttools-0.0.6/prompttools/experiment/widgets/feedback.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      227 2023-07-05 19:13:42.000000 prompttools-0.0.6/prompttools/experiment/widgets/utility.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.718925 prompttools-0.0.6/prompttools/harness/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-04 19:36:44.000000 prompttools-0.0.6/prompttools/harness/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2205 2023-07-08 00:35:30.000000 prompttools-0.0.6/prompttools/harness/chat_history_harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2684 2023-07-05 23:52:26.000000 prompttools-0.0.6/prompttools/harness/chat_model_comparison_harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      184 2023-07-05 16:26:46.000000 prompttools-0.0.6/prompttools/harness/document_retrieval_harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      185 2023-07-05 16:26:17.000000 prompttools-0.0.6/prompttools/harness/function_call_harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2314 2023-07-05 22:40:03.000000 prompttools-0.0.6/prompttools/harness/harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3105 2023-07-08 00:35:30.000000 prompttools-0.0.6/prompttools/harness/prompt_template_harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3175 2023-07-08 00:35:30.000000 prompttools-0.0.6/prompttools/harness/system_prompt_harness.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.720385 prompttools-0.0.6/prompttools/mock/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:14.000000 prompttools-0.0.6/prompttools/mock/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1246 2023-07-05 22:19:30.000000 prompttools-0.0.6/prompttools/mock/mock.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.723026 prompttools-0.0.6/prompttools/requests/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-04 19:36:44.000000 prompttools-0.0.6/prompttools/requests/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2591 2023-07-05 19:53:59.000000 prompttools-0.0.6/prompttools/requests/request_queue.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1624 2023-07-05 22:40:03.000000 prompttools-0.0.6/prompttools/requests/retries.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.725928 prompttools-0.0.6/prompttools/testing/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:08.000000 prompttools-0.0.6/prompttools/testing/__init__.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.727678 prompttools-0.0.6/prompttools/testing/error/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:11.000000 prompttools-0.0.6/prompttools/testing/error/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      840 2023-07-05 19:53:59.000000 prompttools-0.0.6/prompttools/testing/error/failure.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3788 2023-07-08 00:33:36.000000 prompttools-0.0.6/prompttools/testing/prompttest.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.731768 prompttools-0.0.6/prompttools/testing/runner/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:10.000000 prompttools-0.0.6/prompttools/testing/runner/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     4261 2023-07-08 00:35:30.000000 prompttools-0.0.6/prompttools/testing/runner/prompt_template_runner.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1638 2023-07-05 22:40:03.000000 prompttools-0.0.6/prompttools/testing/runner/runner.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     4199 2023-07-08 00:35:30.000000 prompttools-0.0.6/prompttools/testing/runner/system_prompt_runner.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      177 2023-07-05 19:53:59.000000 prompttools-0.0.6/prompttools/testing/threshold_type.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       89 2023-07-08 01:06:44.000000 prompttools-0.0.6/prompttools/version.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 01:07:06.698298 prompttools-0.0.6/prompttools.egg-info/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5647 2023-07-08 01:07:06.000000 prompttools-0.0.6/prompttools.egg-info/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1675 2023-07-08 01:07:06.000000 prompttools-0.0.6/prompttools.egg-info/SOURCES.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-08 01:07:06.000000 prompttools-0.0.6/prompttools.egg-info/dependency_links.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-04 19:41:18.000000 prompttools-0.0.6/prompttools.egg-info/not-zip-safe
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-08 01:07:06.000000 prompttools-0.0.6/prompttools.egg-info/requires.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       12 2023-07-08 01:07:06.000000 prompttools-0.0.6/prompttools.egg-info/top_level.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      698 2023-07-08 00:40:54.000000 prompttools-0.0.6/pyproject.toml
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-05 21:42:59.000000 prompttools-0.0.6/requirements.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-07-08 01:07:06.733588 prompttools-0.0.6/setup.cfg
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3737 2023-07-08 01:06:53.000000 prompttools-0.0.6/setup.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-07-08 00:40:51.000000 prompttools-0.0.6/version.txt
```

### Comparing `prompttools-0.0.5/LICENSE` & `prompttools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.5/PKG-INFO` & `prompttools-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompttools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tools for LLM prompt testing and experimentation
 Home-page: https://github.com/hegelai/prompttools
 Author: Hegel AI
 Author-email: Hegel AI <team@hegel-ai.com>
 License: Proprietary
 Project-URL: Homepage, https://github.com/hegelai/prompttools
 Project-URL: Bug Tracker, https://github.com/hegelai/prompttools
@@ -15,14 +15,38 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PromptTools
 
 Welcome to `prompttools` created by [Hegel AI](https://hegel-ai.com/)! This repo offers a set of free, open-source tools for testing and experimenting with prompts. The core idea is to enable developers to evaluate prompts using familiar interfaces like _code_ and _notebooks_.
 
+## Quickstart
+
+To install `prompttools`, you can use `pip`:
+
+```
+pip install prompttools
+```
+
+You can run a simple example of a `prompttools` with the following
+
+```
+DEBUG=1 python examples/prompttests/example.py
+```
+
+To run the example outside of `DEBUG` mode, you'll need to bring your own OpenAI API key. 
+This is because `prompttools` makes a call to OpenAI from your machine. For example:
+
+```
+OPENAI_API_KEY=sk-... python examples/prompttests/example.py
+```
+
+You can see the full example [here](/examples/prompttests/example.py).
+
+
 ## Using `prompttools`
 
 There are primarily two ways you can use `prompttools` in your LLM workflow:
 
 1. Run experiments in [notebooks](/examples/notebooks/).
 1. Write [unit tests](/examples/prompttests/example.py) and integrate them into your CI/CD workflow [via Github Actions](/.github/workflows/post-commit.yaml).
```

### Comparing `prompttools-0.0.5/README.md` & `prompttools-0.0.6/prompttools.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,52 @@
+Metadata-Version: 2.1
+Name: prompttools
+Version: 0.0.6
+Summary: Tools for LLM prompt testing and experimentation
+Home-page: https://github.com/hegelai/prompttools
+Author: Hegel AI
+Author-email: Hegel AI <team@hegel-ai.com>
+License: Proprietary
+Project-URL: Homepage, https://github.com/hegelai/prompttools
+Project-URL: Bug Tracker, https://github.com/hegelai/prompttools
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PromptTools
 
 Welcome to `prompttools` created by [Hegel AI](https://hegel-ai.com/)! This repo offers a set of free, open-source tools for testing and experimenting with prompts. The core idea is to enable developers to evaluate prompts using familiar interfaces like _code_ and _notebooks_.
 
+## Quickstart
+
+To install `prompttools`, you can use `pip`:
+
+```
+pip install prompttools
+```
+
+You can run a simple example of a `prompttools` with the following
+
+```
+DEBUG=1 python examples/prompttests/example.py
+```
+
+To run the example outside of `DEBUG` mode, you'll need to bring your own OpenAI API key. 
+This is because `prompttools` makes a call to OpenAI from your machine. For example:
+
+```
+OPENAI_API_KEY=sk-... python examples/prompttests/example.py
+```
+
+You can see the full example [here](/examples/prompttests/example.py).
+
+
 ## Using `prompttools`
 
 There are primarily two ways you can use `prompttools` in your LLM workflow:
 
 1. Run experiments in [notebooks](/examples/notebooks/).
 1. Write [unit tests](/examples/prompttests/example.py) and integrate them into your CI/CD workflow [via Github Actions](/.github/workflows/post-commit.yaml).
```

### Comparing `prompttools-0.0.5/pyproject.toml` & `prompttools-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prompttools"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Hegel AI", email="team@hegel-ai.com" },
 ]
 description = "Tools for LLM prompt testing and experimentation"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `prompttools-0.0.5/setup.py` & `prompttools-0.0.6/setup.py`

 * *Files identical despite different names*

