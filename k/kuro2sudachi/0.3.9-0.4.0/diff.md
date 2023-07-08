# Comparing `tmp/kuro2sudachi-0.3.9.tar.gz` & `tmp/kuro2sudachi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuro2sudachi-0.3.9.tar", max compression
+gzip compressed data, was "kuro2sudachi-0.4.0.tar", max compression
```

## Comparing `kuro2sudachi-0.3.9.tar` & `kuro2sudachi-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2904 2023-06-26 15:47:20.263852 kuro2sudachi-0.3.9/README.md
--rw-r--r--   0        0        0      676 2023-07-07 19:21:29.605898 kuro2sudachi-0.3.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.3.9/src/kuro2sudachi/__init__.py
--rw-r--r--   0        0        0     6433 2023-07-07 19:21:20.419418 kuro2sudachi-0.3.9/src/kuro2sudachi/core.py
--rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.3.9/src/kuro2sudachi/normalizer.py
--rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.3.9/src/kuro2sudachi/rewrite.def
--rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 kuro2sudachi-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     2851 2023-07-08 16:34:19.105217 kuro2sudachi-0.4.0/README.md
+-rw-r--r--   0        0        0      694 2023-07-08 16:34:19.115112 kuro2sudachi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.4.0/src/kuro2sudachi/__init__.py
+-rw-r--r--   0        0        0     7051 2023-07-08 16:34:19.117661 kuro2sudachi-0.4.0/src/kuro2sudachi/core.py
+-rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.4.0/src/kuro2sudachi/normalizer.py
+-rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.4.0/src/kuro2sudachi/rewrite.def
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 kuro2sudachi-0.4.0/PKG-INFO
```

### Comparing `kuro2sudachi-0.3.9/README.md` & `kuro2sudachi-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "cost": 5000
     }
 }
 
 ```
 
 ```$
-$ kuro2sudachi kuromoji_dict.txt -o sudachi_user_dict.txt -c convert_config.json
+$ kuro2sudachi kuromoji_dict.txt -o sudachi_user_dict.txt -c kuro2sudachi.json
 ```
 
 if you want to ignore unsupported pos error & invalid format, use `--ignore` flag.
 
 ## Dictionary type
 
 You can specify the dictionary with the tokenize option -s (default: core).
@@ -72,15 +72,15 @@
 output includes unit devision info.
 
 ```sh
 $ cat kuromoji_dict.txt
 融合たんぱく質,融合たんぱく質,融合たんぱく質,名詞
 発作性心房細動,発作性心房細動,発作性心房細動,名詞
 
-$ kuro2sudachi kuromoji_dict.txt -o sudachi_user_dict.txt -c convert_config.json --ignore
+$ kuro2sudachi kuromoji_dict.txt -o sudachi_user_dict.txt -c kuro2sudachi.json --ignore
 
 $ cat sudachi_user_dict.txt
 融合たんぱく質,4786,4786,5000,融合たんぱく質,名詞,普通名詞,一般,*,*,*,,融合たんぱく質,*,C,*,660881/810248,*
 発作性心房細動,4786,4786,5000,発作性心房細動,名詞,普通名詞,一般,*,*,*,,発作性心房細動,*,C,584006/434835/428494/619020,2756385/428494/619020,*
 ```
 
 ## Splitting Words defined by kuromoji
@@ -103,12 +103,7 @@
 ```
 
 exec kuro2sudachi command
 
 ```sh
 $ poetry run kuro2sudachi tests/kuromoji_dict_test.txt -o sudachi_user_dict.txt
 ```
-
-## TODO
-
-- [ ] split mode
-- [ ] default rewrite
```

### Comparing `kuro2sudachi-0.3.9/pyproject.toml` & `kuro2sudachi-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuro2sudachi"
-version = "0.3.9"
+version = "0.4.0"
 description = ""
 authors = ["po3rin"]
 repository = "http://github.com/po3rin/kuro2sudachi"
 homepage = "http://github.com/po3rin/kuro2sudachi"
 readme = "README.md"
 license = "Apache-2.0"
 include = ["rewrite.def"]
@@ -20,11 +20,12 @@
 sudachidict-core = "^20230110"
 sudachidict-full = "^20230110"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^6.2.1"
 twine = "^4.0.2"
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `kuro2sudachi-0.3.9/src/kuro2sudachi/core.py` & `kuro2sudachi-0.4.0/src/kuro2sudachi/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from sudachipy import dictionary, tokenizer
-from kuro2sudachi.normalizer import SudachiCharNormalizer
-import jaconv
-import fileinput
 import argparse
+import fileinput
 import json
 import os
 import re
+from dataclasses import dataclass
+
+import jaconv
+from sudachipy import dictionary, tokenizer
 
+from kuro2sudachi.normalizer import SudachiCharNormalizer
 
 mode = tokenizer.Tokenizer.SplitMode.C
 
 parser = argparse.ArgumentParser(
     description="convert kuromoji user dict to sudacchi user dict"
 )
 parser.add_argument("file", help="kuromoji dict file path")
@@ -30,16 +32,17 @@
     "--rm_already_exist",
     action="store_true",
     help="remove words system dict already exist",
 )
 parser.add_argument("-r", "--sudachi_setting", help="the setting file in JSON format")
 parser.add_argument("-s", "--sudachi_dict_type", help="sudachidict type")
 parser.add_argument(
-    "-m",
-    "--merge_dict",
+    "-u",
+    "--unit_word_dict",
+    default="",
     help="A dictionary for split registration of words that are not in the system dictionary. Must be specified as a user dictionary in sudachi's configuration file (json).",
 )
 parser.add_argument(
     "--ignore",
     action="store_true",
     help="ignore invalid format line / unsupported pos error / oov error in splitted word",
 )
@@ -74,40 +77,48 @@
     pass
 
 
 class OOVError(Error):
     pass
 
 
+@dataclass
+class UnitWord:
+    word_id: int
+    line: str
+
+
 class Converter:
     def __init__(
         self,
         rewrite_file,
         config=None,
         sudachi_setting=None,
         dict_type="core",
         rm=False,
+        unit_words_dict: dict[str, UnitWord] = {},
     ):
         if rewrite_file == "":
             raise DictFormatError("rewrite.def file path is required")
 
         self.tokenizer = dictionary.Dictionary(
-            dict=dict_type, config_path=sudachi_setting
+            config_path=sudachi_setting, dict=dict_type
         ).create()
 
         if config is not None:
             with open(config) as f:
                 s = json.load(f)
         else:
             s = default_setting
 
         self.rewrite = rewrite_file
         self.setting = s
         self.rm = rm
         self.normalizer = SudachiCharNormalizer(rewrite_def_path=self.rewrite)
+        self.unit_words_dict = unit_words_dict
 
     def convert(self, line: str) -> str:
         data = line.split(",")
         try:
             word = data[0]
             # splited = data[1]
             yomi = self.nomlized_yomi(data[2].replace(" ", ""))
@@ -154,15 +165,18 @@
             if ",".join(m.part_of_speech()) == "名詞,数詞,*,*,*,*":
                 return "*"
 
             if m.is_oov() or m.dictionary_id() == -1:
                 oov.append(m.surface())
                 continue
 
-            word_ids.append(str(m.word_id()))
+            if str(m) in self.unit_words_dict:
+                word_ids.append(f"U{str(self.unit_words_dict[str(m)].word_id)}")
+            else:
+                word_ids.append(str(m.word_id()))
 
         if len(oov) > 0:
             raise OOVError(f"split word has out of vocab: {oov} in {normalized}")
 
         return "/".join(word_ids)
 
     def split(self, normalized: str, udm: list[str]) -> str:
@@ -189,29 +203,33 @@
     args = parser.parse_args()
     out = open(args.out, "wt")
     rewrite = args.rewrite_def
     rm = args.rm_already_exist
     config = args.config
     sudachi_setting = args.sudachi_setting
     sudachi_dict_type = args.sudachi_dict_type
-    merge_dict = args.merge_dict
+    unit_word_dict = args.unit_word_dict
+
+    unit_words_dict: dict[str, UnitWord] = {}
+    if not unit_word_dict == "":
+        with fileinput.input(files=unit_word_dict) as merge_dict:
+            for i, line in enumerate(merge_dict):
+                line = line.replace("\n", "")
+                unit_words_dict[line.split(",")[0]] = UnitWord(word_id=i, line=line)
+                out.write(f"{line}\n")
 
     c = Converter(
         rewrite,
         config,
         sudachi_setting=sudachi_setting,
         dict_type=sudachi_dict_type,
         rm=rm,
+        unit_words_dict=unit_words_dict,
     )
 
-    with fileinput.input(files=merge_dict) as merged:
-        for line in merged:
-            line = line.replace("\n", "")
-            out.write(f"{line}\n")
-
     with fileinput.input(files=args.file) as input:
         for line in input:
             line = line.strip()
             if line == "":
                 continue
             if line[0] == "#":
                 continue
```

### Comparing `kuro2sudachi-0.3.9/src/kuro2sudachi/normalizer.py` & `kuro2sudachi-0.4.0/src/kuro2sudachi/normalizer.py`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.3.9/src/kuro2sudachi/rewrite.def` & `kuro2sudachi-0.4.0/src/kuro2sudachi/rewrite.def`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.3.9/PKG-INFO` & `kuro2sudachi-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuro2sudachi
-Version: 0.3.9
+Version: 0.4.0
 Summary: 
 Home-page: http://github.com/po3rin/kuro2sudachi
 License: Apache-2.0
 Author: po3rin
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -51,15 +51,15 @@
         "cost": 5000
     }
 }
 
 ```
 
 ```$
-$ kuro2sudachi kuromoji_dict.txt -o sudachi_user_dict.txt -c convert_config.json
+$ kuro2sudachi kuromoji_dict.txt -o sudachi_user_dict.txt -c kuro2sudachi.json
 ```
 
 if you want to ignore unsupported pos error & invalid format, use `--ignore` flag.
 
 ## Dictionary type
 
 You can specify the dictionary with the tokenize option -s (default: core).
@@ -91,15 +91,15 @@
 output includes unit devision info.
 
 ```sh
 $ cat kuromoji_dict.txt
 融合たんぱく質,融合たんぱく質,融合たんぱく質,名詞
 発作性心房細動,発作性心房細動,発作性心房細動,名詞
 
-$ kuro2sudachi kuromoji_dict.txt -o sudachi_user_dict.txt -c convert_config.json --ignore
+$ kuro2sudachi kuromoji_dict.txt -o sudachi_user_dict.txt -c kuro2sudachi.json --ignore
 
 $ cat sudachi_user_dict.txt
 融合たんぱく質,4786,4786,5000,融合たんぱく質,名詞,普通名詞,一般,*,*,*,,融合たんぱく質,*,C,*,660881/810248,*
 発作性心房細動,4786,4786,5000,発作性心房細動,名詞,普通名詞,一般,*,*,*,,発作性心房細動,*,C,584006/434835/428494/619020,2756385/428494/619020,*
 ```
 
 ## Splitting Words defined by kuromoji
@@ -123,12 +123,7 @@
 
 exec kuro2sudachi command
 
 ```sh
 $ poetry run kuro2sudachi tests/kuromoji_dict_test.txt -o sudachi_user_dict.txt
 ```
 
-## TODO
-
-- [ ] split mode
-- [ ] default rewrite
-
```

