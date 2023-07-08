# Comparing `tmp/CallingGPT-0.0.0.7.tar.gz` & `tmp/CallingGPT-0.0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CallingGPT-0.0.0.7.tar", last modified: Wed Jun 21 11:09:46 2023, max compression
+gzip compressed data, was "CallingGPT-0.0.1.0.tar", last modified: Sat Jul  8 02:12:01 2023, max compression
```

## Comparing `CallingGPT-0.0.0.7.tar` & `CallingGPT-0.0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-21 11:09:46.089198 CallingGPT-0.0.0.7/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4492 2023-06-21 11:09:46.089198 CallingGPT-0.0.0.7/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4088 2023-06-21 11:09:10.000000 CallingGPT-0.0.0.7/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-21 11:09:46.089198 CallingGPT-0.0.0.7/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      785 2023-06-21 11:09:36.000000 CallingGPT-0.0.0.7/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-21 11:09:46.081198 CallingGPT-0.0.0.7/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-21 11:09:46.085198 CallingGPT-0.0.0.7/src/CallingGPT/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:05:39.000000 CallingGPT-0.0.0.7/src/CallingGPT/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-21 11:09:46.085198 CallingGPT-0.0.0.7/src/CallingGPT/cli/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1887 2023-06-20 11:59:49.000000 CallingGPT-0.0.0.7/src/CallingGPT/cli/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-21 11:09:46.089198 CallingGPT-0.0.0.7/src/CallingGPT/entities/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.7/src/CallingGPT/entities/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6805 2023-06-21 11:09:10.000000 CallingGPT-0.0.0.7/src/CallingGPT/entities/namespace.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-21 11:09:46.089198 CallingGPT-0.0.0.7/src/CallingGPT/session/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.7/src/CallingGPT/session/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1913 2023-06-20 12:29:42.000000 CallingGPT-0.0.0.7/src/CallingGPT/session/session.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-21 11:09:46.085198 CallingGPT-0.0.0.7/src/CallingGPT.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4492 2023-06-21 11:09:46.000000 CallingGPT-0.0.0.7/src/CallingGPT.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      407 2023-06-21 11:09:46.000000 CallingGPT-0.0.0.7/src/CallingGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-21 11:09:46.000000 CallingGPT-0.0.0.7/src/CallingGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-21 11:09:46.000000 CallingGPT-0.0.0.7/src/CallingGPT.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2023-06-21 11:09:46.000000 CallingGPT-0.0.0.7/src/CallingGPT.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-08 02:12:01.665213 CallingGPT-0.0.1.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5309 2023-07-08 02:12:01.665213 CallingGPT-0.0.1.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4905 2023-07-08 02:11:07.000000 CallingGPT-0.0.1.0/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-08 02:12:01.665213 CallingGPT-0.0.1.0/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      756 2023-07-08 02:11:07.000000 CallingGPT-0.0.1.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-08 02:12:01.661213 CallingGPT-0.0.1.0/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-08 02:12:01.661213 CallingGPT-0.0.1.0/src/CallingGPT/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:05:39.000000 CallingGPT-0.0.1.0/src/CallingGPT/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-08 02:12:01.665213 CallingGPT-0.0.1.0/src/CallingGPT/cli/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2414 2023-07-08 02:11:07.000000 CallingGPT-0.0.1.0/src/CallingGPT/cli/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-08 02:12:01.665213 CallingGPT-0.0.1.0/src/CallingGPT/entities/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.1.0/src/CallingGPT/entities/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6963 2023-06-21 11:10:23.000000 CallingGPT-0.0.1.0/src/CallingGPT/entities/namespace.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-08 02:12:01.665213 CallingGPT-0.0.1.0/src/CallingGPT/session/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.1.0/src/CallingGPT/session/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1935 2023-07-08 02:11:07.000000 CallingGPT-0.0.1.0/src/CallingGPT/session/session.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-08 02:12:01.665213 CallingGPT-0.0.1.0/src/CallingGPT.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5309 2023-07-08 02:12:01.000000 CallingGPT-0.0.1.0/src/CallingGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      407 2023-07-08 02:12:01.000000 CallingGPT-0.0.1.0/src/CallingGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-08 02:12:01.000000 CallingGPT-0.0.1.0/src/CallingGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-07-08 02:12:01.000000 CallingGPT-0.0.1.0/src/CallingGPT.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2023-07-08 02:12:01.000000 CallingGPT-0.0.1.0/src/CallingGPT.egg-info/top_level.txt
```

### Comparing `CallingGPT-0.0.0.7/PKG-INFO` & `CallingGPT-0.0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: CallingGPT
-Version: 0.0.0.7
-Summary: GPT's function calling feature wrapper
-Home-page: https://github.com/RockChinQ/CallingGPT
-Author: RockChinQ
-Author-email: 1010553892@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # CallingGPT
 
 [![PyPi](https://img.shields.io/pypi/v/CallingGPT.svg)](https://pypi.python.org/pypi/CallingGPT)
 
 GPT's Function Calling Demo, a experiment of self-hosted ChatGPT-Plugins-like platform.
 
 > Recommend reading: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
@@ -55,49 +43,58 @@
 ```
 
 Then you can talk to the bot.
 
 ```
 $ python main.py examples/greet.py 
 Using module: examples.greet
->>> hello and who are you?              
-<<< Hello! I am an AI assistant here to help you. How may I assist you today?
+>>> Hello and who are you?
+<<< Hello! I am an AI assistant. How can I assist you today?
 >>> say hello to Rock
-func<examples.greet.greet>: Hello, Rock!
+call<examples-greet-greet>: {
+  "user": "Rock"
+}
+<<< Hello, Rock! How can I assist you today?
 >>> and to Alice
-func<examples.greet.greet>: Hello, Alice!
->>> 
+call<examples-greet-greet>: {
+  "user": "Alice"
+}
+<<< Hello, Alice! How can I assist you today?
+>>>
 ```
 
-Type `help` to get help.
+Type `help` to get help.  
+See [wiki](https://github.com/RockChinQ/CallingGPT/wiki/1.-Function-Format) for the function format.
 
 ### Other Examples
 
 <details>
-<summary>examples/draw.py</summary>
+<summary>examples/draw_and_wrapper_md.py </summary>
 
 Provides a `dalle_draw` function to use DALL·E model when user ask GPT to draw something.
 
 ```bash
-python main.py examples/draw.py
+python main.py examples/draw_and_wrapper_md.py 
 ```
 
 ```
-$ python main.py examples/draw.py 
-Using module: examples.draw
->>> draw cars heading home under the sunset
-func<examples.draw.dalle_draw>: {
-  "created": 1687098971,
-  "data": [
-    {
-      "url": "https://oaidalleapiprodscus.blob.core.windows.net/private/org-VS9HEpJba78GXVfOcmVo7qaM/user-OHa7Jo3kL4XJDg9lo7AzdWNT/img-eAwt4YgHn6ed1cr96MoRWs0d.png?st=2023-06-18T13%3A36%3A11Z&se=2023-06-18T15%3A36%3A11Z&sp=r&sv=2021-08-06&sr=b&rscd=inline&rsct=image/png&skoid=6aaadede-4fb3-4698-a8f6-684d7786b067&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2023-06-17T20%3A54%3A10Z&ske=2023-06-18T20%3A54%3A10Z&sks=b&skv=2021-08-06&sig=ZY4DTE1fYPyT7/jYBLJLuAgxpNuPsOhjbid1CWTyfKo%3D"
-    }
-  ]
+$ python main.py examples/draw_and_wrapper_md.py 
+Using module: examples.draw_and_wrapper_md
+>>> hello!
+<<< Hi there! How can I assist you today?
+>>> draw a sunset for me please
+call<examples-draw_and_wrapper_md-draw>: {
+  "prompt": "sunset"
 }
->>>
+<<< Sure! Here's a beautiful sunset for you:
+
+![Sunset](https://oaidalleapiprodscus.blob.core.windows.net/private/org-VS9HEpJba78GXVfOcmVo7qaM/user-OHa7Jo3kL4XJDg9lo7AzdWNT/img-QmDUiwp1IGFcu8pDGZh0i7r8.png)
+
+I hope you like it! Let me know if there's anything else I can help you with.
+>>> 
 ```
 
 </details>
 
 ## For Code
 
 1. Install the package
@@ -150,11 +147,31 @@
     import your_module_a, your_module_b
     import openai
 
     openai.api_key = 'your_openai_api_key'
 
     session = Session([your_module_a, your_module_b])
 
-    session.ask("your prompt")
+    for reply in session.ask("your prompt"):
+        # session.ask will yield each time the api returns a result,
+        # before calling function, it will print the function name and args.
+        # e.g. here's a function call:
+        # {
+        #   "role": "assistant",
+        #   "content": null,
+        #   "function_call": {
+        #     "name": "examples-draw_and_wrapper_md-draw",
+        #     "arguments": "{\n  \"prompt\": \"cat\"\n}"
+        #   }
+        # }
+        # 
+        # while here's a normal reply:
+        # {
+        #   "role": "assistant",
+        #   "content": "Hello, I am an AI assistant. How can I assist you today?"
+        # }
+        print(reply)
     ```
 
     `Session` will automatically manage context for you.
+  
+See [wiki](https://github.com/RockChinQ/CallingGPT/wiki/1.-Function-Format) for the function format.
```

### Comparing `CallingGPT-0.0.0.7/README.md` & `CallingGPT-0.0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: CallingGPT
+Version: 0.0.1.0
+Summary: GPT's function calling feature wrapper
+Home-page: https://github.com/RockChinQ/CallingGPT
+Author: RockChinQ
+Author-email: 1010553892@qq.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # CallingGPT
 
 [![PyPi](https://img.shields.io/pypi/v/CallingGPT.svg)](https://pypi.python.org/pypi/CallingGPT)
 
 GPT's Function Calling Demo, a experiment of self-hosted ChatGPT-Plugins-like platform.
 
 > Recommend reading: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
@@ -43,49 +55,58 @@
 ```
 
 Then you can talk to the bot.
 
 ```
 $ python main.py examples/greet.py 
 Using module: examples.greet
->>> hello and who are you?              
-<<< Hello! I am an AI assistant here to help you. How may I assist you today?
+>>> Hello and who are you?
+<<< Hello! I am an AI assistant. How can I assist you today?
 >>> say hello to Rock
-func<examples.greet.greet>: Hello, Rock!
+call<examples-greet-greet>: {
+  "user": "Rock"
+}
+<<< Hello, Rock! How can I assist you today?
 >>> and to Alice
-func<examples.greet.greet>: Hello, Alice!
->>> 
+call<examples-greet-greet>: {
+  "user": "Alice"
+}
+<<< Hello, Alice! How can I assist you today?
+>>>
 ```
 
-Type `help` to get help.
+Type `help` to get help.  
+See [wiki](https://github.com/RockChinQ/CallingGPT/wiki/1.-Function-Format) for the function format.
 
 ### Other Examples
 
 <details>
-<summary>examples/draw.py</summary>
+<summary>examples/draw_and_wrapper_md.py </summary>
 
 Provides a `dalle_draw` function to use DALL·E model when user ask GPT to draw something.
 
 ```bash
-python main.py examples/draw.py
+python main.py examples/draw_and_wrapper_md.py 
 ```
 
 ```
-$ python main.py examples/draw.py 
-Using module: examples.draw
->>> draw cars heading home under the sunset
-func<examples.draw.dalle_draw>: {
-  "created": 1687098971,
-  "data": [
-    {
-      "url": "https://oaidalleapiprodscus.blob.core.windows.net/private/org-VS9HEpJba78GXVfOcmVo7qaM/user-OHa7Jo3kL4XJDg9lo7AzdWNT/img-eAwt4YgHn6ed1cr96MoRWs0d.png?st=2023-06-18T13%3A36%3A11Z&se=2023-06-18T15%3A36%3A11Z&sp=r&sv=2021-08-06&sr=b&rscd=inline&rsct=image/png&skoid=6aaadede-4fb3-4698-a8f6-684d7786b067&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2023-06-17T20%3A54%3A10Z&ske=2023-06-18T20%3A54%3A10Z&sks=b&skv=2021-08-06&sig=ZY4DTE1fYPyT7/jYBLJLuAgxpNuPsOhjbid1CWTyfKo%3D"
-    }
-  ]
+$ python main.py examples/draw_and_wrapper_md.py 
+Using module: examples.draw_and_wrapper_md
+>>> hello!
+<<< Hi there! How can I assist you today?
+>>> draw a sunset for me please
+call<examples-draw_and_wrapper_md-draw>: {
+  "prompt": "sunset"
 }
->>>
+<<< Sure! Here's a beautiful sunset for you:
+
+![Sunset](https://oaidalleapiprodscus.blob.core.windows.net/private/org-VS9HEpJba78GXVfOcmVo7qaM/user-OHa7Jo3kL4XJDg9lo7AzdWNT/img-QmDUiwp1IGFcu8pDGZh0i7r8.png)
+
+I hope you like it! Let me know if there's anything else I can help you with.
+>>> 
 ```
 
 </details>
 
 ## For Code
 
 1. Install the package
@@ -138,11 +159,31 @@
     import your_module_a, your_module_b
     import openai
 
     openai.api_key = 'your_openai_api_key'
 
     session = Session([your_module_a, your_module_b])
 
-    session.ask("your prompt")
+    for reply in session.ask("your prompt"):
+        # session.ask will yield each time the api returns a result,
+        # before calling function, it will print the function name and args.
+        # e.g. here's a function call:
+        # {
+        #   "role": "assistant",
+        #   "content": null,
+        #   "function_call": {
+        #     "name": "examples-draw_and_wrapper_md-draw",
+        #     "arguments": "{\n  \"prompt\": \"cat\"\n}"
+        #   }
+        # }
+        # 
+        # while here's a normal reply:
+        # {
+        #   "role": "assistant",
+        #   "content": "Hello, I am an AI assistant. How can I assist you today?"
+        # }
+        print(reply)
     ```
 
     `Session` will automatically manage context for you.
+  
+See [wiki](https://github.com/RockChinQ/CallingGPT/wiki/1.-Function-Format) for the function format.
```

### Comparing `CallingGPT-0.0.0.7/src/CallingGPT/cli/__init__.py` & `CallingGPT-0.0.1.0/src/CallingGPT/cli/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,22 +37,37 @@
             except Exception as e:
                 logging.error("Failed to import module {}.".format(module_name))
                 logging.error(e)
             session.namespace.add_modules(modules)
         else:
             resp = session.ask(cmd)
 
-            if resp['type'] == 'function_call':
-                print(
-                    "func<{}>: {}".format(
-                        resp['func'],
-                        resp['value']
+            for repl in resp:
+                if 'function_call' in repl:
+                    print(
+                        "call<{}>: {}".format(
+                            repl['function_call']['name'],
+                            repl['function_call']['arguments']
+                        )
                     )
-                )
-            elif resp['type'] == 'message':
-                print(
-                    "<<< {}".format(
-                        resp['value']
+                else:
+                    print(
+                        "<<< {}".format(
+                            repl['content']
+                        )
                     )
-                )
+
+            # if resp['type'] == 'function_call':
+            #     print(
+            #         "func<{}>: {}".format(
+            #             resp['func'],
+            #             resp['value']
+            #         )
+            #     )
+            # elif resp['type'] == 'message':
+            #     print(
+            #         "<<< {}".format(
+            #             resp['value']
+            #         )
+            #     )
 
         cmd = input(">>> ")
```

### Comparing `CallingGPT-0.0.0.7/src/CallingGPT/entities/namespace.py` & `CallingGPT-0.0.1.0/src/CallingGPT/entities/namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,17 +153,20 @@
 
     def _retrieve_functions(self):
         self.functions = {}
         for module in self.modules:
             # assert module is a module
             assert isinstance(module, type(sys))
             # ignore non-function attributes
-            functions = {k: v for k, v in module.__dict__.items() if callable(v)}
-            # ignore private functions
-            functions = {k: v for k, v in functions.items() if not k.startswith('_')}
+            if not hasattr(module, '__functions__'):
+                functions = {k: v for k, v in module.__dict__.items() if callable(v)}
+                # ignore private functions
+                functions = {k: v for k, v in functions.items() if not k.startswith('_')}
+            else:
+                functions = {v.__name__: v for v in module.__functions__ }
 
             self.functions[module.__name__.replace(".","-")] = {}
 
             for name, function in functions.items():
                 funtion_dict = get_func_schema(function)
 
                 self.functions[module.__name__.replace(".","-")][name] = funtion_dict
```

### Comparing `CallingGPT-0.0.0.7/src/CallingGPT/session/session.py` & `CallingGPT-0.0.1.0/src/CallingGPT/session/session.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,65 +13,65 @@
     model: str = "gpt-3.5-turbo-0613"
 
     def __init__(self, modules: list, model: str = "gpt-3.5-turbo-0613"):
         self.namespace = Namespace(modules)
         self.model = model
 
     def ask(self, msg: str) -> dict:
-        self.messages.append(
+        # copy messages
+
+        messages = self.messages.copy()
+
+        messages.append(
             {
                 "role": "user",
                 "content": msg
             }
         )
+        while True:
 
-        args = {
-            "model": self.model,
-            "messages": self.messages,
-        }
-
-        if len(self.namespace.functions_list) > 0:
-            args['functions'] = self.namespace.functions_list
-            args['function_call'] = "auto"
+            args = {
+                "model": self.model,
+                "messages": messages,
+            }
 
-        resp = openai.ChatCompletion.create(
-            **args
-        )
+            if len(self.namespace.functions_list) > 0:
+                args['functions'] = self.namespace.functions_list
+                args['function_call'] = "auto"
 
-        logging.debug("Response: {}".format(resp))
-        reply_msg = resp["choices"][0]['message']
+            resp = openai.ChatCompletion.create(
+                **args
+            )
 
-        ret = {}
+            logging.debug("Response: {}".format(resp))
+            reply_msg = resp["choices"][0]['message']
 
-        if 'function_call' in reply_msg:
+            yield reply_msg
 
-            fc = reply_msg['function_call']
-            args = json.loads(fc['arguments'])
-            call_ret = self._call_function(fc['name'], args)
-
-            self.messages.append({
-                "role": "function",
-                "name": fc['name'],
-                "content": str(call_ret)
-            })
-
-            ret = {
-                "type": "function_call",
-                "func": fc['name'].replace('-', '.'),
-                "value": call_ret,
-            }
-        else:
-            ret = {
-                "type": "message",
-                "value": reply_msg['content'],
-            }
+            ret = {}
+
+            if 'function_call' in reply_msg:
+
+                fc = reply_msg['function_call']
+                args = json.loads(fc['arguments'])
+                call_ret = self._call_function(fc['name'], args)
+
+                messages.append({
+                    "role": "function",
+                    "name": fc['name'],
+                    "content": str(call_ret)
+                })
+
+                self.messages = messages.copy()
+            else:
+                messages.append({
+                    "role": "assistant",
+                    "content": reply_msg['content']
+                })
 
-            self.messages.append({
-                "role": "assistant",
-                "content": reply_msg['content']
-            })
+                self.messages = messages.copy()
 
-        return ret
+                break
 
     def _call_function(self, function_name: str, args: dict):
         return self.namespace.call_function(function_name, args)
```

### Comparing `CallingGPT-0.0.0.7/src/CallingGPT.egg-info/PKG-INFO` & `CallingGPT-0.0.1.0/src/CallingGPT.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CallingGPT
-Version: 0.0.0.7
+Version: 0.0.1.0
 Summary: GPT's function calling feature wrapper
 Home-page: https://github.com/RockChinQ/CallingGPT
 Author: RockChinQ
 Author-email: 1010553892@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -55,49 +55,58 @@
 ```
 
 Then you can talk to the bot.
 
 ```
 $ python main.py examples/greet.py 
 Using module: examples.greet
->>> hello and who are you?              
-<<< Hello! I am an AI assistant here to help you. How may I assist you today?
+>>> Hello and who are you?
+<<< Hello! I am an AI assistant. How can I assist you today?
 >>> say hello to Rock
-func<examples.greet.greet>: Hello, Rock!
+call<examples-greet-greet>: {
+  "user": "Rock"
+}
+<<< Hello, Rock! How can I assist you today?
 >>> and to Alice
-func<examples.greet.greet>: Hello, Alice!
->>> 
+call<examples-greet-greet>: {
+  "user": "Alice"
+}
+<<< Hello, Alice! How can I assist you today?
+>>>
 ```
 
-Type `help` to get help.
+Type `help` to get help.  
+See [wiki](https://github.com/RockChinQ/CallingGPT/wiki/1.-Function-Format) for the function format.
 
 ### Other Examples
 
 <details>
-<summary>examples/draw.py</summary>
+<summary>examples/draw_and_wrapper_md.py </summary>
 
 Provides a `dalle_draw` function to use DALL·E model when user ask GPT to draw something.
 
 ```bash
-python main.py examples/draw.py
+python main.py examples/draw_and_wrapper_md.py 
 ```
 
 ```
-$ python main.py examples/draw.py 
-Using module: examples.draw
->>> draw cars heading home under the sunset
-func<examples.draw.dalle_draw>: {
-  "created": 1687098971,
-  "data": [
-    {
-      "url": "https://oaidalleapiprodscus.blob.core.windows.net/private/org-VS9HEpJba78GXVfOcmVo7qaM/user-OHa7Jo3kL4XJDg9lo7AzdWNT/img-eAwt4YgHn6ed1cr96MoRWs0d.png?st=2023-06-18T13%3A36%3A11Z&se=2023-06-18T15%3A36%3A11Z&sp=r&sv=2021-08-06&sr=b&rscd=inline&rsct=image/png&skoid=6aaadede-4fb3-4698-a8f6-684d7786b067&sktid=a48cca56-e6da-484e-a814-9c849652bcb3&skt=2023-06-17T20%3A54%3A10Z&ske=2023-06-18T20%3A54%3A10Z&sks=b&skv=2021-08-06&sig=ZY4DTE1fYPyT7/jYBLJLuAgxpNuPsOhjbid1CWTyfKo%3D"
-    }
-  ]
+$ python main.py examples/draw_and_wrapper_md.py 
+Using module: examples.draw_and_wrapper_md
+>>> hello!
+<<< Hi there! How can I assist you today?
+>>> draw a sunset for me please
+call<examples-draw_and_wrapper_md-draw>: {
+  "prompt": "sunset"
 }
->>>
+<<< Sure! Here's a beautiful sunset for you:
+
+![Sunset](https://oaidalleapiprodscus.blob.core.windows.net/private/org-VS9HEpJba78GXVfOcmVo7qaM/user-OHa7Jo3kL4XJDg9lo7AzdWNT/img-QmDUiwp1IGFcu8pDGZh0i7r8.png)
+
+I hope you like it! Let me know if there's anything else I can help you with.
+>>> 
 ```
 
 </details>
 
 ## For Code
 
 1. Install the package
@@ -150,11 +159,31 @@
     import your_module_a, your_module_b
     import openai
 
     openai.api_key = 'your_openai_api_key'
 
     session = Session([your_module_a, your_module_b])
 
-    session.ask("your prompt")
+    for reply in session.ask("your prompt"):
+        # session.ask will yield each time the api returns a result,
+        # before calling function, it will print the function name and args.
+        # e.g. here's a function call:
+        # {
+        #   "role": "assistant",
+        #   "content": null,
+        #   "function_call": {
+        #     "name": "examples-draw_and_wrapper_md-draw",
+        #     "arguments": "{\n  \"prompt\": \"cat\"\n}"
+        #   }
+        # }
+        # 
+        # while here's a normal reply:
+        # {
+        #   "role": "assistant",
+        #   "content": "Hello, I am an AI assistant. How can I assist you today?"
+        # }
+        print(reply)
     ```
 
     `Session` will automatically manage context for you.
+  
+See [wiki](https://github.com/RockChinQ/CallingGPT/wiki/1.-Function-Format) for the function format.
```

