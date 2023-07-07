# Comparing `tmp/audio_separator-0.3.1.tar.gz` & `tmp/audio_separator-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.3.1.tar", max compression
+gzip compressed data, was "audio_separator-0.3.2.tar", max compression
```

## Comparing `audio_separator-0.3.1.tar` & `audio_separator-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-30 05:57:58.913442 audio_separator-0.3.1/LICENSE
--rw-r--r--   0        0        0     6659 2023-07-02 02:44:13.948375 audio_separator-0.3.1/README.md
--rw-r--r--   0        0        0       33 2023-06-30 18:38:54.200542 audio_separator-0.3.1/audio_separator/__init__.py
--rw-r--r--   0        0        0    11878 2023-07-07 18:49:58.574514 audio_separator-0.3.1/audio_separator/separator.py
--rw-r--r--   0        0        0        0 2023-06-30 05:58:37.414385 audio_separator-0.3.1/audio_separator/utils/__init__.py
--rwxr-xr-x   0        0        0     2241 2023-07-07 19:01:19.825510 audio_separator-0.3.1/audio_separator/utils/cli.py
--rw-r--r--   0        0        0    21906 2023-07-07 18:41:58.680039 audio_separator-0.3.1/audio_separator/utils/spec_utils.py
--rw-r--r--   0        0        0      760 2023-07-07 17:27:08.214286 audio_separator-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7480 1970-01-01 00:00:00.000000 audio_separator-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-07 19:33:30.805769 audio_separator-0.3.2/LICENSE
+-rw-r--r--   0        0        0     7203 2023-07-07 19:33:30.805769 audio_separator-0.3.2/README.md
+-rw-r--r--   0        0        0       33 2023-07-07 19:33:30.805769 audio_separator-0.3.2/audio_separator/__init__.py
+-rw-r--r--   0        0        0    11878 2023-07-07 19:33:30.805769 audio_separator-0.3.2/audio_separator/separator.py
+-rw-r--r--   0        0        0        0 2023-07-07 19:33:30.805769 audio_separator-0.3.2/audio_separator/utils/__init__.py
+-rwxr-xr-x   0        0        0     2241 2023-07-07 19:33:30.805769 audio_separator-0.3.2/audio_separator/utils/cli.py
+-rw-r--r--   0        0        0    21906 2023-07-07 19:33:30.805769 audio_separator-0.3.2/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0      760 2023-07-07 19:33:30.805769 audio_separator-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8024 1970-01-01 00:00:00.000000 audio_separator-0.3.2/PKG-INFO
```

### Comparing `audio_separator-0.3.1/LICENSE` & `audio_separator-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.3.1/README.md` & `audio_separator-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 ```sh
 audio-separator [audio_file] --model_name [model_name]
     
     audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
     model_name: (Optional) The name of the model to use for separation. Default: UVR_MDXNET_KARA_2
     model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
     output_dir: (Optional) The directory where the separated files will be saved. If not specified, outputs to current dir.
+    use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
+    log_level: (Optional) The log level. Default: logging.DEBUG
+    log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 ```
 
 Example:
 
 ```
 audio-separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
 ```
@@ -65,14 +68,17 @@
 
 ## Parameters for the Separator class
 
 - audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
 - model_name: (Optional) The name of the model to use for separation. Defaults to 'UVR_MDXNET_KARA_2', a very powerful model for Karaoke instrumental tracks.
 - model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
 - output_dir: (Optional) Directory where the separated files will be saved. If not specified, outputs to current dir.
+- use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
+- log_level: (Optional) The log level. Default: logging.DEBUG
+- log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 
 ## Requirements 📋
 
 Python <= 3.10 (one of the dependencies doesn't like 3.11 yet)
 
 Libraries: onnx, onnxruntime, numpy, soundfile, librosa, torch, wget, six
```

### Comparing `audio_separator-0.3.1/audio_separator/separator.py` & `audio_separator-0.3.2/audio_separator/separator.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.3.1/audio_separator/utils/cli.py` & `audio_separator-0.3.2/audio_separator/utils/cli.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.3.1/audio_separator/utils/spec_utils.py` & `audio_separator-0.3.2/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.3.1/pyproject.toml` & `audio_separator-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "audio-separator"
-version = "0.3.1"
+version = "0.3.2"
 description = "Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "audio_separator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `audio_separator-0.3.1/PKG-INFO` & `audio_separator-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.3.1
+Version: 0.3.2
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -54,14 +54,17 @@
 ```sh
 audio-separator [audio_file] --model_name [model_name]
     
     audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
     model_name: (Optional) The name of the model to use for separation. Default: UVR_MDXNET_KARA_2
     model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
     output_dir: (Optional) The directory where the separated files will be saved. If not specified, outputs to current dir.
+    use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
+    log_level: (Optional) The log level. Default: logging.DEBUG
+    log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 ```
 
 Example:
 
 ```
 audio-separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
 ```
@@ -87,14 +90,17 @@
 
 ## Parameters for the Separator class
 
 - audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
 - model_name: (Optional) The name of the model to use for separation. Defaults to 'UVR_MDXNET_KARA_2', a very powerful model for Karaoke instrumental tracks.
 - model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
 - output_dir: (Optional) Directory where the separated files will be saved. If not specified, outputs to current dir.
+- use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
+- log_level: (Optional) The log level. Default: logging.DEBUG
+- log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 
 ## Requirements 📋
 
 Python <= 3.10 (one of the dependencies doesn't like 3.11 yet)
 
 Libraries: onnx, onnxruntime, numpy, soundfile, librosa, torch, wget, six
```

