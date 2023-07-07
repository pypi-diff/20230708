# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722.tar", last modified: Fri Jul  7 18:48:24 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306.tar", last modified: Fri Jul  7 22:24:06 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:48:24.367593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-07 18:48:24.367593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 18:48:24.367593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-07 18:48:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:48:24.363593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:48:24.367593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15457 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3959 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:48:24.367593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-07 18:48:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-07 18:48:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 18:48:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-07 18:48:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-07 18:48:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:24:06.652116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-07 22:24:06.652116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 22:24:06.652116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-07 22:24:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:24:06.648116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:24:06.648116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15504 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-07-07 22:23:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:24:06.652116 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-07 22:24:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-07 22:24:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 22:24:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-07 22:24:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-07 22:24:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230707184722
+Version: 1.0.0.dev20230707222306
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230707184722",
+  version="1.0.0.dev20230707222306",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,20 +304,22 @@
     # TODO: I am thinking that that this won't delete everything?
     #  Needs batches -rk
     #  Needs passed in list of files by prefix
     def __remove_existing_s3_objects(
         self,
         output_zarr_prefix
     ):
+        print('removing existing s3 objects')
         for key in self.__s3.list_objects(  # problem here
                 bucket_name=self.__output_bucket,
                 prefix=output_zarr_prefix,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
         ):
+
             self.__s3.delete(
                 bucket_name=self.__output_bucket,
                 key=key,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
             )
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import boto3
 from collections.abc import Generator
 
 class S3Operations:
     #####################################################################
-    def __get_client(self, access_key_id=None, secret_access_key=None):
+    def __get_client(
+        self,
+        access_key_id=None,
+        secret_access_key=None
+    ):
         client = None
         if access_key_id:
             client = boto3.Session().client(
                 service_name='s3',
                 aws_access_key_id=access_key_id,
                 aws_secret_access_key=secret_access_key
             )
@@ -16,24 +20,27 @@
         return client
 
     #####################################################################
     def list_objects(  # analog to "find_children_objects"
         self,
         bucket_name,
         prefix,
-        access_key_id,
-        secret_access_key
+        access_key_id=None,
+        secret_access_key=None
     ):
         keys = []
-        for page in self.__get_client(
-                access_key_id,
-                secret_access_key
-        ).get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
+        s3_client = self.__get_client(
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key
+        )
+        print(s3_client.meta.endpoint_url)
+        print(s3_client.meta.region_name)
+        print(s3_client.meta.config.signature_version)  # s3v4
+        for page in s3_client.get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
             # problem here
-            contents = page["Contents"]
             if 'Contents' in page.keys():
                 keys.extend(page['Contents'])
         return keys
 
     #####################################################################
     def get_s3_files(self):
         # gets a set of files
@@ -45,16 +52,16 @@
         bucket_name,
         key,
         file_name,
         access_key_id=None,  # This should always be a bucket we have aws credentials for
         secret_access_key=None
     ):
         self.__get_client(
-            access_key_id,
-            secret_access_key
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key
         ).download_file(Bucket=bucket_name, Key=key, Filename=file_name)
 
     #####################################################################
     def __chunked(
             self,
             ll: list,
             n: int
@@ -80,15 +87,18 @@
     def delete(
         self,
         bucket_name,
         key,
         access_key_id=None,
         secret_access_key=None
     ):
-        self.__get_client(access_key_id, secret_access_key).delete_object(
+        self.__get_client(
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key
+        ).delete_object(
             Bucket=bucket_name,
             Key=key,
         )
 
     #####################################################################
     def delete_children_files(  # was "delete_remote_objects"
         self,
@@ -99,15 +109,18 @@
     ):
         # deletes all given keys in s3 bucket
         objects_to_delete = []
         for raw_zarr_file in raw_zarr_files:
             objects_to_delete.append({'Key': raw_zarr_file['Key']})
         # Delete in groups of 100 — Boto3 constraint
         for batch in self.__chunked(ll=objects_to_delete, n=100):
-            deleted = self.__get_client(access_key_id, secret_access_key).delete_objects(
+            deleted = self.__get_client(
+                access_key_id=access_key_id,
+                secret_access_key=secret_access_key
+            ).delete_objects(
                 Bucket=output_bucket,
                 Delete={
                     "Objects": batch
                 }
             )
             print(f"Deleted {len(deleted['Deleted'])} files")
 
@@ -117,10 +130,10 @@
         file_name,
         bucket_name,
         key,
         access_key_id=None,
         secret_access_key=None
     ):
         self.__get_client(
-            access_key_id,
-            secret_access_key
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key
         ).upload_file(file_name, bucket_name, key)
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230707184722
+Version: 1.0.0.dev20230707222306
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707222306/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

