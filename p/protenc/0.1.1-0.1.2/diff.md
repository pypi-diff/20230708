# Comparing `tmp/protenc-0.1.1.tar.gz` & `tmp/protenc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protenc-0.1.1.tar", max compression
+gzip compressed data, was "protenc-0.1.2.tar", max compression
```

## Comparing `protenc-0.1.1.tar` & `protenc-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1073 2022-11-28 21:45:10.255165 protenc-0.1.1/LICENSE
--rw-r--r--   0        0        0     4038 2022-11-28 22:05:03.400852 protenc-0.1.1/README.md
--rw-r--r--   0        0        0       76 2022-11-28 10:37:54.457085 protenc-0.1.1/protenc/__init__.py
--rw-r--r--   0        0        0        0 2022-11-28 21:46:34.360000 protenc-0.1.1/protenc/console/__init__.py
--rw-r--r--   0        0        0     8045 2022-11-29 11:13:02.991428 protenc-0.1.1/protenc/console/extract.py
--rw-r--r--   0        0        0     4694 2022-11-29 12:55:30.629741 protenc-0.1.1/protenc/io.py
--rw-r--r--   0        0        0     6299 2022-11-28 21:57:43.327507 protenc-0.1.1/protenc/models.py
--rw-r--r--   0        0        0     3252 2022-11-29 11:24:02.392340 protenc-0.1.1/protenc/utils.py
--rw-r--r--   0        0        0      598 2022-12-01 11:09:33.741370 protenc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5180 1970-01-01 00:00:00.000000 protenc-0.1.1/setup.py
--rw-r--r--   0        0        0     4867 1970-01-01 00:00:00.000000 protenc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-11-28 21:45:10.255165 protenc-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3912 2023-07-08 08:48:54.982857 protenc-0.1.2/README.md
+-rw-r--r--   0        0        0      115 2023-07-08 07:56:46.608131 protenc-0.1.2/protenc/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-28 21:46:34.360000 protenc-0.1.2/protenc/console/__init__.py
+-rw-r--r--   0        0        0     8045 2023-07-08 08:10:22.936689 protenc-0.1.2/protenc/console/extract.py
+-rw-r--r--   0        0        0     2828 2023-07-08 08:49:28.423231 protenc-0.1.2/protenc/encoder.py
+-rw-r--r--   0        0        0     4694 2022-11-29 12:55:30.629741 protenc-0.1.2/protenc/io.py
+-rw-r--r--   0        0        0     6396 2023-07-08 07:50:34.654201 protenc-0.1.2/protenc/models.py
+-rw-r--r--   0        0        0      192 2023-07-08 08:11:23.346052 protenc-0.1.2/protenc/types.py
+-rw-r--r--   0        0        0     3725 2023-07-08 07:43:19.325374 protenc-0.1.2/protenc/utils.py
+-rw-r--r--   0        0        0      696 2023-07-08 08:50:41.228062 protenc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5070 1970-01-01 00:00:00.000000 protenc-0.1.2/setup.py
+-rw-r--r--   0        0        0     4847 1970-01-01 00:00:00.000000 protenc-0.1.2/PKG-INFO
```

### Comparing `protenc-0.1.1/LICENSE` & `protenc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `protenc-0.1.1/README.md` & `protenc-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,62 +5,48 @@
 
 * [ProtTrans](https://github.com/agemagician/ProtTrans) family
 * [ESM](https://github.com/facebookresearch/esm)
 * AlphaFold (coming soon™)
 
 **Note:** the project is work in progress.
 
-Motivation
-----------
-
-
-
 Usage
 -----
 
 ### Installation
 
 ```bash
 pip install protenc
 ```
 
-**Note:** while ProtEnc depends on [pytorch](https://pytorch.org/), it is not part of the formal dependencies. 
-This is due to the large number of different pytorch distributions which may mismatch with the target environment.
+**Note:** while ProtEnc depends on [PyTorch](https://pytorch.org/), it is not part of the formal project dependencies. 
+This is due to the large number of different PyTorch distributions which may mismatch with the target environment.
+It therefore has be installed manually.
 
 ### Python API
 
 ```python
 import protenc
-import torch
 
 # List available models
 print(protenc.list_models())
 
-# Instantiate a model
-model = protenc.get_model('esm2_t33_650M_UR50D')
+# Load encoder model
+encoder = protenc.get_encoder('esm2_t30_150M_UR50D', device='cuda')
 
 proteins = [
   'MKTVRQERLKSIVRILERSKEPVSGAQLAEELSVSRQVIVQDIAYLRSLGYNIVATPRGYVLAGG',
   'KALTARQQEVFDLIRDHISQTGMPPTRAEIAQRLGFRSPNAAEEHLKALARKGVIEIVSGASRGIRLLQEE'
 ]
 
-batch = model.prepare_sequences(proteins)
-
-# Use GPU if available
-if torch.cuda.is_available():
-  model = model.to('cuda')
-  batch = protenc.utils.to_device(batch, 'cuda')
-
-for embed in model(batch):
-  # Embeddings have shape [L, D] where L is the sequence length and D the 
-  # embedding dimensionality.
+for embed in encoder(proteins, return_format='numpy'):
+  # Embeddings have shape [L, D] where L is the sequence length and D the  embedding dimensionality.
   print(embed.shape)
   
-  # Derive a single per-protein embedding vector by averaging along the 
-  # sequence dimension
+  # Derive a single per-protein embedding vector by averaging along the sequence dimension
   embed.mean(0)
 ```
 
 ### Command-line interface
 
 After installation, use the `protenc` shell command for bulk generation and export of protein embeddings.
```

### Comparing `protenc-0.1.1/protenc/console/extract.py` & `protenc-0.1.2/protenc/console/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import protenc
 
 from functools import partial
 from pathlib import Path
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 from protenc import io as io, utils
-from protenc.models import EmbeddingKind
+from protenc.models import EmbeddingType
 
 
 def get_input_reader_cls(args):
     input_path = Path(args.input_path)
     infer = args.input_format in [None, 'infer']
     if infer:
         input_format = input_path.suffix[1:]
@@ -93,15 +93,15 @@
         for labels, sequences in batches:
             sequences = utils.to_device(sequences, args.device)
             output = model(sequences)
 
             for label, embedding in zip(labels, output):
                 embedding = embedding.cpu().numpy()
 
-                if args.compute_mean and model.embedding_kind == EmbeddingKind.PER_RESIDUE:
+                if args.compute_mean and model.embedding_kind == EmbeddingType.PER_RESIDUE:
                     assert embedding.ndim == 2
                     embedding = embedding.mean(0)
 
                 if args.cast_to:
                     embedding = embedding.astype(args.cast_to)
 
                 if not args.dry_run:
```

### Comparing `protenc-0.1.1/protenc/io.py` & `protenc-0.1.2/protenc/io.py`

 * *Files identical despite different names*

### Comparing `protenc-0.1.1/protenc/models.py` & `protenc-0.1.2/protenc/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     BertModel,
     BertTokenizer,
     T5EncoderModel,
     T5Tokenizer
 )
 
 
-class EmbeddingKind(Enum):
+class EmbeddingType(Enum):
     PER_RESIDUE = 'per_residue'
     PER_PROTEIN = 'per_protein'
 
 
 class BaseProteinEmbeddingModel(nn.Module):
-    embedding_kind: EmbeddingKind
+    embedding_type: EmbeddingType
 
     def prepare_sequences(self, sequences):
         return NotImplementedError
 
     def forward(self, input):
         raise NotImplementedError
 
@@ -36,15 +36,15 @@
         config = model_cls.config_class.from_pretrained(model_name)
         model = model_cls(config)
         tokenizer = tokenizer_cls.from_pretrained(model_name)
         return model, tokenizer
 
 
 class BaseProtTransEmbeddingModel(BaseProteinEmbeddingModel):
-    embedding_kind = EmbeddingKind.PER_RESIDUE
+    embedding_kind = EmbeddingType.PER_RESIDUE
     available_models = None
 
     def __init__(self, model, tokenizer):
         super().__init__()
         self.model = model
         self.model.eval()
         self.tokenizer = tokenizer
@@ -131,15 +131,15 @@
         super().__init__(model=model, tokenizer=tokenizer)
 
     def _post_process_embedding(self, embedding, seq_len):
         return embedding[:seq_len - 1]
 
 
 class ESMEmbeddingModel(BaseProteinEmbeddingModel):
-    embedding_kind = EmbeddingKind.PER_RESIDUE
+    embedding_kind = EmbeddingType.PER_RESIDUE
 
     def __init__(self, model_name: str, repr_layer: int):
         super().__init__()
 
         self.model, self.alphabet = torch.hub.load('facebookresearch/esm:main', model_name)
         self.model.eval()
         self.batch_converter = self.alphabet.get_batch_converter()
@@ -181,9 +181,14 @@
 ])
 
 
 def list_models():
     return list(embedding_models)
 
 
-def get_model(model_name):
-    return embedding_models[model_name]()
+def get_model(model_name, device=None):
+    model = embedding_models[model_name]()
+
+    if device is not None:
+        model = model.to(device)
+    
+    return model
```

### Comparing `protenc-0.1.1/protenc/utils.py` & `protenc-0.1.2/protenc/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import hashlib
 import pickle
 import random
 import re
-
+import numpy as np
 import lmdb
 import torch
 
 from itertools import chain
 from collections.abc import Mapping
 from humanfriendly import parse_size
 
@@ -84,14 +84,34 @@
 def read_from_lmdb(path):
     with lmdb.open(str(path), readonly=True) as env:
         with env.begin() as txn, txn.cursor() as cursor:
             for key, value in cursor.iternext():
                 yield key.decode(), pickle.loads(value)
 
 
+return_formats = {
+    'torch': (torch.Tensor, torch.tensor),
+    'numpy': (np.ndarray, np.array)
+}
+
+def to_return_format(x, return_format):
+    format = return_formats.get(return_format)
+
+    if format is None:
+        raise ValueError(f'Unknown return format {return_format}. '
+                         f'Supported formats are {list(return_formats)}')
+    
+    cls, cast_fn = format
+
+    if isinstance(x, cls):
+        return x
+
+    return cast_fn(x)
+
+
 class IteratorWrapper(IterableDataset):
     def __init__(self, it):
         self.it = it
 
     def __iter__(self):
         yield from self.it
```

### Comparing `protenc-0.1.1/pyproject.toml` & `protenc-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "protenc"
-version = "0.1.1"
+version = "0.1.2"
 description = "Extract protein embeddings from pretrained models."
 authors = ["Kristian Klemon <kristian.klemon@gmail.com>"]
 readme = "README.md"
 packages = [{include = "protenc"}]
+repository = "https://github.com/kklemon/ProtEnc"
+homepage = "https://github.com/kklemon/ProtEnc"
 
 [tool.poetry.scripts]
 protenc = 'protenc.console.extract:entrypoint'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 transformers = "^4.24.0"
```

### Comparing `protenc-0.1.1/setup.py` & `protenc-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,22 @@
  'transformers>=4.24.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['protenc = protenc.console.extract:entrypoint']}
 
 setup_kwargs = {
     'name': 'protenc',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Extract protein embeddings from pretrained models.',
-    'long_description': "ProtEnc: generate protein embeddings the easy way\n=======\n\n[ProtEnc](https://github.com/kklemon/ProtEnc) aims to simplify extraction of protein embeddings from various pre-trained models by providing simple APIs and bulk generation scripts for the ever-growing jungle of protein language models (pLMs). Currently, supported models are:\n\n* [ProtTrans](https://github.com/agemagician/ProtTrans) family\n* [ESM](https://github.com/facebookresearch/esm)\n* AlphaFold (coming soon™)\n\n**Note:** the project is work in progress.\n\nMotivation\n----------\n\n\n\nUsage\n-----\n\n### Installation\n\n```bash\npip install protenc\n```\n\n**Note:** while ProtEnc depends on [pytorch](https://pytorch.org/), it is not part of the formal dependencies. \nThis is due to the large number of different pytorch distributions which may mismatch with the target environment.\n\n### Python API\n\n```python\nimport protenc\nimport torch\n\n# List available models\nprint(protenc.list_models())\n\n# Instantiate a model\nmodel = protenc.get_model('esm2_t33_650M_UR50D')\n\nproteins = [\n  'MKTVRQERLKSIVRILERSKEPVSGAQLAEELSVSRQVIVQDIAYLRSLGYNIVATPRGYVLAGG',\n  'KALTARQQEVFDLIRDHISQTGMPPTRAEIAQRLGFRSPNAAEEHLKALARKGVIEIVSGASRGIRLLQEE'\n]\n\nbatch = model.prepare_sequences(proteins)\n\n# Use GPU if available\nif torch.cuda.is_available():\n  model = model.to('cuda')\n  batch = protenc.utils.to_device(batch, 'cuda')\n\nfor embed in model(batch):\n  # Embeddings have shape [L, D] where L is the sequence length and D the \n  # embedding dimensionality.\n  print(embed.shape)\n  \n  # Derive a single per-protein embedding vector by averaging along the \n  # sequence dimension\n  embed.mean(0)\n```\n\n### Command-line interface\n\nAfter installation, use the `protenc` shell command for bulk generation and export of protein embeddings.\n\n```bash\nprotenc <path-to-protein-sequences> <path-to-output> --model_name=<name-of-model>\n```\n\nBy default, input and output formats are inferred from the file extensions.\n\nRun\n\n```bash\nprotenc --help\n```\n\nfor a detailed usage description.\n\n**Example**\n\nGenerate protein embeddings using the ESM2 650M model for sequences provided in a [FASTA](https://en.wikipedia.org/wiki/FASTA_format) file and write embeddings to an [LMDB](https://en.wikipedia.org/wiki/Lightning_Memory-Mapped_Database):\n\n```bash\nprotenc proteins.fasta embeddings.lmdb --model_name=esm2_t33_650M_UR50D\n```\n\nThe generated embeddings will be stored in a lmdb key-value store and can be easily accessed using the `read_from_lmdb` utility function:\n\n```python\nfrom protenc.utils import read_from_lmdb\n\nfor label, embed in read_from_lmdb('embeddings.lmdb'):\n    print(label, embed)\n```\n\n**Features**\n\nInput formats:\n* CSV\n* JSON\n* [FASTA](https://en.wikipedia.org/wiki/FASTA_format)\n\nOutput format:\n* [LMDB](https://en.wikipedia.org/wiki/Lightning_Memory-Mapped_Database)\n* [HDF5](https://en.wikipedia.org/wiki/Hierarchical_Data_Format) (coming soon)\n\nGeneral:\n* Multi-GPU inference with (`--data_parallel`)\n* FP16 inference (`--amp`)\n\nDevelopment\n-----------\n\nClone the repository:\n\n```bash\ngit clone git+https://github.com/kklemon/protenc.git\n```\n\nInstall dependencies via [Poetry](https://python-poetry.org/):\n\n```bash\npoetry install\n```\n\nContribution\n------------\n\nHave feature ideas or found a bug? Love to see support for a new model? Feel free to [create an issue](https://github.com/kklemon/ProtEnc/issues/new).\n\nTodo\n----\n\n- [ ] Support for more input formats\n  - [X] CSV\n  - [ ] Parquet\n  - [X] FASTA\n  - [X] JSON\n- [ ] Support for more output formats\n  - [X] LMDB\n  - [ ] HDF5\n  - [ ] DataFrame\n  - [ ] Pickle\n- [ ] Large models support\n  - [ ] Model offloading\n  - [ ] Sharding\n- [ ] Support for more protein language models\n  - [X] Whole ProtTrans family\n  - [X] Whole ESM family\n  - [ ] AlphaFold (?)\n- [X] Implement all remaining TODOs in code\n- [ ] Distributed inference\n- [ ] Maybe support some sort of optimized inference such as quantization\n  - This may be up to the model providers\n- [ ] Improve documentation\n- [ ] Support translation of gene sequences\n- [ ] Add tests. We need tests!!!",
+    'long_description': "ProtEnc: generate protein embeddings the easy way\n=======\n\n[ProtEnc](https://github.com/kklemon/ProtEnc) aims to simplify extraction of protein embeddings from various pre-trained models by providing simple APIs and bulk generation scripts for the ever-growing jungle of protein language models (pLMs). Currently, supported models are:\n\n* [ProtTrans](https://github.com/agemagician/ProtTrans) family\n* [ESM](https://github.com/facebookresearch/esm)\n* AlphaFold (coming soon™)\n\n**Note:** the project is work in progress.\n\nUsage\n-----\n\n### Installation\n\n```bash\npip install protenc\n```\n\n**Note:** while ProtEnc depends on [PyTorch](https://pytorch.org/), it is not part of the formal project dependencies. \nThis is due to the large number of different PyTorch distributions which may mismatch with the target environment.\nIt therefore has be installed manually.\n\n### Python API\n\n```python\nimport protenc\n\n# List available models\nprint(protenc.list_models())\n\n# Load encoder model\nencoder = protenc.get_encoder('esm2_t30_150M_UR50D', device='cuda')\n\nproteins = [\n  'MKTVRQERLKSIVRILERSKEPVSGAQLAEELSVSRQVIVQDIAYLRSLGYNIVATPRGYVLAGG',\n  'KALTARQQEVFDLIRDHISQTGMPPTRAEIAQRLGFRSPNAAEEHLKALARKGVIEIVSGASRGIRLLQEE'\n]\n\nfor embed in encoder(proteins, return_format='numpy'):\n  # Embeddings have shape [L, D] where L is the sequence length and D the  embedding dimensionality.\n  print(embed.shape)\n  \n  # Derive a single per-protein embedding vector by averaging along the sequence dimension\n  embed.mean(0)\n```\n\n### Command-line interface\n\nAfter installation, use the `protenc` shell command for bulk generation and export of protein embeddings.\n\n```bash\nprotenc <path-to-protein-sequences> <path-to-output> --model_name=<name-of-model>\n```\n\nBy default, input and output formats are inferred from the file extensions.\n\nRun\n\n```bash\nprotenc --help\n```\n\nfor a detailed usage description.\n\n**Example**\n\nGenerate protein embeddings using the ESM2 650M model for sequences provided in a [FASTA](https://en.wikipedia.org/wiki/FASTA_format) file and write embeddings to an [LMDB](https://en.wikipedia.org/wiki/Lightning_Memory-Mapped_Database):\n\n```bash\nprotenc proteins.fasta embeddings.lmdb --model_name=esm2_t33_650M_UR50D\n```\n\nThe generated embeddings will be stored in a lmdb key-value store and can be easily accessed using the `read_from_lmdb` utility function:\n\n```python\nfrom protenc.utils import read_from_lmdb\n\nfor label, embed in read_from_lmdb('embeddings.lmdb'):\n    print(label, embed)\n```\n\n**Features**\n\nInput formats:\n* CSV\n* JSON\n* [FASTA](https://en.wikipedia.org/wiki/FASTA_format)\n\nOutput format:\n* [LMDB](https://en.wikipedia.org/wiki/Lightning_Memory-Mapped_Database)\n* [HDF5](https://en.wikipedia.org/wiki/Hierarchical_Data_Format) (coming soon)\n\nGeneral:\n* Multi-GPU inference with (`--data_parallel`)\n* FP16 inference (`--amp`)\n\nDevelopment\n-----------\n\nClone the repository:\n\n```bash\ngit clone git+https://github.com/kklemon/protenc.git\n```\n\nInstall dependencies via [Poetry](https://python-poetry.org/):\n\n```bash\npoetry install\n```\n\nContribution\n------------\n\nHave feature ideas or found a bug? Love to see support for a new model? Feel free to [create an issue](https://github.com/kklemon/ProtEnc/issues/new).\n\nTodo\n----\n\n- [ ] Support for more input formats\n  - [X] CSV\n  - [ ] Parquet\n  - [X] FASTA\n  - [X] JSON\n- [ ] Support for more output formats\n  - [X] LMDB\n  - [ ] HDF5\n  - [ ] DataFrame\n  - [ ] Pickle\n- [ ] Large models support\n  - [ ] Model offloading\n  - [ ] Sharding\n- [ ] Support for more protein language models\n  - [X] Whole ProtTrans family\n  - [X] Whole ESM family\n  - [ ] AlphaFold (?)\n- [X] Implement all remaining TODOs in code\n- [ ] Distributed inference\n- [ ] Maybe support some sort of optimized inference such as quantization\n  - This may be up to the model providers\n- [ ] Improve documentation\n- [ ] Support translation of gene sequences\n- [ ] Add tests. We need tests!!!",
     'author': 'Kristian Klemon',
     'author_email': 'kristian.klemon@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/kklemon/ProtEnc',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `protenc-0.1.1/PKG-INFO` & `protenc-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: protenc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extract protein embeddings from pretrained models.
+Home-page: https://github.com/kklemon/ProtEnc
 Author: Kristian Klemon
 Author-email: kristian.klemon@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,75 +15,62 @@
 Requires-Dist: humanfriendly (>=10.0,<11.0)
 Requires-Dist: json-stream (>=2.1.1,<3.0.0)
 Requires-Dist: lmdb (>=1.3.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: sentencepiece (>=0.1.97,<0.2.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: transformers (>=4.24.0,<5.0.0)
+Project-URL: Repository, https://github.com/kklemon/ProtEnc
 Description-Content-Type: text/markdown
 
 ProtEnc: generate protein embeddings the easy way
 =======
 
 [ProtEnc](https://github.com/kklemon/ProtEnc) aims to simplify extraction of protein embeddings from various pre-trained models by providing simple APIs and bulk generation scripts for the ever-growing jungle of protein language models (pLMs). Currently, supported models are:
 
 * [ProtTrans](https://github.com/agemagician/ProtTrans) family
 * [ESM](https://github.com/facebookresearch/esm)
 * AlphaFold (coming soon™)
 
 **Note:** the project is work in progress.
 
-Motivation
-----------
-
-
-
 Usage
 -----
 
 ### Installation
 
 ```bash
 pip install protenc
 ```
 
-**Note:** while ProtEnc depends on [pytorch](https://pytorch.org/), it is not part of the formal dependencies. 
-This is due to the large number of different pytorch distributions which may mismatch with the target environment.
+**Note:** while ProtEnc depends on [PyTorch](https://pytorch.org/), it is not part of the formal project dependencies. 
+This is due to the large number of different PyTorch distributions which may mismatch with the target environment.
+It therefore has be installed manually.
 
 ### Python API
 
 ```python
 import protenc
-import torch
 
 # List available models
 print(protenc.list_models())
 
-# Instantiate a model
-model = protenc.get_model('esm2_t33_650M_UR50D')
+# Load encoder model
+encoder = protenc.get_encoder('esm2_t30_150M_UR50D', device='cuda')
 
 proteins = [
   'MKTVRQERLKSIVRILERSKEPVSGAQLAEELSVSRQVIVQDIAYLRSLGYNIVATPRGYVLAGG',
   'KALTARQQEVFDLIRDHISQTGMPPTRAEIAQRLGFRSPNAAEEHLKALARKGVIEIVSGASRGIRLLQEE'
 ]
 
-batch = model.prepare_sequences(proteins)
-
-# Use GPU if available
-if torch.cuda.is_available():
-  model = model.to('cuda')
-  batch = protenc.utils.to_device(batch, 'cuda')
-
-for embed in model(batch):
-  # Embeddings have shape [L, D] where L is the sequence length and D the 
-  # embedding dimensionality.
+for embed in encoder(proteins, return_format='numpy'):
+  # Embeddings have shape [L, D] where L is the sequence length and D the  embedding dimensionality.
   print(embed.shape)
   
-  # Derive a single per-protein embedding vector by averaging along the 
-  # sequence dimension
+  # Derive a single per-protein embedding vector by averaging along the sequence dimension
   embed.mean(0)
 ```
 
 ### Command-line interface
 
 After installation, use the `protenc` shell command for bulk generation and export of protein embeddings.
```

