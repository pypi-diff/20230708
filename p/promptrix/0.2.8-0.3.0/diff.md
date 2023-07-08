# Comparing `tmp/promptrix-0.2.8.tar.gz` & `tmp/promptrix-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptrix-0.2.8.tar", last modified: Fri Jul  7 20:18:37 2023, max compression
+gzip compressed data, was "promptrix-0.3.0.tar", last modified: Sat Jul  8 01:26:00 2023, max compression
```

## Comparing `promptrix-0.2.8.tar` & `promptrix-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-07 20:18:37.047666 promptrix-0.2.8/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.8/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-07-07 20:18:37.043666 promptrix-0.2.8/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1607 2023-06-15 20:10:06.000000 promptrix-0.2.8/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      833 2023-07-07 20:18:29.000000 promptrix-0.2.8/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-07 20:18:37.047666 promptrix-0.2.8/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-07 20:18:37.043666 promptrix-0.2.8/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-07 20:18:37.043666 promptrix-0.2.8/src/promptrix/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      759 2023-06-27 16:18:19.000000 promptrix-0.2.8/src/promptrix/AssistantMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2576 2023-06-27 16:18:52.000000 promptrix-0.2.8/src/promptrix/ConversationHistory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.8/src/promptrix/FunctionRegistry.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      607 2023-06-14 17:33:19.000000 promptrix-0.2.8/src/promptrix/GPT3Tokenizer.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1187 2023-06-15 17:06:46.000000 promptrix-0.2.8/src/promptrix/GroupSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-15 17:06:10.000000 promptrix-0.2.8/src/promptrix/LayoutEngine.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.8/src/promptrix/Prompt.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2507 2023-07-07 19:01:24.000000 promptrix-0.2.8/src/promptrix/PromptSectionBase.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.8/src/promptrix/SystemMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5879 2023-07-07 18:58:41.000000 promptrix-0.2.8/src/promptrix/TemplateSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.8/src/promptrix/TextSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.2.8/src/promptrix/UserMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-07-07 18:57:37.000000 promptrix-0.2.8/src/promptrix/Utilities.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-19 22:47:47.000000 promptrix-0.2.8/src/promptrix/VolatileMemory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.8/src/promptrix/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.8/src/promptrix/promptrixTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-07 20:18:37.043666 promptrix-0.2.8/src/promptrix.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-07-07 20:18:37.000000 promptrix-0.2.8/src/promptrix.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-07-07 20:18:37.000000 promptrix-0.2.8/src/promptrix.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-07 20:18:37.000000 promptrix-0.2.8/src/promptrix.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-07-07 20:18:37.000000 promptrix-0.2.8/src/promptrix.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-07-07 20:18:37.000000 promptrix-0.2.8/src/promptrix.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:26:00.392543 promptrix-0.3.0/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.3.0/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-07-08 01:26:00.392543 promptrix-0.3.0/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1607 2023-06-15 20:10:06.000000 promptrix-0.3.0/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      833 2023-07-08 01:25:51.000000 promptrix-0.3.0/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-08 01:26:00.392543 promptrix-0.3.0/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:26:00.392543 promptrix-0.3.0/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:26:00.392543 promptrix-0.3.0/src/promptrix/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      759 2023-06-27 16:18:19.000000 promptrix-0.3.0/src/promptrix/AssistantMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2576 2023-06-27 16:18:52.000000 promptrix-0.3.0/src/promptrix/ConversationHistory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.3.0/src/promptrix/FunctionRegistry.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      607 2023-06-14 17:33:19.000000 promptrix-0.3.0/src/promptrix/GPT3Tokenizer.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1187 2023-06-15 17:06:46.000000 promptrix-0.3.0/src/promptrix/GroupSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-15 17:06:10.000000 promptrix-0.3.0/src/promptrix/LayoutEngine.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.3.0/src/promptrix/Prompt.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2507 2023-07-07 19:01:24.000000 promptrix-0.3.0/src/promptrix/PromptSectionBase.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.3.0/src/promptrix/SystemMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5879 2023-07-07 18:58:41.000000 promptrix-0.3.0/src/promptrix/TemplateSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.3.0/src/promptrix/TextSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.3.0/src/promptrix/UserMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-07-07 18:57:37.000000 promptrix-0.3.0/src/promptrix/Utilities.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-19 22:47:47.000000 promptrix-0.3.0/src/promptrix/VolatileMemory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.3.0/src/promptrix/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.3.0/src/promptrix/promptrixTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:26:00.392543 promptrix-0.3.0/src/promptrix.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-07-08 01:26:00.000000 promptrix-0.3.0/src/promptrix.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-07-08 01:26:00.000000 promptrix-0.3.0/src/promptrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-08 01:26:00.000000 promptrix-0.3.0/src/promptrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-07-08 01:26:00.000000 promptrix-0.3.0/src/promptrix.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-07-08 01:26:00.000000 promptrix-0.3.0/src/promptrix.egg-info/top_level.txt
```

### Comparing `promptrix-0.2.8/LICENSE` & `promptrix-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/PKG-INFO` & `promptrix-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.8
+Version: 0.3.0
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/promptrix
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.2.8/README.md` & `promptrix-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/pyproject.toml` & `promptrix-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptrix"
-version = "0.2.8"
+version = "0.3.0"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "Promptrix. A prompt layout manager for LLMs"
 #documentation = "https://github.com/Stevenic/promptrix-py/README.md"
```

### Comparing `promptrix-0.2.8/src/promptrix/AssistantMessage.py` & `promptrix-0.3.0/src/promptrix/AssistantMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/ConversationHistory.py` & `promptrix-0.3.0/src/promptrix/ConversationHistory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/FunctionRegistry.py` & `promptrix-0.3.0/src/promptrix/FunctionRegistry.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/GPT3Tokenizer.py` & `promptrix-0.3.0/src/promptrix/GPT3Tokenizer.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/GroupSection.py` & `promptrix-0.3.0/src/promptrix/GroupSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/LayoutEngine.py` & `promptrix-0.3.0/src/promptrix/LayoutEngine.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/PromptSectionBase.py` & `promptrix-0.3.0/src/promptrix/PromptSectionBase.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/TemplateSection.py` & `promptrix-0.3.0/src/promptrix/TemplateSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/TextSection.py` & `promptrix-0.3.0/src/promptrix/TextSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/UserMessage.py` & `promptrix-0.3.0/src/promptrix/UserMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/Utilities.py` & `promptrix-0.3.0/src/promptrix/Utilities.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/VolatileMemory.py` & `promptrix-0.3.0/src/promptrix/VolatileMemory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix/promptrixTypes.py` & `promptrix-0.3.0/src/promptrix/promptrixTypes.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.8/src/promptrix.egg-info/PKG-INFO` & `promptrix-0.3.0/src/promptrix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.8
+Version: 0.3.0
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/promptrix
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.2.8/src/promptrix.egg-info/SOURCES.txt` & `promptrix-0.3.0/src/promptrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

