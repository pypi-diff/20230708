# Comparing `tmp/pyassorted-0.7.2.tar.gz` & `tmp/pyassorted-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyassorted-0.7.2.tar", max compression
+gzip compressed data, was "pyassorted-0.7.3.tar", max compression
```

## Comparing `pyassorted-0.7.2.tar` & `pyassorted-0.7.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1066 2023-02-15 09:16:45.010069 pyassorted-0.7.2/LICENSE
--rw-r--r--   0        0        0     6993 2023-05-27 10:25:12.261799 pyassorted-0.7.2/README.md
--rw-r--r--   0        0        0       53 2023-04-01 13:44:09.334164 pyassorted-0.7.2/pyassorted/__init__.py
--rw-r--r--   0        0        0      116 2023-02-17 09:28:12.934937 pyassorted-0.7.2/pyassorted/asyncio/__init__.py
--rw-r--r--   0        0        0     1349 2023-04-01 13:44:09.334680 pyassorted-0.7.2/pyassorted/asyncio/executor.py
--rw-r--r--   0        0        0     2943 2023-05-15 11:57:33.581730 pyassorted-0.7.2/pyassorted/asyncio/io.py
--rw-r--r--   0        0        0     1017 2023-02-15 09:50:56.450314 pyassorted-0.7.2/pyassorted/asyncio/utils.py
--rw-r--r--   0        0        0       61 2023-03-27 15:28:16.228462 pyassorted-0.7.2/pyassorted/cache/__init__.py
--rw-r--r--   0        0        0     8109 2023-03-27 15:28:16.228823 pyassorted-0.7.2/pyassorted/cache/cache.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:33.581794 pyassorted-0.7.2/pyassorted/collections/__init__.py
--rw-r--r--   0        0        0     3087 2023-07-08 06:39:42.921979 pyassorted-0.7.2/pyassorted/collections/sqlitedict.py
--rw-r--r--   0        0        0      148 2023-05-15 11:57:33.582436 pyassorted-0.7.2/pyassorted/datetime/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-15 11:57:33.582699 pyassorted-0.7.2/pyassorted/datetime/datetime.py
--rw-r--r--   0        0        0     2013 2023-05-15 11:57:33.582972 pyassorted-0.7.2/pyassorted/datetime/timer.py
--rw-r--r--   0        0        0        0 2023-06-12 12:04:26.629790 pyassorted-0.7.2/pyassorted/encrypt/__init__.py
--rw-r--r--   0        0        0     2257 2023-07-07 10:20:46.735970 pyassorted-0.7.2/pyassorted/encrypt/io.py
--rw-r--r--   0        0        0     2602 2023-05-27 10:25:12.262734 pyassorted-0.7.2/pyassorted/io/__init__.py
--rw-r--r--   0        0        0     2365 2023-05-27 10:25:12.262951 pyassorted-0.7.2/pyassorted/io/watch.py
--rw-r--r--   0        0        0       56 2023-04-01 13:44:09.335149 pyassorted-0.7.2/pyassorted/lock/__init__.py
--rw-r--r--   0        0        0     4191 2023-04-01 13:44:09.335570 pyassorted-0.7.2/pyassorted/lock/filelock.py
--rw-r--r--   0        0        0        0 2023-07-07 10:23:45.350340 pyassorted-0.7.2/pyassorted/standard/__init__.py
--rw-r--r--   0        0        0     2788 2023-07-07 10:57:46.398428 pyassorted-0.7.2/pyassorted/standard/language_code.py
--rw-r--r--   0        0        0      130 2023-06-08 14:19:30.918842 pyassorted-0.7.2/pyassorted/string/__init__.py
--rw-r--r--   0        0        0      269 2023-06-08 14:18:59.300447 pyassorted-0.7.2/pyassorted/string/rand.py
--rw-r--r--   0        0        0     1924 2023-06-06 09:03:20.787667 pyassorted-0.7.2/pyassorted/string/replace.py
--rw-r--r--   0        0        0       18 2023-07-08 06:44:20.848606 pyassorted-0.7.2/pyassorted/version.py
--rw-r--r--   0        0        0      546 2023-07-08 06:42:44.156083 pyassorted-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     7597 1970-01-01 00:00:00.000000 pyassorted-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-15 09:16:45.010069 pyassorted-0.7.3/LICENSE
+-rw-r--r--   0        0        0     6993 2023-05-27 10:25:12.261799 pyassorted-0.7.3/README.md
+-rw-r--r--   0        0        0       53 2023-04-01 13:44:09.334164 pyassorted-0.7.3/pyassorted/__init__.py
+-rw-r--r--   0        0        0      116 2023-02-17 09:28:12.934937 pyassorted-0.7.3/pyassorted/asyncio/__init__.py
+-rw-r--r--   0        0        0     1349 2023-04-01 13:44:09.334680 pyassorted-0.7.3/pyassorted/asyncio/executor.py
+-rw-r--r--   0        0        0     2943 2023-05-15 11:57:33.581730 pyassorted-0.7.3/pyassorted/asyncio/io.py
+-rw-r--r--   0        0        0     1017 2023-02-15 09:50:56.450314 pyassorted-0.7.3/pyassorted/asyncio/utils.py
+-rw-r--r--   0        0        0       61 2023-03-27 15:28:16.228462 pyassorted-0.7.3/pyassorted/cache/__init__.py
+-rw-r--r--   0        0        0     8109 2023-03-27 15:28:16.228823 pyassorted-0.7.3/pyassorted/cache/cache.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:57:33.581794 pyassorted-0.7.3/pyassorted/collections/__init__.py
+-rw-r--r--   0        0        0     3361 2023-07-08 07:11:56.488841 pyassorted-0.7.3/pyassorted/collections/sqlitedict.py
+-rw-r--r--   0        0        0      148 2023-05-15 11:57:33.582436 pyassorted-0.7.3/pyassorted/datetime/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-15 11:57:33.582699 pyassorted-0.7.3/pyassorted/datetime/datetime.py
+-rw-r--r--   0        0        0     2013 2023-05-15 11:57:33.582972 pyassorted-0.7.3/pyassorted/datetime/timer.py
+-rw-r--r--   0        0        0        0 2023-06-12 12:04:26.629790 pyassorted-0.7.3/pyassorted/encrypt/__init__.py
+-rw-r--r--   0        0        0     2257 2023-07-07 10:20:46.735970 pyassorted-0.7.3/pyassorted/encrypt/io.py
+-rw-r--r--   0        0        0     2602 2023-05-27 10:25:12.262734 pyassorted-0.7.3/pyassorted/io/__init__.py
+-rw-r--r--   0        0        0     2365 2023-05-27 10:25:12.262951 pyassorted-0.7.3/pyassorted/io/watch.py
+-rw-r--r--   0        0        0       56 2023-04-01 13:44:09.335149 pyassorted-0.7.3/pyassorted/lock/__init__.py
+-rw-r--r--   0        0        0     4191 2023-04-01 13:44:09.335570 pyassorted-0.7.3/pyassorted/lock/filelock.py
+-rw-r--r--   0        0        0        0 2023-07-07 10:23:45.350340 pyassorted-0.7.3/pyassorted/standard/__init__.py
+-rw-r--r--   0        0        0     2788 2023-07-07 10:57:46.398428 pyassorted-0.7.3/pyassorted/standard/language_code.py
+-rw-r--r--   0        0        0      130 2023-06-08 14:19:30.918842 pyassorted-0.7.3/pyassorted/string/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-08 14:18:59.300447 pyassorted-0.7.3/pyassorted/string/rand.py
+-rw-r--r--   0        0        0     1924 2023-06-06 09:03:20.787667 pyassorted-0.7.3/pyassorted/string/replace.py
+-rw-r--r--   0        0        0       18 2023-07-08 07:15:02.933967 pyassorted-0.7.3/pyassorted/version.py
+-rw-r--r--   0        0        0      546 2023-07-08 07:14:54.454599 pyassorted-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     7597 1970-01-01 00:00:00.000000 pyassorted-0.7.3/PKG-INFO
```

### Comparing `pyassorted-0.7.2/LICENSE` & `pyassorted-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/README.md` & `pyassorted-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/asyncio/executor.py` & `pyassorted-0.7.3/pyassorted/asyncio/executor.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/asyncio/io.py` & `pyassorted-0.7.3/pyassorted/asyncio/io.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/asyncio/utils.py` & `pyassorted-0.7.3/pyassorted/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/cache/cache.py` & `pyassorted-0.7.3/pyassorted/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/collections/sqlitedict.py` & `pyassorted-0.7.3/pyassorted/collections/sqlitedict.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,24 @@
     ...     await sql_dict.async_set("key", "value")
     ...     assert (await sql_dict.async_get("key")) == "value"
     >>>
     >>> asyncio.run(main())
     """
 
     def __init__(
-        self, sqlite_filepath: Text = ":memory:", tablename: Text = "cache", **kwargs
+        self,
+        sqlite_filepath: Text = ":memory:",
+        tablename: Text = "cache",
+        auto_commit: bool = True,
+        **kwargs,
     ):
         self._sqlite_filepath = sqlite_filepath
         self._tablename = tablename
+        self.auto_commit = auto_commit
+
         self._conn = sqlite3.connect(self._sqlite_filepath, check_same_thread=False)
         self._cursor = self._conn.cursor()
         self._cursor.execute(
             f"CREATE TABLE IF NOT EXISTS {self._tablename} (key TEXT PRIMARY KEY, value TEXT)"
         )
         self._conn.commit()
 
@@ -57,14 +63,16 @@
     def __setitem__(self, key: PrimitiveType, value: Any):
         self.validate_key(key=key)
         value_bytes = pickle.dumps(value)
         self._cursor.execute(
             f"INSERT OR REPLACE INTO {self._tablename} (key, value) VALUES (?, ?)",
             (key, value_bytes),
         )
+        if self.auto_commit:
+            self.commit()
 
     def __iter__(self):
         self._cursor.execute(f"SELECT key, value FROM {self._tablename}")
         for row in self._cursor:
             yield (row[0], pickle.loads(row[1]))
 
     def set(self, key: PrimitiveType, value: Any):
@@ -73,19 +81,24 @@
     def get(self, key: PrimitiveType, default: Any = None) -> Any:
         self.validate_key(key=key)
         try:
             return self[key]
         except KeyError:
             return default
 
+    def commit(self):
+        self._conn.commit()
+
     def items(self):
         return self.__iter__()
 
     async def async_set(self, key: PrimitiveType, value: Any):
         await run_func(self.set, key=key, value=value)
+        if self.auto_commit:
+            await run_func(self.commit)
 
     async def async_get(self, key: PrimitiveType):
         return await run_func(self.get, key=key)
 
     def validate_key(self, key: Any, raise_error: bool = True) -> bool:
         if isinstance(key, (str, numbers.Number, None)):
             return True
```

### Comparing `pyassorted-0.7.2/pyassorted/datetime/datetime.py` & `pyassorted-0.7.3/pyassorted/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/datetime/timer.py` & `pyassorted-0.7.3/pyassorted/datetime/timer.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/encrypt/io.py` & `pyassorted-0.7.3/pyassorted/encrypt/io.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/io/__init__.py` & `pyassorted-0.7.3/pyassorted/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/io/watch.py` & `pyassorted-0.7.3/pyassorted/io/watch.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/lock/filelock.py` & `pyassorted-0.7.3/pyassorted/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/standard/language_code.py` & `pyassorted-0.7.3/pyassorted/standard/language_code.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyassorted/string/replace.py` & `pyassorted-0.7.3/pyassorted/string/replace.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.2/pyproject.toml` & `pyassorted-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyassorted"
-version = "0.7.2"
+version = "0.7.3"
 description = "A library has light-weight assorted utils in Prue-Python."
 authors = ["Allen Chou <f1470891079@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1, <4.0.0"
```

### Comparing `pyassorted-0.7.2/PKG-INFO` & `pyassorted-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyassorted
-Version: 0.7.2
+Version: 0.7.3
 Summary: A library has light-weight assorted utils in Prue-Python.
 License: MIT
 Author: Allen Chou
 Author-email: f1470891079@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

