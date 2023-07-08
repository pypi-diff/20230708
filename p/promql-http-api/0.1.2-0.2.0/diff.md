# Comparing `tmp/promql_http_api-0.1.2.tar.gz` & `tmp/promql_http_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promql_http_api-0.1.2.tar", max compression
+gzip compressed data, was "promql_http_api-0.2.0.tar", max compression
```

## Comparing `promql_http_api-0.1.2.tar` & `promql_http_api-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    10764 2023-01-27 09:07:19.549411 promql_http_api-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     5399 2023-03-31 07:16:58.738739 promql_http_api-0.1.2/README.md
--rw-r--r--   0        0        0      746 2023-01-27 09:07:19.565408 promql_http_api-0.1.2/promql_http_api/__init__.py
--rw-r--r--   0        0        0     1049 2023-01-27 09:07:19.816418 promql_http_api-0.1.2/promql_http_api/alerts.py
--rw-r--r--   0        0        0     1070 2023-01-27 09:07:19.833422 promql_http_api-0.1.2/promql_http_api/alertsmanagers.py
--rw-r--r--   0        0        0     3388 2023-01-27 09:07:19.810420 promql_http_api-0.1.2/promql_http_api/api.py
--rw-r--r--   0        0        0     1724 2023-01-27 09:07:19.827419 promql_http_api-0.1.2/promql_http_api/api_endpoint.py
--rw-r--r--   0        0        0     4527 2023-03-31 07:15:17.659745 promql_http_api-0.1.2/promql_http_api/api_response.py
--rw-r--r--   0        0        0     1065 2023-01-27 09:07:19.831419 promql_http_api-0.1.2/promql_http_api/buildinfo.py
--rw-r--r--   0        0        0     1056 2023-01-27 09:07:19.829418 promql_http_api-0.1.2/promql_http_api/config.py
--rw-r--r--   0        0        0     1053 2023-01-27 09:07:19.850430 promql_http_api-0.1.2/promql_http_api/flags.py
--rw-r--r--   0        0        0     1190 2023-01-27 09:07:19.812420 promql_http_api-0.1.2/promql_http_api/format_query.py
--rw-r--r--   0        0        0       45 2023-01-27 09:07:19.566419 promql_http_api-0.1.2/promql_http_api/http_config.py
--rw-r--r--   0        0        0     1344 2023-01-27 09:37:30.210288 promql_http_api-0.1.2/promql_http_api/label_values.py
--rw-r--r--   0        0        0     1068 2023-01-27 09:37:38.611318 promql_http_api-0.1.2/promql_http_api/labels.py
--rw-r--r--   0        0        0     6374 2023-01-27 09:07:19.823412 promql_http_api-0.1.2/promql_http_api/query.py
--rw-r--r--   0        0        0     1246 2023-01-27 09:07:19.818421 promql_http_api-0.1.2/promql_http_api/rules.py
--rw-r--r--   0        0        0     1071 2023-01-27 09:07:19.840413 promql_http_api-0.1.2/promql_http_api/runtimeinfo.py
--rw-r--r--   0        0        0     1497 2023-01-27 09:33:47.634307 promql_http_api-0.1.2/promql_http_api/series.py
--rw-r--r--   0        0        0     1257 2023-01-27 09:07:19.825417 promql_http_api-0.1.2/promql_http_api/targets.py
--rw-r--r--   0        0        0     1162 2023-03-31 07:18:48.585745 promql_http_api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6654 1970-01-01 00:00:00.000000 promql_http_api-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10764 2023-01-27 09:07:19.549411 promql_http_api-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     5735 2023-07-08 03:05:34.164333 promql_http_api-0.2.0/README.md
+-rw-r--r--   0        0        0      746 2023-01-27 09:07:19.565408 promql_http_api-0.2.0/promql_http_api/__init__.py
+-rw-r--r--   0        0        0     1049 2023-01-27 09:07:19.816418 promql_http_api-0.2.0/promql_http_api/alerts.py
+-rw-r--r--   0        0        0     1070 2023-01-27 09:07:19.833422 promql_http_api-0.2.0/promql_http_api/alertsmanagers.py
+-rw-r--r--   0        0        0     3388 2023-07-06 19:53:17.638030 promql_http_api-0.2.0/promql_http_api/api.py
+-rw-r--r--   0        0        0     1724 2023-01-27 09:07:19.827419 promql_http_api-0.2.0/promql_http_api/api_endpoint.py
+-rw-r--r--   0        0        0     4527 2023-03-31 07:15:17.659745 promql_http_api-0.2.0/promql_http_api/api_response.py
+-rw-r--r--   0        0        0     1065 2023-01-27 09:07:19.831419 promql_http_api-0.2.0/promql_http_api/buildinfo.py
+-rw-r--r--   0        0        0     1056 2023-01-27 09:07:19.829418 promql_http_api-0.2.0/promql_http_api/config.py
+-rw-r--r--   0        0        0     1053 2023-01-27 09:07:19.850430 promql_http_api-0.2.0/promql_http_api/flags.py
+-rw-r--r--   0        0        0     1190 2023-01-27 09:07:19.812420 promql_http_api-0.2.0/promql_http_api/format_query.py
+-rw-r--r--   0        0        0       44 2023-07-08 03:05:34.339332 promql_http_api-0.2.0/promql_http_api/http_config.py
+-rw-r--r--   0        0        0     1344 2023-01-27 09:37:30.210288 promql_http_api-0.2.0/promql_http_api/label_values.py
+-rw-r--r--   0        0        0     1068 2023-01-27 09:37:38.611318 promql_http_api-0.2.0/promql_http_api/labels.py
+-rw-r--r--   0        0        0     6844 2023-07-08 05:37:13.396655 promql_http_api-0.2.0/promql_http_api/query.py
+-rw-r--r--   0        0        0     1246 2023-01-27 09:07:19.818421 promql_http_api-0.2.0/promql_http_api/rules.py
+-rw-r--r--   0        0        0     1071 2023-01-27 09:07:19.840413 promql_http_api-0.2.0/promql_http_api/runtimeinfo.py
+-rw-r--r--   0        0        0     1497 2023-01-27 09:33:47.634307 promql_http_api-0.2.0/promql_http_api/series.py
+-rw-r--r--   0        0        0     1257 2023-01-27 09:07:19.825417 promql_http_api-0.2.0/promql_http_api/targets.py
+-rw-r--r--   0        0        0     1209 2023-07-08 03:05:34.684361 promql_http_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6881 1970-01-01 00:00:00.000000 promql_http_api-0.2.0/PKG-INFO
```

### Comparing `promql_http_api-0.1.2/LICENSE.md` & `promql_http_api-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/README.md` & `promql_http_api-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 Prometheus is an open-source system monitoring and alerting toolkit. It collects metrics from configured targets at given intervals, evaluates rule expressions, displays the results, and can trigger alerts if some condition is observed to be true. The Prometheus server exposes an HTTP API for querying the collected data, and a query language called PromQL.
 
 This library is intended to help data scientists who would like to harvest data from a Prometheus server for analysis and visualization. The library is design to be simple to use, and to provide a convenient interface to the Prometheus HTTP API. It is also designed to be performant and scalable, by using the [requests](https://requests.readthedocs.io/en/master/) library and caching HTTP connections to the Prometheus server between API accesses.
 
 For unstable connections, the library supports retrying failed requests. The user may specify the number of retries, the time-out between retries, and the back-off factor for the retry interval.
 
+Version 0.2.0 improves timezone awareness. Starting in this version, the HTTP API query is issued with a timestamp value in the 'time', 'start', and 'end' fields. In addition, the query schema now supports a 'timezone' element (provided as a timezone object), which controls the timestamp column formatting in the returned dataframe.
+
+
 ## Installation
 
 To install as a root user:
 
 ```commandline
 python3 -m pip install promql-http-api
 ```
```

### Comparing `promql_http_api-0.1.2/promql_http_api/__init__.py` & `promql_http_api-0.2.0/promql_http_api/__init__.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/alerts.py` & `promql_http_api-0.2.0/promql_http_api/alerts.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/alertsmanagers.py` & `promql_http_api-0.2.0/promql_http_api/alertsmanagers.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/api.py` & `promql_http_api-0.2.0/promql_http_api/api.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/api_endpoint.py` & `promql_http_api-0.2.0/promql_http_api/api_endpoint.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/api_response.py` & `promql_http_api-0.2.0/promql_http_api/api_response.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/buildinfo.py` & `promql_http_api-0.2.0/promql_http_api/buildinfo.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/config.py` & `promql_http_api-0.2.0/promql_http_api/config.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/flags.py` & `promql_http_api-0.2.0/promql_http_api/flags.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/format_query.py` & `promql_http_api-0.2.0/promql_http_api/format_query.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/label_values.py` & `promql_http_api-0.2.0/promql_http_api/label_values.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/labels.py` & `promql_http_api-0.2.0/promql_http_api/labels.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/query.py` & `promql_http_api-0.2.0/promql_http_api/query.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,126 +13,126 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
 from datetime import timezone
 import logging
-import pandas as pd
+from pandas import DataFrame, Timestamp
 from .api_endpoint import ApiEndpoint
+import pytz
 
 
 class Base(ApiEndpoint):
     '''
     Base class for Query and QueryRange endpoints
     '''
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.logger = logging.getLogger(f"{__name__}::{self.__class__.__name__}")
         self.timezone = timezone.utc
         self.time_format = "%Y-%m-%dT%H:%M:%S"
-        self.schema: dict = None  # type: ignore
-        self.prom_results: list = None  # type: ignore
+        self.schema = None
+        self.prom_results = {}
 
-    def to_dataframe(self):
+    def to_dataframe(self) -> DataFrame:
         '''
         Convert the PromQL query results to a Pandas DataFrame
         Implicitly executes the query if it has not already been executed
 
         Parameters:
             None
         Returns:
             df (DataFrame): The query results as a Pandas DataFrame
         '''
         data = self.response.data()
         if data is None:
-            return None
+            raise ValueError("No data in PromQL query response")
 
         self.prom_results = data['result']
         if len(self.prom_results) == 0:
-            return None
-        logging.debug(f'prom_results: {self.prom_results}')
+            raise ValueError("PromQL query response has no results")
+        self.logger.debug(f'prom_results: {self.prom_results}')
+
+        if self.schema:
+            self.timezone = self.schema.get('timezone', pytz.timezone('UTC'))
 
         prom_result_type = data['resultType']
         if prom_result_type == 'vector':
-            return self.to_dataframe_vector()
+            return self._vector_to_dataframe()
         elif prom_result_type == 'matrix':
-            return self.to_dataframe_matrix()
+            return self._matrix_to_dataframe()
         else:
-            return None
+            raise ValueError(f"Unexpected PromQL result type: {prom_result_type}")
 
-    def to_dataframe_vector(self):
+    def _vector_to_dataframe(self) -> DataFrame:
         '''
         Helper function to convert a vector result to a Pandas DataFrame
         '''
         records = []
-        columns = self.get_columns()
+        columns = self.get_schema_columns()
         for result in self.prom_results:
             prom_metric = result['metric']
-            columns: list[str] = \
-                columns if columns else list(prom_metric.keys())
+            columns = columns if columns else list(prom_metric.keys())
             record = [prom_metric[column] for column in columns]
             value = result['value']
-            timestamp = value[0]
-            timestr = self.timestamp_to_str(timestamp)
+            pd_timestamp = Timestamp(value[0], unit='s', tz=self.timezone)
             result = self.cast(value[1])
-            full_record = [timestr] + record + [result]
-            logging.debug(f'record = {full_record}')
+            full_record = [pd_timestamp] + record + [result]
+            self.logger.debug(f'record = {full_record}')
             records.append(full_record)
         columns = ['timestamp'] + columns + ['value']
-        df = pd.DataFrame(records, columns=columns)
+        df = DataFrame(records, columns=columns)
         return df
 
-    def to_dataframe_matrix(self):
+    def _matrix_to_dataframe(self):
         records = []
-        columns = self.get_columns()
+        columns = self.get_schema_columns()
         for result in self.prom_results:
             prom_metric = result['metric']
             values = result['values']
             columns = columns if columns else list(prom_metric.keys())
             record = [prom_metric[column] for column in columns]
             for value in values:
-                timestamp = value[0]
-                timestr = self.timestamp_to_str(timestamp)
+                pd_timestamp = Timestamp(value[0], unit='s', tz=self.timezone)
                 result = self.cast(value[1])
-                full_record = [timestr] + record + [result]
-                logging.debug(f'record = {full_record}')
+                full_record = [pd_timestamp] + record + [result]
+                self.logger.debug(f'record = {full_record}')
                 records.append(full_record)
         columns = ['timestamp'] + columns + ['value']
-        df = pd.DataFrame(records, columns=columns)
+        df = DataFrame(records, columns=columns)
         return df
 
-    def get_columns(self) -> list:
+    def get_schema_columns(self) -> list[str]:
         if self.schema:
-            return self.schema['columns']
+            return self.schema.get('columns', [])
         else:
-            return None  # type: ignore
-
-    def timestamp_to_str(self, timestamp):
-        date_time = datetime.fromtimestamp(timestamp)
-        return date_time.astimezone(self.timezone).strftime(self.time_format)
+            return []
 
     def cast(self, result):
         if self.schema:
-            dtype: type = self.schema.get('dtype', str)
+            dtype = self.schema.get('dtype', str)
             result = dtype(result)
         return result
 
 
 class Query(Base):
     '''
     Query API endpoint class
     '''
 
     def __init__(self,
-                 url: str = None,    # type: ignore
-                 query: str = None,  # type: ignore
-                 time: str = None):  # type: ignore
+                 url: str = "",
+                 query: str = "",
+                 time: datetime = datetime.now()):
         super().__init__(url)
-        self.query: str = query
+        self.logger = logging.getLogger(f"{__name__}::{self.__class__.__name__}")
+        self.logger.debug(f"url = {url}; query = {query}; time = {time}")
+        self.query = query
         self.time = time
 
     def __str__(self):
         return self.query
 
     def __repr__(self):
         return self.query
@@ -142,38 +142,42 @@
         Make the URL for the API endpoint
 
         Parameters:
             None
         Returns:
             url (str): The URL for the API endpoint
         '''
-        url = '/api/v1/query?query=' + self.query
-        url += '&time=' + self.time if self.time else ''
+        url = '/api/v1/query?query=' + str(self.query)
+        if self.time:
+            time_str = str(self.time.timestamp())
+            url += '&time=' + time_str
         return url
 
-    def to_dataframe(self, schema: dict = None):  # type: ignore
+    def to_dataframe(self, schema: dict | None = None):
         if self.query is None:
             return None
         self.schema = schema
         self.__call__()
         return super().to_dataframe()
 
 
 class QueryRange(Base):
     '''
     QueryRange API endpoint class
     '''
 
     def __init__(self,
-                 url: str = None,    # type: ignore
-                 query: str = None,  # type: ignore
-                 start: str = None,  # type: ignore
-                 end: str = None,    # type: ignore
-                 step: str = None):  # type: ignore
+                 url: str,
+                 query: str,
+                 start: datetime,
+                 end: datetime,
+                 step: str):
         super().__init__(url)
+        self.logger = logging.getLogger(f"{__name__}::{self.__class__.__name__}")
+        self.logger.debug(f'query = {query}; start = {start}; end = {end}; step = {step}')
         self.query = query
         self.start = start
         self.end = end
         self.step = step
 
     def __str__(self):
         return self.query
@@ -186,19 +190,22 @@
         Make the URL for the API endpoint
 
         Parameters:
             None
         Returns:
             url (str): The URL for the API endpoint
         '''
+        start = str(self.start.timestamp())
+        end = str(self.end.timestamp())
         url = '/api/v1/query_range?query=' + self.query
-        url += '&start=' + self.start
-        url += '&end=' + self.end
+        url += '&start=' + start
+        url += '&end=' + end
         url += '&step=' + self.step
+        self.logger.debug(f'returned url = {url}')
         return url
 
-    def to_dataframe(self, schema: dict = None):  # type: ignore
+    def to_dataframe(self, schema: dict = {}):
         if self.query is None:
             return None
         self.schema = schema
         self.__call__()
         return super().to_dataframe()
```

### Comparing `promql_http_api-0.1.2/promql_http_api/rules.py` & `promql_http_api-0.2.0/promql_http_api/rules.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/runtimeinfo.py` & `promql_http_api-0.2.0/promql_http_api/runtimeinfo.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/series.py` & `promql_http_api-0.2.0/promql_http_api/series.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/promql_http_api/targets.py` & `promql_http_api-0.2.0/promql_http_api/targets.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.1.2/pyproject.toml` & `promql_http_api-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promql-http-api"
-version = "0.1.2"
+version = "0.2.0"
 description = "Query a Prometheus server and get a Pandas DataFrame"
 homepage = "https://github.com/nir-arad/promql-http-api"
 repository = "https://github.com/nir-arad/promql-http-api"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["prometheus", "promql", "pandas", "dataframe"]
 authors = ["Nir Arad"]
@@ -19,15 +19,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = {version = ">=0.22,<0.24", source = "pypi"}
-requests = "^2.28.2"
+requests = "^2.31.0"
+pandas = "^2.0.0"
+types-setuptools = "^68.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 pytest-cov = "^3.0.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/nir-arad/promql-http-api/issues"
```

### Comparing `promql_http_api-0.1.2/PKG-INFO` & `promql_http_api-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promql-http-api
-Version: 0.1.2
+Version: 0.2.0
 Summary: Query a Prometheus server and get a Pandas DataFrame
 Home-page: https://github.com/nir-arad/promql-http-api
 License: Apache-2.0
 Keywords: prometheus,promql,pandas,dataframe
 Author: Nir Arad
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -12,21 +12,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: httpx (>=0.22,<0.24)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: types-setuptools (>=68.0.0,<69.0.0)
 Project-URL: Bug Tracker, https://github.com/nir-arad/promql-http-api/issues
 Project-URL: Repository, https://github.com/nir-arad/promql-http-api
 Description-Content-Type: text/markdown
 
 # PromQL HTTP API
 
 This python package provides a [Prometheus](https://prometheus.io/) HTTP API client library.
@@ -35,14 +33,17 @@
 
 Prometheus is an open-source system monitoring and alerting toolkit. It collects metrics from configured targets at given intervals, evaluates rule expressions, displays the results, and can trigger alerts if some condition is observed to be true. The Prometheus server exposes an HTTP API for querying the collected data, and a query language called PromQL.
 
 This library is intended to help data scientists who would like to harvest data from a Prometheus server for analysis and visualization. The library is design to be simple to use, and to provide a convenient interface to the Prometheus HTTP API. It is also designed to be performant and scalable, by using the [requests](https://requests.readthedocs.io/en/master/) library and caching HTTP connections to the Prometheus server between API accesses.
 
 For unstable connections, the library supports retrying failed requests. The user may specify the number of retries, the time-out between retries, and the back-off factor for the retry interval.
 
+Version 0.2.0 improves timezone awareness. Starting in this version, the HTTP API query is issued with a timestamp value in the 'time', 'start', and 'end' fields. In addition, the query schema now supports a 'timezone' element (provided as a timezone object), which controls the timestamp column formatting in the returned dataframe.
+
+
 ## Installation
 
 To install as a root user:
 
 ```commandline
 python3 -m pip install promql-http-api
 ```
```

