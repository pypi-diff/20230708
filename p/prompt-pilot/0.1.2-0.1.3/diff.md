# Comparing `tmp/prompt_pilot-0.1.2.tar.gz` & `tmp/prompt_pilot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_pilot-0.1.2.tar", max compression
+gzip compressed data, was "prompt_pilot-0.1.3.tar", max compression
```

## Comparing `prompt_pilot-0.1.2.tar` & `prompt_pilot-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1578 2023-07-08 07:43:18.536140 prompt_pilot-0.1.2/README.md
--rwxr-xr-x   0        0        0      209 2023-07-07 18:33:52.688086 prompt_pilot-0.1.2/prompt_pilot/__init__.py
--rwxr-xr-x   0        0        0     4744 2023-07-07 20:08:33.415961 prompt_pilot-0.1.2/prompt_pilot/api_ai.py
--rwxr-xr-x   0        0        0      532 2023-07-08 07:38:19.348176 prompt_pilot-0.1.2/prompt_pilot/api_data.py
--rwxr-xr-x   0        0        0    18102 2023-07-08 07:36:13.087761 prompt_pilot-0.1.2/prompt_pilot/assistants.py
--rwxr-xr-x   0        0        0     4033 2023-07-08 07:32:37.247094 prompt_pilot-0.1.2/prompt_pilot/characters.py
--rwxr-xr-x   0        0        0        4 2023-07-07 20:08:32.196697 prompt_pilot-0.1.2/prompt_pilot/data_science.py
--rwxr-xr-x   0        0        0    13934 2023-07-08 07:37:43.498089 prompt_pilot-0.1.2/prompt_pilot/image_generation.py
--rwxr-xr-x   0        0        0      336 2023-07-08 04:44:14.738643 prompt_pilot-0.1.2/prompt_pilot/img_to_img.py
--rwxr-xr-x   0        0        0      355 2023-07-08 04:44:18.398896 prompt_pilot-0.1.2/prompt_pilot/inpainting.py
--rwxr-xr-x   0        0        0      520 2023-07-08 07:44:04.417129 prompt_pilot-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 prompt_pilot-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1643 2023-07-08 08:54:54.490780 prompt_pilot-0.1.3/README.md
+-rwxr-xr-x   0        0        0      209 2023-07-07 18:33:52.688086 prompt_pilot-0.1.3/prompt_pilot/__init__.py
+-rwxr-xr-x   0        0        0     4744 2023-07-08 08:49:53.313829 prompt_pilot-0.1.3/prompt_pilot/api_ai.py
+-rwxr-xr-x   0        0        0      532 2023-07-08 07:38:19.348176 prompt_pilot-0.1.3/prompt_pilot/api_data.py
+-rwxr-xr-x   0        0        0    18102 2023-07-08 08:54:03.830313 prompt_pilot-0.1.3/prompt_pilot/assistants.py
+-rwxr-xr-x   0        0        0     4033 2023-07-08 08:53:04.616038 prompt_pilot-0.1.3/prompt_pilot/characters.py
+-rwxr-xr-x   0        0        0     1206 2023-07-08 08:55:38.581405 prompt_pilot-0.1.3/prompt_pilot/data_science.py
+-rwxr-xr-x   0        0        0    13934 2023-07-08 08:21:58.165604 prompt_pilot-0.1.3/prompt_pilot/image_generation.py
+-rwxr-xr-x   0        0        0      336 2023-07-08 04:44:14.738643 prompt_pilot-0.1.3/prompt_pilot/img_to_img.py
+-rwxr-xr-x   0        0        0      355 2023-07-08 04:44:18.398896 prompt_pilot-0.1.3/prompt_pilot/inpainting.py
+-rwxr-xr-x   0        0        0      520 2023-07-08 08:56:03.022062 prompt_pilot-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 prompt_pilot-0.1.3/PKG-INFO
```

### Comparing `prompt_pilot-0.1.2/README.md` & `prompt_pilot-0.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,28 +3,34 @@
 *DISCLAIMER: This is a work in progress, and I'm sharing it as a temporary solution with some functions that you can experiment with.*
 
 Prompt Pilot is a library designed for prompt engineering in AI models. It introduces the concept of "prompt functions" to streamline the prompt creation process. With just one function, developers can create complex prompts effortlessly.
 
 Here's an example implementation for creating a digital marketing chatbot:
 
 ```
-# import the required functions from prompt_pilot
-from prompt_pilot.assistants import digital_marketing_analyst 
-from prompt_pilot.api_ai import stablelm
+# import the required functions from prompt_pilot.
+from prompt_pilot.assistants import life_coach
+from prompt_pilot.api_ai import gpt3
+#import config function from decouple to read api_key
+import decouple 
 
-# configure your apikey
-api_key = config("REPLICATE_API_TOKEN") 
 # use promptpilot to generate prompt
-prompt = digital_marketing_analyst() 
-# use promptpilot's api call functions to pass prompt and apikey. Here, we are using the StableLM model
-output = stablelm(prompt, api_key)
+prompt = life_coach(name="Rocky")
+print(prompt)
+
+# configure your apikey
+openai_api_key = decouple.config("OPENAI_API_KEY")
 
-print(output)
+# use promptpilot's api call functions to pass prompt and apikey
+output = gpt3(prompt=prompt, api_key=openai_api_key)
+print(output
 ```
 
+
+
 By automating both prompt engineering and API calls to AI models, Prompt Pilot significantly reduces the code required to build a chatbot. With just 5-6 lines of code, you can have a fully functional chatbot up and running in very little time.
 
 Here's what you can build with prompt-pilot:
 
-- Chatbots and other NLP tasks : Personalized chatbots for business usecase, personal usecase, and academic usecase. API calls to OpenAI and LLMs on Replicate
-- Image models : Varying styles for image generators. API calls to image models on Replicate
-- Data science : Automating data-science by incorporating LLMs (OpenAI) into the process to perform analysis
+- **Chatbots and other NLP tasks :** Personalized chatbots for business usecase, personal usecase, and academic usecase. API calls to OpenAI and LLMs on Replicate
+- **Image models :** Varying styles for image generators. API calls to image models on Replicate
+- **Data science :** Automating data-science by incorporating LLMs (OpenAI) into the process to perform analysis
```

### Comparing `prompt_pilot-0.1.2/prompt_pilot/api_ai.py` & `prompt_pilot-0.1.3/prompt_pilot/api_ai.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.1.2/prompt_pilot/api_data.py` & `prompt_pilot-0.1.3/prompt_pilot/api_data.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.1.2/prompt_pilot/assistants.py` & `prompt_pilot-0.1.3/prompt_pilot/assistants.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.1.2/prompt_pilot/characters.py` & `prompt_pilot-0.1.3/prompt_pilot/characters.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.1.2/prompt_pilot/image_generation.py` & `prompt_pilot-0.1.3/prompt_pilot/image_generation.py`

 * *Files identical despite different names*

### Comparing `prompt_pilot-0.1.2/pyproject.toml` & `prompt_pilot-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prompt-pilot"
-version = "0.1.2"
+version = "0.1.3"
 description = "Library for prompt engineering"
 authors = ["Amar <amar439412@gmail.com>"]
 readme = "README.md"
 packages = [{include = "prompt_pilot"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `prompt_pilot-0.1.2/PKG-INFO` & `prompt_pilot-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-pilot
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library for prompt engineering
 Author: Amar
 Author-email: amar439412@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,29 +21,35 @@
 *DISCLAIMER: This is a work in progress, and I'm sharing it as a temporary solution with some functions that you can experiment with.*
 
 Prompt Pilot is a library designed for prompt engineering in AI models. It introduces the concept of "prompt functions" to streamline the prompt creation process. With just one function, developers can create complex prompts effortlessly.
 
 Here's an example implementation for creating a digital marketing chatbot:
 
 ```
-# import the required functions from prompt_pilot
-from prompt_pilot.assistants import digital_marketing_analyst 
-from prompt_pilot.api_ai import stablelm
+# import the required functions from prompt_pilot.
+from prompt_pilot.assistants import life_coach
+from prompt_pilot.api_ai import gpt3
+#import config function from decouple to read api_key
+import decouple 
 
-# configure your apikey
-api_key = config("REPLICATE_API_TOKEN") 
 # use promptpilot to generate prompt
-prompt = digital_marketing_analyst() 
-# use promptpilot's api call functions to pass prompt and apikey. Here, we are using the StableLM model
-output = stablelm(prompt, api_key)
+prompt = life_coach(name="Rocky")
+print(prompt)
+
+# configure your apikey
+openai_api_key = decouple.config("OPENAI_API_KEY")
 
-print(output)
+# use promptpilot's api call functions to pass prompt and apikey
+output = gpt3(prompt=prompt, api_key=openai_api_key)
+print(output
 ```
 
+
+
 By automating both prompt engineering and API calls to AI models, Prompt Pilot significantly reduces the code required to build a chatbot. With just 5-6 lines of code, you can have a fully functional chatbot up and running in very little time.
 
 Here's what you can build with prompt-pilot:
 
-- Chatbots and other NLP tasks : Personalized chatbots for business usecase, personal usecase, and academic usecase. API calls to OpenAI and LLMs on Replicate
-- Image models : Varying styles for image generators. API calls to image models on Replicate
-- Data science : Automating data-science by incorporating LLMs (OpenAI) into the process to perform analysis
+- **Chatbots and other NLP tasks :** Personalized chatbots for business usecase, personal usecase, and academic usecase. API calls to OpenAI and LLMs on Replicate
+- **Image models :** Varying styles for image generators. API calls to image models on Replicate
+- **Data science :** Automating data-science by incorporating LLMs (OpenAI) into the process to perform analysis
```

