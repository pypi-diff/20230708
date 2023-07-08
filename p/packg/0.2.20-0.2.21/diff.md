# Comparing `tmp/packg-0.2.20.tar.gz` & `tmp/packg-0.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.2.20.tar", last modified: Fri Jul  7 09:16:06 2023, max compression
+gzip compressed data, was "packg-0.2.21.tar", last modified: Sat Jul  8 13:02:24 2023, max compression
```

## Comparing `packg-0.2.20.tar` & `packg-0.2.21.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 09:16:06.216212 packg-0.2.20/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.20/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-07 09:16:06.216212 packg-0.2.20/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-07-07 09:15:31.000000 packg-0.2.20/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.20/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-07 09:15:31.000000 packg-0.2.20/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-07-07 09:16:06.216212 packg-0.2.20/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 09:16:06.088209 packg-0.2.20/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 09:16:06.164211 packg-0.2.20/src/packg/
--rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5770 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/constclass.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      530 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/debugging.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/dtime.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     8349 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/import_from_source.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 09:16:06.208211 packg-0.2.20/src/packg/iotools/
--rw-------   0 gings    (14999) lmb-mit   (1061)      592 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/iotools/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/iotools/compressed.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/iotools/gitmatcher.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/iotools/jsonext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/iotools/jsonext_encoder.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3779 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/iotools/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4840 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/iotools/yamlext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5493 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/paths.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 09:16:06.212211 packg-0.2.20/src/packg/run/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3522 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/run/syncjupytext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5464 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/strings.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/system.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/tensors.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-07-07 09:15:31.000000 packg-0.2.20/src/packg/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 09:16:06.188211 packg-0.2.20/src/packg.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-07 09:16:06.000000 packg-0.2.20/src/packg.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      763 2023-07-07 09:16:06.000000 packg-0.2.20/src/packg.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-07-07 09:16:06.000000 packg-0.2.20/src/packg.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-07 09:16:06.000000 packg-0.2.20/src/packg.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-07-07 09:16:06.000000 packg-0.2.20/src/packg.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.20/src/packg.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.741776 packg-0.2.21/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.21/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-08 13:02:24.741776 packg-0.2.21/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-07-07 09:15:31.000000 packg-0.2.21/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.21/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-07 09:15:31.000000 packg-0.2.21/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-07-08 13:02:24.745776 packg-0.2.21/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.557773 packg-0.2.21/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.641774 packg-0.2.21/src/packg/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-07-08 13:01:40.000000 packg-0.2.21/src/packg/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5770 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/constclass.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      530 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/debugging.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/dtime.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     8349 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/import_from_source.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.729776 packg-0.2.21/src/packg/iotools/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      707 2023-07-08 13:01:40.000000 packg-0.2.21/src/packg/iotools/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/iotools/compressed.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/iotools/gitmatcher.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/iotools/jsonext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/iotools/jsonext_encoder.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4014 2023-07-08 13:01:40.000000 packg-0.2.21/src/packg/iotools/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4840 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/iotools/yamlext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5493 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/paths.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.733776 packg-0.2.21/src/packg/run/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3522 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/run/syncjupytext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5464 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/strings.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/system.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/tensors.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.685775 packg-0.2.21/src/packg.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-08 13:02:24.000000 packg-0.2.21/src/packg.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      763 2023-07-08 13:02:24.000000 packg-0.2.21/src/packg.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-07-08 13:02:24.000000 packg-0.2.21/src/packg.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-08 13:02:24.000000 packg-0.2.21/src/packg.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-07-08 13:02:24.000000 packg-0.2.21/src/packg.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.21/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.2.20/LICENSE` & `packg-0.2.21/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/PKG-INFO` & `packg-0.2.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.20
+Version: 0.2.21
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.20 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.21 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.20/README.md` & `packg-0.2.21/README.md`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/pyproject.toml` & `packg-0.2.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/caching.py` & `packg-0.2.21/src/packg/caching.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/constclass.py` & `packg-0.2.21/src/packg/constclass.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/debugging.py` & `packg-0.2.21/src/packg/debugging.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/import_from_source.py` & `packg-0.2.21/src/packg/import_from_source.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/iotools/jsonext.py` & `packg-0.2.21/src/packg/iotools/jsonext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/iotools/jsonext_encoder.py` & `packg-0.2.21/src/packg/iotools/jsonext_encoder.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/iotools/misc.py` & `packg-0.2.21/src/packg/iotools/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,43 +58,56 @@
         bytes content
     """
     if isinstance(file_or_io, PathTypeCls):
         return Path(file_or_io).read_bytes()
     return file_or_io.read()
 
 
-def yield_nonempty_stripped_lines(lines_obj: Union[Iterable, str, TextIO]) -> Iterable[str]:
+def yield_chunked_bytes(file_or_io: PathOrIO, chunk_size=1024 * 1024) -> Iterable[bytes]:
+    """
+
+    Args:
+        file_or_io: file name or open file-like object
+        chunk_size: chunk size in bytes, default 1MB
+
+    Returns:
+        bytes content
+    """
+    with open_file_or_io(file_or_io, mode="rb") as fh:
+        while True:
+            data = fh.read(chunk_size)
+            if len(data) == 0:
+                break
+            yield data
+
+
+def yield_nonempty_stripped_lines(lines_obj: Union[PathOrIO, Iterable[str]]) -> Iterable[str]:
     """
     Read lines from input, strip whitespaces, skip empty lines, yield lines.
 
     Args:
-        lines_obj: Can be an iterable of str (list, opened file) or
-            a str that will be split at newlines.
+        lines_obj: Can be any of:
+            - iterable of str (list, opened file)
+            - filepath str or Path
 
     Returns:
         Generator of stripped lines
 
     Examples:
         >>> for li in yield_nonempty_stripped_lines(["  a  ", "  ", "  b  "]): print(li, end=",")
         a,b,
     """
     if isinstance(lines_obj, str):
         lines_obj = lines_obj.splitlines()
-    for line in lines_obj:
-        line = line.strip()
-        if line == "":
-            continue
-        yield line
-
-
-def yield_nonempty_stripped_lines_from_file(
-        file_path: PathType, encoding: str = "utf-8") -> Iterable[str]:
-    """Same as above, but for filenames."""
-    with Path(file_path).open("r", encoding=encoding) as fh:
-        yield from yield_nonempty_stripped_lines(fh)
+    with open_file_or_io(lines_obj) as fh:
+        for line in fh:
+            line = line.strip()
+            if line == "":
+                continue
+            yield line
 
 
 def sort_file_paths_with_dirs_separated(
         file_paths: List[PathType], natsorted: bool = False,
         dirs_first: bool = True) -> List[Path]:
     """
     Sort a list of file paths, separating files inside subdirectories from files in the root.
```

### Comparing `packg-0.2.20/src/packg/iotools/yamlext.py` & `packg-0.2.21/src/packg/iotools/yamlext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/log.py` & `packg-0.2.21/src/packg/log.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/paths.py` & `packg-0.2.21/src/packg/paths.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/run/syncjupytext.py` & `packg-0.2.21/src/packg/run/syncjupytext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/strings.py` & `packg-0.2.21/src/packg/strings.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/system.py` & `packg-0.2.21/src/packg/system.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/tensors.py` & `packg-0.2.21/src/packg/tensors.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg/typext.py` & `packg-0.2.21/src/packg/typext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.20/src/packg.egg-info/PKG-INFO` & `packg-0.2.21/src/packg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.20
+Version: 0.2.21
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.20 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.21 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.20/src/packg.egg-info/SOURCES.txt` & `packg-0.2.21/src/packg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

