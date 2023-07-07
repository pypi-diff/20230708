# Comparing `tmp/cbcmgr-1.3.6.tar.gz` & `tmp/cbcmgr-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.3.6.tar", last modified: Fri Jul  7 20:37:01 2023, max compression
+gzip compressed data, was "cbcmgr-1.3.7.tar", last modified: Fri Jul  7 23:46:08 2023, max compression
```

## Comparing `cbcmgr-1.3.6.tar` & `cbcmgr-1.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:37:01.794421 cbcmgr-1.3.6/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.6/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 20:37:01.794245 cbcmgr-1.3.6/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.6/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:37:01.726436 cbcmgr-1.3.6/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.6/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.6/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    26442 2023-07-07 20:36:57.000000 cbcmgr-1.3.6/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 19:40:32.000000 cbcmgr-1.3.6/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.3.6/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.6/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.6/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.6/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.6/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.6/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:37:01.793880 cbcmgr-1.3.6/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 20:37:01.000000 cbcmgr-1.3.6/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 20:37:01.000000 cbcmgr-1.3.6/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 20:37:01.000000 cbcmgr-1.3.6/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 20:37:01.000000 cbcmgr-1.3.6/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 20:37:01.000000 cbcmgr-1.3.6/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 20:37:01.794482 cbcmgr-1.3.6/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 20:33:10.000000 cbcmgr-1.3.6/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 23:46:08.080478 cbcmgr-1.3.7/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.7/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 23:46:08.080349 cbcmgr-1.3.7/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.7/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 23:46:08.061800 cbcmgr-1.3.7/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.7/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11122 2023-07-07 23:20:50.000000 cbcmgr-1.3.7/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    27405 2023-07-07 23:33:22.000000 cbcmgr-1.3.7/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)    11287 2023-07-07 23:20:50.000000 cbcmgr-1.3.7/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.3.7/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.7/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.7/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.3.7/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.7/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.7/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 23:46:08.080137 cbcmgr-1.3.7/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 23:46:08.000000 cbcmgr-1.3.7/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 23:46:08.000000 cbcmgr-1.3.7/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 23:46:08.000000 cbcmgr-1.3.7/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 23:46:08.000000 cbcmgr-1.3.7/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 23:46:08.000000 cbcmgr-1.3.7/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 23:46:08.080521 cbcmgr-1.3.7/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 21:00:17.000000 cbcmgr-1.3.7/setup.py
```

### Comparing `cbcmgr-1.3.6/LICENSE.txt` & `cbcmgr-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.6/PKG-INFO` & `cbcmgr-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.6
+Version: 1.3.7
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.6/README.md` & `cbcmgr-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.6/cbcmgr/cb_connect.py` & `cbcmgr-1.3.7/cbcmgr/cb_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
             self.collection(collection)
         return self
 
     def bucket(self, name: str):
         logger.debug(f"bucket: connecting bucket {name}")
         if self._cluster:
             self._bucket = retry_inline(self._cluster.bucket, name)
+            self._bucket_name = name
         else:
             raise ClusterNotConnected("no cluster connected")
 
     def scope(self, name: str = "_default"):
         if self._bucket:
             logger.debug(f"scope: connecting scope {name}")
             self._cluster.wait_until_ready(timedelta(seconds=4), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue]))
```

### Comparing `cbcmgr-1.3.6/cbcmgr/cb_management.py` & `cbcmgr-1.3.7/cbcmgr/cb_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -494,24 +494,57 @@
 
             except AttributeError:
                 raise PathMapUpsertError(f"cb_map_upsert: key {c.path} not found")
 
             except Exception as err:
                 raise PathMapUpsertError(f"cb_map_upsert: error {err}")
 
+    @retry()
+    def _cb_upsert(self, cluster, c_name, meta_id, doc_data, timeout=5):
+        upsert_options = UpsertOptions(timeout=timedelta(seconds=timeout))
+        try:
+            logger.debug(f"upsert -> {c_name}: {meta_id}")
+            bucket = cluster.bucket(self._bucket_name)
+            collection = bucket.scope(self._scope_name).collection(c_name)
+            result = collection.upsert(meta_id, doc_data, upsert_options)
+            return result.cas
+        except Exception as error:
+            raise CollectionUpsertError(f"upsert error: {error}")
+
+    @retry()
+    def _create_collection(self, cluster, c_name):
+        bucket = cluster.bucket(self._bucket_name)
+        cm = bucket.collections()
+        try:
+            collection_spec = CollectionSpec(c_name, scope_name=self._scope_name)
+            cm.create_collection(collection_spec, CreateCollectionOptions(timeout=timedelta(seconds=10)))
+            self._verify_collection(cm, c_name)
+        except CollectionAlreadyExistsException:
+            pass
+        except Exception as error:
+            raise CollectionCreateException(f"collection create error: {error}")
+
+    @retry()
+    def _verify_collection(self, cm, c_name):
+        sm = next((s for s in cm.get_all_scopes() if s.name == self._scope_name), None)
+        valid = next((i for i in sm.collections if i.name == c_name), None)
+        if not valid:
+            raise CollectionCreateException(f"collection {c_name} was not created")
+
     def cb_map_upsert(self,
                       prefix: str,
                       config: UpsertMapConfig,
                       json_file: str = None,
                       xml_file: str = None,
                       json_data: str = None,
                       xml_data: str = None,
                       timeout=5):
         tasks = set()
         executor = concurrent.futures.ThreadPoolExecutor()
+        cluster = Cluster.connect(self.cb_connect_string, self.cluster_options)
 
         if json_file:
             with open(json_file, mode="r") as json_xml:
                 data = json.load(json_xml)
         elif xml_file:
             with open(xml_file, mode="rb") as input_xml:
                 contents = input_xml.read()
@@ -519,39 +552,28 @@
         elif json_data:
             data = json.loads(json_data)
         elif xml_data:
             data = xmltodict.parse(xml_data)
         else:
             raise PathMapUpsertError(f"cb_map_upsert: JSON or XML input data is required")
 
-        def _cb_upsert(collection, meta_id, doc_data):
-            try:
-                upsert_options = UpsertOptions(timeout=timedelta(seconds=timeout))
-                _collection = self._scope.collection(collection)
-                result = retry_inline(_collection.upsert, meta_id, doc_data, upsert_options)
-                logger.debug(f"upsert -> {collection}: {meta_id}: cas {result.cas}")
-                return result.cas
-            except Exception as error:
-                raise CollectionUpsertError(f"upsert error: {error}")
-
-        def _create_collection(c_name):
-            try:
-                collection_spec = CollectionSpec(c_name, scope_name=self._scope.name)
-                cm = self._bucket.collections()
-                cm.create_collection(collection_spec, CreateCollectionOptions(timeout=timedelta(seconds=10)))
-            except CollectionAlreadyExistsException:
-                pass
-            except Exception as error:
-                raise CollectionCreateException(f"collection create error: {error}")
-
         for c in config.paths:
             if c.collection:
                 logger.debug(f"cb_map_upsert: creating collection {c.name}")
-                retry_inline(_create_collection, c.name)
+                tasks.add(executor.submit(self._create_collection, cluster, c.name))
+
+        while tasks:
+            done, tasks = concurrent.futures.wait(tasks, return_when=concurrent.futures.FIRST_COMPLETED)
+            for task in done:
+                try:
+                    task.result()
+                except Exception as err:
+                    raise PathMapUpsertError(f"cb_map_upsert: {err}")
 
+        tasks.clear()
         for c in config.paths:
             logger.debug(f"cb_map_upsert: processing key {c.path} name {c.name}")
 
             subset = copy_path(c.path, data)
 
             if not subset or len(subset) == 0:
                 if c.optional:
@@ -567,22 +589,23 @@
             if c.exclude:
                 logger.debug(f"cb_map_upsert: excluding {','.join(c.exclude)}")
                 subset = omit_path(subset, c.exclude)
 
             if c.p_type == MapUpsertType.DOCUMENT:
                 doc_id = self.key_format(c.id, subset, text=prefix)
                 logger.debug(f"cb_map_upsert: processing doc ID {doc_id}")
-                tasks.add(executor.submit(_cb_upsert, collection_name, doc_id, {c.name: subset}))
+                doc = {c.name: subset}
+                tasks.add(executor.submit(self._cb_upsert, cluster, collection_name, doc_id, doc, timeout))
             elif c.p_type == MapUpsertType.LIST:
                 logger.debug(f"cb_map_upsert: processing list")
                 if not isinstance(subset, list):
                     raise PathMapUpsertError(f"cb_map_upsert: path {c.path} type {type(subset)} incompatible with list mode")
                 for doc in subset:
                     doc_id = self.key_format(c.id, doc, text=prefix, id_key=c.id_key)
-                    tasks.add(executor.submit(_cb_upsert, collection_name, doc_id, doc))
+                    tasks.add(executor.submit(self._cb_upsert, cluster, collection_name, doc_id, doc, timeout))
 
         while tasks:
             done, tasks = concurrent.futures.wait(tasks, return_when=concurrent.futures.FIRST_COMPLETED)
             for task in done:
                 try:
                     task.result()
                 except Exception as err:
```

### Comparing `cbcmgr-1.3.6/cbcmgr/cb_session.py` & `cbcmgr-1.3.7/cbcmgr/cb_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     def __init__(self, hostname: str, username: str, password: str, ssl=False, external=False):
         self.cluster_node_count = None
         self._cluster = None
         self._bucket = None
         self._scope = None
         self._collection = None
+        self._bucket_name = None
         self._scope_name = "_default"
         self._collection_name = "_default"
         self.username = username
         self.password = password
         self.ssl = ssl
         self.rally_host_name = hostname
         self.rally_cluster_node = self.rally_host_name
```

### Comparing `cbcmgr-1.3.6/cbcmgr/config.py` & `cbcmgr-1.3.7/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.6/cbcmgr/exceptions.py` & `cbcmgr-1.3.7/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.6/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.3.7/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.6/cbcmgr/retry.py` & `cbcmgr-1.3.7/cbcmgr/retry.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 
 import time
 import asyncio
 import logging
 from typing import Callable
 from functools import wraps
 
+logger = logging.getLogger('cbutil.retry')
+logger.addHandler(logging.NullHandler())
+
 
 def retry_inline(func, *args, retry_count=10, factor=0.01, **kwargs):
-    logger = logging.getLogger(retry_inline.__name__)
     for retry_number in range(retry_count + 1):
         try:
             return func(*args, **kwargs)
         except Exception as err:
             if retry_number == retry_count:
                 logger.debug(f"{func.__name__} retry limit exceeded: {err}")
                 raise
@@ -24,15 +26,14 @@
 
 
 def retry(retry_count=10,
           factor=0.01,
           allow_list=None,
           always_raise_list=None
           ) -> Callable:
-    logger = logging.getLogger(retry.__name__)
 
     def retry_handler(func):
         if not asyncio.iscoroutinefunction(func):
             @wraps(func)
             def f_wrapper(*args, **kwargs):
                 for retry_number in range(retry_count + 1):
                     try:
```

### Comparing `cbcmgr-1.3.6/cbcmgr/schema.py` & `cbcmgr-1.3.7/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.6/cbcmgr/util.py` & `cbcmgr-1.3.7/cbcmgr/util.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.6/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.3.7/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.6
+Version: 1.3.7
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.6/setup.py` & `cbcmgr-1.3.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.3.6',
+    version='1.3.7',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```

