# Comparing `tmp/be_great-0.0.4.tar.gz` & `tmp/be_great-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "be_great-0.0.4.tar", last modified: Sat Apr  1 11:32:56 2023, max compression
+gzip compressed data, was "be_great-0.0.5.tar", last modified: Sat Jul  8 20:51:48 2023, max compression
```

## Comparing `be_great-0.0.4.tar` & `be_great-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 11:32:56.861246 be_great-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1090 2023-04-01 11:20:05.000000 be_great-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3943 2023-04-01 11:32:56.861246 be_great-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2043 2023-04-01 11:20:05.000000 be_great-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 11:32:56.857246 be_great-0.0.4/be_great/
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-01 11:20:05.000000 be_great-0.0.4/be_great/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15755 2023-04-01 11:20:05.000000 be_great-0.0.4/be_great/great.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-04-01 11:20:05.000000 be_great-0.0.4/be_great/great_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5345 2023-04-01 11:20:05.000000 be_great-0.0.4/be_great/great_start.py
--rw-r--r--   0 root         (0) root         (0)     1392 2023-04-01 11:20:05.000000 be_great-0.0.4/be_great/great_trainer.py
--rw-r--r--   0 root         (0) root         (0)     3181 2023-04-01 11:20:05.000000 be_great-0.0.4/be_great/great_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 11:32:56.861246 be_great-0.0.4/be_great.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3943 2023-04-01 11:32:56.000000 be_great-0.0.4/be_great.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      330 2023-04-01 11:32:56.000000 be_great-0.0.4/be_great.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 11:32:56.000000 be_great-0.0.4/be_great.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-01 11:32:56.000000 be_great-0.0.4/be_great.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-01 11:32:56.000000 be_great-0.0.4/be_great.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      994 2023-04-01 11:25:56.000000 be_great-0.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-01 11:32:56.865246 be_great-0.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 20:51:48.594634 be_great-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-08 20:42:13.000000 be_great-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4816 2023-07-08 20:51:48.590634 be_great-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2916 2023-07-08 20:42:13.000000 be_great-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 20:51:48.590634 be_great-0.0.5/be_great/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 20:42:13.000000 be_great-0.0.5/be_great/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22761 2023-07-08 20:42:13.000000 be_great-0.0.5/be_great/great.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-08 20:42:13.000000 be_great-0.0.5/be_great/great_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5414 2023-07-08 20:42:13.000000 be_great-0.0.5/be_great/great_start.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-07-08 20:42:13.000000 be_great-0.0.5/be_great/great_trainer.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2023-07-08 20:42:13.000000 be_great-0.0.5/be_great/great_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 20:51:48.590634 be_great-0.0.5/be_great.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4816 2023-07-08 20:51:48.000000 be_great-0.0.5/be_great.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-08 20:51:48.000000 be_great-0.0.5/be_great.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 20:51:48.000000 be_great-0.0.5/be_great.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-08 20:51:48.000000 be_great-0.0.5/be_great.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-08 20:51:48.000000 be_great-0.0.5/be_great.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-07-08 20:50:22.000000 be_great-0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 20:51:48.594634 be_great-0.0.5/setup.cfg
```

### Comparing `be_great-0.0.4/LICENSE` & `be_great-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `be_great-0.0.4/PKG-INFO` & `be_great-0.0.5/be_great.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: be_great
-Version: 0.0.4
+Name: be-great
+Version: 0.0.5
 Summary: Generating Realistic Tabular Data using Large Language Models
 Author-email: Kathrin Sessler <kathrin.sessler@tum.de>
 License: MIT License
         
         Copyright (c) 2022 Kathrin Seßler and Vadim Borisov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,14 +31,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/be-great.svg)](https://badge.fury.io/py/be-great) [![Downloads](https://static.pepy.tech/badge/be-great)](https://pepy.tech/project/be-great)
 
 [//]: # (![Screenshot]&#40;https://github.com/kathrinse/be_great/blob/main/imgs/GReaT_logo.png&#41;)
 <p align="center">
 <img src="https://github.com/kathrinse/be_great/raw/main/imgs/GReaT_logo.png" width="326"/>
 </p>
 
 <p align="center">
@@ -67,21 +68,37 @@
 In the example below, we show how the GReaT approach is used to generate synthetic tabular data for the California Housing dataset.
 ```python
 from be_great import GReaT
 from sklearn.datasets import fetch_california_housing
 
 data = fetch_california_housing(as_frame=True).frame
 
-model = GReaT(llm='distilgpt2', batch_size=32, epochs=50)
+model = GReaT(llm='distilgpt2', batch_size=32, epochs=25)
 model.fit(data)
 synthetic_data = model.sample(n_samples=100)
 ```
 
-<!---
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kathrinse/be_great/blob/main/examples/GReaT_colab_example.ipynb)--->
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kathrinse/be_great/blob/main/examples/GReaT_colab_example.ipynb)
+
+### Imputing a sample
+GReaT also features an interface to impute, i.e., fill in, missing values in arbitrary combinations. This requires a trained ``model``, for instance one obtained using the code snippet above, and a ```pd.DataFrame``` where missing values are set to NaN.
+A minimal example is provided below:
+```python
+# test_data: pd.DataFrame with samples from the distribution
+# model: GReaT trained on the data distribution that should be imputed
+
+# Drop values randomly from test_data
+import numpy as np
+for clm in test_data.columns:
+    test_data[clm]=test_data[clm].apply(lambda x: (x if np.random.rand() > 0.5 else np.nan))
+
+imputed_data = model.impute(test_data, max_length=200)
+```
+
+
 
 ## GReaT Citation 
 
 If you use GReaT, please link or cite our work:
 
 ``` bibtex
 @inproceedings{borisov2023language,
```

### Comparing `be_great-0.0.4/README.md` & `be_great-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[![PyPI version](https://badge.fury.io/py/be-great.svg)](https://badge.fury.io/py/be-great) [![Downloads](https://static.pepy.tech/badge/be-great)](https://pepy.tech/project/be-great)
 
 [//]: # (![Screenshot]&#40;https://github.com/kathrinse/be_great/blob/main/imgs/GReaT_logo.png&#41;)
 <p align="center">
 <img src="https://github.com/kathrinse/be_great/raw/main/imgs/GReaT_logo.png" width="326"/>
 </p>
 
 <p align="center">
@@ -30,21 +31,37 @@
 In the example below, we show how the GReaT approach is used to generate synthetic tabular data for the California Housing dataset.
 ```python
 from be_great import GReaT
 from sklearn.datasets import fetch_california_housing
 
 data = fetch_california_housing(as_frame=True).frame
 
-model = GReaT(llm='distilgpt2', batch_size=32, epochs=50)
+model = GReaT(llm='distilgpt2', batch_size=32, epochs=25)
 model.fit(data)
 synthetic_data = model.sample(n_samples=100)
 ```
 
-<!---
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kathrinse/be_great/blob/main/examples/GReaT_colab_example.ipynb)--->
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kathrinse/be_great/blob/main/examples/GReaT_colab_example.ipynb)
+
+### Imputing a sample
+GReaT also features an interface to impute, i.e., fill in, missing values in arbitrary combinations. This requires a trained ``model``, for instance one obtained using the code snippet above, and a ```pd.DataFrame``` where missing values are set to NaN.
+A minimal example is provided below:
+```python
+# test_data: pd.DataFrame with samples from the distribution
+# model: GReaT trained on the data distribution that should be imputed
+
+# Drop values randomly from test_data
+import numpy as np
+for clm in test_data.columns:
+    test_data[clm]=test_data[clm].apply(lambda x: (x if np.random.rand() > 0.5 else np.nan))
+
+imputed_data = model.impute(test_data, max_length=200)
+```
+
+
 
 ## GReaT Citation 
 
 If you use GReaT, please link or cite our work:
 
 ``` bibtex
 @inproceedings{borisov2023language,
```

### Comparing `be_great-0.0.4/be_great/great.py` & `be_great-0.0.5/be_great/great.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,27 +6,37 @@
 
 import numpy as np
 import pandas as pd
 
 from tqdm import tqdm
 
 import torch
-from transformers import (AutoTokenizer,
-                          AutoModelForCausalLM,
-                          TrainingArguments)
+from transformers import AutoTokenizer, AutoModelForCausalLM, TrainingArguments
 
 from be_great.great_dataset import GReaTDataset, GReaTDataCollator
-from be_great.great_start import GReaTStart, CategoricalStart, ContinuousStart, RandomStart
+from be_great.great_start import (
+    GReaTStart,
+    CategoricalStart,
+    ContinuousStart,
+    RandomStart,
+    _pad_tokens,
+)
 from be_great.great_trainer import GReaTTrainer
-from be_great.great_utils import _array_to_dataframe, _get_column_distribution, _convert_tokens_to_text, \
-    _convert_text_to_tabular_data
+from be_great.great_utils import (
+    _array_to_dataframe,
+    _get_column_distribution,
+    _convert_tokens_to_text,
+    _convert_text_to_tabular_data,
+    _partial_df_to_promts,
+    bcolors,
+)
 
 
 class GReaT:
-    """ GReaT Class
+    """GReaT Class
 
     The GReaT class handles the whole generation flow. It is used to fine-tune a large language model for tabular data,
     and to sample synthetic tabular data.
 
     Attributes:
         llm (str): HuggingFace checkpoint of a pretrained large language model, used a basis of our model
         tokenizer (AutoTokenizer): Tokenizer, automatically downloaded from llm-checkpoint
@@ -39,49 +49,93 @@
          https://huggingface.co/docs/transformers/main/en/main_classes/trainer#transformers.TrainingArguments
         columns (list): List of all features/columns of the tabular dataset
         num_cols (list): List of all numerical features/columns of the tabular dataset
         conditional_col (str): Name of a feature/column on which the sampling can be conditioned
         conditional_col_dist (dict | list): Distribution of the feature/column specified by condtional_col
     """
 
-    def __init__(self, llm: str, experiment_dir: str = "trainer_great", epochs: int = 100,
-                 batch_size: int = 8, **train_kwargs):
-        """ Initializes GReaT.
+    def __init__(
+        self,
+        llm: str,
+        experiment_dir: str = "trainer_great",
+        epochs: int = 100,
+        batch_size: int = 8,
+        efficient_finetuning: str = "",
+        **train_kwargs,
+    ):
+        """Initializes GReaT.
 
         Args:
             llm: HuggingFace checkpoint of a pretrained large language model, used a basis of our model
             experiment_dir:  Directory, where the training checkpoints will be saved
             epochs: Number of epochs to fine-tune the model
             batch_size: Batch size used for fine-tuning
+            efficient_finetuning: Indication of fune-tuning method
             train_kwargs: Additional hyperparameters added to the TrainingArguments used by the HuggingFaceLibrary,
              see here the full list of all possible values
              https://huggingface.co/docs/transformers/main/en/main_classes/trainer#transformers.TrainingArguments
         """
         # Load Model and Tokenizer from HuggingFace
+        self.efficient_finetuning = efficient_finetuning
         self.llm = llm
         self.tokenizer = AutoTokenizer.from_pretrained(self.llm)
         self.tokenizer.pad_token = self.tokenizer.eos_token
         self.model = AutoModelForCausalLM.from_pretrained(self.llm)
 
+        if self.efficient_finetuning == "lora":
+            # Lazy importing
+            try:
+                from peft import (
+                    LoraConfig,
+                    get_peft_model,
+                    prepare_model_for_int8_training,
+                    TaskType,
+                )
+            except ImportError:
+                raise ImportError(
+                    "This function requires the 'perf' package. Please install it with - pip install peft"
+                )
+
+            # Define LoRA Config
+            lora_config = LoraConfig(
+                r=16,  # only training 0.16% of the parameters of the model
+                lora_alpha=32,
+                target_modules=[
+                    "c_attn"
+                ],  # this is specific for gpt2 model, to be adapted
+                lora_dropout=0.05,
+                bias="none",
+                task_type=TaskType.CAUSAL_LM,  # this is specific for gpt2 model, to be adapted
+            )
+            # prepare int-8 model for training
+            self.model = prepare_model_for_int8_training(self.model)
+            # add LoRA adaptor
+            self.model = get_peft_model(self.model, lora_config)
+            self.model.print_trainable_parameters()
+
         # Set the training hyperparameters
         self.experiment_dir = experiment_dir
         self.epochs = epochs
         self.batch_size = batch_size
         self.train_hyperparameters = train_kwargs
 
         # Needed for the sampling process
         self.columns = None
         self.num_cols = None
         self.conditional_col = None
         self.conditional_col_dist = None
 
-    def fit(self, data: tp.Union[pd.DataFrame, np.ndarray], column_names: tp.Optional[tp.List[str]] = None,
-            conditional_col: tp.Optional[str] = None, resume_from_checkpoint: tp.Union[bool, str] = False) \
-            -> GReaTTrainer:
-        """ Fine-tune GReaT using tabular data.
+    def fit(
+        self,
+        data: tp.Union[pd.DataFrame, np.ndarray],
+        column_names: tp.Optional[tp.List[str]] = None,
+        conditional_col: tp.Optional[str] = None,
+        resume_from_checkpoint: tp.Union[bool, str] = False,
+    ) -> GReaTTrainer:
+        """Fine-tune GReaT using tabular data.
 
         Args:
             data: Pandas DataFrame or Numpy Array that contains the tabular data
             column_names: If data is Numpy Array, the feature names have to be defined. If data is Pandas
             DataFrame, the value is ignored
             conditional_col: If given, the distribution of this column is saved and used as a starting
             point for the generation process later. If None, the last column is considered as conditional feature
@@ -98,30 +152,44 @@
         # Convert DataFrame into HuggingFace dataset object
         logging.info("Convert data into HuggingFace dataset object...")
         great_ds = GReaTDataset.from_pandas(df)
         great_ds.set_tokenizer(self.tokenizer)
 
         # Set training hyperparameters
         logging.info("Create GReaT Trainer...")
-        training_args = TrainingArguments(self.experiment_dir,
-                                          num_train_epochs=self.epochs,
-                                          per_device_train_batch_size=self.batch_size,
-                                          **self.train_hyperparameters)
-        great_trainer = GReaTTrainer(self.model, training_args, train_dataset=great_ds, tokenizer=self.tokenizer,
-                                     data_collator=GReaTDataCollator(self.tokenizer))
+        training_args = TrainingArguments(
+            self.experiment_dir,
+            num_train_epochs=self.epochs,
+            per_device_train_batch_size=self.batch_size,
+            **self.train_hyperparameters,
+        )
+        great_trainer = GReaTTrainer(
+            self.model,
+            training_args,
+            train_dataset=great_ds,
+            tokenizer=self.tokenizer,
+            data_collator=GReaTDataCollator(self.tokenizer),
+        )
 
         # Start training
         logging.info("Start training...")
         great_trainer.train(resume_from_checkpoint=resume_from_checkpoint)
         return great_trainer
 
-    def sample(self, n_samples: int,
-               start_col: tp.Optional[str] = "", start_col_dist: tp.Optional[tp.Union[dict, list]] = None,
-               temperature: float = 0.7, k: int = 100, max_length: int = 100, device: str = "cuda") -> pd.DataFrame:
-        """ Generate synthetic tabular data samples
+    def sample(
+        self,
+        n_samples: int,
+        start_col: tp.Optional[str] = "",
+        start_col_dist: tp.Optional[tp.Union[dict, list]] = None,
+        temperature: float = 0.7,
+        k: int = 100,
+        max_length: int = 100,
+        device: str = "cuda",
+    ) -> pd.DataFrame:
+        """Generate synthetic tabular data samples
 
         Args:
             n_samples: Number of synthetic samples to generate
             start_col: Feature to use as starting point for the generation process. If not given, the target
              learned during the fitting is used as starting point
             start_col_dist: Feature distribution of the starting feature. Should have the format
              "{F1: p1, F2: p2, ...}" for discrete columns or be a list of possible values for continuous columns.
@@ -145,45 +213,76 @@
 
         # Init empty DataFrame for the generated samples
         df_gen = pd.DataFrame(columns=self.columns)
 
         # Start generation process
         with tqdm(total=n_samples) as pbar:
             already_generated = 0
-            while n_samples > df_gen.shape[0]:
-                start_tokens = great_start.get_start_tokens(k)
-                start_tokens = torch.tensor(start_tokens).to(device)
-
-                # Generate tokens
-                tokens = self.model.generate(input_ids=start_tokens, max_length=max_length,
-                                             do_sample=True, temperature=temperature, pad_token_id=50256)
-
-                # Convert tokens back to tabular data
-                text_data = _convert_tokens_to_text(tokens, self.tokenizer)
-                df_gen = _convert_text_to_tabular_data(text_data, df_gen)
-
-                # Remove rows with flawed numerical values
-                for i_num_cols in self.num_cols:
-                    df_gen = df_gen[pd.to_numeric(df_gen[i_num_cols], errors='coerce').notnull()]
-
-                df_gen[self.num_cols] = df_gen[self.num_cols].astype(float)
-
-                # Remove rows with missing values
-                df_gen = df_gen.drop(df_gen[df_gen.isna().any(axis=1)].index)
-
-                # Update process bar
-                pbar.update(df_gen.shape[0] - already_generated)
-                already_generated = df_gen.shape[0]
+            _cnt = 0
+            try:
+                while n_samples > df_gen.shape[0]:
+                    start_tokens = great_start.get_start_tokens(k)
+                    start_tokens = torch.tensor(start_tokens).to(device)
+
+                    # Generate tokens
+                    tokens = self.model.generate(
+                        input_ids=start_tokens,
+                        max_length=max_length,
+                        do_sample=True,
+                        temperature=temperature,
+                        pad_token_id=50256,
+                    )
+
+                    # Convert tokens back to tabular data
+                    text_data = _convert_tokens_to_text(tokens, self.tokenizer)
+                    df_gen = _convert_text_to_tabular_data(text_data, df_gen)
+
+                    # Remove rows with flawed numerical values
+                    for i_num_cols in self.num_cols:
+                        df_gen = df_gen[
+                            pd.to_numeric(df_gen[i_num_cols], errors="coerce").notnull()
+                        ]
+
+                    df_gen[self.num_cols] = df_gen[self.num_cols].astype(float)
+
+                    # Remove rows with missing values
+                    df_gen = df_gen.drop(df_gen[df_gen.isna().any(axis=1)].index)
+
+                    # Update process bar
+                    pbar.update(df_gen.shape[0] - already_generated)
+                    already_generated = df_gen.shape[0]
+
+                    # Check if we actually generating synth samples and if not break everything
+                    _cnt += 1
+                    if _cnt > 13 and already_generated == 0:  # (:
+                        raise Exception("Breaking the generation loop!")
+
+            except Exception as e:
+                print(f"{bcolors.FAIL}An error has occurred: {str(e)}{bcolors.ENDC}")
+                print(
+                    f"{bcolors.WARNING}To address this issue, consider fine-tuning the GReaT model for an longer period. This can be achieved by increasing the number of epochs.{bcolors.ENDC}"
+                )
+                print(
+                    f"{bcolors.WARNING}Alternatively, you might consider increasing the max_length parameter within the sample function. For example: model.sample(n_samples=10, max_length=2000){bcolors.ENDC}"
+                )
+                print(
+                    f"{bcolors.OKBLUE}If the problem persists despite these adjustments, feel free to raise an issue on our GitHub page at: https://github.com/kathrinse/be_great/issues{bcolors.ENDC}"
+                )
 
         df_gen = df_gen.reset_index(drop=True)
         return df_gen.head(n_samples)
 
-    def great_sample(self, starting_prompts: tp.Union[str, list[str]], temperature: float = 0.7, max_length: int = 100,
-                     device: str = "cuda") -> pd.DataFrame:
-        """ Generate synthetic tabular data samples conditioned on a given input.
+    def great_sample(
+        self,
+        starting_prompts: tp.Union[str, list[str]],
+        temperature: float = 0.7,
+        max_length: int = 100,
+        device: str = "cuda",
+    ) -> pd.DataFrame:
+        """Generate synthetic tabular data samples conditioned on a given input.
 
         Args:
             starting_prompts: String or List of Strings on which the output is conditioned.
              For example, "Sex is female, Age is 26"
             temperature: The generation samples each token from the probability distribution given by a softmax
              function. The temperature parameter controls the softmax function. A low temperature makes it sharper
              (0 equals greedy search), a high temperature brings more diversity but also uncertainty into the output.
@@ -194,34 +293,123 @@
 
          Returns:
             Pandas DataFrame with synthetic data generated based on starting_prompts
         """
         # ToDo: Add n_samples argument to generate more samples for one conditional input.
 
         self.model.to(device)
-        starting_prompts = [starting_prompts] if isinstance(starting_prompts, str) else starting_prompts
+        starting_prompts = (
+            [starting_prompts]
+            if isinstance(starting_prompts, str)
+            else starting_prompts
+        )
         generated_data = []
 
         # Generate a sample for each starting point
-        for prompt in tqdm(starting_prompts):
+        if len(starting_prompts) > 1:
+            loop_iter = tqdm(starting_prompts)
+        else:
+            loop_iter = starting_prompts
+        for prompt in loop_iter:
             start_token = torch.tensor(self.tokenizer(prompt)["input_ids"]).to(device)
 
             # Generate tokens
-            gen = self.model.generate(input_ids=torch.unsqueeze(start_token, 0), max_length=max_length,
-                                      do_sample=True, temperature=temperature, pad_token_id=50256)
+            gen = self.model.generate(
+                input_ids=torch.unsqueeze(start_token, 0),
+                max_length=max_length,
+                do_sample=True,
+                temperature=temperature,
+                pad_token_id=50256,
+            )
             generated_data.append(torch.squeeze(gen))
 
         # Convert Text back to Tabular Data
         decoded_data = _convert_tokens_to_text(generated_data, self.tokenizer)
-        df_gen = _convert_text_to_tabular_data(decoded_data, pd.DataFrame(columns=self.columns))
+        df_gen = _convert_text_to_tabular_data(
+            decoded_data, pd.DataFrame(columns=self.columns)
+        )
 
         return df_gen
 
+    def impute(
+        self,
+        df_miss: pd.DataFrame,
+        temperature: float = 0.7,
+        k: int = 100,
+        max_length: int = 100,
+        max_retries=15,
+        device: str = "cuda",
+    ) -> pd.DataFrame:
+        """Impute a DataFrame with missing values using a trained GReaT model.
+        Args:
+            df_miss: pandas data frame of the exact same format (column names, value ranges/types) as the data that
+             was used to train the GReaT model, however some values might be missing, which is indicated by the value of NaN.
+             This function will sample the missing values conditioned on the remaining values.
+            temperature: The generation samples each token from the probability distribution given by a softmax
+             function. The temperature parameter controls the softmax function. A low temperature makes it sharper
+             (0 equals greedy search), a high temperature brings more diversity but also uncertainty into the output.
+             See this blog article (https://huggingface.co/blog/how-to-generate) to read more about the generation
+             process
+            k: Sampling Batch Size. Set as high as possible. Speeds up the generation process significantly
+            max_length: Maximal number of tokens to generate - has to be long enough to not cut any information!
+            device: Set to "cpu" if the GPU should not be used. You can also specify the specific GPU to run on.
+
+        Returns:
+            Pandas DataFrame with n_samples rows of generated data
+        """
+
+        # Check DataFrame passed.
+        if set(df_miss.columns) != set(self.columns):
+            raise ValueError(
+                "The column names in the DataFrame passed to impute do not match the columns of the GReaT model."
+            )
+
+        self.model.to(device)
+
+        # start_token = torch.tensor(_pad_tokens(self.tokenizer(starting_prompts)["input_ids"])).to(device)
+        index = 0
+        df_list = []
+        with tqdm(total=len(df_miss)) as pbar:
+            while index < len(df_miss):
+                is_complete = False
+                retries = 0
+                df_curr = df_miss.iloc[[index]]
+                org_index = df_curr.index  # Keep index in new DataFrame
+                while not is_complete:
+                    num_attrs_missing = pd.isna(df_curr).sum().sum()
+                    # print("Number of missing values: ",  num_attrs_missing)
+                    # Generate text promt from current features.
+                    starting_prompts = _partial_df_to_promts(df_curr)
+                    df_curr = self.great_sample(
+                        starting_prompts, temperature, max_length, device=device
+                    )
+
+                    # Convert numerical values to float, flawed numerical values to NaN
+                    for i_num_cols in self.num_cols:
+                        df_curr[i_num_cols] = pd.to_numeric(
+                            df_curr[i_num_cols], errors="coerce"
+                        )
+                    df_curr[self.num_cols] = df_curr[self.num_cols].astype(np.float)
+
+                    # Check for missing values
+                    nans = df_curr.isna()
+                    if not df_curr.isna().any().any():
+                        is_complete = True
+                        df_list.append(df_curr.set_index(org_index))
+                    else:
+                        retries += 1
+                    if retries == max_retries:
+                        warnings.warn("Max retries reached.")
+                        break
+                index += 1
+                pbar.update(1)
+        return pd.concat(df_list, axis=0)
+
     def save(self, path: str):
-        """ Save GReaT Model
+        """Save GReaT Model
 
         Saves the model weights and a configuration file in the given directory.
 
         Args:
             path: Path where to save the model
         """
         # Make directory
@@ -234,34 +422,36 @@
         with open(path + "/config.json", "w") as f:
             attributes = self.__dict__.copy()
             attributes.pop("tokenizer")
             attributes.pop("model")
 
             # NDArray is not JSON serializable and therefore has to be converted into a list.
             if isinstance(attributes["conditional_col_dist"], np.ndarray):
-                attributes["conditional_col_dist"] = list(attributes["conditional_col_dist"])
+                attributes["conditional_col_dist"] = list(
+                    attributes["conditional_col_dist"]
+                )
 
             json.dump(attributes, f)
 
         # Save model weights
         torch.save(self.model.state_dict(), path + "/model.pt")
 
     def load_finetuned_model(self, path: str):
-        """ Load fine-tuned model
+        """Load fine-tuned model
 
         Load the weights of a fine-tuned large language model into the GReaT pipeline
 
         Args:
             path: Path to the fine-tuned model
         """
         self.model.load_state_dict(torch.load(path))
 
     @classmethod
     def load_from_dir(cls, path: str):
-        """ Load GReaT class
+        """Load GReaT class
 
         Load trained GReaT model from directory.
 
         Args:
             path: Directory where GReaT model is saved
 
         Returns:
@@ -286,35 +476,50 @@
         return great
 
     def _update_column_information(self, df: pd.DataFrame):
         # Update the column names (and numerical columns for some sanity checks after sampling)
         self.columns = df.columns.to_list()
         self.num_cols = df.select_dtypes(include=np.number).columns.to_list()
 
-    def _update_conditional_information(self, df: pd.DataFrame, conditional_col: tp.Optional[str] = None):
-        assert conditional_col is None or isinstance(conditional_col, str), \
-            f"The column name has to be a string and not {type(conditional_col)}"
-        assert conditional_col is None or conditional_col in df.columns, \
-            f"The column name {conditional_col} is not in the feature names of the given dataset"
+    def _update_conditional_information(
+        self, df: pd.DataFrame, conditional_col: tp.Optional[str] = None
+    ):
+        assert conditional_col is None or isinstance(
+            conditional_col, str
+        ), f"The column name has to be a string and not {type(conditional_col)}"
+        assert (
+            conditional_col is None or conditional_col in df.columns
+        ), f"The column name {conditional_col} is not in the feature names of the given dataset"
 
         # Take the distribution of the conditional column for a starting point in the generation process
         self.conditional_col = conditional_col if conditional_col else df.columns[-1]
         self.conditional_col_dist = _get_column_distribution(df, self.conditional_col)
 
-    def _get_start_sampler(self, start_col: tp.Optional[str],
-                           start_col_dist: tp.Optional[tp.Union[tp.Dict, tp.List]]) -> GReaTStart:
+    def _get_start_sampler(
+        self,
+        start_col: tp.Optional[str],
+        start_col_dist: tp.Optional[tp.Union[tp.Dict, tp.List]],
+    ) -> GReaTStart:
         if start_col and start_col_dist is None:
-            raise ValueError(f"Start column {start_col} was given, but no corresponding distribution.")
+            raise ValueError(
+                f"Start column {start_col} was given, but no corresponding distribution."
+            )
         if start_col_dist is not None and not start_col:
-            raise ValueError(f"Start column distribution {start_col} was given, the column name is missing.")
-
-        assert start_col is None or isinstance(start_col, str), \
-            f"The column name has to be a string and not {type(start_col)}"
-        assert start_col_dist is None or isinstance(start_col_dist, dict) or isinstance(start_col_dist, list), \
-            f"The distribution of the start column on has to be a list or a dict and not {type(start_col_dist)}"
+            raise ValueError(
+                f"Start column distribution {start_col} was given, the column name is missing."
+            )
+
+        assert start_col is None or isinstance(
+            start_col, str
+        ), f"The column name has to be a string and not {type(start_col)}"
+        assert (
+            start_col_dist is None
+            or isinstance(start_col_dist, dict)
+            or isinstance(start_col_dist, list)
+        ), f"The distribution of the start column on has to be a list or a dict and not {type(start_col_dist)}"
 
         start_col = start_col if start_col else self.conditional_col
         start_col_dist = start_col_dist if start_col_dist else self.conditional_col_dist
 
         if isinstance(start_col_dist, dict):
             return CategoricalStart(self.tokenizer, start_col, start_col_dist)
         elif isinstance(start_col_dist, list):
```

### Comparing `be_great-0.0.4/be_great/great_dataset.py` & `be_great-0.0.5/be_great/great_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,58 +3,68 @@
 
 from datasets import Dataset
 from dataclasses import dataclass
 from transformers import DataCollatorWithPadding
 
 
 class GReaTDataset(Dataset):
-    """ GReaT Dataset
+    """GReaT Dataset
 
     The GReaTDataset overwrites the _getitem function of the HuggingFace Dataset Class to include the permutation step.
 
     Attributes:
         tokenizer (AutoTokenizer): Tokenizer from HuggingFace
     """
+
     def set_tokenizer(self, tokenizer):
-        """ Set the Tokenizer
+        """Set the Tokenizer
 
         Args:
             tokenizer: Tokenizer from HuggingFace
         """
         self.tokenizer = tokenizer
 
-    def _getitem(self, key: tp.Union[int, slice, str], decoded: bool = True, **kwargs) -> tp.Union[tp.Dict, tp.List]:
-        """ Get Item from Tabular Data
+    def _getitem(
+        self, key: tp.Union[int, slice, str], decoded: bool = True, **kwargs
+    ) -> tp.Union[tp.Dict, tp.List]:
+        """Get Item from Tabular Data
 
         Get one instance of the tabular data, permuted, converted to text and tokenized.
         """
         # If int, what else?
         row = self._data.fast_slice(key, 1)
 
         shuffle_idx = list(range(row.num_columns))
         random.shuffle(shuffle_idx)
 
         shuffled_text = ", ".join(
-            ["%s is %s" % (row.column_names[i], str(row.columns[i].to_pylist()[0]).strip()) for i in shuffle_idx]
+            [
+                "%s is %s"
+                % (row.column_names[i], str(row.columns[i].to_pylist()[0]).strip())
+                for i in shuffle_idx
+            ]
         )
 
         tokenized_text = self.tokenizer(shuffled_text)
         return tokenized_text
+
     def __getitems__(self, keys: tp.Union[int, slice, str, list]):
         if isinstance(keys, list):
             return [self._getitem(key) for key in keys]
         else:
             return self._getitem(keys)
 
+
 @dataclass
 class GReaTDataCollator(DataCollatorWithPadding):
-    """ GReaT Data Collator
+    """GReaT Data Collator
 
     Overwrites the DataCollatorWithPadding to also pad the labels and not only the input_ids
     """
+
     def __call__(self, features: tp.List[tp.Dict[str, tp.Any]]):
         batch = self.tokenizer.pad(
             features,
             padding=self.padding,
             max_length=self.max_length,
             pad_to_multiple_of=self.pad_to_multiple_of,
             return_tensors=self.return_tensors,
```

### Comparing `be_great-0.0.4/be_great/great_start.py` & `be_great-0.0.5/be_great/great_start.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,57 +23,59 @@
     """
     max_length = len(max(tokens, key=len))
     tokens = [_pad(t, max_length) for t in tokens]
     return tokens
 
 
 class GReaTStart:
-    """ Abstract super class GReaT Start
+    """Abstract super class GReaT Start
 
     GReaT Start creates tokens to start the generation process.
 
     Attributes:
         tokenizer (AutoTokenizer): Tokenizer, automatically downloaded from llm-checkpoint
     """
+
     def __init__(self, tokenizer):
         """
         Initializes the super class.
 
         Args:
             tokenizer: Tokenizer from the HuggingFace library
         """
         self.tokenizer = tokenizer
 
     def get_start_tokens(self, n_samples: int) -> tp.List[tp.List[int]]:
-        """ Get Start Tokens
+        """Get Start Tokens
 
         Creates starting points for the generation process
 
         Args:
             n_samples: Number of start prompts to create
 
         Returns:
             List of n_sample lists with tokens
         """
         raise NotImplementedError("This has to be overwritten but the subclasses")
 
 
 class CategoricalStart(GReaTStart):
-    """ Categorical Starting Feature
+    """Categorical Starting Feature
 
     A categorical column with its categories is used as starting point.
 
     Attributes:
         start_col (str): Name of the categorical column
         population (list[str]): Possible values the column can take
         weights (list[float]): Probabilities for the individual categories
 
     """
+
     def __init__(self, tokenizer, start_col: str, start_col_dist: dict):
-        """ Initializes the Categorical Start
+        """Initializes the Categorical Start
 
         Args:
             tokenizer: Tokenizer from the HuggingFace library
             start_col: Name of the categorical column
             start_col_dist: Distribution of the categorical column (dict of form {"Cat A": 0.8, "Cat B": 0.2})
         """
         super().__init__(tokenizer)
@@ -89,27 +91,34 @@
         start_words = random.choices(self.population, self.weights, k=n_samples)
         start_text = [self.start_col + " is " + str(s) + "," for s in start_words]
         start_tokens = _pad_tokens(self.tokenizer(start_text)["input_ids"])
         return start_tokens
 
 
 class ContinuousStart(GReaTStart):
-    """ Continuous Starting Feature
+    """Continuous Starting Feature
 
     A continuous column with some noise is used as starting point.
 
     Attributes:
         start_col (str): Name of the continuous column
         start_col_dist (list[float]): The continuous column from the train data set
         noise (float): Size of noise that is added to each value
         decimal_places (int): Number of decimal places the continuous values have
     """
-    def __init__(self, tokenizer, start_col: str, start_col_dist: tp.List[float],
-                 noise: float = .01, decimal_places: int = 5):
-        """ Initializes the Continuous Start
+
+    def __init__(
+        self,
+        tokenizer,
+        start_col: str,
+        start_col_dist: tp.List[float],
+        noise: float = 0.01,
+        decimal_places: int = 5,
+    ):
+        """Initializes the Continuous Start
 
         Args:
             tokenizer: Tokenizer from the HuggingFace library
             start_col: Name of the continuous column
             start_col_dist: The continuous column from the train data set
             noise: Size of noise that is added to each value
             decimal_places: Number of decimal places the continuous values have
@@ -123,29 +132,33 @@
         self.start_col_dist = start_col_dist
         self.noise = noise
         self.decimal_places = decimal_places
 
     def get_start_tokens(self, n_samples):
         start_words = random.choices(self.start_col_dist, k=n_samples)
         # start_words += np.random.normal(size=n_samples) * self.noise  # add noise to start words
-        start_text = [self.start_col + " is " + format(s, f".{self.decimal_places}f") + "," for s in start_words]
+        start_text = [
+            self.start_col + " is " + format(s, f".{self.decimal_places}f") + ","
+            for s in start_words
+        ]
         start_tokens = _pad_tokens(self.tokenizer(start_text)["input_ids"])
         return start_tokens
 
 
 class RandomStart(GReaTStart):
-    """ Random Starting Features
+    """Random Starting Features
 
     Random column names are used as start point. Can be used if no distribution of any column is known.
 
     Attributes:
         all_columns (List[str]): Names of all columns
     """
+
     def __init__(self, tokenizer, all_columns: tp.List[str]):
-        """ Initializes the Random Start
+        """Initializes the Random Start
 
         Args:
             tokenizer: Tokenizer from the HuggingFace library
             all_columns: Names of all columns
         """
         super().__init__(tokenizer)
         self.all_columns = all_columns
```

### Comparing `be_great-0.0.4/be_great/great_trainer.py` & `be_great-0.0.5/be_great/great_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,28 @@
     random.seed(worker_seed)
     np.random.seed(worker_seed)
     torch.manual_seed(worker_seed)
     torch.cuda.manual_seed_all(worker_seed)
 
 
 class GReaTTrainer(Trainer):
-    """ GReaT Trainer
+    """GReaT Trainer
 
     Overwrites the get_train_dataloader methode of the HuggingFace Trainer to not remove the "unused" columns -
     they are needed later!
     """
+
     def get_train_dataloader(self) -> DataLoader:
         if self.train_dataset is None:
             raise ValueError("Trainer: training requires a train_dataset.")
 
         data_collator = self.data_collator
-        train_dataset = self.train_dataset  # self._remove_unused_columns(self.train_dataset, description="training")
+        train_dataset = (
+            self.train_dataset
+        )  # self._remove_unused_columns(self.train_dataset, description="training")
         train_sampler = self._get_train_sampler()
 
         return DataLoader(
             train_dataset,
             batch_size=self._train_batch_size,
             sampler=train_sampler,
             collate_fn=data_collator,
```

### Comparing `be_great-0.0.4/pyproject.toml` & `be_great-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "be_great"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Kathrin Sessler", email="kathrin.sessler@tum.de" },
 ]
 description = "Generating Realistic Tabular Data using Large Language Models"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
@@ -16,20 +16,21 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["great", "pytorch", "tabular data", "data generation", "transformer", "language models", "deep learning"]
 dependencies = [
     "datasets >= 2.5.2",
-    "numpy >= 1.24.1",
+    "numpy >= 1.24.2",
     "pandas >= 1.4.4",
     "scikit_learn >= 1.1.1",
     "torch >= 1.10.2",
     "tqdm >= 4.64.1",
-    "transformers >= 4.22.1"
+    "transformers >= 4.22.1",
+    "accelerate >= 0.20.1",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/kathrinse/be_great"
 "Documentation" = "https://kathrinse.github.io/be_great/"
 
 [tool.setuptools]
```

