# Comparing `tmp/aider-chat-0.8.0.tar.gz` & `tmp/aider-chat-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aider-chat-0.8.0.tar", last modified: Thu Jul  6 21:09:18 2023, max compression
+gzip compressed data, was "aider-chat-0.8.1.tar", last modified: Sat Jul  8 04:19:53 2023, max compression
```

## Comparing `aider-chat-0.8.0.tar` & `aider-chat-0.8.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:18.870857 aider-chat-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-06 21:09:08.000000 aider-chat-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 21:09:08.000000 aider-chat-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-06 21:09:18.870857 aider-chat-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-07-06 21:09:08.000000 aider-chat-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:18.866856 aider-chat-0.8.0/aider/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:18.870857 aider-chat-0.8.0/aider/coders/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34171 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/base_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/base_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/editblock_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/editblock_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/editblock_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/editblock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/single_wholefile_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/single_wholefile_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/wholefile_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/wholefile_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/wholefile_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/coders/wholefile_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13059 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-06 21:09:08.000000 aider-chat-0.8.0/aider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:18.870857 aider-chat-0.8.0/aider_chat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-06 21:09:18.000000 aider-chat-0.8.0/aider_chat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-06 21:09:18.000000 aider-chat-0.8.0/aider_chat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:09:18.000000 aider-chat-0.8.0/aider_chat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 21:09:18.000000 aider-chat-0.8.0/aider_chat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-06 21:09:18.000000 aider-chat-0.8.0/aider_chat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:09:18.000000 aider-chat-0.8.0/aider_chat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:18.870857 aider-chat-0.8.0/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:08.000000 aider-chat-0.8.0/benchmark/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18449 2023-07-06 21:09:08.000000 aider-chat-0.8.0/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-06 21:09:08.000000 aider-chat-0.8.0/benchmark/prompts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-06 21:09:08.000000 aider-chat-0.8.0/benchmark/rungrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-06 21:09:08.000000 aider-chat-0.8.0/benchmark/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-06 21:09:08.000000 aider-chat-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:09:18.870857 aider-chat-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-06 21:09:08.000000 aider-chat-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:18.870857 aider-chat-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:09:08.000000 aider-chat-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-06 21:09:08.000000 aider-chat-0.8.0/tests/test_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-06 21:09:08.000000 aider-chat-0.8.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-06 21:09:08.000000 aider-chat-0.8.0/tests/test_editblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-06 21:09:08.000000 aider-chat-0.8.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-06 21:09:08.000000 aider-chat-0.8.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 21:09:08.000000 aider-chat-0.8.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-06 21:09:08.000000 aider-chat-0.8.0/tests/test_repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-06 21:09:08.000000 aider-chat-0.8.0/tests/test_wholefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.505076 aider-chat-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-08 04:19:37.000000 aider-chat-0.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 04:19:37.000000 aider-chat-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-08 04:19:53.505076 aider-chat-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-07-08 04:19:37.000000 aider-chat-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.501075 aider-chat-0.8.1/aider/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.501075 aider-chat-0.8.1/aider/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34358 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/base_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/base_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/editblock_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/editblock_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/editblock_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/editblock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/single_wholefile_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/single_wholefile_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/wholefile_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/wholefile_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/wholefile_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/coders/wholefile_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-08 04:19:37.000000 aider-chat-0.8.1/aider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.501075 aider-chat-0.8.1/aider_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 04:19:53.000000 aider-chat-0.8.1/aider_chat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.505076 aider-chat-0.8.1/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:37.000000 aider-chat-0.8.1/benchmark/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18449 2023-07-08 04:19:37.000000 aider-chat-0.8.1/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-08 04:19:37.000000 aider-chat-0.8.1/benchmark/prompts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-08 04:19:37.000000 aider-chat-0.8.1/benchmark/rungrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-08 04:19:37.000000 aider-chat-0.8.1/benchmark/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 04:19:37.000000 aider-chat-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 04:19:53.505076 aider-chat-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-08 04:19:37.000000 aider-chat-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:53.505076 aider-chat-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_editblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-07-08 04:19:37.000000 aider-chat-0.8.1/tests/test_wholefile.py
```

### Comparing `aider-chat-0.8.0/LICENSE.txt` & `aider-chat-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/PKG-INFO` & `aider-chat-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.8.0
+Version: 0.8.1
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
 
 `aider` is a command-line chat tool that allows you to write and edit
 code with OpenAI's GPT models.  You can ask GPT to help you start
 a new project, or modify code in your existing git repo.
 Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting. 
 It also has features that [help GPT-4 understand and modify larger codebases](https://aider.chat/docs/ctags.html).
 
 
+- [FAQ](https://aider.chat/docs/faq.html)
 
 ## Getting started
 
 ```
 $ pip install aider-chat
 $ export OPENAI_API_KEY=your-key-goes-here
 $ aider myapp.py
@@ -62,19 +63,17 @@
   * GitHub: `python -m pip install git+https://github.com/paul-gauthier/aider.git`
   * Local clone: `python -m pip install -e .` 
 
 2. Set up your OpenAI API key:
   * As an environment variable:
     * `export OPENAI_API_KEY=sk-...` on Linux or Mac
     * `setx OPENAI_API_KEY sk-...` in Windows PowerShell
-  * Or include `openai-api-key: sk-...` in an `.aider.config.yml` file in your current directory or at the root of your git repo, alongside the `.git` dir.
+  * Or include `openai-api-key: sk-...` in an `.aider.conf.yml` file in your home directory or at the root of your git repo, alongside the `.git` dir.
 
-3. Optionally, install [universal ctags](https://github.com/universal-ctags/ctags). This is helpful if you plan to use aider and GPT-4 with repositories that have more than a handful of files.  This allows aider to build a [map of your entire git repo](https://aider.chat/docs/ctags.html) and share it with GPT to help it better understand and modify large codebases.
-  * The `ctags` command needs to be on your shell path so that it will run by default when aider invokes `ctags ...`.
-  * You need a build which includes the json feature. You can check by running `ctags --version` and looking for `+json` in the `Optional compiled features` list.
+3. Optionally, install [universal ctags](https://github.com/universal-ctags/ctags). This is helpful if you plan to use aider and GPT-4 with repositories that have more than a handful of files.  This allows aider to build a [map of your entire git repo](https://aider.chat/docs/ctags.html) and share it with GPT to help it better understand and modify large codebases. See the [FAQ entry about ctags](https://aider.chat/docs/faq.html#how-do-i-get-ctags-working) for more info.
 
 ## Usage
 
 Run the `aider` tool by executing the following command:
 
 ```
 aider <file1> <file2> ...
```

### Comparing `aider-chat-0.8.0/README.md` & `aider-chat-0.8.1/aider_chat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+Metadata-Version: 2.1
+Name: aider-chat
+Version: 0.8.1
+Summary: aider is GPT powered coding in your terminal
+Home-page: https://github.com/paul-gauthier/aider
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # aider is GPT powered coding in your terminal
 
 `aider` is a command-line chat tool that allows you to write and edit
 code with OpenAI's GPT models.  You can ask GPT to help you start
 a new project, or modify code in your existing git repo.
 Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting. 
 It also has features that [help GPT-4 understand and modify larger codebases](https://aider.chat/docs/ctags.html).
 
-![aider screencast](assets/screencast.svg)
 
-- [Getting started](#getting-started)
-- [Example chat transcripts](#example-chat-transcripts)
-- [Features](#features)
-- [Installation](#installation)
-- [Usage](#usage)
-- [In-chat commands](#in-chat-commands)
-- [Tips](#tips)
-- [GPT-4 vs GPT-3.5](#gpt-4-vs-gpt-35)
+- [FAQ](https://aider.chat/docs/faq.html)
 
 ## Getting started
 
 ```
 $ pip install aider-chat
 $ export OPENAI_API_KEY=your-key-goes-here
 $ aider myapp.py
@@ -63,19 +63,17 @@
   * GitHub: `python -m pip install git+https://github.com/paul-gauthier/aider.git`
   * Local clone: `python -m pip install -e .` 
 
 2. Set up your OpenAI API key:
   * As an environment variable:
     * `export OPENAI_API_KEY=sk-...` on Linux or Mac
     * `setx OPENAI_API_KEY sk-...` in Windows PowerShell
-  * Or include `openai-api-key: sk-...` in an `.aider.config.yml` file in your current directory or at the root of your git repo, alongside the `.git` dir.
+  * Or include `openai-api-key: sk-...` in an `.aider.conf.yml` file in your home directory or at the root of your git repo, alongside the `.git` dir.
 
-3. Optionally, install [universal ctags](https://github.com/universal-ctags/ctags). This is helpful if you plan to use aider and GPT-4 with repositories that have more than a handful of files.  This allows aider to build a [map of your entire git repo](https://aider.chat/docs/ctags.html) and share it with GPT to help it better understand and modify large codebases.
-  * The `ctags` command needs to be on your shell path so that it will run by default when aider invokes `ctags ...`.
-  * You need a build which includes the json feature. You can check by running `ctags --version` and looking for `+json` in the `Optional compiled features` list.
+3. Optionally, install [universal ctags](https://github.com/universal-ctags/ctags). This is helpful if you plan to use aider and GPT-4 with repositories that have more than a handful of files.  This allows aider to build a [map of your entire git repo](https://aider.chat/docs/ctags.html) and share it with GPT to help it better understand and modify large codebases. See the [FAQ entry about ctags](https://aider.chat/docs/faq.html#how-do-i-get-ctags-working) for more info.
 
 ## Usage
 
 Run the `aider` tool by executing the following command:
 
 ```
 aider <file1> <file2> ...
```

### Comparing `aider-chat-0.8.0/aider/coders/base_coder.py` & `aider-chat-0.8.1/aider/coders/base_coder.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,15 +204,22 @@
         if len(self.abs_fnames) == 1:
             self.root = os.path.dirname(list(self.abs_fnames)[0])
         elif self.abs_fnames:
             self.root = os.path.commonpath(list(self.abs_fnames))
         else:
             self.root = os.getcwd()
 
-        self.root = os.path.abspath(self.root)
+        self.root = utils.safe_abs_path(self.root)
+
+    def add_rel_fname(self, rel_fname):
+        self.abs_fnames.add(self.abs_root_path(rel_fname))
+
+    def abs_root_path(self, path):
+        res = Path(self.root) / path
+        return utils.safe_abs_path(res)
 
     def set_repo(self, cmd_line_fnames):
         if not cmd_line_fnames:
             cmd_line_fnames = ["."]
 
         repo_paths = []
         for fname in cmd_line_fnames:
@@ -222,15 +229,15 @@
                 fname.parent.mkdir(parents=True, exist_ok=True)
                 fname.touch()
 
             fname = fname.resolve()
 
             try:
                 repo_path = git.Repo(fname, search_parent_directories=True).working_dir
-                repo_path = os.path.abspath(repo_path)
+                repo_path = utils.safe_abs_path(repo_path)
                 repo_paths.append(repo_path)
             except git.exc.InvalidGitRepositoryError:
                 pass
 
             if fname.is_dir():
                 continue
 
@@ -243,15 +250,15 @@
         if num_repos > 1:
             self.io.tool_error("Files are in different git repos.")
             return
 
         # https://github.com/gitpython-developers/GitPython/issues/427
         self.repo = git.Repo(repo_paths.pop(), odbt=git.GitDB)
 
-        self.root = os.path.abspath(self.repo.working_tree_dir)
+        self.root = utils.safe_abs_path(self.repo.working_tree_dir)
 
         new_files = []
         for fname in self.abs_fnames:
             relative_fname = self.get_rel_fname(fname)
 
             tracked_files = set(self.get_tracked_files())
             if relative_fname not in tracked_files:
@@ -324,15 +331,15 @@
     def get_files_content(self, fnames=None):
         if not fnames:
             fnames = self.abs_fnames
 
         prompt = ""
         for fname, content in self.get_abs_fnames_content():
             relative_fname = self.get_rel_fname(fname)
-            prompt = "\n"
+            prompt += "\n"
             prompt += relative_fname
             prompt += f"\n{self.fence[0]}\n"
             prompt += content
             prompt += f"{self.fence[1]}\n"
 
         return prompt
 
@@ -580,15 +587,15 @@
         for rel_fname in mentioned_rel_fnames:
             self.io.tool_output(rel_fname)
 
         if not self.io.confirm_ask("Add these files to the chat?"):
             return
 
         for rel_fname in mentioned_rel_fnames:
-            self.abs_fnames.add(os.path.abspath(os.path.join(self.root, rel_fname)))
+            self.add_rel_fname(rel_fname)
 
         return prompts.added_files.format(fnames=", ".join(mentioned_rel_fnames))
 
     @backoff.on_exception(
         backoff.expo,
         (
             Timeout,
@@ -902,28 +909,28 @@
         else:
             files = self.get_inchat_relative_files()
 
         return sorted(set(files))
 
     def get_all_abs_files(self):
         files = self.get_all_relative_files()
-        files = [os.path.abspath(os.path.join(self.root, path)) for path in files]
+        files = [self.abs_root_path(path) for path in files]
         return files
 
     def get_last_modified(self):
         files = self.get_all_abs_files()
         if not files:
             return 0
         return max(Path(path).stat().st_mtime for path in files)
 
     def get_addable_relative_files(self):
         return set(self.get_all_relative_files()) - set(self.get_inchat_relative_files())
 
     def allowed_to_edit(self, path, write_content=None):
-        full_path = os.path.abspath(os.path.join(self.root, path))
+        full_path = self.abs_root_path(path)
 
         if full_path in self.abs_fnames:
             if write_content:
                 self.io.write_text(full_path, write_content)
             return full_path
 
         if not Path(full_path).exists():
@@ -950,14 +957,16 @@
 
         if write_content:
             self.io.write_text(full_path, write_content)
 
         return full_path
 
     def get_tracked_files(self):
+        if not self.repo:
+            return []
         # convert to appropriate os.sep, since git always normalizes to /
         files = set(self.repo.git.ls_files().splitlines())
         res = set(str(Path(PurePosixPath(path))) for path in files)
         return res
 
     apply_update_errors = 0
```

### Comparing `aider-chat-0.8.0/aider/coders/editblock_coder.py` & `aider-chat-0.8.1/aider/coders/editblock_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider/coders/editblock_func_coder.py` & `aider-chat-0.8.1/aider/coders/editblock_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider/coders/editblock_func_prompts.py` & `aider-chat-0.8.1/aider/coders/editblock_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider/coders/editblock_prompts.py` & `aider-chat-0.8.1/aider/coders/editblock_prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     # Func to multiply
     def mul(a,b)
 =======
     # updated comment
     # Function to add
     def add(a,b):
 >>>>>>> UPDATED
+```
 
 Every *edit block* must be fenced w/triple backticks with the correct code language.
 Every *edit block* must start with the full path! *NEVER* propose edit blocks for *read-only* files.
 The ORIGINAL section must be an *exact* set of lines from the file:
 - NEVER SKIP LINES!
 - Include all original leading spaces and indentation!
```

### Comparing `aider-chat-0.8.0/aider/coders/single_wholefile_func_coder.py` & `aider-chat-0.8.1/aider/coders/single_wholefile_func_coder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 from aider import diffs
 
 from ..dump import dump  # noqa: F401
 from .base_coder import Coder
 from .single_wholefile_func_prompts import SingleWholeFileFunctionPrompts
 
 
@@ -84,15 +82,15 @@
 
         return res
 
     def live_diffs(self, fname, content, final):
         lines = content.splitlines(keepends=True)
 
         # ending an existing block
-        full_path = os.path.abspath(os.path.join(self.root, fname))
+        full_path = self.abs_root_path(fname)
 
         content = self.io.read_text(full_path)
         if content is None:
             orig_lines = []
         else:
             orig_lines = content.splitlines()
```

### Comparing `aider-chat-0.8.0/aider/coders/single_wholefile_func_prompts.py` & `aider-chat-0.8.1/aider/coders/single_wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider/coders/wholefile_coder.py` & `aider-chat-0.8.1/aider/coders/wholefile_coder.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,18 @@
             context += "# Context:\n"
             for msg in history:
                 if msg["role"] == "user":
                     context += msg["role"].upper() + ": " + msg["content"] + "\n"
         return context
 
     def render_incremental_response(self, final):
-        return self.update_files(mode="diff")
+        try:
+            return self.update_files(mode="diff")
+        except ValueError:
+            return self.partial_response_content
 
     def update_files(self, mode="update"):
         content = self.partial_response_content
 
         edited = set()
         chat_files = self.get_inchat_relative_files()
 
@@ -48,28 +51,20 @@
             if line.startswith(self.fence[0]) or line.startswith(self.fence[1]):
                 if fname is not None:
                     # ending an existing block
                     saw_fname = None
 
                     full_path = (Path(self.root) / fname).absolute()
 
-                    if mode == "diff" and full_path.exists():
-                        orig_lines = self.io.read_text(full_path).splitlines(keepends=True)
-
-                        show_diff = diffs.diff_partial_update(
-                            orig_lines,
-                            new_lines,
-                            final=True,
-                        ).splitlines()
-                        output += show_diff
-                    else:
-                        if self.allowed_to_edit(fname):
-                            edited.add(fname)
-                            new_lines = "".join(new_lines)
-                            self.io.write_text(full_path, new_lines)
+                    if mode == "diff":
+                        output += self.do_live_diff(full_path, new_lines)
+                    elif self.allowed_to_edit(fname):
+                        edited.add(fname)
+                        new_lines = "".join(new_lines)
+                        self.io.write_text(full_path, new_lines)
 
                     fname = None
                     new_lines = []
                     continue
 
                 # fname==None ... starting a new block
                 if i > 0:
@@ -102,27 +97,33 @@
 
                 output.append(line)
 
         if mode == "diff":
             if fname is not None:
                 # ending an existing block
                 full_path = (Path(self.root) / fname).absolute()
-
-                if mode == "diff" and full_path.exists():
-                    orig_lines = self.io.read_text(full_path).splitlines(keepends=True)
-
-                    show_diff = diffs.diff_partial_update(
-                        orig_lines,
-                        new_lines,
-                    ).splitlines()
-                    output += show_diff
-
+                output += self.do_live_diff(full_path, new_lines)
             return "\n".join(output)
 
         if fname:
             full_path = self.allowed_to_edit(fname)
             if full_path:
                 edited.add(fname)
                 new_lines = "".join(new_lines)
                 self.io.write_text(full_path, new_lines)
 
         return edited
+
+    def do_live_diff(self, full_path, new_lines):
+        if full_path.exists():
+            orig_lines = self.io.read_text(full_path).splitlines(keepends=True)
+
+            show_diff = diffs.diff_partial_update(
+                orig_lines,
+                new_lines,
+                final=True,
+            ).splitlines()
+            output = show_diff
+        else:
+            output = ["```"] + new_lines + ["```"]
+
+        return output
```

### Comparing `aider-chat-0.8.0/aider/coders/wholefile_func_coder.py` & `aider-chat-0.8.1/aider/coders/wholefile_func_coder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 from aider import diffs
 
 from ..dump import dump  # noqa: F401
 from .base_coder import Coder
 from .wholefile_func_prompts import WholeFileFunctionPrompts
 
 
@@ -95,15 +93,15 @@
 
         return res
 
     def live_diffs(self, fname, content, final):
         lines = content.splitlines(keepends=True)
 
         # ending an existing block
-        full_path = os.path.abspath(os.path.join(self.root, fname))
+        full_path = self.abs_root_path(fname)
 
         content = self.io.read_text(full_path)
         if content is None:
             orig_lines = []
         else:
             orig_lines = content.splitlines()
```

### Comparing `aider-chat-0.8.0/aider/coders/wholefile_func_prompts.py` & `aider-chat-0.8.1/aider/coders/wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider/coders/wholefile_prompts.py` & `aider-chat-0.8.1/aider/coders/wholefile_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider/commands.py` & `aider-chat-0.8.1/aider/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
-import os
 import shlex
 import subprocess
 import sys
 from pathlib import Path
 
 import git
 import tiktoken
 from prompt_toolkit.completion import Completion
 
 from aider import prompts
 
+from .dump import dump  # noqa: F401
+
 
 class Commands:
     def __init__(self, io, coder):
         self.io = io
         self.coder = coder
         self.tokenizer = tiktoken.encoding_for_model(coder.main_model.name)
 
@@ -215,57 +216,72 @@
     def completions_add(self, partial):
         files = set(self.coder.get_all_relative_files())
         files = files - set(self.coder.get_inchat_relative_files())
         for fname in files:
             if partial.lower() in fname.lower():
                 yield Completion(fname, start_position=-len(partial))
 
+    def glob_filtered_to_repo(self, pattern):
+        matched_files = Path(self.coder.root).glob(pattern)
+        matched_files = [fn.relative_to(self.coder.root) for fn in matched_files]
+
+        # if repo, filter against it
+        if self.coder.repo:
+            git_files = self.coder.get_tracked_files()
+            matched_files = [fn for fn in matched_files if str(fn) in git_files]
+
+        return list(map(str, matched_files))
+
     def cmd_add(self, args):
-        "Add matching files to the chat session"
+        "Add matching files to the chat session using glob patterns"
 
         added_fnames = []
-        files = self.coder.get_all_relative_files()
+        git_added = []
+        git_files = self.coder.get_tracked_files()
+
         for word in args.split():
-            matched_files = [file for file in files if word in file]
+            matched_files = self.glob_filtered_to_repo(word)
 
             if not matched_files:
-                if self.coder.repo is not None:
-                    create_file = self.io.confirm_ask(
-                        (
-                            f"No files matched '{word}'. Do you want to create the file and add it"
-                            " to git?"
-                        ),
-                    )
+                if any(char in word for char in "*?[]"):
+                    self.io.tool_error(f"No files to add matching pattern: {word}")
                 else:
-                    create_file = self.io.confirm_ask(
+                    if Path(word).exists():
+                        matched_files = [word]
+                    elif self.io.confirm_ask(
                         f"No files matched '{word}'. Do you want to create the file?"
-                    )
+                    ):
+                        (Path(self.coder.root) / word).touch()
+                        matched_files = [word]
 
-                if create_file:
-                    (Path(self.coder.root) / word).touch()
+            for matched_file in matched_files:
+                abs_file_path = self.coder.abs_root_path(matched_file)
 
-                    matched_files = [word]
-                    if self.coder.repo is not None:
-                        self.coder.repo.git.add(os.path.join(self.coder.root, word))
-                        commit_message = f"aider: Created and added {word} to git."
-                        self.coder.repo.git.commit("-m", commit_message, "--no-verify")
-                else:
-                    self.io.tool_error(f"No files matched '{word}'")
+                if self.coder.repo and matched_file not in git_files:
+                    self.coder.repo.git.add(abs_file_path)
+                    git_added.append(matched_file)
 
-            for matched_file in matched_files:
-                abs_file_path = os.path.abspath(os.path.join(self.coder.root, matched_file))
                 if abs_file_path not in self.coder.abs_fnames:
                     content = self.io.read_text(abs_file_path)
                     if content is not None:
                         self.coder.abs_fnames.add(abs_file_path)
                         self.io.tool_output(f"Added {matched_file} to the chat")
                         added_fnames.append(matched_file)
+                    else:
+                        self.io.tool_error(f"Unable to read {matched_file}")
                 else:
                     self.io.tool_error(f"{matched_file} is already in the chat")
 
+        if self.coder.repo and git_added:
+            git_added = " ".join(git_added)
+            commit_message = f"aider: Added {git_added}"
+            self.coder.repo.git.commit("-m", commit_message, "--no-verify")
+            commit_hash = self.coder.repo.head.commit.hexsha[:7]
+            self.io.tool_output(f"Commit {commit_hash} {commit_message}")
+
         if not added_fnames:
             return
 
         # only reply if there's been some chatting since the last edit
         if not self.coder.cur_messages:
             return
 
@@ -283,26 +299,24 @@
         "Remove matching files from the chat session"
 
         if not args.strip():
             self.io.tool_output("Dropping all files from the chat session.")
             self.coder.abs_fnames = set()
 
         for word in args.split():
-            matched_files = [
-                file
-                for file in self.coder.abs_fnames
-                if word.lower() in os.path.relpath(file, self.coder.root).lower()
-            ]
+            matched_files = self.glob_filtered_to_repo(word)
+
             if not matched_files:
                 self.io.tool_error(f"No files matched '{word}'")
 
             for matched_file in matched_files:
-                relative_fname = os.path.relpath(matched_file, self.coder.root)
-                self.coder.abs_fnames.remove(matched_file)
-                self.io.tool_output(f"Removed {relative_fname} from the chat")
+                abs_fname = str(Path(matched_file).resolve())
+                if abs_fname in self.coder.abs_fnames:
+                    self.coder.abs_fnames.remove(abs_fname)
+                    self.io.tool_output(f"Removed {matched_file} from the chat")
 
     def cmd_run(self, args):
         "Run a shell command and optionally add the output to the chat"
         try:
             parsed_args = shlex.split(args)
             result = subprocess.run(
                 parsed_args, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, text=True
@@ -331,15 +345,15 @@
         "List all known files and those included in the chat session"
 
         files = self.coder.get_all_relative_files()
 
         other_files = []
         chat_files = []
         for file in files:
-            abs_file_path = os.path.abspath(os.path.join(self.coder.root, file))
+            abs_file_path = self.coder.abs_root_path(file)
             if abs_file_path in self.coder.abs_fnames:
                 chat_files.append(file)
             else:
                 other_files.append(file)
 
         if not chat_files and not other_files:
             self.io.tool_output("\nNo files in chat or git repo.")
```

### Comparing `aider-chat-0.8.0/aider/diffs.py` & `aider-chat-0.8.1/aider/diffs.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider/dump.py` & `aider-chat-0.8.1/aider/dump.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider/io.py` & `aider-chat-0.8.1/aider/io.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider/main.py` & `aider-chat-0.8.1/aider/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+from pathlib import Path
 
 import configargparse
 import git
 
 from aider import __version__, models
 from aider.coders import Coder
 from aider.io import InputOutput
@@ -19,19 +20,23 @@
 
 def main(args=None, input=None, output=None):
     if args is None:
         args = sys.argv[1:]
 
     git_root = get_git_root()
 
-    default_config_files = [
-        os.path.expanduser("~/.aider.conf.yml"),
-    ]
+    conf_fname = Path(".aider.conf.yml")
+
+    default_config_files = [conf_fname.resolve()]  # CWD
     if git_root:
-        default_config_files.insert(0, os.path.join(git_root, ".aider.conf.yml"))
+        git_conf = Path(git_root) / conf_fname  # git root
+        if git_conf not in default_config_files:
+            default_config_files.append(git_conf)
+    default_config_files.append(Path.home() / conf_fname)  # homedir
+    default_config_files = list(map(str, default_config_files))
 
     parser = configargparse.ArgumentParser(
         description="aider is GPT powered coding in your terminal",
         add_config_file_help=True,
         default_config_files=default_config_files,
         config_file_parser_class=configargparse.YAMLConfigFileParser,
         auto_env_var_prefix="AIDER_",
@@ -46,16 +51,16 @@
 
     parser.add_argument(
         "-c",
         "--config",
         is_config_file=True,
         metavar="CONFIG_FILE",
         help=(
-            "Specify the config file (default: search for .aider.conf.yml in git root or home"
-            " directory)"
+            "Specify the config file (default: search for .aider.conf.yml in git root, cwd"
+            " or home directory)"
         ),
     )
 
     parser.add_argument(
         "files",
         metavar="FILE",
         nargs="*",
@@ -251,14 +256,28 @@
         output=output,
         user_input_color=args.user_input_color,
         tool_output_color=args.tool_output_color,
         tool_error_color=args.tool_error_color,
         dry_run=args.dry_run,
     )
 
+    if not git_root and args.git:
+        if io.confirm_ask("No git repo found, create one to track GPT's changes (recommended)?"):
+            repo = git.Repo.init(os.getcwd())
+            with repo.config_writer() as git_config:
+                if not git_config.has_option("user", "name"):
+                    git_config.set_value("user", "name", "Your Name")
+                    io.tool_error('Update git name with: git config --global user.name "Your Name"')
+                if not git_config.has_option("user", "email"):
+                    git_config.set_value("user", "email", "you@example.com")
+                    io.tool_error(
+                        'Update git email with: git config --global user.email "you@example.com"'
+                    )
+            io.tool_output("Git repository created in the current working directory.")
+
     if args.verbose:
         show = parser.format_values()
         io.tool_output(show)
         io.tool_output("Option settings:")
         for arg, val in sorted(vars(args).items()):
             io.tool_output(f"  - {arg}: {val}")
 
@@ -266,15 +285,17 @@
 
     if not args.openai_api_key:
         if os.name == "nt":
             io.tool_error(
                 "No OpenAI API key provided. Use --openai-api-key or setx OPENAI_API_KEY."
             )
         else:
-            io.tool_error("No OpenAI API key provided. Use --openai-api-key or env OPENAI_API_KEY.")
+            io.tool_error(
+                "No OpenAI API key provided. Use --openai-api-key or export OPENAI_API_KEY."
+            )
         return 1
 
     main_model = models.Model(args.model)
 
     coder = Coder.create(
         main_model,
         args.edit_format,
```

### Comparing `aider-chat-0.8.0/aider/models.py` & `aider-chat-0.8.1/aider/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             self.edit_format = "diff"
             self.use_repo_map = True
             self.send_undo_reply = True
 
             if tokens == 8:
                 self.prompt_price = 0.03
                 self.completion_price = 0.06
+                self.always_available = True
             elif tokens == 32:
                 self.prompt_price = 0.06
                 self.completion_price = 0.12
 
             return
 
         if self.is_gpt35():
```

### Comparing `aider-chat-0.8.0/aider/prompts.py` & `aider-chat-0.8.1/aider/prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider/repomap.py` & `aider-chat-0.8.1/aider/repomap.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,21 @@
     else:
         res.append(path_components[-1])
     return res
 
 
 class RepoMap:
     CACHE_VERSION = 1
-    ctags_cmd = ["ctags", "--fields=+S", "--extras=-F", "--output-format=json"]
+    ctags_cmd = [
+        "ctags",
+        "--fields=+S",
+        "--extras=-F",
+        "--output-format=json",
+        "--output-encoding=utf-8",
+    ]
     IDENT_CACHE_DIR = f".aider.ident.cache.v{CACHE_VERSION}"
     TAGS_CACHE_DIR = f".aider.tags.cache.v{CACHE_VERSION}"
 
     ctags_disabled_reason = "ctags not initialized"
 
     def __init__(
         self,
@@ -167,19 +173,28 @@
     def run_ctags(self, filename):
         # Check if the file is in the cache and if the modification time has not changed
         file_mtime = os.path.getmtime(filename)
         cache_key = filename
         if cache_key in self.TAGS_CACHE and self.TAGS_CACHE[cache_key]["mtime"] == file_mtime:
             return self.TAGS_CACHE[cache_key]["data"]
 
-        cmd = self.ctags_cmd + [filename]
+        cmd = self.ctags_cmd + [
+            f"--input-encoding={self.io.encoding}",
+            filename,
+        ]
         output = subprocess.check_output(cmd, stderr=subprocess.PIPE).decode("utf-8")
-        output = output.splitlines()
+        output_lines = output.splitlines()
 
-        data = [json.loads(line) for line in output]
+        data = []
+        for line in output_lines:
+            try:
+                data.append(json.loads(line))
+            except json.decoder.JSONDecodeError as err:
+                self.io.tool_error(f"Error parsing ctags output: {err}")
+                self.io.tool_error(repr(line))
 
         # Update the cache
         self.TAGS_CACHE[cache_key] = {"mtime": file_mtime, "data": data}
         self.save_tags_cache()
         return data
 
     def check_for_ctags(self):
```

### Comparing `aider-chat-0.8.0/aider_chat.egg-info/PKG-INFO` & `aider-chat-0.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1
-Name: aider-chat
-Version: 0.8.0
-Summary: aider is GPT powered coding in your terminal
-Home-page: https://github.com/paul-gauthier/aider
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # aider is GPT powered coding in your terminal
 
 `aider` is a command-line chat tool that allows you to write and edit
 code with OpenAI's GPT models.  You can ask GPT to help you start
 a new project, or modify code in your existing git repo.
 Aider makes it easy to git commit, diff & undo changes proposed by GPT without copy/pasting. 
 It also has features that [help GPT-4 understand and modify larger codebases](https://aider.chat/docs/ctags.html).
 
+![aider screencast](assets/screencast.svg)
 
+- [Getting started](#getting-started)
+- [Example chat transcripts](#example-chat-transcripts)
+- [Features](#features)
+- [Installation](#installation)
+- [Usage](#usage)
+- [In-chat commands](#in-chat-commands)
+- [Tips](#tips)
+- [GPT-4 vs GPT-3.5](#gpt-4-vs-gpt-35)
+- [FAQ](https://aider.chat/docs/faq.html)
 
 ## Getting started
 
 ```
 $ pip install aider-chat
 $ export OPENAI_API_KEY=your-key-goes-here
 $ aider myapp.py
@@ -62,19 +64,17 @@
   * GitHub: `python -m pip install git+https://github.com/paul-gauthier/aider.git`
   * Local clone: `python -m pip install -e .` 
 
 2. Set up your OpenAI API key:
   * As an environment variable:
     * `export OPENAI_API_KEY=sk-...` on Linux or Mac
     * `setx OPENAI_API_KEY sk-...` in Windows PowerShell
-  * Or include `openai-api-key: sk-...` in an `.aider.config.yml` file in your current directory or at the root of your git repo, alongside the `.git` dir.
+  * Or include `openai-api-key: sk-...` in an `.aider.conf.yml` file in your home directory or at the root of your git repo, alongside the `.git` dir.
 
-3. Optionally, install [universal ctags](https://github.com/universal-ctags/ctags). This is helpful if you plan to use aider and GPT-4 with repositories that have more than a handful of files.  This allows aider to build a [map of your entire git repo](https://aider.chat/docs/ctags.html) and share it with GPT to help it better understand and modify large codebases.
-  * The `ctags` command needs to be on your shell path so that it will run by default when aider invokes `ctags ...`.
-  * You need a build which includes the json feature. You can check by running `ctags --version` and looking for `+json` in the `Optional compiled features` list.
+3. Optionally, install [universal ctags](https://github.com/universal-ctags/ctags). This is helpful if you plan to use aider and GPT-4 with repositories that have more than a handful of files.  This allows aider to build a [map of your entire git repo](https://aider.chat/docs/ctags.html) and share it with GPT to help it better understand and modify large codebases. See the [FAQ entry about ctags](https://aider.chat/docs/faq.html#how-do-i-get-ctags-working) for more info.
 
 ## Usage
 
 Run the `aider` tool by executing the following command:
 
 ```
 aider <file1> <file2> ...
```

### Comparing `aider-chat-0.8.0/aider_chat.egg-info/SOURCES.txt` & `aider-chat-0.8.1/aider_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/aider_chat.egg-info/requires.txt` & `aider-chat-0.8.1/aider_chat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/benchmark/benchmark.py` & `aider-chat-0.8.1/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/benchmark/rungrid.py` & `aider-chat-0.8.1/benchmark/rungrid.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/benchmark/test_benchmark.py` & `aider-chat-0.8.1/benchmark/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/requirements.txt` & `aider-chat-0.8.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/setup.py` & `aider-chat-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/tests/test_coder.py` & `aider-chat-0.8.1/tests/test_coder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import tempfile
 import unittest
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 import openai
 import requests
@@ -34,34 +33,70 @@
         mock_repo.git.ls_files.return_value = "file1.txt\nfile2.py"
         coder.repo = mock_repo
 
         # Call the check_for_file_mentions method
         coder.check_for_file_mentions("Please check file1.txt and file2.py")
 
         # Check if coder.abs_fnames contains both files
-        expected_files = {os.path.abspath("file1.txt"), os.path.abspath("file2.py")}
+        expected_files = set(
+            map(
+                str,
+                [
+                    Path(coder.root) / "file1.txt",
+                    Path(coder.root) / "file2.py",
+                ],
+            )
+        )
         self.assertEqual(coder.abs_fnames, expected_files)
 
+    def test_get_files_content(self):
+        tempdir = Path(tempfile.mkdtemp())
+
+        file1 = tempdir / "file1.txt"
+        file2 = tempdir / "file2.txt"
+
+        file1.touch()
+        file2.touch()
+
+        files = [file1, file2]
+
+        # Initialize the Coder object with the mocked IO and mocked repo
+        coder = Coder.create(
+            models.GPT4, None, io=InputOutput(), openai_api_key="fake_key", fnames=files
+        )
+
+        content = coder.get_files_content().splitlines()
+        self.assertIn("file1.txt", content)
+        self.assertIn("file2.txt", content)
+
     def test_check_for_filename_mentions_of_longer_paths(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
         coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
 
         # Mock the git repo
         mock_repo = MagicMock()
-        mock_repo.git.ls_files.return_value = "./file1.txt\n./file2.py"
+        mock_repo.git.ls_files.return_value = "file1.txt\nfile2.py"
         coder.repo = mock_repo
 
         # Call the check_for_file_mentions method
         coder.check_for_file_mentions("Please check file1.txt and file2.py")
 
         # Check if coder.abs_fnames contains both files
-        expected_files = {os.path.abspath("file1.txt"), os.path.abspath("file2.py")}
+        expected_files = set(
+            map(
+                str,
+                [
+                    Path(coder.root) / "file1.txt",
+                    Path(coder.root) / "file2.py",
+                ],
+            )
+        )
         self.assertEqual(coder.abs_fnames, expected_files)
 
     def test_check_for_ambiguous_filename_mentions_of_longer_paths(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
```

### Comparing `aider-chat-0.8.0/tests/test_editblock.py` & `aider-chat-0.8.1/tests/test_editblock.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/tests/test_io.py` & `aider-chat-0.8.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/tests/test_main.py` & `aider-chat-0.8.1/tests/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from unittest import TestCase
 from unittest.mock import patch
 
 from prompt_toolkit.input import DummyInput
 from prompt_toolkit.output import DummyOutput
 
+from aider.dump import dump  # noqa: F401
 from aider.main import main
 
 
 class TestMain(TestCase):
     def setUp(self):
         os.environ["OPENAI_API_KEY"] = "deadbeef"
         self.original_cwd = os.getcwd()
@@ -24,27 +25,44 @@
 
     def tearDown(self):
         os.chdir(self.original_cwd)
         shutil.rmtree(self.tempdir, ignore_errors=True)
         self.patcher.stop()
 
     def test_main_with_empty_dir_no_files_on_command(self):
-        main([], input=DummyInput(), output=DummyOutput())
+        main(["--no-git"], input=DummyInput(), output=DummyOutput())
 
     def test_main_with_empty_dir_new_file(self):
-        main(["foo.txt"], input=DummyInput(), output=DummyOutput())
+        main(["foo.txt", "--yes"], input=DummyInput(), output=DummyOutput())
         self.assertTrue(os.path.exists("foo.txt"))
 
     def test_main_with_empty_git_dir_new_file(self):
         subprocess.run(["git", "init"])
         subprocess.run(["git", "config", "user.email", "dummy@example.com"])
         subprocess.run(["git", "config", "user.name", "Dummy User"])
         main(["--yes", "foo.txt"], input=DummyInput(), output=DummyOutput())
         self.assertTrue(os.path.exists("foo.txt"))
 
+    def test_main_with_git_config_yml(self):
+        subprocess.run(["git", "init"])
+        subprocess.run(["git", "config", "user.email", "dummy@example.com"])
+        subprocess.run(["git", "config", "user.name", "Dummy User"])
+
+        Path(".aider.conf.yml").write_text("no-auto-commits: true\n")
+        with patch("aider.main.Coder.create") as MockCoder:
+            main([], input=DummyInput(), output=DummyOutput())
+            _, kwargs = MockCoder.call_args
+            assert kwargs["auto_commits"] is False
+
+        Path(".aider.conf.yml").write_text("auto-commits: true\n")
+        with patch("aider.main.Coder.create") as MockCoder:
+            main([], input=DummyInput(), output=DummyOutput())
+            _, kwargs = MockCoder.call_args
+            assert kwargs["auto_commits"] is True
+
     def test_main_with_empty_git_dir_new_subdir_file(self):
         subprocess.run(["git", "init"])
         subprocess.run(["git", "config", "user.email", "dummy@example.com"])
         subprocess.run(["git", "config", "user.name", "Dummy User"])
         subdir = Path("subdir")
         subdir.mkdir()
         fname = subdir / "foo.txt"
@@ -55,15 +73,17 @@
         # This will throw a git error on windows if get_tracked_files doesn't
         # properly convert git/posix/paths to git\posix\paths.
         # Because aider will try and `git add` a file that's already in the repo.
         main(["--yes", str(fname)], input=DummyInput(), output=DummyOutput())
 
     def test_main_args(self):
         with patch("aider.main.Coder.create") as MockCoder:
-            main(["--no-auto-commits"], input=DummyInput())
+            # --yes will just ok the git repo without blocking on input
+            # following calls to main will see the new repo already
+            main(["--no-auto-commits", "--yes"], input=DummyInput())
             _, kwargs = MockCoder.call_args
             assert kwargs["auto_commits"] is False
 
         with patch("aider.main.Coder.create") as MockCoder:
             main(["--auto-commits"], input=DummyInput())
             _, kwargs = MockCoder.call_args
             assert kwargs["auto_commits"] is True
```

### Comparing `aider-chat-0.8.0/tests/test_models.py` & `aider-chat-0.8.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/tests/test_repomap.py` & `aider-chat-0.8.1/tests/test_repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.8.0/tests/test_wholefile.py` & `aider-chat-0.8.1/tests/test_wholefile.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,39 @@
 
     def tearDown(self):
         os.chdir(self.original_cwd)
         shutil.rmtree(self.tempdir, ignore_errors=True)
 
         self.patcher.stop()
 
+    def test_no_files(self):
+        # Initialize WholeFileCoder with the temporary directory
+        io = InputOutput(yes=True)
+
+        coder = WholeFileCoder(main_model=models.GPT35, io=io, fnames=[])
+        coder.partial_response_content = (
+            'To print "Hello, World!" in most programming languages, you can use the following'
+            ' code:\n\n```python\nprint("Hello, World!")\n```\n\nThis code will output "Hello,'
+            ' World!" to the console.'
+        )
+
+        # This is throwing ValueError!
+        coder.render_incremental_response(True)
+
+    def test_no_files_new_file_should_ask(self):
+        io = InputOutput(yes=False)  # <- yes=FALSE
+        coder = WholeFileCoder(main_model=models.GPT35, io=io, fnames=[])
+        coder.partial_response_content = (
+            'To print "Hello, World!" in most programming languages, you can use the following'
+            ' code:\n\nfoo.js\n```python\nprint("Hello, World!")\n```\n\nThis code will output'
+            ' "Hello, World!" to the console.'
+        )
+        coder.update_files()
+        self.assertFalse(Path("foo.js").exists())
+
     def test_update_files(self):
         # Create a sample file in the temporary directory
         sample_file = "sample.txt"
         with open(sample_file, "w") as f:
             f.write("Original content\n")
 
         # Initialize WholeFileCoder with the temporary directory
```

