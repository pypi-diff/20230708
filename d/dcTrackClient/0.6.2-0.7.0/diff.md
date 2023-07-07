# Comparing `tmp/dctrackclient-0.6.2.tar.gz` & `tmp/dctrackclient-0.7.0.tar.gz`

## Comparing `dctrackclient-0.6.2.tar` & `dctrackclient-0.7.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    16849 2020-02-02 00:00:00.000000 dctrackclient-0.6.2/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.6.2/.gitignore
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    19970 2020-02-02 00:00:00.000000 dctrackclient-0.6.2/../README.md
--rw-r--r--   0        0        0    20592 2020-02-02 00:00:00.000000 dctrackclient-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    17052 2020-02-02 00:00:00.000000 dctrackclient-0.7.0/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.7.0/.gitignore
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    20524 2020-02-02 00:00:00.000000 dctrackclient-0.7.0/../README.md
+-rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 dctrackclient-0.7.0/PKG-INFO
```

### Comparing `dctrackclient-0.6.2/src/dcTrackClient/__init__.py` & `dctrackclient-0.7.0/src/dcTrackClient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,25 @@
     def __init__(self, baseUrl: str, username: str = '', password: str = '', apiToken: str = ''):
         """Provide either a username and password, or an API token to access the dcTrack database with Python."""
         self.__BASE_URL = baseUrl
         self.__USERNAME = username
         self.__PASSWORD = password
         self.__APITOKEN = apiToken
 
-    def __request(self, method: str, endpoint: str, body: dict = None):
-        if self.__USERNAME and self.__PASSWORD:
-            return requests.request(method,  self.__BASE_URL + '/' + endpoint, json=body, auth=(self.__USERNAME, self.__PASSWORD)).json()
-        elif self.__APITOKEN:
-            return requests.request(method, self.__BASE_URL + '/' + endpoint, json=body, headers={'Authorization': 'Token ' + self.__APITOKEN}).json()
+    def generateToken(self) -> str:
+        """Generate and return an API token."""
+        if self.__USERNAME and self.__PASSWORD and not self.__APITOKEN:
+            return requests.request('POST', self.__BASE_URL + '/api/v2/authentication/login', auth=(self.__USERNAME, self.__PASSWORD)).headers['Authorization'].split()[1]
         else:
-            raise Exception('Undefined username/password or token.')
+            raise Exception('Username/password undefined or token predefined.')
+
+    def __request(self, method: str, endpoint: str, body: dict = None):
+        if not self.__APITOKEN:
+            self.__APITOKEN = self.generateToken()
+        return requests.request(method, self.__BASE_URL + '/' + endpoint, json=body, headers={'Authorization': 'Bearer ' + self.__APITOKEN}).json()
 
     def getItem(self, id: int):
         """Get item details using the item ID."""
         return self.__request('GET', '/api/v2/dcimoperations/items/' + str(id) + '/?')
 
     def createItem(self, returnDetails: bool, payload: dict):
         """Create a new item. When returnDetails is set to true, the API call will return the full json payload. If set to false, the call returns only the "id" and "tiName"."""
```

### Comparing `dctrackclient-0.6.2/pyproject.toml` & `dctrackclient-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.6.2"
+version = "0.7.0"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.6.2/../README.md` & `dctrackclient-0.7.0/../README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==0.6.2
+pip install dcTrackClient==0.7.0
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@0.6.2
+npm i dctrackclient@0.7.0
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -33,14 +33,28 @@
 import { Client } from 'dctrackclient';
 // Using a username and password // 
 const api = new Client('https://dctrack.example.com/', { username: 'user', password: 'pass' });
 // Using an API token //
 const api = new Client('https://dctrack.example.com/', { apiToken: 'token' });
 ```
 
+## Obtain an API Token
+> Obtain an API token using the `Client.generateToken()` function provided. Re-authentication is not necessary, the API token will automatically be used in subsequent API calls. The function returns the token's value in case the user wants to store the token for the next initialization of the API.
+
+### Python
+```py
+token = api.generateToken()
+```
+
+### JavaScript
+Notice the `await` keyword before the function call. This is because the JavaScript library is asynchronous and returns a `Promise` to the return value. All the API calls in this library require that keyword.
+```js
+const token = await api.generateToken();
+```
+
 # Usage Example
 This section demonstrates item manipulation with the API client.
 
 ## Create an item
 > This example shows the minimum attributes required to create an item using the [`createItem`](#createitemreturndetails-payload) function. View the comprehensive list of item attributes in the [official documentation](https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm#APIGuide/REST_API_JSON_Objects_for_Managed_Items.htm). Make sure to capture the return value of this function to see the created item details, such as the unique numeric item ID, or to determine if an error occurred while creating an item.
 
 ### Python
@@ -51,15 +65,15 @@
     'cmbMake': 'item make',
     'cmbModel': 'item model'
 })
 print(response)
 ```
 
 ### JavaScript
-Notice the `await` keyword before the function call. This is because the JavaScript library is asynchronous and returns a `Promise` to the return value. All the API calls in this library require that keyword.
+See the JavaScript section on [obtaining an API token](#obtain-an-api-token) why the `await` keyword is required.
 ```js
 let response = await api.createItem(true/false, {
     'cmbLocation': 'item location',
     'tiName': 'item name',
     'cmbMake': 'item make',
     'cmbModel': 'item model'
 });
```

### Comparing `dctrackclient-0.6.2/PKG-INFO` & `dctrackclient-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.6.2
+Version: 0.7.0
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,20 +20,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==0.6.2
+pip install dcTrackClient==0.7.0
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@0.6.2
+npm i dctrackclient@0.7.0
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -49,14 +49,28 @@
 import { Client } from 'dctrackclient';
 // Using a username and password // 
 const api = new Client('https://dctrack.example.com/', { username: 'user', password: 'pass' });
 // Using an API token //
 const api = new Client('https://dctrack.example.com/', { apiToken: 'token' });
 ```
 
+## Obtain an API Token
+> Obtain an API token using the `Client.generateToken()` function provided. Re-authentication is not necessary, the API token will automatically be used in subsequent API calls. The function returns the token's value in case the user wants to store the token for the next initialization of the API.
+
+### Python
+```py
+token = api.generateToken()
+```
+
+### JavaScript
+Notice the `await` keyword before the function call. This is because the JavaScript library is asynchronous and returns a `Promise` to the return value. All the API calls in this library require that keyword.
+```js
+const token = await api.generateToken();
+```
+
 # Usage Example
 This section demonstrates item manipulation with the API client.
 
 ## Create an item
 > This example shows the minimum attributes required to create an item using the [`createItem`](#createitemreturndetails-payload) function. View the comprehensive list of item attributes in the [official documentation](https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm#APIGuide/REST_API_JSON_Objects_for_Managed_Items.htm). Make sure to capture the return value of this function to see the created item details, such as the unique numeric item ID, or to determine if an error occurred while creating an item.
 
 ### Python
@@ -67,15 +81,15 @@
     'cmbMake': 'item make',
     'cmbModel': 'item model'
 })
 print(response)
 ```
 
 ### JavaScript
-Notice the `await` keyword before the function call. This is because the JavaScript library is asynchronous and returns a `Promise` to the return value. All the API calls in this library require that keyword.
+See the JavaScript section on [obtaining an API token](#obtain-an-api-token) why the `await` keyword is required.
 ```js
 let response = await api.createItem(true/false, {
     'cmbLocation': 'item location',
     'tiName': 'item name',
     'cmbMake': 'item make',
     'cmbModel': 'item model'
 });
```

