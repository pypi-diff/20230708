# Comparing `tmp/pyhackrf2-1.0.2.tar.gz` & `tmp/pyhackrf2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhackrf2-1.0.2.tar", last modified: Sat Jul  8 19:43:31 2023, max compression
+gzip compressed data, was "pyhackrf2-1.0.3.tar", last modified: Sat Jul  8 19:55:26 2023, max compression
```

## Comparing `pyhackrf2-1.0.2.tar` & `pyhackrf2-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:43:31.130037 pyhackrf2-1.0.2/
--rw-r--r--   0 alex       (501) staff       (20)     4627 2023-07-08 19:43:31.129677 pyhackrf2-1.0.2/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     4316 2023-07-08 19:27:39.000000 pyhackrf2-1.0.2/README.md
--rw-r--r--   0 alex       (501) staff       (20)      434 2023-07-08 19:28:42.000000 pyhackrf2-1.0.2/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-07-08 19:43:31.130101 pyhackrf2-1.0.2/setup.cfg
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:43:31.126776 pyhackrf2-1.0.2/src/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:43:31.127605 pyhackrf2-1.0.2/src/pyhackrf2/
--rw-r--r--   0 alex       (501) staff       (20)    18072 2023-07-08 19:05:33.000000 pyhackrf2-1.0.2/src/pyhackrf2/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     5017 2023-05-29 21:31:56.000000 pyhackrf2-1.0.2/src/pyhackrf2/cinterface.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:43:31.128973 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     4627 2023-07-08 19:43:31.000000 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      262 2023-07-08 19:43:31.000000 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-08 19:43:31.000000 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       12 2023-07-08 19:43:31.000000 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       10 2023-07-08 19:43:31.000000 pyhackrf2-1.0.2/src/pyhackrf2.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:55:26.202399 pyhackrf2-1.0.3/
+-rw-r--r--   0 alex       (501) staff       (20)     4627 2023-07-08 19:55:26.202214 pyhackrf2-1.0.3/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     4316 2023-07-08 19:46:57.000000 pyhackrf2-1.0.3/README.md
+-rw-r--r--   0 alex       (501) staff       (20)      434 2023-07-08 19:54:53.000000 pyhackrf2-1.0.3/pyproject.toml
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-07-08 19:55:26.202447 pyhackrf2-1.0.3/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:55:26.199586 pyhackrf2-1.0.3/src/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:55:26.200784 pyhackrf2-1.0.3/src/pyhackrf2/
+-rw-r--r--   0 alex       (501) staff       (20)    18095 2023-07-08 19:54:39.000000 pyhackrf2-1.0.3/src/pyhackrf2/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     5017 2023-05-29 21:31:56.000000 pyhackrf2-1.0.3/src/pyhackrf2/cinterface.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-08 19:55:26.201992 pyhackrf2-1.0.3/src/pyhackrf2.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     4627 2023-07-08 19:55:26.000000 pyhackrf2-1.0.3/src/pyhackrf2.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      262 2023-07-08 19:55:26.000000 pyhackrf2-1.0.3/src/pyhackrf2.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-08 19:55:26.000000 pyhackrf2-1.0.3/src/pyhackrf2.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       12 2023-07-08 19:55:26.000000 pyhackrf2-1.0.3/src/pyhackrf2.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       10 2023-07-08 19:55:26.000000 pyhackrf2-1.0.3/src/pyhackrf2.egg-info/top_level.txt
```

### Comparing `pyhackrf2-1.0.2/PKG-INFO` & `pyhackrf2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhackrf2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python bindings for libhackrf rewritten
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `pyhackrf2-1.0.2/README.md` & `pyhackrf2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhackrf2-1.0.2/src/pyhackrf2/__init__.py` & `pyhackrf2-1.0.3/src/pyhackrf2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
             return np.array([])
 
         self._sample_count_limit = int(2 * num_samples)
         self.start_rx()
 
         while self._transceiver_mode != TransceiverMode.HACKRF_TRANSCEIVER_MODE_OFF:
             pass
+        self.stop_rx()
         # convert samples to iq
         values = np.array(self.buffer).astype(np.int8)
         iq = values.astype(np.float64).view(np.complex128)
         iq /= 127.5
         iq -= 1 + 1j
         return iq
```

### Comparing `pyhackrf2-1.0.2/src/pyhackrf2/cinterface.py` & `pyhackrf2-1.0.3/src/pyhackrf2/cinterface.py`

 * *Files identical despite different names*

### Comparing `pyhackrf2-1.0.2/src/pyhackrf2.egg-info/PKG-INFO` & `pyhackrf2-1.0.3/src/pyhackrf2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhackrf2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python bindings for libhackrf rewritten
 Classifier: Topic :: Communications :: Ham Radio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

