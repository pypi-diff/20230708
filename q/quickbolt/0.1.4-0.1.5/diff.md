# Comparing `tmp/quickbolt-0.1.4.tar.gz` & `tmp/quickbolt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbolt-0.1.4.tar", max compression
+gzip compressed data, was "quickbolt-0.1.5.tar", max compression
```

## Comparing `quickbolt-0.1.4.tar` & `quickbolt-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.1.4/LICENSE
--rw-r--r--   0        0        0     3964 2023-07-03 21:01:01.355674 quickbolt-0.1.4/README.md
--rw-r--r--   0        0        0     1238 2023-07-05 05:53:30.375693 quickbolt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.1.4/quickbolt/__init__.py
--rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.1.4/quickbolt/batch_generation/__init__.py
--rw-r--r--   0        0        0    11311 2023-07-05 02:39:06.705757 quickbolt-0.1.4/quickbolt/batch_generation/batch_generation.py
--rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.1.4/quickbolt/clients/__init__.py
--rw-r--r--   0        0        0     9806 2023-06-29 16:19:54.925810 quickbolt-0.1.4/quickbolt/clients/aio_requests.py
--rw-r--r--   0        0        0    10021 2023-06-29 16:19:54.926154 quickbolt-0.1.4/quickbolt/clients/httpx_requests.py
--rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.1.4/quickbolt/logging/__init__.py
--rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.1.4/quickbolt/logging/async_logger.py
--rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.1.4/quickbolt/pytest/__init__.py
--rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.1.4/quickbolt/pytest/core_pytest_base.py
--rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.1.4/quickbolt/reporting/__init__.py
--rw-r--r--   0        0        0     7522 2023-07-05 05:48:43.803436 quickbolt-0.1.4/quickbolt/reporting/response_csv.py
--rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.1.4/quickbolt/utils/__init__.py
--rw-r--r--   0        0        0     4529 2023-07-05 05:48:43.803703 quickbolt-0.1.4/quickbolt/utils/dictionary.py
--rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.1.4/quickbolt/utils/directory.py
--rw-r--r--   0        0        0     1763 2023-06-27 06:26:52.439989 quickbolt-0.1.4/quickbolt/utils/json.py
--rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.1.4/quickbolt/utils/sync_async.py
--rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.1.4/quickbolt/validations/__init__.py
--rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.1.4/quickbolt/validations/validations.py
--rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 quickbolt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-25 19:02:56.839509 quickbolt-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3964 2023-07-03 21:01:01.355674 quickbolt-0.1.5/README.md
+-rw-r--r--   0        0        0     1238 2023-07-08 00:26:07.761170 quickbolt-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.870537 quickbolt-0.1.5/quickbolt/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-22 00:25:13.788071 quickbolt-0.1.5/quickbolt/batch_generation/__init__.py
+-rw-r--r--   0        0        0    11377 2023-07-07 23:59:06.071578 quickbolt-0.1.5/quickbolt/batch_generation/batch_generation.py
+-rw-r--r--   0        0        0      114 2023-06-22 00:25:13.787989 quickbolt-0.1.5/quickbolt/clients/__init__.py
+-rw-r--r--   0        0        0     9806 2023-06-29 16:19:54.925810 quickbolt-0.1.5/quickbolt/clients/aio_requests.py
+-rw-r--r--   0        0        0    10021 2023-06-29 16:19:54.926154 quickbolt-0.1.5/quickbolt/clients/httpx_requests.py
+-rw-r--r--   0        0        0       55 2023-06-24 02:54:47.182831 quickbolt-0.1.5/quickbolt/logging/__init__.py
+-rw-r--r--   0        0        0     4335 2023-06-29 16:19:54.926720 quickbolt-0.1.5/quickbolt/logging/async_logger.py
+-rw-r--r--   0        0        0       61 2023-06-24 21:22:04.712776 quickbolt-0.1.5/quickbolt/pytest/__init__.py
+-rw-r--r--   0        0        0     4628 2023-06-29 16:19:54.927083 quickbolt-0.1.5/quickbolt/pytest/core_pytest_base.py
+-rw-r--r--   0        0        0        0 2023-06-17 17:15:51.872282 quickbolt-0.1.5/quickbolt/reporting/__init__.py
+-rw-r--r--   0        0        0     7522 2023-07-05 05:48:43.803436 quickbolt-0.1.5/quickbolt/reporting/response_csv.py
+-rw-r--r--   0        0        0        0 2023-06-22 00:47:05.860388 quickbolt-0.1.5/quickbolt/utils/__init__.py
+-rw-r--r--   0        0        0     4529 2023-07-05 05:48:43.803703 quickbolt-0.1.5/quickbolt/utils/dictionary.py
+-rw-r--r--   0        0        0     4096 2023-06-24 17:54:58.289703 quickbolt-0.1.5/quickbolt/utils/directory.py
+-rw-r--r--   0        0        0     2802 2023-07-07 23:59:06.071757 quickbolt-0.1.5/quickbolt/utils/json.py
+-rw-r--r--   0        0        0      398 2023-06-24 18:00:50.491754 quickbolt-0.1.5/quickbolt/utils/sync_async.py
+-rw-r--r--   0        0        0       58 2023-06-22 00:25:13.787912 quickbolt-0.1.5/quickbolt/validations/__init__.py
+-rw-r--r--   0        0        0     4866 2023-06-29 16:19:50.859546 quickbolt-0.1.5/quickbolt/validations/validations.py
+-rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 quickbolt-0.1.5/PKG-INFO
```

### Comparing `quickbolt-0.1.4/LICENSE` & `quickbolt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.4/README.md` & `quickbolt-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.4/pyproject.toml` & `quickbolt-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quickbolt"
-version = "0.1.4"
+version = "0.1.5"
 description = "Asynchronously make and validate requests!"
 authors = ["Ashton Szabo <aszabo00@gmail.com>"]
 repository = "https://github.com/aszabo00/quickbolt"
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Intended Audience :: Information Technology",
```

### Comparing `quickbolt-0.1.4/quickbolt/batch_generation/batch_generation.py` & `quickbolt-0.1.5/quickbolt/batch_generation/batch_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,16 +190,17 @@
     if ";" not in parsed.path:
         marked_path = f";{path}"
         marked_url = marked_url.replace(path, marked_path)
         path = marked_path
 
     _, params = path.split(";")
     params_split = params.lstrip("/").split("/")
+    params_keys = [f"{p}_{i}" for i, p in enumerate(params_split)]
 
-    corruptables = {"params": dict(zip(params_split, params_split))}
+    corruptables = {"params": dict(zip(params_keys, params_split))}
     if corrupt_query_params:
         corruptables.update(query_dict)
     corruptables = dh.flatten(corruptables)
     corruptables_ser = jh.serialize(corruptables)
 
     bad_combos_des = generate_bad_data(corruptables_ser, corruptables, sub_values, min)
     bad_combos_unfl = [dh.unflatten(b) for b in bad_combos_des]
```

### Comparing `quickbolt-0.1.4/quickbolt/clients/aio_requests.py` & `quickbolt-0.1.5/quickbolt/clients/aio_requests.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.4/quickbolt/clients/httpx_requests.py` & `quickbolt-0.1.5/quickbolt/clients/httpx_requests.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.4/quickbolt/logging/async_logger.py` & `quickbolt-0.1.5/quickbolt/logging/async_logger.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.4/quickbolt/pytest/core_pytest_base.py` & `quickbolt-0.1.5/quickbolt/pytest/core_pytest_base.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.4/quickbolt/reporting/response_csv.py` & `quickbolt-0.1.5/quickbolt/reporting/response_csv.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.4/quickbolt/utils/dictionary.py` & `quickbolt-0.1.5/quickbolt/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.4/quickbolt/utils/directory.py` & `quickbolt-0.1.5/quickbolt/utils/directory.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.4/quickbolt/validations/validations.py` & `quickbolt-0.1.5/quickbolt/validations/validations.py`

 * *Files identical despite different names*

### Comparing `quickbolt-0.1.4/PKG-INFO` & `quickbolt-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbolt
-Version: 0.1.4
+Version: 0.1.5
 Summary: Asynchronously make and validate requests!
 Home-page: https://github.com/aszabo00/quickbolt
 License: MIT
 Author: Ashton Szabo
 Author-email: aszabo00@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: Developers
```

