# Comparing `tmp/audio_separator-0.3.3.tar.gz` & `tmp/audio_separator-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.3.3.tar", max compression
+gzip compressed data, was "audio_separator-0.3.4.tar", max compression
```

## Comparing `audio_separator-0.3.3.tar` & `audio_separator-0.3.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-07 22:33:34.268273 audio_separator-0.3.3/LICENSE
--rw-r--r--   0        0        0     7239 2023-07-07 22:33:34.268273 audio_separator-0.3.3/README.md
--rw-r--r--   0        0        0       33 2023-07-07 22:33:34.268273 audio_separator-0.3.3/audio_separator/__init__.py
--rw-r--r--   0        0        0    11878 2023-07-07 22:33:34.268273 audio_separator-0.3.3/audio_separator/separator.py
--rw-r--r--   0        0        0        0 2023-07-07 22:33:34.268273 audio_separator-0.3.3/audio_separator/utils/__init__.py
--rwxr-xr-x   0        0        0     2333 2023-07-07 22:33:34.268273 audio_separator-0.3.3/audio_separator/utils/cli.py
--rw-r--r--   0        0        0    21906 2023-07-07 22:33:34.268273 audio_separator-0.3.3/audio_separator/utils/spec_utils.py
--rw-r--r--   0        0        0      760 2023-07-07 22:33:34.272273 audio_separator-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     8060 1970-01-01 00:00:00.000000 audio_separator-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-07 23:30:53.386155 audio_separator-0.3.4/LICENSE
+-rw-r--r--   0        0        0     7239 2023-07-07 23:30:53.386155 audio_separator-0.3.4/README.md
+-rw-r--r--   0        0        0       33 2023-07-07 23:30:53.386155 audio_separator-0.3.4/audio_separator/__init__.py
+-rw-r--r--   0        0        0    11986 2023-07-07 23:30:53.390156 audio_separator-0.3.4/audio_separator/separator.py
+-rw-r--r--   0        0        0        0 2023-07-07 23:30:53.390156 audio_separator-0.3.4/audio_separator/utils/__init__.py
+-rwxr-xr-x   0        0        0     2333 2023-07-07 23:30:53.390156 audio_separator-0.3.4/audio_separator/utils/cli.py
+-rw-r--r--   0        0        0    21906 2023-07-07 23:30:53.390156 audio_separator-0.3.4/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0      760 2023-07-07 23:30:53.390156 audio_separator-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     8060 1970-01-01 00:00:00.000000 audio_separator-0.3.4/PKG-INFO
```

### Comparing `audio_separator-0.3.3/LICENSE` & `audio_separator-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.3.3/README.md` & `audio_separator-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `audio_separator-0.3.3/audio_separator/separator.py` & `audio_separator-0.3.4/audio_separator/separator.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,24 @@
         output_dir=None,
         use_cuda=False,
         log_level=logging.DEBUG,
         log_formatter=None,
     ):
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)
+        self.log_level = log_level
+        self.log_formatter = log_formatter
 
-        log_handler = logging.StreamHandler()
+        self.log_handler = logging.StreamHandler()
 
-        if log_formatter is None:
-            log_formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(module)s - %(message)s")
+        if self.log_formatter is None:
+            self.log_formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(module)s - %(message)s")
 
-        log_handler.setFormatter(log_formatter)
-        self.logger.addHandler(log_handler)
+        self.log_handler.setFormatter(self.log_formatter)
+        self.logger.addHandler(self.log_handler)
 
         self.logger.debug(
             f"Separator instantiating with input file: {audio_file_path}, model_name: {model_name}, output_dir: {output_dir}, use_cuda: {use_cuda}"
         )
 
         self.model_name = model_name
         self.model_file_dir = model_file_dir
```

### Comparing `audio_separator-0.3.3/audio_separator/utils/cli.py` & `audio_separator-0.3.4/audio_separator/utils/cli.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.3.3/audio_separator/utils/spec_utils.py` & `audio_separator-0.3.4/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.3.3/pyproject.toml` & `audio_separator-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "audio-separator"
-version = "0.3.3"
+version = "0.3.4"
 description = "Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "audio_separator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `audio_separator-0.3.3/PKG-INFO` & `audio_separator-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.3.3
+Version: 0.3.4
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

