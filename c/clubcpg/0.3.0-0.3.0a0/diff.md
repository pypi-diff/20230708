# Comparing `tmp/clubcpg-0.3.0.tar.gz` & `tmp/clubcpg-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clubcpg-0.3.0.tar", max compression
+gzip compressed data, was "clubcpg-0.3.0a0.tar", max compression
```

## Comparing `clubcpg-0.3.0.tar` & `clubcpg-0.3.0a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-07-08 18:13:21.340372 clubcpg-0.3.0/LICENSE
--rw-r--r--   0        0        0     2402 2023-07-08 18:13:21.340372 clubcpg-0.3.0/README.md
--rw-r--r--   0        0        0     7320 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg/CalculateBinCoverage.py
--rw-r--r--   0        0        0    24592 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg/ClusterReads.py
--rw-r--r--   0        0        0     1888 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg/ConnectToCpGNet.py
--rw-r--r--   0        0        0     7816 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg/Imputation.py
--rw-r--r--   0        0        0     1114 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg/OutputComparisonResults.py
--rw-r--r--   0        0        0    13004 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg/ParseBam.py
--rw-r--r--   0        0        0      117 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg/tests/__init__.py
--rw-r--r--   0        0        0     7045 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg/tests/test_Module.py
--rw-r--r--   0        0        0        0 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg_bin/__init__.py
--rwxr-xr-x   0        0        0     6095 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg_bin/clubcpg_cluster.py
--rwxr-xr-x   0        0        0     3963 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg_bin/clubcpg_coverage.py
--rwxr-xr-x   0        0        0     6476 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg_bin/clubcpg_impute_cluster.py
--rwxr-xr-x   0        0        0     5111 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg_bin/clubcpg_impute_coverage.py
--rwxr-xr-x   0        0        0     2614 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg_bin/clubcpg_impute_train.py
--rw-r--r--   0        0        0    13821 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg_prelim/PReLIM.py
--rw-r--r--   0        0        0       78 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg_prelim/__init__.py
--rw-r--r--   0        0        0     2303 2023-07-08 18:13:21.348372 clubcpg-0.3.0/clubcpg_prelim/util/CpG_Bin.py
--rw-r--r--   0        0        0     1516 2023-07-08 18:13:21.408372 clubcpg-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3507 1970-01-01 00:00:00.000000 clubcpg-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-07 22:26:42.543324 clubcpg-0.3.0a0/LICENSE
+-rw-r--r--   0        0        0     2402 2023-07-07 22:26:42.543324 clubcpg-0.3.0a0/README.md
+-rw-r--r--   0        0        0     7320 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/CalculateBinCoverage.py
+-rw-r--r--   0        0        0    24592 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/ClusterReads.py
+-rw-r--r--   0        0        0     1888 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/ConnectToCpGNet.py
+-rw-r--r--   0        0        0     7816 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/Imputation.py
+-rw-r--r--   0        0        0     1114 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/OutputComparisonResults.py
+-rw-r--r--   0        0        0    13004 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/ParseBam.py
+-rw-r--r--   0        0        0      117 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/tests/__init__.py
+-rw-r--r--   0        0        0     7045 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/tests/test_Module.py
+-rw-r--r--   0        0        0        0 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/__init__.py
+-rwxr-xr-x   0        0        0     6095 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/clubcpg_cluster.py
+-rwxr-xr-x   0        0        0     3963 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/clubcpg_coverage.py
+-rwxr-xr-x   0        0        0     6476 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_cluster.py
+-rwxr-xr-x   0        0        0     5111 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_coverage.py
+-rwxr-xr-x   0        0        0     2614 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_train.py
+-rw-r--r--   0        0        0    13821 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_prelim/PReLIM.py
+-rw-r--r--   0        0        0       78 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_prelim/__init__.py
+-rw-r--r--   0        0        0     2303 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_prelim/util/CpG_Bin.py
+-rw-r--r--   0        0        0     1518 2023-07-07 22:26:42.619326 clubcpg-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 clubcpg-0.3.0a0/PKG-INFO
```

### Comparing `clubcpg-0.3.0/LICENSE` & `clubcpg-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/README.md` & `clubcpg-0.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg/CalculateBinCoverage.py` & `clubcpg-0.3.0a0/clubcpg/CalculateBinCoverage.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg/ClusterReads.py` & `clubcpg-0.3.0a0/clubcpg/ClusterReads.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg/ConnectToCpGNet.py` & `clubcpg-0.3.0a0/clubcpg/ConnectToCpGNet.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg/Imputation.py` & `clubcpg-0.3.0a0/clubcpg/Imputation.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg/OutputComparisonResults.py` & `clubcpg-0.3.0a0/clubcpg/OutputComparisonResults.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg/ParseBam.py` & `clubcpg-0.3.0a0/clubcpg/ParseBam.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg/tests/test_Module.py` & `clubcpg-0.3.0a0/clubcpg/tests/test_Module.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg_bin/clubcpg_cluster.py` & `clubcpg-0.3.0a0/clubcpg_bin/clubcpg_cluster.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg_bin/clubcpg_coverage.py` & `clubcpg-0.3.0a0/clubcpg_bin/clubcpg_coverage.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg_bin/clubcpg_impute_cluster.py` & `clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_cluster.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg_bin/clubcpg_impute_coverage.py` & `clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_coverage.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg_bin/clubcpg_impute_train.py` & `clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_train.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg_prelim/PReLIM.py` & `clubcpg-0.3.0a0/clubcpg_prelim/PReLIM.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/clubcpg_prelim/util/CpG_Bin.py` & `clubcpg-0.3.0a0/clubcpg_prelim/util/CpG_Bin.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.3.0/pyproject.toml` & `clubcpg-0.3.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clubcpg"
-version = "0.3.0"
+version = "0.3.0a0"
 description = "CluBCpG is a software package built to analyze whole genome bisulfite sequencing (WGBS) data."
 authors = ["Anthony Scott, PhD <anthony@canthonyscott.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "clubcpg" },
     { include = "clubcpg_prelim" },
```

### Comparing `clubcpg-0.3.0/PKG-INFO` & `clubcpg-0.3.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubcpg
-Version: 0.3.0
+Version: 0.3.0a0
 Summary: CluBCpG is a software package built to analyze whole genome bisulfite sequencing (WGBS) data.
 License: MIT
 Author: Anthony Scott, PhD
 Author-email: anthony@canthonyscott.com
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

