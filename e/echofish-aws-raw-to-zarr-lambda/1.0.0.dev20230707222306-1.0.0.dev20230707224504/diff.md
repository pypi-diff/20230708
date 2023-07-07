# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306.tar", last modified: Fri Jul  7 22:24:06 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504.tar", last modified: Fri Jul  7 22:46:05 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:24:06.652116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-07 22:24:06.652116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 22:24:06.652116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-07 22:24:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:24:06.648116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:24:06.648116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15504 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:24:06.652116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-07 22:24:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-07 22:24:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 22:24:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-07 22:24:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-07 22:24:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:46:05.001730 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-07 22:44:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-07 22:46:05.001730 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-07 22:44:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 22:46:05.001730 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-07 22:46:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:46:04.997730 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:46:04.997730 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 22:44:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-07 22:44:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15582 2023-07-07 22:44:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-07 22:44:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4535 2023-07-07 22:44:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:46:05.001730 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-07 22:46:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-07 22:46:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 22:46:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-07 22:46:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-07 22:46:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230707222306
+Version: 1.0.0.dev20230707224504
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230707222306",
+  version="1.0.0.dev20230707224504",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,14 +305,16 @@
     #  Needs batches -rk
     #  Needs passed in list of files by prefix
     def __remove_existing_s3_objects(
         self,
         output_zarr_prefix
     ):
         print('removing existing s3 objects')
+        print('access key id')
+        print(self.__output_bucket_access_key)
         for key in self.__s3.list_objects(  # problem here
                 bucket_name=self.__output_bucket,
                 prefix=output_zarr_prefix,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
         ):
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,25 @@
     def list_objects(  # analog to "find_children_objects"
         self,
         bucket_name,
         prefix,
         access_key_id=None,
         secret_access_key=None
     ):
+        print(access_key_id)
         keys = []
         s3_client = self.__get_client(
             access_key_id=access_key_id,
             secret_access_key=secret_access_key
         )
+        s3_client.get_bucket_policy(Bucket='noaa-wcsd-zarr-pds')
         print(s3_client.meta.endpoint_url)
         print(s3_client.meta.region_name)
         print(s3_client.meta.config.signature_version)  # s3v4
+        print(s3_client.get_bucket_policy(Bucket='noaa-wcsd-zarr-pds'))
         for page in s3_client.get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
             # problem here
             if 'Contents' in page.keys():
                 keys.extend(page['Contents'])
         return keys
 
     #####################################################################
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230707222306
+Version: 1.0.0.dev20230707224504
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707224504/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

