# Comparing `tmp/textsum-0.1.5.tar.gz` & `tmp/textsum-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textsum-0.1.5.tar", last modified: Tue Jan 31 04:12:31 2023, max compression
+gzip compressed data, was "textsum-0.2.0.tar", last modified: Sat Jul  8 01:11:23 2023, max compression
```

## Comparing `textsum-0.1.5.tar` & `textsum-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 04:12:31.563733 textsum-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 04:12:31.559733 textsum-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 04:12:31.563733 textsum-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-31 04:12:19.000000 textsum-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-01-31 04:12:19.000000 textsum-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-31 04:12:19.000000 textsum-0.1.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-01-31 04:12:19.000000 textsum-0.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-01-31 04:12:19.000000 textsum-0.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-31 04:12:19.000000 textsum-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-01-31 04:12:31.563733 textsum-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-01-31 04:12:19.000000 textsum-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-31 04:12:19.000000 textsum-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-31 04:12:31.567733 textsum-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-31 04:12:19.000000 textsum-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 04:12:31.559733 textsum-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 04:12:31.563733 textsum-0.1.5/src/textsum/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-31 04:12:19.000000 textsum-0.1.5/src/textsum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-01-31 04:12:19.000000 textsum-0.1.5/src/textsum/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-01-31 04:12:19.000000 textsum-0.1.5/src/textsum/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-01-31 04:12:19.000000 textsum-0.1.5/src/textsum/pdf2text.py
--rw-r--r--   0 runner    (1001) docker     (123)    17585 2023-01-31 04:12:19.000000 textsum-0.1.5/src/textsum/summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-01-31 04:12:19.000000 textsum-0.1.5/src/textsum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 04:12:31.563733 textsum-0.1.5/src/textsum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-01-31 04:12:31.000000 textsum-0.1.5/src/textsum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-01-31 04:12:31.000000 textsum-0.1.5/src/textsum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 04:12:31.000000 textsum-0.1.5/src/textsum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-31 04:12:31.000000 textsum-0.1.5/src/textsum.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 04:12:31.000000 textsum-0.1.5/src/textsum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-31 04:12:31.000000 textsum-0.1.5/src/textsum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-31 04:12:31.000000 textsum-0.1.5/src/textsum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-01-31 04:12:19.000000 textsum-0.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:11:23.800959 textsum-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:11:23.796959 textsum-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:11:23.796959 textsum-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-08 01:11:09.000000 textsum-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-08 01:11:09.000000 textsum-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-08 01:11:09.000000 textsum-0.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-08 01:11:09.000000 textsum-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-07-08 01:11:09.000000 textsum-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 01:11:09.000000 textsum-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-07-08 01:11:23.800959 textsum-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-08 01:11:09.000000 textsum-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-08 01:11:09.000000 textsum-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-08 01:11:23.800959 textsum-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-08 01:11:09.000000 textsum-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:11:23.796959 textsum-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:11:23.800959 textsum-0.2.0/src/textsum/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-08 01:11:09.000000 textsum-0.2.0/src/textsum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-08 01:11:09.000000 textsum-0.2.0/src/textsum/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-08 01:11:09.000000 textsum-0.2.0/src/textsum/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-08 01:11:09.000000 textsum-0.2.0/src/textsum/pdf2text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21964 2023-07-08 01:11:09.000000 textsum-0.2.0/src/textsum/summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-08 01:11:09.000000 textsum-0.2.0/src/textsum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:11:23.800959 textsum-0.2.0/src/textsum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-07-08 01:11:23.000000 textsum-0.2.0/src/textsum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-08 01:11:23.000000 textsum-0.2.0/src/textsum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:11:23.000000 textsum-0.2.0/src/textsum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-08 01:11:23.000000 textsum-0.2.0/src/textsum.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:11:23.000000 textsum-0.2.0/src/textsum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-08 01:11:23.000000 textsum-0.2.0/src/textsum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 01:11:23.000000 textsum-0.2.0/src/textsum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-08 01:11:09.000000 textsum-0.2.0/tox.ini
```

### Comparing `textsum-0.1.5/.github/workflows/python-publish.yml` & `textsum-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `textsum-0.1.5/.gitignore` & `textsum-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `textsum-0.1.5/CONTRIBUTING.md` & `textsum-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `textsum-0.1.5/LICENSE` & `textsum-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textsum-0.1.5/setup.cfg` & `textsum-0.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -17,37 +17,40 @@
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
+python_requires = >=3.8
 install_requires = 
 	importlib-metadata; python_version<"3.8"
+	accelerate
 	clean-text
+	fire
 	natsort
 	nltk
 	torch
 	tqdm
 	transformers>=4.26.0
-	accelerate
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 8bit = bitsandbytes
-optimum = optimum
+optimum = optimum[onnxruntime,exporters]
 PDF = 
 	python-doctr[torch]
 	pyspellchecker
 app = 
 	gradio
+	rapidfuzz==2.13.7
 	%(PDF)s
 all = 
 	%(app)s
 	%(optimum)s
 	%(8bit)s
 unidecode = unidecode
 testing =
```

### Comparing `textsum-0.1.5/setup.py` & `textsum-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `textsum-0.1.5/src/textsum/__init__.py` & `textsum-0.2.0/src/textsum/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """
 import sys
 
 from . import summarize, utils
 
 if sys.version_info[:2] >= (3, 8):
-    # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
+    # Import directly (no need for conditional) when `python_requires = >= 3.8`
     from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 else:
     from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
 
 try:
     # Change here if project is renamed and does not equal the package name
     dist_name = __name__
```

### Comparing `textsum-0.1.5/src/textsum/app.py` & `textsum-0.2.0/src/textsum/app.py`

 * *Files identical despite different names*

### Comparing `textsum-0.1.5/src/textsum/pdf2text.py` & `textsum-0.2.0/src/textsum/pdf2text.py`

 * *Files identical despite different names*

### Comparing `textsum-0.1.5/src/textsum/summarize.py` & `textsum-0.2.0/src/textsum/summarize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,76 @@
 """
 summarize.py - a module that contains functions for summarizing text
 """
 import json
 import logging
+import sys
 import warnings
+import pprint as pp
 from pathlib import Path
 
 import torch
 from cleantext import clean
 from tqdm.auto import tqdm
 from transformers import AutoModelForSeq2SeqLM, AutoTokenizer
 
+import textsum
 from textsum.utils import (
     check_bitsandbytes_available,
     get_timestamp,
     postprocess_booksummary,
+    validate_pytorch2,
 )
 
 
 class Summarizer:
     """
-    Summarizer - a class that contains functions for summarizing text with a transformers model
+    Summarizer - utility class for summarizing long text using a pretrained model
     """
 
+    settable_inference_params = [
+        "min_length",
+        "max_length",
+        "no_repeat_ngram_size",
+        "encoder_no_repeat_ngram_size",
+        "repetition_penalty",
+        "num_beams",
+        "num_beam_groups",
+        "length_penalty",
+        "early_stopping",
+        "do_sample",
+    ]  # list of inference parameters that can be set
+
     def __init__(
         self,
         model_name_or_path: str = "pszemraj/long-t5-tglobal-base-16384-book-summary",
         use_cuda: bool = True,
         is_general_attention_model: bool = True,
         token_batch_length: int = 2048,
         batch_stride: int = 16,
         max_length_ratio: float = 0.25,
-        load_in_8bit=False,
+        load_in_8bit: bool = False,
+        compile_model: bool = False,
+        optimum_onnx: bool = False,
+        force_cache: bool = False,
         **kwargs,
     ):
         """
         __init__ - initialize the Summarizer class
 
         :param str model_name_or_path: the name or path of the model to load, defaults to "pszemraj/long-t5-tglobal-base-16384-book-summary"
         :param bool use_cuda: whether to use cuda, defaults to True
         :param bool is_general_attention_model: whether the model is a general attention model, defaults to True
         :param int token_batch_length: the amount of tokens to process in a batch, defaults to 2048
         :param int batch_stride: the amount of tokens to stride the batch by, defaults to 16
         :param float max_length_ratio: the ratio of the token_batch_length to use as the max_length for the model, defaults to 0.25
         :param bool load_in_8bit: whether to load the model in 8bit precision (LLM.int8), defaults to False
+        :param bool compile_model: whether to compile the model (pytorch 2.0+ only), defaults to False
+        :param bool optimum_onnx: whether to load the model in ONNX Runtime, defaults to False
+        :param bool force_cache: whether to force the model to use cache, defaults to False
         :param kwargs: additional keyword arguments to pass to the model as inference parameters
         """
         self.logger = logging.getLogger(__name__)
 
         self.model_name_or_path = model_name_or_path
         self.device = "cuda" if torch.cuda.is_available() and use_cuda else "cpu"
         self.logger.debug(f"loading model {model_name_or_path} to {self.device}")
@@ -60,43 +83,72 @@
                     "You must install bitsandbytes to load the model in 8-bit precision. Please run `pip install bitsandbytes` or `pip install textsum[8bit]`"
                 )
             self.model = AutoModelForSeq2SeqLM.from_pretrained(
                 model_name_or_path,
                 load_in_8bit=load_in_8bit,
                 device_map="auto",
             )
+        elif optimum_onnx:
+            from optimum.onnxruntime import ORTModelForSeq2SeqLM
+            import onnxruntime
+
+            if self.device == "cuda":
+                self.logger.warning(
+                    "ONNX runtime+cuda needs an additional package. manually install onnxruntime-gpu"
+                )
+            provider = (
+                "CUDAExecutionProvider"
+                if "GPU" in onnxruntime.get_device() and self.device == "cuda"
+                else "CPUExecutionProvider"
+            )
+            self.logger.info(f"Loading model in ONNX Runtime to provider:\t{provider}")
+            self.model = ORTModelForSeq2SeqLM.from_pretrained(
+                self.model_name_or_path,
+                provider=provider,
+                export=not Path(self.model_name_or_path).is_dir(),
+            )  # if a directory, already exported
         else:
             self.model = AutoModelForSeq2SeqLM.from_pretrained(
                 self.model_name_or_path,
             ).to(self.device)
+            # device_map="auto" is not added for all models
+
+        if compile_model:
+            if validate_pytorch2() and sys.platform != "win32":
+                self.logger.info("Compiling model")
+                self.model = torch.compile(self.model)
+            else:
+                self.logger.warning(
+                    "Unable to compile model. Please upgrade to PyTorch 2.0 and run on a non-Windows platform"
+                )
+        else:
+            self.logger.debug("Not compiling model")
+
+        if not optimum_onnx:
+            self.model = self.model.eval()
 
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_name_or_path)
         self.is_general_attention_model = (
             is_general_attention_model  # TODO: add a check later
         )
 
         self.logger.info(f"Loaded model {model_name_or_path} to {self.device}")
 
+        if force_cache:
+            self.logger.info("Forcing use_cache to True")
+            self.model.config.use_cache = True
+            self.logger.debug(
+                f"model.config.use_cache: {pp.pformat(self.model.config.to_dict())}"
+            )
+
         # set batch processing parameters
         self.token_batch_length = token_batch_length
         self.batch_stride = batch_stride
         self.max_len_ratio = max_length_ratio
 
-        self.settable_inference_params = [
-            "min_length",
-            "max_length",
-            "no_repeat_ngram_size",
-            "encoder_no_repeat_ngram_size",
-            "repetition_penalty",
-            "num_beams",
-            "num_beam_groups",
-            "length_penalty",
-            "early_stopping",
-            "do_sample",
-        ]  # list of inference parameters that can be set
         self.inference_params = {
             "min_length": 8,
             "max_length": int(token_batch_length * max_length_ratio),
             "no_repeat_ngram_size": 3,
             "encoder_no_repeat_ngram_size": 4,
             "repetition_penalty": 2.5,
             "num_beams": 4,
@@ -110,19 +162,36 @@
             if key in self.settable_inference_params:
                 self.inference_params[key] = value
             else:
                 self.logger.warning(
                     f"{key} is not a supported inference parameter, ignoring"
                 )
 
+        self.config = {
+            "model_name_or_path": model_name_or_path,
+            "use_cuda": use_cuda,
+            # "is_general_attention_model": is_general_attention_model, # TODO: validate later
+            "token_batch_length": token_batch_length,
+            "batch_stride": batch_stride,
+            "max_length_ratio": max_length_ratio,
+            "load_in_8bit": load_in_8bit,
+            "compile_model": compile_model,
+            "optimum_onnx": optimum_onnx,
+            "device": self.device,
+            "inference_params": self.inference_params,
+            "textsum_version": textsum.__version__,
+        }
+
+    def __repr__(self):
+        return f"Summarizer(model_name_or_path={self.model_name_or_path}, use_cuda={self.use_cuda}, token_batch_length={self.token_batch_length}, batch_stride={self.batch_stride}, max_length_ratio={self.max_length_ratio}, load_in_8bit={self.load_in_8bit}, compile_model={self.compile_model}, optimum_onnx={self.optimum_onnx})"
+
     def set_inference_params(
         self,
         new_params: dict = None,
         config_file: str or Path = None,
-        config_metadata_id: str = "META_",
     ):
         """
         set_inference_params - update the inference parameters to use when summarizing text
 
         :param dict new_params: a dictionary of new inference parameters to use, defaults to None
         :param str or Path config_file: a path to a json file containing inference parameters, defaults to None
 
@@ -132,15 +201,15 @@
         assert (
             new_params or config_file
         ), "must provide new_params or config_file to set inference parameters"
 
         new_params = new_params or {}
         # load from config file if provided
         if config_file:
-            with open(config_file, "r") as f:
+            with open(config_file, "r", encoding="utf-8") as f:
                 config_params = json.load(f)
             config_params = {
                 k: v
                 for k, v in config_params.items()
                 if k in self.settable_inference_params
             }  # remove key:value pairs that start with config_metadata_id
             new_params.update(config_params)
@@ -155,14 +224,23 @@
                     f"{key} is not a valid inference parameter, ignoring"
                 )
 
     def get_inference_params(self):
         """get the inference parameters currently being used"""
         return self.inference_params
 
+    def print_config(self):
+        """print the current configuration"""
+        print(json.dumps(self.config, indent=2))
+
+    def save_config(self, path: str or Path = "textsum_config.json"):
+        """save the current configuration to a json file"""
+        with open(path, "w", encoding="utf-8") as f:
+            json.dump(self.config, f, indent=2)
+
     def update_loglevel(self, loglevel: int = logging.INFO):
         """update the loglevel of the logger"""
         self.logger.setLevel(loglevel)
 
     def summarize_and_score(self, ids, mask, **kwargs):
         """
         summarize_and_score - summarize a batch of text and return the summary and output scores
@@ -214,57 +292,70 @@
         return summary, score
 
     def summarize_via_tokenbatches(
         self,
         input_text: str,
         batch_length: int = None,
         batch_stride: int = None,
+        min_batch_length: int = 512,
+        pad_incomplete_batch: bool = True,
         **kwargs,
     ):
         """
         summarize_via_tokenbatches - given a string of text, split it into batches of tokens and summarize each batch
 
         :param str input_text: the text to summarize
         :param int batch_length: number of tokens to include in each input batch, default None (self.token_batch_length)
         :param int batch_stride: number of tokens to stride between batches, default None (self.token_batch_stride)
+        :param bool pad_incomplete_batch: whether to pad the last batch to the length of the longest batch, default True
         :return: a list of summaries, a list of scores, and a list of the input text for each batch
         """
 
-        # log all input parameters
-        if batch_length and batch_length < 512:
+        batch_length = self.token_batch_length if batch_length is None else batch_length
+        batch_stride = self.batch_stride if batch_stride is None else batch_stride
+
+        if batch_length < min_batch_length:
             self.logger.warning(
-                "WARNING: entered batch_length was too low at {batch_length}, resetting to 512"
+                f"batch_length must be at least {min_batch_length}. Setting batch_length to {min_batch_length}"
             )
-            batch_length = 512
+            batch_length = min_batch_length
 
         self.logger.debug(
             f"batch_length: {batch_length} batch_stride: {batch_stride}, kwargs: {kwargs}"
         )
         if kwargs:
             # if received kwargs, update inference params
             self.set_inference_params(**kwargs)
 
         params = self.get_inference_params()
 
         encoded_input = self.tokenizer(
             input_text,
             padding="max_length",
             truncation=True,
-            max_length=batch_length or self.token_batch_length,
-            stride=batch_stride or self.batch_stride,
+            max_length=batch_length,
+            stride=batch_stride,
             return_overflowing_tokens=True,
-            add_special_tokens=False,
             return_tensors="pt",
         )
         in_id_arr, att_arr = encoded_input.input_ids, encoded_input.attention_mask
 
         gen_summaries = []
         pbar = tqdm(total=len(in_id_arr), desc="Generating Summaries")
 
         for _id, _mask in zip(in_id_arr, att_arr):
+            # If the batch is smaller than batch_length, pad it with the model's pad token
+            if len(_id) < batch_length and pad_incomplete_batch:
+                self.logger.debug(
+                    f"padding batch of length {len(_id)} to {batch_length}"
+                )
+                pad_token = self.tokenizer.pad_token_id
+                difference = batch_length - len(_id)
+                _id = torch.cat([_id, torch.tensor([pad_token] * difference)])
+                _mask = torch.cat([_mask, torch.tensor([0] * difference)])
 
             result, score = self.summarize_and_score(
                 ids=_id,
                 mask=_mask,
                 **params,
             )
             score = round(float(score), 4)
@@ -315,16 +406,15 @@
                 for s in summary_data
             ]
         else:
             sum_text = [s["summary"][0] for s in summary_data]
 
         sum_scores = [f"\n - {round(s['summary_score'],4)}" for s in summary_data]
         scores_text = "\n".join(sum_scores)
-        full_summary = "\n\t".join(sum_text)
-
+        full_summary = "\n".join(sum_text)
         if return_string:
             return full_summary
 
         target_file = Path(target_file)
         if not target_file.parent.exists():
             logging.info(f"Creating directory {target_file.parent}")
             target_file.parent.mkdir(parents=True)
@@ -333,27 +423,25 @@
 
         with open(
             target_file,
             "w",
             encoding="utf-8",
             errors="ignore",
         ) as fo:
-
             fo.writelines(full_summary)
 
         if save_scores:
             with open(
                 target_file,
                 "a",
                 encoding="utf-8",
                 errors="ignore",
             ) as fo:
-
-                fo.write("\n" * 3)
-                fo.write(f"\n\nSection Scores for {target_file.stem}:\n")
+                fo.write("\n" * 2 + "---\n\n")
+                fo.write(f"Section Scores for {target_file.stem}:\n")
                 fo.writelines(scores_text)
                 fo.write("\n\n---\n")
 
         self.logger.info(f"Saved summary to {target_file.resolve()}")
 
     def summarize_string(
         self,
@@ -454,20 +542,24 @@
         metadata_path = (
             output_path / "summarization_parameters.json"
             if output_path.is_dir()
             else output_path
         )  # if output_path is a file, use that, otherwise use the default name
 
         exported_params = self.get_inference_params().copy()
-        exported_params["META_huggingface_model"] = (
-            self.model_name_or_path if hf_tag is None else hf_tag
-        )
-        exported_params["META_date"] = get_timestamp()
+        metadata = {
+            "META_huggingface_model": (
+                self.model_name_or_path if hf_tag is None else hf_tag
+            ),
+            "META_date": get_timestamp(),
+            "META_textsum_version": textsum.__version__,
+        }
+        exported_params["METADATA"] = metadata
 
         self.logger.info(f"Saving parameters to {metadata_path}")
         with open(metadata_path, "w") as write_file:
-            json.dump(exported_params, write_file, indent=4)
+            json.dump(exported_params, write_file, indent=2)
 
         logging.debug(f"Saved parameters to {metadata_path}")
         if verbose:
             self.logger.info(f"parameters: {exported_params}")
             print(f"saved parameters to {metadata_path}")
```

### Comparing `textsum-0.1.5/src/textsum/utils.py` & `textsum-0.2.0/src/textsum/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,22 @@
 
     if verbose:
         print(f"GPU found: {gpu_name}")
     # check if it is an A100
     return bool("A100" in gpu_name)
 
 
+def validate_pytorch2(torch_version: str = None):
+    torch_version = torch.__version__ if torch_version is None else torch_version
+
+    pattern = r"^2\.\d+(\.\d+)*"
+
+    return True if re.match(pattern, torch_version) else False
+
+
 def cstr(s, color="black"):
     """styles a string with a color"""
     return "<text style=color:{}>{}</text>".format(color, s)
 
 
 def color_print(text: str, c_id="pink"):
     """helper function to print colored text to the terminal"""
@@ -149,31 +157,40 @@
     """
     # remove any existing handlers
     root = logging.getLogger()
     if root.handlers:
         for handler in root.handlers:
             root.removeHandler(handler)
 
-    logformat = "[%(asctime)s] %(levelname)s:%(name)s:%(message)s"
+    log_format = "[%(asctime)s] %(levelname)s:%(name)s:%(message)s"
+    debug_format = (
+        "%(asctime)s [%(levelname)s] %(name)s %(filename)s:%(lineno)d - %(message)s"
+    )
     if logfile is None:
         logging.basicConfig(
             level=loglevel,
             stream=sys.stdout,
-            format=logformat,
+            format=log_format,
             datefmt="%Y-%m-%d %H:%M:%S",
         )
     else:
+        logfile = Path(logfile)
         loglevel = (
-            logging.INFO if not loglevel in [logging.DEBUG, logging.INFO] else loglevel
+            logging.INFO
+            if not loglevel in [logging.DEBUG, logging.INFO, logging.WARNING]
+            else loglevel
         )
+        if loglevel == logging.DEBUG:
+            logfile.unlink(missing_ok=True)
+
         logging.basicConfig(
             level=loglevel,
             filename=logfile,
             filemode="w",
-            format=logformat,
+            format=debug_format if loglevel == logging.DEBUG else log_format,
             datefmt="%Y-%m-%d %H:%M:%S",
         )
 
 
 def postprocess_booksummary(text: str, custom_phrases: list = None) -> str:
     """
     postprocess_booksummary - postprocess the book summary
@@ -188,17 +205,16 @@
         "In this chapter, ",
         "In this paper, ",
     ]  # the default phrases to remove (from booksum dataset)
 
     if custom_phrases is not None:
         REMOVAL_PHRASES.extend(custom_phrases)
     for pr in REMOVAL_PHRASES:
-
         text = text.replace(pr, "")
-    return text
+    return text.strip()
 
 
 def check_bitsandbytes_available():
     """
     check_bitsandbytes_available - check if the bitsandbytes library is available
     """
     try:
```

### Comparing `textsum-0.1.5/src/textsum.egg-info/SOURCES.txt` & `textsum-0.2.0/src/textsum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `textsum-0.1.5/tox.ini` & `textsum-0.2.0/tox.ini`

 * *Files identical despite different names*

