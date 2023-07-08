# Comparing `tmp/themis_imager_readfile-1.2.2.tar.gz` & `tmp/themis_imager_readfile-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themis_imager_readfile-1.2.2.tar", max compression
+gzip compressed data, was "themis_imager_readfile-1.2.3.tar", max compression
```

## Comparing `themis_imager_readfile-1.2.2.tar` & `themis_imager_readfile-1.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.2.2/LICENSE
--rw-r--r--   0        0        0     2763 2023-05-15 18:17:56.997619 themis_imager_readfile-1.2.2/README.md
--rw-r--r--   0        0        0      666 2023-06-01 19:09:36.235074 themis_imager_readfile-1.2.2/pyproject.toml
--rw-r--r--   0        0        0       49 2023-06-01 19:09:36.268075 themis_imager_readfile-1.2.2/themis_imager_readfile/__init__.py
--rw-r--r--   0        0        0     9408 2023-06-01 19:13:29.828869 themis_imager_readfile-1.2.2/themis_imager_readfile/_themis.py
--rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 themis_imager_readfile-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.2.3/LICENSE
+-rw-r--r--   0        0        0     3024 2023-06-01 19:32:23.797257 themis_imager_readfile-1.2.3/README.md
+-rw-r--r--   0        0        0      666 2023-07-08 17:01:00.200056 themis_imager_readfile-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-07-08 17:01:00.227056 themis_imager_readfile-1.2.3/themis_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     9432 2023-07-08 17:01:12.764308 themis_imager_readfile-1.2.3/themis_imager_readfile/_themis.py
+-rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 themis_imager_readfile-1.2.3/PKG-INFO
```

### Comparing `themis_imager_readfile-1.2.2/LICENSE` & `themis_imager_readfile-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.2.2/README.md` & `themis_imager_readfile-1.2.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,22 @@
 
 ```python
 >>> import themis_imager_readfile, glob
 >>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
 >>> img, meta, problematic_files = themis_imager_readfile.read(file_list, workers=4)
 ```
 
+### Read with no output
+
+```python
+>>> import themis_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
+>>> img, meta, problematic_files = themis_imager_readfile.read(file_list, workers=4, quiet=True)
+```
+
 ## Development
 
 Clone the repository and install dependencies using Poetry.
 
 ```console
 $ git clone https://github.com/ucalgary-aurora/themis-imager-readfile.git
 $ cd themis-imager-readfile/python
```

### Comparing `themis_imager_readfile-1.2.2/pyproject.toml` & `themis_imager_readfile-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "themis-imager-readfile"
-version = "1.2.2"
+version = "1.2.3"
 description = "Read functions for THEMIS ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `themis_imager_readfile-1.2.2/themis_imager_readfile/_themis.py` & `themis_imager_readfile-1.2.3/themis_imager_readfile/_themis.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         try:
             data = pool.map(partial(__themis_readfile_worker, quiet=quiet), file_list)
         except KeyboardInterrupt:
             pool.terminate()  # gracefully kill children
             return np.empty((0, 0, 0), dtype=THEMIS_DT), [], []
         else:
             pool.close()
+            pool.join()
     else:
         # don't bother using multiprocessing with one worker, just call the worker function directly
         data = []
         for f in file_list:
             data.append(__themis_readfile_worker(f, quiet=quiet))
 
     # derive number of frames to prepare for
```

### Comparing `themis_imager_readfile-1.2.2/PKG-INFO` & `themis_imager_readfile-1.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themis-imager-readfile
-Version: 1.2.2
+Version: 1.2.3
 Summary: Read functions for THEMIS ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/themis-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -71,14 +71,22 @@
 
 ```python
 >>> import themis_imager_readfile, glob
 >>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
 >>> img, meta, problematic_files = themis_imager_readfile.read(file_list, workers=4)
 ```
 
+### Read with no output
+
+```python
+>>> import themis_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
+>>> img, meta, problematic_files = themis_imager_readfile.read(file_list, workers=4, quiet=True)
+```
+
 ## Development
 
 Clone the repository and install dependencies using Poetry.
 
 ```console
 $ git clone https://github.com/ucalgary-aurora/themis-imager-readfile.git
 $ cd themis-imager-readfile/python
```

