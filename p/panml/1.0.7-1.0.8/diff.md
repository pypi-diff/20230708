# Comparing `tmp/panml-1.0.7.tar.gz` & `tmp/panml-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-1.0.7.tar", last modified: Sat Jun 17 04:41:07 2023, max compression
+gzip compressed data, was "panml-1.0.8.tar", last modified: Sat Jul  8 11:33:57 2023, max compression
```

## Comparing `panml-1.0.7.tar` & `panml-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.215625 panml-1.0.7/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.7/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-17 04:41:07.215939 panml-1.0.7/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.7/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.209970 panml-1.0.7/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.7/panml/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.212626 panml-1.0.7/panml/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.7/panml/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9448 2023-06-17 04:40:13.000000 panml-1.0.7/panml/clustering/faiss.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.7/panml/constants.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.7/panml/environments.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.214082 panml-1.0.7/panml/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.7/panml/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    24501 2023-06-15 12:36:48.000000 panml-1.0.7/panml/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    15604 2023-06-14 02:30:39.000000 panml-1.0.7/panml/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-11 00:13:19.000000 panml-1.0.7/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.7/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.211812 panml-1.0.7/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-17 04:41:07.000000 panml-1.0.7/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-17 04:41:07.000000 panml-1.0.7/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-17 04:41:07.000000 panml-1.0.7/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-17 04:41:07.000000 panml-1.0.7/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-17 04:41:07.000000 panml-1.0.7/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-17 04:41:07.216999 panml-1.0.7/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-17 04:40:13.000000 panml-1.0.7/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-17 04:41:07.215102 panml-1.0.7/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.7/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    12552 2023-06-15 12:36:48.000000 panml-1.0.7/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-07-08 11:33:57.182720 panml-1.0.8/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.8/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-07-08 11:33:57.183009 panml-1.0.8/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.8/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-07-08 11:33:57.175823 panml-1.0.8/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.8/panml/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-07-08 11:33:57.178437 panml-1.0.8/panml/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.8/panml/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9448 2023-06-17 04:40:13.000000 panml-1.0.8/panml/clustering/faiss.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     6288 2023-07-08 11:32:14.000000 panml-1.0.8/panml/constants.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.8/panml/environments.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-07-08 11:33:57.180058 panml-1.0.8/panml/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.8/panml/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    26140 2023-07-08 03:51:09.000000 panml-1.0.8/panml/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    15604 2023-06-14 02:30:39.000000 panml-1.0.8/panml/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2740 2023-07-08 03:51:09.000000 panml-1.0.8/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.8/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-07-08 11:33:57.177565 panml-1.0.8/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-07-08 11:33:57.000000 panml-1.0.8/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-07-08 11:33:57.000000 panml-1.0.8/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-07-08 11:33:57.000000 panml-1.0.8/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-07-08 11:33:57.000000 panml-1.0.8/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-07-08 11:33:57.000000 panml-1.0.8/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-07-08 11:33:57.184011 panml-1.0.8/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-07-08 11:32:14.000000 panml-1.0.8/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-07-08 11:33:57.181739 panml-1.0.8/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.8/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    12552 2023-06-15 12:36:48.000000 panml-1.0.8/test/test_VectorEngine.py
```

### Comparing `panml-1.0.7/LICENSE` & `panml-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-1.0.7/PKG-INFO` & `panml-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.7
+Version: 1.0.8
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.7/README.md` & `panml-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `panml-1.0.7/panml/clustering/faiss.py` & `panml-1.0.8/panml/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.7/panml/constants.py` & `panml-1.0.8/panml/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,20 @@
         'StabilityAI/stablelm-base-alpha-7b',
         'StabilityAI/stablelm-tuned-alpha-3b',
         'StabilityAI/stablelm-tuned-alpha-7b',
         'h2oai/h2ogpt-oasst1-512-12b',
         'h2oai/h2ogpt-oasst1-512-20b',
         'Salesforce/codegen-350M-multi',
         'Salesforce/codegen-2B-multi',
+        'Salesforce/codegen2-1B',
+        'Salesforce/codegen2-7B',
+        'Salesforce/codegen2-16B',
+        'Salesforce/codegen25-7b-multi',
+        'Salesforce/codegen25-7b-mono',
+        'Salesforce/codegen25-7b-instruct',
         'bigcode/starcoder',
         'bert-base-uncased',
         'distilbert-base-uncased',
         'roberta-base',
         'distilroberta-base',
         'togethercomputer/RedPajama-INCITE-Base-3B-v1',
         'togethercomputer/RedPajama-INCITE-Instruct-3B-v1',
@@ -175,14 +181,22 @@
 PEFT_LORA_DEFAULT_ARGS = {
     'inference_mode': False, 
     'r': 8, 
     'lora_alpha': 32, 
     'lora_dropout': 0.1,
 }
 
+# Bits and Bytes configuration default arguments
+BNB_DEFAULT_ARGS = {
+    'load_in_4bit': True,
+    'bnb_4bit_use_double_quant': True,
+    'bnb_4bit_quant_type': 'nf4',
+    'bnb_4bit_compute_dtype': 'torch.bfloat16'
+}
+
 # == Prompt constants ==
 # Prompt templates
 CHAIN_OF_THOUGHT_PROMPT = [
     {"append": "Let's think this step by step."}
 ]
 
 EXPLAIN_PROMPT = [
```

### Comparing `panml-1.0.7/panml/environments.py` & `panml-1.0.8/panml/environments.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.7/panml/llm/huggingface.py` & `panml-1.0.8/panml/llm/huggingface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 import pandas as pd
 import torch
-from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoModelForMaskedLM, AutoTokenizer
+from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoModelForMaskedLM, AutoTokenizer, BitsAndBytesConfig
 from transformers import TrainingArguments, Trainer, Seq2SeqTrainingArguments, Seq2SeqTrainer, DataCollatorForLanguageModeling, DataCollatorForSeq2Seq
 from datasets import Dataset
 from peft import get_peft_model, PeftModel, PeftConfig, LoraConfig, TaskType
 from typing import Union, Callable
-from panml.constants import SUPPORTED_LLMS_PEFT_LORA, TOKENIZER_DEFAULT_ARGS, TRAINER_ARGS, PEFT_LORA_DEFAULT_ARGS
+from panml.constants import SUPPORTED_LLMS_PEFT_LORA, TOKENIZER_DEFAULT_ARGS, TRAINER_ARGS, PEFT_LORA_DEFAULT_ARGS, BNB_DEFAULT_ARGS
 
 # HuggingFace model class
 class HuggingFaceModelPack:
     '''
     HuggingFace Hub model pack class
     '''
     # Initialize class variables
@@ -18,23 +18,37 @@
         self.model_name = model # model name
         self.trainer_args = TRAINER_ARGS # model trainer arguments
         self.supported_models_peft_lora = SUPPORTED_LLMS_PEFT_LORA # supported LLMs for LoRA implementation
         self.peft_config = None # PEFT LoRA configuration
         self.device = 'cpu' # model training and inference hardware setting
         self.evaluation_result = None # model training evaluation result
         self.prediction_history = [] # model inference history in prompt loop
+        self.qlora = False  # bool for QLoRA finetuning
         
         # Get tokenizer arguments
         tokenzier_args = {k: model_args.pop(k) for k in list(TOKENIZER_DEFAULT_ARGS.keys()) if k in model_args}
         for k in TOKENIZER_DEFAULT_ARGS:
             tokenzier_args.setdefault(k, TOKENIZER_DEFAULT_ARGS[k])
         self.padding_length = tokenzier_args['padding_length']
         self.input_block_size = tokenzier_args['input_block_size']
         self.tokenizer_batch = tokenzier_args['tokenizer_batch']
-        
+
+        # Get QLoRA configuration from model args
+        if 'qlora' in model_args:
+            qlora_args = model_args.pop('qlora')
+            if 'bnb_config' in qlora_args:
+                self.qlora = True
+                bnb_config = qlora_args.pop('bnb_config')
+                if not isinstance(bnb_config, BitsAndBytesConfig):
+                    for i in BNB_DEFAULT_ARGS:
+                        bnb_config.setdefault(i, BNB_DEFAULT_ARGS[i])
+                    bnb_config = BitsAndBytesConfig(**bnb_config)
+            else:
+                raise ValueError('QLoRA should contain bits and bytes configuration for quantization_config')
+                
         # Get PEFT LoRA configuration from model args
         peft_lora_args, load_peft_lora = {}, False
         if 'peft_lora' in model_args:
             peft_lora_args = model_args.pop('peft_lora')
             if 'load' in peft_lora_args:
                 load_peft_lora = peft_lora_args.pop('load')
             else:
@@ -69,15 +83,25 @@
             if 'flan' in self.model_name:
                 self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.model_name, **model_args)
             elif 'bert' in self.model_name:
                 self.model_hf = AutoModelForMaskedLM.from_pretrained(self.model_name, **model_args)
             else:
                 self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args)
         elif source == 'local':
-            if load_peft_lora:
+            if self.qlora:
+                # Set QLoRA trained model
+                self.peft_config = PeftConfig.from_pretrained(self.model_name)
+                if 'flan' in self.peft_config.base_model_name_or_path:
+                    self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.peft_config.base_model_name_or_path, quantization_config=bnb_config, **model_args)
+                elif 'bert' in self.peft_config.base_model_name_or_path:
+                    self.model_hf = AutoModelForMaskedLM.from_pretrained(self.peft_config.base_model_name_or_path, quantization_config=bnb_config, **model_args)
+                else:
+                    self.model_hf = AutoModelForCausalLM.from_pretrained(self.peft_config.base_model_name_or_path, quantization_config=bnb_config, **model_args)
+                self.model_hf = PeftModel.from_pretrained(self.model_hf, self.model_name)
+            elif load_peft_lora:
                 # Set LoRA trained model
                 self.peft_config = PeftConfig.from_pretrained(self.model_name)
                 if 'flan' in self.peft_config.base_model_name_or_path:
                     self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args)
                 elif 'bert' in self.peft_config.base_model_name_or_path:
                     self.model_hf = AutoModelForMaskedLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args)
                 else:
```

### Comparing `panml-1.0.7/panml/llm/openai.py` & `panml-1.0.8/panml/llm/openai.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.7/panml/models.py` & `panml-1.0.8/panml/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,11 +40,11 @@
             ImportEnvironment(['openai', 'pandas', 'torch']).validate()
             if self.model not in self.supported_models['openai']:
                 raise ValueError('The specified model currently is not supported in this package. Supported OpenAI models are: ' + ' '.join([f"{m}" for m in self.supported_models['openai']]))
             if self.api_key is None:
                 raise ValueError('api key has not been specified for OpenAI model call')
             self.instance = OpenAIModelPack(model=self.model, api_key=self.api_key)
 
-    # Direct to the attribute ofthe sub model pack class (attribute not found in the main model pack class)
+    # Direct to the attribute of the sub model pack class (attribute not found in the main model pack class)
     def __getattr__(self, name):
         return self.instance.__getattribute__(name)
```

### Comparing `panml-1.0.7/panml/search.py` & `panml-1.0.8/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.7/panml.egg-info/PKG-INFO` & `panml-1.0.8/panml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.7
+Version: 1.0.8
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.7/setup.py` & `panml-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '1.0.7', # version
+  version = '1.0.8', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-1.0.7/test/test_ModelPack.py` & `panml-1.0.8/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.7/test/test_VectorEngine.py` & `panml-1.0.8/test/test_VectorEngine.py`

 * *Files identical despite different names*

