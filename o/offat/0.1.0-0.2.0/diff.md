# Comparing `tmp/offat-0.1.0.tar.gz` & `tmp/offat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offat-0.1.0.tar", max compression
+gzip compressed data, was "offat-0.2.0.tar", max compression
```

## Comparing `offat-0.1.0.tar` & `offat-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1071 2023-07-02 18:52:35.065253 offat-0.1.0/LICENSE
--rw-r--r--   0        0        0     5061 2023-07-02 18:44:57.627346 offat-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-27 13:39:00.229447 offat-0.1.0/offat/__init__.py
--rw-r--r--   0        0        0     1126 2023-07-02 18:44:57.627621 offat-0.1.0/offat/__main__.py
--rw-r--r--   0        0        0     4528 2023-07-02 12:32:18.660759 offat-0.1.0/offat/http.py
--rw-r--r--   0        0        0     1121 2023-07-02 11:53:54.132005 offat-0.1.0/offat/logger.py
--rw-r--r--   0        0        0     1017 2023-07-02 18:44:57.627927 offat-0.1.0/offat/openapi.py
--rw-r--r--   0        0        0        0 2023-07-02 11:56:53.216486 offat-0.1.0/offat/tester/__init__.py
--rw-r--r--   0        0        0     1273 2023-07-02 18:44:57.628224 offat-0.1.0/offat/tester/test_generator.py
--rw-r--r--   0        0        0      919 2023-07-02 18:44:57.628400 offat-0.1.0/offat/tester/test_results.py
--rw-r--r--   0        0        0     2082 2023-07-02 18:44:57.628594 offat-0.1.0/offat/tester/test_runner.py
--rw-r--r--   0        0        0     1775 2023-07-02 10:46:07.892803 offat-0.1.0/offat/utils.py
--rw-r--r--   0        0        0      879 2023-07-02 18:44:57.629669 offat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 offat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-08 13:53:24.791561 offat-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5063 2023-07-08 13:53:24.791561 offat-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-08 13:53:24.791561 offat-0.2.0/offat/__init__.py
+-rw-r--r--   0        0        0     1366 2023-07-08 13:53:24.791561 offat-0.2.0/offat/__main__.py
+-rw-r--r--   0        0        0     4276 2023-07-08 13:53:24.791561 offat-0.2.0/offat/http.py
+-rw-r--r--   0        0        0     1121 2023-07-08 13:53:24.791561 offat-0.2.0/offat/logger.py
+-rw-r--r--   0        0        0     3767 2023-07-08 13:53:24.791561 offat-0.2.0/offat/openapi.py
+-rw-r--r--   0        0        0        0 2023-07-08 13:53:24.791561 offat-0.2.0/offat/tester/__init__.py
+-rw-r--r--   0        0        0      262 2023-07-08 13:53:24.791561 offat-0.2.0/offat/tester/fuzzer.py
+-rw-r--r--   0        0        0     8427 2023-07-08 13:53:24.791561 offat-0.2.0/offat/tester/test_generator.py
+-rw-r--r--   0        0        0     1230 2023-07-08 13:53:24.791561 offat-0.2.0/offat/tester/test_results.py
+-rw-r--r--   0        0        0     2609 2023-07-08 13:53:24.791561 offat-0.2.0/offat/tester/test_runner.py
+-rw-r--r--   0        0        0     1775 2023-07-08 13:53:24.791561 offat-0.2.0/offat/utils.py
+-rw-r--r--   0        0        0      873 2023-07-08 13:53:24.791561 offat-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6031 1970-01-01 00:00:00.000000 offat-0.2.0/PKG-INFO
```

### Comparing `offat-0.1.0/LICENSE` & `offat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offat-0.1.0/README.md` & `offat-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # OFFAT - OFFensive Api Tester
 
-Automatically Tests for vulnerabilities after generating tests openapi specification file.
+Automatically Tests for vulnerabilities after generating tests from openapi specification file.
 
 ![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-test-undocumented-api-endpoint-http-method.png)
 
 ## PyPi Downloads
 
 |Period|Count|
 |:----:|:---:|
@@ -65,15 +65,15 @@
 - install with poetry
 
   ```bash
   # without options
   poetry install
   ```
 
-## Start PyHTools
+## Start OffAT
 
 - run offat
 
   ```bash
   python3 -m offat
   ```
```

### Comparing `offat-0.1.0/offat/__main__.py` & `offat-0.2.0/offat/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,24 +12,30 @@
     parser = ArgumentParser(prog='offat')
     parser.add_argument('-f','--file', dest='fpath', type=str, help='path of openapi/swagger specification file', required=True)
     
     args = parser.parse_args()
 
     api_parser = OpenAPIParser(args.fpath)
 
-    # create test objs
+    # create tester objs
     test_runner = TestRunner()
     test_table_generator = TestResultTable()
+    test_generator = TestGenerator()
 
+    
     # test for unsupported http methods
-    test_generator = TestGenerator()
-    unsupported_http_endpoint_tests = test_generator.check_unsupported_http_methods(api_parser.base_url, api_parser._get_endpoints())
+    # unsupported_http_endpoint_tests = test_generator.check_unsupported_http_methods(api_parser.base_url, api_parser._get_endpoints())
+    # test_results = run(test_runner.run_tests(unsupported_http_endpoint_tests))
+    # results = test_table_generator.generate_result_table(test_results)
+    # print(results)
 
-    # run tests
-    test_results = run(test_runner.run_tests(unsupported_http_endpoint_tests))
 
-    # generate results
+    # sqli fuzz test
+    sqli_fuzz_tests = test_generator.sqli_fuzz_params(api_parser)
+    test_results = run(test_runner.run_tests(sqli_fuzz_tests))
     results = test_table_generator.generate_result_table(test_results)
     print(results)
 
+    # generate results
+
 if __name__ == '__main__':
     start()
```

### Comparing `offat-0.1.0/offat/http.py` & `offat-0.2.0/offat/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,17 +112,7 @@
         Returns:
             dict: returns request and response data as dict
         '''
         async with self._semaphore:
             response = await super().request(url, method, session, *args, **kwargs)
             await asyncio.sleep(self._delay)
             return response
-
-
-# async def test():
-#     req = AsyncRLRequests(delay=4)
-#     res = await asyncio.gather(asyncio.ensure_future(await req.request('https://httpbin.org/get', method='GET')))
-
-#     print(res[-1])
-
-# if __name__ == '__main__':
-#     asyncio.run(test())
```

### Comparing `offat-0.1.0/offat/logger.py` & `offat-0.2.0/offat/logger.py`

 * *Files identical despite different names*

### Comparing `offat-0.1.0/offat/tester/test_results.py` & `offat-0.2.0/offat/tester/test_results.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,30 @@
 class TestResultTable:
     def __init__(self, tablefmt:str='heavy_outline', headers:str='keys',*args, **kwargs) -> None:
         self.tablefmt = tablefmt
         self.headers = headers
         self.args = args
         self.kwargs = kwargs
 
-    def generate_result_table(self, results:list):
-        return tabulate(self._sanitize_results(results), headers=self.headers, tablefmt=self.tablefmt, *self.args, **self.kwargs)
+    def generate_result_table(self, results:list, filter_passed_results:bool=True):
+        return tabulate(self._sanitize_results(results, filter_passed_results), headers=self.headers, tablefmt=self.tablefmt, *self.args, **self.kwargs)
     
     def _sanitize_results(self, results:list, filter_passed_results:bool=True):
-        # remove args, kwargs and url keys
+        if filter_passed_results:
+            results = list(filter(lambda x: not x.get('result'), results))
+
+        # remove args, kwargs and other unrequired keys for results
         for result in results:
+            if result['result']:
+                result['result'] = u"\u2713"
+            else:
+                result['result'] = u"\u00d7"
+
             del result['url']
             del result['args']
             del result['kwargs']
             del result['test_name']
             del result['response_filter']
-
-        if filter_passed_results:
-            results = filter(lambda x: not x.get('result'), results)
-
+            del result['success_codes']
+            del result['body_params']
+            
         return results
-
```

### Comparing `offat-0.1.0/offat/tester/test_runner.py` & `offat-0.2.0/offat/tester/test_runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,35 +14,53 @@
 class TestRunner:
     def __init__(self, rate_limit:int=None, delay:float=None, headers:dict=None) -> None:
         if rate_limit and delay:
             self._client = AsyncRLRequests(rate_limit=rate_limit, delay=delay, headers=headers)
         else:
             self._client = AsyncRequests(headers=headers)
 
+    def _generate_body_payload(self, body_params:list[dict]):
+        '''Generate body payload from passed data'''
+        json_payload = {}
+        for param in body_params:
+            param_in = param.get('in')
+            param_name = param.get('name')
+            param_value = param.get('value')
+
+
+            match param_in:
+                case 'body':
+                    json_payload[param_name] = param_value
+                case _:
+                    continue
+
+        return json_payload
 
     async def status_code_filter_request(self, test_task):
         url = test_task.get('url')
         http_method = test_task.get('method')
         success_codes = test_task.get('success_codes', [200, 301])
         args = test_task.get('args')
         kwargs = test_task.get('kwargs')
+        body_params = test_task.get('body_params')
 
+        if body_params:
+            kwargs['json'] = self._generate_body_payload(body_params)
         try:
             response = await self._client.request(url=url, method=http_method, *args, **kwargs)
         except ConnectionRefusedError:
             logger.error('Connection Failed! Server refused Connection!!')
 
         test_result = test_task
         if isinstance(response, dict) and response.get('status') in success_codes:
-            test_result['result'] = False # test failed
-            test_result['result_detail'] = 'Endpoint performs HTTP method which is not documented'
+            result = False # test failed
         else:
-            test_result['result'] = True # test passed
-            test_result['result_detail'] = 'Endpoint does not perform any HTTP method which is not documented'
-
+            result = True # test passed
+        test_result['result'] = result
+        test_result['result_details'] = test_result['result_details'].get(result)
 
         return test_result
 
 
     async def run_tests(self, test_tasks:list):
         '''run tests generated from test generator module'''
         tasks = []
```

### Comparing `offat-0.1.0/offat/utils.py` & `offat-0.2.0/offat/utils.py`

 * *Files identical despite different names*

### Comparing `offat-0.1.0/pyproject.toml` & `offat-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "offat"
-version = "0.1.0"
+version = "0.2.0"
 description = "Offensive API tester tool automates checks for common API vulnerabilities"
 authors = ["Dhrumil Mistry <56185972+dmdhrumilmistry@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -17,19 +17,19 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 
 
 [tool.poetry.urls]
 "Home" = "https://github.com/dmdhrumilmistry/offat"
-"Bug Tracker" = "https://github.com/dmdhrumilmistry/pyhtools/issues"
+"Bug Tracker" = "https://github.com/dmdhrumilmistry/offat/issues"
 "Support" = "https://github.com/sponsors/dmdhrumilmistry/"
 "PayPal" = "https://paypal.me/dmdhrumilmistry"
 
 
 [tool.poetry.scripts]
-pyhtools = "offat.__main__:start"
+offat = "offat.__main__:start"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `offat-0.1.0/PKG-INFO` & `offat-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: offat
-Version: 0.1.0
+Version: 0.2.0
 Summary: Offensive API tester tool automates checks for common API vulnerabilities
 License: MIT
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: openapi-spec-validator (>=0.5.7,<0.6.0)
 Requires-Dist: prance (>=23.6.21.0,<24.0.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Project-URL: Bug Tracker, https://github.com/dmdhrumilmistry/pyhtools/issues
+Project-URL: Bug Tracker, https://github.com/dmdhrumilmistry/offat/issues
 Project-URL: Home, https://github.com/dmdhrumilmistry/offat
 Project-URL: PayPal, https://paypal.me/dmdhrumilmistry
 Project-URL: Support, https://github.com/sponsors/dmdhrumilmistry/
 Description-Content-Type: text/markdown
 
 # OFFAT - OFFensive Api Tester
 
-Automatically Tests for vulnerabilities after generating tests openapi specification file.
+Automatically Tests for vulnerabilities after generating tests from openapi specification file.
 
 ![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-test-undocumented-api-endpoint-http-method.png)
 
 ## PyPi Downloads
 
 |Period|Count|
 |:----:|:---:|
@@ -88,15 +88,15 @@
 - install with poetry
 
   ```bash
   # without options
   poetry install
   ```
 
-## Start PyHTools
+## Start OffAT
 
 - run offat
 
   ```bash
   python3 -m offat
   ```
```

