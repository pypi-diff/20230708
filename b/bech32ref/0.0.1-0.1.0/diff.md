# Comparing `tmp/bech32ref-0.0.1.tar.gz` & `tmp/bech32ref-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bech32ref-0.0.1.tar", last modified: Mon Jan 17 22:43:12 2022, max compression
+gzip compressed data, was "bech32ref-0.1.0.tar", max compression
```

## Comparing `bech32ref-0.0.1.tar` & `bech32ref-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,6 @@
-drwxrwxr-x   0 niftynei  (1000) niftynei  (1000)        0 2022-01-17 22:43:12.190686 bech32ref-0.0.1/
--rw-rw-r--   0 niftynei  (1000) niftynei  (1000)      758 2022-01-17 22:43:12.190686 bech32ref-0.0.1/PKG-INFO
--rw-rw-r--   0 niftynei  (1000) niftynei  (1000)      253 2022-01-17 21:38:24.000000 bech32ref-0.0.1/README.md
-drwxrwxr-x   0 niftynei  (1000) niftynei  (1000)        0 2022-01-17 22:43:12.190686 bech32ref-0.0.1/bech32ref/
--rw-rw-r--   0 niftynei  (1000) niftynei  (1000)      187 2022-01-17 22:25:36.000000 bech32ref-0.0.1/bech32ref/__init__.py
--rw-rw-r--   0 niftynei  (1000) niftynei  (1000)     5022 2022-01-17 21:33:21.000000 bech32ref-0.0.1/bech32ref/segwit_addr.py
--rwxrwxr-x   0 niftynei  (1000) niftynei  (1000)     8804 2022-01-17 22:25:23.000000 bech32ref-0.0.1/bech32ref/tests.py
-drwxrwxr-x   0 niftynei  (1000) niftynei  (1000)        0 2022-01-17 22:43:12.190686 bech32ref-0.0.1/bech32ref.egg-info/
--rw-rw-r--   0 niftynei  (1000) niftynei  (1000)      758 2022-01-17 22:43:12.000000 bech32ref-0.0.1/bech32ref.egg-info/PKG-INFO
--rw-rw-r--   0 niftynei  (1000) niftynei  (1000)      216 2022-01-17 22:43:12.000000 bech32ref-0.0.1/bech32ref.egg-info/SOURCES.txt
--rw-rw-r--   0 niftynei  (1000) niftynei  (1000)        1 2022-01-17 22:43:12.000000 bech32ref-0.0.1/bech32ref.egg-info/dependency_links.txt
--rw-rw-r--   0 niftynei  (1000) niftynei  (1000)       10 2022-01-17 22:43:12.000000 bech32ref-0.0.1/bech32ref.egg-info/top_level.txt
--rw-rw-r--   0 niftynei  (1000) niftynei  (1000)       38 2022-01-17 22:43:12.190686 bech32ref-0.0.1/setup.cfg
--rw-rw-r--   0 niftynei  (1000) niftynei  (1000)      815 2022-01-17 22:42:55.000000 bech32ref-0.0.1/setup.py
+-rw-r--r--   0        0        0      253 2023-07-08 03:58:34.996704 bech32ref-0.1.0/README.md
+-rw-r--r--   0        0        0      187 2023-07-08 03:58:34.996704 bech32ref-0.1.0/bech32ref/__init__.py
+-rw-r--r--   0        0        0     5004 2023-07-08 03:58:56.045371 bech32ref-0.1.0/bech32ref/segwit_addr.py
+-rwxr-xr-x   0        0        0     8804 2023-07-08 03:58:34.996704 bech32ref-0.1.0/bech32ref/tests.py
+-rw-r--r--   0        0        0      350 2023-07-08 04:01:46.678776 bech32ref-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 bech32ref-0.1.0/PKG-INFO
```

### Comparing `bech32ref-0.0.1/PKG-INFO` & `bech32ref-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: bech32ref
-Version: 0.0.1
-Summary: Port of @sipa's bech32 reference implementation. Includes bech32m
-Home-page: https://github.com/niftynei/bech32ref
-Author: Pieter Wiulle
-Author-email: pieter@wuille.net
+Version: 0.1.0
+Summary: A bech32 implemenation, slightly modified to allow for >90char strings
 License: MIT
-Description: # bech32m for Python
-        
-        This is a straight port of @sipa's Python reference implementation of bech32 and bech32m.
-        
-        Original can be found here: [https://github.com/sipa/bech32/tree/master/ref/python](https://github.com/sipa/bech32/tree/master/ref/python).
-        
-Platform: UNKNOWN
+Author: niftynei
+Author-email: niftynei@gmail.com
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+
+# bech32m for Python
+
+This is a straight port of @sipa's Python reference implementation of bech32 and bech32m.
+
+Original can be found here: [https://github.com/sipa/bech32/tree/master/ref/python](https://github.com/sipa/bech32/tree/master/ref/python).
+
```

### Comparing `bech32ref-0.0.1/bech32ref/segwit_addr.py` & `bech32ref-0.1.0/bech32ref/segwit_addr.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 def bech32_decode(bech):
     """Validate a Bech32/Bech32m string, and determine HRP and data."""
     if ((any(ord(x) < 33 or ord(x) > 126 for x in bech)) or
             (bech.lower() != bech and bech.upper() != bech)):
         return (None, None, None)
     bech = bech.lower()
     pos = bech.rfind('1')
-    if pos < 1 or pos + 7 > len(bech) or len(bech) > 90:
+    if pos < 1 or pos + 7 > len(bech):
         return (None, None, None)
     if not all(x in CHARSET for x in bech[pos+1:]):
         return (None, None, None)
     hrp = bech[:pos]
     data = [CHARSET.find(x) for x in bech[pos+1:]]
     spec = bech32_verify_checksum(hrp, data)
     if spec is None:
```

### Comparing `bech32ref-0.0.1/bech32ref/tests.py` & `bech32ref-0.1.0/bech32ref/tests.py`

 * *Files identical despite different names*

