# Comparing `tmp/benimang-0.3.7.tar.gz` & `tmp/benimang-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.3.7.tar", last modified: Thu Jul  6 08:30:31 2023, max compression
+gzip compressed data, was "benimang-0.3.8.tar", last modified: Sat Jul  8 04:04:06 2023, max compression
```

## Comparing `benimang-0.3.7.tar` & `benimang-0.3.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:30:31.855549 benimang-0.3.7/
--rw-rw-rw-   0        0        0       29 2023-05-30 09:18:28.000000 benimang-0.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0      258 2023-07-06 08:30:31.855549 benimang-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 08:30:31.848547 benimang-0.3.7/beni/
--rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.7/beni/__init__.py
--rw-rw-rw-   0        0        0     6350 2023-06-29 02:15:26.000000 benimang-0.3.7/beni/bbyte.py
--rw-rw-rw-   0        0        0     5789 2023-07-05 03:38:40.000000 benimang-0.3.7/beni/bcache.py
--rw-rw-rw-   0        0        0    11460 2023-06-29 07:06:28.000000 benimang-0.3.7/beni/bcmd.py
--rw-rw-rw-   0        0        0     1941 2023-06-09 08:30:18.000000 benimang-0.3.7/beni/bcolor.py
--rw-rw-rw-   0        0        0      436 2023-06-29 07:09:07.000000 benimang-0.3.7/beni/bdefine.py
--rw-rw-rw-   0        0        0     2423 2023-06-26 06:18:37.000000 benimang-0.3.7/beni/bexecute.py
--rw-rw-rw-   0        0        0     1908 2023-06-29 01:45:33.000000 benimang-0.3.7/beni/bfile.py
--rw-rw-rw-   0        0        0     4562 2023-07-06 08:05:26.000000 benimang-0.3.7/beni/bfunc.py
--rw-rw-rw-   0        0        0     1029 2023-06-28 03:38:59.000000 benimang-0.3.7/beni/bhash.py
--rw-rw-rw-   0        0        0     5745 2023-06-26 09:08:25.000000 benimang-0.3.7/beni/bhttp.py
--rw-rw-rw-   0        0        0     2583 2023-06-13 01:57:12.000000 benimang-0.3.7/beni/binput.py
--rw-rw-rw-   0        0        0     5708 2023-06-30 02:08:08.000000 benimang-0.3.7/beni/block.py
--rw-rw-rw-   0        0        0     3989 2023-06-29 01:25:39.000000 benimang-0.3.7/beni/blog.py
--rw-rw-rw-   0        0        0     5790 2023-06-29 01:32:58.000000 benimang-0.3.7/beni/bpath.py
--rw-rw-rw-   0        0        0     2450 2023-06-29 01:26:10.000000 benimang-0.3.7/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1058 2023-06-27 03:17:47.000000 benimang-0.3.7/beni/bprogress.py
--rw-rw-rw-   0        0        0     3373 2023-07-06 08:05:08.000000 benimang-0.3.7/beni/bqiniu.py
--rw-rw-rw-   0        0        0     9866 2023-06-29 01:31:14.000000 benimang-0.3.7/beni/bsqlite.py
--rw-rw-rw-   0        0        0      759 2023-06-29 01:45:35.000000 benimang-0.3.7/beni/bstorage.py
--rw-rw-rw-   0        0        0     1981 2023-06-26 02:57:46.000000 benimang-0.3.7/beni/btable.py
--rw-rw-rw-   0        0        0     4987 2023-07-05 06:44:09.000000 benimang-0.3.7/beni/btask.py
--rw-rw-rw-   0        0        0     1378 2023-06-29 07:10:32.000000 benimang-0.3.7/beni/btime.py
--rw-rw-rw-   0        0        0      324 2023-06-30 02:01:04.000000 benimang-0.3.7/beni/btype.py
--rw-rw-rw-   0        0        0     2392 2023-06-29 02:21:02.000000 benimang-0.3.7/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:30:31.853549 benimang-0.3.7/benimang.egg-info/
--rw-rw-rw-   0        0        0      258 2023-07-06 08:30:31.000000 benimang-0.3.7/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-07-06 08:30:31.000000 benimang-0.3.7/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:30:31.000000 benimang-0.3.7/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-06 08:30:31.000000 benimang-0.3.7/benimang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       93 2023-07-06 08:30:31.000000 benimang-0.3.7/benimang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-06 08:30:31.000000 benimang-0.3.7/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-07-06 08:06:55.000000 benimang-0.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 08:30:31.855549 benimang-0.3.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-06 08:30:31.854549 benimang-0.3.7/test/
--rw-rw-rw-   0        0        0      638 2023-05-30 09:18:28.000000 benimang-0.3.7/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:04:06.036956 benimang-0.3.8/
+-rw-rw-rw-   0        0        0       29 2023-05-30 09:18:28.000000 benimang-0.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      258 2023-07-08 04:04:06.036956 benimang-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 04:04:06.027954 benimang-0.3.8/beni/
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-0.3.8/beni/__init__.py
+-rw-rw-rw-   0        0        0     6350 2023-06-29 02:15:26.000000 benimang-0.3.8/beni/bbyte.py
+-rw-rw-rw-   0        0        0     5789 2023-07-05 03:38:40.000000 benimang-0.3.8/beni/bcache.py
+-rw-rw-rw-   0        0        0    11460 2023-06-29 07:06:28.000000 benimang-0.3.8/beni/bcmd.py
+-rw-rw-rw-   0        0        0     1941 2023-06-09 08:30:18.000000 benimang-0.3.8/beni/bcolor.py
+-rw-rw-rw-   0        0        0      436 2023-06-29 07:09:07.000000 benimang-0.3.8/beni/bdefine.py
+-rw-rw-rw-   0        0        0     2423 2023-07-08 04:02:39.000000 benimang-0.3.8/beni/bexecute.py
+-rw-rw-rw-   0        0        0     1908 2023-06-29 01:45:33.000000 benimang-0.3.8/beni/bfile.py
+-rw-rw-rw-   0        0        0     4562 2023-07-06 08:05:26.000000 benimang-0.3.8/beni/bfunc.py
+-rw-rw-rw-   0        0        0     1029 2023-06-28 03:38:59.000000 benimang-0.3.8/beni/bhash.py
+-rw-rw-rw-   0        0        0     5745 2023-06-26 09:08:25.000000 benimang-0.3.8/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2583 2023-06-13 01:57:12.000000 benimang-0.3.8/beni/binput.py
+-rw-rw-rw-   0        0        0     5708 2023-06-30 02:08:08.000000 benimang-0.3.8/beni/block.py
+-rw-rw-rw-   0        0        0     3989 2023-06-29 01:25:39.000000 benimang-0.3.8/beni/blog.py
+-rw-rw-rw-   0        0        0     5790 2023-06-29 01:32:58.000000 benimang-0.3.8/beni/bpath.py
+-rw-rw-rw-   0        0        0     2450 2023-07-08 04:02:42.000000 benimang-0.3.8/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1058 2023-06-27 03:17:47.000000 benimang-0.3.8/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3373 2023-07-06 08:05:08.000000 benimang-0.3.8/beni/bqiniu.py
+-rw-rw-rw-   0        0        0     9866 2023-07-08 04:03:05.000000 benimang-0.3.8/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      759 2023-06-29 01:45:35.000000 benimang-0.3.8/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1981 2023-06-26 02:57:46.000000 benimang-0.3.8/beni/btable.py
+-rw-rw-rw-   0        0        0     4987 2023-07-05 06:44:09.000000 benimang-0.3.8/beni/btask.py
+-rw-rw-rw-   0        0        0     1378 2023-06-29 07:10:32.000000 benimang-0.3.8/beni/btime.py
+-rw-rw-rw-   0        0        0      324 2023-06-30 02:01:04.000000 benimang-0.3.8/beni/btype.py
+-rw-rw-rw-   0        0        0     2392 2023-06-29 02:21:02.000000 benimang-0.3.8/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:04:06.034956 benimang-0.3.8/benimang.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-08 04:04:05.000000 benimang-0.3.8/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-07-08 04:03:36.000000 benimang-0.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 04:04:06.037957 benimang-0.3.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 04:04:06.035956 benimang-0.3.8/test/
+-rw-rw-rw-   0        0        0      638 2023-05-30 09:18:28.000000 benimang-0.3.8/test/test_sample.py
```

### Comparing `benimang-0.3.7/beni/bbyte.py` & `benimang-0.3.8/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bcache.py` & `benimang-0.3.8/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bcmd.py` & `benimang-0.3.8/beni/bcmd.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bcolor.py` & `benimang-0.3.8/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bexecute.py` & `benimang-0.3.8/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bfile.py` & `benimang-0.3.8/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bfunc.py` & `benimang-0.3.8/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bhash.py` & `benimang-0.3.8/beni/bhash.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bhttp.py` & `benimang-0.3.8/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/binput.py` & `benimang-0.3.8/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/block.py` & `benimang-0.3.8/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/blog.py` & `benimang-0.3.8/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bpath.py` & `benimang-0.3.8/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bplaywright.py` & `benimang-0.3.8/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bprogress.py` & `benimang-0.3.8/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bqiniu.py` & `benimang-0.3.8/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bsqlite.py` & `benimang-0.3.8/beni/bsqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         async with self.write() as db:
             return await db.update(table, data, statement, *args)
 
     async def get(self, sql: str, *args: Any):
         async with self.read() as db:
             return await db.get(sql, *args)
 
-    async def getList(self, sql: str, *args: Any):
+    async def get_ary(self, sql: str, *args: Any):
         async with self.read() as db:
             return await db.get_ary(sql, *args)
 
     async def value(self, sql: str, *args: Any):
         async with self.read() as db:
             return await db.value(sql, *args)
 
@@ -313,15 +313,15 @@
             *args,
         )
         if row:
             return cls(**dict(row))
 
     @classmethod
     async def _get_ary(cls, statement: str = '', *args: Any, fields: set[str] | None = None):
-        rows = await cls._db.getList(
+        rows = await cls._db.get_ary(
             f'''
             SELECT
                 {fields and ', '.join(fields) or '*'}
             FROM
                 `{cls.TABLE}`
             {statement}
             ''',
```

### Comparing `benimang-0.3.7/beni/bstorage.py` & `benimang-0.3.8/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/btable.py` & `benimang-0.3.8/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/btask.py` & `benimang-0.3.8/beni/btask.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/btime.py` & `benimang-0.3.8/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/beni/bzip.py` & `benimang-0.3.8/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/benimang.egg-info/SOURCES.txt` & `benimang-0.3.8/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benimang-0.3.7/pyproject.toml` & `benimang-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://peps.python.org/pep-0621/#example
 
 [project]
 name = "benimang"
-version = "0.3.7"
+version = "0.3.8"
 description = "utils library for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni"]
 authors = [
   {email = "benimang@126.com"},
   {name = "Beni Mang"}
 ]
```

### Comparing `benimang-0.3.7/test/test_sample.py` & `benimang-0.3.8/test/test_sample.py`

 * *Files identical despite different names*

