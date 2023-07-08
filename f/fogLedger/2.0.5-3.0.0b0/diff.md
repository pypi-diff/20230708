# Comparing `tmp/fogLedger-2.0.5.tar.gz` & `tmp/fogLedger-3.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fogLedger-2.0.5.tar", last modified: Wed Jul  5 00:35:35 2023, max compression
+gzip compressed data, was "fogLedger-3.0.0b0.tar", last modified: Sat Jul  8 02:07:38 2023, max compression
```

## Comparing `fogLedger-2.0.5.tar` & `fogLedger-3.0.0b0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:35:35.295874 fogLedger-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-05 00:35:25.000000 fogLedger-2.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-05 00:35:35.295874 fogLedger-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-05 00:35:25.000000 fogLedger-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:35:35.295874 fogLedger-2.0.5/fogLedger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-05 00:35:35.000000 fogLedger-2.0.5/fogLedger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-05 00:35:35.000000 fogLedger-2.0.5/fogLedger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:35:35.000000 fogLedger-2.0.5/fogLedger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:35:35.000000 fogLedger-2.0.5/fogLedger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 00:35:35.000000 fogLedger-2.0.5/fogLedger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 00:35:35.000000 fogLedger-2.0.5/fogLedger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:35:35.295874 fogLedger-2.0.5/fogledger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:35:25.000000 fogLedger-2.0.5/fogledger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:35:35.295874 fogLedger-2.0.5/fogledger/indy/
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-05 00:35:25.000000 fogLedger-2.0.5/fogledger/indy/IndyBasic.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 00:35:25.000000 fogLedger-2.0.5/fogledger/indy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 00:35:25.000000 fogLedger-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:35:35.295874 fogLedger-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-05 00:35:25.000000 fogLedger-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/fogLedger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 02:07:38.000000 fogLedger-3.0.0b0/fogLedger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/fogledger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/fogledger/indy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/indy/IndyBasic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/indy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/fogledger/iota/
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/iota/IotaBasic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/iota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/test-iota-distributed-network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/fogledger/test-iota-local-network.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 02:07:38.588073 fogLedger-3.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-08 02:07:27.000000 fogLedger-3.0.0b0/setup.py
```

### Comparing `fogLedger-2.0.5/LICENSE.txt` & `fogLedger-3.0.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fogLedger-2.0.5/PKG-INFO` & `fogLedger-3.0.0b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fogLedger
-Version: 2.0.5
+Version: 3.0.0b0
 Summary: Plugin to build DLTs in Fogbed.
 Home-page: https://github.com/larsid/FogLedger/tree/v2.0.0
 Author: Matheus Nascimento
 Author-email: matheusnascimentoti99@gmail.com
 Keywords: networking,emulator,protocol,Internet,dlt,indy,fog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fogLedger-2.0.5/README.md` & `fogLedger-3.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `fogLedger-2.0.5/fogLedger.egg-info/PKG-INFO` & `fogLedger-3.0.0b0/fogLedger.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fogLedger
-Version: 2.0.5
+Version: 3.0.0b0
 Summary: Plugin to build DLTs in Fogbed.
 Home-page: https://github.com/larsid/FogLedger/tree/v2.0.0
 Author: Matheus Nascimento
 Author-email: matheusnascimentoti99@gmail.com
 Keywords: networking,emulator,protocol,Internet,dlt,indy,fog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fogLedger-2.0.5/fogledger/indy/IndyBasic.py` & `fogLedger-3.0.0b0/fogledger/indy/IndyBasic.py`

 * *Files identical despite different names*

### Comparing `fogLedger-2.0.5/setup.py` & `fogLedger-3.0.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="fogLedger",
-    version="2.0.5",
+    version="3.0.0-beta",
     description='Plugin to build DLTs in Fogbed.',
     long_description='Plugin to build DLT in Fogbed. Suport Hyperledger Indy. \
         The FogLedger is a plugin for [Fogbed](https://github.com/larsid/fogbed). It allows you to emulate a fog network with distributed ledgers. \
         Currently, FogLedger has suport for Hyperledger Indy. It is a distributed ledger, purpose-built for decentralized identity. \
         It provides tools, libraries, and reusable components for creating and using independent digital identities rooted on blockchains or other distributed ledgers so that they are interoperable across administrative domains, applications, and any other silo. \
         Indy is interoperable with other blockchains or can be used standalone powering the decentralization of identity. \
         With FogLedger you can create a network of nodes running Hyperledger Indy. A emulation can have multiple networks of nodes running different distributed ledgers. \
```

