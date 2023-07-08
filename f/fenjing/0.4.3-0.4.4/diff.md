# Comparing `tmp/fenjing-0.4.3.tar.gz` & `tmp/fenjing-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.3.tar", last modified: Sat Jul  8 11:58:23 2023, max compression
+gzip compressed data, was "fenjing-0.4.4.tar", last modified: Sat Jul  8 13:38:09 2023, max compression
```

## Comparing `fenjing-0.4.3.tar` & `fenjing-0.4.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:58:23.172106 fenjing-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-08 11:58:13.000000 fenjing-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 11:58:13.000000 fenjing-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-08 11:58:23.172106 fenjing-0.4.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6120 2023-07-08 11:58:13.000000 fenjing-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 11:58:13.000000 fenjing-0.4.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:58:23.168106 fenjing-0.4.3/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7292 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    31678 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:58:23.172106 fenjing-0.4.3/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:58:23.168106 fenjing-0.4.3/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-08 11:58:23.000000 fenjing-0.4.3/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-08 11:58:23.000000 fenjing-0.4.3/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:58:23.000000 fenjing-0.4.3/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 11:58:23.000000 fenjing-0.4.3/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 11:58:23.000000 fenjing-0.4.3/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 11:58:13.000000 fenjing-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 11:58:23.172106 fenjing-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-08 11:58:13.000000 fenjing-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:58:23.172106 fenjing-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-08 11:58:13.000000 fenjing-0.4.3/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-08 11:58:13.000000 fenjing-0.4.3/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:38:09.305641 fenjing-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-08 13:37:59.000000 fenjing-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 13:37:59.000000 fenjing-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-08 13:38:09.301641 fenjing-0.4.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6120 2023-07-08 13:37:59.000000 fenjing-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 13:37:59.000000 fenjing-0.4.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:38:09.301641 fenjing-0.4.4/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7292 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31678 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:38:09.301641 fenjing-0.4.4/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:38:09.301641 fenjing-0.4.4/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-08 13:38:09.000000 fenjing-0.4.4/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-08 13:38:09.000000 fenjing-0.4.4/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 13:38:09.000000 fenjing-0.4.4/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 13:38:09.000000 fenjing-0.4.4/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 13:38:09.000000 fenjing-0.4.4/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 13:37:59.000000 fenjing-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 13:38:09.305641 fenjing-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-08 13:37:59.000000 fenjing-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:38:09.301641 fenjing-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-08 13:37:59.000000 fenjing-0.4.4/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-08 13:37:59.000000 fenjing-0.4.4/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.3/LICENSE` & `fenjing-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/PKG-INFO` & `fenjing-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.3/README.md` & `fenjing-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/cli.py` & `fenjing-0.4.4/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/colorize.py` & `fenjing-0.4.4/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/config_payload.py` & `fenjing-0.4.4/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/const.py` & `fenjing-0.4.4/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/context_vars.py` & `fenjing-0.4.4/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/form.py` & `fenjing-0.4.4/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/form_cracker.py` & `fenjing-0.4.4/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/full_payload_gen.py` & `fenjing-0.4.4/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/payload_gen.py` & `fenjing-0.4.4/fenjing/payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/requester.py` & `fenjing-0.4.4/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/scan_url.py` & `fenjing-0.4.4/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/shell_payload.py` & `fenjing-0.4.4/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/templates/index.html` & `fenjing-0.4.4/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/waf_func_gen.py` & `fenjing-0.4.4/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing/webui.py` & `fenjing-0.4.4/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.4/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.3/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.4/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/setup.py` & `fenjing-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/tests/test_full_payload_gen.py` & `fenjing-0.4.4/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.3/tests/test_payload_gen.py` & `fenjing-0.4.4/tests/test_payload_gen.py`

 * *Files identical despite different names*

