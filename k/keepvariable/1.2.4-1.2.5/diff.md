# Comparing `tmp/keepvariable-1.2.4.tar.gz` & `tmp/keepvariable-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepvariable-1.2.4.tar", last modified: Fri Jun 23 17:44:19 2023, max compression
+gzip compressed data, was "keepvariable-1.2.5.tar", last modified: Sat Jul  8 14:05:19 2023, max compression
```

## Comparing `keepvariable-1.2.4.tar` & `keepvariable-1.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 17:44:19.689001 keepvariable-1.2.4/
--rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.2.4/LICENSE
--rw-rw-rw-   0        0        0     2146 2023-06-23 17:44:19.688004 keepvariable-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 17:44:19.656089 keepvariable-1.2.4/keepvariable/
--rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.2.4/keepvariable/__init__.py
--rw-rw-rw-   0        0        0    25108 2023-06-23 17:43:47.000000 keepvariable-1.2.4/keepvariable/keepvariable_core.py
--rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.2.4/keepvariable/keepvariable_model.py
--rw-rw-rw-   0        0        0     1684 2023-05-25 15:03:40.000000 keepvariable-1.2.4/keepvariable/kv_redis_example.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:44:19.687006 keepvariable-1.2.4/keepvariable.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-06-23 17:44:18.000000 keepvariable-1.2.4/keepvariable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-06-23 17:44:19.000000 keepvariable-1.2.4/keepvariable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 17:44:18.000000 keepvariable-1.2.4/keepvariable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-23 17:44:19.000000 keepvariable-1.2.4/keepvariable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-23 17:44:19.000000 keepvariable-1.2.4/keepvariable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 17:44:19.689001 keepvariable-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-06-23 17:44:01.000000 keepvariable-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:05:19.652903 keepvariable-1.2.5/
+-rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     2146 2023-07-08 14:05:19.651524 keepvariable-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 14:05:19.631416 keepvariable-1.2.5/keepvariable/
+-rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.2.5/keepvariable/__init__.py
+-rw-rw-rw-   0        0        0    28122 2023-07-08 14:04:20.000000 keepvariable-1.2.5/keepvariable/keepvariable_core.py
+-rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.2.5/keepvariable/keepvariable_model.py
+-rw-rw-rw-   0        0        0     1684 2023-05-25 15:03:40.000000 keepvariable-1.2.5/keepvariable/kv_redis_example.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:05:19.651524 keepvariable-1.2.5/keepvariable.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-07-08 14:05:18.000000 keepvariable-1.2.5/keepvariable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-07-08 14:05:19.000000 keepvariable-1.2.5/keepvariable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 14:05:18.000000 keepvariable-1.2.5/keepvariable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 14:05:19.000000 keepvariable-1.2.5/keepvariable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-08 14:05:19.000000 keepvariable-1.2.5/keepvariable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 14:05:19.652979 keepvariable-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-07-08 14:04:57.000000 keepvariable-1.2.5/setup.py
```

### Comparing `keepvariable-1.2.4/LICENSE` & `keepvariable-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `keepvariable-1.2.4/PKG-INFO` & `keepvariable-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.2.4
+Version: 1.2.5
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.2.4/README.md` & `keepvariable-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `keepvariable-1.2.4/keepvariable/keepvariable_core.py` & `keepvariable-1.2.5/keepvariable/keepvariable_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,17 +181,18 @@
         :type additional_params: Optional[dict], optional
         :return: Jsonified value
         :rtype: Any
         """
         if additional_params is None:
             additional_params = {}
 
+            
         if isinstance(value, type(None)):
-            value = {"object_type": "NoneType"}              # Redis does not natively support None values
-        elif isinstance(value, (list, bool, dict)):
+            value = {"object_type": "NoneType"} # Redis does not natively support None values
+        elif isinstance(value, list) or isinstance(value, bool) or isinstance(value, dict):
             value = json.dumps(value)
         elif isinstance(value, pd.DataFrame):
             value = self._json_serialize_dataframe(value)
             # Old implementation
             # TODO: Keep for now, delete in following commits
             # data = value.values.tolist()
             # columns = list(value.columns)
@@ -218,17 +219,16 @@
         elif inspect.isclass(value):
             code = additional_params.get("code")
             value = {"code": code, "object_type": "class"}
             value = json.dumps(code)
 
         return value
 
-    def decode_loaded_value(
-        self, value: str
-    ) -> Union[dict, pd.DataFrame, np.ndarray, datetime.datetime]:
+    def decode_loaded_value(self,
+                            value: str) -> Union[dict, pd.DataFrame, np.ndarray, datetime.datetime]:
         """
         Decode value stored in redis into it's initial value.
         For functions and classes only their code is returned --> they need to be evaluated afterwards!!!.
 
         :param value: Variable value from redis
         :type value: Any
         :return: Parsed variable value
@@ -240,28 +240,21 @@
             if "object_type" in value and isinstance(value, dict):
                 if value["object_type"] == "NoneType":
                     return None
                 elif value["object_type"] == "pd.DataFrame":
                     df = pd.DataFrame(value["data"], columns=value["columns"])
                     return df
                 elif value["object_type"] == "np.ndarray":
-                    array = pd.DataFrame(
-                        value["data"]
-                    ).values  # to ensure 64bit values in array
+                    array = pd.DataFrame(value["data"]).values  # to ensure 64bit values in array
                     return array
 
                 elif value["object_type"] == "datetime.datetime":
-                    datetime_value = datetime.datetime.strptime(
-                        value["data"], "%Y-%m-%d %H:%M:%S"
-                    )
+                    datetime_value = datetime.datetime.strptime(value["data"], "%Y-%m-%d %H:%M:%S")
                     return datetime_value
-                elif (
-                    value["object_type"] == "function" or
-                    value["object_type"] == "class"
-                ):
+                elif (value["object_type"] == "function" or value["object_type"] == "class"):
                     return value["code"]
             return value
         except json.JSONDecodeError:  # if type is str, it fails to decode
             return value
 
     @abstractmethod
     def lock(self, *args, **kwargs) -> RedisLock:
@@ -279,17 +272,17 @@
     def json_mset(self, name: str, params: dict) -> None:
         """Set multiple keys in json document - explanations are in abstract subclasses docstrings."""
         pass
 
     @abstractmethod
     def query(
         self, *, text_params: Optional[dict[str, tuple]] = None,
-        tag_params: Optional[dict[str, tuple]] = None,
-        field_to_sort_by: Optional[str] = None, asc=True, **kwargs
-    ) ->  dict[str, dict]:
+        tag_params: Optional[dict[str, tuple]] = None, field_to_sort_by: Optional[str] = None,
+        asc=True, **kwargs
+    ) -> dict[str, dict]:
         """Query KeepVariable store - explanations are in abstract subclasses docstrings."""
         pass
 
     # Implemented, but currently not used
     @abstractmethod
     def arrlen(self, name: str, path: str) -> Optional[int]:
         """
@@ -314,14 +307,33 @@
         :param path: Redis JSON path string e.g. "job.nodes[2].status"
         :type path: str
         :return: Final size of the array
         :rtype: Optional[int]
         """
         pass
 
+    @abstractmethod
+    def scan(self, match_string: str, count: int = 50, type_: Optional[str] = None):
+        """
+        Find saved keys, matching their name with a given glob-style pattern.
+        This command does not block the server, as it is based on a cursor-style iterator.
+
+        :param match_string: string pattern to match keys against, e.g. 'jobs:*'
+        :type match_string: str
+        :param count: how many rows to fetch in one iteration, defaults to 50
+        :type count: int, optional
+        :param type_: filter on specified Redis key type, defaults to None
+        :type type_: Optional[str], optional
+        """
+        pass
+
+    @abstractmethod
+    def delete(self, *names: list[str]) -> int:
+        pass
+
 
 class KeepVariableDummyRedisServer(AbstractKeepVariableServer):
     def __init__(self, host="localhost"):
         self.host = host
         self.storage = {}
 
     def lock(self, *args, **kwargs) -> RedisLock:
@@ -334,25 +346,27 @@
                 return True
 
             def release(self):
                 pass
 
         return DummyLock()
 
-    def set(self, key, value, additional_params: Optional[dict] = None):
-        if additional_params is None:
-            additional_params = {}
+    def set(self, key: str, value, additional_params: Optional[dict] = None) -> dict[str, str]:
+        additional_params = {} if additional_params is None else additional_params
 
         value = self.parse_saved_value(value, additional_params)
         self.storage[key] = value
         return {key: value}
 
+    # QUESTION: For in-app memory, is there a point to store serialized values? - Dom: yes, it is not used only as in-app memory
     def get(self, key: str) -> Union[dict, pd.DataFrame, np.ndarray, datetime.datetime]:
         value = self.storage.get(key)
-
+        
+        
+          
         # Do not move this condition to decode_loaded_value(), it only deals with missing keys
         if value is None:
             return None
 
         decoded_value = self.decode_loaded_value(value)
         return decoded_value
 
@@ -367,17 +381,15 @@
         More info: https://redis.io/docs/stack/json/path/
         :type params: dict
 
         e.g.
         params = {"$.is_saved"=true, "$.status"=SomeEnum.COMPLETED.value}
         """
         for json_xpath, value in params.items():
-            element, last_element, last_index = self._extract_object_from_path(
-                name, json_xpath
-            )
+            element, last_element, last_index = self._extract_object_from_path(name, json_xpath)
             if last_index:
                 element[last_element][last_index] = value
             else:
                 element[last_element] = value
 
     def query(
         self,
@@ -398,18 +410,16 @@
         :type tag_params: dict[str, tuple]
         :param sort_by_name: attribute name by which results should be sorted
         :type sort_by_name: str
         :return: [('jobs:43', job_dict), ...]
         :rtype: list[tuple]
         """
         found_jobs: dict[str, dict] = {
-            job_name: value
-            for job_name, value in self.storage.items()
-            if name in job_name
-          }  # {'jobs:43': job_dict, ...}
+            job_name: value for job_name, value in self.storage.items() if name in job_name
+        }  # {'jobs:43': job_dict, ...}
 
         # TAG search
         if tag_params is not None:
             for field, values in tag_params.items():
                 found_jobs = {
                     job_id: job for job_id, job in found_jobs.items()
                     if job.get(field) and job.get(field) in values
@@ -423,53 +433,49 @@
                     found_jobs = {
                         job_id: job for job_id, job in found_jobs.items()
                         if job.get(field) and value in job.get(field)
                     }
 
         if field_to_sort_by:
             found_jobs_list = sorted(found_jobs.items(), key=lambda x: x[1][field_to_sort_by])
-        if not asc:
-            found_jobs_list.reverse()
+            if not asc:
+                found_jobs_list.reverse()
+            found_jobs = dict(found_jobs_list)
 
-        return dict(found_jobs_list)
+        return found_jobs
 
     def arrlen(self, name: str, path: str) -> Optional[int]:
         try:
-            element, last_element, last_index = self._extract_object_from_path(
-                name, path
-            )
+            element, last_element, last_index = self._extract_object_from_path(name, path)
             if last_index:
                 return len(element[last_element][last_index])
             else:
                 return len(element[last_element])
         except (KeyError, IndexError) as e:
             raise AssertionError(
                 "Nested object does not exist - most probably due to incorrect path arg"
             ) from e
 
     def arrappend(self, name: str, path: str, objects: Sequence) -> Optional[int]:
         try:
-            element, last_element, last_index = self._extract_object_from_path(
-                name, path
-            )
+            element, last_element, last_index = self._extract_object_from_path(name, path)
             if last_index:
                 for obj in objects:
                     element[last_element][last_index].append(obj)
                 return len(element[last_element][last_index])
             else:
                 for obj in objects:
                     element[last_element].append(obj)
                 return len(element[last_element])
         except (KeyError, IndexError) as e:
             raise AssertionError(
                 "Nested object does not exist - most probably due to incorrect path arg"
             ) from e
 
-    def _extract_object_from_path(self, name: str,
-                                  path: str) -> tuple[Any, str, Optional[int]]:
+    def _extract_object_from_path(self, name: str, path: str) -> tuple[Any, str, Optional[int]]:
         """
         Recursively traverses a JSON document under 'name' to access the object defined by the 'path' argument.
 
         :param name: key under which a JSON document is stored
         :type name: str
         :param path: Redis JSON path string e.g. "job.nodes[2].status"
         :type path: str
@@ -515,28 +521,47 @@
             if index is not None:
                 nested_object = nested_object[element][index]
             else:
                 nested_object = nested_object[element]
 
         return nested_object, element_list[-1], index_list[-1]
 
+    def scan(self, match_string: str, *args, **kwargs) -> list[str]:
+        """
+        Find saved keys, matching their name with a given glob-style pattern.
+        This command does not block the server, as it is based on a cursor-style iterator.
+
+        :param match_string: string pattern to match keys against, e.g. 'jobs:*'
+        :type match_string: str
+        :return: list of found key names
+        :rtype: list[str]
+        """
+        # Convert glob-style pattern to regex
+        match_pattern = match_string.replace("*", ".*").replace("?", ".")
+        results = [key for key in self.storage.keys() if re.search(match_pattern, key)]
+        return results
+
+    def delete(self, *names: list[str]) -> int:
+        return sum(1 for name in names if self.storage.pop(name, None))
+
 
 class KeepVariableRedisServer(AbstractKeepVariableServer):
-    def __init__(self, host="localhost", port=6379, password: Optional[str] = None):
+    def __init__(
+        self, host="localhost", port=6379, db=0, username='default', password: Optional[str] = None
+    ):
         self.host: str = host
         self.port: int = port
+        self.db = db
+        self.username: str = username
         self.password: Optional[str] = password
 
+        # Redis instance maintains connection pool internally, additionally it is thread-safe.
         self.redis = redis.Redis(
-            host=self.host,
-            port=self.port,
-            db=0,
-            password=self.password,
-            decode_responses=True,
-            charset="utf-8",
+            host=self.host, port=self.port, username=self.username, db=self.db,
+            password=self.password, decode_responses=True, charset="utf-8"
         )
 
     @property
     def kept_variables(self):
         return self._kept_variables
 
     @kept_variables.setter
@@ -552,21 +577,24 @@
             additional_params = {}
 
         value = self.parse_saved_value(value, additional_params)
         result = self.redis.set(key, value)
         return result
 
     def get(self, key: str) -> Optional[Any]:
-        value = self.redis.get(key)
-
-        # Do not move this condition to decode_loaded_value(), it only deals with missing keys
-        if value is None:
-            return None
-
-        decoded_value = self.decode_loaded_value(value)
+        try:
+            value = self.redis.get(key)
+      
+            # Do not move this condition to decode_loaded_value(), it only deals with missing keys
+            if value is None:
+                return value
+            decoded_value = self.decode_loaded_value(value)
+        # Raised when trying to get JSON document in Redis. JSON documents have their own get method
+        except redis.exceptions.ResponseError:
+            decoded_value = self.redis.json().get(key)
         return decoded_value
 
     def json_mset(self, name: str, params: dict[str, Any], transaction=True) -> None:
         """
         Set multiple keys in Redis JSON document. This method uses RedisJSON.
 
         :param name: Key of the Redis variable
@@ -586,31 +614,31 @@
                 pipe.json().set(name, json_xpath, value)
             pipe.execute()
 
     def query(
         self, *, text_params: Optional[dict[str, tuple]] = None,
         tag_params: Optional[dict[str, tuple]] = None, index_name: str,
         field_to_sort_by: Optional[str] = None, asc=True, **kwargs
-    ) -> dict[str, dict]:
+    ) -> dict:
         """
         Simplified wrapper to RedisSearch. Allows to search and sort by a value of Redis TAG/TEXT fields.
         Simplistic on purpose, to avoid bloat. Additional functionality should be added in case of need.
 
         :param text_params: key name to a tuple of values mapping, e.g. {'status': ('pipel', ...), ...}
         :type text_params: dict[str, tuple]
         :param tag_params: key name to a tuple of values mapping, e.g. {'status': ('QUEUED', ...), ...}
         :type tag_params: dict[str, tuple]
         :param index_name: name of the Redis index used for querying
         :type index_name: str
         :param field_to_sort_by: attribute name by which results should be sorted, defaults to None
         :type field_to_sort_by: Optional[str], optional
         :param asc: True if sort in ascending order, defaults to True
         :type asc: bool, optional
-        :return: {'jobs:43': job_json, ...}
-        :rtype: dict[str, dict]
+        :return: {'jobs:43': job_dict, ...}
+        :rtype: dict[str, Any]
         """
         final_query = ""
 
         if text_params is not None:
             text_query_template = "@{field}:{value}"
             for field, values in text_params.items():
                 value_str = "|".join(values)
@@ -618,21 +646,46 @@
 
         if tag_params is not None:
             tag_query_template = "@{field}:{{{value}}}"
             for field, values in tag_params.items():
                 value_str = "|".join(values)
                 final_query += tag_query_template.format(field=field, value=value_str)
 
+        # If no query was specified, return all records from the index
+        if not final_query:
+            final_query = "*"
+
         # Query example: "@type:PIPEL @status:{QUEUED|COMPLETED}"
         # Explanation: find all jobs with type field containing 'PIPEL' and status being either 'QUEUED' or 'COMPLETED'
         query_object = Query(final_query)
         if field_to_sort_by:
             query_object.sort_by(field_to_sort_by, asc=asc)
 
         job_docs: list = self.redis.ft(index_name).search(query_object).docs
-        return {job_doc.id: job_doc.json for job_doc in job_docs}
+        return {job_doc.id: self.decode_loaded_value(job_doc.json) for job_doc in job_docs}
 
     def arrlen(self, name: str, path: str) -> Optional[int]:
         return self.redis.json().arrlen(name, path).pop()
 
     def arrappend(self, name: str, path: str, objects: Sequence) -> Optional[int]:
         return self.redis.json().arrappend(name, path, *objects).pop()
+
+    def scan(self, match_string: str, count: int = 50, type_: Optional[str] = None) -> list[str]:
+        """
+        Find saved keys, matching their name with a given glob-style pattern.
+        This command does not block the server, as it is based on a cursor-style iterator.
+
+        https://redis.io/commands/scan/
+
+        :param match_string: string pattern to match keys against, e.g. 'jobs:*'
+        :type match_string: str
+        :param count: how many rows, defaults to 50
+        :type count: int, optional
+        :param type_: filter on specified Redis key type, defaults to None
+        :type type_: Optional[str], optional
+        :return: list of found keys
+        :rtype: list[str]
+        """
+        return list(self.redis.scan_iter(match_string, count, type_))
+
+    def delete(self, *names: list[str]) -> int:
+        return self.redis.delete(*names)
```

### Comparing `keepvariable-1.2.4/keepvariable/kv_redis_example.py` & `keepvariable-1.2.5/keepvariable/kv_redis_example.py`

 * *Files identical despite different names*

### Comparing `keepvariable-1.2.4/keepvariable.egg-info/PKG-INFO` & `keepvariable-1.2.5/keepvariable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.2.4
+Version: 1.2.5
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.2.4/setup.py` & `keepvariable-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='keepvariable',
-    version='1.2.4',
+    version='1.2.5',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='A Python package keeping the values of variables between separate runs in a seamless and effortless way.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/keepvariable',
     packages=setuptools.find_packages(),
```

