# Comparing `tmp/aider-chat-0.8.1.tar.gz` & `tmp/aider-chat-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aider-chat-0.8.1.tar", last modified: Sat Jul  8 04:19:53 2023, max compression
+gzip compressed data, was "aider-chat-0.8.2.tar", last modified: Sat Jul  8 13:10:32 2023, max compression
```

## Comparing `aider-chat-0.8.1.tar` & `aider-chat-0.8.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.505076 aider-chat-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-08 04:19:37.000000 aider-chat-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 04:19:37.000000 aider-chat-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-08 04:19:53.505076 aider-chat-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-07-08 04:19:37.000000 aider-chat-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.501075 aider-chat-0.8.1/aider/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.501075 aider-chat-0.8.1/aider/coders/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34358 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/base_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/base_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/editblock_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/editblock_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/editblock_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/editblock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/single_wholefile_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/single_wholefile_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/wholefile_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/wholefile_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/wholefile_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/wholefile_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.501075 aider-chat-0.8.1/aider_chat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.505076 aider-chat-0.8.1/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:37.000000 aider-chat-0.8.1/benchmark/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18449 2023-07-08 04:19:37.000000 aider-chat-0.8.1/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-08 04:19:37.000000 aider-chat-0.8.1/benchmark/prompts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-08 04:19:37.000000 aider-chat-0.8.1/benchmark/rungrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-08 04:19:37.000000 aider-chat-0.8.1/benchmark/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 04:19:37.000000 aider-chat-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 04:19:53.505076 aider-chat-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-08 04:19:37.000000 aider-chat-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.505076 aider-chat-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_editblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_wholefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.455631 aider-chat-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-08 13:10:22.000000 aider-chat-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 13:10:22.000000 aider-chat-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-08 13:10:32.455631 aider-chat-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-07-08 13:10:22.000000 aider-chat-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.451631 aider-chat-0.8.2/aider/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.451631 aider-chat-0.8.2/aider/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34402 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/base_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/base_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/editblock_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/editblock_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/editblock_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/editblock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/single_wholefile_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/single_wholefile_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/wholefile_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/wholefile_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/wholefile_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/coders/wholefile_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-08 13:10:22.000000 aider-chat-0.8.2/aider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.455631 aider-chat-0.8.2/aider_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 13:10:32.000000 aider-chat-0.8.2/aider_chat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.455631 aider-chat-0.8.2/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:22.000000 aider-chat-0.8.2/benchmark/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18449 2023-07-08 13:10:22.000000 aider-chat-0.8.2/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-08 13:10:22.000000 aider-chat-0.8.2/benchmark/prompts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-08 13:10:22.000000 aider-chat-0.8.2/benchmark/rungrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-08 13:10:22.000000 aider-chat-0.8.2/benchmark/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 13:10:22.000000 aider-chat-0.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 13:10:32.455631 aider-chat-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-08 13:10:22.000000 aider-chat-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:32.455631 aider-chat-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_editblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-07-08 13:10:22.000000 aider-chat-0.8.2/tests/test_wholefile.py
```

### Comparing `aider-chat-0.8.1/LICENSE.txt` & `aider-chat-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/PKG-INFO` & `aider-chat-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.8.1
+Version: 0.8.2
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
```

### Comparing `aider-chat-0.8.1/README.md` & `aider-chat-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/coders/base_coder.py` & `aider-chat-0.8.2/aider/coders/base_coder.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,14 +481,16 @@
         try:
             interrupted = self.send(messages, functions=self.functions)
         except ExhaustedContextWindow:
             exhausted = True
         except openai.error.InvalidRequestError as err:
             if "maximum context length" in str(err):
                 exhausted = True
+            else:
+                raise err
 
         if exhausted:
             self.num_exhausted_context_windows += 1
             self.io.tool_error("The chat session is larger than the context window!\n")
             self.commands.cmd_tokens("")
             self.io.tool_error("\nTo reduce token usage:")
             self.io.tool_error(" - Use /drop to remove unneeded files from the chat session.")
```

### Comparing `aider-chat-0.8.1/aider/coders/editblock_coder.py` & `aider-chat-0.8.2/aider/coders/editblock_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/coders/editblock_func_coder.py` & `aider-chat-0.8.2/aider/coders/editblock_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/coders/editblock_func_prompts.py` & `aider-chat-0.8.2/aider/coders/editblock_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/coders/editblock_prompts.py` & `aider-chat-0.8.2/aider/coders/editblock_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/coders/single_wholefile_func_coder.py` & `aider-chat-0.8.2/aider/coders/single_wholefile_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/coders/single_wholefile_func_prompts.py` & `aider-chat-0.8.2/aider/coders/single_wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/coders/wholefile_coder.py` & `aider-chat-0.8.2/aider/coders/wholefile_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/coders/wholefile_func_coder.py` & `aider-chat-0.8.2/aider/coders/wholefile_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/coders/wholefile_func_prompts.py` & `aider-chat-0.8.2/aider/coders/wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/coders/wholefile_prompts.py` & `aider-chat-0.8.2/aider/coders/wholefile_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/commands.py` & `aider-chat-0.8.2/aider/commands.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/diffs.py` & `aider-chat-0.8.2/aider/diffs.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/dump.py` & `aider-chat-0.8.2/aider/dump.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/io.py` & `aider-chat-0.8.2/aider/io.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/main.py` & `aider-chat-0.8.2/aider/main.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/models.py` & `aider-chat-0.8.2/aider/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,14 @@
             self.edit_format = "diff"
             self.use_repo_map = True
             self.send_undo_reply = True
 
             if tokens == 8:
                 self.prompt_price = 0.03
                 self.completion_price = 0.06
-                self.always_available = True
             elif tokens == 32:
                 self.prompt_price = 0.06
                 self.completion_price = 0.12
 
             return
 
         if self.is_gpt35():
```

### Comparing `aider-chat-0.8.1/aider/prompts.py` & `aider-chat-0.8.2/aider/prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/repomap.py` & `aider-chat-0.8.2/aider/repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider/utils.py` & `aider-chat-0.8.2/aider/utils.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider_chat.egg-info/PKG-INFO` & `aider-chat-0.8.2/aider_chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.8.1
+Version: 0.8.2
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
```

### Comparing `aider-chat-0.8.1/aider_chat.egg-info/SOURCES.txt` & `aider-chat-0.8.2/aider_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/aider_chat.egg-info/requires.txt` & `aider-chat-0.8.2/aider_chat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/benchmark/benchmark.py` & `aider-chat-0.8.2/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/benchmark/rungrid.py` & `aider-chat-0.8.2/benchmark/rungrid.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/benchmark/test_benchmark.py` & `aider-chat-0.8.2/benchmark/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/requirements.txt` & `aider-chat-0.8.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/setup.py` & `aider-chat-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/tests/test_coder.py` & `aider-chat-0.8.2/tests/test_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/tests/test_commands.py` & `aider-chat-0.8.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/tests/test_editblock.py` & `aider-chat-0.8.2/tests/test_editblock.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/tests/test_io.py` & `aider-chat-0.8.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/tests/test_main.py` & `aider-chat-0.8.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/tests/test_models.py` & `aider-chat-0.8.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/tests/test_repomap.py` & `aider-chat-0.8.2/tests/test_repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.1/tests/test_wholefile.py` & `aider-chat-0.8.2/tests/test_wholefile.py`

 * *Files identical despite different names*

