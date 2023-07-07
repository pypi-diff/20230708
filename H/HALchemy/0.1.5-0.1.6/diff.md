# Comparing `tmp/HALchemy-0.1.5-py3-none-any.whl.zip` & `tmp/HALchemy-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5800 bytes, number of entries: 7
+Zip file size: 5482 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Jul-04 01:21 halchemy/__init__.py
--rw-rw-rw-  2.0 fat     6873 b- defN 23-Jul-04 02:22 halchemy/api.py
+-rw-rw-rw-  2.0 fat     6308 b- defN 23-Jul-06 16:47 halchemy/api.py
 -rw-rw-rw-  2.0 fat     2548 b- defN 23-Jul-01 18:46 halchemy/requests_helper.py
--rw-rw-rw-  2.0 fat     2339 b- defN 23-Jul-04 03:01 HALchemy-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 03:01 HALchemy-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-04 03:01 HALchemy-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      532 b- defN 23-Jul-04 03:01 HALchemy-0.1.5.dist-info/RECORD
-7 files, 12466 bytes uncompressed, 4858 bytes compressed:  61.0%
+-rw-rw-rw-  2.0 fat     1872 b- defN 23-Jul-07 22:03 HALchemy-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 22:03 HALchemy-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-07 22:03 HALchemy-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      532 b- defN 23-Jul-07 22:03 HALchemy-0.1.6.dist-info/RECORD
+7 files, 11434 bytes uncompressed, 4540 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: halchemy/api.py
 Comment: 
 
 Filename: halchemy/requests_helper.py
 Comment: 
 
-Filename: HALchemy-0.1.5.dist-info/METADATA
+Filename: HALchemy-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: HALchemy-0.1.5.dist-info/WHEEL
+Filename: HALchemy-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: HALchemy-0.1.5.dist-info/top_level.txt
+Filename: HALchemy-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: HALchemy-0.1.5.dist-info/RECORD
+Filename: HALchemy-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## halchemy/api.py

```diff
@@ -64,31 +64,46 @@
                 print(f'This link is templated.  You must supply a value for {ex}')
                 return ''
         
         query_string = urlencode(parameters)
             
         return f"{url}{'?' if parameters else ''}{query_string}"
 
-    def post_to_url(self, url, data):
-        if type(data) is not str:
-            data = json.dumps(data)
-        response = self._api.post(url, data=data)
+    def get(self, url='/'):
+        response = self._api.get(url)
+        if response.status_code == 404:
+            return None
         try:
             response.raise_for_status()
             return response.json()
         except:
-            if response.status_code == 422:
-                issue = response.json().get('_issues', {}).get('name', '')
-                if 'is not unique' in issue:
-                    new_data = json.loads(data)
-                    new_data['name'] += ' ~'
-                    return self._api.post(url, data=new_data)
-            message = f'{response.status_code} {response.reason}'
+            message = f'GET {url} - {response.status_code} {response.reason}'
             details = response.text
-            raise RuntimeError(f'POST {url} - {message}\n{details}\n\n{data}')
+            raise RuntimeError(f'{message}\n{details}')
+
+    def get_from_rel(self, resource, rel='self', parameters={}, template={}):        
+        url = self.url_from_rel(resource, rel, parameters, template)
+        return self.get(url)
+
+    def get_from_rel_with_lookup(self, resource, rel, lookup, parameters={}):        
+        url = resource['_links'][rel]['href']
+        if url[-1] != '/':
+            url += '/'
+        url += lookup
+        
+        query_string = urlencode(parameters)
+            
+        return self.get(f"{url}{'?' if parameters else ''}{query_string}")        
+
+    def post_to_url(self, url, data):
+        if type(data) is not str:
+            data = json.dumps(data)
+        response = self._api.post(url, data=data)
+        response.raise_for_status()
+        return response.json()
 
     def post_to_rel(self, resource, rel, data, parameters={}, template={}):
         url = self.url_from_rel(resource, rel, parameters, template)
         return self.post_to_url(url, data)
 
     def patch_resource(self, resource, data):
         if type(data) is not str:
@@ -103,15 +118,15 @@
             response.raise_for_status()
             return response.json()
         except:
             message = f'{response.status_code} {response.reason}'
             details = response.text
             raise RuntimeError(f'PATCH {url}\n{headers}\n{message}\n{details}\n\n{data}')
 
-    def put_to_resource(self, resource, data, rel='self'):
+    def put_to_rel(self, resource, rel, data):
         if type(data) is not str:
             data = json.dumps(data)
         url = self.url_from_rel(resource, rel)
         headers = {
             'If-Match': resource['_etag']
         }
         response = self._api.put(url, data=data, headers=headers)
@@ -120,40 +135,14 @@
             response.raise_for_status()
             return response.json()
         except:
             message = f'{response.status_code} {response.reason}'
             details = response.text
             raise RuntimeError(f'PUT {url}\n{headers}\n{message}\n{details}\n\n{data}')
 
-    def get(self, url='/'):
-        response = self._api.get(url)
-        if response.status_code == 404:
-            return None
-        try:
-            response.raise_for_status()
-            return response.json()
-        except:
-            message = f'GET {url} - {response.status_code} {response.reason}'
-            details = response.text
-            raise RuntimeError(f'{message}\n{details}')
-
-    def get_from_rel(self, resource, rel='self', parameters={}, template={}):        
-        url = self.url_from_rel(resource, rel, parameters, template)
-        return self.get(url)
-
-    def get_from_rel_with_lookup(self, resource, rel, lookup, parameters={}):        
-        url = resource['_links'][rel]['href']
-        if url[-1] != '/':
-            url = url + '/'
-        url += lookup
-        
-        query_string = urlencode(parameters)
-            
-        return self.get(f"{url}{'?' if parameters else ''}{query_string}")        
-
     def delete_collection(self, url):
         response = self._api.delete(url)
 
         try:
             response.raise_for_status()
         except:
             message = f'{response.status_code} {response.reason}'
```

## Comparing `HALchemy-0.1.5.dist-info/METADATA` & `HALchemy-0.1.6.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,62 @@
 Metadata-Version: 2.1
 Name: HALchemy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Toolkit for creating clients of HAL based Hypermedia APIs.
 Home-page: https://github.com/pointw-dev/HALchemy
 Author: Michael Ottoson
 Author-email: michael@pointw.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+Requires-Dist: requests
 
-# HALchemy
+# HALchemy for Python
+**HAL-based Hypermedia API clients for humans.**
+
+![](../../img/halchemy-full-word.png)
+
+![](../../img/python.png)
 
-HAL-based Hypermedia API clients for humans.
 
 > This project has lofty goals, and is in its very early stages.  Please use with caution and beware of breaking changes until at least v0.7.0
 
-## Methods
-* def **url_from_rel**(resource, rel, parameters={}, template={}):
-* def **post_to_url**(self, url, data):
-* def **post_to_rel**(self, resource, rel, data, parameters={}, template={}):
-* def **patch_resource**(self, resource, data):
-* def **put_to_resource**(self, resource, data, rel='self'):
-* def **get**(self, url='/'):
-* def **get_from_rel**(self, resource, rel='self', parameters={}, template={}):        
-* def **get_from_rel_with_lookup**(self, resource, rel, lookup, parameters={}):        
-* def **delete_collection**(self, url):
-* def **delete_resource**(self, resource):
 
 
+## Getting started
+
+```bash
+pip install halchemy
+```
 
-## Features
-
-* parameters and templates
-* additional lookup (implicit templates)
-* requests library remembers defaults
-  * base url (allowing .get('/path')
-  * auth (saving managing headers with each request - defaults to Basic root:password)
-* can use python dict for POST/PUT/PATCH data (automatically converts to JSON)
+In your code, instantiate an `Api` object with the base URL of your API
 
-* in post_to_url():
 ```python
-except:
-    if response.status_code == 422:
-        issue = response.json().get('_issues', {}).get('name', '')
-        if 'is not unique' in issue:
-            new_data = json.loads(data)
-            new_data['name'] += ' ~'
-            return self._api.post(url, data=new_data)
-    message = f'{response.status_code} {response.reason}'
-    details = response.text
-            raise RuntimeError(f'POST {url} - {message}\n{details}\n\n{data}')
+from halchemy import Api
+
+api = Api('http://example.org/api')
+
+root = api.get()                           # get the root resource
+people = api.get_from_rel(root, 'people')  # follow the people rel to get the list of people
 ```
 
-## Roadmap
+(more docs coming)
+
+## Methods
+
+* **get**(self, url='/')
+* **get_from_rel**(self, resource, rel='self', parameters={}, template={})
+* **get_from_rel_with_lookup**(self, resource, rel, lookup, parameters={})
+* **post_to_rel**(self, resource, rel, data, parameters={}, template={})
+* **patch_resource**(self, resource, data)
+* **put_to_rel**(self, resource, data, rel='self')
+* **delete_collection**(self, url)
+* **delete_resource**(self, resource)
+* **url_from_rel**(resource, rel, parameters={}, template={})
+* **post_to_url**(self, url, data)
 
-* chainable requests
-* HAL Forms
-* as many languages as we can get to
```

## Comparing `HALchemy-0.1.5.dist-info/RECORD` & `HALchemy-0.1.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 halchemy/__init__.py,sha256=uOY88fxo04Ofw2_FpvGJ6LziQpDTE2o6aWfNP5May5M,73
-halchemy/api.py,sha256=R_Cweh-s_1-3jGtn_J7zsDW2z9fUwvM1WB9okUcJRsY,6873
+halchemy/api.py,sha256=tYG6iNs2smqPmt-TKzlBbihMUXmWiMcl1OZ_yQ1ReBw,6308
 halchemy/requests_helper.py,sha256=7mV5ts4jN3viuvpTWoYogkap8v1HpYe0wIWxf9N0KMI,2548
-HALchemy-0.1.5.dist-info/METADATA,sha256=VVu73u5GXGo5CcuQwY3dtyocG9j9xXlWDPY1uvtM8hU,2339
-HALchemy-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-HALchemy-0.1.5.dist-info/top_level.txt,sha256=QDAX4T2q2TC09LWO_LgEyuEBr-lPTU86p48miwnpfzw,9
-HALchemy-0.1.5.dist-info/RECORD,,
+HALchemy-0.1.6.dist-info/METADATA,sha256=uYJ_A4j_4uX5xgLvdOiaAUk0cTpIAG1HtX0wilHkiWY,1872
+HALchemy-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+HALchemy-0.1.6.dist-info/top_level.txt,sha256=QDAX4T2q2TC09LWO_LgEyuEBr-lPTU86p48miwnpfzw,9
+HALchemy-0.1.6.dist-info/RECORD,,
```

