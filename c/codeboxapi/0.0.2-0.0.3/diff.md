# Comparing `tmp/codeboxapi-0.0.2.tar.gz` & `tmp/codeboxapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeboxapi-0.0.2.tar", max compression
+gzip compressed data, was "codeboxapi-0.0.3.tar", max compression
```

## Comparing `codeboxapi-0.0.2.tar` & `codeboxapi-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-07-06 14:15:22.624340 codeboxapi-0.0.2/LICENSE
--rw-r--r--   0        0        0      971 2023-07-08 10:14:31.926381 codeboxapi-0.0.2/README.md
--rw-r--r--   0        0        0      453 2023-07-08 10:18:47.139651 codeboxapi-0.0.2/codeboxapi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 20:22:44.654362 codeboxapi-0.0.2/codeboxapi/chromebox.todo
--rw-r--r--   0        0        0     2719 2023-07-08 09:58:01.107350 codeboxapi-0.0.2/codeboxapi/codebox.py
--rw-r--r--   0        0        0      373 2023-07-08 09:58:38.756932 codeboxapi-0.0.2/codeboxapi/config.py
--rw-r--r--   0        0        0     1822 2023-07-06 15:43:19.461194 codeboxapi-0.0.2/codeboxapi/errors.py
--rw-r--r--   0        0        0        0 2023-07-06 20:21:56.443613 codeboxapi-0.0.2/codeboxapi/repobox.todo
--rw-r--r--   0        0        0      401 2023-07-04 21:36:12.057702 codeboxapi-0.0.2/codeboxapi/schema.py
--rw-r--r--   0        0        0      801 2023-07-08 10:18:34.557809 codeboxapi-0.0.2/codeboxapi/utils.py
--rw-r--r--   0        0        0        0 2023-07-06 20:21:44.232581 codeboxapi-0.0.2/codeboxapi/vectorbox.todo
--rw-r--r--   0        0        0      498 2023-07-08 10:20:54.482470 codeboxapi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1700 2023-07-08 10:21:01.938900 codeboxapi-0.0.2/setup.py
--rw-r--r--   0        0        0     1532 2023-07-08 10:21:01.939111 codeboxapi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-06 14:15:22.624340 codeboxapi-0.0.3/LICENSE
+-rw-r--r--   0        0        0      990 2023-07-08 10:23:43.952201 codeboxapi-0.0.3/README.md
+-rw-r--r--   0        0        0      453 2023-07-08 10:18:47.139651 codeboxapi-0.0.3/codeboxapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 20:22:44.654362 codeboxapi-0.0.3/codeboxapi/chromebox.todo
+-rw-r--r--   0        0        0     2942 2023-07-08 12:29:47.418125 codeboxapi-0.0.3/codeboxapi/codebox.py
+-rw-r--r--   0        0        0      373 2023-07-08 09:58:38.756932 codeboxapi-0.0.3/codeboxapi/config.py
+-rw-r--r--   0        0        0     1822 2023-07-06 15:43:19.461194 codeboxapi-0.0.3/codeboxapi/errors.py
+-rw-r--r--   0        0        0        0 2023-07-06 20:21:56.443613 codeboxapi-0.0.3/codeboxapi/repobox.todo
+-rw-r--r--   0        0        0      401 2023-07-04 21:36:12.057702 codeboxapi-0.0.3/codeboxapi/schema.py
+-rw-r--r--   0        0        0      913 2023-07-08 12:34:43.495991 codeboxapi-0.0.3/codeboxapi/utils.py
+-rw-r--r--   0        0        0        0 2023-07-06 20:21:44.232581 codeboxapi-0.0.3/codeboxapi/vectorbox.todo
+-rw-r--r--   0        0        0      498 2023-07-08 12:40:57.341467 codeboxapi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1721 2023-07-08 12:41:02.674332 codeboxapi-0.0.3/setup.py
+-rw-r--r--   0        0        0     1551 2023-07-08 12:41:02.674492 codeboxapi-0.0.3/PKG-INFO
```

### Comparing `codeboxapi-0.0.2/LICENSE` & `codeboxapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.2/README.md` & `codeboxapi-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```bash
 pip install codeboxapi
 ```
 
 ## Usage
 
 ```python
-import codebox as cb
+import codeboxapi as cb
 
 cb.set_api_key("your-api-key")
 # or put your api key inside the .env file
 # CODEBOX_API_KEY=your-api-key
 
 # create and startup
 codebox = CodeBox()
@@ -29,14 +29,16 @@
 print(codebox.status() == "running")
 
 # run some code
 result = codebox.run("print('Hello, World!')")
 
 # print the result
 print(result)
+
+codebox.stop()
 ```
 
 ## Contributing
 
 Feel free to contribute to this project.
 You can open an issue or submit a pull request.
```

### Comparing `codeboxapi-0.0.2/codeboxapi/codebox.py` & `codeboxapi-0.0.3/codeboxapi/codebox.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,33 +57,39 @@
             )
         )
         
     def upload_file(self, name: str, content: bytes) -> dict:
         return self.codebox_request(
             method="POST",
             endpoint="/upload",
-            files={
-                "file": (name, content),
-            },
+            files={"file": (name, content)},
             content_type=None
         )
     
     # def upload_files(self, files: dict[str, bytes]) -> dict:
     #     return self.codebox_request(
     #         method="POST",
     #         endpoint="/upload",
     #         files=files,
     #     )
     
     def download_file(self, file_name: str) -> dict:
         return self.codebox_request(
             method="GET",
             endpoint="/download",
+            body={"file_name": file_name},
+            content_type=None,
+        )
+        
+    def install_package(self, package_name: str) -> dict:
+        return self.codebox_request(
+            method="POST",
+            endpoint="/install",
             body={
-                "file_name": file_name,
+                "package_name": package_name,
             },
         )
     
     def get_available_files(self) -> list[str]:
         return self.codebox_request(
             method="GET",
             endpoint="/files",
```

### Comparing `codeboxapi-0.0.2/codeboxapi/errors.py` & `codeboxapi-0.0.3/codeboxapi/errors.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.2/codeboxapi/utils.py` & `codeboxapi-0.0.3/codeboxapi/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,17 @@
             "Authorization": f"Bearer {settings.CODEBOX_API_KEY}",
         },
         json=body,
         files=files,
     )
     content = response.content.decode()
     if response.status_code == 200:
-        return json.loads(content)
+        if response.headers['Content-Type'] == 'application/json':
+            return json.loads(content)
+        else:
+            return content
     else:
         raise Exception(f"Error: {response.status_code} {content}")
 
 
 def set_api_key(api_key: str) -> None:
     settings.CODEBOX_API_KEY = api_key
```

### Comparing `codeboxapi-0.0.2/setup.py` & `codeboxapi-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['python-dotenv>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'codeboxapi',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'CodeBox is the simplest cloud infrastructure for your LLM Apps and Services.',
-    'long_description': '# CodeBox\n\nCodeBox is the simplest cloud infrastructure for your LLM Apps and Services.\nIt allows you to run python code in an isolated/sandboxed environment.\nAdditionally, it provides simple fileIO (and vector database support coming soon).\n\n## Installation\n\nYou can install CodeBox with pip:\n\n```bash\npip install codeboxapi\n```\n\n## Usage\n\n```python\nimport codebox as cb\n\ncb.set_api_key("your-api-key")\n# or put your api key inside the .env file\n# CODEBOX_API_KEY=your-api-key\n\n# create and startup\ncodebox = CodeBox()\ncodebox.start()\n\n# check if it\'s running\nprint(codebox.status() == "running")\n\n# run some code\nresult = codebox.run("print(\'Hello, World!\')")\n\n# print the result\nprint(result)\n```\n\n## Contributing\n\nFeel free to contribute to this project.\nYou can open an issue or submit a pull request.\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n\n## Contact\n\nYou can contact me at [pleurae-berets.0u@icloud.com](mailto:pleurae-berets.0u@icloud.com)\n',
+    'long_description': '# CodeBox\n\nCodeBox is the simplest cloud infrastructure for your LLM Apps and Services.\nIt allows you to run python code in an isolated/sandboxed environment.\nAdditionally, it provides simple fileIO (and vector database support coming soon).\n\n## Installation\n\nYou can install CodeBox with pip:\n\n```bash\npip install codeboxapi\n```\n\n## Usage\n\n```python\nimport codeboxapi as cb\n\ncb.set_api_key("your-api-key")\n# or put your api key inside the .env file\n# CODEBOX_API_KEY=your-api-key\n\n# create and startup\ncodebox = CodeBox()\ncodebox.start()\n\n# check if it\'s running\nprint(codebox.status() == "running")\n\n# run some code\nresult = codebox.run("print(\'Hello, World!\')")\n\n# print the result\nprint(result)\n\ncodebox.stop()\n```\n\n## Contributing\n\nFeel free to contribute to this project.\nYou can open an issue or submit a pull request.\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n\n## Contact\n\nYou can contact me at [pleurae-berets.0u@icloud.com](mailto:pleurae-berets.0u@icloud.com)\n',
     'author': 'Shroominic',
     'author_email': 'pleurae-berets.0u@icloud.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `codeboxapi-0.0.2/PKG-INFO` & `codeboxapi-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeboxapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: CodeBox is the simplest cloud infrastructure for your LLM Apps and Services.
 License: MIT
 Author: Shroominic
 Author-email: pleurae-berets.0u@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 ```bash
 pip install codeboxapi
 ```
 
 ## Usage
 
 ```python
-import codebox as cb
+import codeboxapi as cb
 
 cb.set_api_key("your-api-key")
 # or put your api key inside the .env file
 # CODEBOX_API_KEY=your-api-key
 
 # create and startup
 codebox = CodeBox()
@@ -45,14 +45,16 @@
 print(codebox.status() == "running")
 
 # run some code
 result = codebox.run("print('Hello, World!')")
 
 # print the result
 print(result)
+
+codebox.stop()
 ```
 
 ## Contributing
 
 Feel free to contribute to this project.
 You can open an issue or submit a pull request.
```

