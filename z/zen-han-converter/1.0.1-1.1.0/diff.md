# Comparing `tmp/zen_han_converter-1.0.1.tar.gz` & `tmp/zen_han_converter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen_han_converter-1.0.1.tar", last modified: Fri Jul  7 15:50:52 2023, max compression
+gzip compressed data, was "zen_han_converter-1.1.0.tar", last modified: Sat Jul  8 13:57:24 2023, max compression
```

## Comparing `zen_han_converter-1.0.1.tar` & `zen_han_converter-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/tests/test_zen_han_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/zen_han_converter/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/zen_han_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/zen_han_converter/han_to_zen_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/zen_han_converter/zen_han_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/zen_han_converter/zen_to_han_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/zen_han_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-07 15:50:52.000000 zen_han_converter-1.0.1/zen_han_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-07 15:50:52.000000 zen_han_converter-1.0.1/zen_han_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:50:52.000000 zen_han_converter-1.0.1/zen_han_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 15:50:52.000000 zen_han_converter-1.0.1/zen_han_converter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:57:24.711431 zen_han_converter-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-08 13:57:24.711431 zen_han_converter-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-08 13:57:15.000000 zen_han_converter-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 13:57:24.711431 zen_han_converter-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 13:57:15.000000 zen_han_converter-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:57:24.707431 zen_han_converter-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 13:57:15.000000 zen_han_converter-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-08 13:57:15.000000 zen_han_converter-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-08 13:57:15.000000 zen_han_converter-1.1.0/tests/test_zen_han_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:57:24.711431 zen_han_converter-1.1.0/zen_han_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 13:57:15.000000 zen_han_converter-1.1.0/zen_han_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-08 13:57:15.000000 zen_han_converter-1.1.0/zen_han_converter/han_to_zen_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-08 13:57:15.000000 zen_han_converter-1.1.0/zen_han_converter/zen_han_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-08 13:57:15.000000 zen_han_converter-1.1.0/zen_han_converter/zen_to_han_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:57:24.711431 zen_han_converter-1.1.0/zen_han_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-08 13:57:24.000000 zen_han_converter-1.1.0/zen_han_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-08 13:57:24.000000 zen_han_converter-1.1.0/zen_han_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 13:57:24.000000 zen_han_converter-1.1.0/zen_han_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 13:57:24.000000 zen_han_converter-1.1.0/zen_han_converter.egg-info/top_level.txt
```

### Comparing `zen_han_converter-1.0.1/PKG-INFO` & `zen_han_converter-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen_han_converter
-Version: 1.0.1
+Version: 1.1.0
 Summary: Converts full-width and half-width characters.
 Home-page: https://github.com/n4cl/zen_han_converter.git
 Author: n4cl
 Author-email: devn4cl@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,21 +15,28 @@
 zen_han_converter
 ===
 
 # Description
 
 This is a tool for converting full-width and half-width characters to each other, implemented only with Python's standard modules.
 
+# Target characters
+
+- Latin alphabet
+- Arabic numerals
+- ASCII symbols
+- Space
+
 # Installaction
 
 ```
 pip install zen_han_converter
 ```
 
 # Usage
 
 ```
->>> from zen_han_convter import ZenToHan
+>>> from zen_han_converter import ZenToHan
 >>> zen_to_han = ZenToHan()
 >>> zen_to_han.convert('ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ')
 'abcdefghijklmnopqrstuvwxyz'
 ```
```

### Comparing `zen_han_converter-1.0.1/setup.py` & `zen_han_converter-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="zen_han_converter",
-    version="1.0.1",
+    version="1.1.0",
     author="n4cl",
     author_email="devn4cl@gmail.com",
     description="Converts full-width and half-width characters.",
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/n4cl/zen_han_converter.git",
     license='MIT',
```

### Comparing `zen_han_converter-1.0.1/tests/test_zen_han_converter.py` & `zen_han_converter-1.1.0/tests/test_zen_han_converter.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,21 @@
     zen_to_han = ZenToHan(alphabet_table=True, number_table=True, ascii_symbol_table=True)
     assert zen_to_han.convert('ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ') == 'abcdefghijklmnopqrstuvwxyz'
     assert zen_to_han.convert('abcdefghijklmnopqrstuvwxyz') == 'abcdefghijklmnopqrstuvwxyz'
     assert zen_to_han.convert('０１２３４５６７８９') == '0123456789'
     assert zen_to_han.convert('0123456789') == '0123456789'
     assert zen_to_han.convert("！＂＃＄％＆＇（）＊＋，－．／：；＜＝＞？＠［＼］＾＿｀｛｜｝～") == "!\"#$%&'()*+,-./:;<=>?@[\\]^_`{|}~"
     assert zen_to_han.convert("!\"#$%&'()*+,-./:;<=>?@[\\]^_`{|}~") == "!\"#$%&'()*+,-./:;<=>?@[\\]^_`{|}~"
+    assert zen_to_han.convert("　") == " "
+    assert zen_to_han.convert(" ") == " "
 
 
 def test_HanToZen():
     han_to_zen = HanToZen(alphabet_table=True, number_table=True, ascii_symbol_table=True)
     assert han_to_zen.convert("abcdefghijklmnopqrstuvwxyz") == "ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ"
     assert han_to_zen.convert("ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ") == "ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ"
     assert han_to_zen.convert("0123456789") == "０１２３４５６７８９"
     assert han_to_zen.convert("０１２３４５６７８９") == "０１２３４５６７８９"
     assert han_to_zen.convert("!\"#$%&'()*+,-./:;<=>?@[\\]^_`{|}~") == "！＂＃＄％＆＇（）＊＋，－．／：；＜＝＞？＠［＼］＾＿｀｛｜｝～"
     assert han_to_zen.convert("！＂＃＄％＆＇（）＊＋，－．／：；＜＝＞？＠［＼］＾＿｀｛｜｝～") == "！＂＃＄％＆＇（）＊＋，－．／：；＜＝＞？＠［＼］＾＿｀｛｜｝～"
+    assert han_to_zen.convert(" ") == "　"
+    assert han_to_zen.convert("　") == "　"
```

### Comparing `zen_han_converter-1.0.1/zen_han_converter/han_to_zen_table.py` & `zen_han_converter-1.1.0/zen_han_converter/han_to_zen_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,7 +96,11 @@
 "_": "＿",
 "`": "｀",
 "{": "｛",
 "|": "｜",
 "}": "｝",
 "~": "～",
 }
+
+SPACE = {
+" ": "　",
+}
```

### Comparing `zen_han_converter-1.0.1/zen_han_converter/zen_han_converter.py` & `zen_han_converter-1.1.0/zen_han_converter/zen_han_converter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from .han_to_zen_table import LATIN_ALPHABET as HAN2ZEN_LATIN_ALPHABET, \
                              ARABIC_NUMERALS as HAN2ZEN_ARABIC_NUMERALS, \
-                             ASCII_SYMBOL as HAN2ZEN_ASCII_SYMBOL
+                             ASCII_SYMBOL as HAN2ZEN_ASCII_SYMBOL, \
+                             SPACE as HAN2ZEN_SPACE
 from .zen_to_han_table import LATIN_ALPHABET as ZEN2HAN_LATIN_ALPHABET, \
                              ARABIC_NUMERALS as ZEN2HAN_ARABIC_NUMERALS, \
-                             ASCII_SYMBOL as ZEN2HAN_ASCII_SYMBOL
+                             ASCII_SYMBOL as ZEN2HAN_ASCII_SYMBOL, \
+                             SPACE as ZEN2HAN_SPACE
 
 
 class BaseConverter:
     """
     コンバーターの基底クラス
     """
     def __init__(self, table):
@@ -20,31 +22,43 @@
         return text.translate(self.table)
 
 
 class ZenToHan(BaseConverter):
     """
     全角を半角に変換するクラス
     """
-    def __init__(self, alphabet_table=True, number_table=True, ascii_symbol_table=True):
+    def __init__(self,
+                 alphabet_table=True,
+                 number_table=True,
+                 ascii_symbol_table=True,
+                 space_table=True):
         _table = {}
         if alphabet_table:
             _table.update(ZEN2HAN_LATIN_ALPHABET)
         if number_table:
             _table.update(ZEN2HAN_ARABIC_NUMERALS)
         if ascii_symbol_table:
             _table.update(ZEN2HAN_ASCII_SYMBOL)
+        if space_table:
+            _table.update(ZEN2HAN_SPACE)
         super().__init__(_table)
 
 
 class HanToZen(BaseConverter):
     """
     半角を全角に変換するクラス
     """
-    def __init__(self, alphabet_table=True, number_table=True, ascii_symbol_table=True):
+    def __init__(self,
+                 alphabet_table=True,
+                 number_table=True,
+                 ascii_symbol_table=True,
+                 space_table=True):
         _table = {}
         if alphabet_table:
             _table.update(HAN2ZEN_LATIN_ALPHABET)
         if number_table:
             _table.update(HAN2ZEN_ARABIC_NUMERALS)
         if ascii_symbol_table:
             _table.update(HAN2ZEN_ASCII_SYMBOL)
+        if space_table:
+            _table.update(HAN2ZEN_SPACE)
         super().__init__(_table)
```

### Comparing `zen_han_converter-1.0.1/zen_han_converter/zen_to_han_table.py` & `zen_han_converter-1.1.0/zen_han_converter/zen_to_han_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,7 +96,11 @@
 "＿": "_",
 "｀": "`",
 "｛": "{",
 "｜": "|",
 "｝": "}",
 "～": "~",
 }
+
+SPACE = {
+"　": " ",
+}
```

### Comparing `zen_han_converter-1.0.1/zen_han_converter.egg-info/PKG-INFO` & `zen_han_converter-1.1.0/zen_han_converter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-han-converter
-Version: 1.0.1
+Version: 1.1.0
 Summary: Converts full-width and half-width characters.
 Home-page: https://github.com/n4cl/zen_han_converter.git
 Author: n4cl
 Author-email: devn4cl@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,21 +15,28 @@
 zen_han_converter
 ===
 
 # Description
 
 This is a tool for converting full-width and half-width characters to each other, implemented only with Python's standard modules.
 
+# Target characters
+
+- Latin alphabet
+- Arabic numerals
+- ASCII symbols
+- Space
+
 # Installaction
 
 ```
 pip install zen_han_converter
 ```
 
 # Usage
 
 ```
->>> from zen_han_convter import ZenToHan
+>>> from zen_han_converter import ZenToHan
 >>> zen_to_han = ZenToHan()
 >>> zen_to_han.convert('ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ')
 'abcdefghijklmnopqrstuvwxyz'
 ```
```

