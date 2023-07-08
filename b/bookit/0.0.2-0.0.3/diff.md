# Comparing `tmp/bookit-0.0.2.tar.gz` & `tmp/bookit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookit-0.0.2.tar", last modified: Sat Jul  8 19:35:08 2023, max compression
+gzip compressed data, was "bookit-0.0.3.tar", last modified: Sat Jul  8 19:45:48 2023, max compression
```

## Comparing `bookit-0.0.2.tar` & `bookit-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-08 19:35:08.164428 bookit-0.0.2/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1068 2023-07-08 19:21:27.000000 bookit-0.0.2/LICENSE
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      197 2023-07-08 19:21:27.000000 bookit-0.0.2/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2155 2023-07-08 19:35:08.164428 bookit-0.0.2/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-07-08 19:10:41.000000 bookit-0.0.2/README.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-08 19:35:08.164428 bookit-0.0.2/bookit/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-07-08 19:34:57.000000 bookit-0.0.2/bookit/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       89 2023-07-08 19:16:02.000000 bookit-0.0.2/bookit/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2495 2023-07-08 19:16:02.000000 bookit-0.0.2/bookit/bookit.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      801 2023-07-08 19:16:02.000000 bookit-0.0.2/bookit/cli.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-08 19:35:08.164428 bookit-0.0.2/bookit.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2155 2023-07-08 19:35:08.000000 bookit-0.0.2/bookit.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      299 2023-07-08 19:35:08.000000 bookit-0.0.2/bookit.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-07-08 19:35:08.000000 bookit-0.0.2/bookit.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       24 2023-07-08 19:35:08.000000 bookit-0.0.2/bookit.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        7 2023-07-08 19:35:08.000000 bookit-0.0.2/bookit.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      403 2023-07-08 19:35:08.164428 bookit-0.0.2/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      918 2023-07-08 19:34:57.000000 bookit-0.0.2/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-08 19:35:08.164428 bookit-0.0.2/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-07-07 19:40:00.000000 bookit-0.0.2/tests/.gitkeep
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-07-08 19:17:02.000000 bookit-0.0.2/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-08 19:45:48.300063 bookit-0.0.3/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1068 2023-07-08 19:21:27.000000 bookit-0.0.3/LICENSE
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      197 2023-07-08 19:21:27.000000 bookit-0.0.3/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2155 2023-07-08 19:45:48.300063 bookit-0.0.3/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-07-08 19:10:41.000000 bookit-0.0.3/README.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-08 19:45:48.300063 bookit-0.0.3/bookit/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-07-08 19:45:40.000000 bookit-0.0.3/bookit/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       89 2023-07-08 19:16:02.000000 bookit-0.0.3/bookit/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2610 2023-07-08 19:44:44.000000 bookit-0.0.3/bookit/bookit.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      801 2023-07-08 19:16:02.000000 bookit-0.0.3/bookit/cli.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-08 19:45:48.300063 bookit-0.0.3/bookit.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     2155 2023-07-08 19:45:48.000000 bookit-0.0.3/bookit.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      299 2023-07-08 19:45:48.000000 bookit-0.0.3/bookit.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-07-08 19:45:48.000000 bookit-0.0.3/bookit.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       24 2023-07-08 19:45:48.000000 bookit-0.0.3/bookit.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        7 2023-07-08 19:45:48.000000 bookit-0.0.3/bookit.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      403 2023-07-08 19:45:48.300063 bookit-0.0.3/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      918 2023-07-08 19:45:40.000000 bookit-0.0.3/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-07-08 19:45:48.300063 bookit-0.0.3/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-07-07 19:40:00.000000 bookit-0.0.3/tests/.gitkeep
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-07-08 19:17:02.000000 bookit-0.0.3/tests/__init__.py
```

### Comparing `bookit-0.0.2/LICENSE` & `bookit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bookit-0.0.2/PKG-INFO` & `bookit-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Doc site generator
 Home-page: https://github.com/agmoss/bookit
 Author: Andrew Moss
 Author-email: andrew@m0ss.dev
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bookit-0.0.2/README.md` & `bookit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bookit-0.0.2/bookit/bookit.py` & `bookit-0.0.3/bookit/bookit.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,17 @@
         ):
             continue
 
         file_path = os.path.join(dirpath, filename)
         new_dir = dirpath.replace(repo_path, book_path, 1)
 
         if filename.endswith(".md"):
+            # TODO: Refactor this
+            if not os.path.exists(new_dir):
+                os.makedirs(new_dir)
             new_file_path = os.path.join(new_dir, filename)
             shutil.copy(file_path, new_file_path)
             continue
 
         new_file_path = os.path.join(new_dir, f"{filename}.md")
 
         if not os.path.exists(new_dir):
```

### Comparing `bookit-0.0.2/bookit/cli.py` & `bookit-0.0.3/bookit/cli.py`

 * *Files identical despite different names*

### Comparing `bookit-0.0.2/bookit.egg-info/PKG-INFO` & `bookit-0.0.3/bookit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Doc site generator
 Home-page: https://github.com/agmoss/bookit
 Author: Andrew Moss
 Author-email: andrew@m0ss.dev
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bookit-0.0.2/setup.py` & `bookit-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Andrew Moss",
     author_email="andrew@m0ss.dev",
     python_requires=">=3.7",
     name="bookit",
-    version="0.0.2",
+    version="0.0.3",
     description="Doc site generator",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

