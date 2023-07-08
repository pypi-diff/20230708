# Comparing `tmp/hirakanadic-0.0.3.tar.gz` & `tmp/hirakanadic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hirakanadic-0.0.3.tar", max compression
+gzip compressed data, was "hirakanadic-0.0.4.tar", max compression
```

## Comparing `hirakanadic-0.0.3.tar` & `hirakanadic-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1148 2021-06-22 12:43:01.050287 hirakanadic-0.0.3/README.md
--rw-r--r--   0        0        0     2835 2021-06-22 16:07:36.155164 hirakanadic-0.0.3/hirakanadic/cli.py
--rw-r--r--   0        0        0      572 2021-06-22 16:08:48.863494 hirakanadic-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2004 2021-06-22 16:09:10.025963 hirakanadic-0.0.3/setup.py
--rw-r--r--   0        0        0     1880 2021-06-22 16:09:10.026293 hirakanadic-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1148 2023-06-26 16:31:17.676657 hirakanadic-0.0.4/README.md
+-rw-r--r--   0        0        0     2830 2023-07-08 08:18:58.796524 hirakanadic-0.0.4/hirakanadic/cli.py
+-rw-r--r--   0        0        0      573 2023-07-08 08:19:58.120152 hirakanadic-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1782 1970-01-01 00:00:00.000000 hirakanadic-0.0.4/PKG-INFO
```

### Comparing `hirakanadic-0.0.3/README.md` & `hirakanadic-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hirakanadic-0.0.3/hirakanadic/cli.py` & `hirakanadic-0.0.4/hirakanadic/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             self.split_mode = tokenizer.Tokenizer.SplitMode.A
         if split_mode == "B":
             self.split_mode = tokenizer.Tokenizer.SplitMode.B
         if split_mode == "C":
             self.split_mode = tokenizer.Tokenizer.SplitMode.C
 
         self.tokenizer = dictionary.Dictionary(
-            dict_type=dict_type, config_path=sudachi_setting
+            dict=dict_type, config_path=sudachi_setting
         ).create()
 
         self.already = []
 
     def convert(
         self, text: str, left_id: int = 5646, right_id: int = 5646, cost: int = 7000
     ) -> str:
```

### Comparing `hirakanadic-0.0.3/pyproject.toml` & `hirakanadic-0.0.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "hirakanadic"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["po3rin"]
 repository = "http://github.com/po3rin/hirakanadic"
 homepage = "http://github.com/po3rin/hirakanadic"
 readme = "README.md"
 license = "Apache-2.0"
 
 [tool.poetry.scripts]
 hirakanadic = "hirakanadic.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-sudachipy = "^0.5.2"
-sudachidict_full = "^20210608"
-SudachiDict-core = "^20210608"
+python = "^3.11"
+sudachipy = "^0.6.7"
+sudachidict-core = "^20230110"
+sudachidict-full = "^20230110"
 jaconv = "^0.2.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.1"
 
 [build-system]
 requires = ["poetry>=0.12"]
```

### Comparing `hirakanadic-0.0.3/setup.py` & `hirakanadic-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,54 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hirakanadic
+Version: 0.0.4
+Summary: 
+Home-page: http://github.com/po3rin/hirakanadic
+License: Apache-2.0
+Author: po3rin
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: jaconv (>=0.2.4,<0.3.0)
+Requires-Dist: sudachidict-core (>=20230110,<20230111)
+Requires-Dist: sudachidict-full (>=20230110,<20230111)
+Requires-Dist: sudachipy (>=0.6.7,<0.7.0)
+Project-URL: Repository, http://github.com/po3rin/hirakanadic
+Description-Content-Type: text/markdown
+
+# hirakanadic
+
+[![PyPi version](https://img.shields.io/pypi/v/hirakanadic.svg)](https://pypi.python.org/pypi/hirakanadic/)
+![PyTest](https://github.com/po3rin/hirakanadic/workflows/PyTest/badge.svg)
+[![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-390/)
+
+## Install
+
+```sh
+$ pip install hirakanadic
+```
+
+## Usage
+
+```sh
+$ hirakanadic example/input.txt -o out.txt
+```
+
+input file
+
+```
+コレステロール値
+陰のうヘルニア
+濾胞性リンパ腫
+コリネバクテリウム・ウルセランス感染症
+```
+
+result
+
+```
+これすてろーる,5146,5146,7000,これすてろーる,名詞,普通名詞,一般,*,*,*,コレステロール,コレステロール,*,*,*,*,*
+へるにあ,5146,5146,7000,へるにあ,名詞,普通名詞,一般,*,*,*,ヘルニア,ヘルニア,*,*,*,*,*
+こりねばくてりうむ,5146,5146,7000,こりねばくてりうむ,名詞,普通名詞,一般,*,*,*,コリネバクテリウム,コリネバクテリウム,*,*,*,*,*
+うるせらんす,5146,5146,7000,うるせらんす,名詞,普通名詞,一般,*,*,*,ウルセランス,ウルセランス,*,*,*,*,*
+```
 
-packages = \
-['hirakanadic']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['SudachiDict-core>=20210608,<20210609',
- 'jaconv>=0.2.4,<0.3.0',
- 'sudachidict_full>=20210608,<20210609',
- 'sudachipy>=0.5.2,<0.6.0']
-
-entry_points = \
-{'console_scripts': ['hirakanadic = hirakanadic.cli:cli']}
-
-setup_kwargs = {
-    'name': 'hirakanadic',
-    'version': '0.0.3',
-    'description': '',
-    'long_description': '# hirakanadic\n\n[![PyPi version](https://img.shields.io/pypi/v/hirakanadic.svg)](https://pypi.python.org/pypi/hirakanadic/)\n![PyTest](https://github.com/po3rin/hirakanadic/workflows/PyTest/badge.svg)\n[![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-390/)\n\n## Install\n\n```sh\n$ pip install hirakanadic\n```\n\n## Usage\n\n```sh\n$ hirakanadic example/input.txt -o out.txt\n```\n\ninput file\n\n```\nコレステロール値\n陰のうヘルニア\n濾胞性リンパ腫\nコリネバクテリウム・ウルセランス感染症\n```\n\nresult\n\n```\nこれすてろーる,5146,5146,7000,これすてろーる,名詞,普通名詞,一般,*,*,*,コレステロール,コレステロール,*,*,*,*,*\nへるにあ,5146,5146,7000,へるにあ,名詞,普通名詞,一般,*,*,*,ヘルニア,ヘルニア,*,*,*,*,*\nこりねばくてりうむ,5146,5146,7000,こりねばくてりうむ,名詞,普通名詞,一般,*,*,*,コリネバクテリウム,コリネバクテリウム,*,*,*,*,*\nうるせらんす,5146,5146,7000,うるせらんす,名詞,普通名詞,一般,*,*,*,ウルセランス,ウルセランス,*,*,*,*,*\n```\n',
-    'author': 'po3rin',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'http://github.com/po3rin/hirakanadic',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

