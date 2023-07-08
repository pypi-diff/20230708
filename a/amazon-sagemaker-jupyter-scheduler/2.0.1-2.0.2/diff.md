# Comparing `tmp/amazon_sagemaker_jupyter_scheduler-2.0.1.tar.gz` & `tmp/amazon_sagemaker_jupyter_scheduler-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_sagemaker_jupyter_scheduler-2.0.1.tar", last modified: Wed Jul  5 23:58:08 2023, max compression
+gzip compressed data, was "amazon_sagemaker_jupyter_scheduler-2.0.2.tar", last modified: Sat Jul  8 01:27:42 2023, max compression
```

## Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1.tar` & `amazon_sagemaker_jupyter_scheduler-2.0.2.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.125582 amazon_sagemaker_jupyter_scheduler-2.0.1/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/.eslintignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1026 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/.eslintrc.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1605 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/.gitignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/.prettierignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/.prettierrc
--rw-r--r--   0 p4admin  (12569) amazon     (100)      739 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/Config
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2329 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/DEVELOPMENT.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)      686 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/MANIFEST.in
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-07-05 23:58:08.125582 amazon_sagemaker_jupyter_scheduler-2.0.1/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)      347 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/README.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2046 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/RELEASE.md
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.101583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      806 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      455 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/_version.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.105583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/advanced_environments/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/advanced_environments/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      163 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/advanced_environments/base_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5969 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    13864 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2541 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/app_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      465 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/aws_config.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.093583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/botocore_model/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.093583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.105583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/
--rw-r--r--   0 p4admin  (12569) amazon     (100)  1469732 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)    19161 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/clients.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2538 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/cron_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2060 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/deletable_resource.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1501 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/environment_detector.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5211 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3338 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      820 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/extension.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5757 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/file_uploader.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6084 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    65897 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1533 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.105583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4948 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.093583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/schemas/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.093583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.105583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1130 2023-07-05 23:57:57.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4834 2023-07-05 23:57:57.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.109583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   242036 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      166 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    26299 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)   106222 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      412 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    13283 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   209775 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      706 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4059 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    50576 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/993.faa5510ce9696a850c76.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8346 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.a68376e83adb25bf29b1.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-07-05 23:57:57.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    66200 2023-07-05 23:58:07.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6440 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/logging.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    30236 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/model_converter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3796 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/models.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.109583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      759 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      528 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/revenue.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9468 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4682 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3788 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/tags.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2295 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      498 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/s3_uri.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    43813 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/scheduler.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.113582 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/__init__.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.113582 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/helpers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/helpers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      913 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.113582 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/providers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/providers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9555 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8033 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    14065 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3180 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1145 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    17404 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1694 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2149 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1895 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1529 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1512 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6823 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2280 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3519 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5843 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    24154 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1747 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    33726 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      427 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_utils.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2805 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.101583 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler.egg-info/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-07-05 23:58:08.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9270 2023-07-05 23:58:08.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-07-05 23:58:08.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-07-05 23:58:08.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 p4admin  (12569) amazon     (100)      208 2023-07-05 23:58:08.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler.egg-info/requires.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-05 23:58:08.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler.egg-info/top_level.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)      261 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/babel.config.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)       73 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/custom.d.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      827 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/jest.config.base.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      510 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/jest.config.js
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.113582 amazon_sagemaker_jupyter_scheduler-2.0.1/jupyter-config/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.113582 amazon_sagemaker_jupyter_scheduler-2.0.1/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      109 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/jupyter-config/jupyter_server_config.d/amazon_sagemaker_jupyter_scheduler.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      306 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/jupyter-config/jupyter_server_config.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)   965893 2023-07-05 23:57:56.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/package-lock.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4834 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/package.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      127 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/pyproject.toml
--rw-r--r--   0 p4admin  (12569) amazon     (100)      133 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/requirements.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-07-05 23:58:08.125582 amazon_sagemaker_jupyter_scheduler-2.0.1/setup.cfg
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3069 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/setup.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.113582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.113582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/__mocks__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/__mocks__/fileMock.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.113582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/__tests__/
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    12302 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/__tests__/CreateNotebookJobForm.spec.tsx
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)     4348 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/__tests__/VpcCheckbox.spec.tsx
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    13449 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/__tests__/initalValueHelpers.spec.ts
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    11135 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/__tests__/validationHelpers.spec.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.093583 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.113582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      964 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/Link.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      754 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/RouterLink.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/__test__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1005 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/__test__/Link.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      609 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/__test__/RouterLink.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      184 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/selectinput/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1583 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/selectinput/SelectInput.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       56 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/selectinput/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      967 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/selectinput/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/textinput/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1626 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/textinput/TextInput.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/textinput/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1656 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/textinput/__tests__/TextInput.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       54 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/textinput/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2932 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/textinput/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      206 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/textinput/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/tooltip/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1348 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/tooltip/Tooltip.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/tooltip/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1040 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/tooltip/__tests__/Tooltip.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/tooltip/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      553 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/tooltip/styles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/constants/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7978 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/constants/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       53 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/constants/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       99 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/constants/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      186 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/plugins/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3429 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/plugins/ScheduleNotebookDisablerPlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1455 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/plugins/ScheduleNotebookPlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       92 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/plugins/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3328 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/themeProvider.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/types/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      420 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/types/images.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       82 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/types/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      141 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/types/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/types/sagemaker.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1929 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/PluginEnvironmentProvider.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.117582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1833 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      123 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1528 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/images.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      108 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1205 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1017 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/rendering.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.121582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4226 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJob.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.121582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.121582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/
--rw-r--r--   0 p4admin  (12569) amazon     (100)    15893 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.121582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3900 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3230 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1094 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.121582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3551 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       55 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      285 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4808 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    13805 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1229 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/InputContainer.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.121582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/JobEnvironment/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2737 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      712 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/JobEnvironment/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1280 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3138 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1554 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:58:08.125582 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1613 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6035 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      552 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12172 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    64113 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      781 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1305 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       41 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7544 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1727 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2216 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/mockResponses.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2723 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9250 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/tsconfig.base.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      304 2023-07-05 23:56:06.000000 amazon_sagemaker_jupyter_scheduler-2.0.1/tsconfig.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/.eslintignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1026 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/.eslintrc.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1605 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/.gitignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/.prettierignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/.prettierrc
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      739 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/Config
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2329 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/DEVELOPMENT.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      686 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/MANIFEST.in
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      347 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/README.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2046 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/RELEASE.md
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.148769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      806 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      455 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/_version.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.152769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      163 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/base_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5969 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    13864 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2541 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/app_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      465 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/aws_config.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.140769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/botocore_model/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.140769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.152769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)  1377688 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    19161 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/clients.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2538 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/cron_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2060 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/deletable_resource.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1501 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/environment_detector.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5211 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3338 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      820 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/extension.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5757 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/file_uploader.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6084 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    65897 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1533 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.152769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4948 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.140769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.140769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.152769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1130 2023-07-08 01:27:32.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4834 2023-07-08 01:27:32.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.156769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   242036 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      166 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    26299 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   106222 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      412 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    13283 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   209775 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      706 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4059 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    50576 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/993.faa5510ce9696a850c76.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8346 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.9f672e548acd2153a221.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-07-08 01:27:32.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    66200 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6440 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/logging.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    30236 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/model_converter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3796 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/models.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.156769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      759 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      528 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/revenue.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9468 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4682 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3788 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/tags.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2295 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      498 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/s3_uri.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    43813 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/scheduler.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.160769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/__init__.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.160769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/helpers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/helpers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      913 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.160769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9555 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8033 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    14065 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3180 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1145 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    17404 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1694 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2149 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1895 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1529 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1512 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6823 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2280 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3519 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5843 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    24154 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1747 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    33726 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      427 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_utils.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2805 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.152769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9270 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      208 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/requires.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      261 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/babel.config.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       73 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/custom.d.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      827 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/jest.config.base.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      510 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/jest.config.js
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.160769 amazon_sagemaker_jupyter_scheduler-2.0.2/jupyter-config/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.160769 amazon_sagemaker_jupyter_scheduler-2.0.2/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      109 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/jupyter-config/jupyter_server_config.d/amazon_sagemaker_jupyter_scheduler.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      306 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/jupyter-config/jupyter_server_config.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   965893 2023-07-08 01:27:31.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/package-lock.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4834 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/package.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      127 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/pyproject.toml
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      133 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/requirements.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/setup.cfg
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3069 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/setup.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__mocks__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__mocks__/fileMock.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    12302 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/CreateNotebookJobForm.spec.tsx
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)     4348 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/VpcCheckbox.spec.tsx
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    13449 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/initalValueHelpers.spec.ts
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    11135 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/validationHelpers.spec.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.140769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      964 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/Link.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      754 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/RouterLink.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/__test__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1005 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/__test__/Link.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      609 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/__test__/RouterLink.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      184 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1583 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/SelectInput.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       56 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      967 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1626 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/TextInput.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1656 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/__tests__/TextInput.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       54 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2932 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      206 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1348 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/Tooltip.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1040 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/__tests__/Tooltip.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      553 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/styles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/constants/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7978 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/constants/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       53 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/constants/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       99 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/constants/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      186 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3429 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/ScheduleNotebookDisablerPlugin.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1455 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/ScheduleNotebookPlugin.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       92 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3328 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/themeProvider.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/types/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      420 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/types/images.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       82 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/types/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      141 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/types/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/types/sagemaker.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1929 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/PluginEnvironmentProvider.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1833 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      123 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1528 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/images.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      108 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1205 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1017 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/rendering.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4226 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJob.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    15893 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3900 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3230 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1094 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3551 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       55 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      285 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4808 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    13805 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1229 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/InputContainer.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2737 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      712 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1280 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3138 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1554 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1613 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6035 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      552 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12172 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    64113 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      781 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1305 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       41 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7544 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1727 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2216 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/mockResponses.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2723 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9250 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/tsconfig.base.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      304 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/tsconfig.json
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/.eslintrc.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/.gitignore` & `amazon_sagemaker_jupyter_scheduler-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/Config` & `amazon_sagemaker_jupyter_scheduler-2.0.2/Config`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/DEVELOPMENT.md` & `amazon_sagemaker_jupyter_scheduler-2.0.2/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/MANIFEST.in` & `amazon_sagemaker_jupyter_scheduler-2.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/PKG-INFO` & `amazon_sagemaker_jupyter_scheduler-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_sagemaker_jupyter_scheduler
-Version: 2.0.1
+Version: 2.0.2
 Summary: Amazon SageMaker Jupyter Scheduler based on the https://pypi.org/project/jupyter-scheduler/
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Scheduling Notebooks,Notebooks,Amazon Sagemaker
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/RELEASE.md` & `amazon_sagemaker_jupyter_scheduler-2.0.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/__init__.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/app_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/app_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8833812564087994%*

 * *Differences: {"'documentation'": "'<p>Provides APIs for creating and managing Amazon SageMaker resources. </p> "*

 * *                    '<p>Other Resources:</p> <ul> <li> <p> <a '*

 * *                    'href="https://docs.aws.amazon.com/sagemaker/latest/dg/whatis.html#first-time-user">Amazon '*

 * *                    'SageMaker Developer Guide</a> </p> </li> <li> <p> <a '*

 * *                    'href="https://docs.aws.amazon.com/augmented-ai/2019-11-07/APIReference/Welcome.html">Amazon '*

 * *                    "Augmented AI Runtime AP […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<p>Provides APIs for creating and managing SageMaker resources. </p> <p>Other Resources:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/whatis.html#first-time-user\">SageMaker Developer Guide</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/augmented-ai/2019-11-07/APIReference/Welcome.html\">Amazon Augmented AI Runtime API Reference</a> </p> </li> </ul>",
+    "documentation": "<p>Provides APIs for creating and managing Amazon SageMaker resources. </p> <p>Other Resources:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/whatis.html#first-time-user\">Amazon SageMaker Developer Guide</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/augmented-ai/2019-11-07/APIReference/Welcome.html\">Amazon Augmented AI Runtime API Reference</a> </p> </li> </ul>",
     "metadata": {
         "apiVersion": "2017-07-24",
         "endpointPrefix": "api.sagemaker",
         "jsonVersion": "1.1",
         "protocol": "json",
         "serviceAbbreviation": "SageMaker",
         "serviceFullName": "Amazon SageMaker Service",
@@ -33,15 +33,15 @@
             },
             "name": "AddAssociation",
             "output": {
                 "shape": "AddAssociationResponse"
             }
         },
         "AddTags": {
-            "documentation": "<p>Adds or overwrites one or more tags for the specified SageMaker resource. You can add tags to notebook instances, training jobs, hyperparameter tuning jobs, batch transform jobs, models, labeling jobs, work teams, endpoint configurations, and endpoints.</p> <p>Each tag consists of a key and an optional value. Tag keys must be unique per resource. For more information about tags, see For more information, see <a href=\"https://aws.amazon.com/answers/account-management/aws-tagging-strategies/\">Amazon Web Services Tagging Strategies</a>.</p> <note> <p>Tags that you add to a hyperparameter tuning job by calling this API are also added to any training jobs that the hyperparameter tuning job launches after you call this API, but not to training jobs that the hyperparameter tuning job launched before you called this API. To make sure that the tags associated with a hyperparameter tuning job are also added to all training jobs that the hyperparameter tuning job launches, add the tags when you first create the tuning job by specifying them in the <code>Tags</code> parameter of <a>CreateHyperParameterTuningJob</a> </p> </note> <note> <p>Tags that you add to a SageMaker Studio Domain or User Profile by calling this API are also added to any Apps that the Domain or User Profile launches after you call this API, but not to Apps that the Domain or User Profile launched before you called this API. To make sure that the tags associated with a Domain or User Profile are also added to all Apps that the Domain or User Profile launches, add the tags when you first create the Domain or User Profile by specifying them in the <code>Tags</code> parameter of <a>CreateDomain</a> or <a>CreateUserProfile</a>.</p> </note>",
+            "documentation": "<p>Adds or overwrites one or more tags for the specified Amazon SageMaker resource. You can add tags to notebook instances, training jobs, hyperparameter tuning jobs, batch transform jobs, models, labeling jobs, work teams, endpoint configurations, and endpoints.</p> <p>Each tag consists of a key and an optional value. Tag keys must be unique per resource. For more information about tags, see For more information, see <a href=\"https://aws.amazon.com/answers/account-management/aws-tagging-strategies/\">Amazon Web Services Tagging Strategies</a>.</p> <note> <p>Tags that you add to a hyperparameter tuning job by calling this API are also added to any training jobs that the hyperparameter tuning job launches after you call this API, but not to training jobs that the hyperparameter tuning job launched before you called this API. To make sure that the tags associated with a hyperparameter tuning job are also added to all training jobs that the hyperparameter tuning job launches, add the tags when you first create the tuning job by specifying them in the <code>Tags</code> parameter of <a>CreateHyperParameterTuningJob</a> </p> </note> <note> <p>Tags that you add to a SageMaker Studio Domain or User Profile by calling this API are also added to any Apps that the Domain or User Profile launches after you call this API, but not to Apps that the Domain or User Profile launched before you called this API. To make sure that the tags associated with a Domain or User Profile are also added to all Apps that the Domain or User Profile launches, add the tags when you first create the Domain or User Profile by specifying them in the <code>Tags</code> parameter of <a>CreateDomain</a> or <a>CreateUserProfile</a>.</p> </note>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "AddTagsInput"
             },
@@ -102,29 +102,29 @@
             },
             "name": "CreateAction",
             "output": {
                 "shape": "CreateActionResponse"
             }
         },
         "CreateAlgorithm": {
-            "documentation": "<p>Create a machine learning algorithm that you can use in SageMaker and list in the Amazon Web Services Marketplace.</p>",
+            "documentation": "<p>Create a machine learning algorithm that you can use in Amazon SageMaker and list in the Amazon Web Services Marketplace.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateAlgorithmInput"
             },
             "name": "CreateAlgorithm",
             "output": {
                 "shape": "CreateAlgorithmOutput"
             }
         },
         "CreateApp": {
-            "documentation": "<p>Creates a running app for the specified UserProfile. This operation is automatically invoked by Amazon SageMaker Studio upon access to the associated Domain, and when new kernel configurations are selected by the user. A user may have multiple Apps active simultaneously.</p>",
+            "documentation": "<p>Creates a running app for the specified UserProfile. Supported apps are <code>JupyterServer</code> and <code>KernelGateway</code>. This operation is automatically invoked by Amazon SageMaker Studio upon access to the associated Domain, and when new kernel configurations are selected by the user. A user may have multiple Apps active simultaneously.</p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 },
                 {
                     "shape": "ResourceInUse"
                 }
@@ -198,15 +198,15 @@
             },
             "name": "CreateAutoMLJob",
             "output": {
                 "shape": "CreateAutoMLJobResponse"
             }
         },
         "CreateCodeRepository": {
-            "documentation": "<p>Creates a Git repository as a resource in your SageMaker account. You can associate the repository with notebook instances so that you can use Git source control for the notebooks you create. The Git repository is a resource in your SageMaker account, so it can be associated with more than one notebook instance, and it persists independently from the lifecycle of any notebook instances it is associated with.</p> <p>The repository can be hosted either in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository.</p>",
+            "documentation": "<p>Creates a Git repository as a resource in your Amazon SageMaker account. You can associate the repository with notebook instances so that you can use Git source control for the notebooks you create. The Git repository is a resource in your Amazon SageMaker account, so it can be associated with more than one notebook instance, and it persists independently from the lifecycle of any notebook instances it is associated with.</p> <p>The repository can be hosted either in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateCodeRepositoryInput"
             },
@@ -316,15 +316,14 @@
             },
             "name": "CreateDomain",
             "output": {
                 "shape": "CreateDomainResponse"
             }
         },
         "CreateEdgeDeploymentPlan": {
-            "documentation": "<p>Creates an edge deployment plan, consisting of multiple stages. Each stage may have a different deployment configuration and devices.</p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -335,15 +334,14 @@
             },
             "name": "CreateEdgeDeploymentPlan",
             "output": {
                 "shape": "CreateEdgeDeploymentPlanResponse"
             }
         },
         "CreateEdgeDeploymentStage": {
-            "documentation": "<p>Creates a new stage in an existing edge deployment plan.</p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -367,15 +365,15 @@
             },
             "input": {
                 "shape": "CreateEdgePackagingJobRequest"
             },
             "name": "CreateEdgePackagingJob"
         },
         "CreateEndpoint": {
-            "documentation": "<p>Creates an endpoint using the endpoint configuration specified in the request. SageMaker uses the endpoint to provision resources and deploy models. You create the endpoint configuration with the <a>CreateEndpointConfig</a> API. </p> <p> Use this API to deploy models using SageMaker hosting services. </p> <p>For an example that calls this method when deploying a model to SageMaker hosting services, see the <a href=\"https://github.com/aws/amazon-sagemaker-examples/blob/master/sagemaker-fundamentals/create-endpoint/create_endpoint.ipynb\">Create Endpoint example notebook.</a> </p> <note> <p> You must not delete an <code>EndpointConfig</code> that is in use by an endpoint that is live or while the <code>UpdateEndpoint</code> or <code>CreateEndpoint</code> operations are being performed on the endpoint. To update an endpoint, you must create a new <code>EndpointConfig</code>.</p> </note> <p>The endpoint name must be unique within an Amazon Web Services Region in your Amazon Web Services account. </p> <p>When it receives the request, SageMaker creates the endpoint, launches the resources (ML compute instances), and deploys the model(s) on them. </p> <note> <p>When you call <a>CreateEndpoint</a>, a load call is made to DynamoDB to verify that your endpoint configuration exists. When you read data from a DynamoDB table supporting <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html\"> <code>Eventually Consistent Reads</code> </a>, the response might not reflect the results of a recently completed write operation. The response might include some stale data. If the dependent entities are not yet in DynamoDB, this causes a validation error. If you repeat your read request after a short time, the response should return the latest data. So retry logic is recommended to handle these possible issues. We also recommend that customers call <a>DescribeEndpointConfig</a> before calling <a>CreateEndpoint</a> to minimize the potential impact of a DynamoDB eventually consistent read.</p> </note> <p>When SageMaker receives the request, it sets the endpoint status to <code>Creating</code>. After it creates the endpoint, it sets the status to <code>InService</code>. SageMaker can then process incoming requests for inferences. To check the status of an endpoint, use the <a>DescribeEndpoint</a> API.</p> <p>If any of the models hosted at this endpoint get model data from an Amazon S3 location, SageMaker uses Amazon Web Services Security Token Service to download model artifacts from the S3 path you provided. Amazon Web Services STS is activated in your IAM user account by default. If you previously deactivated Amazon Web Services STS for a region, you need to reactivate Amazon Web Services STS for that region. For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_enable-regions.html\">Activating and Deactivating Amazon Web Services STS in an Amazon Web Services Region</a> in the <i>Amazon Web Services Identity and Access Management User Guide</i>.</p> <note> <p> To add the IAM role policies for using this API operation, go to the <a href=\"https://console.aws.amazon.com/iam/\">IAM console</a>, and choose Roles in the left navigation pane. Search the IAM role that you want to grant access to use the <a>CreateEndpoint</a> and <a>CreateEndpointConfig</a> API operations, add the following policies to the role. </p> <ul> <li> <p>Option 1: For a full SageMaker access, search and attach the <code>AmazonSageMakerFullAccess</code> policy.</p> </li> <li> <p>Option 2: For granting a limited access to an IAM role, paste the following Action elements manually into the JSON file of the IAM role: </p> <p> <code>\"Action\": [\"sagemaker:CreateEndpoint\", \"sagemaker:CreateEndpointConfig\"]</code> </p> <p> <code>\"Resource\": [</code> </p> <p> <code>\"arn:aws:sagemaker:region:account-id:endpoint/endpointName\"</code> </p> <p> <code>\"arn:aws:sagemaker:region:account-id:endpoint-config/endpointConfigName\"</code> </p> <p> <code>]</code> </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/api-permissions-reference.html\">SageMaker API Permissions: Actions, Permissions, and Resources Reference</a>.</p> </li> </ul> </note>",
+            "documentation": "<p>Creates an endpoint using the endpoint configuration specified in the request. Amazon SageMaker uses the endpoint to provision resources and deploy models. You create the endpoint configuration with the <a>CreateEndpointConfig</a> API. </p> <p> Use this API to deploy models using Amazon SageMaker hosting services. </p> <p>For an example that calls this method when deploying a model to Amazon SageMaker hosting services, see the <a href=\"https://github.com/aws/amazon-sagemaker-examples/blob/master/sagemaker-fundamentals/create-endpoint/create_endpoint.ipynb\">Create Endpoint example notebook.</a> </p> <note> <p> You must not delete an <code>EndpointConfig</code> that is in use by an endpoint that is live or while the <code>UpdateEndpoint</code> or <code>CreateEndpoint</code> operations are being performed on the endpoint. To update an endpoint, you must create a new <code>EndpointConfig</code>.</p> </note> <p>The endpoint name must be unique within an Amazon Web Services Region in your Amazon Web Services account. </p> <p>When it receives the request, Amazon SageMaker creates the endpoint, launches the resources (ML compute instances), and deploys the model(s) on them. </p> <note> <p>When you call <a>CreateEndpoint</a>, a load call is made to DynamoDB to verify that your endpoint configuration exists. When you read data from a DynamoDB table supporting <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html\"> <code>Eventually Consistent Reads</code> </a>, the response might not reflect the results of a recently completed write operation. The response might include some stale data. If the dependent entities are not yet in DynamoDB, this causes a validation error. If you repeat your read request after a short time, the response should return the latest data. So retry logic is recommended to handle these possible issues. We also recommend that customers call <a>DescribeEndpointConfig</a> before calling <a>CreateEndpoint</a> to minimize the potential impact of a DynamoDB eventually consistent read.</p> </note> <p>When Amazon SageMaker receives the request, it sets the endpoint status to <code>Creating</code>. After it creates the endpoint, it sets the status to <code>InService</code>. Amazon SageMaker can then process incoming requests for inferences. To check the status of an endpoint, use the <a>DescribeEndpoint</a> API.</p> <p>If any of the models hosted at this endpoint get model data from an Amazon S3 location, Amazon SageMaker uses Amazon Web Services Security Token Service to download model artifacts from the S3 path you provided. Amazon Web Services STS is activated in your IAM user account by default. If you previously deactivated Amazon Web Services STS for a region, you need to reactivate Amazon Web Services STS for that region. For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_enable-regions.html\">Activating and Deactivating Amazon Web Services STS in an Amazon Web Services Region</a> in the <i>Amazon Web Services Identity and Access Management User Guide</i>.</p> <note> <p> To add the IAM role policies for using this API operation, go to the <a href=\"https://console.aws.amazon.com/iam/\">IAM console</a>, and choose Roles in the left navigation pane. Search the IAM role that you want to grant access to use the <a>CreateEndpoint</a> and <a>CreateEndpointConfig</a> API operations, add the following policies to the role. </p> <ul> <li> <p>Option 1: For a full SageMaker access, search and attach the <code>AmazonSageMakerFullAccess</code> policy.</p> </li> <li> <p>Option 2: For granting a limited access to an IAM role, paste the following Action elements manually into the JSON file of the IAM role: </p> <p> <code>\"Action\": [\"sagemaker:CreateEndpoint\", \"sagemaker:CreateEndpointConfig\"]</code> </p> <p> <code>\"Resource\": [</code> </p> <p> <code>\"arn:aws:sagemaker:region:account-id:endpoint/endpointName\"</code> </p> <p> <code>\"arn:aws:sagemaker:region:account-id:endpoint-config/endpointConfigName\"</code> </p> <p> <code>]</code> </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/api-permissions-reference.html\">SageMaker API Permissions: Actions, Permissions, and Resources Reference</a>.</p> </li> </ul> </note>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -386,15 +384,15 @@
             },
             "name": "CreateEndpoint",
             "output": {
                 "shape": "CreateEndpointOutput"
             }
         },
         "CreateEndpointConfig": {
-            "documentation": "<p>Creates an endpoint configuration that SageMaker hosting services uses to deploy models. In the configuration, you identify one or more models, created using the <code>CreateModel</code> API, to deploy and the resources that you want SageMaker to provision. Then you call the <a>CreateEndpoint</a> API.</p> <note> <p> Use this API if you want to use SageMaker hosting services to deploy models into production. </p> </note> <p>In the request, you define a <code>ProductionVariant</code>, for each model that you want to deploy. Each <code>ProductionVariant</code> parameter also describes the resources that you want SageMaker to provision. This includes the number and type of ML compute instances to deploy. </p> <p>If you are hosting multiple models, you also assign a <code>VariantWeight</code> to specify how much traffic you want to allocate to each model. For example, suppose that you want to host two models, A and B, and you assign traffic weight 2 for model A and 1 for model B. SageMaker distributes two-thirds of the traffic to Model A, and one-third to model B. </p> <note> <p>When you call <a>CreateEndpoint</a>, a load call is made to DynamoDB to verify that your endpoint configuration exists. When you read data from a DynamoDB table supporting <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html\"> <code>Eventually Consistent Reads</code> </a>, the response might not reflect the results of a recently completed write operation. The response might include some stale data. If the dependent entities are not yet in DynamoDB, this causes a validation error. If you repeat your read request after a short time, the response should return the latest data. So retry logic is recommended to handle these possible issues. We also recommend that customers call <a>DescribeEndpointConfig</a> before calling <a>CreateEndpoint</a> to minimize the potential impact of a DynamoDB eventually consistent read.</p> </note>",
+            "documentation": "<p>Creates an endpoint configuration that Amazon SageMaker hosting services uses to deploy models. In the configuration, you identify one or more models, created using the <code>CreateModel</code> API, to deploy and the resources that you want Amazon SageMaker to provision. Then you call the <a>CreateEndpoint</a> API.</p> <note> <p> Use this API if you want to use Amazon SageMaker hosting services to deploy models into production. </p> </note> <p>In the request, you define a <code>ProductionVariant</code>, for each model that you want to deploy. Each <code>ProductionVariant</code> parameter also describes the resources that you want Amazon SageMaker to provision. This includes the number and type of ML compute instances to deploy. </p> <p>If you are hosting multiple models, you also assign a <code>VariantWeight</code> to specify how much traffic you want to allocate to each model. For example, suppose that you want to host two models, A and B, and you assign traffic weight 2 for model A and 1 for model B. Amazon SageMaker distributes two-thirds of the traffic to Model A, and one-third to model B. </p> <note> <p>When you call <a>CreateEndpoint</a>, a load call is made to DynamoDB to verify that your endpoint configuration exists. When you read data from a DynamoDB table supporting <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html\"> <code>Eventually Consistent Reads</code> </a>, the response might not reflect the results of a recently completed write operation. The response might include some stale data. If the dependent entities are not yet in DynamoDB, this causes a validation error. If you repeat your read request after a short time, the response should return the latest data. So retry logic is recommended to handle these possible issues. We also recommend that customers call <a>DescribeEndpointConfig</a> before calling <a>CreateEndpoint</a> to minimize the potential impact of a DynamoDB eventually consistent read.</p> </note>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -490,15 +488,15 @@
             },
             "name": "CreateHumanTaskUi",
             "output": {
                 "shape": "CreateHumanTaskUiResponse"
             }
         },
         "CreateHyperParameterTuningJob": {
-            "documentation": "<p>Starts a hyperparameter tuning job. A hyperparameter tuning job finds the best version of a model by running many training jobs on your dataset using the algorithm you choose and values for hyperparameters within ranges that you specify. It then chooses the hyperparameter values that result in a model that performs the best, as measured by an objective metric that you choose.</p> <p>A hyperparameter tuning job automatically creates Amazon SageMaker experiments, trials, and trial components for each training job that it runs. You can view these entities in Amazon SageMaker Studio. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/experiments-view-compare.html#experiments-view\">View Experiments, Trials, and Trial Components</a>.</p> <important> <p>Do not include any security-sensitive information including account access IDs, secrets or tokens in any hyperparameter field. If the use of security-sensitive credentials are detected, SageMaker will reject your training job request and return an exception error.</p> </important>",
+            "documentation": "<p>Starts a hyperparameter tuning job. A hyperparameter tuning job finds the best version of a model by running many training jobs on your dataset using the algorithm you choose and values for hyperparameters within ranges that you specify. It then chooses the hyperparameter values that result in a model that performs the best, as measured by an objective metric that you choose.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 }
@@ -512,15 +510,15 @@
             },
             "name": "CreateHyperParameterTuningJob",
             "output": {
                 "shape": "CreateHyperParameterTuningJobResponse"
             }
         },
         "CreateImage": {
-            "documentation": "<p>Creates a custom SageMaker image. A SageMaker image is a set of image versions. Each image version represents a container image stored in Amazon Elastic Container Registry (ECR). For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/studio-byoi.html\">Bring your own SageMaker image</a>.</p>",
+            "documentation": "<p>Creates a custom SageMaker image. A SageMaker image is a set of image versions. Each image version represents a container image stored in Amazon Container Registry (ECR). For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/studio-byoi.html\">Bring your own SageMaker image</a>.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 }
@@ -534,15 +532,15 @@
             },
             "name": "CreateImage",
             "output": {
                 "shape": "CreateImageResponse"
             }
         },
         "CreateImageVersion": {
-            "documentation": "<p>Creates a version of the SageMaker image specified by <code>ImageName</code>. The version represents the Amazon Elastic Container Registry (ECR) container image specified by <code>BaseImage</code>.</p>",
+            "documentation": "<p>Creates a version of the SageMaker image specified by <code>ImageName</code>. The version represents the Amazon Container Registry (ECR) container image specified by <code>BaseImage</code>.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 },
@@ -558,14 +556,35 @@
                 "shape": "CreateImageVersionRequest"
             },
             "name": "CreateImageVersion",
             "output": {
                 "shape": "CreateImageVersionResponse"
             }
         },
+        "CreateInferenceExperiment": {
+            "errors": [
+                {
+                    "shape": "ResourceInUse"
+                },
+                {
+                    "shape": "ResourceLimitExceeded"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "CreateInferenceExperimentRequest"
+            },
+            "name": "CreateInferenceExperiment",
+            "output": {
+                "shape": "CreateInferenceExperimentResponse"
+            }
+        },
         "CreateInferenceRecommendationsJob": {
             "documentation": "<p>Starts a recommendation job. You can create either an instance recommendation or load test job.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
@@ -603,15 +622,15 @@
             },
             "name": "CreateLabelingJob",
             "output": {
                 "shape": "CreateLabelingJobResponse"
             }
         },
         "CreateModel": {
-            "documentation": "<p>Creates a model in SageMaker. In the request, you name the model and describe a primary container. For the primary container, you specify the Docker image that contains inference code, artifacts (from prior training), and a custom environment map that the inference code uses when you deploy the model for predictions.</p> <p>Use this API to create a model if you want to use SageMaker hosting services or run a batch transform job.</p> <p>To host your model, you create an endpoint configuration with the <code>CreateEndpointConfig</code> API, and then create an endpoint with the <code>CreateEndpoint</code> API. SageMaker then deploys all of the containers that you defined for the model in the hosting environment. </p> <p>For an example that calls this method when deploying a model to SageMaker hosting services, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/realtime-endpoints-deployment.html#realtime-endpoints-deployment-create-model\">Create a Model (Amazon Web Services SDK for Python (Boto 3)).</a> </p> <p>To run a batch transform using your model, you start a job with the <code>CreateTransformJob</code> API. SageMaker uses your model and your dataset to get inferences which are then saved to a specified S3 location.</p> <p>In the request, you also provide an IAM role that SageMaker can assume to access model artifacts and docker image for deployment on ML compute hosting instances or for batch transform jobs. In addition, you also use the IAM role to manage permissions the inference code needs. For example, if the inference code access any other Amazon Web Services resources, you grant necessary permissions via this role.</p>",
+            "documentation": "<p>Creates a model in Amazon SageMaker. In the request, you name the model and describe a primary container. For the primary container, you specify the Docker image that contains inference code, artifacts (from prior training), and a custom environment map that the inference code uses when you deploy the model for predictions.</p> <p>Use this API to create a model if you want to use Amazon SageMaker hosting services or run a batch transform job.</p> <p>To host your model, you create an endpoint configuration with the <code>CreateEndpointConfig</code> API, and then create an endpoint with the <code>CreateEndpoint</code> API. Amazon SageMaker then deploys all of the containers that you defined for the model in the hosting environment. </p> <p>For an example that calls this method when deploying a model to Amazon SageMaker hosting services, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/ex1-deploy-model.html#ex1-deploy-model-boto\">Deploy the Model to Amazon SageMaker Hosting Services (Amazon Web Services SDK for Python (Boto 3)).</a> </p> <p>To run a batch transform using your model, you start a job with the <code>CreateTransformJob</code> API. Amazon SageMaker uses your model and your dataset to get inferences which are then saved to a specified S3 location.</p> <p>In the <code>CreateModel</code> request, you must define a container with the <code>PrimaryContainer</code> parameter.</p> <p>In the request, you also provide an IAM role that Amazon SageMaker can assume to access model artifacts and docker image for deployment on ML compute hosting instances or for batch transform jobs. In addition, you also use the IAM role to manage permissions the inference code needs. For example, if the inference code access any other Amazon Web Services resources, you grant necessary permissions via this role.</p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -643,14 +662,59 @@
                 "shape": "CreateModelBiasJobDefinitionRequest"
             },
             "name": "CreateModelBiasJobDefinition",
             "output": {
                 "shape": "CreateModelBiasJobDefinitionResponse"
             }
         },
+        "CreateModelCard": {
+            "errors": [
+                {
+                    "shape": "ResourceLimitExceeded"
+                },
+                {
+                    "shape": "ConflictException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "CreateModelCardRequest"
+            },
+            "name": "CreateModelCard",
+            "output": {
+                "shape": "CreateModelCardResponse"
+            }
+        },
+        "CreateModelCardExportJob": {
+            "errors": [
+                {
+                    "shape": "ResourceNotFound"
+                },
+                {
+                    "shape": "ResourceLimitExceeded"
+                },
+                {
+                    "shape": "ConflictException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "CreateModelCardExportJobRequest"
+            },
+            "name": "CreateModelCardExportJob",
+            "output": {
+                "shape": "CreateModelCardExportJobResponse"
+            }
+        },
         "CreateModelExplainabilityJobDefinition": {
             "documentation": "<p>Creates the definition for a model explainability job.</p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 },
                 {
@@ -666,15 +730,15 @@
             },
             "name": "CreateModelExplainabilityJobDefinition",
             "output": {
                 "shape": "CreateModelExplainabilityJobDefinitionResponse"
             }
         },
         "CreateModelPackage": {
-            "documentation": "<p>Creates a model package that you can use to create SageMaker models or list on Amazon Web Services Marketplace, or a versioned model that is part of a model group. Buyers can subscribe to model packages listed on Amazon Web Services Marketplace to create models in SageMaker.</p> <p>To create a model package by specifying a Docker container that contains your inference code and the Amazon S3 location of your model artifacts, provide values for <code>InferenceSpecification</code>. To create a model from an algorithm resource that you created or subscribed to in Amazon Web Services Marketplace, provide a value for <code>SourceAlgorithmSpecification</code>.</p> <note> <p>There are two types of model packages:</p> <ul> <li> <p>Versioned - a model that is part of a model group in the model registry.</p> </li> <li> <p>Unversioned - a model package that is not part of a model group.</p> </li> </ul> </note>",
+            "documentation": "<p>Creates a model package that you can use to create Amazon SageMaker models or list on Amazon Web Services Marketplace, or a versioned model that is part of a model group. Buyers can subscribe to model packages listed on Amazon Web Services Marketplace to create models in Amazon SageMaker.</p> <p>To create a model package by specifying a Docker container that contains your inference code and the Amazon S3 location of your model artifacts, provide values for <code>InferenceSpecification</code>. To create a model from an algorithm resource that you created or subscribed to in Amazon Web Services Marketplace, provide a value for <code>SourceAlgorithmSpecification</code>.</p> <note> <p>There are two types of model packages:</p> <ul> <li> <p>Versioned - a model that is part of a model group in the model registry.</p> </li> <li> <p>Unversioned - a model package that is not part of a model group.</p> </li> </ul> </note>",
             "errors": [
                 {
                     "shape": "ConflictException"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 }
@@ -751,15 +815,15 @@
             },
             "name": "CreateMonitoringSchedule",
             "output": {
                 "shape": "CreateMonitoringScheduleResponse"
             }
         },
         "CreateNotebookInstance": {
-            "documentation": "<p>Creates an SageMaker notebook instance. A notebook instance is a machine learning (ML) compute instance running on a Jupyter notebook. </p> <p>In a <code>CreateNotebookInstance</code> request, specify the type of ML compute instance that you want to run. SageMaker launches the instance, installs common libraries that you can use to explore datasets for model training, and attaches an ML storage volume to the notebook instance. </p> <p>SageMaker also provides a set of example notebooks. Each notebook demonstrates how to use SageMaker with a specific algorithm or with a machine learning framework. </p> <p>After receiving the request, SageMaker does the following:</p> <ol> <li> <p>Creates a network interface in the SageMaker VPC.</p> </li> <li> <p>(Option) If you specified <code>SubnetId</code>, SageMaker creates a network interface in your own VPC, which is inferred from the subnet ID that you provide in the input. When creating this network interface, SageMaker attaches the security group that you specified in the request to the network interface that it creates in your VPC.</p> </li> <li> <p>Launches an EC2 instance of the type specified in the request in the SageMaker VPC. If you specified <code>SubnetId</code> of your VPC, SageMaker specifies both network interfaces when launching this instance. This enables inbound traffic from your own VPC to the notebook instance, assuming that the security groups allow it.</p> </li> </ol> <p>After creating the notebook instance, SageMaker returns its Amazon Resource Name (ARN). You can't change the name of a notebook instance after you create it.</p> <p>After SageMaker creates the notebook instance, you can connect to the Jupyter server and work in Jupyter notebooks. For example, you can write code to explore a dataset that you can use for model training, train a model, host models by creating SageMaker endpoints, and validate hosted models. </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/how-it-works.html\">How It Works</a>. </p>",
+            "documentation": "<p>Creates an Amazon SageMaker notebook instance. A notebook instance is a machine learning (ML) compute instance running on a Jupyter notebook. </p> <p>In a <code>CreateNotebookInstance</code> request, specify the type of ML compute instance that you want to run. Amazon SageMaker launches the instance, installs common libraries that you can use to explore datasets for model training, and attaches an ML storage volume to the notebook instance. </p> <p>Amazon SageMaker also provides a set of example notebooks. Each notebook demonstrates how to use Amazon SageMaker with a specific algorithm or with a machine learning framework. </p> <p>After receiving the request, Amazon SageMaker does the following:</p> <ol> <li> <p>Creates a network interface in the Amazon SageMaker VPC.</p> </li> <li> <p>(Option) If you specified <code>SubnetId</code>, Amazon SageMaker creates a network interface in your own VPC, which is inferred from the subnet ID that you provide in the input. When creating this network interface, Amazon SageMaker attaches the security group that you specified in the request to the network interface that it creates in your VPC.</p> </li> <li> <p>Launches an EC2 instance of the type specified in the request in the Amazon SageMaker VPC. If you specified <code>SubnetId</code> of your VPC, Amazon SageMaker specifies both network interfaces when launching this instance. This enables inbound traffic from your own VPC to the notebook instance, assuming that the security groups allow it.</p> </li> </ol> <p>After creating the notebook instance, Amazon SageMaker returns its Amazon Resource Name (ARN). You can't change the name of a notebook instance after you create it.</p> <p>After Amazon SageMaker creates the notebook instance, you can connect to the Jupyter server and work in Jupyter notebooks. For example, you can write code to explore a dataset that you can use for model training, train a model, host models by creating Amazon SageMaker endpoints, and validate hosted models. </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/how-it-works.html\">How It Works</a>. </p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -811,15 +875,15 @@
             },
             "name": "CreatePipeline",
             "output": {
                 "shape": "CreatePipelineResponse"
             }
         },
         "CreatePresignedDomainUrl": {
-            "documentation": "<p>Creates a URL for a specified UserProfile in a Domain. When accessed in a web browser, the user will be automatically signed in to Amazon SageMaker Studio, and granted access to all of the Apps and files associated with the Domain's Amazon Elastic File System (EFS) volume. This operation can only be called when the authentication mode equals IAM. </p> <p>The IAM role or user passed to this API defines the permissions to access the app. Once the presigned URL is created, no additional permission is required to access this URL. IAM authorization policies for this API are also enforced for every HTTP request and WebSocket frame that attempts to connect to the app.</p> <p>You can restrict access to this API and to the URL that it returns to a list of IP addresses, Amazon VPCs or Amazon VPC Endpoints that you specify. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/studio-interface-endpoint.html\">Connect to SageMaker Studio Through an Interface VPC Endpoint</a> .</p> <note> <p>The URL that you get from a call to <code>CreatePresignedDomainUrl</code> has a default timeout of 5 minutes. You can configure this value using <code>ExpiresInSeconds</code>. If you try to use the URL after the timeout limit expires, you are directed to the Amazon Web Services console sign-in page.</p> </note>",
+            "documentation": "<p>Creates a URL for a specified UserProfile in a Domain. When accessed in a web browser, the user will be automatically signed in to Amazon SageMaker Studio, and granted access to all of the Apps and files associated with the Domain's Amazon Elastic File System (EFS) volume. This operation can only be called when the authentication mode equals IAM. </p> <p>The IAM role or user used to call this API defines the permissions to access the app. Once the presigned URL is created, no additional permission is required to access this URL. IAM authorization policies for this API are also enforced for every HTTP request and WebSocket frame that attempts to connect to the app.</p> <p>You can restrict access to this API and to the URL that it returns to a list of IP addresses, Amazon VPCs or Amazon VPC Endpoints that you specify. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/studio-interface-endpoint.html\">Connect to SageMaker Studio Through an Interface VPC Endpoint</a> .</p> <note> <p>The URL that you get from a call to <code>CreatePresignedDomainUrl</code> has a default timeout of 5 minutes. You can configure this value using <code>ExpiresInSeconds</code>. If you try to use the URL after the timeout limit expires, you are directed to the Amazon Web Services console sign-in page.</p> </note>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -830,15 +894,15 @@
             },
             "name": "CreatePresignedDomainUrl",
             "output": {
                 "shape": "CreatePresignedDomainUrlResponse"
             }
         },
         "CreatePresignedNotebookInstanceUrl": {
-            "documentation": "<p>Returns a URL that you can use to connect to the Jupyter server from a notebook instance. In the SageMaker console, when you choose <code>Open</code> next to a notebook instance, SageMaker opens a new tab showing the Jupyter server home page from the notebook instance. The console uses this API to get the URL and show the page.</p> <p> The IAM role or user used to call this API defines the permissions to access the notebook instance. Once the presigned URL is created, no additional permission is required to access this URL. IAM authorization policies for this API are also enforced for every HTTP request and WebSocket frame that attempts to connect to the notebook instance.</p> <p>You can restrict access to this API and to the URL that it returns to a list of IP addresses that you specify. Use the <code>NotIpAddress</code> condition operator and the <code>aws:SourceIP</code> condition context key to specify the list of IP addresses that you want to have access to the notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/security_iam_id-based-policy-examples.html#nbi-ip-filter\">Limit Access to a Notebook Instance by IP Address</a>.</p> <note> <p>The URL that you get from a call to <a>CreatePresignedNotebookInstanceUrl</a> is valid only for 5 minutes. If you try to use the URL after the 5-minute limit expires, you are directed to the Amazon Web Services console sign-in page.</p> </note>",
+            "documentation": "<p>Returns a URL that you can use to connect to the Jupyter server from a notebook instance. In the Amazon SageMaker console, when you choose <code>Open</code> next to a notebook instance, Amazon SageMaker opens a new tab showing the Jupyter server home page from the notebook instance. The console uses this API to get the URL and show the page.</p> <p> The IAM role or user used to call this API defines the permissions to access the notebook instance. Once the presigned URL is created, no additional permission is required to access this URL. IAM authorization policies for this API are also enforced for every HTTP request and WebSocket frame that attempts to connect to the notebook instance.</p> <p>You can restrict access to this API and to the URL that it returns to a list of IP addresses that you specify. Use the <code>NotIpAddress</code> condition operator and the <code>aws:SourceIP</code> condition context key to specify the list of IP addresses that you want to have access to the notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/security_iam_id-based-policy-examples.html#nbi-ip-filter\">Limit Access to a Notebook Instance by IP Address</a>.</p> <note> <p>The URL that you get from a call to <a>CreatePresignedNotebookInstanceUrl</a> is valid only for 5 minutes. If you try to use the URL after the 5-minute limit expires, you are directed to the Amazon Web Services console sign-in page.</p> </note>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreatePresignedNotebookInstanceUrlInput"
             },
@@ -887,14 +951,35 @@
                 "shape": "CreateProjectInput"
             },
             "name": "CreateProject",
             "output": {
                 "shape": "CreateProjectOutput"
             }
         },
+        "CreateSpace": {
+            "errors": [
+                {
+                    "shape": "ResourceLimitExceeded"
+                },
+                {
+                    "shape": "ResourceInUse"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "CreateSpaceRequest"
+            },
+            "name": "CreateSpace",
+            "output": {
+                "shape": "CreateSpaceResponse"
+            }
+        },
         "CreateStudioLifecycleConfig": {
             "documentation": "<p>Creates a new Studio Lifecycle Configuration.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 }
             ],
@@ -907,15 +992,15 @@
             },
             "name": "CreateStudioLifecycleConfig",
             "output": {
                 "shape": "CreateStudioLifecycleConfigResponse"
             }
         },
         "CreateTrainingJob": {
-            "documentation": "<p>Starts a model training job. After training completes, SageMaker saves the resulting model artifacts to an Amazon S3 location that you specify. </p> <p>If you choose to host your model using SageMaker hosting services, you can use the resulting model artifacts as part of the model. You can also use the artifacts in a machine learning service other than SageMaker, provided that you know how to use them for inference. </p> <p>In the request body, you provide the following: </p> <ul> <li> <p> <code>AlgorithmSpecification</code> - Identifies the training algorithm to use. </p> </li> <li> <p> <code>HyperParameters</code> - Specify these algorithm-specific parameters to enable the estimation of model parameters during training. Hyperparameters can be tuned to optimize this learning process. For a list of hyperparameters for each training algorithm provided by SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. </p> <important> <p>Do not include any security-sensitive information including account access IDs, secrets or tokens in any hyperparameter field. If the use of security-sensitive credentials are detected, SageMaker will reject your training job request and return an exception error.</p> </important> </li> <li> <p> <code>InputDataConfig</code> - Describes the input required by the training job and the Amazon S3, EFS, or FSx location where it is stored.</p> </li> <li> <p> <code>OutputDataConfig</code> - Identifies the Amazon S3 bucket where you want SageMaker to save the results of model training. </p> </li> <li> <p> <code>ResourceConfig</code> - Identifies the resources, ML compute instances, and ML storage volumes to deploy for model training. In distributed training, you specify more than one instance. </p> </li> <li> <p> <code>EnableManagedSpotTraining</code> - Optimize the cost of training machine learning models by up to 80% by using Amazon EC2 Spot instances. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-managed-spot-training.html\">Managed Spot Training</a>. </p> </li> <li> <p> <code>RoleArn</code> - The Amazon Resource Name (ARN) that SageMaker assumes to perform tasks on your behalf during model training. You must grant this role the necessary permissions so that SageMaker can successfully complete model training. </p> </li> <li> <p> <code>StoppingCondition</code> - To help cap training costs, use <code>MaxRuntimeInSeconds</code> to set a time limit for training. Use <code>MaxWaitTimeInSeconds</code> to specify how long a managed spot training job has to complete. </p> </li> <li> <p> <code>Environment</code> - The environment variables to set in the Docker container.</p> </li> <li> <p> <code>RetryStrategy</code> - The number of times to retry the job when the job fails due to an <code>InternalServerError</code>.</p> </li> </ul> <p> For more information about SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/how-it-works.html\">How It Works</a>. </p>",
+            "documentation": "<p>Starts a model training job. After training completes, Amazon SageMaker saves the resulting model artifacts to an Amazon S3 location that you specify. </p> <p>If you choose to host your model using Amazon SageMaker hosting services, you can use the resulting model artifacts as part of the model. You can also use the artifacts in a machine learning service other than Amazon SageMaker, provided that you know how to use them for inference. </p> <p>In the request body, you provide the following: </p> <ul> <li> <p> <code>AlgorithmSpecification</code> - Identifies the training algorithm to use. </p> </li> <li> <p> <code>HyperParameters</code> - Specify these algorithm-specific parameters to enable the estimation of model parameters during training. Hyperparameters can be tuned to optimize this learning process. For a list of hyperparameters for each training algorithm provided by Amazon SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. </p> </li> <li> <p> <code>InputDataConfig</code> - Describes the training dataset and the Amazon S3, EFS, or FSx location where it is stored.</p> </li> <li> <p> <code>OutputDataConfig</code> - Identifies the Amazon S3 bucket where you want Amazon SageMaker to save the results of model training. </p> </li> <li> <p> <code>ResourceConfig</code> - Identifies the resources, ML compute instances, and ML storage volumes to deploy for model training. In distributed training, you specify more than one instance. </p> </li> <li> <p> <code>EnableManagedSpotTraining</code> - Optimize the cost of training machine learning models by up to 80% by using Amazon EC2 Spot instances. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-managed-spot-training.html\">Managed Spot Training</a>. </p> </li> <li> <p> <code>RoleArn</code> - The Amazon Resource Name (ARN) that Amazon SageMaker assumes to perform tasks on your behalf during model training. You must grant this role the necessary permissions so that Amazon SageMaker can successfully complete model training. </p> </li> <li> <p> <code>StoppingCondition</code> - To help cap training costs, use <code>MaxRuntimeInSeconds</code> to set a time limit for training. Use <code>MaxWaitTimeInSeconds</code> to specify how long a managed spot training job has to complete. </p> </li> <li> <p> <code>Environment</code> - The environment variables to set in the Docker container.</p> </li> <li> <p> <code>RetryStrategy</code> - The number of times to retry the job when the job fails due to an <code>InternalServerError</code>.</p> </li> </ul> <p> For more information about Amazon SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/how-it-works.html\">How It Works</a>. </p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 },
@@ -932,15 +1017,15 @@
             },
             "name": "CreateTrainingJob",
             "output": {
                 "shape": "CreateTrainingJobResponse"
             }
         },
         "CreateTransformJob": {
-            "documentation": "<p>Starts a transform job. A transform job uses a trained model to get inferences on a dataset and saves these results to an Amazon S3 location that you specify.</p> <p>To perform batch transformations, you create a transform job and use the data that you have readily available.</p> <p>In the request body, you provide the following:</p> <ul> <li> <p> <code>TransformJobName</code> - Identifies the transform job. The name must be unique within an Amazon Web Services Region in an Amazon Web Services account.</p> </li> <li> <p> <code>ModelName</code> - Identifies the model to use. <code>ModelName</code> must be the name of an existing Amazon SageMaker model in the same Amazon Web Services Region and Amazon Web Services account. For information on creating a model, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateModel.html\">CreateModel</a>.</p> </li> <li> <p> <code>TransformInput</code> - Describes the dataset to be transformed and the Amazon S3 location where it is stored.</p> </li> <li> <p> <code>TransformOutput</code> - Identifies the Amazon S3 location where you want Amazon SageMaker to save the results from the transform job.</p> </li> <li> <p> <code>TransformResources</code> - Identifies the ML compute instances for the transform job.</p> </li> </ul> <p>For more information about how batch transformation works, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-transform.html\">Batch Transform</a>.</p>",
+            "documentation": "<p>Starts a transform job. A transform job uses a trained model to get inferences on a dataset and saves these results to an Amazon S3 location that you specify.</p> <p>To perform batch transformations, you create a transform job and use the data that you have readily available.</p> <p>In the request body, you provide the following:</p> <ul> <li> <p> <code>TransformJobName</code> - Identifies the transform job. The name must be unique within an Amazon Web Services Region in an Amazon Web Services account.</p> </li> <li> <p> <code>ModelName</code> - Identifies the model to use. <code>ModelName</code> must be the name of an existing Amazon SageMaker model in the same Amazon Web Services Region and Amazon Web Services account. For information on creating a model, see <a>CreateModel</a>.</p> </li> <li> <p> <code>TransformInput</code> - Describes the dataset to be transformed and the Amazon S3 location where it is stored.</p> </li> <li> <p> <code>TransformOutput</code> - Identifies the Amazon S3 location where you want Amazon SageMaker to save the results from the transform job.</p> </li> <li> <p> <code>TransformResources</code> - Identifies the ML compute instances for the transform job.</p> </li> </ul> <p>For more information about how batch transformation works, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-transform.html\">Batch Transform</a>.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 },
@@ -998,15 +1083,15 @@
             },
             "name": "CreateTrialComponent",
             "output": {
                 "shape": "CreateTrialComponentResponse"
             }
         },
         "CreateUserProfile": {
-            "documentation": "<p>Creates a user profile. A user profile represents a single user within a domain, and is the main way to reference a \"person\" for the purposes of sharing, reporting, and other user-oriented features. This entity is created when a user onboards to Amazon SageMaker Studio. If an administrator invites a person by email or imports them from IAM Identity Center, a user profile is automatically created. A user profile is the primary holder of settings for an individual user and has a reference to the user's private Amazon Elastic File System (EFS) home directory. </p>",
+            "documentation": "<p>Creates a user profile. A user profile represents a single user within a domain, and is the main way to reference a \"person\" for the purposes of sharing, reporting, and other user-oriented features. This entity is created when a user onboards to Amazon SageMaker Studio. If an administrator invites a person by email or imports them from SSO, a user profile is automatically created. A user profile is the primary holder of settings for an individual user and has a reference to the user's private Amazon Elastic File System (EFS) home directory. </p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 },
                 {
                     "shape": "ResourceInUse"
                 }
@@ -1221,15 +1306,15 @@
             },
             "input": {
                 "shape": "DeleteDeviceFleetRequest"
             },
             "name": "DeleteDeviceFleet"
         },
         "DeleteDomain": {
-            "documentation": "<p>Used to delete a domain. If you onboarded with IAM mode, you will need to delete your domain to onboard again using IAM Identity Center. Use with caution. All of the members of the domain will lose access to their EFS volume, including data, notebooks, and other artifacts. </p>",
+            "documentation": "<p>Used to delete a domain. If you onboarded with IAM mode, you will need to delete your domain to onboard again using SSO. Use with caution. All of the members of the domain will lose access to their EFS volume, including data, notebooks, and other artifacts. </p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
                     "shape": "ResourceNotFound"
                 }
@@ -1240,15 +1325,14 @@
             },
             "input": {
                 "shape": "DeleteDomainRequest"
             },
             "name": "DeleteDomain"
         },
         "DeleteEdgeDeploymentPlan": {
-            "documentation": "<p>Deletes an edge deployment plan if (and only if) all the stages in the plan are inactive or there are no stages in the plan.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -1256,15 +1340,14 @@
             },
             "input": {
                 "shape": "DeleteEdgeDeploymentPlanRequest"
             },
             "name": "DeleteEdgeDeploymentPlan"
         },
         "DeleteEdgeDeploymentStage": {
-            "documentation": "<p>Delete a stage in an edge deployment plan if (and only if) the stage is inactive.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -1272,15 +1355,15 @@
             },
             "input": {
                 "shape": "DeleteEdgeDeploymentStageRequest"
             },
             "name": "DeleteEdgeDeploymentStage"
         },
         "DeleteEndpoint": {
-            "documentation": "<p>Deletes an endpoint. SageMaker frees up all of the resources that were deployed when the endpoint was created. </p> <p>SageMaker retires any custom KMS key grants associated with the endpoint, meaning you don't need to use the <a href=\"http://docs.aws.amazon.com/kms/latest/APIReference/API_RevokeGrant.html\">RevokeGrant</a> API call.</p> <p>When you delete your endpoint, SageMaker asynchronously deletes associated endpoint resources such as KMS key grants. You might still see these resources in your account for a few minutes after deleting your endpoint. Do not delete or revoke the permissions for your <code> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateModel.html#sagemaker-CreateModel-request-ExecutionRoleArn\">ExecutionRoleArn</a> </code>, otherwise SageMaker cannot delete these resources.</p>",
+            "documentation": "<p>Deletes an endpoint. Amazon SageMaker frees up all of the resources that were deployed when the endpoint was created. </p> <p>Amazon SageMaker retires any custom KMS key grants associated with the endpoint, meaning you don't need to use the <a href=\"http://docs.aws.amazon.com/kms/latest/APIReference/API_RevokeGrant.html\">RevokeGrant</a> API call.</p> <p>When you delete your endpoint, SageMaker asynchronously deletes associated endpoint resources such as KMS key grants. You might still see these resources in your account for a few minutes after deleting your endpoint. Do not delete or revoke the permissions for your <code> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateModel.html#sagemaker-CreateModel-request-ExecutionRoleArn\">ExecutionRoleArn</a> </code>, otherwise SageMaker cannot delete these resources.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteEndpointInput"
             },
@@ -1413,16 +1496,37 @@
                 "shape": "DeleteImageVersionRequest"
             },
             "name": "DeleteImageVersion",
             "output": {
                 "shape": "DeleteImageVersionResponse"
             }
         },
+        "DeleteInferenceExperiment": {
+            "errors": [
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DeleteInferenceExperimentRequest"
+            },
+            "name": "DeleteInferenceExperiment",
+            "output": {
+                "shape": "DeleteInferenceExperimentResponse"
+            }
+        },
         "DeleteModel": {
-            "documentation": "<p>Deletes a model. The <code>DeleteModel</code> API deletes only the model entry that was created in SageMaker when you called the <code>CreateModel</code> API. It does not delete model artifacts, inference code, or the IAM role that you specified when creating the model. </p>",
+            "documentation": "<p>Deletes a model. The <code>DeleteModel</code> API deletes only the model entry that was created in Amazon SageMaker when you called the <code>CreateModel</code> API. It does not delete model artifacts, inference code, or the IAM role that you specified when creating the model. </p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteModelInput"
             },
@@ -1440,14 +1544,32 @@
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteModelBiasJobDefinitionRequest"
             },
             "name": "DeleteModelBiasJobDefinition"
         },
+        "DeleteModelCard": {
+            "errors": [
+                {
+                    "shape": "ResourceNotFound"
+                },
+                {
+                    "shape": "ConflictException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DeleteModelCardRequest"
+            },
+            "name": "DeleteModelCard"
+        },
         "DeleteModelExplainabilityJobDefinition": {
             "documentation": "<p>Deletes an Amazon SageMaker model explainability job definition.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
@@ -1457,15 +1579,15 @@
             },
             "input": {
                 "shape": "DeleteModelExplainabilityJobDefinitionRequest"
             },
             "name": "DeleteModelExplainabilityJobDefinition"
         },
         "DeleteModelPackage": {
-            "documentation": "<p>Deletes a model package.</p> <p>A model package is used to create SageMaker models or list on Amazon Web Services Marketplace. Buyers can subscribe to model packages listed on Amazon Web Services Marketplace to create models in SageMaker.</p>",
+            "documentation": "<p>Deletes a model package.</p> <p>A model package is used to create Amazon SageMaker models or list on Amazon Web Services Marketplace. Buyers can subscribe to model packages listed on Amazon Web Services Marketplace to create models in Amazon SageMaker.</p>",
             "errors": [
                 {
                     "shape": "ConflictException"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -1532,15 +1654,15 @@
             },
             "input": {
                 "shape": "DeleteMonitoringScheduleRequest"
             },
             "name": "DeleteMonitoringSchedule"
         },
         "DeleteNotebookInstance": {
-            "documentation": "<p> Deletes an SageMaker notebook instance. Before you can delete a notebook instance, you must call the <code>StopNotebookInstance</code> API. </p> <important> <p>When you delete a notebook instance, you lose all of your data. SageMaker removes the ML compute instance, and deletes the ML storage volume and the network interface associated with the notebook instance. </p> </important>",
+            "documentation": "<p> Deletes an Amazon SageMaker notebook instance. Before you can delete a notebook instance, you must call the <code>StopNotebookInstance</code> API. </p> <important> <p>When you delete a notebook instance, you lose all of your data. Amazon SageMaker removes the ML compute instance, and deletes the ML storage volume and the network interface associated with the notebook instance. </p> </important>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteNotebookInstanceInput"
             },
@@ -1588,14 +1710,32 @@
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteProjectInput"
             },
             "name": "DeleteProject"
         },
+        "DeleteSpace": {
+            "errors": [
+                {
+                    "shape": "ResourceInUse"
+                },
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DeleteSpaceRequest"
+            },
+            "name": "DeleteSpace"
+        },
         "DeleteStudioLifecycleConfig": {
             "documentation": "<p>Deletes the Studio Lifecycle Configuration. In order to delete the Lifecycle Configuration, there must be no running apps using the Lifecycle Configuration. You must also remove the Lifecycle Configuration from UserSettings in all Domains and UserProfiles.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 },
                 {
@@ -1608,15 +1748,15 @@
             },
             "input": {
                 "shape": "DeleteStudioLifecycleConfigRequest"
             },
             "name": "DeleteStudioLifecycleConfig"
         },
         "DeleteTags": {
-            "documentation": "<p>Deletes the specified tags from an SageMaker resource.</p> <p>To list a resource's tags, use the <code>ListTags</code> API. </p> <note> <p>When you call this API to delete tags from a hyperparameter tuning job, the deleted tags are not removed from training jobs that the hyperparameter tuning job launched before you called this API.</p> </note> <note> <p>When you call this API to delete tags from a SageMaker Studio Domain or User Profile, the deleted tags are not removed from Apps that the SageMaker Studio Domain or User Profile launched before you called this API.</p> </note>",
+            "documentation": "<p>Deletes the specified tags from an Amazon SageMaker resource.</p> <p>To list a resource's tags, use the <code>ListTags</code> API. </p> <note> <p>When you call this API to delete tags from a hyperparameter tuning job, the deleted tags are not removed from training jobs that the hyperparameter tuning job launched before you called this API.</p> </note> <note> <p>When you call this API to delete tags from a SageMaker Studio Domain or User Profile, the deleted tags are not removed from Apps that the SageMaker Studio Domain or User Profile launched before you called this API.</p> </note>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteTagsInput"
             },
@@ -1960,15 +2100,14 @@
             },
             "name": "DescribeDomain",
             "output": {
                 "shape": "DescribeDomainResponse"
             }
         },
         "DescribeEdgeDeploymentPlan": {
-            "documentation": "<p>Describes an edge deployment plan with deployment status per stage.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -2064,15 +2203,14 @@
             },
             "name": "DescribeFeatureGroup",
             "output": {
                 "shape": "DescribeFeatureGroupResponse"
             }
         },
         "DescribeFeatureMetadata": {
-            "documentation": "<p>Shows the metadata for a feature within a feature group.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -2177,14 +2315,32 @@
                 "shape": "DescribeImageVersionRequest"
             },
             "name": "DescribeImageVersion",
             "output": {
                 "shape": "DescribeImageVersionResponse"
             }
         },
+        "DescribeInferenceExperiment": {
+            "errors": [
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DescribeInferenceExperimentRequest"
+            },
+            "name": "DescribeInferenceExperiment",
+            "output": {
+                "shape": "DescribeInferenceExperimentResponse"
+            }
+        },
         "DescribeInferenceRecommendationsJob": {
             "documentation": "<p>Provides the results of the Inference Recommender job. One or more recommendation jobs are returned.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
@@ -2267,14 +2423,50 @@
                 "shape": "DescribeModelBiasJobDefinitionRequest"
             },
             "name": "DescribeModelBiasJobDefinition",
             "output": {
                 "shape": "DescribeModelBiasJobDefinitionResponse"
             }
         },
+        "DescribeModelCard": {
+            "errors": [
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DescribeModelCardRequest"
+            },
+            "name": "DescribeModelCard",
+            "output": {
+                "shape": "DescribeModelCardResponse"
+            }
+        },
+        "DescribeModelCardExportJob": {
+            "errors": [
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DescribeModelCardExportJobRequest"
+            },
+            "name": "DescribeModelCardExportJob",
+            "output": {
+                "shape": "DescribeModelCardExportJobResponse"
+            }
+        },
         "DescribeModelExplainabilityJobDefinition": {
             "documentation": "<p>Returns a description of a model explainability job definition.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
@@ -2470,14 +2662,32 @@
                 "shape": "DescribeProjectInput"
             },
             "name": "DescribeProject",
             "output": {
                 "shape": "DescribeProjectOutput"
             }
         },
+        "DescribeSpace": {
+            "errors": [
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DescribeSpaceRequest"
+            },
+            "name": "DescribeSpace",
+            "output": {
+                "shape": "DescribeSpaceResponse"
+            }
+        },
         "DescribeStudioLifecycleConfig": {
             "documentation": "<p>Describes the Studio Lifecycle Configuration.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
@@ -2984,15 +3194,14 @@
             },
             "name": "ListDomains",
             "output": {
                 "shape": "ListDomainsResponse"
             }
         },
         "ListEdgeDeploymentPlans": {
-            "documentation": "<p>Lists all edge deployment plans.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListEdgeDeploymentPlansRequest"
             },
@@ -3142,16 +3351,28 @@
                 "shape": "ListImagesRequest"
             },
             "name": "ListImages",
             "output": {
                 "shape": "ListImagesResponse"
             }
         },
+        "ListInferenceExperiments": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListInferenceExperimentsRequest"
+            },
+            "name": "ListInferenceExperiments",
+            "output": {
+                "shape": "ListInferenceExperimentsResponse"
+            }
+        },
         "ListInferenceRecommendationsJobSteps": {
-            "documentation": "<p>Returns a list of the subtasks for an Inference Recommender job.</p> <p>The supported subtasks are benchmarks, which evaluate the performance of your model on different instance types.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListInferenceRecommendationsJobStepsRequest"
             },
@@ -3231,14 +3452,58 @@
                 "shape": "ListModelBiasJobDefinitionsRequest"
             },
             "name": "ListModelBiasJobDefinitions",
             "output": {
                 "shape": "ListModelBiasJobDefinitionsResponse"
             }
         },
+        "ListModelCardExportJobs": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListModelCardExportJobsRequest"
+            },
+            "name": "ListModelCardExportJobs",
+            "output": {
+                "shape": "ListModelCardExportJobsResponse"
+            }
+        },
+        "ListModelCardVersions": {
+            "errors": [
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListModelCardVersionsRequest"
+            },
+            "name": "ListModelCardVersions",
+            "output": {
+                "shape": "ListModelCardVersionsResponse"
+            }
+        },
+        "ListModelCards": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListModelCardsRequest"
+            },
+            "name": "ListModelCards",
+            "output": {
+                "shape": "ListModelCardsResponse"
+            }
+        },
         "ListModelExplainabilityJobDefinitions": {
             "documentation": "<p>Lists model explainability job definitions that satisfy various filters.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -3315,14 +3580,50 @@
                 "shape": "ListModelsInput"
             },
             "name": "ListModels",
             "output": {
                 "shape": "ListModelsOutput"
             }
         },
+        "ListMonitoringAlertHistory": {
+            "errors": [
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListMonitoringAlertHistoryRequest"
+            },
+            "name": "ListMonitoringAlertHistory",
+            "output": {
+                "shape": "ListMonitoringAlertHistoryResponse"
+            }
+        },
+        "ListMonitoringAlerts": {
+            "errors": [
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListMonitoringAlertsRequest"
+            },
+            "name": "ListMonitoringAlerts",
+            "output": {
+                "shape": "ListMonitoringAlertsResponse"
+            }
+        },
         "ListMonitoringExecutions": {
             "documentation": "<p>Returns list of all monitoring job executions.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -3358,15 +3659,15 @@
             },
             "name": "ListNotebookInstanceLifecycleConfigs",
             "output": {
                 "shape": "ListNotebookInstanceLifecycleConfigsOutput"
             }
         },
         "ListNotebookInstances": {
-            "documentation": "<p>Returns a list of the SageMaker notebook instances in the requester's account in an Amazon Web Services Region. </p>",
+            "documentation": "<p>Returns a list of the Amazon SageMaker notebook instances in the requester's account in an Amazon Web Services Region. </p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListNotebookInstancesInput"
             },
@@ -3470,16 +3771,28 @@
                 "shape": "ListProjectsInput"
             },
             "name": "ListProjects",
             "output": {
                 "shape": "ListProjectsOutput"
             }
         },
+        "ListSpaces": {
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListSpacesRequest"
+            },
+            "name": "ListSpaces",
+            "output": {
+                "shape": "ListSpacesResponse"
+            }
+        },
         "ListStageDevices": {
-            "documentation": "<p>Lists devices allocated to the stage, containing detailed device information and deployment status.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListStageDevicesRequest"
             },
@@ -3518,15 +3831,15 @@
             },
             "name": "ListSubscribedWorkteams",
             "output": {
                 "shape": "ListSubscribedWorkteamsResponse"
             }
         },
         "ListTags": {
-            "documentation": "<p>Returns the tags for the specified SageMaker resource.</p>",
+            "documentation": "<p>Returns the tags for the specified Amazon SageMaker resource.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListTagsInput"
             },
@@ -3810,24 +4123,44 @@
             },
             "name": "SendPipelineExecutionStepSuccess",
             "output": {
                 "shape": "SendPipelineExecutionStepSuccessResponse"
             }
         },
         "StartEdgeDeploymentStage": {
-            "documentation": "<p>Starts a stage in an edge deployment plan.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StartEdgeDeploymentStageRequest"
             },
             "name": "StartEdgeDeploymentStage"
         },
+        "StartInferenceExperiment": {
+            "errors": [
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "StartInferenceExperimentRequest"
+            },
+            "name": "StartInferenceExperiment",
+            "output": {
+                "shape": "StartInferenceExperimentResponse"
+            }
+        },
         "StartMonitoringSchedule": {
             "documentation": "<p>Starts a previously stopped monitoring schedule.</p> <note> <p>By default, when you successfully create a new schedule, the status of a monitoring schedule is <code>scheduled</code>.</p> </note>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
@@ -3837,15 +4170,15 @@
             },
             "input": {
                 "shape": "StartMonitoringScheduleRequest"
             },
             "name": "StartMonitoringSchedule"
         },
         "StartNotebookInstance": {
-            "documentation": "<p>Launches an ML compute instance with the latest version of the libraries and attaches your ML storage volume. After configuring the notebook instance, SageMaker sets the notebook instance status to <code>InService</code>. A notebook instance's status must be <code>InService</code> before you can connect to your Jupyter notebook. </p>",
+            "documentation": "<p>Launches an ML compute instance with the latest version of the libraries and attaches your ML storage volume. After configuring the notebook instance, Amazon SageMaker sets the notebook instance status to <code>InService</code>. A notebook instance's status must be <code>InService</code> before you can connect to your Jupyter notebook. </p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -3907,15 +4240,14 @@
             },
             "input": {
                 "shape": "StopCompilationJobRequest"
             },
             "name": "StopCompilationJob"
         },
         "StopEdgeDeploymentStage": {
-            "documentation": "<p>Stops a stage in an edge deployment plan.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StopEdgeDeploymentStageRequest"
             },
@@ -3944,14 +4276,35 @@
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StopHyperParameterTuningJobRequest"
             },
             "name": "StopHyperParameterTuningJob"
         },
+        "StopInferenceExperiment": {
+            "errors": [
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "StopInferenceExperimentRequest"
+            },
+            "name": "StopInferenceExperiment",
+            "output": {
+                "shape": "StopInferenceExperimentResponse"
+            }
+        },
         "StopInferenceRecommendationsJob": {
             "documentation": "<p>Stops an Inference Recommender job.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
@@ -3993,15 +4346,15 @@
             },
             "input": {
                 "shape": "StopMonitoringScheduleRequest"
             },
             "name": "StopMonitoringSchedule"
         },
         "StopNotebookInstance": {
-            "documentation": "<p>Terminates the ML compute instance. Before terminating the instance, SageMaker disconnects the ML storage volume from it. SageMaker preserves the ML storage volume. SageMaker stops charging you for the ML compute instance when you call <code>StopNotebookInstance</code>.</p> <p>To access data on the ML storage volume for a notebook instance that has been terminated, call the <code>StartNotebookInstance</code> API. <code>StartNotebookInstance</code> launches another ML compute instance, configures it, and attaches the preserved ML storage volume so you can continue your work. </p>",
+            "documentation": "<p>Terminates the ML compute instance. Before terminating the instance, Amazon SageMaker disconnects the ML storage volume from it. Amazon SageMaker preserves the ML storage volume. Amazon SageMaker stops charging you for the ML compute instance when you call <code>StopNotebookInstance</code>.</p> <p>To access data on the ML storage volume for a notebook instance that has been terminated, call the <code>StartNotebookInstance</code> API. <code>StartNotebookInstance</code> launches another ML compute instance, configures it, and attaches the preserved ML storage volume so you can continue your work. </p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StopNotebookInstanceInput"
             },
@@ -4039,15 +4392,15 @@
             },
             "input": {
                 "shape": "StopProcessingJobRequest"
             },
             "name": "StopProcessingJob"
         },
         "StopTrainingJob": {
-            "documentation": "<p>Stops a training job. To stop a job, SageMaker sends the algorithm the <code>SIGTERM</code> signal, which delays job termination for 120 seconds. Algorithms might use this 120-second window to save the model artifacts, so the results of the training is not lost. </p> <p>When it receives a <code>StopTrainingJob</code> request, SageMaker changes the status of the job to <code>Stopping</code>. After SageMaker stops the job, it sets the status to <code>Stopped</code>.</p>",
+            "documentation": "<p>Stops a training job. To stop a job, Amazon SageMaker sends the algorithm the <code>SIGTERM</code> signal, which delays job termination for 120 seconds. Algorithms might use this 120-second window to save the model artifacts, so the results of the training is not lost. </p> <p>When it receives a <code>StopTrainingJob</code> request, Amazon SageMaker changes the status of the job to <code>Stopping</code>. After Amazon SageMaker stops the job, it sets the status to <code>Stopped</code>.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4222,15 +4575,15 @@
             },
             "name": "UpdateDomain",
             "output": {
                 "shape": "UpdateDomainResponse"
             }
         },
         "UpdateEndpoint": {
-            "documentation": "<p>Deploys the new <code>EndpointConfig</code> specified in the request, switches to using newly created endpoint, and then deletes resources provisioned for the endpoint using the previous <code>EndpointConfig</code> (there is no availability loss). </p> <p>When SageMaker receives the request, it sets the endpoint status to <code>Updating</code>. After updating the endpoint, it sets the status to <code>InService</code>. To check the status of an endpoint, use the <a>DescribeEndpoint</a> API. </p> <note> <p>You must not delete an <code>EndpointConfig</code> in use by an endpoint that is live or while the <code>UpdateEndpoint</code> or <code>CreateEndpoint</code> operations are being performed on the endpoint. To update an endpoint, you must create a new <code>EndpointConfig</code>.</p> <p>If you delete the <code>EndpointConfig</code> of an endpoint that is active or being created or updated you may lose visibility into the instance type the endpoint is using. The endpoint must be deleted in order to stop incurring charges.</p> </note>",
+            "documentation": "<p>Deploys the new <code>EndpointConfig</code> specified in the request, switches to using newly created endpoint, and then deletes resources provisioned for the endpoint using the previous <code>EndpointConfig</code> (there is no availability loss). </p> <p>When Amazon SageMaker receives the request, it sets the endpoint status to <code>Updating</code>. After updating the endpoint, it sets the status to <code>InService</code>. To check the status of an endpoint, use the <a>DescribeEndpoint</a> API. </p> <note> <p>You must not delete an <code>EndpointConfig</code> in use by an endpoint that is live or while the <code>UpdateEndpoint</code> or <code>CreateEndpoint</code> operations are being performed on the endpoint. To update an endpoint, you must create a new <code>EndpointConfig</code>.</p> <p>If you delete the <code>EndpointConfig</code> of an endpoint that is active or being created or updated you may lose visibility into the instance type the endpoint is using. The endpoint must be deleted in order to stop incurring charges.</p> </note>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4241,15 +4594,15 @@
             },
             "name": "UpdateEndpoint",
             "output": {
                 "shape": "UpdateEndpointOutput"
             }
         },
         "UpdateEndpointWeightsAndCapacities": {
-            "documentation": "<p>Updates variant weight of one or more variants associated with an existing endpoint, or capacity of one variant associated with an existing endpoint. When it receives the request, SageMaker sets the endpoint status to <code>Updating</code>. After updating the endpoint, it sets the status to <code>InService</code>. To check the status of an endpoint, use the <a>DescribeEndpoint</a> API. </p>",
+            "documentation": "<p>Updates variant weight of one or more variants associated with an existing endpoint, or capacity of one variant associated with an existing endpoint. When it receives the request, Amazon SageMaker sets the endpoint status to <code>Updating</code>. After updating the endpoint, it sets the status to <code>InService</code>. To check the status of an endpoint, use the <a>DescribeEndpoint</a> API. </p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4282,15 +4635,14 @@
             },
             "name": "UpdateExperiment",
             "output": {
                 "shape": "UpdateExperimentResponse"
             }
         },
         "UpdateFeatureGroup": {
-            "documentation": "<p>Updates the feature group.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4301,15 +4653,14 @@
             },
             "name": "UpdateFeatureGroup",
             "output": {
                 "shape": "UpdateFeatureGroupResponse"
             }
         },
         "UpdateFeatureMetadata": {
-            "documentation": "<p>Updates the description and parameters of the feature group.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4338,28 +4689,94 @@
                 "shape": "UpdateImageRequest"
             },
             "name": "UpdateImage",
             "output": {
                 "shape": "UpdateImageResponse"
             }
         },
+        "UpdateInferenceExperiment": {
+            "errors": [
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "UpdateInferenceExperimentRequest"
+            },
+            "name": "UpdateInferenceExperiment",
+            "output": {
+                "shape": "UpdateInferenceExperimentResponse"
+            }
+        },
+        "UpdateModelCard": {
+            "errors": [
+                {
+                    "shape": "ResourceNotFound"
+                },
+                {
+                    "shape": "ResourceLimitExceeded"
+                },
+                {
+                    "shape": "ConflictException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "UpdateModelCardRequest"
+            },
+            "name": "UpdateModelCard",
+            "output": {
+                "shape": "UpdateModelCardResponse"
+            }
+        },
         "UpdateModelPackage": {
             "documentation": "<p>Updates a versioned model.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "UpdateModelPackageInput"
             },
             "name": "UpdateModelPackage",
             "output": {
                 "shape": "UpdateModelPackageOutput"
             }
         },
+        "UpdateMonitoringAlert": {
+            "errors": [
+                {
+                    "shape": "ResourceLimitExceeded"
+                },
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "UpdateMonitoringAlertRequest"
+            },
+            "name": "UpdateMonitoringAlert",
+            "output": {
+                "shape": "UpdateMonitoringAlertResponse"
+            }
+        },
         "UpdateMonitoringSchedule": {
             "documentation": "<p>Updates a previously created schedule.</p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 },
                 {
@@ -4464,16 +4881,40 @@
                 "shape": "UpdateProjectInput"
             },
             "name": "UpdateProject",
             "output": {
                 "shape": "UpdateProjectOutput"
             }
         },
+        "UpdateSpace": {
+            "errors": [
+                {
+                    "shape": "ResourceLimitExceeded"
+                },
+                {
+                    "shape": "ResourceInUse"
+                },
+                {
+                    "shape": "ResourceNotFound"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "UpdateSpaceRequest"
+            },
+            "name": "UpdateSpace",
+            "output": {
+                "shape": "UpdateSpaceResponse"
+            }
+        },
         "UpdateTrainingJob": {
-            "documentation": "<p>Update a model training job to request a new Debugger profiling configuration or to change warm pool retention length.</p>",
+            "documentation": "<p>Update a model training job to request a new Debugger profiling configuration.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4553,15 +4994,15 @@
             },
             "name": "UpdateUserProfile",
             "output": {
                 "shape": "UpdateUserProfileResponse"
             }
         },
         "UpdateWorkforce": {
-            "documentation": "<p>Use this operation to update your workforce. You can use this operation to require that workers use specific IP addresses to work on tasks and to update your OpenID Connect (OIDC) Identity Provider (IdP) workforce configuration.</p> <p>The worker portal is now supported in VPC and public internet.</p> <p> Use <code>SourceIpConfig</code> to restrict worker access to tasks to a specific range of IP addresses. You specify allowed IP addresses by creating a list of up to ten <a href=\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html\">CIDRs</a>. By default, a workforce isn't restricted to specific IP addresses. If you specify a range of IP addresses, workers who attempt to access tasks using any IP address outside the specified range are denied and get a <code>Not Found</code> error message on the worker portal.</p> <p>To restrict access to all the workers in public internet, add the <code>SourceIpConfig</code> CIDR value as \"0.0.0.0/0\".</p> <important> <p>Amazon SageMaker does not support Source Ip restriction for worker portals in VPC.</p> </important> <p>Use <code>OidcConfig</code> to update the configuration of a workforce created using your own OIDC IdP. </p> <important> <p>You can only update your OIDC IdP configuration when there are no work teams associated with your workforce. You can delete work teams using the operation.</p> </important> <p>After restricting access to a range of IP addresses or updating your OIDC IdP configuration with this operation, you can view details about your update workforce using the operation.</p> <important> <p>This operation only applies to private workforces.</p> </important>",
+            "documentation": "<p>Use this operation to update your workforce. You can use this operation to require that workers use specific IP addresses to work on tasks and to update your OpenID Connect (OIDC) Identity Provider (IdP) workforce configuration.</p> <p> Use <code>SourceIpConfig</code> to restrict worker access to tasks to a specific range of IP addresses. You specify allowed IP addresses by creating a list of up to ten <a href=\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html\">CIDRs</a>. By default, a workforce isn't restricted to specific IP addresses. If you specify a range of IP addresses, workers who attempt to access tasks using any IP address outside the specified range are denied and get a <code>Not Found</code> error message on the worker portal.</p> <p>Use <code>OidcConfig</code> to update the configuration of a workforce created using your own OIDC IdP. </p> <important> <p>You can only update your OIDC IdP configuration when there are no work teams associated with your workforce. You can delete work teams using the operation.</p> </important> <p>After restricting access to a range of IP addresses or updating your OIDC IdP configuration with this operation, you can view details about your update workforce using the operation.</p> <important> <p>This operation only applies to private workforces.</p> </important>",
             "errors": [
                 {
                     "shape": "ConflictException"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4732,15 +5173,15 @@
                 "Tags"
             ],
             "type": "structure"
         },
         "AddTagsOutput": {
             "members": {
                 "Tags": {
-                    "documentation": "<p>A list of tags associated with the SageMaker resource.</p>",
+                    "documentation": "<p>A list of tags associated with the Amazon SageMaker resource.</p>",
                     "shape": "TagList"
                 }
             },
             "type": "structure"
         },
         "AdditionalCodeRepositoryNamesOrUrls": {
             "max": 3,
@@ -4858,38 +5299,36 @@
             "enum": [
                 "Name",
                 "CreationTime"
             ],
             "type": "string"
         },
         "AlgorithmSpecification": {
-            "documentation": "<p>Specifies the training algorithm to use in a <a>CreateTrainingJob</a> request.</p> <p>For more information about algorithms provided by SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. For information about using your own algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>. </p>",
+            "documentation": "<p>Specifies the training algorithm to use in a <a>CreateTrainingJob</a> request.</p> <p>For more information about algorithms provided by Amazon SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. For information about using your own algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>. </p>",
             "members": {
                 "AlgorithmName": {
-                    "documentation": "<p>The name of the algorithm resource to use for the training job. This must be an algorithm resource that you created or subscribe to on Amazon Web Services Marketplace.</p> <note> <p>You must specify either the algorithm name to the <code>AlgorithmName</code> parameter or the image URI of the algorithm container to the <code>TrainingImage</code> parameter.</p> <p>Note that the <code>AlgorithmName</code> parameter is mutually exclusive with the <code>TrainingImage</code> parameter. If you specify a value for the <code>AlgorithmName</code> parameter, you can't specify a value for <code>TrainingImage</code>, and vice versa.</p> <p>If you specify values for both parameters, the training job might break; if you don't specify any value for both parameters, the training job might raise a <code>null</code> error.</p> </note>",
+                    "documentation": "<p>The name of the algorithm resource to use for the training job. This must be an algorithm resource that you created or subscribe to on Amazon Web Services Marketplace. If you specify a value for this parameter, you can't specify a value for <code>TrainingImage</code>.</p>",
                     "shape": "ArnOrName"
                 },
                 "ContainerArguments": {
-                    "documentation": "<p>The arguments for a container used to run a training job. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms-training-algo-dockerfile.html\">How Amazon SageMaker Runs Your Training Image</a> for additional information.</p>",
                     "shape": "TrainingContainerArguments"
                 },
                 "ContainerEntrypoint": {
-                    "documentation": "<p>The <a href=\"https://docs.docker.com/engine/reference/builder/\">entrypoint script for a Docker container</a> used to run a training job. This script takes precedence over the default train processing instructions. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms-training-algo-dockerfile.html\">How Amazon SageMaker Runs Your Training Image</a> for more information.</p>",
                     "shape": "TrainingContainerEntrypoint"
                 },
                 "EnableSageMakerMetricsTimeSeries": {
-                    "documentation": "<p>To generate and save time-series metrics during training, set to <code>true</code>. The default is <code>false</code> and time-series metrics aren't generated except in the following cases:</p> <ul> <li> <p>You use one of the SageMaker built-in algorithms</p> </li> <li> <p>You use one of the following <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/pre-built-containers-frameworks-deep-learning.html\">Prebuilt SageMaker Docker Images</a>:</p> <ul> <li> <p>Tensorflow (version &gt;= 1.15)</p> </li> <li> <p>MXNet (version &gt;= 1.6)</p> </li> <li> <p>PyTorch (version &gt;= 1.3)</p> </li> </ul> </li> <li> <p>You specify at least one <a>MetricDefinition</a> </p> </li> </ul>",
+                    "documentation": "<p>To generate and save time-series metrics during training, set to <code>true</code>. The default is <code>false</code> and time-series metrics aren't generated except in the following cases:</p> <ul> <li> <p>You use one of the Amazon SageMaker built-in algorithms</p> </li> <li> <p>You use one of the following <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/pre-built-containers-frameworks-deep-learning.html\">Prebuilt Amazon SageMaker Docker Images</a>:</p> <ul> <li> <p>Tensorflow (version &gt;= 1.15)</p> </li> <li> <p>MXNet (version &gt;= 1.6)</p> </li> <li> <p>PyTorch (version &gt;= 1.3)</p> </li> </ul> </li> <li> <p>You specify at least one <a>MetricDefinition</a> </p> </li> </ul>",
                     "shape": "Boolean"
                 },
                 "MetricDefinitions": {
-                    "documentation": "<p>A list of metric definition objects. Each object specifies the metric name and regular expressions used to parse algorithm logs. SageMaker publishes each metric to Amazon CloudWatch.</p>",
+                    "documentation": "<p>A list of metric definition objects. Each object specifies the metric name and regular expressions used to parse algorithm logs. Amazon SageMaker publishes each metric to Amazon CloudWatch.</p>",
                     "shape": "MetricDefinitionList"
                 },
                 "TrainingImage": {
-                    "documentation": "<p>The registry path of the Docker image that contains the training algorithm. For information about docker registry paths for SageMaker built-in algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-algo-docker-registry-paths.html\">Docker Registry Paths and Example Code</a> in the <i>Amazon SageMaker developer guide</i>. SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information about using your custom training container, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>.</p> <note> <p>You must specify either the algorithm name to the <code>AlgorithmName</code> parameter or the image URI of the algorithm container to the <code>TrainingImage</code> parameter.</p> <p>For more information, see the note in the <code>AlgorithmName</code> parameter description.</p> </note>",
+                    "documentation": "<p>The registry path of the Docker image that contains the training algorithm. For information about docker registry paths for built-in algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-algo-docker-registry-paths.html\">Algorithms Provided by Amazon SageMaker: Common Parameters</a>. Amazon SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>.</p>",
                     "shape": "AlgorithmImage"
                 },
                 "TrainingInputMode": {
                     "shape": "TrainingInputMode"
                 }
             },
             "required": [
@@ -4984,26 +5423,26 @@
         "AlgorithmSummaryList": {
             "member": {
                 "shape": "AlgorithmSummary"
             },
             "type": "list"
         },
         "AlgorithmValidationProfile": {
-            "documentation": "<p>Defines a training job and a batch transform job that SageMaker runs to validate your algorithm.</p> <p>The data provided in the validation profile is made available to your buyers on Amazon Web Services Marketplace.</p>",
+            "documentation": "<p>Defines a training job and a batch transform job that Amazon SageMaker runs to validate your algorithm.</p> <p>The data provided in the validation profile is made available to your buyers on Amazon Web Services Marketplace.</p>",
             "members": {
                 "ProfileName": {
                     "documentation": "<p>The name of the profile for the algorithm. The name must have 1 to 63 characters. Valid characters are a-z, A-Z, 0-9, and - (hyphen).</p>",
                     "shape": "EntityName"
                 },
                 "TrainingJobDefinition": {
-                    "documentation": "<p>The <code>TrainingJobDefinition</code> object that describes the training job that SageMaker runs to validate your algorithm.</p>",
+                    "documentation": "<p>The <code>TrainingJobDefinition</code> object that describes the training job that Amazon SageMaker runs to validate your algorithm.</p>",
                     "shape": "TrainingJobDefinition"
                 },
                 "TransformJobDefinition": {
-                    "documentation": "<p>The <code>TransformJobDefinition</code> object that describes the transform job that SageMaker runs to validate your algorithm.</p>",
+                    "documentation": "<p>The <code>TransformJobDefinition</code> object that describes the transform job that Amazon SageMaker runs to validate your algorithm.</p>",
                     "shape": "TransformJobDefinition"
                 }
             },
             "required": [
                 "ProfileName",
                 "TrainingJobDefinition"
             ],
@@ -5014,22 +5453,22 @@
             "member": {
                 "shape": "AlgorithmValidationProfile"
             },
             "min": 1,
             "type": "list"
         },
         "AlgorithmValidationSpecification": {
-            "documentation": "<p>Specifies configurations for one or more training jobs that SageMaker runs to test the algorithm.</p>",
+            "documentation": "<p>Specifies configurations for one or more training jobs that Amazon SageMaker runs to test the algorithm.</p>",
             "members": {
                 "ValidationProfiles": {
-                    "documentation": "<p>An array of <code>AlgorithmValidationProfile</code> objects, each of which specifies a training job and batch transform job that SageMaker runs to validate your algorithm.</p>",
+                    "documentation": "<p>An array of <code>AlgorithmValidationProfile</code> objects, each of which specifies a training job and batch transform job that Amazon SageMaker runs to validate your algorithm.</p>",
                     "shape": "AlgorithmValidationProfiles"
                 },
                 "ValidationRole": {
-                    "documentation": "<p>The IAM roles that SageMaker uses to run the training jobs.</p>",
+                    "documentation": "<p>The IAM roles that Amazon SageMaker uses to run the training jobs.</p>",
                     "shape": "RoleArn"
                 }
             },
             "required": [
                 "ValidationRole",
                 "ValidationProfiles"
             ],
@@ -5068,14 +5507,17 @@
                     "documentation": "<p>The creation time.</p>",
                     "shape": "CreationTime"
                 },
                 "DomainId": {
                     "documentation": "<p>The domain ID.</p>",
                     "shape": "DomainId"
                 },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                },
                 "Status": {
                     "documentation": "<p>The status.</p>",
                     "shape": "AppStatus"
                 },
                 "UserProfileName": {
                     "documentation": "<p>The user profile name.</p>",
                     "shape": "UserProfileName"
@@ -5471,28 +5913,28 @@
                     "documentation": "<p>The source type.</p>",
                     "shape": "String256"
                 }
             },
             "type": "structure"
         },
         "AsyncInferenceClientConfig": {
-            "documentation": "<p>Configures the behavior of the client used by SageMaker to interact with the model container during asynchronous inference.</p>",
+            "documentation": "<p>Configures the behavior of the client used by Amazon SageMaker to interact with the model container during asynchronous inference.</p>",
             "members": {
                 "MaxConcurrentInvocationsPerInstance": {
-                    "documentation": "<p>The maximum number of concurrent requests sent by the SageMaker client to the model container. If no value is provided, SageMaker chooses an optimal value.</p>",
+                    "documentation": "<p>The maximum number of concurrent requests sent by the SageMaker client to the model container. If no value is provided, Amazon SageMaker will choose an optimal value for you.</p>",
                     "shape": "MaxConcurrentInvocationsPerInstance"
                 }
             },
             "type": "structure"
         },
         "AsyncInferenceConfig": {
             "documentation": "<p>Specifies configuration for how an endpoint performs asynchronous inference.</p>",
             "members": {
                 "ClientConfig": {
-                    "documentation": "<p>Configures the behavior of the client used by SageMaker to interact with the model container during asynchronous inference.</p>",
+                    "documentation": "<p>Configures the behavior of the client used by Amazon SageMaker to interact with the model container during asynchronous inference.</p>",
                     "shape": "AsyncInferenceClientConfig"
                 },
                 "OutputConfig": {
                     "documentation": "<p>Specifies the configuration for asynchronous inference invocation outputs.</p>",
                     "shape": "AsyncInferenceOutputConfig"
                 }
             },
@@ -5515,15 +5957,15 @@
             },
             "type": "structure"
         },
         "AsyncInferenceOutputConfig": {
             "documentation": "<p>Specifies the configuration for asynchronous inference invocation outputs.</p>",
             "members": {
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that SageMaker uses to encrypt the asynchronous inference output in Amazon S3.</p> <p/>",
+                    "documentation": "<p>The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that Amazon SageMaker uses to encrypt the asynchronous inference output in Amazon S3.</p> <p/>",
                     "shape": "KmsKeyId"
                 },
                 "NotificationConfig": {
                     "documentation": "<p>Specifies the configuration for notifications of inference results for asynchronous inference.</p>",
                     "shape": "AsyncInferenceNotificationConfig"
                 },
                 "S3OutputPath": {
@@ -5700,18 +6142,16 @@
                 "CandidateStatus",
                 "CreationTime",
                 "LastModifiedTime"
             ],
             "type": "structure"
         },
         "AutoMLCandidateGenerationConfig": {
-            "documentation": "<p>Stores the config information for how a candidate is generated (optional).</p>",
             "members": {
                 "FeatureSpecificationS3Uri": {
-                    "documentation": "<p>A URL to the Amazon S3 data source containing selected features from the input data source to run an Autopilot job. You can input <code>FeatureAttributeNames</code> (optional) in JSON format as shown below: </p> <p> <code>{ \"FeatureAttributeNames\":[\"col1\", \"col2\", ...] }</code>.</p> <p>You can also specify the data type of the feature (optional) in the format shown below:</p> <p> <code>{ \"FeatureDataTypes\":{\"col1\":\"numeric\", \"col2\":\"categorical\" ... } }</code> </p> <note> <p>These column keys may not include the target column.</p> </note> <p>In ensembling mode, Autopilot will only support the following data types: <code>numeric</code>, <code>categorical</code>, <code>text</code> and <code>datetime</code>. In HPO mode, Autopilot can support <code>numeric</code>, <code>categorical</code>, <code>text</code>, <code>datetime</code> and <code>sequence</code>.</p> <p>If only <code>FeatureDataTypes</code> is provided, the column keys (<code>col1</code>, <code>col2</code>,..) should be a subset of the column names in the input data. </p> <p>If both <code>FeatureDataTypes</code> and <code>FeatureAttributeNames</code> are provided, then the column keys should be a subset of the column names provided in <code>FeatureAttributeNames</code>. </p> <p>The key name <code>FeatureAttributeNames</code> is fixed. The values listed in <code>[\"col1\", \"col2\", ...]</code> is case sensitive and should be a list of strings containing unique values that are a subset of the column names in the input data. The list of columns provided must not include the target column.</p>",
                     "shape": "S3Uri"
                 }
             },
             "type": "structure"
         },
         "AutoMLCandidateStep": {
             "documentation": "<p>Information about the steps for a candidate and what step it is working on.</p>",
@@ -5739,18 +6179,17 @@
         "AutoMLCandidates": {
             "member": {
                 "shape": "AutoMLCandidate"
             },
             "type": "list"
         },
         "AutoMLChannel": {
-            "documentation": "<p>A channel is a named input source that training algorithms can consume. The validation dataset size is limited to less than 2 GB. The training dataset size must be less than 100 GB. For more information, see .</p> <note> <p>A validation dataset must contain the same headers as the training dataset.</p> </note> <p/>",
+            "documentation": "<p>A channel is a named input source that training algorithms can consume. For more information, see .</p>",
             "members": {
                 "ChannelType": {
-                    "documentation": "<p>The channel type (optional) is an <code>enum</code> string. The default value is <code>training</code>. Channels for training and validation must share the same <code>ContentType</code> and <code>TargetAttributeName</code>. For information on specifying training and validation channel types, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-datasets-problem-types.html#autopilot-data-sources-training-or-validation\"> <code>How to specify training and validation datasets</code> </a>.</p>",
                     "shape": "AutoMLChannelType"
                 },
                 "CompressionType": {
                     "documentation": "<p>You can use <code>Gzip</code> or <code>None</code>. The default value is <code>None</code>.</p>",
                     "shape": "CompressionType"
                 },
                 "ContentType": {
@@ -5808,28 +6247,26 @@
             },
             "type": "list"
         },
         "AutoMLDataSource": {
             "documentation": "<p>The data source for the Autopilot job.</p>",
             "members": {
                 "S3DataSource": {
-                    "documentation": "<p>The Amazon S3 location of the input data.</p>",
+                    "documentation": "<p>The Amazon S3 location of the input data.</p> <note> <p>The input data must be in CSV format and contain at least 500 rows.</p> </note>",
                     "shape": "AutoMLS3DataSource"
                 }
             },
             "required": [
                 "S3DataSource"
             ],
             "type": "structure"
         },
         "AutoMLDataSplitConfig": {
-            "documentation": "<p>This structure specifies how to split the data into train and validation datasets. The validation and training datasets must contain the same headers. The validation dataset must be less than 2 GB in size.</p>",
             "members": {
                 "ValidationFraction": {
-                    "documentation": "<p>The validation fraction (optional) is a float that specifies the portion of the training dataset to be used for validation. The default value is 0.2, and values must be greater than 0 and less than 1. We recommend setting this value to be less than 0.5.</p>",
                     "shape": "ValidationFraction"
                 }
             },
             "type": "structure"
         },
         "AutoMLFailureReason": {
             "max": 1024,
@@ -5871,37 +6308,34 @@
                     "shape": "MaxAutoMLJobRuntimeInSeconds"
                 },
                 "MaxCandidates": {
                     "documentation": "<p>The maximum number of times a training job is allowed to run.</p>",
                     "shape": "MaxCandidates"
                 },
                 "MaxRuntimePerTrainingJobInSeconds": {
-                    "documentation": "<p>The maximum time, in seconds, that each training job executed inside hyperparameter tuning is allowed to run as part of a hyperparameter tuning job. For more information, see the used by the action.</p>",
+                    "documentation": "<p>The maximum time, in seconds, that each training job is allowed to run as part of a hyperparameter tuning job. For more information, see the used by the action.</p>",
                     "shape": "MaxRuntimePerTrainingJobInSeconds"
                 }
             },
             "type": "structure"
         },
         "AutoMLJobConfig": {
             "documentation": "<p>A collection of settings used for an AutoML job.</p>",
             "members": {
                 "CandidateGenerationConfig": {
-                    "documentation": "<p>The configuration for generating a candidate for an AutoML job (optional). </p>",
                     "shape": "AutoMLCandidateGenerationConfig"
                 },
                 "CompletionCriteria": {
                     "documentation": "<p>How long an AutoML job is allowed to run, or how many candidates a job is allowed to generate.</p>",
                     "shape": "AutoMLJobCompletionCriteria"
                 },
                 "DataSplitConfig": {
-                    "documentation": "<p>The configuration for splitting the input training dataset.</p> <p>Type: AutoMLDataSplitConfig</p>",
                     "shape": "AutoMLDataSplitConfig"
                 },
                 "Mode": {
-                    "documentation": "<p>The method that Autopilot uses to train the data. You can either specify the mode manually or let Autopilot choose for you based on the dataset size by selecting <code>AUTO</code>. In <code>AUTO</code> mode, Autopilot chooses <code>ENSEMBLING</code> for datasets smaller than 100 MB, and <code>HYPERPARAMETER_TUNING</code> for larger ones.</p> <p>The <code>ENSEMBLING</code> mode uses a multi-stack ensemble model to predict classification and regression tasks directly from your dataset. This machine learning mode combines several base models to produce an optimal predictive model. It then uses a stacking ensemble method to combine predictions from contributing members. A multi-stack ensemble model can provide better performance over a single model by combining the predictive capabilities of multiple models. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-suppprt\">Autopilot algorithm support</a> for a list of algorithms supported by <code>ENSEMBLING</code> mode.</p> <p>The <code>HYPERPARAMETER_TUNING</code> (HPO) mode uses the best hyperparameters to train the best version of a model. HPO will automatically select an algorithm for the type of problem you want to solve. Then HPO finds the best hyperparameters according to your objective metric. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-suppprt\">Autopilot algorithm support</a> for a list of algorithms supported by <code>HYPERPARAMETER_TUNING</code> mode.</p>",
                     "shape": "AutoMLMode"
                 },
                 "SecurityConfig": {
                     "documentation": "<p>The security configuration for traffic encryption or Amazon VPC settings.</p>",
                     "shape": "AutoMLSecurityConfig"
                 }
             },
@@ -5961,14 +6395,22 @@
                 "InProgress",
                 "Failed",
                 "Stopped",
                 "Stopping"
             ],
             "type": "string"
         },
+        "AutoMLJobStepMetadata": {
+            "members": {
+                "Arn": {
+                    "shape": "AutoMLJobArn"
+                }
+            },
+            "type": "structure"
+        },
         "AutoMLJobSummaries": {
             "member": {
                 "shape": "AutoMLJobSummary"
             },
             "type": "list"
         },
         "AutoMLJobSummary": {
@@ -6104,15 +6546,15 @@
             "min": 1,
             "type": "list"
         },
         "AutoMLS3DataSource": {
             "documentation": "<p>The Amazon S3 data source.</p>",
             "members": {
                 "S3DataType": {
-                    "documentation": "<p>The data type.</p> <p>A ManifestFile should have the format shown below:</p> <p> <code>[ {\"prefix\": \"s3://DOC-EXAMPLE-BUCKET/DOC-EXAMPLE-FOLDER/DOC-EXAMPLE-PREFIX/\"}, </code> </p> <p> <code>\"DOC-EXAMPLE-RELATIVE-PATH/DOC-EXAMPLE-FOLDER/DATA-1\",</code> </p> <p> <code>\"DOC-EXAMPLE-RELATIVE-PATH/DOC-EXAMPLE-FOLDER/DATA-2\",</code> </p> <p> <code>... \"DOC-EXAMPLE-RELATIVE-PATH/DOC-EXAMPLE-FOLDER/DATA-N\" ]</code> </p> <p>An S3Prefix should have the following format: </p> <p> <code>s3://DOC-EXAMPLE-BUCKET/DOC-EXAMPLE-FOLDER-OR-FILE</code> </p>",
+                    "documentation": "<p>The data type.</p>",
                     "shape": "AutoMLS3DataType"
                 },
                 "S3Uri": {
                     "documentation": "<p>The URL to the Amazon S3 data source.</p>",
                     "shape": "S3Uri"
                 }
             },
@@ -6176,26 +6618,22 @@
             "enum": [
                 "AWS/Rekognition/DetectModerationLabels/Image/V3",
                 "AWS/Textract/AnalyzeDocument/Forms/V1"
             ],
             "type": "string"
         },
         "BatchDataCaptureConfig": {
-            "documentation": "<p>Configuration to control how SageMaker captures inference data for batch transform jobs.</p>",
             "members": {
                 "DestinationS3Uri": {
-                    "documentation": "<p>The Amazon S3 location being used to capture the data.</p>",
                     "shape": "S3Uri"
                 },
                 "GenerateInferenceId": {
-                    "documentation": "<p>Flag that indicates whether to append inference id to the output.</p>",
                     "shape": "Boolean"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of a Amazon Web Services Key Management Service key that SageMaker uses to encrypt data on the storage volume attached to the ML compute instance that hosts the batch transform job.</p> <p>The KmsKeyId can be any of the following formats: </p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias name ARN: <code>arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul>",
                     "shape": "KmsKeyId"
                 }
             },
             "required": [
                 "DestinationS3Uri"
             ],
             "type": "structure"
@@ -6300,77 +6738,63 @@
             "enum": [
                 "MultiRecord",
                 "SingleRecord"
             ],
             "type": "string"
         },
         "BatchTransformInput": {
-            "documentation": "<p>Input object for the batch transform job.</p>",
             "members": {
                 "DataCapturedDestinationS3Uri": {
-                    "documentation": "<p>The Amazon S3 location being used to capture the data.</p>",
                     "shape": "DestinationS3Uri"
                 },
                 "DatasetFormat": {
-                    "documentation": "<p>The dataset format for your batch transform job.</p>",
                     "shape": "MonitoringDatasetFormat"
                 },
                 "EndTimeOffset": {
-                    "documentation": "<p>If specified, monitoring jobs substract this time from the end time. For information about using offsets for scheduling monitoring jobs, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-monitor-model-quality-schedule.html\">Schedule Model Quality Monitoring Jobs</a>.</p>",
                     "shape": "MonitoringTimeOffsetString"
                 },
                 "FeaturesAttribute": {
-                    "documentation": "<p>The attributes of the input data that are the input features.</p>",
                     "shape": "String"
                 },
                 "InferenceAttribute": {
-                    "documentation": "<p>The attribute of the input data that represents the ground truth label.</p>",
                     "shape": "String"
                 },
                 "LocalPath": {
-                    "documentation": "<p>Path to the filesystem where the batch transform data is available to the container.</p>",
                     "shape": "ProcessingLocalPath"
                 },
                 "ProbabilityAttribute": {
-                    "documentation": "<p>In a classification problem, the attribute that represents the class probability.</p>",
                     "shape": "String"
                 },
                 "ProbabilityThresholdAttribute": {
-                    "documentation": "<p>The threshold for the class probability to be evaluated as a positive result.</p>",
                     "shape": "ProbabilityThresholdAttribute"
                 },
                 "S3DataDistributionType": {
-                    "documentation": "<p>Whether input data distributed in Amazon S3 is fully replicated or sharded by an S3 key. Defaults to <code>FullyReplicated</code> </p>",
                     "shape": "ProcessingS3DataDistributionType"
                 },
                 "S3InputMode": {
-                    "documentation": "<p>Whether the <code>Pipe</code> or <code>File</code> is used as the input mode for transferring data for the monitoring job. <code>Pipe</code> mode is recommended for large datasets. <code>File</code> mode is useful for small files that fit in memory. Defaults to <code>File</code>.</p>",
                     "shape": "ProcessingS3InputMode"
                 },
                 "StartTimeOffset": {
-                    "documentation": "<p>If specified, monitoring jobs substract this time from the start time. For information about using offsets for scheduling monitoring jobs, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-monitor-model-quality-schedule.html\">Schedule Model Quality Monitoring Jobs</a>.</p>",
                     "shape": "MonitoringTimeOffsetString"
                 }
             },
             "required": [
                 "DataCapturedDestinationS3Uri",
                 "DatasetFormat",
                 "LocalPath"
             ],
             "type": "structure"
         },
         "Bias": {
             "documentation": "<p>Contains bias metrics for a model.</p>",
             "members": {
                 "PostTrainingReport": {
-                    "documentation": "<p>The post-training bias report for a model.</p>",
                     "shape": "MetricsSource"
                 },
                 "PreTrainingReport": {
-                    "documentation": "<p>The pre-training bias report for a model.</p>",
                     "shape": "MetricsSource"
                 },
                 "Report": {
                     "documentation": "<p>The bias report for a model</p>",
                     "shape": "MetricsSource"
                 }
             },
@@ -6465,15 +6889,14 @@
             "documentation": "<p>The location of artifacts for an AutoML candidate job.</p>",
             "members": {
                 "Explainability": {
                     "documentation": "<p>The Amazon S3 prefix to the explainability artifacts generated for the AutoML candidate.</p>",
                     "shape": "ExplainabilityLocation"
                 },
                 "ModelInsights": {
-                    "documentation": "<p>The Amazon S3 prefix to the model insight artifacts generated for the AutoML candidate.</p>",
                     "shape": "ModelInsightsLocation"
                 }
             },
             "required": [
                 "Explainability"
             ],
             "type": "structure"
@@ -6541,18 +6964,16 @@
         "CandidateSteps": {
             "member": {
                 "shape": "AutoMLCandidateStep"
             },
             "type": "list"
         },
         "CanvasAppSettings": {
-            "documentation": "<p>The SageMaker Canvas app settings.</p>",
             "members": {
                 "TimeSeriesForecastingSettings": {
-                    "documentation": "<p>Time series forecast settings for the Canvas app.</p>",
                     "shape": "TimeSeriesForecastingSettings"
                 }
             },
             "type": "structure"
         },
         "CapacitySize": {
             "documentation": "<p>Specifies the endpoint capacity to activate for production.</p>",
@@ -6580,39 +7001,39 @@
             "type": "string"
         },
         "CapacitySizeValue": {
             "min": 1,
             "type": "integer"
         },
         "CaptureContentTypeHeader": {
-            "documentation": "<p>Configuration specifying how to treat different headers. If no headers are specified SageMaker will by default base64 encode when capturing the data.</p>",
+            "documentation": "<p/>",
             "members": {
                 "CsvContentTypes": {
-                    "documentation": "<p>The list of all content type headers that SageMaker will treat as CSV and capture accordingly.</p>",
+                    "documentation": "<p/>",
                     "shape": "CsvContentTypes"
                 },
                 "JsonContentTypes": {
-                    "documentation": "<p>The list of all content type headers that SageMaker will treat as JSON and capture accordingly.</p>",
+                    "documentation": "<p/>",
                     "shape": "JsonContentTypes"
                 }
             },
             "type": "structure"
         },
         "CaptureMode": {
             "enum": [
                 "Input",
                 "Output"
             ],
             "type": "string"
         },
         "CaptureOption": {
-            "documentation": "<p>Specifies data Model Monitor will capture.</p>",
+            "documentation": "<p/>",
             "members": {
                 "CaptureMode": {
-                    "documentation": "<p>Specify the boundary of data to capture.</p>",
+                    "documentation": "<p/>",
                     "shape": "CaptureMode"
                 }
             },
             "required": [
                 "CaptureMode"
             ],
             "type": "structure"
@@ -6735,19 +7156,19 @@
                     "shape": "ContentType"
                 },
                 "DataSource": {
                     "documentation": "<p>The location of the channel data.</p>",
                     "shape": "DataSource"
                 },
                 "InputMode": {
-                    "documentation": "<p>(Optional) The input mode to use for the data channel in a training job. If you don't set a value for <code>InputMode</code>, SageMaker uses the value set for <code>TrainingInputMode</code>. Use this parameter to override the <code>TrainingInputMode</code> setting in a <a>AlgorithmSpecification</a> request when you have a channel that needs a different input mode from the training job's general setting. To download the data from Amazon Simple Storage Service (Amazon S3) to the provisioned ML storage volume, and mount the directory to a Docker volume, use <code>File</code> input mode. To stream data directly from Amazon S3 to the container, choose <code>Pipe</code> input mode.</p> <p>To use a model for incremental training, choose <code>File</code> input model.</p>",
+                    "documentation": "<p>(Optional) The input mode to use for the data channel in a training job. If you don't set a value for <code>InputMode</code>, Amazon SageMaker uses the value set for <code>TrainingInputMode</code>. Use this parameter to override the <code>TrainingInputMode</code> setting in a <a>AlgorithmSpecification</a> request when you have a channel that needs a different input mode from the training job's general setting. To download the data from Amazon Simple Storage Service (Amazon S3) to the provisioned ML storage volume, and mount the directory to a Docker volume, use <code>File</code> input mode. To stream data directly from Amazon S3 to the container, choose <code>Pipe</code> input mode.</p> <p>To use a model for incremental training, choose <code>File</code> input model.</p>",
                     "shape": "TrainingInputMode"
                 },
                 "RecordWrapperType": {
-                    "documentation": "<p/> <p>Specify RecordIO as the value when input data is in raw format but the training algorithm requires the RecordIO format. In this case, SageMaker wraps each individual S3 object in a RecordIO record. If the input data is already in RecordIO format, you don't need to set this attribute. For more information, see <a href=\"https://mxnet.apache.org/api/architecture/note_data_loading#data-format\">Create a Dataset Using RecordIO</a>. </p> <p>In File mode, leave this field unset or set it to None.</p>",
+                    "documentation": "<p/> <p>Specify RecordIO as the value when input data is in raw format but the training algorithm requires the RecordIO format. In this case, Amazon SageMaker wraps each individual S3 object in a RecordIO record. If the input data is already in RecordIO format, you don't need to set this attribute. For more information, see <a href=\"https://mxnet.apache.org/api/architecture/note_data_loading#data-format\">Create a Dataset Using RecordIO</a>. </p> <p>In File mode, leave this field unset or set it to None.</p>",
                     "shape": "RecordWrapper"
                 },
                 "ShuffleConfig": {
                     "documentation": "<p>A configuration for a shuffle option for input data in a channel. If you use <code>S3Prefix</code> for <code>S3DataType</code>, this shuffles the results of the S3 key prefix matches. If you use <code>ManifestFile</code>, the order of the S3 object references in the <code>ManifestFile</code> is shuffled. If you use <code>AugmentedManifestFile</code>, the order of the JSON lines in the <code>AugmentedManifestFile</code> is shuffled. The shuffling order is determined using the <code>Seed</code> value.</p> <p>For Pipe input mode, shuffling is done at the start of every epoch. With large datasets this ensures that the order of the training data is different for each epoch, it helps reduce bias and possible overfitting. In a multi-node training job when ShuffleConfig is combined with <code>S3DataDistributionType</code> of <code>ShardedByS3Key</code>, the data is shuffled across nodes so that the content sent to a particular node on the first epoch might be sent to a different node on the second epoch.</p>",
                     "shape": "ShuffleConfig"
                 }
             },
@@ -6810,15 +7231,15 @@
             "documentation": "<p>Contains information about the output location for managed spot training checkpoint data. </p>",
             "members": {
                 "LocalPath": {
                     "documentation": "<p>(Optional) The local directory where checkpoints are written. The default directory is <code>/opt/ml/checkpoints/</code>. </p>",
                     "shape": "DirectoryPath"
                 },
                 "S3Uri": {
-                    "documentation": "<p>Identifies the S3 path where you want SageMaker to store checkpoints. For example, <code>s3://bucket-name/key-name-prefix</code>.</p>",
+                    "documentation": "<p>Identifies the S3 path where you want Amazon SageMaker to store checkpoints. For example, <code>s3://bucket-name/key-name-prefix</code>.</p>",
                     "shape": "S3Uri"
                 }
             },
             "required": [
                 "S3Uri"
             ],
             "type": "structure"
@@ -6882,26 +7303,22 @@
         "ClarifyEnableExplanations": {
             "max": 64,
             "min": 1,
             "pattern": ".*",
             "type": "string"
         },
         "ClarifyExplainerConfig": {
-            "documentation": "<p>The configuration parameters for the SageMaker Clarify explainer.</p>",
             "members": {
                 "EnableExplanations": {
-                    "documentation": "<p>A JMESPath boolean expression used to filter which records to explain. Explanations are activated by default. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-online-explainability-create-endpoint.html#clarify-online-explainability-create-endpoint-enable\"> <code>EnableExplanations</code> </a>for additional information.</p>",
                     "shape": "ClarifyEnableExplanations"
                 },
                 "InferenceConfig": {
-                    "documentation": "<p>The inference configuration parameter for the model container.</p>",
                     "shape": "ClarifyInferenceConfig"
                 },
                 "ShapConfig": {
-                    "documentation": "<p>The configuration for SHAP analysis.</p>",
                     "shape": "ClarifyShapConfig"
                 }
             },
             "required": [
                 "ShapConfig"
             ],
             "type": "structure"
@@ -6939,58 +7356,46 @@
         "ClarifyHeader": {
             "max": 64,
             "min": 1,
             "pattern": ".*",
             "type": "string"
         },
         "ClarifyInferenceConfig": {
-            "documentation": "<p>The inference configuration parameter for the model container.</p>",
             "members": {
                 "ContentTemplate": {
-                    "documentation": "<p>A template string used to format a JSON record into an acceptable model container input. For example, a <code>ContentTemplate</code> string <code>'{\"myfeatures\":$features}'</code> will format a list of features <code>[1,2,3]</code> into the record string <code>'{\"myfeatures\":[1,2,3]}'</code>. Required only when the model container input is in JSON Lines format.</p>",
                     "shape": "ClarifyContentTemplate"
                 },
                 "FeatureHeaders": {
-                    "documentation": "<p>The names of the features. If provided, these are included in the endpoint response payload to help readability of the <code>InvokeEndpoint</code> output. See the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-online-explainability-invoke-endpoint.html#clarify-online-explainability-response\">Response</a> section under <b>Invoke the endpoint</b> in the Developer Guide for more information.</p>",
                     "shape": "ClarifyFeatureHeaders"
                 },
                 "FeatureTypes": {
-                    "documentation": "<p>A list of data types of the features (optional). Applicable only to NLP explainability. If provided, <code>FeatureTypes</code> must have at least one <code>'text'</code> string (for example, <code>['text']</code>). If <code>FeatureTypes</code> is not provided, the explainer infers the feature types based on the baseline data. The feature types are included in the endpoint response payload. For additional information see the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-online-explainability-invoke-endpoint.html#clarify-online-explainability-response\">response</a> section under <b>Invoke the endpoint</b> in the Developer Guide for more information.</p>",
                     "shape": "ClarifyFeatureTypes"
                 },
                 "FeaturesAttribute": {
-                    "documentation": "<p>Provides the JMESPath expression to extract the features from a model container input in JSON Lines format. For example, if <code>FeaturesAttribute</code> is the JMESPath expression <code>'myfeatures'</code>, it extracts a list of features <code>[1,2,3]</code> from request data <code>'{\"myfeatures\":[1,2,3]}'</code>.</p>",
                     "shape": "ClarifyFeaturesAttribute"
                 },
                 "LabelAttribute": {
-                    "documentation": "<p>A JMESPath expression used to locate the list of label headers in the model container output.</p> <p> <b>Example</b>: If the model container output of a batch request is <code>'{\"labels\":[\"cat\",\"dog\",\"fish\"],\"probability\":[0.6,0.3,0.1]}'</code>, then set <code>LabelAttribute</code> to <code>'labels'</code> to extract the list of label headers <code>[\"cat\",\"dog\",\"fish\"]</code> </p>",
                     "shape": "ClarifyLabelAttribute"
                 },
                 "LabelHeaders": {
-                    "documentation": "<p>For multiclass classification problems, the label headers are the names of the classes. Otherwise, the label header is the name of the predicted label. These are used to help readability for the output of the <code>InvokeEndpoint</code> API. See the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-online-explainability-invoke-endpoint.html#clarify-online-explainability-response\">response</a> section under <b>Invoke the endpoint</b> in the Developer Guide for more information. If there are no label headers in the model container output, provide them manually using this parameter.</p>",
                     "shape": "ClarifyLabelHeaders"
                 },
                 "LabelIndex": {
-                    "documentation": "<p>A zero-based index used to extract a label header or list of label headers from model container output in CSV format.</p> <p> <b>Example for a multiclass model:</b> If the model container output consists of label headers followed by probabilities: <code>'\"[\\'cat\\',\\'dog\\',\\'fish\\']\",\"[0.1,0.6,0.3]\"'</code>, set <code>LabelIndex</code> to <code>0</code> to select the label headers <code>['cat','dog','fish']</code>.</p>",
                     "shape": "ClarifyLabelIndex"
                 },
                 "MaxPayloadInMB": {
-                    "documentation": "<p>The maximum payload size (MB) allowed of a request from the explainer to the model container. Defaults to <code>6</code> MB.</p>",
                     "shape": "ClarifyMaxPayloadInMB"
                 },
                 "MaxRecordCount": {
-                    "documentation": "<p>The maximum number of records in a request that the model container can process when querying the model container for the predictions of a <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-online-explainability-create-endpoint.html#clarify-online-explainability-create-endpoint-synthetic\">synthetic dataset</a>. A record is a unit of input data that inference can be made on, for example, a single line in CSV data. If <code>MaxRecordCount</code> is <code>1</code>, the model container expects one record per request. A value of 2 or greater means that the model expects batch requests, which can reduce overhead and speed up the inferencing process. If this parameter is not provided, the explainer will tune the record count per request according to the model container's capacity at runtime.</p>",
                     "shape": "ClarifyMaxRecordCount"
                 },
                 "ProbabilityAttribute": {
-                    "documentation": "<p>A JMESPath expression used to extract the probability (or score) from the model container output if the model container is in JSON Lines format.</p> <p> <b>Example</b>: If the model container output of a single request is <code>'{\"predicted_label\":1,\"probability\":0.6}'</code>, then set <code>ProbabilityAttribute</code> to <code>'probability'</code>.</p>",
                     "shape": "ClarifyProbabilityAttribute"
                 },
                 "ProbabilityIndex": {
-                    "documentation": "<p>A zero-based index used to extract a probability value (score) or list from model container output in CSV format. If this value is not provided, the entire model container output will be treated as a probability value (score) or list.</p> <p> <b>Example for a single class model:</b> If the model container output consists of a string-formatted prediction label followed by its probability: <code>'1,0.6'</code>, set <code>ProbabilityIndex</code> to <code>1</code> to select the probability value <code>0.6</code>.</p> <p> <b>Example for a multiclass model:</b> If the model container output consists of a string-formatted prediction label followed by its probability: <code>'\"[\\'cat\\',\\'dog\\',\\'fish\\']\",\"[0.1,0.6,0.3]\"'</code>, set <code>ProbabilityIndex</code> to <code>1</code> to select the probability values <code>[0.1,0.6,0.3]</code>.</p>",
                     "shape": "ClarifyProbabilityIndex"
                 }
             },
             "type": "structure"
         },
         "ClarifyLabelAttribute": {
             "max": 64,
@@ -7037,52 +7442,42 @@
         "ClarifyShapBaseline": {
             "max": 4096,
             "min": 1,
             "pattern": "[\\s\\S]+",
             "type": "string"
         },
         "ClarifyShapBaselineConfig": {
-            "documentation": "<p>The configuration for the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-feature-attribute-shap-baselines.html\">SHAP baseline</a> (also called the background or reference dataset) of the Kernal SHAP algorithm.</p> <note> <ul> <li> <p>The number of records in the baseline data determines the size of the synthetic dataset, which has an impact on latency of explainability requests. For more information, see the <b>Synthetic data</b> of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-online-explainability-create-endpoint.html\">Configure and create an endpoint</a>.</p> </li> <li> <p> <code>ShapBaseline</code> and <code>ShapBaselineUri</code> are mutually exclusive parameters. One or the either is required to configure a SHAP baseline. </p> </li> </ul> </note>",
             "members": {
                 "MimeType": {
-                    "documentation": "<p>The MIME type of the baseline data. Choose from <code>'text/csv'</code> or <code>'application/jsonlines'</code>. Defaults to <code>'text/csv'</code>.</p>",
                     "shape": "ClarifyMimeType"
                 },
                 "ShapBaseline": {
-                    "documentation": "<p>The inline SHAP baseline data in string format. <code>ShapBaseline</code> can have one or multiple records to be used as the baseline dataset. The format of the SHAP baseline file should be the same format as the training dataset. For example, if the training dataset is in CSV format and each record contains four features, and all features are numerical, then the format of the baseline data should also share these characteristics. For natural language processing (NLP) of text columns, the baseline value should be the value used to replace the unit of text specified by the <code>Granularity</code> of the <code>TextConfig</code> parameter. The size limit for <code>ShapBasline</code> is 4 KB. Use the <code>ShapBaselineUri</code> parameter if you want to provide more than 4 KB of baseline data.</p>",
                     "shape": "ClarifyShapBaseline"
                 },
                 "ShapBaselineUri": {
-                    "documentation": "<p>The uniform resource identifier (URI) of the S3 bucket where the SHAP baseline file is stored. The format of the SHAP baseline file should be the same format as the format of the training dataset. For example, if the training dataset is in CSV format, and each record in the training dataset has four features, and all features are numerical, then the baseline file should also have this same format. Each record should contain only the features. If you are using a virtual private cloud (VPC), the <code>ShapBaselineUri</code> should be accessible to the VPC. For more information about setting up endpoints with Amazon Virtual Private Cloud, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/infrastructure-give-access.html\">Give SageMaker access to Resources in your Amazon Virtual Private Cloud</a>.</p>",
                     "shape": "Url"
                 }
             },
             "type": "structure"
         },
         "ClarifyShapConfig": {
-            "documentation": "<p>The configuration for SHAP analysis using SageMaker Clarify Explainer.</p>",
             "members": {
                 "NumberOfSamples": {
-                    "documentation": "<p>The number of samples to be used for analysis by the Kernal SHAP algorithm. </p> <note> <p>The number of samples determines the size of the synthetic dataset, which has an impact on latency of explainability requests. For more information, see the <b>Synthetic data</b> of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-online-explainability-create-endpoint.html\">Configure and create an endpoint</a>.</p> </note>",
                     "shape": "ClarifyShapNumberOfSamples"
                 },
                 "Seed": {
-                    "documentation": "<p>The starting value used to initialize the random number generator in the explainer. Provide a value for this parameter to obtain a deterministic SHAP result.</p>",
                     "shape": "ClarifyShapSeed"
                 },
                 "ShapBaselineConfig": {
-                    "documentation": "<p>The configuration for the SHAP baseline of the Kernal SHAP algorithm.</p>",
                     "shape": "ClarifyShapBaselineConfig"
                 },
                 "TextConfig": {
-                    "documentation": "<p>A parameter that indicates if text features are treated as text and explanations are provided for individual units of text. Required for natural language processing (NLP) explainability only.</p>",
                     "shape": "ClarifyTextConfig"
                 },
                 "UseLogit": {
-                    "documentation": "<p>A Boolean toggle to indicate if you want to use the logit function (true) or log-odds units (false) for model predictions. Defaults to false.</p>",
                     "shape": "ClarifyShapUseLogit"
                 }
             },
             "required": [
                 "ShapBaselineConfig"
             ],
             "type": "structure"
@@ -7094,22 +7489,19 @@
         "ClarifyShapSeed": {
             "type": "integer"
         },
         "ClarifyShapUseLogit": {
             "type": "boolean"
         },
         "ClarifyTextConfig": {
-            "documentation": "<p>A parameter used to configure the SageMaker Clarify explainer to treat text features as text so that explanations are provided for individual units of text. Required only for natural language processing (NLP) explainability. </p>",
             "members": {
                 "Granularity": {
-                    "documentation": "<p>The unit of granularity for the analysis of text features. For example, if the unit is <code>'token'</code>, then each token (like a word in English) of the text is treated as a feature. SHAP values are computed for each unit/feature.</p>",
                     "shape": "ClarifyTextGranularity"
                 },
                 "Language": {
-                    "documentation": "<p>Specifies the language of the text features in <a href=\" https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes\">ISO 639-1</a> or <a href=\"https://en.wikipedia.org/wiki/ISO_639-3\">ISO 639-3</a> code of a supported language. </p> <note> <p>For a mix of multiple languages, use code <code>'xx'</code>.</p> </note>",
                     "shape": "ClarifyTextLanguage"
                 }
             },
             "required": [
                 "Language",
                 "Granularity"
             ],
@@ -7203,14 +7595,32 @@
         },
         "ClientToken": {
             "max": 36,
             "min": 1,
             "pattern": "^[a-zA-Z0-9-]+$",
             "type": "string"
         },
+        "CodeRepositories": {
+            "max": 10,
+            "member": {
+                "shape": "CodeRepository"
+            },
+            "type": "list"
+        },
+        "CodeRepository": {
+            "members": {
+                "RepositoryUrl": {
+                    "shape": "RepositoryUrl"
+                }
+            },
+            "required": [
+                "RepositoryUrl"
+            ],
+            "type": "structure"
+        },
         "CodeRepositoryArn": {
             "max": 2048,
             "min": 1,
             "pattern": "arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:code-repository/.*",
             "type": "string"
         },
         "CodeRepositoryContains": {
@@ -7530,15 +7940,15 @@
                     "shape": "ContainerHostname"
                 },
                 "Environment": {
                     "documentation": "<p>The environment variables to set in the Docker container. Each key and value in the <code>Environment</code> string to string map can have length of up to 1024. We support up to 16 entries in the map. </p>",
                     "shape": "EnvironmentMap"
                 },
                 "Image": {
-                    "documentation": "<p>The path where inference code is stored. This can be either in Amazon EC2 Container Registry or in a Docker registry that is accessible from the same VPC that you configure for your endpoint. If you are using your own custom algorithm instead of an algorithm provided by SageMaker, the inference code must meet SageMaker requirements. SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a> </p>",
+                    "documentation": "<p>The path where inference code is stored. This can be either in Amazon EC2 Container Registry or in a Docker registry that is accessible from the same VPC that you configure for your endpoint. If you are using your own custom algorithm instead of an algorithm provided by Amazon SageMaker, the inference code must meet Amazon SageMaker requirements. Amazon SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a> </p>",
                     "shape": "ContainerImage"
                 },
                 "ImageConfig": {
                     "documentation": "<p>Specifies whether the model container is in Amazon ECR or a private Docker registry accessible from your Amazon Virtual Private Cloud (VPC). For information about storing containers in a private Docker registry, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms-containers-inference-private.html\">Use a Private Docker Registry for Real-Time Inference Containers</a> </p>",
                     "shape": "ImageConfig"
                 },
                 "InferenceSpecificationName": {
@@ -7546,15 +7956,15 @@
                     "shape": "InferenceSpecificationName"
                 },
                 "Mode": {
                     "documentation": "<p>Whether the container hosts a single model or multiple models.</p>",
                     "shape": "ContainerMode"
                 },
                 "ModelDataUrl": {
-                    "documentation": "<p>The S3 path where the model artifacts, which result from model training, are stored. This path must point to a single gzip compressed tar archive (.tar.gz suffix). The S3 path is required for SageMaker built-in algorithms, but not if you use your own algorithms. For more information on built-in algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-algo-docker-registry-paths.html\">Common Parameters</a>. </p> <note> <p>The model artifacts must be in an S3 bucket that is in the same region as the model or endpoint you are creating.</p> </note> <p>If you provide a value for this parameter, SageMaker uses Amazon Web Services Security Token Service to download model artifacts from the S3 path you provide. Amazon Web Services STS is activated in your IAM user account by default. If you previously deactivated Amazon Web Services STS for a region, you need to reactivate Amazon Web Services STS for that region. For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_enable-regions.html\">Activating and Deactivating Amazon Web Services STS in an Amazon Web Services Region</a> in the <i>Amazon Web Services Identity and Access Management User Guide</i>.</p> <important> <p>If you use a built-in algorithm to create a model, SageMaker requires that you provide a S3 path to the model artifacts in <code>ModelDataUrl</code>.</p> </important>",
+                    "documentation": "<p>The S3 path where the model artifacts, which result from model training, are stored. This path must point to a single gzip compressed tar archive (.tar.gz suffix). The S3 path is required for Amazon SageMaker built-in algorithms, but not if you use your own algorithms. For more information on built-in algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-algo-docker-registry-paths.html\">Common Parameters</a>. </p> <note> <p>The model artifacts must be in an S3 bucket that is in the same region as the model or endpoint you are creating.</p> </note> <p>If you provide a value for this parameter, Amazon SageMaker uses Amazon Web Services Security Token Service to download model artifacts from the S3 path you provide. Amazon Web Services STS is activated in your IAM user account by default. If you previously deactivated Amazon Web Services STS for a region, you need to reactivate Amazon Web Services STS for that region. For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_enable-regions.html\">Activating and Deactivating Amazon Web Services STS in an Amazon Web Services Region</a> in the <i>Amazon Web Services Identity and Access Management User Guide</i>.</p> <important> <p>If you use a built-in algorithm to create a model, Amazon SageMaker requires that you provide a S3 path to the model artifacts in <code>ModelDataUrl</code>.</p> </important>",
                     "shape": "Url"
                 },
                 "ModelPackageName": {
                     "documentation": "<p>The name or Amazon Resource Name (ARN) of the model package to use to create the model.</p>",
                     "shape": "VersionedArnOrName"
                 },
                 "MultiModelConfig": {
@@ -7705,15 +8115,15 @@
                     "shape": "ParameterValue"
                 },
                 "Name": {
                     "documentation": "<p>The name of the continuous hyperparameter to tune.</p>",
                     "shape": "ParameterKey"
                 },
                 "ScalingType": {
-                    "documentation": "<p>The scale that hyperparameter tuning uses to search the hyperparameter range. For information about choosing a hyperparameter scale, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-define-ranges.html#scaling-type\">Hyperparameter Scaling</a>. One of the following values:</p> <dl> <dt>Auto</dt> <dd> <p>SageMaker hyperparameter tuning chooses the best scale for the hyperparameter.</p> </dd> <dt>Linear</dt> <dd> <p>Hyperparameter tuning searches the values in the hyperparameter range by using a linear scale.</p> </dd> <dt>Logarithmic</dt> <dd> <p>Hyperparameter tuning searches the values in the hyperparameter range by using a logarithmic scale.</p> <p>Logarithmic scaling works only for ranges that have only values greater than 0.</p> </dd> <dt>ReverseLogarithmic</dt> <dd> <p>Hyperparameter tuning searches the values in the hyperparameter range by using a reverse logarithmic scale.</p> <p>Reverse logarithmic scaling works only for ranges that are entirely within the range 0&lt;=x&lt;1.0.</p> </dd> </dl>",
+                    "documentation": "<p>The scale that hyperparameter tuning uses to search the hyperparameter range. For information about choosing a hyperparameter scale, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-define-ranges.html#scaling-type\">Hyperparameter Scaling</a>. One of the following values:</p> <dl> <dt>Auto</dt> <dd> <p>Amazon SageMaker hyperparameter tuning chooses the best scale for the hyperparameter.</p> </dd> <dt>Linear</dt> <dd> <p>Hyperparameter tuning searches the values in the hyperparameter range by using a linear scale.</p> </dd> <dt>Logarithmic</dt> <dd> <p>Hyperparameter tuning searches the values in the hyperparameter range by using a logarithmic scale.</p> <p>Logarithmic scaling works only for ranges that have only values greater than 0.</p> </dd> <dt>ReverseLogarithmic</dt> <dd> <p>Hyperparameter tuning searches the values in the hyperparameter range by using a reverse logarithmic scale.</p> <p>Reverse logarithmic scaling works only for ranges that are entirely within the range 0&lt;=x&lt;1.0.</p> </dd> </dl>",
                     "shape": "HyperParameterScalingType"
                 }
             },
             "required": [
                 "Name",
                 "MinValue",
                 "MaxValue"
@@ -7819,15 +8229,15 @@
                     "shape": "TagList"
                 },
                 "TrainingSpecification": {
                     "documentation": "<p>Specifies details about training jobs run by this algorithm, including the following:</p> <ul> <li> <p>The Amazon ECR path of the container and the version digest of the algorithm.</p> </li> <li> <p>The hyperparameters that the algorithm supports.</p> </li> <li> <p>The instance types that the algorithm supports for training.</p> </li> <li> <p>Whether the algorithm supports distributed training.</p> </li> <li> <p>The metrics that the algorithm emits to Amazon CloudWatch.</p> </li> <li> <p>Which metrics that the algorithm emits can be used as the objective metric for hyperparameter tuning jobs.</p> </li> <li> <p>The input channels that the algorithm supports for training data. For example, an algorithm might support <code>train</code>, <code>validation</code>, and <code>test</code> channels.</p> </li> </ul>",
                     "shape": "TrainingSpecification"
                 },
                 "ValidationSpecification": {
-                    "documentation": "<p>Specifies configurations for one or more training jobs and that SageMaker runs to test the algorithm's training code and, optionally, one or more batch transform jobs that SageMaker runs to test the algorithm's inference code.</p>",
+                    "documentation": "<p>Specifies configurations for one or more training jobs and that Amazon SageMaker runs to test the algorithm's training code and, optionally, one or more batch transform jobs that Amazon SageMaker runs to test the algorithm's inference code.</p>",
                     "shape": "AlgorithmValidationSpecification"
                 }
             },
             "required": [
                 "AlgorithmName",
                 "TrainingSpecification"
             ],
@@ -7848,15 +8258,15 @@
         "CreateAppImageConfigRequest": {
             "members": {
                 "AppImageConfigName": {
                     "documentation": "<p>The name of the AppImageConfig. Must be unique to your account.</p>",
                     "shape": "AppImageConfigName"
                 },
                 "KernelGatewayImageConfig": {
-                    "documentation": "<p>The KernelGatewayImageConfig. You can only specify one image kernel in the AppImageConfig API. This kernel will be shown to users before the image starts. Once the image runs, all kernels are visible in JupyterLab.</p>",
+                    "documentation": "<p>The KernelGatewayImageConfig.</p>",
                     "shape": "KernelGatewayImageConfig"
                 },
                 "Tags": {
                     "documentation": "<p>A list of tags to apply to the AppImageConfig.</p>",
                     "shape": "TagList"
                 }
             },
@@ -7877,37 +8287,39 @@
         "CreateAppRequest": {
             "members": {
                 "AppName": {
                     "documentation": "<p>The name of the app.</p>",
                     "shape": "AppName"
                 },
                 "AppType": {
-                    "documentation": "<p>The type of app.</p>",
+                    "documentation": "<p>The type of app. Supported apps are <code>JupyterServer</code> and <code>KernelGateway</code>. <code>TensorBoard</code> is not supported.</p>",
                     "shape": "AppType"
                 },
                 "DomainId": {
                     "documentation": "<p>The domain ID.</p>",
                     "shape": "DomainId"
                 },
                 "ResourceSpec": {
-                    "documentation": "<p>The instance type and the Amazon Resource Name (ARN) of the SageMaker image created on the instance.</p> <note> <p>The value of <code>InstanceType</code> passed as part of the <code>ResourceSpec</code> in the <code>CreateApp</code> call overrides the value passed as part of the <code>ResourceSpec</code> configured for the user profile or the domain. If <code>InstanceType</code> is not specified in any of those three <code>ResourceSpec</code> values for a <code>KernelGateway</code> app, the <code>CreateApp</code> call fails with a request validation error.</p> </note>",
+                    "documentation": "<p>The instance type and the Amazon Resource Name (ARN) of the SageMaker image created on the instance.</p>",
                     "shape": "ResourceSpec"
                 },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                },
                 "Tags": {
                     "documentation": "<p>Each tag consists of a key and an optional value. Tag keys must be unique per resource.</p>",
                     "shape": "TagList"
                 },
                 "UserProfileName": {
                     "documentation": "<p>The user profile name.</p>",
                     "shape": "UserProfileName"
                 }
             },
             "required": [
                 "DomainId",
-                "UserProfileName",
                 "AppType",
                 "AppName"
             ],
             "type": "structure"
         },
         "CreateAppResponse": {
             "members": {
@@ -7958,15 +8370,15 @@
                 }
             },
             "type": "structure"
         },
         "CreateAutoMLJobRequest": {
             "members": {
                 "AutoMLJobConfig": {
-                    "documentation": "<p>A collection of settings used to configure an AutoML job.</p>",
+                    "documentation": "<p>Contains <code>CompletionCriteria</code> and <code>SecurityConfig</code> settings for the AutoML job.</p>",
                     "shape": "AutoMLJobConfig"
                 },
                 "AutoMLJobName": {
                     "documentation": "<p>Identifies an Autopilot job. The name must be unique to your account and is case-insensitive.</p>",
                     "shape": "AutoMLJobName"
                 },
                 "AutoMLJobObjective": {
@@ -7974,27 +8386,27 @@
                     "shape": "AutoMLJobObjective"
                 },
                 "GenerateCandidateDefinitionsOnly": {
                     "documentation": "<p>Generates possible candidates without training the models. A candidate is a combination of data preprocessors, algorithms, and algorithm parameter settings.</p>",
                     "shape": "GenerateCandidateDefinitionsOnly"
                 },
                 "InputDataConfig": {
-                    "documentation": "<p>An array of channel objects that describes the input data and its location. Each channel is a named input source. Similar to <code>InputDataConfig</code> supported by . Format(s) supported: CSV, Parquet. A minimum of 500 rows is required for the training dataset. There is not a minimum number of rows required for the validation dataset.</p>",
+                    "documentation": "<p>An array of channel objects that describes the input data and its location. Each channel is a named input source. Similar to <code>InputDataConfig</code> supported by . Format(s) supported: CSV. Minimum of 500 rows.</p>",
                     "shape": "AutoMLInputDataConfig"
                 },
                 "ModelDeployConfig": {
                     "documentation": "<p>Specifies how to generate the endpoint name for an automatic one-click Autopilot model deployment.</p>",
                     "shape": "ModelDeployConfig"
                 },
                 "OutputDataConfig": {
                     "documentation": "<p>Provides information about encryption and the Amazon S3 output path needed to store artifacts from an AutoML job. Format(s) supported: CSV.</p>",
                     "shape": "AutoMLOutputDataConfig"
                 },
                 "ProblemType": {
-                    "documentation": "<p>Defines the type of supervised learning available for the candidates. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-automate-model-development-problem-types.html\"> Amazon SageMaker Autopilot problem types and algorithm support</a>.</p>",
+                    "documentation": "<p>Defines the type of supervised learning available for the candidates. Options include: <code>BinaryClassification</code>, <code>MulticlassClassification</code>, and <code>Regression</code>. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-automate-model-development-problem-types.html\"> Amazon SageMaker Autopilot problem types and algorithm support</a>.</p>",
                     "shape": "ProblemType"
                 },
                 "RoleArn": {
                     "documentation": "<p>The ARN of the role that is used to access the data.</p>",
                     "shape": "RoleArn"
                 },
                 "Tags": {
@@ -8258,14 +8670,17 @@
                     "documentation": "<p>The entity that creates and manages the required security groups for inter-app communication in <code>VPCOnly</code> mode. Required when <code>CreateDomain.AppNetworkAccessType</code> is <code>VPCOnly</code> and <code>DomainSettings.RStudioServerProDomainSettings.DomainExecutionRoleArn</code> is provided.</p>",
                     "shape": "AppSecurityGroupManagement"
                 },
                 "AuthMode": {
                     "documentation": "<p>The mode of authentication that members use to access the domain.</p>",
                     "shape": "AuthMode"
                 },
+                "DefaultSpaceSettings": {
+                    "shape": "DefaultSpaceSettings"
+                },
                 "DefaultUserSettings": {
                     "documentation": "<p>The default settings to use to create a user profile when <code>UserSettings</code> isn't specified in the call to the <code>CreateUserProfile</code> API.</p> <p> <code>SecurityGroups</code> is aggregated when specified in both calls. For all other settings in <code>UserSettings</code>, the values specified in <code>CreateUserProfile</code> take precedence over those specified in <code>CreateDomain</code>.</p>",
                     "shape": "UserSettings"
                 },
                 "DomainName": {
                     "documentation": "<p>A name for the domain.</p>",
                     "shape": "DomainName"
@@ -8318,61 +8733,53 @@
                 }
             },
             "type": "structure"
         },
         "CreateEdgeDeploymentPlanRequest": {
             "members": {
                 "DeviceFleetName": {
-                    "documentation": "<p>The device fleet used for this edge deployment plan.</p>",
                     "shape": "EntityName"
                 },
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the edge deployment plan.</p>",
                     "shape": "EntityName"
                 },
                 "ModelConfigs": {
-                    "documentation": "<p>List of models associated with the edge deployment plan.</p>",
                     "shape": "EdgeDeploymentModelConfigs"
                 },
                 "Stages": {
-                    "documentation": "<p>List of stages of the edge deployment plan. The number of stages is limited to 10 per deployment.</p>",
                     "shape": "DeploymentStages"
                 },
                 "Tags": {
-                    "documentation": "<p>List of tags with which to tag the edge deployment plan.</p>",
                     "shape": "TagList"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanName",
                 "ModelConfigs",
                 "DeviceFleetName"
             ],
             "type": "structure"
         },
         "CreateEdgeDeploymentPlanResponse": {
             "members": {
                 "EdgeDeploymentPlanArn": {
-                    "documentation": "<p>The ARN of the edge deployment plan.</p>",
                     "shape": "EdgeDeploymentPlanArn"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanArn"
             ],
             "type": "structure"
         },
         "CreateEdgeDeploymentStageRequest": {
             "members": {
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the edge deployment plan.</p>",
                     "shape": "EntityName"
                 },
                 "Stages": {
-                    "documentation": "<p>List of stages to be added to the edge deployment plan.</p>",
                     "shape": "DeploymentStages"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanName",
                 "Stages"
             ],
@@ -8433,25 +8840,27 @@
                     "shape": "DataCaptureConfig"
                 },
                 "EndpointConfigName": {
                     "documentation": "<p>The name of the endpoint configuration. You specify this name in a <a>CreateEndpoint</a> request. </p>",
                     "shape": "EndpointConfigName"
                 },
                 "ExplainerConfig": {
-                    "documentation": "<p>A member of <code>CreateEndpointConfig</code> that enables explainers.</p>",
                     "shape": "ExplainerConfig"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of a Amazon Web Services Key Management Service key that SageMaker uses to encrypt data on the storage volume attached to the ML compute instance that hosts the endpoint.</p> <p>The KmsKeyId can be any of the following formats: </p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias name ARN: <code>arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>The KMS key policy must grant permission to the IAM role that you specify in your <code>CreateEndpoint</code>, <code>UpdateEndpoint</code> requests. For more information, refer to the Amazon Web Services Key Management Service section<a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html\"> Using Key Policies in Amazon Web Services KMS </a> </p> <note> <p>Certain Nitro-based instances include local storage, dependent on the instance type. Local storage volumes are encrypted using a hardware module on the instance. You can't request a <code>KmsKeyId</code> when using an instance type with local storage. If any of the models that you specify in the <code>ProductionVariants</code> parameter use nitro-based instances with local storage, do not specify a value for the <code>KmsKeyId</code> parameter. If you specify a value for <code>KmsKeyId</code> when using any nitro-based instances with local storage, the call to <code>CreateEndpointConfig</code> fails.</p> <p>For a list of instance types that support local instance storage, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html#instance-store-volumes\">Instance Store Volumes</a>.</p> <p>For more information about local instance storage encryption, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ssd-instance-store.html\">SSD Instance Store Volumes</a>.</p> </note>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of a Amazon Web Services Key Management Service key that Amazon SageMaker uses to encrypt data on the storage volume attached to the ML compute instance that hosts the endpoint.</p> <p>The KmsKeyId can be any of the following formats: </p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias name ARN: <code>arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>The KMS key policy must grant permission to the IAM role that you specify in your <code>CreateEndpoint</code>, <code>UpdateEndpoint</code> requests. For more information, refer to the Amazon Web Services Key Management Service section<a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html\"> Using Key Policies in Amazon Web Services KMS </a> </p> <note> <p>Certain Nitro-based instances include local storage, dependent on the instance type. Local storage volumes are encrypted using a hardware module on the instance. You can't request a <code>KmsKeyId</code> when using an instance type with local storage. If any of the models that you specify in the <code>ProductionVariants</code> parameter use nitro-based instances with local storage, do not specify a value for the <code>KmsKeyId</code> parameter. If you specify a value for <code>KmsKeyId</code> when using any nitro-based instances with local storage, the call to <code>CreateEndpointConfig</code> fails.</p> <p>For a list of instance types that support local instance storage, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html#instance-store-volumes\">Instance Store Volumes</a>.</p> <p>For more information about local instance storage encryption, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ssd-instance-store.html\">SSD Instance Store Volumes</a>.</p> </note>",
                     "shape": "KmsKeyId"
                 },
                 "ProductionVariants": {
                     "documentation": "<p>An list of <code>ProductionVariant</code> objects, one for each model that you want to host at this endpoint.</p>",
                     "shape": "ProductionVariantList"
                 },
+                "ShadowProductionVariants": {
+                    "shape": "ProductionVariantList"
+                },
                 "Tags": {
                     "documentation": "<p>An array of key-value pairs. You can use tags to categorize your Amazon Web Services resources in different ways, for example, by purpose, owner, or environment. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a>.</p>",
                     "shape": "TagList"
                 }
             },
             "required": [
                 "EndpointConfigName",
@@ -8714,15 +9123,15 @@
                 "HyperParameterTuningJobConfig"
             ],
             "type": "structure"
         },
         "CreateHyperParameterTuningJobResponse": {
             "members": {
                 "HyperParameterTuningJobArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the tuning job. SageMaker assigns an ARN to a hyperparameter tuning job when you create it.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the tuning job. Amazon SageMaker assigns an ARN to a hyperparameter tuning job when you create it.</p>",
                     "shape": "HyperParameterTuningJobArn"
                 }
             },
             "required": [
                 "HyperParameterTuningJobArn"
             ],
             "type": "structure"
@@ -8764,15 +9173,15 @@
                 }
             },
             "type": "structure"
         },
         "CreateImageVersionRequest": {
             "members": {
                 "BaseImage": {
-                    "documentation": "<p>The registry path of the container image to use as the starting point for this version. The path is an Amazon Elastic Container Registry (ECR) URI in the following format:</p> <p> <code>&lt;acct-id&gt;.dkr.ecr.&lt;region&gt;.amazonaws.com/&lt;repo-name[:tag] or [@digest]&gt;</code> </p>",
+                    "documentation": "<p>The registry path of the container image to use as the starting point for this version. The path is an Amazon Container Registry (ECR) URI in the following format:</p> <p> <code>&lt;acct-id&gt;.dkr.ecr.&lt;region&gt;.amazonaws.com/&lt;repo-name[:tag] or [@digest]&gt;</code> </p>",
                     "shape": "ImageBaseImage"
                 },
                 "ClientToken": {
                     "documentation": "<p>A unique ID. If not specified, the Amazon Web Services CLI and Amazon Web Services SDKs, such as the SDK for Python (Boto3), add a unique value to the call.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientToken"
                 },
@@ -8793,14 +9202,71 @@
                 "ImageVersionArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the image version.</p>",
                     "shape": "ImageVersionArn"
                 }
             },
             "type": "structure"
         },
+        "CreateInferenceExperimentRequest": {
+            "members": {
+                "DataStorageConfig": {
+                    "shape": "InferenceExperimentDataStorageConfig"
+                },
+                "Description": {
+                    "shape": "InferenceExperimentDescription"
+                },
+                "EndpointName": {
+                    "shape": "EndpointName"
+                },
+                "KmsKey": {
+                    "shape": "KmsKeyId"
+                },
+                "ModelVariants": {
+                    "shape": "ModelVariantConfigList"
+                },
+                "Name": {
+                    "shape": "InferenceExperimentName"
+                },
+                "RoleArn": {
+                    "shape": "RoleArn"
+                },
+                "Schedule": {
+                    "shape": "InferenceExperimentSchedule"
+                },
+                "ShadowModeConfig": {
+                    "shape": "ShadowModeConfig"
+                },
+                "Tags": {
+                    "shape": "TagList"
+                },
+                "Type": {
+                    "shape": "InferenceExperimentType"
+                }
+            },
+            "required": [
+                "Name",
+                "Type",
+                "RoleArn",
+                "EndpointName",
+                "ModelVariants",
+                "ShadowModeConfig"
+            ],
+            "type": "structure"
+        },
+        "CreateInferenceExperimentResponse": {
+            "members": {
+                "InferenceExperimentArn": {
+                    "shape": "InferenceExperimentArn"
+                }
+            },
+            "required": [
+                "InferenceExperimentArn"
+            ],
+            "type": "structure"
+        },
         "CreateInferenceRecommendationsJobRequest": {
             "members": {
                 "InputConfig": {
                     "documentation": "<p>Provides information about the versioned model package Amazon Resource Name (ARN), the traffic pattern, and endpoint configurations.</p>",
                     "shape": "RecommendationJobInputConfig"
                 },
                 "JobDescription": {
@@ -8812,15 +9278,14 @@
                     "shape": "RecommendationJobName"
                 },
                 "JobType": {
                     "documentation": "<p>Defines the type of recommendation job. Specify <code>Default</code> to initiate an instance recommendation and <code>Advanced</code> to initiate a load test. If left unspecified, Amazon SageMaker Inference Recommender will run an instance recommendation (<code>DEFAULT</code>) job.</p>",
                     "shape": "RecommendationJobType"
                 },
                 "OutputConfig": {
-                    "documentation": "<p>Provides information about the output artifacts and the KMS key to use for Amazon S3 server-side encryption.</p>",
                     "shape": "RecommendationJobOutputConfig"
                 },
                 "RoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of an IAM role that enables Amazon SageMaker to perform tasks on your behalf.</p>",
                     "shape": "RoleArn"
                 },
                 "StoppingConditions": {
@@ -8975,14 +9440,83 @@
                 }
             },
             "required": [
                 "JobDefinitionArn"
             ],
             "type": "structure"
         },
+        "CreateModelCardExportJobRequest": {
+            "members": {
+                "ModelCardExportJobName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardVersion": {
+                    "shape": "Integer"
+                },
+                "OutputConfig": {
+                    "shape": "ModelCardExportOutputConfig"
+                }
+            },
+            "required": [
+                "ModelCardName",
+                "ModelCardExportJobName",
+                "OutputConfig"
+            ],
+            "type": "structure"
+        },
+        "CreateModelCardExportJobResponse": {
+            "members": {
+                "ModelCardExportJobArn": {
+                    "shape": "ModelCardExportJobArn"
+                }
+            },
+            "required": [
+                "ModelCardExportJobArn"
+            ],
+            "type": "structure"
+        },
+        "CreateModelCardRequest": {
+            "members": {
+                "Content": {
+                    "shape": "ModelCardContent"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardStatus": {
+                    "shape": "ModelCardStatus"
+                },
+                "SecurityConfig": {
+                    "shape": "ModelCardSecurityConfig"
+                },
+                "Tags": {
+                    "shape": "TagList"
+                }
+            },
+            "required": [
+                "ModelCardName",
+                "Content",
+                "ModelCardStatus"
+            ],
+            "type": "structure"
+        },
+        "CreateModelCardResponse": {
+            "members": {
+                "ModelCardArn": {
+                    "shape": "ModelCardArn"
+                }
+            },
+            "required": [
+                "ModelCardArn"
+            ],
+            "type": "structure"
+        },
         "CreateModelExplainabilityJobDefinitionRequest": {
             "members": {
                 "JobDefinitionName": {
                     "documentation": "<p> The name of the model explainability job definition. The name must be unique within an Amazon Web Services Region in the Amazon Web Services account.</p>",
                     "shape": "MonitoringJobDefinitionName"
                 },
                 "JobResources": {
@@ -9048,15 +9582,15 @@
                     "shape": "ContainerDefinitionList"
                 },
                 "EnableNetworkIsolation": {
                     "documentation": "<p>Isolates the model container. No inbound or outbound network calls can be made to or from the model container.</p>",
                     "shape": "Boolean"
                 },
                 "ExecutionRoleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that SageMaker can assume to access model artifacts and docker image for deployment on ML compute instances or for batch transform jobs. Deploying on ML compute instances is part of model hosting. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html\">SageMaker Roles</a>. </p> <note> <p>To be able to pass this role to SageMaker, the caller of this API must have the <code>iam:PassRole</code> permission.</p> </note>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that Amazon SageMaker can assume to access model artifacts and docker image for deployment on ML compute instances or for batch transform jobs. Deploying on ML compute instances is part of model hosting. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html\">Amazon SageMaker Roles</a>. </p> <note> <p>To be able to pass this role to Amazon SageMaker, the caller of this API must have the <code>iam:PassRole</code> permission.</p> </note>",
                     "shape": "RoleArn"
                 },
                 "InferenceExecutionConfig": {
                     "documentation": "<p>Specifies details of how containers in a multi-container endpoint are called.</p>",
                     "shape": "InferenceExecutionConfig"
                 },
                 "ModelName": {
@@ -9081,15 +9615,15 @@
                 "ExecutionRoleArn"
             ],
             "type": "structure"
         },
         "CreateModelOutput": {
             "members": {
                 "ModelArn": {
-                    "documentation": "<p>The ARN of the model created in SageMaker.</p>",
+                    "documentation": "<p>The ARN of the model created in Amazon SageMaker.</p>",
                     "shape": "ModelArn"
                 }
             },
             "required": [
                 "ModelArn"
             ],
             "type": "structure"
@@ -9189,19 +9723,19 @@
                     "shape": "SourceAlgorithmSpecification"
                 },
                 "Tags": {
                     "documentation": "<p>A list of key value pairs associated with the model. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a> in the <i>Amazon Web Services General Reference Guide</i>.</p>",
                     "shape": "TagList"
                 },
                 "Task": {
-                    "documentation": "<p>The machine learning task your model package accomplishes. Common machine learning tasks include object detection and image classification. The following tasks are supported by Inference Recommender: <code>\"IMAGE_CLASSIFICATION\"</code> | <code>\"OBJECT_DETECTION\"</code> | <code>\"TEXT_GENERATION\"</code> |<code>\"IMAGE_SEGMENTATION\"</code> | <code>\"FILL_MASK\"</code> | <code>\"CLASSIFICATION\"</code> | <code>\"REGRESSION\"</code> | <code>\"OTHER\"</code>.</p> <p>Specify \"OTHER\" if none of the tasks listed fit your use case.</p>",
+                    "documentation": "<p>The machine learning task your model package accomplishes. Common machine learning tasks include object detection and image classification.</p>",
                     "shape": "String"
                 },
                 "ValidationSpecification": {
-                    "documentation": "<p>Specifies configurations for one or more transform jobs that SageMaker runs to test the model package.</p>",
+                    "documentation": "<p>Specifies configurations for one or more transform jobs that Amazon SageMaker runs to test the model package.</p>",
                     "shape": "ModelPackageValidationSpecification"
                 }
             },
             "type": "structure"
         },
         "CreateModelPackageOutput": {
             "members": {
@@ -9313,35 +9847,34 @@
         "CreateNotebookInstanceInput": {
             "members": {
                 "AcceleratorTypes": {
                     "documentation": "<p>A list of Elastic Inference (EI) instance types to associate with this notebook instance. Currently, only one instance type can be associated with a notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/ei.html\">Using Elastic Inference in Amazon SageMaker</a>.</p>",
                     "shape": "NotebookInstanceAcceleratorTypes"
                 },
                 "AdditionalCodeRepositories": {
-                    "documentation": "<p>An array of up to three Git repositories to associate with the notebook instance. These can be either the names of Git repositories stored as resources in your account, or the URL of Git repositories in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. These repositories are cloned at the same level as the default repository of your notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with SageMaker Notebook Instances</a>.</p>",
+                    "documentation": "<p>An array of up to three Git repositories to associate with the notebook instance. These can be either the names of Git repositories stored as resources in your account, or the URL of Git repositories in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. These repositories are cloned at the same level as the default repository of your notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with Amazon SageMaker Notebook Instances</a>.</p>",
                     "shape": "AdditionalCodeRepositoryNamesOrUrls"
                 },
                 "DefaultCodeRepository": {
-                    "documentation": "<p>A Git repository to associate with the notebook instance as its default code repository. This can be either the name of a Git repository stored as a resource in your account, or the URL of a Git repository in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. When you open a notebook instance, it opens in the directory that contains this repository. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with SageMaker Notebook Instances</a>.</p>",
+                    "documentation": "<p>A Git repository to associate with the notebook instance as its default code repository. This can be either the name of a Git repository stored as a resource in your account, or the URL of a Git repository in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. When you open a notebook instance, it opens in the directory that contains this repository. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with Amazon SageMaker Notebook Instances</a>.</p>",
                     "shape": "CodeRepositoryNameOrUrl"
                 },
                 "DirectInternetAccess": {
-                    "documentation": "<p>Sets whether SageMaker provides internet access to the notebook instance. If you set this to <code>Disabled</code> this notebook instance is able to access resources only in your VPC, and is not be able to connect to SageMaker training and endpoint services unless you configure a NAT Gateway in your VPC.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/appendix-additional-considerations.html#appendix-notebook-and-internet-access\">Notebook Instances Are Internet-Enabled by Default</a>. You can set the value of this parameter to <code>Disabled</code> only if you set a value for the <code>SubnetId</code> parameter.</p>",
+                    "documentation": "<p>Sets whether Amazon SageMaker provides internet access to the notebook instance. If you set this to <code>Disabled</code> this notebook instance is able to access resources only in your VPC, and is not be able to connect to Amazon SageMaker training and endpoint services unless you configure a NAT Gateway in your VPC.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/appendix-additional-considerations.html#appendix-notebook-and-internet-access\">Notebook Instances Are Internet-Enabled by Default</a>. You can set the value of this parameter to <code>Disabled</code> only if you set a value for the <code>SubnetId</code> parameter.</p>",
                     "shape": "DirectInternetAccess"
                 },
                 "InstanceMetadataServiceConfiguration": {
-                    "documentation": "<p>Information on the IMDS configuration of the notebook instance</p>",
                     "shape": "InstanceMetadataServiceConfiguration"
                 },
                 "InstanceType": {
                     "documentation": "<p>The type of ML compute instance to launch for the notebook instance.</p>",
                     "shape": "InstanceType"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of a Amazon Web Services Key Management Service key that SageMaker uses to encrypt data on the storage volume attached to your notebook instance. The KMS key you provide must be enabled. For information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/enabling-keys.html\">Enabling and Disabling Keys</a> in the <i>Amazon Web Services Key Management Service Developer Guide</i>.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of a Amazon Web Services Key Management Service key that Amazon SageMaker uses to encrypt data on the storage volume attached to your notebook instance. The KMS key you provide must be enabled. For information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/enabling-keys.html\">Enabling and Disabling Keys</a> in the <i>Amazon Web Services Key Management Service Developer Guide</i>.</p>",
                     "shape": "KmsKeyId"
                 },
                 "LifecycleConfigName": {
                     "documentation": "<p>The name of a lifecycle configuration to associate with the notebook instance. For information about lifestyle configurations, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/notebook-lifecycle-config.html\">Step 2.1: (Optional) Customize a Notebook Instance</a>.</p>",
                     "shape": "NotebookInstanceLifecycleConfigName"
                 },
                 "NotebookInstanceName": {
@@ -9349,15 +9882,15 @@
                     "shape": "NotebookInstanceName"
                 },
                 "PlatformIdentifier": {
                     "documentation": "<p>The platform identifier of the notebook instance runtime environment.</p>",
                     "shape": "PlatformIdentifier"
                 },
                 "RoleArn": {
-                    "documentation": "<p> When you send any requests to Amazon Web Services resources from the notebook instance, SageMaker assumes this role to perform tasks on your behalf. You must grant this role necessary permissions so SageMaker can perform these tasks. The policy must allow the SageMaker service principal (sagemaker.amazonaws.com) permissions to assume this role. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html\">SageMaker Roles</a>. </p> <note> <p>To be able to pass this role to SageMaker, the caller of this API must have the <code>iam:PassRole</code> permission.</p> </note>",
+                    "documentation": "<p> When you send any requests to Amazon Web Services resources from the notebook instance, Amazon SageMaker assumes this role to perform tasks on your behalf. You must grant this role necessary permissions so Amazon SageMaker can perform these tasks. The policy must allow the Amazon SageMaker service principal (sagemaker.amazonaws.com) permissions to assume this role. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html\">Amazon SageMaker Roles</a>. </p> <note> <p>To be able to pass this role to Amazon SageMaker, the caller of this API must have the <code>iam:PassRole</code> permission.</p> </note>",
                     "shape": "RoleArn"
                 },
                 "RootAccess": {
                     "documentation": "<p>Whether root access is enabled or disabled for users of the notebook instance. The default value is <code>Enabled</code>.</p> <note> <p>Lifecycle configurations need root access to be able to set up a notebook instance. Because of this, lifecycle configurations associated with a notebook instance always run with root access even if you disable root access for users.</p> </note>",
                     "shape": "RootAccess"
                 },
                 "SecurityGroupIds": {
@@ -9488,14 +10021,17 @@
                     "documentation": "<p>The number of seconds until the pre-signed URL expires. This value defaults to 300.</p>",
                     "shape": "ExpiresInSeconds"
                 },
                 "SessionExpirationDurationInSeconds": {
                     "documentation": "<p>The session expiration duration in seconds. This value defaults to 43200.</p>",
                     "shape": "SessionExpirationDurationInSeconds"
                 },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                },
                 "UserProfileName": {
                     "documentation": "<p>The name of the UserProfile to sign-in as.</p>",
                     "shape": "UserProfileName"
                 }
             },
             "required": [
                 "DomainId",
@@ -9641,14 +10177,43 @@
             },
             "required": [
                 "ProjectArn",
                 "ProjectId"
             ],
             "type": "structure"
         },
+        "CreateSpaceRequest": {
+            "members": {
+                "DomainId": {
+                    "shape": "DomainId"
+                },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                },
+                "SpaceSettings": {
+                    "shape": "SpaceSettings"
+                },
+                "Tags": {
+                    "shape": "TagList"
+                }
+            },
+            "required": [
+                "DomainId",
+                "SpaceName"
+            ],
+            "type": "structure"
+        },
+        "CreateSpaceResponse": {
+            "members": {
+                "SpaceArn": {
+                    "shape": "SpaceArn"
+                }
+            },
+            "type": "structure"
+        },
         "CreateStudioLifecycleConfigRequest": {
             "members": {
                 "StudioLifecycleConfigAppType": {
                     "documentation": "<p>The App type that the Lifecycle Configuration is attached to.</p>",
                     "shape": "StudioLifecycleConfigAppType"
                 },
                 "StudioLifecycleConfigContent": {
@@ -9679,15 +10244,15 @@
                 }
             },
             "type": "structure"
         },
         "CreateTrainingJobRequest": {
             "members": {
                 "AlgorithmSpecification": {
-                    "documentation": "<p>The registry path of the Docker image that contains the training algorithm and algorithm-specific metadata, including the input mode. For more information about algorithms provided by SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. For information about providing your own algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>. </p>",
+                    "documentation": "<p>The registry path of the Docker image that contains the training algorithm and algorithm-specific metadata, including the input mode. For more information about algorithms provided by Amazon SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. For information about providing your own algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>. </p>",
                     "shape": "AlgorithmSpecification"
                 },
                 "CheckpointConfig": {
                     "documentation": "<p>Contains information about the output location for managed spot training checkpoint data.</p>",
                     "shape": "CheckpointConfig"
                 },
                 "DebugHookConfig": {
@@ -9702,57 +10267,57 @@
                     "shape": "Boolean"
                 },
                 "EnableManagedSpotTraining": {
                     "documentation": "<p>To train models using managed spot training, choose <code>True</code>. Managed spot training provides a fully managed and scalable infrastructure for training machine learning models. this option is useful when training jobs can be interrupted and when there is flexibility when the training job is run. </p> <p>The complete and intermediate results of jobs are stored in an Amazon S3 bucket, and can be used as a starting point to train models incrementally. Amazon SageMaker provides metrics and logs in CloudWatch. They can be used to see when managed spot training jobs are running, interrupted, resumed, or completed. </p>",
                     "shape": "Boolean"
                 },
                 "EnableNetworkIsolation": {
-                    "documentation": "<p>Isolates the training container. No inbound or outbound network calls can be made, except for calls between peers within a training cluster for distributed training. If you enable network isolation for training jobs that are configured to use a VPC, SageMaker downloads and uploads customer data and model artifacts through the specified VPC, but the training container does not have network access.</p>",
+                    "documentation": "<p>Isolates the training container. No inbound or outbound network calls can be made, except for calls between peers within a training cluster for distributed training. If you enable network isolation for training jobs that are configured to use a VPC, Amazon SageMaker downloads and uploads customer data and model artifacts through the specified VPC, but the training container does not have network access.</p>",
                     "shape": "Boolean"
                 },
                 "Environment": {
                     "documentation": "<p>The environment variables to set in the Docker container.</p>",
                     "shape": "TrainingEnvironmentMap"
                 },
                 "ExperimentConfig": {
                     "shape": "ExperimentConfig"
                 },
                 "HyperParameters": {
-                    "documentation": "<p>Algorithm-specific parameters that influence the quality of the model. You set hyperparameters before you start the learning process. For a list of hyperparameters for each training algorithm provided by SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. </p> <p>You can specify a maximum of 100 hyperparameters. Each hyperparameter is a key-value pair. Each key and value is limited to 256 characters, as specified by the <code>Length Constraint</code>. </p> <important> <p>Do not include any security-sensitive information including account access IDs, secrets or tokens in any hyperparameter field. If the use of security-sensitive credentials are detected, SageMaker will reject your training job request and return an exception error.</p> </important>",
+                    "documentation": "<p>Algorithm-specific parameters that influence the quality of the model. You set hyperparameters before you start the learning process. For a list of hyperparameters for each training algorithm provided by Amazon SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. </p> <p>You can specify a maximum of 100 hyperparameters. Each hyperparameter is a key-value pair. Each key and value is limited to 256 characters, as specified by the <code>Length Constraint</code>. </p>",
                     "shape": "HyperParameters"
                 },
                 "InputDataConfig": {
-                    "documentation": "<p>An array of <code>Channel</code> objects. Each channel is a named input source. <code>InputDataConfig</code> describes the input data and its location. </p> <p>Algorithms can accept input data from one or more channels. For example, an algorithm might have two channels of input data, <code>training_data</code> and <code>validation_data</code>. The configuration for each channel provides the S3, EFS, or FSx location where the input data is stored. It also provides information about the stored data: the MIME type, compression method, and whether the data is wrapped in RecordIO format. </p> <p>Depending on the input mode that the algorithm supports, SageMaker either copies input data files from an S3 bucket to a local directory in the Docker container, or makes it available as input streams. For example, if you specify an EFS location, input data files are available as input streams. They do not need to be downloaded.</p>",
+                    "documentation": "<p>An array of <code>Channel</code> objects. Each channel is a named input source. <code>InputDataConfig</code> describes the input data and its location. </p> <p>Algorithms can accept input data from one or more channels. For example, an algorithm might have two channels of input data, <code>training_data</code> and <code>validation_data</code>. The configuration for each channel provides the S3, EFS, or FSx location where the input data is stored. It also provides information about the stored data: the MIME type, compression method, and whether the data is wrapped in RecordIO format. </p> <p>Depending on the input mode that the algorithm supports, Amazon SageMaker either copies input data files from an S3 bucket to a local directory in the Docker container, or makes it available as input streams. For example, if you specify an EFS location, input data files will be made available as input streams. They do not need to be downloaded.</p>",
                     "shape": "InputDataConfig"
                 },
                 "OutputDataConfig": {
-                    "documentation": "<p>Specifies the path to the S3 location where you want to store model artifacts. SageMaker creates subfolders for the artifacts. </p>",
+                    "documentation": "<p>Specifies the path to the S3 location where you want to store model artifacts. Amazon SageMaker creates subfolders for the artifacts. </p>",
                     "shape": "OutputDataConfig"
                 },
                 "ProfilerConfig": {
                     "shape": "ProfilerConfig"
                 },
                 "ProfilerRuleConfigurations": {
                     "documentation": "<p>Configuration information for Debugger rules for profiling system and framework metrics.</p>",
                     "shape": "ProfilerRuleConfigurations"
                 },
                 "ResourceConfig": {
-                    "documentation": "<p>The resources, including the ML compute instances and ML storage volumes, to use for model training. </p> <p>ML storage volumes store model artifacts and incremental states. Training algorithms might also use ML storage volumes for scratch space. If you want SageMaker to use the ML storage volume to store the training data, choose <code>File</code> as the <code>TrainingInputMode</code> in the algorithm specification. For distributed training algorithms, specify an instance count greater than 1.</p>",
+                    "documentation": "<p>The resources, including the ML compute instances and ML storage volumes, to use for model training. </p> <p>ML storage volumes store model artifacts and incremental states. Training algorithms might also use ML storage volumes for scratch space. If you want Amazon SageMaker to use the ML storage volume to store the training data, choose <code>File</code> as the <code>TrainingInputMode</code> in the algorithm specification. For distributed training algorithms, specify an instance count greater than 1.</p>",
                     "shape": "ResourceConfig"
                 },
                 "RetryStrategy": {
                     "documentation": "<p>The number of times to retry the job when the job fails due to an <code>InternalServerError</code>.</p>",
                     "shape": "RetryStrategy"
                 },
                 "RoleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of an IAM role that SageMaker can assume to perform tasks on your behalf. </p> <p>During model training, SageMaker needs your permission to read input data from an S3 bucket, download a Docker image that contains training code, write model artifacts to an S3 bucket, write logs to Amazon CloudWatch Logs, and publish metrics to Amazon CloudWatch. You grant permissions for all of these tasks to an IAM role. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html\">SageMaker Roles</a>. </p> <note> <p>To be able to pass this role to SageMaker, the caller of this API must have the <code>iam:PassRole</code> permission.</p> </note>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of an IAM role that Amazon SageMaker can assume to perform tasks on your behalf. </p> <p>During model training, Amazon SageMaker needs your permission to read input data from an S3 bucket, download a Docker image that contains training code, write model artifacts to an S3 bucket, write logs to Amazon CloudWatch Logs, and publish metrics to Amazon CloudWatch. You grant permissions for all of these tasks to an IAM role. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html\">Amazon SageMaker Roles</a>. </p> <note> <p>To be able to pass this role to Amazon SageMaker, the caller of this API must have the <code>iam:PassRole</code> permission.</p> </note>",
                     "shape": "RoleArn"
                 },
                 "StoppingCondition": {
-                    "documentation": "<p>Specifies a limit to how long a model training job can run. It also specifies how long a managed Spot training job has to complete. When the job reaches the time limit, SageMaker ends the training job. Use this API to cap model training costs.</p> <p>To stop a job, SageMaker sends the algorithm the <code>SIGTERM</code> signal, which delays job termination for 120 seconds. Algorithms can use this 120-second window to save the model artifacts, so the results of training are not lost. </p>",
+                    "documentation": "<p>Specifies a limit to how long a model training job can run. It also specifies how long a managed Spot training job has to complete. When the job reaches the time limit, Amazon SageMaker ends the training job. Use this API to cap model training costs.</p> <p>To stop a job, Amazon SageMaker sends the algorithm the <code>SIGTERM</code> signal, which delays job termination for 120 seconds. Algorithms can use this 120-second window to save the model artifacts, so the results of training are not lost. </p>",
                     "shape": "StoppingCondition"
                 },
                 "Tags": {
                     "documentation": "<p>An array of key-value pairs. You can use tags to categorize your Amazon Web Services resources in different ways, for example, by purpose, owner, or environment. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a>.</p>",
                     "shape": "TagList"
                 },
                 "TensorBoardOutputConfig": {
@@ -9792,15 +10357,14 @@
         "CreateTransformJobRequest": {
             "members": {
                 "BatchStrategy": {
                     "documentation": "<p>Specifies the number of records to include in a mini-batch for an HTTP inference request. A <i>record</i> <i/> is a single unit of input data that inference can be made on. For example, a single line in a CSV file is a record. </p> <p>To enable the batch strategy, you must set the <code>SplitType</code> property to <code>Line</code>, <code>RecordIO</code>, or <code>TFRecord</code>.</p> <p>To use only one record when making an HTTP invocation request to a container, set <code>BatchStrategy</code> to <code>SingleRecord</code> and <code>SplitType</code> to <code>Line</code>.</p> <p>To fit as many records in a mini-batch as can fit within the <code>MaxPayloadInMB</code> limit, set <code>BatchStrategy</code> to <code>MultiRecord</code> and <code>SplitType</code> to <code>Line</code>.</p>",
                     "shape": "BatchStrategy"
                 },
                 "DataCaptureConfig": {
-                    "documentation": "<p>Configuration to control how SageMaker captures inference data.</p>",
                     "shape": "BatchDataCaptureConfig"
                 },
                 "DataProcessing": {
                     "documentation": "<p>The data structure used to specify the data to be used for inference in a batch transform job and to associate the data that is relevant to the prediction results in the output. The input filter provided allows you to exclude input data that is not needed for inference in a batch transform job. The output filter provided allows you to include input data relevant to interpreting the predictions in the output from the job. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-transform-data-processing.html\">Associate Prediction Results with their Corresponding Input Records</a>.</p>",
                     "shape": "DataProcessing"
                 },
                 "Environment": {
@@ -9811,15 +10375,15 @@
                     "shape": "ExperimentConfig"
                 },
                 "MaxConcurrentTransforms": {
                     "documentation": "<p>The maximum number of parallel requests that can be sent to each instance in a transform job. If <code>MaxConcurrentTransforms</code> is set to <code>0</code> or left unset, Amazon SageMaker checks the optional execution-parameters to determine the settings for your chosen algorithm. If the execution-parameters endpoint is not enabled, the default value is <code>1</code>. For more information on execution-parameters, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms-batch-code.html#your-algorithms-batch-code-how-containe-serves-requests\">How Containers Serve Requests</a>. For built-in algorithms, you don't need to set a value for <code>MaxConcurrentTransforms</code>.</p>",
                     "shape": "MaxConcurrentTransforms"
                 },
                 "MaxPayloadInMB": {
-                    "documentation": "<p>The maximum allowed size of the payload, in MB. A <i>payload</i> is the data portion of a record (without metadata). The value in <code>MaxPayloadInMB</code> must be greater than, or equal to, the size of a single record. To estimate the size of a record in MB, divide the size of your dataset by the number of records. To ensure that the records fit within the maximum payload size, we recommend using a slightly larger value. The default value is <code>6</code> MB. </p> <p>The value of <code>MaxPayloadInMB</code> cannot be greater than 100 MB. If you specify the <code>MaxConcurrentTransforms</code> parameter, the value of <code>(MaxConcurrentTransforms * MaxPayloadInMB)</code> also cannot exceed 100 MB.</p> <p>For cases where the payload might be arbitrarily large and is transmitted using HTTP chunked encoding, set the value to <code>0</code>. This feature works only in supported algorithms. Currently, Amazon SageMaker built-in algorithms do not support HTTP chunked encoding.</p>",
+                    "documentation": "<p>The maximum allowed size of the payload, in MB. A <i>payload</i> is the data portion of a record (without metadata). The value in <code>MaxPayloadInMB</code> must be greater than, or equal to, the size of a single record. To estimate the size of a record in MB, divide the size of your dataset by the number of records. To ensure that the records fit within the maximum payload size, we recommend using a slightly larger value. The default value is <code>6</code> MB. </p> <p>For cases where the payload might be arbitrarily large and is transmitted using HTTP chunked encoding, set the value to <code>0</code>. This feature works only in supported algorithms. Currently, Amazon SageMaker built-in algorithms do not support HTTP chunked encoding.</p>",
                     "shape": "MaxPayloadInMB"
                 },
                 "ModelClientConfig": {
                     "documentation": "<p>Configures the timeout and maximum number of retries for processing a transform job invocation.</p>",
                     "shape": "ModelClientConfig"
                 },
                 "ModelName": {
@@ -9964,19 +10528,19 @@
         "CreateUserProfileRequest": {
             "members": {
                 "DomainId": {
                     "documentation": "<p>The ID of the associated Domain.</p>",
                     "shape": "DomainId"
                 },
                 "SingleSignOnUserIdentifier": {
-                    "documentation": "<p>A specifier for the type of value specified in SingleSignOnUserValue. Currently, the only supported value is \"UserName\". If the Domain's AuthMode is IAM Identity Center, this field is required. If the Domain's AuthMode is not IAM Identity Center, this field cannot be specified. </p>",
+                    "documentation": "<p>A specifier for the type of value specified in SingleSignOnUserValue. Currently, the only supported value is \"UserName\". If the Domain's AuthMode is SSO, this field is required. If the Domain's AuthMode is not SSO, this field cannot be specified. </p>",
                     "shape": "SingleSignOnUserIdentifier"
                 },
                 "SingleSignOnUserValue": {
-                    "documentation": "<p>The username of the associated Amazon Web Services Single Sign-On User for this UserProfile. If the Domain's AuthMode is IAM Identity Center, this field is required, and must match a valid username of a user in your directory. If the Domain's AuthMode is not IAM Identity Center, this field cannot be specified. </p>",
+                    "documentation": "<p>The username of the associated Amazon Web Services Single Sign-On User for this UserProfile. If the Domain's AuthMode is SSO, this field is required, and must match a valid username of a user in your directory. If the Domain's AuthMode is not SSO, this field cannot be specified. </p>",
                     "shape": "String256"
                 },
                 "Tags": {
                     "documentation": "<p>Each tag consists of a key and an optional value. Tag keys must be unique per resource.</p> <p>Tags that you specify for the User Profile are also added to all Apps that the User Profile launches.</p>",
                     "shape": "TagList"
                 },
                 "UserProfileName": {
@@ -10021,15 +10585,14 @@
                     "shape": "TagList"
                 },
                 "WorkforceName": {
                     "documentation": "<p>The name of the private workforce.</p>",
                     "shape": "WorkforceName"
                 },
                 "WorkforceVpcConfig": {
-                    "documentation": "<p>Use this parameter to configure a workforce using VPC.</p>",
                     "shape": "WorkforceVpcConfigRequest"
                 }
             },
             "required": [
                 "WorkforceName"
             ],
             "type": "structure"
@@ -10162,69 +10725,69 @@
         "CustomerMetadataValue": {
             "max": 256,
             "min": 1,
             "pattern": "^([\\p{L}\\p{Z}\\p{N}_.:\\/=+\\-@]*)${1,256}",
             "type": "string"
         },
         "DataCaptureConfig": {
-            "documentation": "<p>Configuration to control how SageMaker captures inference data.</p>",
+            "documentation": "<p/>",
             "members": {
                 "CaptureContentTypeHeader": {
-                    "documentation": "<p>Configuration specifying how to treat different headers. If no headers are specified SageMaker will by default base64 encode when capturing the data.</p>",
+                    "documentation": "<p/>",
                     "shape": "CaptureContentTypeHeader"
                 },
                 "CaptureOptions": {
-                    "documentation": "<p>Specifies data Model Monitor will capture. You can configure whether to collect only input, only output, or both</p>",
+                    "documentation": "<p/>",
                     "shape": "CaptureOptionList"
                 },
                 "DestinationS3Uri": {
-                    "documentation": "<p>The Amazon S3 location used to capture the data.</p>",
+                    "documentation": "<p/>",
                     "shape": "DestinationS3Uri"
                 },
                 "EnableCapture": {
-                    "documentation": "<p>Whether data capture should be enabled or disabled (defaults to enabled).</p>",
+                    "documentation": "<p/>",
                     "shape": "EnableCapture"
                 },
                 "InitialSamplingPercentage": {
-                    "documentation": "<p>The percentage of requests SageMaker will capture. A lower value is recommended for Endpoints with high traffic.</p>",
+                    "documentation": "<p/>",
                     "shape": "SamplingPercentage"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of a Amazon Web Services Key Management Service key that SageMaker uses to encrypt data on the storage volume attached to the ML compute instance that hosts the endpoint.</p> <p>The KmsKeyId can be any of the following formats: </p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias name ARN: <code>arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul>",
+                    "documentation": "<p/>",
                     "shape": "KmsKeyId"
                 }
             },
             "required": [
                 "InitialSamplingPercentage",
                 "DestinationS3Uri",
                 "CaptureOptions"
             ],
             "type": "structure"
         },
         "DataCaptureConfigSummary": {
-            "documentation": "<p>The currently active data capture configuration used by your Endpoint.</p>",
+            "documentation": "<p/>",
             "members": {
                 "CaptureStatus": {
-                    "documentation": "<p>Whether data capture is currently functional.</p>",
+                    "documentation": "<p/>",
                     "shape": "CaptureStatus"
                 },
                 "CurrentSamplingPercentage": {
-                    "documentation": "<p>The percentage of requests being captured by your Endpoint.</p>",
+                    "documentation": "<p/>",
                     "shape": "SamplingPercentage"
                 },
                 "DestinationS3Uri": {
-                    "documentation": "<p>The Amazon S3 location being used to capture the data.</p>",
+                    "documentation": "<p/>",
                     "shape": "DestinationS3Uri"
                 },
                 "EnableCapture": {
-                    "documentation": "<p>Whether data capture is enabled or disabled.</p>",
+                    "documentation": "<p/>",
                     "shape": "EnableCapture"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The KMS key being used to encrypt the data in Amazon S3.</p>",
+                    "documentation": "<p/>",
                     "shape": "KmsKeyId"
                 }
             },
             "required": [
                 "EnableCapture",
                 "CaptureStatus",
                 "CurrentSamplingPercentage",
@@ -10273,23 +10836,23 @@
             "pattern": "[\\S\\s]+",
             "type": "string"
         },
         "DataProcessing": {
             "documentation": "<p>The data structure used to specify the data to be used for inference in a batch transform job and to associate the data that is relevant to the prediction results in the output. The input filter provided allows you to exclude input data that is not needed for inference in a batch transform job. The output filter provided allows you to include input data relevant to interpreting the predictions in the output from the job. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-transform-data-processing.html\">Associate Prediction Results with their Corresponding Input Records</a>.</p>",
             "members": {
                 "InputFilter": {
-                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-transform-data-processing.html#data-processing-operators\">JSONPath</a> expression used to select a portion of the input data to pass to the algorithm. Use the <code>InputFilter</code> parameter to exclude fields, such as an ID column, from the input. If you want SageMaker to pass the entire input dataset to the algorithm, accept the default value <code>$</code>.</p> <p>Examples: <code>\"$\"</code>, <code>\"$[1:]\"</code>, <code>\"$.features\"</code> </p>",
+                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-transform-data-processing.html#data-processing-operators\">JSONPath</a> expression used to select a portion of the input data to pass to the algorithm. Use the <code>InputFilter</code> parameter to exclude fields, such as an ID column, from the input. If you want Amazon SageMaker to pass the entire input dataset to the algorithm, accept the default value <code>$</code>.</p> <p>Examples: <code>\"$\"</code>, <code>\"$[1:]\"</code>, <code>\"$.features\"</code> </p>",
                     "shape": "JsonPath"
                 },
                 "JoinSource": {
                     "documentation": "<p>Specifies the source of the data to join with the transformed data. The valid values are <code>None</code> and <code>Input</code>. The default value is <code>None</code>, which specifies not to join the input with the transformed data. If you want the batch transform job to join the original input data with the transformed data, set <code>JoinSource</code> to <code>Input</code>. You can specify <code>OutputFilter</code> as an additional filter to select a portion of the joined dataset and store it in the output file.</p> <p>For JSON or JSONLines objects, such as a JSON array, SageMaker adds the transformed data to the input JSON object in an attribute called <code>SageMakerOutput</code>. The joined result for JSON must be a key-value pair object. If the input is not a key-value pair object, SageMaker creates a new JSON file. In the new JSON file, and the input data is stored under the <code>SageMakerInput</code> key and the results are stored in <code>SageMakerOutput</code>.</p> <p>For CSV data, SageMaker takes each row as a JSON array and joins the transformed data with the input by appending each transformed row to the end of the input. The joined data has the original input data followed by the transformed data and the output is a CSV file.</p> <p>For information on how joining in applied, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-transform-data-processing.html#batch-transform-data-processing-workflow\">Workflow for Associating Inferences with Input Records</a>.</p>",
                     "shape": "JoinSource"
                 },
                 "OutputFilter": {
-                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-transform-data-processing.html#data-processing-operators\">JSONPath</a> expression used to select a portion of the joined dataset to save in the output file for a batch transform job. If you want SageMaker to store the entire input dataset in the output file, leave the default value, <code>$</code>. If you specify indexes that aren't within the dimension size of the joined dataset, you get an error.</p> <p>Examples: <code>\"$\"</code>, <code>\"$[0,5:]\"</code>, <code>\"$['id','SageMakerOutput']\"</code> </p>",
+                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-transform-data-processing.html#data-processing-operators\">JSONPath</a> expression used to select a portion of the joined dataset to save in the output file for a batch transform job. If you want Amazon SageMaker to store the entire input dataset in the output file, leave the default value, <code>$</code>. If you specify indexes that aren't within the dimension size of the joined dataset, you get an error.</p> <p>Examples: <code>\"$\"</code>, <code>\"$[0,5:]\"</code>, <code>\"$['id','SageMakerOutput']\"</code> </p>",
                     "shape": "JsonPath"
                 }
             },
             "type": "structure"
         },
         "DataQualityAppSpecification": {
             "documentation": "<p>Information about the container that a data quality monitoring job runs.</p>",
@@ -10340,15 +10903,14 @@
             },
             "type": "structure"
         },
         "DataQualityJobInput": {
             "documentation": "<p>The input for the data quality monitoring job. Currently endpoints are supported for input.</p>",
             "members": {
                 "BatchTransformInput": {
-                    "documentation": "<p>Input object for the batch transform job.</p>",
                     "shape": "BatchTransformInput"
                 },
                 "EndpointInput": {
                     "shape": "EndpointInput"
                 }
             },
             "type": "structure"
@@ -10503,14 +11065,31 @@
             "type": "list"
         },
         "DefaultGid": {
             "max": 65535,
             "min": 0,
             "type": "integer"
         },
+        "DefaultSpaceSettings": {
+            "members": {
+                "ExecutionRole": {
+                    "shape": "RoleArn"
+                },
+                "JupyterServerAppSettings": {
+                    "shape": "JupyterServerAppSettings"
+                },
+                "KernelGatewayAppSettings": {
+                    "shape": "KernelGatewayAppSettings"
+                },
+                "SecurityGroups": {
+                    "shape": "SecurityGroupIds"
+                }
+            },
+            "type": "structure"
+        },
         "DefaultUid": {
             "max": 65535,
             "min": 0,
             "type": "integer"
         },
         "DeleteActionRequest": {
             "members": {
@@ -10567,22 +11146,24 @@
                     "documentation": "<p>The type of app.</p>",
                     "shape": "AppType"
                 },
                 "DomainId": {
                     "documentation": "<p>The domain ID.</p>",
                     "shape": "DomainId"
                 },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                },
                 "UserProfileName": {
                     "documentation": "<p>The user profile name.</p>",
                     "shape": "UserProfileName"
                 }
             },
             "required": [
                 "DomainId",
-                "UserProfileName",
                 "AppType",
                 "AppName"
             ],
             "type": "structure"
         },
         "DeleteArtifactRequest": {
             "members": {
@@ -10708,31 +11289,28 @@
                 "DomainId"
             ],
             "type": "structure"
         },
         "DeleteEdgeDeploymentPlanRequest": {
             "members": {
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the edge deployment plan to delete.</p>",
                     "shape": "EntityName"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanName"
             ],
             "type": "structure"
         },
         "DeleteEdgeDeploymentStageRequest": {
             "members": {
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the edge deployment plan from which the stage will be deleted.</p>",
                     "shape": "EntityName"
                 },
                 "StageName": {
-                    "documentation": "<p>The name of the stage.</p>",
                     "shape": "EntityName"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanName",
                 "StageName"
             ],
@@ -10860,26 +11438,59 @@
             ],
             "type": "structure"
         },
         "DeleteImageVersionResponse": {
             "members": {},
             "type": "structure"
         },
+        "DeleteInferenceExperimentRequest": {
+            "members": {
+                "Name": {
+                    "shape": "InferenceExperimentName"
+                }
+            },
+            "required": [
+                "Name"
+            ],
+            "type": "structure"
+        },
+        "DeleteInferenceExperimentResponse": {
+            "members": {
+                "InferenceExperimentArn": {
+                    "shape": "InferenceExperimentArn"
+                }
+            },
+            "required": [
+                "InferenceExperimentArn"
+            ],
+            "type": "structure"
+        },
         "DeleteModelBiasJobDefinitionRequest": {
             "members": {
                 "JobDefinitionName": {
                     "documentation": "<p>The name of the model bias job definition to delete.</p>",
                     "shape": "MonitoringJobDefinitionName"
                 }
             },
             "required": [
                 "JobDefinitionName"
             ],
             "type": "structure"
         },
+        "DeleteModelCardRequest": {
+            "members": {
+                "ModelCardName": {
+                    "shape": "EntityName"
+                }
+            },
+            "required": [
+                "ModelCardName"
+            ],
+            "type": "structure"
+        },
         "DeleteModelExplainabilityJobDefinitionRequest": {
             "members": {
                 "JobDefinitionName": {
                     "documentation": "<p>The name of the model explainability job definition to delete.</p>",
                     "shape": "MonitoringJobDefinitionName"
                 }
             },
@@ -10959,15 +11570,15 @@
                 "MonitoringScheduleName"
             ],
             "type": "structure"
         },
         "DeleteNotebookInstanceInput": {
             "members": {
                 "NotebookInstanceName": {
-                    "documentation": "<p>The name of the SageMaker notebook instance to delete.</p>",
+                    "documentation": "<p>The name of the Amazon SageMaker notebook instance to delete.</p>",
                     "shape": "NotebookInstanceName"
                 }
             },
             "required": [
                 "NotebookInstanceName"
             ],
             "type": "structure"
@@ -11019,14 +11630,29 @@
                 }
             },
             "required": [
                 "ProjectName"
             ],
             "type": "structure"
         },
+        "DeleteSpaceRequest": {
+            "members": {
+                "DomainId": {
+                    "shape": "DomainId"
+                },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                }
+            },
+            "required": [
+                "DomainId",
+                "SpaceName"
+            ],
+            "type": "structure"
+        },
         "DeleteStudioLifecycleConfigRequest": {
             "members": {
                 "StudioLifecycleConfigName": {
                     "documentation": "<p>The name of the Studio Lifecycle Configuration to delete.</p>",
                     "shape": "StudioLifecycleConfigName"
                 }
             },
@@ -11193,26 +11819,22 @@
             },
             "required": [
                 "BlueGreenUpdatePolicy"
             ],
             "type": "structure"
         },
         "DeploymentStage": {
-            "documentation": "<p>Contains information about a stage in an edge deployment plan.</p>",
             "members": {
                 "DeploymentConfig": {
-                    "documentation": "<p>Configuration of the deployment details.</p>",
                     "shape": "EdgeDeploymentConfig"
                 },
                 "DeviceSelectionConfig": {
-                    "documentation": "<p>Configuration of the devices in the stage.</p>",
                     "shape": "DeviceSelectionConfig"
                 },
                 "StageName": {
-                    "documentation": "<p>The name of the stage.</p>",
                     "shape": "EntityName"
                 }
             },
             "required": [
                 "StageName",
                 "DeviceSelectionConfig"
             ],
@@ -11225,30 +11847,25 @@
         "DeploymentStageStatusSummaries": {
             "member": {
                 "shape": "DeploymentStageStatusSummary"
             },
             "type": "list"
         },
         "DeploymentStageStatusSummary": {
-            "documentation": "<p>Contains information summarizing the deployment stage results.</p>",
             "members": {
                 "DeploymentConfig": {
-                    "documentation": "<p>Configuration of the deployment details.</p>",
                     "shape": "EdgeDeploymentConfig"
                 },
                 "DeploymentStatus": {
-                    "documentation": "<p>General status of the current state.</p>",
                     "shape": "EdgeDeploymentStatus"
                 },
                 "DeviceSelectionConfig": {
-                    "documentation": "<p>Configuration of the devices in the stage.</p>",
                     "shape": "DeviceSelectionConfig"
                 },
                 "StageName": {
-                    "documentation": "<p>The name of the stage.</p>",
                     "shape": "EntityName"
                 }
             },
             "required": [
                 "StageName",
                 "DeviceSelectionConfig",
                 "DeploymentConfig",
@@ -11396,15 +12013,15 @@
                     "shape": "ProductId"
                 },
                 "TrainingSpecification": {
                     "documentation": "<p>Details about training jobs run by this algorithm.</p>",
                     "shape": "TrainingSpecification"
                 },
                 "ValidationSpecification": {
-                    "documentation": "<p>Details about configurations for one or more training jobs that SageMaker runs to test the algorithm.</p>",
+                    "documentation": "<p>Details about configurations for one or more training jobs that Amazon SageMaker runs to test the algorithm.</p>",
                     "shape": "AlgorithmValidationSpecification"
                 }
             },
             "required": [
                 "AlgorithmName",
                 "AlgorithmArn",
                 "CreationTime",
@@ -11461,22 +12078,24 @@
                     "documentation": "<p>The type of app.</p>",
                     "shape": "AppType"
                 },
                 "DomainId": {
                     "documentation": "<p>The domain ID.</p>",
                     "shape": "DomainId"
                 },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                },
                 "UserProfileName": {
                     "documentation": "<p>The user profile name.</p>",
                     "shape": "UserProfileName"
                 }
             },
             "required": [
                 "DomainId",
-                "UserProfileName",
                 "AppType",
                 "AppName"
             ],
             "type": "structure"
         },
         "DescribeAppResponse": {
             "members": {
@@ -11512,14 +12131,17 @@
                     "documentation": "<p>The timestamp of the last user's activity. <code>LastUserActivityTimestamp</code> is also updated when SageMaker performs health checks without user activity. As a result, this value is set to the same value as <code>LastHealthCheckTimestamp</code>.</p>",
                     "shape": "Timestamp"
                 },
                 "ResourceSpec": {
                     "documentation": "<p>The instance type and the Amazon Resource Name (ARN) of the SageMaker image created on the instance.</p>",
                     "shape": "ResourceSpec"
                 },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                },
                 "Status": {
                     "documentation": "<p>The status.</p>",
                     "shape": "AppStatus"
                 },
                 "UserProfileName": {
                     "documentation": "<p>The user profile name.</p>",
                     "shape": "UserProfileName"
@@ -12122,14 +12744,17 @@
                     "documentation": "<p>The domain's authentication mode.</p>",
                     "shape": "AuthMode"
                 },
                 "CreationTime": {
                     "documentation": "<p>The creation time.</p>",
                     "shape": "CreationTime"
                 },
+                "DefaultSpaceSettings": {
+                    "shape": "DefaultSpaceSettings"
+                },
                 "DefaultUserSettings": {
                     "documentation": "<p>Settings which are applied to UserProfiles in this domain if settings are not explicitly specified in a given UserProfile. </p>",
                     "shape": "UserSettings"
                 },
                 "DomainArn": {
                     "documentation": "<p>The domain's Amazon Resource Name (ARN).</p>",
                     "shape": "DomainArn"
@@ -12169,15 +12794,15 @@
                     "shape": "LastModifiedTime"
                 },
                 "SecurityGroupIdForDomainBoundary": {
                     "documentation": "<p>The ID of the security group that authorizes traffic between the <code>RSessionGateway</code> apps and the <code>RStudioServerPro</code> app.</p>",
                     "shape": "SecurityGroupId"
                 },
                 "SingleSignOnManagedApplicationInstanceId": {
-                    "documentation": "<p>The IAM Identity Center managed application instance ID.</p>",
+                    "documentation": "<p>The SSO managed application instance ID.</p>",
                     "shape": "String256"
                 },
                 "Status": {
                     "documentation": "<p>The status.</p>",
                     "shape": "DomainStatus"
                 },
                 "SubnetIds": {
@@ -12194,75 +12819,61 @@
                 }
             },
             "type": "structure"
         },
         "DescribeEdgeDeploymentPlanRequest": {
             "members": {
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the deployment plan to describe.</p>",
                     "shape": "EntityName"
                 },
                 "MaxResults": {
-                    "documentation": "<p>The maximum number of results to select (50 by default).</p>",
                     "shape": "DeploymentStageMaxResults"
                 },
                 "NextToken": {
-                    "documentation": "<p>If the edge deployment plan has enough stages to require tokening, then this is the response from the last list of stages returned.</p>",
                     "shape": "NextToken"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanName"
             ],
             "type": "structure"
         },
         "DescribeEdgeDeploymentPlanResponse": {
             "members": {
                 "CreationTime": {
-                    "documentation": "<p>The time when the edge deployment plan was created.</p>",
                     "shape": "Timestamp"
                 },
                 "DeviceFleetName": {
-                    "documentation": "<p>The device fleet used for this edge deployment plan.</p>",
                     "shape": "EntityName"
                 },
                 "EdgeDeploymentFailed": {
-                    "documentation": "<p>The number of edge devices that failed the deployment.</p>",
                     "shape": "Integer"
                 },
                 "EdgeDeploymentPending": {
-                    "documentation": "<p>The number of edge devices yet to pick up deployment, or in progress.</p>",
                     "shape": "Integer"
                 },
                 "EdgeDeploymentPlanArn": {
-                    "documentation": "<p>The ARN of edge deployment plan.</p>",
                     "shape": "EdgeDeploymentPlanArn"
                 },
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the edge deployment plan.</p>",
                     "shape": "EntityName"
                 },
                 "EdgeDeploymentSuccess": {
-                    "documentation": "<p>The number of edge devices with the successful deployment.</p>",
                     "shape": "Integer"
                 },
                 "LastModifiedTime": {
-                    "documentation": "<p>The time when the edge deployment plan was last updated.</p>",
                     "shape": "Timestamp"
                 },
                 "ModelConfigs": {
-                    "documentation": "<p>List of models associated with the edge deployment plan.</p>",
                     "shape": "EdgeDeploymentModelConfigs"
                 },
                 "NextToken": {
-                    "documentation": "<p>Token to use when calling the next set of stages in the edge deployment plan.</p>",
                     "shape": "NextToken"
                 },
                 "Stages": {
-                    "documentation": "<p>List of stages in the edge deployment plan.</p>",
                     "shape": "DeploymentStageStatusSummaries"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanArn",
                 "EdgeDeploymentPlanName",
                 "ModelConfigs",
@@ -12379,28 +12990,30 @@
                     "shape": "DataCaptureConfig"
                 },
                 "EndpointConfigArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the endpoint configuration.</p>",
                     "shape": "EndpointConfigArn"
                 },
                 "EndpointConfigName": {
-                    "documentation": "<p>Name of the SageMaker endpoint configuration.</p>",
+                    "documentation": "<p>Name of the Amazon SageMaker endpoint configuration.</p>",
                     "shape": "EndpointConfigName"
                 },
                 "ExplainerConfig": {
-                    "documentation": "<p>The configuration parameters for an explainer.</p>",
                     "shape": "ExplainerConfig"
                 },
                 "KmsKeyId": {
                     "documentation": "<p>Amazon Web Services KMS key ID Amazon SageMaker uses to encrypt data when storing it on the ML storage volume attached to the instance.</p>",
                     "shape": "KmsKeyId"
                 },
                 "ProductionVariants": {
                     "documentation": "<p>An array of <code>ProductionVariant</code> objects, one for each model that you want to host at this endpoint.</p>",
                     "shape": "ProductionVariantList"
+                },
+                "ShadowProductionVariants": {
+                    "shape": "ProductionVariantList"
                 }
             },
             "required": [
                 "EndpointConfigName",
                 "EndpointConfigArn",
                 "ProductionVariants",
                 "CreationTime"
@@ -12445,15 +13058,14 @@
                     "shape": "EndpointName"
                 },
                 "EndpointStatus": {
                     "documentation": "<p>The status of the endpoint.</p> <ul> <li> <p> <code>OutOfService</code>: Endpoint is not available to take incoming requests.</p> </li> <li> <p> <code>Creating</code>: <a>CreateEndpoint</a> is executing.</p> </li> <li> <p> <code>Updating</code>: <a>UpdateEndpoint</a> or <a>UpdateEndpointWeightsAndCapacities</a> is executing.</p> </li> <li> <p> <code>SystemUpdating</code>: Endpoint is undergoing maintenance and cannot be updated or deleted or re-scaled until it has completed. This maintenance operation does not change any customer-specified values such as VPC config, KMS encryption, model, instance type, or instance count.</p> </li> <li> <p> <code>RollingBack</code>: Endpoint fails to scale up or down or change its variant weight and is in the process of rolling back to its previous configuration. Once the rollback completes, endpoint returns to an <code>InService</code> status. This transitional status only applies to an endpoint that has autoscaling enabled and is undergoing variant weight or capacity changes as part of an <a>UpdateEndpointWeightsAndCapacities</a> call or when the <a>UpdateEndpointWeightsAndCapacities</a> operation is called explicitly.</p> </li> <li> <p> <code>InService</code>: Endpoint is available to process incoming requests.</p> </li> <li> <p> <code>Deleting</code>: <a>DeleteEndpoint</a> is executing.</p> </li> <li> <p> <code>Failed</code>: Endpoint could not be created, updated, or re-scaled. Use <a>DescribeEndpointOutput$FailureReason</a> for information about the failure. <a>DeleteEndpoint</a> is the only operation that can be performed on a failed endpoint.</p> </li> </ul>",
                     "shape": "EndpointStatus"
                 },
                 "ExplainerConfig": {
-                    "documentation": "<p>The configuration parameters for an explainer.</p>",
                     "shape": "ExplainerConfig"
                 },
                 "FailureReason": {
                     "documentation": "<p>If the status of the endpoint is <code>Failed</code>, the reason why it failed. </p>",
                     "shape": "FailureReason"
                 },
                 "LastDeploymentConfig": {
@@ -12467,14 +13079,17 @@
                 "PendingDeploymentSummary": {
                     "documentation": "<p>Returns the summary of an in-progress deployment. This field is only returned when the endpoint is creating or updating with a new endpoint configuration.</p>",
                     "shape": "PendingDeploymentSummary"
                 },
                 "ProductionVariants": {
                     "documentation": "<p> An array of <a>ProductionVariantSummary</a> objects, one for each model hosted behind this endpoint. </p>",
                     "shape": "ProductionVariantSummaryList"
+                },
+                "ShadowProductionVariants": {
+                    "shape": "ProductionVariantSummaryList"
                 }
             },
             "required": [
                 "EndpointName",
                 "EndpointArn",
                 "EndpointConfigName",
                 "EndpointStatus",
@@ -12583,19 +13198,17 @@
                     "shape": "FeatureGroupName"
                 },
                 "FeatureGroupStatus": {
                     "documentation": "<p>The status of the feature group.</p>",
                     "shape": "FeatureGroupStatus"
                 },
                 "LastModifiedTime": {
-                    "documentation": "<p>A timestamp indicating when the feature group was last updated.</p>",
                     "shape": "LastModifiedTime"
                 },
                 "LastUpdateStatus": {
-                    "documentation": "<p>A value indicating whether the update made to the feature group was successful.</p>",
                     "shape": "LastUpdateStatus"
                 },
                 "NextToken": {
                     "documentation": "<p>A token to resume pagination of the list of <code>Features</code> (<code>FeatureDefinitions</code>).</p>",
                     "shape": "NextToken"
                 },
                 "OfflineStoreConfig": {
@@ -12607,15 +13220,14 @@
                     "shape": "OfflineStoreStatus"
                 },
                 "OnlineStoreConfig": {
                     "documentation": "<p>The configuration for the <code>OnlineStore</code>.</p>",
                     "shape": "OnlineStoreConfig"
                 },
                 "OnlineStoreTotalSizeBytes": {
-                    "documentation": "<p>The size of the <code>OnlineStore</code> in bytes.</p>",
                     "shape": "OnlineStoreTotalSizeBytes"
                 },
                 "RecordIdentifierFeatureName": {
                     "documentation": "<p>The name of the <code>Feature</code> used for <code>RecordIdentifier</code>, whose value uniquely identifies a record stored in the feature store.</p>",
                     "shape": "FeatureName"
                 },
                 "RoleArn": {
@@ -12633,60 +13245,50 @@
                 "NextToken"
             ],
             "type": "structure"
         },
         "DescribeFeatureMetadataRequest": {
             "members": {
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group containing the feature.</p>",
                     "shape": "FeatureGroupName"
                 },
                 "FeatureName": {
-                    "documentation": "<p>The name of the feature.</p>",
                     "shape": "FeatureName"
                 }
             },
             "required": [
                 "FeatureGroupName",
                 "FeatureName"
             ],
             "type": "structure"
         },
         "DescribeFeatureMetadataResponse": {
             "members": {
                 "CreationTime": {
-                    "documentation": "<p>A timestamp indicating when the feature was created.</p>",
                     "shape": "CreationTime"
                 },
                 "Description": {
-                    "documentation": "<p>The description you added to describe the feature.</p>",
                     "shape": "FeatureDescription"
                 },
                 "FeatureGroupArn": {
-                    "documentation": "<p>The Amazon Resource Number (ARN) of the feature group that contains the feature.</p>",
                     "shape": "FeatureGroupArn"
                 },
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group that you've specified.</p>",
                     "shape": "FeatureGroupName"
                 },
                 "FeatureName": {
-                    "documentation": "<p>The name of the feature that you've specified.</p>",
                     "shape": "FeatureName"
                 },
                 "FeatureType": {
-                    "documentation": "<p>The data type of the feature.</p>",
                     "shape": "FeatureType"
                 },
                 "LastModifiedTime": {
-                    "documentation": "<p>A timestamp indicating when the metadata for the feature group was modified. For example, if you add a parameter describing the feature, the timestamp changes to reflect the last time you </p>",
                     "shape": "LastModifiedTime"
                 },
                 "Parameters": {
-                    "documentation": "<p>The key-value pairs that you added to describe the feature.</p>",
                     "shape": "FeatureParameters"
                 }
             },
             "required": [
                 "FeatureGroupArn",
                 "FeatureGroupName",
                 "FeatureName",
@@ -12996,14 +13598,86 @@
                 "Version": {
                     "documentation": "<p>The version number.</p>",
                     "shape": "ImageVersionNumber"
                 }
             },
             "type": "structure"
         },
+        "DescribeInferenceExperimentRequest": {
+            "members": {
+                "Name": {
+                    "shape": "InferenceExperimentName"
+                }
+            },
+            "required": [
+                "Name"
+            ],
+            "type": "structure"
+        },
+        "DescribeInferenceExperimentResponse": {
+            "members": {
+                "Arn": {
+                    "shape": "InferenceExperimentArn"
+                },
+                "CompletionTime": {
+                    "shape": "Timestamp"
+                },
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "DataStorageConfig": {
+                    "shape": "InferenceExperimentDataStorageConfig"
+                },
+                "Description": {
+                    "shape": "InferenceExperimentDescription"
+                },
+                "EndpointMetadata": {
+                    "shape": "EndpointMetadata"
+                },
+                "KmsKey": {
+                    "shape": "KmsKeyId"
+                },
+                "LastModifiedTime": {
+                    "shape": "Timestamp"
+                },
+                "ModelVariants": {
+                    "shape": "ModelVariantConfigSummaryList"
+                },
+                "Name": {
+                    "shape": "InferenceExperimentName"
+                },
+                "RoleArn": {
+                    "shape": "RoleArn"
+                },
+                "Schedule": {
+                    "shape": "InferenceExperimentSchedule"
+                },
+                "ShadowModeConfig": {
+                    "shape": "ShadowModeConfig"
+                },
+                "Status": {
+                    "shape": "InferenceExperimentStatus"
+                },
+                "StatusReason": {
+                    "shape": "InferenceExperimentStatusReason"
+                },
+                "Type": {
+                    "shape": "InferenceExperimentType"
+                }
+            },
+            "required": [
+                "Arn",
+                "Name",
+                "Type",
+                "Status",
+                "EndpointMetadata",
+                "ModelVariants"
+            ],
+            "type": "structure"
+        },
         "DescribeInferenceRecommendationsJobRequest": {
             "members": {
                 "JobName": {
                     "documentation": "<p>The name of the job. The name must be unique within an Amazon Web Services Region in the Amazon Web Services account.</p>",
                     "shape": "RecommendationJobName"
                 }
             },
@@ -13019,15 +13693,14 @@
                     "shape": "Timestamp"
                 },
                 "CreationTime": {
                     "documentation": "<p>A timestamp that shows when the job was created.</p>",
                     "shape": "CreationTime"
                 },
                 "EndpointPerformances": {
-                    "documentation": "<p>The performance results from running an Inference Recommender job on an existing endpoint.</p>",
                     "shape": "EndpointPerformances"
                 },
                 "FailureReason": {
                     "documentation": "<p>If the job fails, provides information why the job failed.</p>",
                     "shape": "FailureReason"
                 },
                 "InferenceRecommendations": {
@@ -13154,15 +13827,15 @@
                     "shape": "Timestamp"
                 },
                 "OutputConfig": {
                     "documentation": "<p>The location of the job's output data and the Amazon Web Services Key Management Service key ID for the key used to encrypt the output data, if any.</p>",
                     "shape": "LabelingJobOutputConfig"
                 },
                 "RoleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) that SageMaker assumes to perform tasks on your behalf during data labeling.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) that Amazon SageMaker assumes to perform tasks on your behalf during data labeling.</p>",
                     "shape": "RoleArn"
                 },
                 "StoppingConditions": {
                     "documentation": "<p>A set of conditions for stopping a labeling job. If any of the conditions are met, the job is automatically stopped.</p>",
                     "shape": "LabelingJobStoppingConditions"
                 },
                 "Tags": {
@@ -13296,14 +13969,131 @@
                 "ModelBiasJobInput",
                 "ModelBiasJobOutputConfig",
                 "JobResources",
                 "RoleArn"
             ],
             "type": "structure"
         },
+        "DescribeModelCardExportJobRequest": {
+            "members": {
+                "ModelCardExportJobArn": {
+                    "shape": "ModelCardExportJobArn"
+                }
+            },
+            "required": [
+                "ModelCardExportJobArn"
+            ],
+            "type": "structure"
+        },
+        "DescribeModelCardExportJobResponse": {
+            "members": {
+                "CreatedAt": {
+                    "shape": "Timestamp"
+                },
+                "ExportArtifacts": {
+                    "shape": "ModelCardExportArtifacts"
+                },
+                "FailureReason": {
+                    "shape": "FailureReason"
+                },
+                "LastModifiedAt": {
+                    "shape": "Timestamp"
+                },
+                "ModelCardExportJobArn": {
+                    "shape": "ModelCardExportJobArn"
+                },
+                "ModelCardExportJobName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardVersion": {
+                    "shape": "Integer"
+                },
+                "OutputConfig": {
+                    "shape": "ModelCardExportOutputConfig"
+                },
+                "Status": {
+                    "shape": "ModelCardExportJobStatus"
+                }
+            },
+            "required": [
+                "ModelCardExportJobName",
+                "ModelCardExportJobArn",
+                "Status",
+                "ModelCardName",
+                "ModelCardVersion",
+                "OutputConfig",
+                "CreatedAt",
+                "LastModifiedAt"
+            ],
+            "type": "structure"
+        },
+        "DescribeModelCardRequest": {
+            "members": {
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardVersion": {
+                    "shape": "Integer"
+                }
+            },
+            "required": [
+                "ModelCardName"
+            ],
+            "type": "structure"
+        },
+        "DescribeModelCardResponse": {
+            "members": {
+                "Content": {
+                    "shape": "ModelCardContent"
+                },
+                "CreatedBy": {
+                    "shape": "UserContext"
+                },
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "LastModifiedBy": {
+                    "shape": "UserContext"
+                },
+                "LastModifiedTime": {
+                    "shape": "Timestamp"
+                },
+                "ModelCardArn": {
+                    "shape": "ModelCardArn"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardProcessingStatus": {
+                    "shape": "ModelCardProcessingStatus"
+                },
+                "ModelCardStatus": {
+                    "shape": "ModelCardStatus"
+                },
+                "ModelCardVersion": {
+                    "shape": "Integer"
+                },
+                "SecurityConfig": {
+                    "shape": "ModelCardSecurityConfig"
+                }
+            },
+            "required": [
+                "ModelCardArn",
+                "ModelCardName",
+                "ModelCardVersion",
+                "Content",
+                "ModelCardStatus",
+                "CreationTime",
+                "CreatedBy"
+            ],
+            "type": "structure"
+        },
         "DescribeModelExplainabilityJobDefinitionRequest": {
             "members": {
                 "JobDefinitionName": {
                     "documentation": "<p>The name of the model explainability job definition. The name must be unique within an Amazon Web Services Region in the Amazon Web Services account.</p>",
                     "shape": "MonitoringJobDefinitionName"
                 }
             },
@@ -13403,15 +14193,15 @@
                     "shape": "InferenceExecutionConfig"
                 },
                 "ModelArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the model.</p>",
                     "shape": "ModelArn"
                 },
                 "ModelName": {
-                    "documentation": "<p>Name of the SageMaker model.</p>",
+                    "documentation": "<p>Name of the Amazon SageMaker model.</p>",
                     "shape": "ModelName"
                 },
                 "PrimaryContainer": {
                     "documentation": "<p>The location of the primary inference code, associated artifacts, and custom environment map that the inference code uses when it is deployed in production. </p>",
                     "shape": "ContainerDefinition"
                 },
                 "VpcConfig": {
@@ -13426,15 +14216,15 @@
                 "ModelArn"
             ],
             "type": "structure"
         },
         "DescribeModelPackageGroupInput": {
             "members": {
                 "ModelPackageGroupName": {
-                    "documentation": "<p>The name of gthe model group to describe.</p>",
+                    "documentation": "<p>The name of the model group to describe.</p>",
                     "shape": "ArnOrName"
                 }
             },
             "required": [
                 "ModelPackageGroupName"
             ],
             "type": "structure"
@@ -13523,15 +14313,15 @@
                     "documentation": "<p>Details about inference jobs that can be run with models based on this model package.</p>",
                     "shape": "InferenceSpecification"
                 },
                 "LastModifiedBy": {
                     "shape": "UserContext"
                 },
                 "LastModifiedTime": {
-                    "documentation": "<p>The last time that the model package was modified.</p>",
+                    "documentation": "<p>The last time the model package was modified.</p>",
                     "shape": "Timestamp"
                 },
                 "MetadataProperties": {
                     "shape": "MetadataProperties"
                 },
                 "ModelApprovalStatus": {
                     "documentation": "<p>The approval status of the model package.</p>",
@@ -13784,63 +14574,62 @@
         "DescribeNotebookInstanceOutput": {
             "members": {
                 "AcceleratorTypes": {
                     "documentation": "<p>A list of the Elastic Inference (EI) instance types associated with this notebook instance. Currently only one EI instance type can be associated with a notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/ei.html\">Using Elastic Inference in Amazon SageMaker</a>.</p>",
                     "shape": "NotebookInstanceAcceleratorTypes"
                 },
                 "AdditionalCodeRepositories": {
-                    "documentation": "<p>An array of up to three Git repositories associated with the notebook instance. These can be either the names of Git repositories stored as resources in your account, or the URL of Git repositories in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. These repositories are cloned at the same level as the default repository of your notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with SageMaker Notebook Instances</a>.</p>",
+                    "documentation": "<p>An array of up to three Git repositories associated with the notebook instance. These can be either the names of Git repositories stored as resources in your account, or the URL of Git repositories in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. These repositories are cloned at the same level as the default repository of your notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with Amazon SageMaker Notebook Instances</a>.</p>",
                     "shape": "AdditionalCodeRepositoryNamesOrUrls"
                 },
                 "CreationTime": {
                     "documentation": "<p>A timestamp. Use this parameter to return the time when the notebook instance was created</p>",
                     "shape": "CreationTime"
                 },
                 "DefaultCodeRepository": {
-                    "documentation": "<p>The Git repository associated with the notebook instance as its default code repository. This can be either the name of a Git repository stored as a resource in your account, or the URL of a Git repository in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. When you open a notebook instance, it opens in the directory that contains this repository. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with SageMaker Notebook Instances</a>.</p>",
+                    "documentation": "<p>The Git repository associated with the notebook instance as its default code repository. This can be either the name of a Git repository stored as a resource in your account, or the URL of a Git repository in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. When you open a notebook instance, it opens in the directory that contains this repository. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with Amazon SageMaker Notebook Instances</a>.</p>",
                     "shape": "CodeRepositoryNameOrUrl"
                 },
                 "DirectInternetAccess": {
-                    "documentation": "<p>Describes whether SageMaker provides internet access to the notebook instance. If this value is set to <i>Disabled</i>, the notebook instance does not have internet access, and cannot connect to SageMaker training and endpoint services.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/appendix-additional-considerations.html#appendix-notebook-and-internet-access\">Notebook Instances Are Internet-Enabled by Default</a>.</p>",
+                    "documentation": "<p>Describes whether Amazon SageMaker provides internet access to the notebook instance. If this value is set to <i>Disabled</i>, the notebook instance does not have internet access, and cannot connect to Amazon SageMaker training and endpoint services.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/appendix-additional-considerations.html#appendix-notebook-and-internet-access\">Notebook Instances Are Internet-Enabled by Default</a>.</p>",
                     "shape": "DirectInternetAccess"
                 },
                 "FailureReason": {
                     "documentation": "<p>If status is <code>Failed</code>, the reason it failed.</p>",
                     "shape": "FailureReason"
                 },
                 "InstanceMetadataServiceConfiguration": {
-                    "documentation": "<p>Information on the IMDS configuration of the notebook instance</p>",
                     "shape": "InstanceMetadataServiceConfiguration"
                 },
                 "InstanceType": {
                     "documentation": "<p>The type of ML compute instance running on the notebook instance.</p>",
                     "shape": "InstanceType"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Web Services KMS key ID SageMaker uses to encrypt data when storing it on the ML storage volume attached to the instance. </p>",
+                    "documentation": "<p>The Amazon Web Services KMS key ID Amazon SageMaker uses to encrypt data when storing it on the ML storage volume attached to the instance. </p>",
                     "shape": "KmsKeyId"
                 },
                 "LastModifiedTime": {
                     "documentation": "<p>A timestamp. Use this parameter to retrieve the time when the notebook instance was last modified. </p>",
                     "shape": "LastModifiedTime"
                 },
                 "NetworkInterfaceId": {
-                    "documentation": "<p>The network interface IDs that SageMaker created at the time of creating the instance. </p>",
+                    "documentation": "<p>The network interface IDs that Amazon SageMaker created at the time of creating the instance. </p>",
                     "shape": "NetworkInterfaceId"
                 },
                 "NotebookInstanceArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the notebook instance.</p>",
                     "shape": "NotebookInstanceArn"
                 },
                 "NotebookInstanceLifecycleConfigName": {
                     "documentation": "<p>Returns the name of a notebook instance lifecycle configuration.</p> <p>For information about notebook instance lifestyle configurations, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/notebook-lifecycle-config.html\">Step 2.1: (Optional) Customize a Notebook Instance</a> </p>",
                     "shape": "NotebookInstanceLifecycleConfigName"
                 },
                 "NotebookInstanceName": {
-                    "documentation": "<p>The name of the SageMaker notebook instance. </p>",
+                    "documentation": "<p>The name of the Amazon SageMaker notebook instance. </p>",
                     "shape": "NotebookInstanceName"
                 },
                 "NotebookInstanceStatus": {
                     "documentation": "<p>The status of the notebook instance.</p>",
                     "shape": "NotebookInstanceStatus"
                 },
                 "PlatformIdentifier": {
@@ -13961,15 +14750,15 @@
             },
             "type": "structure"
         },
         "DescribePipelineRequest": {
             "members": {
                 "PipelineName": {
                     "documentation": "<p>The name of the pipeline to describe.</p>",
-                    "shape": "PipelineName"
+                    "shape": "PipelineNameOrArn"
                 }
             },
             "required": [
                 "PipelineName"
             ],
             "type": "structure"
         },
@@ -14200,14 +14989,61 @@
                 "ProjectId",
                 "ServiceCatalogProvisioningDetails",
                 "ProjectStatus",
                 "CreationTime"
             ],
             "type": "structure"
         },
+        "DescribeSpaceRequest": {
+            "members": {
+                "DomainId": {
+                    "shape": "DomainId"
+                },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                }
+            },
+            "required": [
+                "DomainId",
+                "SpaceName"
+            ],
+            "type": "structure"
+        },
+        "DescribeSpaceResponse": {
+            "members": {
+                "CreationTime": {
+                    "shape": "CreationTime"
+                },
+                "DomainId": {
+                    "shape": "DomainId"
+                },
+                "FailureReason": {
+                    "shape": "FailureReason"
+                },
+                "HomeEfsFileSystemUid": {
+                    "shape": "EfsUid"
+                },
+                "LastModifiedTime": {
+                    "shape": "LastModifiedTime"
+                },
+                "SpaceArn": {
+                    "shape": "SpaceArn"
+                },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                },
+                "SpaceSettings": {
+                    "shape": "SpaceSettings"
+                },
+                "Status": {
+                    "shape": "SpaceStatus"
+                }
+            },
+            "type": "structure"
+        },
         "DescribeStudioLifecycleConfigRequest": {
             "members": {
                 "StudioLifecycleConfigName": {
                     "documentation": "<p>The name of the Studio Lifecycle Configuration to describe.</p>",
                     "shape": "StudioLifecycleConfigName"
                 }
             },
@@ -14288,15 +15124,15 @@
                     "shape": "AlgorithmSpecification"
                 },
                 "AutoMLJobArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of an AutoML job.</p>",
                     "shape": "AutoMLJobArn"
                 },
                 "BillableTimeInSeconds": {
-                    "documentation": "<p>The billable time in seconds. Billable time refers to the absolute wall-clock time.</p> <p>Multiply <code>BillableTimeInSeconds</code> by the number of instances (<code>InstanceCount</code>) in your training cluster to get the total compute time SageMaker bills you if you run distributed training. The formula is as follows: <code>BillableTimeInSeconds * InstanceCount</code> .</p> <p>You can calculate the savings from using managed spot training using the formula <code>(1 - BillableTimeInSeconds / TrainingTimeInSeconds) * 100</code>. For example, if <code>BillableTimeInSeconds</code> is 100 and <code>TrainingTimeInSeconds</code> is 500, the savings is 80%.</p>",
+                    "documentation": "<p>The billable time in seconds. Billable time refers to the absolute wall-clock time.</p> <p>Multiply <code>BillableTimeInSeconds</code> by the number of instances (<code>InstanceCount</code>) in your training cluster to get the total compute time SageMaker will bill you if you run distributed training. The formula is as follows: <code>BillableTimeInSeconds * InstanceCount</code> .</p> <p>You can calculate the savings from using managed spot training using the formula <code>(1 - BillableTimeInSeconds / TrainingTimeInSeconds) * 100</code>. For example, if <code>BillableTimeInSeconds</code> is 100 and <code>TrainingTimeInSeconds</code> is 500, the savings is 80%.</p>",
                     "shape": "BillableTimeInSeconds"
                 },
                 "CheckpointConfig": {
                     "shape": "CheckpointConfig"
                 },
                 "CreationTime": {
                     "documentation": "<p>A timestamp that indicates when the training job was created.</p>",
@@ -14318,15 +15154,15 @@
                     "shape": "Boolean"
                 },
                 "EnableManagedSpotTraining": {
                     "documentation": "<p>A Boolean indicating whether managed spot training is enabled (<code>True</code>) or not (<code>False</code>).</p>",
                     "shape": "Boolean"
                 },
                 "EnableNetworkIsolation": {
-                    "documentation": "<p>If you want to allow inbound or outbound network calls, except for calls between peers within a training cluster for distributed training, choose <code>True</code>. If you enable network isolation for training jobs that are configured to use a VPC, SageMaker downloads and uploads customer data and model artifacts through the specified VPC, but the training container does not have network access.</p>",
+                    "documentation": "<p>If you want to allow inbound or outbound network calls, except for calls between peers within a training cluster for distributed training, choose <code>True</code>. If you enable network isolation for training jobs that are configured to use a VPC, Amazon SageMaker downloads and uploads customer data and model artifacts through the specified VPC, but the training container does not have network access.</p>",
                     "shape": "Boolean"
                 },
                 "Environment": {
                     "documentation": "<p>The environment variables to set in the Docker container.</p>",
                     "shape": "TrainingEnvironmentMap"
                 },
                 "ExperimentConfig": {
@@ -14345,27 +15181,27 @@
                     "shape": "HyperParameters"
                 },
                 "InputDataConfig": {
                     "documentation": "<p>An array of <code>Channel</code> objects that describes each data input channel. </p>",
                     "shape": "InputDataConfig"
                 },
                 "LabelingJobArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the SageMaker Ground Truth labeling job that created the transform or training job.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon SageMaker Ground Truth labeling job that created the transform or training job.</p>",
                     "shape": "LabelingJobArn"
                 },
                 "LastModifiedTime": {
                     "documentation": "<p>A timestamp that indicates when the status of the training job was last modified.</p>",
                     "shape": "Timestamp"
                 },
                 "ModelArtifacts": {
                     "documentation": "<p>Information about the Amazon S3 location that is configured for storing model artifacts. </p>",
                     "shape": "ModelArtifacts"
                 },
                 "OutputDataConfig": {
-                    "documentation": "<p>The S3 path where model artifacts that you configured when creating the job are stored. SageMaker creates subfolders for model artifacts. </p>",
+                    "documentation": "<p>The S3 path where model artifacts that you configured when creating the job are stored. Amazon SageMaker creates subfolders for model artifacts. </p>",
                     "shape": "OutputDataConfig"
                 },
                 "ProfilerConfig": {
                     "shape": "ProfilerConfig"
                 },
                 "ProfilerRuleConfigurations": {
                     "documentation": "<p>Configuration information for Debugger rules for profiling system and framework metrics.</p>",
@@ -14388,42 +15224,42 @@
                     "shape": "RetryStrategy"
                 },
                 "RoleArn": {
                     "documentation": "<p>The Amazon Web Services Identity and Access Management (IAM) role configured for the training job. </p>",
                     "shape": "RoleArn"
                 },
                 "SecondaryStatus": {
-                    "documentation": "<p> Provides detailed information about the state of the training job. For detailed information on the secondary status of the training job, see <code>StatusMessage</code> under <a>SecondaryStatusTransition</a>.</p> <p>SageMaker provides primary statuses and secondary statuses that apply to each of them:</p> <dl> <dt>InProgress</dt> <dd> <ul> <li> <p> <code>Starting</code> - Starting the training job.</p> </li> <li> <p> <code>Downloading</code> - An optional stage for algorithms that support <code>File</code> training input mode. It indicates that data is being downloaded to the ML storage volumes.</p> </li> <li> <p> <code>Training</code> - Training is in progress.</p> </li> <li> <p> <code>Interrupted</code> - The job stopped because the managed spot training instances were interrupted. </p> </li> <li> <p> <code>Uploading</code> - Training is complete and the model artifacts are being uploaded to the S3 location.</p> </li> </ul> </dd> <dt>Completed</dt> <dd> <ul> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> </ul> </dd> <dt>Failed</dt> <dd> <ul> <li> <p> <code>Failed</code> - The training job has failed. The reason for the failure is returned in the <code>FailureReason</code> field of <code>DescribeTrainingJobResponse</code>.</p> </li> </ul> </dd> <dt>Stopped</dt> <dd> <ul> <li> <p> <code>MaxRuntimeExceeded</code> - The job stopped because it exceeded the maximum allowed runtime.</p> </li> <li> <p> <code>MaxWaitTimeExceeded</code> - The job stopped because it exceeded the maximum allowed wait time.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> </dd> <dt>Stopping</dt> <dd> <ul> <li> <p> <code>Stopping</code> - Stopping the training job.</p> </li> </ul> </dd> </dl> <important> <p>Valid values for <code>SecondaryStatus</code> are subject to change. </p> </important> <p>We no longer support the following secondary statuses:</p> <ul> <li> <p> <code>LaunchingMLInstances</code> </p> </li> <li> <p> <code>PreparingTraining</code> </p> </li> <li> <p> <code>DownloadingTrainingImage</code> </p> </li> </ul>",
+                    "documentation": "<p> Provides detailed information about the state of the training job. For detailed information on the secondary status of the training job, see <code>StatusMessage</code> under <a>SecondaryStatusTransition</a>.</p> <p>Amazon SageMaker provides primary statuses and secondary statuses that apply to each of them:</p> <dl> <dt>InProgress</dt> <dd> <ul> <li> <p> <code>Starting</code> - Starting the training job.</p> </li> <li> <p> <code>Downloading</code> - An optional stage for algorithms that support <code>File</code> training input mode. It indicates that data is being downloaded to the ML storage volumes.</p> </li> <li> <p> <code>Training</code> - Training is in progress.</p> </li> <li> <p> <code>Interrupted</code> - The job stopped because the managed spot training instances were interrupted. </p> </li> <li> <p> <code>Uploading</code> - Training is complete and the model artifacts are being uploaded to the S3 location.</p> </li> </ul> </dd> <dt>Completed</dt> <dd> <ul> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> </ul> </dd> <dt>Failed</dt> <dd> <ul> <li> <p> <code>Failed</code> - The training job has failed. The reason for the failure is returned in the <code>FailureReason</code> field of <code>DescribeTrainingJobResponse</code>.</p> </li> </ul> </dd> <dt>Stopped</dt> <dd> <ul> <li> <p> <code>MaxRuntimeExceeded</code> - The job stopped because it exceeded the maximum allowed runtime.</p> </li> <li> <p> <code>MaxWaitTimeExceeded</code> - The job stopped because it exceeded the maximum allowed wait time.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> </dd> <dt>Stopping</dt> <dd> <ul> <li> <p> <code>Stopping</code> - Stopping the training job.</p> </li> </ul> </dd> </dl> <important> <p>Valid values for <code>SecondaryStatus</code> are subject to change. </p> </important> <p>We no longer support the following secondary statuses:</p> <ul> <li> <p> <code>LaunchingMLInstances</code> </p> </li> <li> <p> <code>PreparingTraining</code> </p> </li> <li> <p> <code>DownloadingTrainingImage</code> </p> </li> </ul>",
                     "shape": "SecondaryStatus"
                 },
                 "SecondaryStatusTransitions": {
                     "documentation": "<p>A history of all of the secondary statuses that the training job has transitioned through.</p>",
                     "shape": "SecondaryStatusTransitions"
                 },
                 "StoppingCondition": {
-                    "documentation": "<p>Specifies a limit to how long a model training job can run. It also specifies how long a managed Spot training job has to complete. When the job reaches the time limit, SageMaker ends the training job. Use this API to cap model training costs.</p> <p>To stop a job, SageMaker sends the algorithm the <code>SIGTERM</code> signal, which delays job termination for 120 seconds. Algorithms can use this 120-second window to save the model artifacts, so the results of training are not lost. </p>",
+                    "documentation": "<p>Specifies a limit to how long a model training job can run. It also specifies how long a managed Spot training job has to complete. When the job reaches the time limit, Amazon SageMaker ends the training job. Use this API to cap model training costs.</p> <p>To stop a job, Amazon SageMaker sends the algorithm the <code>SIGTERM</code> signal, which delays job termination for 120 seconds. Algorithms can use this 120-second window to save the model artifacts, so the results of training are not lost. </p>",
                     "shape": "StoppingCondition"
                 },
                 "TensorBoardOutputConfig": {
                     "shape": "TensorBoardOutputConfig"
                 },
                 "TrainingEndTime": {
-                    "documentation": "<p>Indicates the time when the training job ends on training instances. You are billed for the time interval between the value of <code>TrainingStartTime</code> and this time. For successful jobs and stopped jobs, this is the time after model artifacts are uploaded. For failed jobs, this is the time when SageMaker detects a job failure.</p>",
+                    "documentation": "<p>Indicates the time when the training job ends on training instances. You are billed for the time interval between the value of <code>TrainingStartTime</code> and this time. For successful jobs and stopped jobs, this is the time after model artifacts are uploaded. For failed jobs, this is the time when Amazon SageMaker detects a job failure.</p>",
                     "shape": "Timestamp"
                 },
                 "TrainingJobArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the training job.</p>",
                     "shape": "TrainingJobArn"
                 },
                 "TrainingJobName": {
                     "documentation": "<p> Name of the model training job. </p>",
                     "shape": "TrainingJobName"
                 },
                 "TrainingJobStatus": {
-                    "documentation": "<p>The status of the training job.</p> <p>SageMaker provides the following training job statuses:</p> <ul> <li> <p> <code>InProgress</code> - The training is in progress.</p> </li> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> <li> <p> <code>Failed</code> - The training job has failed. To see the reason for the failure, see the <code>FailureReason</code> field in the response to a <code>DescribeTrainingJobResponse</code> call.</p> </li> <li> <p> <code>Stopping</code> - The training job is stopping.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> <p>For more detailed information, see <code>SecondaryStatus</code>. </p>",
+                    "documentation": "<p>The status of the training job.</p> <p>Amazon SageMaker provides the following training job statuses:</p> <ul> <li> <p> <code>InProgress</code> - The training is in progress.</p> </li> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> <li> <p> <code>Failed</code> - The training job has failed. To see the reason for the failure, see the <code>FailureReason</code> field in the response to a <code>DescribeTrainingJobResponse</code> call.</p> </li> <li> <p> <code>Stopping</code> - The training job is stopping.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> <p>For more detailed information, see <code>SecondaryStatus</code>. </p>",
                     "shape": "TrainingJobStatus"
                 },
                 "TrainingStartTime": {
                     "documentation": "<p>Indicates the time when the training job starts on training instances. You are billed for the time interval between this time and the value of <code>TrainingEndTime</code>. The start time in CloudWatch Logs might be later than this time. The difference is due to the time it takes to download the training data and to the size of the training container.</p>",
                     "shape": "Timestamp"
                 },
                 "TrainingTimeInSeconds": {
@@ -14435,15 +15271,14 @@
                     "shape": "HyperParameterTuningJobArn"
                 },
                 "VpcConfig": {
                     "documentation": "<p>A <a>VpcConfig</a> object that specifies the VPC that this training job has access to. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/train-vpc.html\">Protect Training Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
                     "shape": "VpcConfig"
                 },
                 "WarmPoolStatus": {
-                    "documentation": "<p>The status of the warm pool associated with the training job.</p>",
                     "shape": "WarmPoolStatus"
                 }
             },
             "required": [
                 "TrainingJobName",
                 "TrainingJobArn",
                 "ModelArtifacts",
@@ -14479,15 +15314,14 @@
                     "shape": "BatchStrategy"
                 },
                 "CreationTime": {
                     "documentation": "<p>A timestamp that shows when the transform Job was created.</p>",
                     "shape": "Timestamp"
                 },
                 "DataCaptureConfig": {
-                    "documentation": "<p>Configuration to control how SageMaker captures inference data.</p>",
                     "shape": "BatchDataCaptureConfig"
                 },
                 "DataProcessing": {
                     "shape": "DataProcessing"
                 },
                 "Environment": {
                     "documentation": "<p>The environment variables to set in the Docker container. We support up to 16 key and values entries in the map.</p>",
@@ -14625,14 +15459,17 @@
                     "documentation": "<p>The hyperparameters of the component.</p>",
                     "shape": "TrialComponentParameters"
                 },
                 "Source": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the source and, optionally, the job type.</p>",
                     "shape": "TrialComponentSource"
                 },
+                "Sources": {
+                    "shape": "TrialComponentSources"
+                },
                 "StartTime": {
                     "documentation": "<p>When the component started.</p>",
                     "shape": "Timestamp"
                 },
                 "Status": {
                     "documentation": "<p>The status of the component. States include:</p> <ul> <li> <p>InProgress</p> </li> <li> <p>Completed</p> </li> <li> <p>Failed</p> </li> </ul>",
                     "shape": "TrialComponentStatus"
@@ -14740,19 +15577,19 @@
                     "shape": "EfsUid"
                 },
                 "LastModifiedTime": {
                     "documentation": "<p>The last modified time.</p>",
                     "shape": "LastModifiedTime"
                 },
                 "SingleSignOnUserIdentifier": {
-                    "documentation": "<p>The IAM Identity Center user identifier.</p>",
+                    "documentation": "<p>The SSO user identifier.</p>",
                     "shape": "SingleSignOnUserIdentifier"
                 },
                 "SingleSignOnUserValue": {
-                    "documentation": "<p>The IAM Identity Center user value.</p>",
+                    "documentation": "<p>The SSO user value.</p>",
                     "shape": "String256"
                 },
                 "Status": {
                     "documentation": "<p>The status.</p>",
                     "shape": "UserProfileStatus"
                 },
                 "UserProfileArn": {
@@ -14914,58 +15751,46 @@
         "DeviceDeploymentSummaries": {
             "member": {
                 "shape": "DeviceDeploymentSummary"
             },
             "type": "list"
         },
         "DeviceDeploymentSummary": {
-            "documentation": "<p>Contains information summarizing device details and deployment status.</p>",
             "members": {
                 "DeployedStageName": {
-                    "documentation": "<p>The name of the deployed stage.</p>",
                     "shape": "EntityName"
                 },
                 "DeploymentStartTime": {
-                    "documentation": "<p>The time when the deployment on the device started.</p>",
                     "shape": "Timestamp"
                 },
                 "Description": {
-                    "documentation": "<p>The description of the device.</p>",
                     "shape": "DeviceDescription"
                 },
                 "DeviceArn": {
-                    "documentation": "<p>The ARN of the device.</p>",
                     "shape": "DeviceArn"
                 },
                 "DeviceDeploymentStatus": {
-                    "documentation": "<p>The deployment status of the device.</p>",
                     "shape": "DeviceDeploymentStatus"
                 },
                 "DeviceDeploymentStatusMessage": {
-                    "documentation": "<p>The detailed error message for the deployoment status result.</p>",
                     "shape": "String"
                 },
                 "DeviceFleetName": {
-                    "documentation": "<p>The name of the fleet to which the device belongs to.</p>",
                     "shape": "EntityName"
                 },
                 "DeviceName": {
-                    "documentation": "<p>The name of the device.</p>",
                     "shape": "DeviceName"
                 },
                 "EdgeDeploymentPlanArn": {
-                    "documentation": "<p>The ARN of the edge deployment plan.</p>",
                     "shape": "EdgeDeploymentPlanArn"
                 },
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the edge deployment plan.</p>",
                     "shape": "EntityName"
                 },
                 "StageName": {
-                    "documentation": "<p>The name of the stage in the edge deployment plan.</p>",
                     "shape": "EntityName"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanArn",
                 "EdgeDeploymentPlanName",
                 "StageName",
@@ -15031,30 +15856,25 @@
         "DeviceNames": {
             "member": {
                 "shape": "DeviceName"
             },
             "type": "list"
         },
         "DeviceSelectionConfig": {
-            "documentation": "<p>Contains information about the configurations of selected devices.</p>",
             "members": {
                 "DeviceNameContains": {
-                    "documentation": "<p>A filter to select devices with names containing this name.</p>",
                     "shape": "DeviceName"
                 },
                 "DeviceNames": {
-                    "documentation": "<p>List of devices chosen to deploy.</p>",
                     "shape": "DeviceNames"
                 },
                 "DeviceSubsetType": {
-                    "documentation": "<p>Type of device subsets to deploy to the current stage.</p>",
                     "shape": "DeviceSubsetType"
                 },
                 "Percentage": {
-                    "documentation": "<p>Percentage of devices in the fleet to deploy to the current stage.</p>",
                     "shape": "Percentage"
                 }
             },
             "required": [
                 "DeviceSubsetType"
             ],
             "type": "structure"
@@ -15282,15 +16102,14 @@
             },
             "type": "list"
         },
         "DomainSettings": {
             "documentation": "<p>A collection of settings that apply to the <code>SageMaker Domain</code>. These settings are specified through the <code>CreateDomain</code> API call.</p>",
             "members": {
                 "ExecutionRoleIdentityConfig": {
-                    "documentation": "<p>The configuration for attaching a SageMaker user profile name to the execution role as a <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_control-access_monitor.html\">sts:SourceIdentity key</a>.</p>",
                     "shape": "ExecutionRoleIdentityConfig"
                 },
                 "RStudioServerProDomainSettings": {
                     "documentation": "<p>A collection of settings that configure the <code>RStudioServerPro</code> Domain-level app.</p>",
                     "shape": "RStudioServerProDomainSettings"
                 },
                 "SecurityGroupIds": {
@@ -15300,15 +16119,14 @@
             },
             "type": "structure"
         },
         "DomainSettingsForUpdate": {
             "documentation": "<p>A collection of <code>Domain</code> configuration settings to update.</p>",
             "members": {
                 "ExecutionRoleIdentityConfig": {
-                    "documentation": "<p>The configuration for attaching a SageMaker user profile name to the execution role as a <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_control-access_monitor.html\">sts:SourceIdentity key</a>. This configuration can only be modified if there are no apps in the <code>InService</code> or <code>Pending</code> state.</p>",
                     "shape": "ExecutionRoleIdentityConfig"
                 },
                 "RStudioServerProDomainSettingsForUpdate": {
                     "documentation": "<p>A collection of <code>RStudioServerPro</code> Domain-level app settings to update.</p>",
                     "shape": "RStudioServerProDomainSettingsForUpdate"
                 }
             },
@@ -15355,61 +16173,54 @@
             "documentation": "<p>Represents the drift check bias baselines that can be used when the model monitor is set using the model package.</p>",
             "members": {
                 "ConfigFile": {
                     "documentation": "<p>The bias config file for a model.</p>",
                     "shape": "FileSource"
                 },
                 "PostTrainingConstraints": {
-                    "documentation": "<p>The post-training constraints.</p>",
                     "shape": "MetricsSource"
                 },
                 "PreTrainingConstraints": {
-                    "documentation": "<p>The pre-training constraints.</p>",
                     "shape": "MetricsSource"
                 }
             },
             "type": "structure"
         },
         "DriftCheckExplainability": {
             "documentation": "<p>Represents the drift check explainability baselines that can be used when the model monitor is set using the model package. </p>",
             "members": {
                 "ConfigFile": {
                     "documentation": "<p>The explainability config file for the model.</p>",
                     "shape": "FileSource"
                 },
                 "Constraints": {
-                    "documentation": "<p>The drift check explainability constraints.</p>",
                     "shape": "MetricsSource"
                 }
             },
             "type": "structure"
         },
         "DriftCheckModelDataQuality": {
             "documentation": "<p>Represents the drift check data quality baselines that can be used when the model monitor is set using the model package. </p>",
             "members": {
                 "Constraints": {
-                    "documentation": "<p>The drift check model data quality constraints.</p>",
                     "shape": "MetricsSource"
                 },
                 "Statistics": {
-                    "documentation": "<p>The drift check model data quality statistics.</p>",
                     "shape": "MetricsSource"
                 }
             },
             "type": "structure"
         },
         "DriftCheckModelQuality": {
             "documentation": "<p>Represents the drift check model quality baselines that can be used when the model monitor is set using the model package. </p>",
             "members": {
                 "Constraints": {
-                    "documentation": "<p>The drift check model quality constraints.</p>",
                     "shape": "MetricsSource"
                 },
                 "Statistics": {
-                    "documentation": "<p>The drift check model quality statistics.</p>",
                     "shape": "MetricsSource"
                 }
             },
             "type": "structure"
         },
         "EMRStepMetadata": {
             "documentation": "<p>The configurations and outcomes of an Amazon EMR step execution.</p>",
@@ -15448,35 +16259,30 @@
                     "documentation": "<p>The Amazon Resource Name (ARN) of the source lineage entity of the directed edge.</p>",
                     "shape": "AssociationEntityArn"
                 }
             },
             "type": "structure"
         },
         "EdgeDeploymentConfig": {
-            "documentation": "<p>Contains information about the configuration of a deployment.</p>",
             "members": {
                 "FailureHandlingPolicy": {
-                    "documentation": "<p>Toggle that determines whether to rollback to previous configuration if the current deployment fails. By default this is turned on. You may turn this off if you want to investigate the errors yourself.</p>",
                     "shape": "FailureHandlingPolicy"
                 }
             },
             "required": [
                 "FailureHandlingPolicy"
             ],
             "type": "structure"
         },
         "EdgeDeploymentModelConfig": {
-            "documentation": "<p>Contains information about the configuration of a model in a deployment.</p>",
             "members": {
                 "EdgePackagingJobName": {
-                    "documentation": "<p>The edge packaging job associated with this deployment.</p>",
                     "shape": "EntityName"
                 },
                 "ModelHandle": {
-                    "documentation": "<p>The name the device application uses to reference this model.</p>",
                     "shape": "EntityName"
                 }
             },
             "required": [
                 "ModelHandle",
                 "EdgePackagingJobName"
             ],
@@ -15497,84 +16303,68 @@
         "EdgeDeploymentPlanSummaries": {
             "member": {
                 "shape": "EdgeDeploymentPlanSummary"
             },
             "type": "list"
         },
         "EdgeDeploymentPlanSummary": {
-            "documentation": "<p>Contains information summarizing an edge deployment plan.</p>",
             "members": {
                 "CreationTime": {
-                    "documentation": "<p>The time when the edge deployment plan was created.</p>",
                     "shape": "Timestamp"
                 },
                 "DeviceFleetName": {
-                    "documentation": "<p>The name of the device fleet used for the deployment. </p>",
                     "shape": "EntityName"
                 },
                 "EdgeDeploymentFailed": {
-                    "documentation": "<p>The number of edge devices that failed the deployment.</p>",
                     "shape": "Integer"
                 },
                 "EdgeDeploymentPending": {
-                    "documentation": "<p>The number of edge devices yet to pick up the deployment, or in progress.</p>",
                     "shape": "Integer"
                 },
                 "EdgeDeploymentPlanArn": {
-                    "documentation": "<p>The ARN of the edge deployment plan.</p>",
                     "shape": "EdgeDeploymentPlanArn"
                 },
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the edge deployment plan.</p>",
                     "shape": "EntityName"
                 },
                 "EdgeDeploymentSuccess": {
-                    "documentation": "<p>The number of edge devices with the successful deployment.</p>",
                     "shape": "Integer"
                 },
                 "LastModifiedTime": {
-                    "documentation": "<p>The time when the edge deployment plan was last updated.</p>",
                     "shape": "Timestamp"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanArn",
                 "EdgeDeploymentPlanName",
                 "DeviceFleetName",
                 "EdgeDeploymentSuccess",
                 "EdgeDeploymentPending",
                 "EdgeDeploymentFailed"
             ],
             "type": "structure"
         },
         "EdgeDeploymentStatus": {
-            "documentation": "<p>Contains information summarizing the deployment stage results.</p>",
             "members": {
                 "EdgeDeploymentFailedInStage": {
-                    "documentation": "<p>The number of edge devices that failed the deployment in current stage.</p>",
                     "shape": "Integer"
                 },
                 "EdgeDeploymentPendingInStage": {
-                    "documentation": "<p>The number of edge devices yet to pick up the deployment in current stage, or in progress.</p>",
                     "shape": "Integer"
                 },
                 "EdgeDeploymentStageStartTime": {
-                    "documentation": "<p>The time when the deployment API started.</p>",
                     "shape": "Timestamp"
                 },
                 "EdgeDeploymentStatusMessage": {
-                    "documentation": "<p>A detailed message about deployment status in current stage.</p>",
                     "shape": "String"
                 },
                 "EdgeDeploymentSuccessInStage": {
-                    "documentation": "<p>The number of edge devices with the successful deployment in the current stage.</p>",
                     "shape": "Integer"
                 },
                 "StageStatus": {
-                    "documentation": "<p>The general status of the current stage.</p>",
                     "shape": "StageStatus"
                 }
             },
             "required": [
                 "StageStatus",
                 "EdgeDeploymentSuccessInStage",
                 "EdgeDeploymentPendingInStage",
@@ -15885,14 +16675,17 @@
                     "documentation": "<p>A list of monitoring schedules for the endpoint. For information about model monitoring, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-monitor.html\">Amazon SageMaker Model Monitor</a>.</p>",
                     "shape": "MonitoringScheduleList"
                 },
                 "ProductionVariants": {
                     "documentation": "<p>A list of the production variants hosted on the endpoint. Each production variant is a model.</p>",
                     "shape": "ProductionVariantSummaryList"
                 },
+                "ShadowProductionVariants": {
+                    "shape": "ProductionVariantSummaryList"
+                },
                 "Tags": {
                     "documentation": "<p>A list of the tags associated with the endpoint. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a> in the <i>Amazon Web Services General Reference Guide</i>.</p>",
                     "shape": "TagList"
                 }
             },
             "required": [
                 "EndpointName",
@@ -15959,18 +16752,16 @@
         "EndpointConfigSummaryList": {
             "member": {
                 "shape": "EndpointConfigSummary"
             },
             "type": "list"
         },
         "EndpointInfo": {
-            "documentation": "<p>Details about a customer endpoint that was compared in an Inference Recommender job.</p>",
             "members": {
                 "EndpointName": {
-                    "documentation": "<p>The name of a customer's endpoint.</p>",
                     "shape": "EndpointName"
                 }
             },
             "required": [
                 "EndpointName"
             ],
             "type": "structure"
@@ -16050,14 +16841,34 @@
             "max": 10,
             "member": {
                 "shape": "EndpointInputConfiguration"
             },
             "min": 1,
             "type": "list"
         },
+        "EndpointMetadata": {
+            "members": {
+                "EndpointConfigName": {
+                    "shape": "EndpointConfigName"
+                },
+                "EndpointName": {
+                    "shape": "EndpointName"
+                },
+                "EndpointStatus": {
+                    "shape": "EndpointStatus"
+                },
+                "FailureReason": {
+                    "shape": "FailureReason"
+                }
+            },
+            "required": [
+                "EndpointName"
+            ],
+            "type": "structure"
+        },
         "EndpointName": {
             "max": 63,
             "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,62}",
             "type": "string"
         },
         "EndpointNameContains": {
             "max": 63,
@@ -16089,21 +16900,19 @@
                 "VariantName",
                 "InstanceType",
                 "InitialInstanceCount"
             ],
             "type": "structure"
         },
         "EndpointPerformance": {
-            "documentation": "<p>The performance results from running an Inference Recommender job on an existing endpoint.</p>",
             "members": {
                 "EndpointInfo": {
                     "shape": "EndpointInfo"
                 },
                 "Metrics": {
-                    "documentation": "<p>The metrics for an existing endpoint.</p>",
                     "shape": "InferenceMetrics"
                 }
             },
             "required": [
                 "Metrics",
                 "EndpointInfo"
             ],
@@ -16331,14 +17140,17 @@
         "ExperimentConfig": {
             "documentation": "<p>Associates a SageMaker job as a trial component with an experiment and trial. Specified when you call the following APIs:</p> <ul> <li> <p> <a>CreateProcessingJob</a> </p> </li> <li> <p> <a>CreateTrainingJob</a> </p> </li> <li> <p> <a>CreateTransformJob</a> </p> </li> </ul>",
             "members": {
                 "ExperimentName": {
                     "documentation": "<p>The name of an existing experiment to associate the trial component with.</p>",
                     "shape": "ExperimentEntityName"
                 },
+                "RunName": {
+                    "shape": "ExperimentEntityName"
+                },
                 "TrialComponentDisplayName": {
                     "documentation": "<p>The display name for the trial component. If this key isn't specified, the display name is the trial component name.</p>",
                     "shape": "ExperimentEntityName"
                 },
                 "TrialName": {
                     "documentation": "<p>The name of an existing trial to associate the trial component with. If not specified, a new trial is created.</p>",
                     "shape": "ExperimentEntityName"
@@ -16436,18 +17248,16 @@
             "type": "structure"
         },
         "ExplainabilityLocation": {
             "min": 1,
             "type": "string"
         },
         "ExplainerConfig": {
-            "documentation": "<p>A parameter to activate explainers.</p>",
             "members": {
                 "ClarifyExplainerConfig": {
-                    "documentation": "<p>A member of <code>ExplainerConfig</code> that contains configuration parameters for the SageMaker Clarify explainer.</p>",
                     "shape": "ClarifyExplainerConfig"
                 }
             },
             "type": "structure"
         },
         "FailStepMetadata": {
             "documentation": "<p>The container for the metadata for Fail step.</p>",
@@ -16538,19 +17348,17 @@
                     "shape": "FeatureGroupName"
                 },
                 "FeatureGroupStatus": {
                     "documentation": "<p>A <code>FeatureGroup</code> status.</p>",
                     "shape": "FeatureGroupStatus"
                 },
                 "LastModifiedTime": {
-                    "documentation": "<p>A timestamp indicating the last time you updated the feature group.</p>",
                     "shape": "LastModifiedTime"
                 },
                 "LastUpdateStatus": {
-                    "documentation": "<p>A value that indicates whether the feature group was updated successfully.</p>",
                     "shape": "LastUpdateStatus"
                 },
                 "OfflineStoreConfig": {
                     "shape": "OfflineStoreConfig"
                 },
                 "OfflineStoreStatus": {
                     "shape": "OfflineStoreStatus"
@@ -16654,66 +17462,54 @@
                 "FeatureGroupName",
                 "FeatureGroupArn",
                 "CreationTime"
             ],
             "type": "structure"
         },
         "FeatureMetadata": {
-            "documentation": "<p>The metadata for a feature. It can either be metadata that you specify, or metadata that is updated automatically.</p>",
             "members": {
                 "CreationTime": {
-                    "documentation": "<p>A timestamp indicating when the feature was created.</p>",
                     "shape": "CreationTime"
                 },
                 "Description": {
-                    "documentation": "<p>An optional description that you specify to better describe the feature.</p>",
                     "shape": "FeatureDescription"
                 },
                 "FeatureGroupArn": {
-                    "documentation": "<p>The Amazon Resource Number (ARN) of the feature group.</p>",
                     "shape": "FeatureGroupArn"
                 },
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group containing the feature.</p>",
                     "shape": "FeatureGroupName"
                 },
                 "FeatureName": {
-                    "documentation": "<p>The name of feature.</p>",
                     "shape": "FeatureName"
                 },
                 "FeatureType": {
-                    "documentation": "<p>The data type of the feature.</p>",
                     "shape": "FeatureType"
                 },
                 "LastModifiedTime": {
-                    "documentation": "<p>A timestamp indicating when the feature was last modified.</p>",
                     "shape": "LastModifiedTime"
                 },
                 "Parameters": {
-                    "documentation": "<p>Optional key-value pairs that you specify to better describe the feature.</p>",
                     "shape": "FeatureParameters"
                 }
             },
             "type": "structure"
         },
         "FeatureName": {
             "max": 64,
             "min": 1,
             "pattern": "^[a-zA-Z0-9]([-_]*[a-zA-Z0-9]){0,63}",
             "type": "string"
         },
         "FeatureParameter": {
-            "documentation": "<p>A key-value pair that you specify to describe the feature.</p>",
             "members": {
                 "Key": {
-                    "documentation": "<p>A key that must contain a value to describe the feature.</p>",
                     "shape": "FeatureParameterKey"
                 },
                 "Value": {
-                    "documentation": "<p>The value that belongs to a key.</p>",
                     "shape": "FeatureParameterValue"
                 }
             },
             "type": "structure"
         },
         "FeatureParameterAdditions": {
             "max": 25,
@@ -17377,15 +18173,15 @@
             "documentation": "<p>Information required for human workers to complete a labeling task.</p>",
             "members": {
                 "AnnotationConsolidationConfig": {
                     "documentation": "<p>Configures how labels are consolidated across human workers.</p>",
                     "shape": "AnnotationConsolidationConfig"
                 },
                 "MaxConcurrentTaskCount": {
-                    "documentation": "<p>Defines the maximum number of data objects that can be labeled by human workers at the same time. Also referred to as batch size. Each object may have more than one worker at one time. The default value is 1000 objects. To increase the maximum value to 5000 objects, contact Amazon Web Services Support.</p>",
+                    "documentation": "<p>Defines the maximum number of data objects that can be labeled by human workers at the same time. Also referred to as batch size. Each object may have more than one worker at one time. The default value is 1000 objects.</p>",
                     "shape": "MaxConcurrentTaskCount"
                 },
                 "NumberOfHumanWorkersPerDataObject": {
                     "documentation": "<p>The number of human workers that will label an object. </p>",
                     "shape": "NumberOfHumanWorkersPerDataObject"
                 },
                 "PreHumanTaskLambdaArn": {
@@ -17492,15 +18288,15 @@
                     "shape": "ArnOrName"
                 },
                 "MetricDefinitions": {
                     "documentation": "<p>An array of <a>MetricDefinition</a> objects that specify the metrics that the algorithm emits.</p>",
                     "shape": "MetricDefinitionList"
                 },
                 "TrainingImage": {
-                    "documentation": "<p> The registry path of the Docker image that contains the training algorithm. For information about Docker registry paths for built-in algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-algo-docker-registry-paths.html\">Algorithms Provided by Amazon SageMaker: Common Parameters</a>. SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>.</p>",
+                    "documentation": "<p> The registry path of the Docker image that contains the training algorithm. For information about Docker registry paths for built-in algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-algo-docker-registry-paths.html\">Algorithms Provided by Amazon SageMaker: Common Parameters</a>. Amazon SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>.</p>",
                     "shape": "AlgorithmImage"
                 },
                 "TrainingInputMode": {
                     "shape": "TrainingInputMode"
                 }
             },
             "required": [
@@ -17587,34 +18383,33 @@
                     "shape": "Boolean"
                 },
                 "EnableManagedSpotTraining": {
                     "documentation": "<p>A Boolean indicating whether managed spot training is enabled (<code>True</code>) or not (<code>False</code>).</p>",
                     "shape": "Boolean"
                 },
                 "EnableNetworkIsolation": {
-                    "documentation": "<p>Isolates the training container. No inbound or outbound network calls can be made, except for calls between peers within a training cluster for distributed training. If network isolation is used for training jobs that are configured to use a VPC, SageMaker downloads and uploads customer data and model artifacts through the specified VPC, but the training container does not have network access.</p>",
+                    "documentation": "<p>Isolates the training container. No inbound or outbound network calls can be made, except for calls between peers within a training cluster for distributed training. If network isolation is used for training jobs that are configured to use a VPC, Amazon SageMaker downloads and uploads customer data and model artifacts through the specified VPC, but the training container does not have network access.</p>",
                     "shape": "Boolean"
                 },
                 "HyperParameterRanges": {
                     "shape": "ParameterRanges"
                 },
                 "HyperParameterTuningResourceConfig": {
-                    "documentation": "<p>The configuration for the hyperparameter tuning resources, including the compute instances and storage volumes, used for training jobs launched by the tuning job. By default, storage volumes hold model artifacts and incremental states. Choose <code>File</code> for <code>TrainingInputMode</code> in the <code>AlgorithmSpecification</code> parameter to additionally store training data in the storage volume (optional).</p>",
                     "shape": "HyperParameterTuningResourceConfig"
                 },
                 "InputDataConfig": {
                     "documentation": "<p>An array of <a>Channel</a> objects that specify the input for the training jobs that the tuning job launches.</p>",
                     "shape": "InputDataConfig"
                 },
                 "OutputDataConfig": {
                     "documentation": "<p>Specifies the path to the Amazon S3 bucket where you store model artifacts from the training jobs that the tuning job launches.</p>",
                     "shape": "OutputDataConfig"
                 },
                 "ResourceConfig": {
-                    "documentation": "<p>The resources, including the compute instances and storage volumes, to use for the training jobs that the tuning job launches.</p> <p>Storage volumes store model artifacts and incremental states. Training algorithms might also use storage volumes for scratch space. If you want SageMaker to use the storage volume to store the training data, choose <code>File</code> as the <code>TrainingInputMode</code> in the algorithm specification. For distributed training algorithms, specify an instance count greater than 1.</p> <note> <p>If you want to use hyperparameter optimization with instance type flexibility, use <code>HyperParameterTuningResourceConfig</code> instead.</p> </note>",
+                    "documentation": "<p>The resources, including the compute instances and storage volumes, to use for the training jobs that the tuning job launches.</p> <p>Storage volumes store model artifacts and incremental states. Training algorithms might also use storage volumes for scratch space. If you want Amazon SageMaker to use the storage volume to store the training data, choose <code>File</code> as the <code>TrainingInputMode</code> in the algorithm specification. For distributed training algorithms, specify an instance count greater than 1.</p>",
                     "shape": "ResourceConfig"
                 },
                 "RetryStrategy": {
                     "documentation": "<p>The number of times to retry the job when the job fails due to an <code>InternalServerError</code>.</p>",
                     "shape": "RetryStrategy"
                 },
                 "RoleArn": {
@@ -17622,15 +18417,15 @@
                     "shape": "RoleArn"
                 },
                 "StaticHyperParameters": {
                     "documentation": "<p>Specifies the values of hyperparameters that do not change for the tuning job.</p>",
                     "shape": "HyperParameters"
                 },
                 "StoppingCondition": {
-                    "documentation": "<p>Specifies a limit to how long a model hyperparameter training job can run. It also specifies how long a managed spot training job has to complete. When the job reaches the time limit, SageMaker ends the training job. Use this API to cap model training costs.</p>",
+                    "documentation": "<p>Specifies a limit to how long a model hyperparameter training job can run. It also specifies how long a managed spot training job has to complete. When the job reaches the time limit, Amazon SageMaker ends the training job. Use this API to cap model training costs.</p>",
                     "shape": "StoppingCondition"
                 },
                 "TuningObjective": {
                     "shape": "HyperParameterTuningJobObjective"
                 },
                 "VpcConfig": {
                     "documentation": "<p>The <a>VpcConfig</a> object that specifies the VPC that you want the training jobs that this hyperparameter tuning job launches to connect to. Control access to and from your training container by configuring the VPC. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/train-vpc.html\">Protect Training Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
@@ -17662,15 +18457,15 @@
         "HyperParameterTrainingJobSummaries": {
             "member": {
                 "shape": "HyperParameterTrainingJobSummary"
             },
             "type": "list"
         },
         "HyperParameterTrainingJobSummary": {
-            "documentation": "<p>The container for the summary information about a training job.</p>",
+            "documentation": "<p>Specifies summary information about a training job.</p>",
             "members": {
                 "CreationTime": {
                     "documentation": "<p>The date and time that the training job was created.</p>",
                     "shape": "Timestamp"
                 },
                 "FailureReason": {
                     "documentation": "<p>The reason that the training job failed. </p>",
@@ -17681,15 +18476,15 @@
                     "shape": "FinalHyperParameterTuningJobObjectiveMetric"
                 },
                 "ObjectiveStatus": {
                     "documentation": "<p>The status of the objective metric for the training job:</p> <ul> <li> <p>Succeeded: The final objective metric for the training job was evaluated by the hyperparameter tuning job and used in the hyperparameter tuning process.</p> </li> </ul> <ul> <li> <p>Pending: The training job is in progress and evaluation of its final objective metric is pending.</p> </li> </ul> <ul> <li> <p>Failed: The final objective metric for the training job was not evaluated, and was not used in the hyperparameter tuning process. This typically occurs when the training job failed or did not emit an objective metric.</p> </li> </ul>",
                     "shape": "ObjectiveStatus"
                 },
                 "TrainingEndTime": {
-                    "documentation": "<p>Specifies the time when the training job ends on training instances. You are billed for the time interval between the value of <code>TrainingStartTime</code> and this time. For successful jobs and stopped jobs, this is the time after model artifacts are uploaded. For failed jobs, this is the time when SageMaker detects a job failure.</p>",
+                    "documentation": "<p>Specifies the time when the training job ends on training instances. You are billed for the time interval between the value of <code>TrainingStartTime</code> and this time. For successful jobs and stopped jobs, this is the time after model artifacts are uploaded. For failed jobs, this is the time when Amazon SageMaker detects a job failure.</p>",
                     "shape": "Timestamp"
                 },
                 "TrainingJobArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the training job.</p>",
                     "shape": "TrainingJobArn"
                 },
                 "TrainingJobDefinitionName": {
@@ -17729,26 +18524,22 @@
         "HyperParameterTuningAllocationStrategy": {
             "enum": [
                 "Prioritized"
             ],
             "type": "string"
         },
         "HyperParameterTuningInstanceConfig": {
-            "documentation": "<p>The configuration for hyperparameter tuning resources for use in training jobs launched by the tuning job. These resources include compute instances and storage volumes. Specify one or more compute instance configurations and allocation strategies to select resources (optional).</p>",
             "members": {
                 "InstanceCount": {
-                    "documentation": "<p>The number of instances of the type specified by <code>InstanceType</code>. Choose an instance count larger than 1 for distributed training algorithms. See <a href=\"https://docs.aws.amazon.com/data-parallel-use-api.html\">SageMaker distributed training jobs</a> for more information.</p>",
                     "shape": "TrainingInstanceCount"
                 },
                 "InstanceType": {
-                    "documentation": "<p>The instance type used for processing of hyperparameter optimization jobs. Choose from general purpose (no GPUs) instance types: ml.m5.xlarge, ml.m5.2xlarge, and ml.m5.4xlarge or compute optimized (no GPUs) instance types: ml.c5.xlarge and ml.c5.2xlarge. For more information about instance types, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-available-instance-types.html\">instance type descriptions</a>.</p>",
                     "shape": "TrainingInstanceType"
                 },
                 "VolumeSizeInGB": {
-                    "documentation": "<p>The volume size in GB of the data to be processed for hyperparameter optimization (optional).</p>",
                     "shape": "VolumeSizeInGB"
                 }
             },
             "required": [
                 "InstanceType",
                 "InstanceCount",
                 "VolumeSizeInGB"
@@ -17780,23 +18571,22 @@
                     "shape": "ParameterRanges"
                 },
                 "ResourceLimits": {
                     "documentation": "<p>The <a>ResourceLimits</a> object that specifies the maximum number of training jobs and parallel training jobs for this tuning job.</p>",
                     "shape": "ResourceLimits"
                 },
                 "Strategy": {
-                    "documentation": "<p>Specifies how hyperparameter tuning chooses the combinations of hyperparameter values to use for the training job it launches. For information about search strategies, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-how-it-works.html\">How Hyperparameter Tuning Works</a>.</p>",
+                    "documentation": "<p>Specifies how hyperparameter tuning chooses the combinations of hyperparameter values to use for the training job it launches. To use the Bayesian search strategy, set this to <code>Bayesian</code>. To randomly search, set it to <code>Random</code>. For information about search strategies, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-how-it-works.html\">How Hyperparameter Tuning Works</a>.</p>",
                     "shape": "HyperParameterTuningJobStrategyType"
                 },
                 "StrategyConfig": {
-                    "documentation": "<p>The configuration for the <code>Hyperband</code> optimization strategy. This parameter should be provided only if <code>Hyperband</code> is selected as the strategy for <code>HyperParameterTuningJobConfig</code>.</p>",
                     "shape": "HyperParameterTuningJobStrategyConfig"
                 },
                 "TrainingJobEarlyStoppingType": {
-                    "documentation": "<p>Specifies whether to use early stopping for training jobs launched by the hyperparameter tuning job. Because the <code>Hyperband</code> strategy has its own advanced internal early stopping mechanism, <code>TrainingJobEarlyStoppingType</code> must be <code>OFF</code> to use <code>Hyperband</code>. This parameter can take on one of the following values (the default value is <code>OFF</code>):</p> <dl> <dt>OFF</dt> <dd> <p>Training jobs launched by the hyperparameter tuning job do not use early stopping.</p> </dd> <dt>AUTO</dt> <dd> <p>SageMaker stops training jobs launched by the hyperparameter tuning job when they are unlikely to perform better than previously completed training jobs. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-early-stopping.html\">Stop Training Jobs Early</a>.</p> </dd> </dl>",
+                    "documentation": "<p>Specifies whether to use early stopping for training jobs launched by the hyperparameter tuning job. This can be one of the following values (the default value is <code>OFF</code>):</p> <dl> <dt>OFF</dt> <dd> <p>Training jobs launched by the hyperparameter tuning job do not use early stopping.</p> </dd> <dt>AUTO</dt> <dd> <p>Amazon SageMaker stops training jobs launched by the hyperparameter tuning job when they are unlikely to perform better than previously completed training jobs. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-early-stopping.html\">Stop Training Jobs Early</a>.</p> </dd> </dl>",
                     "shape": "TrainingJobEarlyStoppingType"
                 },
                 "TuningJobCompletionCriteria": {
                     "documentation": "<p>The tuning job's completion criteria.</p>",
                     "shape": "TuningJobCompletionCriteria"
                 }
             },
@@ -17840,65 +18630,55 @@
         "HyperParameterTuningJobObjectives": {
             "member": {
                 "shape": "HyperParameterTuningJobObjective"
             },
             "type": "list"
         },
         "HyperParameterTuningJobSearchEntity": {
-            "documentation": "<p>An entity returned by the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_SearchRecord.html\">SearchRecord</a> API containing the properties of a hyperparameter tuning job.</p>",
             "members": {
                 "BestTrainingJob": {
                     "shape": "HyperParameterTrainingJobSummary"
                 },
                 "CreationTime": {
-                    "documentation": "<p>The time that a hyperparameter tuning job was created.</p>",
                     "shape": "Timestamp"
                 },
                 "FailureReason": {
-                    "documentation": "<p>The error that was created when a hyperparameter tuning job failed.</p>",
                     "shape": "FailureReason"
                 },
                 "HyperParameterTuningEndTime": {
-                    "documentation": "<p>The time that a hyperparameter tuning job ended.</p>",
                     "shape": "Timestamp"
                 },
                 "HyperParameterTuningJobArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of a hyperparameter tuning job.</p>",
                     "shape": "HyperParameterTuningJobArn"
                 },
                 "HyperParameterTuningJobConfig": {
                     "shape": "HyperParameterTuningJobConfig"
                 },
                 "HyperParameterTuningJobName": {
-                    "documentation": "<p>The name of a hyperparameter tuning job.</p>",
                     "shape": "HyperParameterTuningJobName"
                 },
                 "HyperParameterTuningJobStatus": {
-                    "documentation": "<p>The status of a hyperparameter tuning job.</p>",
                     "shape": "HyperParameterTuningJobStatus"
                 },
                 "LastModifiedTime": {
-                    "documentation": "<p>The time that a hyperparameter tuning job was last modified.</p>",
                     "shape": "Timestamp"
                 },
                 "ObjectiveStatusCounters": {
                     "shape": "ObjectiveStatusCounters"
                 },
                 "OverallBestTrainingJob": {
                     "shape": "HyperParameterTrainingJobSummary"
                 },
                 "Tags": {
-                    "documentation": "<p>The tags associated with a hyperparameter tuning job. For more information see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>.</p>",
                     "shape": "TagList"
                 },
                 "TrainingJobDefinition": {
                     "shape": "HyperParameterTrainingJobDefinition"
                 },
                 "TrainingJobDefinitions": {
-                    "documentation": "<p>The job definitions included in a hyperparameter tuning job.</p>",
                     "shape": "HyperParameterTrainingJobDefinitions"
                 },
                 "TrainingJobStatusCounters": {
                     "shape": "TrainingJobStatusCounters"
                 },
                 "WarmStartConfig": {
                     "shape": "HyperParameterTuningJobWarmStartConfig"
@@ -17921,18 +18701,16 @@
                 "Failed",
                 "Stopped",
                 "Stopping"
             ],
             "type": "string"
         },
         "HyperParameterTuningJobStrategyConfig": {
-            "documentation": "<p>The configuration for a training job launched by a hyperparameter tuning job. Choose <code>Bayesian</code> for Bayesian optimization, and <code>Random</code> for random search optimization. For more advanced use cases, use <code>Hyperband</code>, which evaluates objective metrics for training jobs after every epoch. For more information about strategies, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-how-it-works.html\">How Hyperparameter Tuning Works</a>.</p>",
             "members": {
                 "HyperbandStrategyConfig": {
-                    "documentation": "<p>The configuration for the object that specifies the <code>Hyperband</code> strategy. This parameter is only supported for the <code>Hyperband</code> selection for <code>Strategy</code> within the <code>HyperParameterTuningJobConfig</code> API.</p>",
                     "shape": "HyperbandStrategyConfig"
                 }
             },
             "type": "structure"
         },
         "HyperParameterTuningJobStrategyType": {
             "documentation": "<p>The strategy hyperparameter tuning uses to find the best combination of hyperparameters for your model. Currently, the only supported value is <code>Bayesian</code>.</p>",
@@ -17982,15 +18760,15 @@
                     "shape": "ObjectiveStatusCounters"
                 },
                 "ResourceLimits": {
                     "documentation": "<p>The <a>ResourceLimits</a> object that specifies the maximum number of training jobs and parallel training jobs allowed for this tuning job.</p>",
                     "shape": "ResourceLimits"
                 },
                 "Strategy": {
-                    "documentation": "<p>Specifies the search strategy hyperparameter tuning uses to choose which hyperparameters to evaluate at each iteration.</p>",
+                    "documentation": "<p>Specifies the search strategy hyperparameter tuning uses to choose which hyperparameters to use for each iteration. Currently, the only valid value is Bayesian.</p>",
                     "shape": "HyperParameterTuningJobStrategyType"
                 },
                 "TrainingJobStatusCounters": {
                     "documentation": "<p>The <a>TrainingJobStatusCounters</a> object that specifies the numbers of training jobs, categorized by status, that this tuning job launched.</p>",
                     "shape": "TrainingJobStatusCounters"
                 }
             },
@@ -18027,38 +18805,31 @@
             "enum": [
                 "IdenticalDataAndAlgorithm",
                 "TransferLearning"
             ],
             "type": "string"
         },
         "HyperParameterTuningResourceConfig": {
-            "documentation": "<p>The configuration of resources, including compute instances and storage volumes for use in training jobs launched by hyperparameter tuning jobs. Specify one or more instance type and count and the allocation strategy for instance selection.</p> <note> <p> <code>HyperParameterTuningResourceConfig</code> supports all of the capabilities of ResourceConfig with added functionality for flexible instance management.</p> </note>",
             "members": {
                 "AllocationStrategy": {
-                    "documentation": "<p>The strategy that determines the order of preference for resources specified in <code>InstanceConfigs</code> used in hyperparameter optimization.</p>",
                     "shape": "HyperParameterTuningAllocationStrategy"
                 },
                 "InstanceConfigs": {
-                    "documentation": "<p>A list containing the configuration(s) for one or more resources for processing hyperparameter jobs. These resources include compute instances and storage volumes to use in model training jobs launched by hyperparameter tuning jobs. The <code>AllocationStrategy</code> controls the order in which multiple configurations provided in <code>InstanceConfigs</code> are used.</p> <note> <p>If you only want to use a single instance configuration inside the <code>HyperParameterTuningResourceConfig</code> API, do not provide a value for <code>InstanceConfigs</code>. Instead, use <code>InstanceType</code>, <code>VolumeSizeInGB</code> and <code>InstanceCount</code>. If you use <code>InstanceConfigs</code>, do not provide values for <code>InstanceType</code>, <code>VolumeSizeInGB</code> or <code>InstanceCount</code>.</p> </note>",
                     "shape": "HyperParameterTuningInstanceConfigs"
                 },
                 "InstanceCount": {
-                    "documentation": "<p>The number of compute instances of type <code>InstanceType</code> to use. For <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/data-parallel-use-api.html\">distributed training</a>, select a value greater than 1.</p>",
                     "shape": "TrainingInstanceCount"
                 },
                 "InstanceType": {
-                    "documentation": "<p>The instance type used to run hyperparameter optimization tuning jobs. See <a href=\"https://docs.aws.amazon.com/notebooks-available-instance-types.html\"> descriptions of instance types</a> for more information.</p>",
                     "shape": "TrainingInstanceType"
                 },
                 "VolumeKmsKeyId": {
-                    "documentation": "<p>A key used by Amazon Web Services Key Management Service to encrypt data on the storage volume attached to the compute instances used to run the training job. You can use either of the following formats to specify a key.</p> <p>KMS Key ID:</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> <p>Amazon Resource Name (ARN) of a KMS key:</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> <p>Some instances use local storage, which use a <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ssd-instance-store.html\">hardware module to encrypt</a> storage volumes. If you choose one of these instance types, you cannot request a <code>VolumeKmsKeyId</code>. For a list of instance types that use local storage, see <a href=\"http://aws.amazon.com/releasenotes/host-instance-storage-volumes-table/\">instance store volumes</a>. For more information about Amazon Web Services Key Management Service, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sms-security-kms-permissions.html\">KMS encryption</a> for more information.</p>",
                     "shape": "KmsKeyId"
                 },
                 "VolumeSizeInGB": {
-                    "documentation": "<p>The volume size in GB for the storage volume to be used in processing hyperparameter optimization jobs (optional). These volumes store model artifacts, incremental states and optionally, scratch space for training algorithms. Do not provide a value for this parameter if a value for <code>InstanceConfigs</code> is also specified.</p> <p>Some instance types have a fixed total local storage size. If you select one of these instances for training, <code>VolumeSizeInGB</code> cannot be greater than this total size. For a list of instance types with local instance storage and their sizes, see <a href=\"http://aws.amazon.com/releasenotes/host-instance-storage-volumes-table/\">instance store volumes</a>.</p> <note> <p>SageMaker supports only the <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-volume-types.html\">General Purpose SSD (gp2)</a> storage volume type.</p> </note>",
                     "shape": "OptionalVolumeSizeInGB"
                 }
             },
             "type": "structure"
         },
         "HyperParameterValue": {
             "max": 2500,
@@ -18073,22 +18844,19 @@
             "min": 0,
             "type": "map",
             "value": {
                 "shape": "HyperParameterValue"
             }
         },
         "HyperbandStrategyConfig": {
-            "documentation": "<p>The configuration for <code>Hyperband</code>, a multi-fidelity based hyperparameter tuning strategy. <code>Hyperband</code> uses the final and intermediate results of a training job to dynamically allocate resources to utilized hyperparameter configurations while automatically stopping under-performing configurations. This parameter should be provided only if <code>Hyperband</code> is selected as the <code>StrategyConfig</code> under the <code>HyperParameterTuningJobConfig</code> API.</p>",
             "members": {
                 "MaxResource": {
-                    "documentation": "<p>The maximum number of resources (such as epochs) that can be used by a training job launched by a hyperparameter tuning job. Once a job reaches the <code>MaxResource</code> value, it is stopped. If a value for <code>MaxResource</code> is not provided, and <code>Hyperband</code> is selected as the hyperparameter tuning strategy, <code>HyperbandTrainingJ</code> attempts to infer <code>MaxResource</code> from the following keys (if present) in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTrainingJobDefinition.html#sagemaker-Type-HyperParameterTrainingJobDefinition-StaticHyperParameters\">StaticsHyperParameters</a>:</p> <ul> <li> <p> <code>epochs</code> </p> </li> <li> <p> <code>numepochs</code> </p> </li> <li> <p> <code>n-epochs</code> </p> </li> <li> <p> <code>n_epochs</code> </p> </li> <li> <p> <code>num_epochs</code> </p> </li> </ul> <p>If <code>HyperbandStrategyConfig</code> is unable to infer a value for <code>MaxResource</code>, it generates a validation error. The maximum value is 20,000 epochs. All metrics that correspond to an objective metric are used to derive <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-early-stopping.html\">early stopping decisions</a>. For <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/distributed-training.html\">distributive</a> training jobs, ensure that duplicate metrics are not printed in the logs across the individual nodes in a training job. If multiple nodes are publishing duplicate or incorrect metrics, training jobs may make an incorrect stopping decision and stop the job prematurely. </p>",
                     "shape": "HyperbandStrategyMaxResource"
                 },
                 "MinResource": {
-                    "documentation": "<p>The minimum number of resources (such as epochs) that can be used by a training job launched by a hyperparameter tuning job. If the value for <code>MinResource</code> has not been reached, the training job will not be stopped by <code>Hyperband</code>.</p>",
                     "shape": "HyperbandStrategyMinResource"
                 }
             },
             "type": "structure"
         },
         "HyperbandStrategyMaxResource": {
             "min": 1,
@@ -18358,27 +19126,147 @@
         "InferenceExecutionMode": {
             "enum": [
                 "Serial",
                 "Direct"
             ],
             "type": "string"
         },
+        "InferenceExperimentArn": {
+            "max": 256,
+            "pattern": "arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:inference-experiment/.*",
+            "type": "string"
+        },
+        "InferenceExperimentDataStorageConfig": {
+            "members": {
+                "ContentType": {
+                    "shape": "CaptureContentTypeHeader"
+                },
+                "Destination": {
+                    "shape": "DestinationS3Uri"
+                },
+                "KmsKey": {
+                    "shape": "KmsKeyId"
+                }
+            },
+            "required": [
+                "Destination"
+            ],
+            "type": "structure"
+        },
+        "InferenceExperimentDescription": {
+            "max": 1024,
+            "pattern": ".*",
+            "type": "string"
+        },
+        "InferenceExperimentList": {
+            "member": {
+                "shape": "InferenceExperimentSummary"
+            },
+            "type": "list"
+        },
+        "InferenceExperimentName": {
+            "max": 120,
+            "min": 1,
+            "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,119}",
+            "type": "string"
+        },
+        "InferenceExperimentSchedule": {
+            "members": {
+                "EndTime": {
+                    "shape": "Timestamp"
+                },
+                "StartTime": {
+                    "shape": "Timestamp"
+                }
+            },
+            "type": "structure"
+        },
+        "InferenceExperimentStatus": {
+            "enum": [
+                "Creating",
+                "Created",
+                "Updating",
+                "Running",
+                "Starting",
+                "Stopping",
+                "Completed",
+                "Cancelled"
+            ],
+            "type": "string"
+        },
+        "InferenceExperimentStatusReason": {
+            "max": 1024,
+            "pattern": ".*",
+            "type": "string"
+        },
+        "InferenceExperimentStopDesiredState": {
+            "enum": [
+                "Completed",
+                "Cancelled"
+            ],
+            "type": "string"
+        },
+        "InferenceExperimentSummary": {
+            "members": {
+                "CompletionTime": {
+                    "shape": "Timestamp"
+                },
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "Description": {
+                    "shape": "InferenceExperimentDescription"
+                },
+                "LastModifiedTime": {
+                    "shape": "Timestamp"
+                },
+                "Name": {
+                    "shape": "InferenceExperimentName"
+                },
+                "RoleArn": {
+                    "shape": "RoleArn"
+                },
+                "Schedule": {
+                    "shape": "InferenceExperimentSchedule"
+                },
+                "Status": {
+                    "shape": "InferenceExperimentStatus"
+                },
+                "StatusReason": {
+                    "shape": "InferenceExperimentStatusReason"
+                },
+                "Type": {
+                    "shape": "InferenceExperimentType"
+                }
+            },
+            "required": [
+                "Name",
+                "Type",
+                "Status",
+                "CreationTime",
+                "LastModifiedTime"
+            ],
+            "type": "structure"
+        },
+        "InferenceExperimentType": {
+            "enum": [
+                "ShadowMode"
+            ],
+            "type": "string"
+        },
         "InferenceImage": {
             "max": 256,
             "type": "string"
         },
         "InferenceMetrics": {
-            "documentation": "<p>The metrics for an existing endpoint compared in an Inference Recommender job.</p>",
             "members": {
                 "MaxInvocations": {
-                    "documentation": "<p>The expected maximum number of requests per minute for the instance.</p>",
                     "shape": "Integer"
                 },
                 "ModelLatency": {
-                    "documentation": "<p>The expected model latency at maximum invocations per minute for the instance.</p>",
                     "shape": "Integer"
                 }
             },
             "required": [
                 "MaxInvocations",
                 "ModelLatency"
             ],
@@ -18468,30 +19356,25 @@
                 "CreationTime",
                 "RoleArn",
                 "LastModifiedTime"
             ],
             "type": "structure"
         },
         "InferenceRecommendationsJobStep": {
-            "documentation": "<p>A returned array object for the <code>Steps</code> response field in the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_InferenceRecommendationsJobStep.html\">ListInferenceRecommendationsJobSteps</a> API command.</p>",
             "members": {
                 "InferenceBenchmark": {
-                    "documentation": "<p>The details for a specific benchmark.</p>",
                     "shape": "RecommendationJobInferenceBenchmark"
                 },
                 "JobName": {
-                    "documentation": "<p>The name of the Inference Recommender job.</p>",
                     "shape": "RecommendationJobName"
                 },
                 "Status": {
-                    "documentation": "<p>The current status of the benchmark.</p>",
                     "shape": "RecommendationJobStatus"
                 },
                 "StepType": {
-                    "documentation": "<p>The type of the subtask.</p> <p> <code>BENCHMARK</code>: Evaluate the performance of your model on different instance types.</p>",
                     "shape": "RecommendationStepType"
                 }
             },
             "required": [
                 "StepType",
                 "JobName",
                 "Status"
@@ -18563,15 +19446,15 @@
                     "shape": "DataInputConfig"
                 },
                 "Framework": {
                     "documentation": "<p>Identifies the framework in which the model was trained. For example: TENSORFLOW.</p>",
                     "shape": "Framework"
                 },
                 "FrameworkVersion": {
-                    "documentation": "<p>Specifies the framework version to use. This API field is only supported for the MXNet, PyTorch, TensorFlow and TensorFlow Lite frameworks.</p> <p>For information about framework versions supported for cloud targets and edge devices, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/neo-supported-cloud.html\">Cloud Supported Instance Types and Frameworks</a> and <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/neo-supported-devices-edge-frameworks.html\">Edge Supported Frameworks</a>.</p>",
+                    "documentation": "<p>Specifies the framework version to use. This API field is only supported for the PyTorch and TensorFlow frameworks.</p> <p>For information about framework versions supported for cloud targets and edge devices, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/neo-supported-cloud.html\">Cloud Supported Instance Types and Frameworks</a> and <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/neo-supported-devices-edge-frameworks.html\">Edge Supported Frameworks</a>.</p>",
                     "shape": "FrameworkVersion"
                 },
                 "S3Uri": {
                     "documentation": "<p>The S3 path where the model artifacts, which result from model training, are stored. This path must point to a single gzip compressed tar archive (.tar.gz suffix).</p>",
                     "shape": "S3Uri"
                 }
             },
@@ -18601,26 +19484,22 @@
             "member": {
                 "shape": "TrainingInputMode"
             },
             "min": 1,
             "type": "list"
         },
         "InstanceGroup": {
-            "documentation": "<p>Defines an instance group for heterogeneous cluster training. When requesting a training job using the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrainingJob.html\">CreateTrainingJob</a> API, you can configure multiple instance groups .</p>",
             "members": {
                 "InstanceCount": {
-                    "documentation": "<p>Specifies the number of instances of the instance group.</p>",
                     "shape": "TrainingInstanceCount"
                 },
                 "InstanceGroupName": {
-                    "documentation": "<p>Specifies the name of the instance group.</p>",
                     "shape": "InstanceGroupName"
                 },
                 "InstanceType": {
-                    "documentation": "<p>Specifies the instance type of the instance group.</p>",
                     "shape": "TrainingInstanceType"
                 }
             },
             "required": [
                 "InstanceType",
                 "InstanceCount",
                 "InstanceGroupName"
@@ -18644,18 +19523,16 @@
             "max": 5,
             "member": {
                 "shape": "InstanceGroup"
             },
             "type": "list"
         },
         "InstanceMetadataServiceConfiguration": {
-            "documentation": "<p>Information on the IMDS configuration of the notebook instance</p>",
             "members": {
                 "MinimumInstanceMetadataServiceVersion": {
-                    "documentation": "<p>Indicates the minimum IMDS version that the notebook instance supports. When passed as part of <code>CreateNotebookInstance</code>, if no value is selected, then it defaults to IMDSv1. This means that both IMDSv1 and IMDSv2 are supported. If passed as part of <code>UpdateNotebookInstance</code>, there is no default.</p>",
                     "shape": "MinimumInstanceMetadataServiceVersion"
                 }
             },
             "required": [
                 "MinimumInstanceMetadataServiceVersion"
             ],
             "type": "structure"
@@ -18749,15 +19626,15 @@
                     "shape": "ParameterValue"
                 },
                 "Name": {
                     "documentation": "<p>The name of the hyperparameter to search.</p>",
                     "shape": "ParameterKey"
                 },
                 "ScalingType": {
-                    "documentation": "<p>The scale that hyperparameter tuning uses to search the hyperparameter range. For information about choosing a hyperparameter scale, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-define-ranges.html#scaling-type\">Hyperparameter Scaling</a>. One of the following values:</p> <dl> <dt>Auto</dt> <dd> <p>SageMaker hyperparameter tuning chooses the best scale for the hyperparameter.</p> </dd> <dt>Linear</dt> <dd> <p>Hyperparameter tuning searches the values in the hyperparameter range by using a linear scale.</p> </dd> <dt>Logarithmic</dt> <dd> <p>Hyperparameter tuning searches the values in the hyperparameter range by using a logarithmic scale.</p> <p>Logarithmic scaling works only for ranges that have only values greater than 0.</p> </dd> </dl>",
+                    "documentation": "<p>The scale that hyperparameter tuning uses to search the hyperparameter range. For information about choosing a hyperparameter scale, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-define-ranges.html#scaling-type\">Hyperparameter Scaling</a>. One of the following values:</p> <dl> <dt>Auto</dt> <dd> <p>Amazon SageMaker hyperparameter tuning chooses the best scale for the hyperparameter.</p> </dd> <dt>Linear</dt> <dd> <p>Hyperparameter tuning searches the values in the hyperparameter range by using a linear scale.</p> </dd> <dt>Logarithmic</dt> <dd> <p>Hyperparameter tuning searches the values in the hyperparameter range by using a logarithmic scale.</p> <p>Logarithmic scaling works only for ranges that have only values greater than 0.</p> </dd> </dl>",
                     "shape": "HyperParameterScalingType"
                 }
             },
             "required": [
                 "Name",
                 "MinValue",
                 "MaxValue"
@@ -18847,20 +19724,23 @@
             "max": 63,
             "min": 0,
             "type": "string"
         },
         "JupyterServerAppSettings": {
             "documentation": "<p>The JupyterServer app settings.</p>",
             "members": {
+                "CodeRepositories": {
+                    "shape": "CodeRepositories"
+                },
                 "DefaultResourceSpec": {
-                    "documentation": "<p>The default instance type and the Amazon Resource Name (ARN) of the default SageMaker image used by the JupyterServer app. If you use the <code>LifecycleConfigArns</code> parameter, then this parameter is also required.</p>",
+                    "documentation": "<p>The default instance type and the Amazon Resource Name (ARN) of the default SageMaker image used by the JupyterServer app.</p>",
                     "shape": "ResourceSpec"
                 },
                 "LifecycleConfigArns": {
-                    "documentation": "<p> The Amazon Resource Name (ARN) of the Lifecycle Configurations attached to the JupyterServerApp. If you use this parameter, the <code>DefaultResourceSpec</code> parameter is also required.</p> <note> <p>To remove a Lifecycle Config, you must set <code>LifecycleConfigArns</code> to an empty list.</p> </note>",
+                    "documentation": "<p> The Amazon Resource Name (ARN) of the Lifecycle Configurations attached to the JupyterServerApp.</p>",
                     "shape": "LifecycleConfigArns"
                 }
             },
             "type": "structure"
         },
         "KeepAlivePeriodInSeconds": {
             "max": 3600,
@@ -18875,19 +19755,19 @@
             "documentation": "<p>The KernelGateway app settings.</p>",
             "members": {
                 "CustomImages": {
                     "documentation": "<p>A list of custom SageMaker images that are configured to run as a KernelGateway app.</p>",
                     "shape": "CustomImages"
                 },
                 "DefaultResourceSpec": {
-                    "documentation": "<p>The default instance type and the Amazon Resource Name (ARN) of the default SageMaker image used by the KernelGateway app.</p> <note> <p>The Amazon SageMaker Studio UI does not use the default instance type value set here. The default instance type set here is used when Apps are created using the Amazon Web Services Command Line Interface or Amazon Web Services CloudFormation and the instance type parameter value is not passed.</p> </note>",
+                    "documentation": "<p>The default instance type and the Amazon Resource Name (ARN) of the default SageMaker image used by the KernelGateway app.</p>",
                     "shape": "ResourceSpec"
                 },
                 "LifecycleConfigArns": {
-                    "documentation": "<p> The Amazon Resource Name (ARN) of the Lifecycle Configurations attached to the the user profile or domain.</p> <note> <p>To remove a Lifecycle Config, you must set <code>LifecycleConfigArns</code> to an empty list.</p> </note>",
+                    "documentation": "<p> The Amazon Resource Name (ARN) of the Lifecycle Configurations attached to the the user profile or domain.</p>",
                     "shape": "LifecycleConfigArns"
                 }
             },
             "type": "structure"
         },
         "KernelGatewayImageConfig": {
             "documentation": "<p>The configuration for the file system and kernels in a SageMaker image running as a KernelGateway app.</p>",
@@ -19031,15 +19911,15 @@
             "pattern": "arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:labeling-job/.*",
             "type": "string"
         },
         "LabelingJobDataAttributes": {
             "documentation": "<p>Attributes of the data specified by the customer. Use these to describe the data to be labeled.</p>",
             "members": {
                 "ContentClassifiers": {
-                    "documentation": "<p>Declares that your content is free of personally identifiable information or adult content. SageMaker may restrict the Amazon Mechanical Turk workers that can view your task based on this information.</p>",
+                    "documentation": "<p>Declares that your content is free of personally identifiable information or adult content. Amazon SageMaker may restrict the Amazon Mechanical Turk workers that can view your task based on this information.</p>",
                     "shape": "ContentClassifiers"
                 }
             },
             "type": "structure"
         },
         "LabelingJobDataSource": {
             "documentation": "<p>Provides information about the location of input data.</p> <p>You must specify at least one of the following: <code>S3DataSource</code> or <code>SnsDataSource</code>.</p> <p>Use <code>SnsDataSource</code> to specify an SNS input topic for a streaming labeling job. If you do not specify and SNS input topic ARN, Ground Truth will create a one-time labeling job.</p> <p>Use <code>S3DataSource</code> to specify an input manifest file for both streaming and one-time labeling jobs. Adding an <code>S3DataSource</code> is optional if you use <code>SnsDataSource</code> to create a streaming labeling job.</p>",
@@ -19119,15 +19999,15 @@
             "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,62}",
             "type": "string"
         },
         "LabelingJobOutput": {
             "documentation": "<p>Specifies the location of the output produced by the labeling job. </p>",
             "members": {
                 "FinalActiveLearningModelArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) for the most recent SageMaker model trained as part of automated data labeling. </p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the most recent Amazon SageMaker model trained as part of automated data labeling. </p>",
                     "shape": "ModelArn"
                 },
                 "OutputDatasetS3Uri": {
                     "documentation": "<p>The Amazon S3 bucket location of the manifest file for labeled data. </p>",
                     "shape": "S3Uri"
                 }
             },
@@ -19310,22 +20190,19 @@
             },
             "type": "structure"
         },
         "LastModifiedTime": {
             "type": "timestamp"
         },
         "LastUpdateStatus": {
-            "documentation": "<p>A value that indicates whether the update was successful.</p>",
             "members": {
                 "FailureReason": {
-                    "documentation": "<p>If the update wasn't successful, indicates the reason why it failed.</p>",
                     "shape": "FailureReason"
                 },
                 "Status": {
-                    "documentation": "<p>A value that indicates whether the update was made successful.</p>",
                     "shape": "LastUpdateStatusValue"
                 }
             },
             "required": [
                 "Status"
             ],
             "type": "structure"
@@ -19492,15 +20369,15 @@
         "ListAlgorithmsOutput": {
             "members": {
                 "AlgorithmSummaryList": {
                     "documentation": "<p>&gt;An array of <code>AlgorithmSummary</code> objects, each of which lists an algorithm.</p>",
                     "shape": "AlgorithmSummaryList"
                 },
                 "NextToken": {
-                    "documentation": "<p>If the response is truncated, SageMaker returns this token. To retrieve the next set of algorithms, use it in the subsequent request.</p>",
+                    "documentation": "<p>If the response is truncated, Amazon SageMaker returns this token. To retrieve the next set of algorithms, use it in the subsequent request.</p>",
                     "shape": "NextToken"
                 }
             },
             "required": [
                 "AlgorithmSummaryList"
             ],
             "type": "structure"
@@ -19577,14 +20454,17 @@
                     "documentation": "<p>The parameter by which to sort the results. The default is CreationTime.</p>",
                     "shape": "AppSortKey"
                 },
                 "SortOrder": {
                     "documentation": "<p>The sort order for the results. The default is Ascending.</p>",
                     "shape": "SortOrder"
                 },
+                "SpaceNameEquals": {
+                    "shape": "SpaceName"
+                },
                 "UserProfileNameEquals": {
                     "documentation": "<p>A parameter to search by user profile name.</p>",
                     "shape": "UserProfileName"
                 }
             },
             "type": "structure"
         },
@@ -20191,65 +21071,53 @@
                 }
             },
             "type": "structure"
         },
         "ListEdgeDeploymentPlansRequest": {
             "members": {
                 "CreationTimeAfter": {
-                    "documentation": "<p>Selects edge deployment plans created after this time.</p>",
                     "shape": "Timestamp"
                 },
                 "CreationTimeBefore": {
-                    "documentation": "<p>Selects edge deployment plans created before this time.</p>",
                     "shape": "Timestamp"
                 },
                 "DeviceFleetNameContains": {
-                    "documentation": "<p>Selects edge deployment plans with a device fleet name containing this name.</p>",
                     "shape": "NameContains"
                 },
                 "LastModifiedTimeAfter": {
-                    "documentation": "<p>Selects edge deployment plans that were last updated after this time.</p>",
                     "shape": "Timestamp"
                 },
                 "LastModifiedTimeBefore": {
-                    "documentation": "<p>Selects edge deployment plans that were last updated before this time.</p>",
                     "shape": "Timestamp"
                 },
                 "MaxResults": {
                     "box": true,
-                    "documentation": "<p>The maximum number of results to select (50 by default).</p>",
                     "shape": "ListMaxResults"
                 },
                 "NameContains": {
-                    "documentation": "<p>Selects edge deployment plans with names containing this name.</p>",
                     "shape": "NameContains"
                 },
                 "NextToken": {
-                    "documentation": "<p>The response from the last list when returning a list large enough to need tokening.</p>",
                     "shape": "NextToken"
                 },
                 "SortBy": {
-                    "documentation": "<p>The column by which to sort the edge deployment plans. Can be one of <code>NAME</code>, <code>DEVICEFLEETNAME</code>, <code>CREATIONTIME</code>, <code>LASTMODIFIEDTIME</code>.</p>",
                     "shape": "ListEdgeDeploymentPlansSortBy"
                 },
                 "SortOrder": {
-                    "documentation": "<p>The direction of the sorting (ascending or descending).</p>",
                     "shape": "SortOrder"
                 }
             },
             "type": "structure"
         },
         "ListEdgeDeploymentPlansResponse": {
             "members": {
                 "EdgeDeploymentPlanSummaries": {
-                    "documentation": "<p>List of summaries of edge deployment plans.</p>",
                     "shape": "EdgeDeploymentPlanSummaries"
                 },
                 "NextToken": {
-                    "documentation": "<p>The token to use when calling the next page of results.</p>",
                     "shape": "NextToken"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanSummaries"
             ],
             "type": "structure"
@@ -20375,15 +21243,15 @@
         "ListEndpointConfigsOutput": {
             "members": {
                 "EndpointConfigs": {
                     "documentation": "<p>An array of endpoint configurations.</p>",
                     "shape": "EndpointConfigSummaryList"
                 },
                 "NextToken": {
-                    "documentation": "<p> If the response is truncated, SageMaker returns this token. To retrieve the next set of endpoint configurations, use it in the subsequent request </p>",
+                    "documentation": "<p> If the response is truncated, Amazon SageMaker returns this token. To retrieve the next set of endpoint configurations, use it in the subsequent request </p>",
                     "shape": "PaginationToken"
                 }
             },
             "required": [
                 "EndpointConfigs"
             ],
             "type": "structure"
@@ -20436,15 +21304,15 @@
         "ListEndpointsOutput": {
             "members": {
                 "Endpoints": {
                     "documentation": "<p> An array or endpoint objects. </p>",
                     "shape": "EndpointSummaryList"
                 },
                 "NextToken": {
-                    "documentation": "<p> If the response is truncated, SageMaker returns this token. To retrieve the next set of training jobs, use it in the subsequent request. </p>",
+                    "documentation": "<p> If the response is truncated, Amazon SageMaker returns this token. To retrieve the next set of training jobs, use it in the subsequent request. </p>",
                     "shape": "PaginationToken"
                 }
             },
             "required": [
                 "Endpoints"
             ],
             "type": "structure"
@@ -20802,50 +21670,92 @@
                 "NextToken": {
                     "documentation": "<p>A token for getting the next set of images, if there are any.</p>",
                     "shape": "NextToken"
                 }
             },
             "type": "structure"
         },
+        "ListInferenceExperimentsRequest": {
+            "members": {
+                "CreationTimeAfter": {
+                    "shape": "Timestamp"
+                },
+                "CreationTimeBefore": {
+                    "shape": "Timestamp"
+                },
+                "LastModifiedTimeAfter": {
+                    "shape": "Timestamp"
+                },
+                "LastModifiedTimeBefore": {
+                    "shape": "Timestamp"
+                },
+                "MaxResults": {
+                    "shape": "MaxResults"
+                },
+                "NameContains": {
+                    "shape": "NameContains"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                },
+                "SortBy": {
+                    "shape": "SortInferenceExperimentsBy"
+                },
+                "SortOrder": {
+                    "shape": "SortOrder"
+                },
+                "StatusEquals": {
+                    "shape": "InferenceExperimentStatus"
+                },
+                "Type": {
+                    "shape": "InferenceExperimentType"
+                }
+            },
+            "type": "structure"
+        },
+        "ListInferenceExperimentsResponse": {
+            "members": {
+                "InferenceExperiments": {
+                    "shape": "InferenceExperimentList"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "type": "structure"
+        },
         "ListInferenceRecommendationsJobStepsRequest": {
             "members": {
                 "JobName": {
-                    "documentation": "<p>The name for the Inference Recommender job.</p>",
                     "shape": "RecommendationJobName"
                 },
                 "MaxResults": {
-                    "documentation": "<p>The maximum number of results to return.</p>",
                     "shape": "MaxResults"
                 },
                 "NextToken": {
-                    "documentation": "<p>A token that you can specify to return more results from the list. Specify this field if you have a token that was returned from a previous request.</p>",
                     "shape": "NextToken"
                 },
                 "Status": {
-                    "documentation": "<p>A filter to return benchmarks of a specified status. If this field is left empty, then all benchmarks are returned.</p>",
                     "shape": "RecommendationJobStatus"
                 },
                 "StepType": {
-                    "documentation": "<p>A filter to return details about the specified type of subtask.</p> <p> <code>BENCHMARK</code>: Evaluate the performance of your model on different instance types.</p>",
                     "shape": "RecommendationStepType"
                 }
             },
             "required": [
                 "JobName"
             ],
             "type": "structure"
         },
         "ListInferenceRecommendationsJobStepsResponse": {
             "members": {
                 "NextToken": {
-                    "documentation": "<p>A token that you can specify in your next request to return more results from the list.</p>",
                     "shape": "NextToken"
                 },
                 "Steps": {
-                    "documentation": "<p>A list of all subtask details in Inference Recommender.</p>",
                     "shape": "InferenceRecommendationsJobSteps"
                 }
             },
             "type": "structure"
         },
         "ListInferenceRecommendationsJobsRequest": {
             "members": {
@@ -20959,15 +21869,15 @@
         "ListLabelingJobsForWorkteamResponse": {
             "members": {
                 "LabelingJobSummaryList": {
                     "documentation": "<p>An array of <code>LabelingJobSummary</code> objects, each describing a labeling job.</p>",
                     "shape": "LabelingJobForWorkteamSummaryList"
                 },
                 "NextToken": {
-                    "documentation": "<p>If the response is truncated, SageMaker returns this token. To retrieve the next set of labeling jobs, use it in the subsequent request.</p>",
+                    "documentation": "<p>If the response is truncated, Amazon SageMaker returns this token. To retrieve the next set of labeling jobs, use it in the subsequent request.</p>",
                     "shape": "NextToken"
                 }
             },
             "required": [
                 "LabelingJobSummaryList"
             ],
             "type": "structure"
@@ -21026,15 +21936,15 @@
         "ListLabelingJobsResponse": {
             "members": {
                 "LabelingJobSummaryList": {
                     "documentation": "<p>An array of <code>LabelingJobSummary</code> objects, each describing a labeling job.</p>",
                     "shape": "LabelingJobSummaryList"
                 },
                 "NextToken": {
-                    "documentation": "<p>If the response is truncated, SageMaker returns this token. To retrieve the next set of labeling jobs, use it in the subsequent request.</p>",
+                    "documentation": "<p>If the response is truncated, Amazon SageMaker returns this token. To retrieve the next set of labeling jobs, use it in the subsequent request.</p>",
                     "shape": "NextToken"
                 }
             },
             "type": "structure"
         },
         "ListLineageEntityParameterKey": {
             "member": {
@@ -21137,14 +22047,155 @@
                 }
             },
             "required": [
                 "JobDefinitionSummaries"
             ],
             "type": "structure"
         },
+        "ListModelCardExportJobsRequest": {
+            "members": {
+                "CreationTimeAfter": {
+                    "shape": "Timestamp"
+                },
+                "CreationTimeBefore": {
+                    "shape": "Timestamp"
+                },
+                "MaxResults": {
+                    "shape": "MaxResults"
+                },
+                "ModelCardExportJobNameContains": {
+                    "shape": "EntityName"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardVersion": {
+                    "shape": "Integer"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                },
+                "SortBy": {
+                    "shape": "ModelCardExportJobSortBy"
+                },
+                "SortOrder": {
+                    "shape": "ModelCardExportJobSortOrder"
+                },
+                "StatusEquals": {
+                    "shape": "ModelCardExportJobStatus"
+                }
+            },
+            "required": [
+                "ModelCardName"
+            ],
+            "type": "structure"
+        },
+        "ListModelCardExportJobsResponse": {
+            "members": {
+                "ModelCardExportJobSummaries": {
+                    "shape": "ModelCardExportJobSummaryList"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "required": [
+                "ModelCardExportJobSummaries"
+            ],
+            "type": "structure"
+        },
+        "ListModelCardVersionsRequest": {
+            "members": {
+                "CreationTimeAfter": {
+                    "shape": "Timestamp"
+                },
+                "CreationTimeBefore": {
+                    "shape": "Timestamp"
+                },
+                "MaxResults": {
+                    "shape": "MaxResults"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardStatus": {
+                    "shape": "ModelCardStatus"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                },
+                "SortBy": {
+                    "shape": "ModelCardVersionSortBy"
+                },
+                "SortOrder": {
+                    "shape": "ModelCardSortOrder"
+                }
+            },
+            "required": [
+                "ModelCardName"
+            ],
+            "type": "structure"
+        },
+        "ListModelCardVersionsResponse": {
+            "members": {
+                "ModelCardVersionSummaryList": {
+                    "shape": "ModelCardVersionSummaryList"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "required": [
+                "ModelCardVersionSummaryList"
+            ],
+            "type": "structure"
+        },
+        "ListModelCardsRequest": {
+            "members": {
+                "CreationTimeAfter": {
+                    "shape": "Timestamp"
+                },
+                "CreationTimeBefore": {
+                    "shape": "Timestamp"
+                },
+                "MaxResults": {
+                    "shape": "MaxResults"
+                },
+                "ModelCardStatus": {
+                    "shape": "ModelCardStatus"
+                },
+                "NameContains": {
+                    "shape": "EntityName"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                },
+                "SortBy": {
+                    "shape": "ModelCardSortBy"
+                },
+                "SortOrder": {
+                    "shape": "ModelCardSortOrder"
+                }
+            },
+            "type": "structure"
+        },
+        "ListModelCardsResponse": {
+            "members": {
+                "ModelCardSummaries": {
+                    "shape": "ModelCardSummaryList"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "required": [
+                "ModelCardSummaries"
+            ],
+            "type": "structure"
+        },
         "ListModelExplainabilityJobDefinitionsRequest": {
             "members": {
                 "CreationTimeAfter": {
                     "documentation": "<p>A filter that returns only model explainability jobs created after a specified time.</p>",
                     "shape": "Timestamp"
                 },
                 "CreationTimeBefore": {
@@ -21324,15 +22375,15 @@
         "ListModelPackagesOutput": {
             "members": {
                 "ModelPackageSummaryList": {
                     "documentation": "<p>An array of <code>ModelPackageSummary</code> objects, each of which lists a model package.</p>",
                     "shape": "ModelPackageSummaryList"
                 },
                 "NextToken": {
-                    "documentation": "<p>If the response is truncated, SageMaker returns this token. To retrieve the next set of model packages, use it in the subsequent request.</p>",
+                    "documentation": "<p>If the response is truncated, Amazon SageMaker returns this token. To retrieve the next set of model packages, use it in the subsequent request.</p>",
                     "shape": "NextToken"
                 }
             },
             "required": [
                 "ModelPackageSummaryList"
             ],
             "type": "structure"
@@ -21426,23 +22477,94 @@
         "ListModelsOutput": {
             "members": {
                 "Models": {
                     "documentation": "<p>An array of <code>ModelSummary</code> objects, each of which lists a model.</p>",
                     "shape": "ModelSummaryList"
                 },
                 "NextToken": {
-                    "documentation": "<p> If the response is truncated, SageMaker returns this token. To retrieve the next set of models, use it in the subsequent request. </p>",
+                    "documentation": "<p> If the response is truncated, Amazon SageMaker returns this token. To retrieve the next set of models, use it in the subsequent request. </p>",
                     "shape": "PaginationToken"
                 }
             },
             "required": [
                 "Models"
             ],
             "type": "structure"
         },
+        "ListMonitoringAlertHistoryRequest": {
+            "members": {
+                "CreationTimeAfter": {
+                    "shape": "Timestamp"
+                },
+                "CreationTimeBefore": {
+                    "shape": "Timestamp"
+                },
+                "MaxResults": {
+                    "shape": "MaxResults"
+                },
+                "MonitoringAlertName": {
+                    "shape": "MonitoringAlertName"
+                },
+                "MonitoringScheduleName": {
+                    "shape": "MonitoringScheduleName"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                },
+                "SortBy": {
+                    "shape": "MonitoringAlertHistorySortKey"
+                },
+                "SortOrder": {
+                    "shape": "SortOrder"
+                },
+                "StatusEquals": {
+                    "shape": "MonitoringAlertStatus"
+                }
+            },
+            "type": "structure"
+        },
+        "ListMonitoringAlertHistoryResponse": {
+            "members": {
+                "MonitoringAlertHistory": {
+                    "shape": "MonitoringAlertHistoryList"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "type": "structure"
+        },
+        "ListMonitoringAlertsRequest": {
+            "members": {
+                "MaxResults": {
+                    "shape": "MaxResults"
+                },
+                "MonitoringScheduleName": {
+                    "shape": "MonitoringScheduleName"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "required": [
+                "MonitoringScheduleName"
+            ],
+            "type": "structure"
+        },
+        "ListMonitoringAlertsResponse": {
+            "members": {
+                "MonitoringAlertSummaries": {
+                    "shape": "MonitoringAlertSummaryList"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "type": "structure"
+        },
         "ListMonitoringExecutionsRequest": {
             "members": {
                 "CreationTimeAfter": {
                     "documentation": "<p>A filter that returns only jobs created after a specified time.</p>",
                     "shape": "Timestamp"
                 },
                 "CreationTimeBefore": {
@@ -21633,15 +22755,15 @@
                 }
             },
             "type": "structure"
         },
         "ListNotebookInstanceLifecycleConfigsOutput": {
             "members": {
                 "NextToken": {
-                    "documentation": "<p>If the response is truncated, SageMaker returns this token. To get the next set of lifecycle configurations, use it in the next request. </p>",
+                    "documentation": "<p>If the response is truncated, Amazon SageMaker returns this token. To get the next set of lifecycle configurations, use it in the next request. </p>",
                     "shape": "NextToken"
                 },
                 "NotebookInstanceLifecycleConfigs": {
                     "documentation": "<p>An array of <code>NotebookInstanceLifecycleConfiguration</code> objects, each listing a lifecycle configuration.</p>",
                     "shape": "NotebookInstanceLifecycleConfigSummaryList"
                 }
             },
@@ -21703,15 +22825,15 @@
                 }
             },
             "type": "structure"
         },
         "ListNotebookInstancesOutput": {
             "members": {
                 "NextToken": {
-                    "documentation": "<p>If the response to the previous <code>ListNotebookInstances</code> request was truncated, SageMaker returns this token. To retrieve the next set of notebook instances, use the token in the next request.</p>",
+                    "documentation": "<p>If the response to the previous <code>ListNotebookInstances</code> request was truncated, Amazon SageMaker returns this token. To retrieve the next set of notebook instances, use the token in the next request.</p>",
                     "shape": "NextToken"
                 },
                 "NotebookInstances": {
                     "documentation": "<p>An array of <code>NotebookInstanceSummary</code> objects, one for each notebook instance.</p>",
                     "shape": "NotebookInstanceSummaryList"
                 }
             },
@@ -21767,15 +22889,15 @@
                 },
                 "NextToken": {
                     "documentation": "<p>If the result of the previous <code>ListPipelineExecutions</code> request was truncated, the response includes a <code>NextToken</code>. To retrieve the next set of pipeline executions, use the token in the next request.</p>",
                     "shape": "NextToken"
                 },
                 "PipelineName": {
                     "documentation": "<p>The name of the pipeline.</p>",
-                    "shape": "PipelineName"
+                    "shape": "PipelineNameOrArn"
                 },
                 "SortBy": {
                     "documentation": "<p>The field by which to sort results. The default is <code>CreatedTime</code>.</p>",
                     "shape": "SortPipelineExecutionsBy"
                 },
                 "SortOrder": {
                     "documentation": "<p>The sort order for results.</p>",
@@ -21986,52 +23108,79 @@
                 }
             },
             "required": [
                 "ProjectSummaryList"
             ],
             "type": "structure"
         },
+        "ListSpacesRequest": {
+            "members": {
+                "DomainIdEquals": {
+                    "shape": "DomainId"
+                },
+                "MaxResults": {
+                    "shape": "MaxResults"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                },
+                "SortBy": {
+                    "shape": "SpaceSortKey"
+                },
+                "SortOrder": {
+                    "shape": "SortOrder"
+                },
+                "SpaceNameContains": {
+                    "shape": "SpaceName"
+                }
+            },
+            "type": "structure"
+        },
+        "ListSpacesResponse": {
+            "members": {
+                "NextToken": {
+                    "shape": "NextToken"
+                },
+                "Spaces": {
+                    "shape": "SpaceList"
+                }
+            },
+            "type": "structure"
+        },
         "ListStageDevicesRequest": {
             "members": {
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the edge deployment plan.</p>",
                     "shape": "EntityName"
                 },
                 "ExcludeDevicesDeployedInOtherStage": {
-                    "documentation": "<p>Toggle for excluding devices deployed in other stages.</p>",
                     "shape": "Boolean"
                 },
                 "MaxResults": {
                     "box": true,
-                    "documentation": "<p>The maximum number of requests to select.</p>",
                     "shape": "ListMaxResults"
                 },
                 "NextToken": {
-                    "documentation": "<p>The response from the last list when returning a list large enough to neeed tokening.</p>",
                     "shape": "NextToken"
                 },
                 "StageName": {
-                    "documentation": "<p>The name of the stage in the deployment.</p>",
                     "shape": "EntityName"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanName",
                 "StageName"
             ],
             "type": "structure"
         },
         "ListStageDevicesResponse": {
             "members": {
                 "DeviceDeploymentSummaries": {
-                    "documentation": "<p>List of summaries of devices allocated to the stage.</p>",
                     "shape": "DeviceDeploymentSummaries"
                 },
                 "NextToken": {
-                    "documentation": "<p>The token to use when calling the next page of results.</p>",
                     "shape": "NextToken"
                 }
             },
             "required": [
                 "DeviceDeploymentSummaries"
             ],
             "type": "structure"
@@ -22131,15 +23280,15 @@
         "ListTagsInput": {
             "members": {
                 "MaxResults": {
                     "documentation": "<p>Maximum number of tags to return.</p>",
                     "shape": "ListTagsMaxResults"
                 },
                 "NextToken": {
-                    "documentation": "<p> If the response to the previous <code>ListTags</code> request is truncated, SageMaker returns this token. To retrieve the next set of tags, use it in the subsequent request. </p>",
+                    "documentation": "<p> If the response to the previous <code>ListTags</code> request is truncated, Amazon SageMaker returns this token. To retrieve the next set of tags, use it in the subsequent request. </p>",
                     "shape": "NextToken"
                 },
                 "ResourceArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the resource whose tags you want to retrieve.</p>",
                     "shape": "ResourceArn"
                 }
             },
@@ -22151,15 +23300,15 @@
         "ListTagsMaxResults": {
             "min": 50,
             "type": "integer"
         },
         "ListTagsOutput": {
             "members": {
                 "NextToken": {
-                    "documentation": "<p> If response is truncated, SageMaker includes a token in the response. You can use this token in your subsequent request to fetch next set of tokens. </p>",
+                    "documentation": "<p> If response is truncated, Amazon SageMaker includes a token in the response. You can use this token in your subsequent request to fetch next set of tokens. </p>",
                     "shape": "NextToken"
                 },
                 "Tags": {
                     "documentation": "<p>An array of <code>Tag</code> objects, each with a tag key and a value.</p>",
                     "shape": "TagList"
                 }
             },
@@ -22253,24 +23402,23 @@
                     "shape": "SortOrder"
                 },
                 "StatusEquals": {
                     "documentation": "<p>A filter that retrieves only training jobs with a specific status.</p>",
                     "shape": "TrainingJobStatus"
                 },
                 "WarmPoolStatusEquals": {
-                    "documentation": "<p>A filter that retrieves only training jobs with a specific warm pool status.</p>",
                     "shape": "WarmPoolResourceStatus"
                 }
             },
             "type": "structure"
         },
         "ListTrainingJobsResponse": {
             "members": {
                 "NextToken": {
-                    "documentation": "<p>If the response is truncated, SageMaker returns this token. To retrieve the next set of training jobs, use it in the subsequent request.</p>",
+                    "documentation": "<p>If the response is truncated, Amazon SageMaker returns this token. To retrieve the next set of training jobs, use it in the subsequent request.</p>",
                     "shape": "NextToken"
                 },
                 "TrainingJobSummaries": {
                     "documentation": "<p>An array of <code>TrainingJobSummary</code> objects, each listing a training job.</p>",
                     "shape": "TrainingJobSummaries"
                 }
             },
@@ -22764,26 +23912,25 @@
                     "shape": "AutoMLMetricEnum"
                 },
                 "Set": {
                     "documentation": "<p>The dataset split from which the AutoML job produced the metric.</p>",
                     "shape": "MetricSetSource"
                 },
                 "StandardMetricName": {
-                    "documentation": "<p>The name of the standard metric. </p> <note> <p>For definitions of the standard metrics, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-metrics\"> <code>Autopilot candidate metrics</code> </a>.</p> </note>",
                     "shape": "AutoMLMetricExtendedEnum"
                 },
                 "Value": {
                     "documentation": "<p>The value of the metric.</p>",
                     "shape": "Float"
                 }
             },
             "type": "structure"
         },
         "MetricDefinition": {
-            "documentation": "<p>Specifies a metric that the training algorithm writes to <code>stderr</code> or <code>stdout</code>. SageMakerhyperparameter tuning captures all defined metrics. You specify one metric that a hyperparameter tuning job uses as its objective metric to choose the best training job.</p>",
+            "documentation": "<p>Specifies a metric that the training algorithm writes to <code>stderr</code> or <code>stdout</code>. Amazon SageMakerhyperparameter tuning captures all defined metrics. You specify one metric that a hyperparameter tuning job uses as its objective metric to choose the best training job.</p>",
             "members": {
                 "Name": {
                     "documentation": "<p>The name of the metric.</p>",
                     "shape": "MetricName"
                 },
                 "Regex": {
                     "documentation": "<p>A regular expression that searches the output of a training job and gets the value of the metric. For more information about using regular expressions to define metrics, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-define-metrics.html\">Defining Objective Metrics</a>.</p>",
@@ -22824,40 +23971,75 @@
             ],
             "type": "string"
         },
         "MetricValue": {
             "type": "float"
         },
         "MetricsSource": {
-            "documentation": "<p>Details about the metrics source.</p>",
+            "documentation": "<p/>",
             "members": {
                 "ContentDigest": {
-                    "documentation": "<p>The hash key used for the metrics source.</p>",
+                    "documentation": "<p/>",
                     "shape": "ContentDigest"
                 },
                 "ContentType": {
-                    "documentation": "<p>The metric source content type.</p>",
+                    "documentation": "<p/>",
                     "shape": "ContentType"
                 },
                 "S3Uri": {
-                    "documentation": "<p>The S3 URI for the metrics source.</p>",
+                    "documentation": "<p/>",
                     "shape": "S3Uri"
                 }
             },
             "required": [
                 "ContentType",
                 "S3Uri"
             ],
             "type": "structure"
         },
         "MinimumInstanceMetadataServiceVersion": {
             "max": 1,
             "pattern": "1|2",
             "type": "string"
         },
+        "Model": {
+            "members": {
+                "Containers": {
+                    "shape": "ContainerDefinitionList"
+                },
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "EnableNetworkIsolation": {
+                    "shape": "Boolean"
+                },
+                "ExecutionRoleArn": {
+                    "shape": "RoleArn"
+                },
+                "InferenceExecutionConfig": {
+                    "shape": "InferenceExecutionConfig"
+                },
+                "ModelArn": {
+                    "shape": "ModelArn"
+                },
+                "ModelName": {
+                    "shape": "ModelName"
+                },
+                "PrimaryContainer": {
+                    "shape": "ContainerDefinition"
+                },
+                "Tags": {
+                    "shape": "TagList"
+                },
+                "VpcConfig": {
+                    "shape": "VpcConfig"
+                }
+            },
+            "type": "structure"
+        },
         "ModelApprovalStatus": {
             "enum": [
                 "Approved",
                 "Rejected",
                 "PendingManualApproval"
             ],
             "type": "string"
@@ -22881,15 +24063,15 @@
             ],
             "type": "structure"
         },
         "ModelBiasAppSpecification": {
             "documentation": "<p>Docker container image configuration object for the model bias job.</p>",
             "members": {
                 "ConfigUri": {
-                    "documentation": "<p>JSON formatted S3 file that defines bias parameters. For more information on this JSON configuration file, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-config-json-monitor-bias-parameters.html\">Configure bias parameters</a>.</p>",
+                    "documentation": "<p>JSON formatted S3 file that defines bias parameters. For more information on this JSON configuration file, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/json-bias-parameter-config.html\">Configure bias parameters</a>.</p>",
                     "shape": "S3Uri"
                 },
                 "Environment": {
                     "documentation": "<p>Sets the environment variables in the Docker container.</p>",
                     "shape": "MonitoringEnvironmentMap"
                 },
                 "ImageUri": {
@@ -22916,15 +24098,14 @@
             },
             "type": "structure"
         },
         "ModelBiasJobInput": {
             "documentation": "<p>Inputs for the model bias job.</p>",
             "members": {
                 "BatchTransformInput": {
-                    "documentation": "<p>Input object for the batch transform job.</p>",
                     "shape": "BatchTransformInput"
                 },
                 "EndpointInput": {
                     "shape": "EndpointInput"
                 },
                 "GroundTruthS3Input": {
                     "documentation": "<p>Location of ground truth labels to use in model bias job.</p>",
@@ -22939,23 +24120,287 @@
         "ModelCacheSetting": {
             "enum": [
                 "Enabled",
                 "Disabled"
             ],
             "type": "string"
         },
+        "ModelCard": {
+            "members": {
+                "Content": {
+                    "shape": "ModelCardContent"
+                },
+                "CreatedBy": {
+                    "shape": "UserContext"
+                },
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "LastModifiedBy": {
+                    "shape": "UserContext"
+                },
+                "LastModifiedTime": {
+                    "shape": "Timestamp"
+                },
+                "ModelCardArn": {
+                    "shape": "ModelCardArn"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardStatus": {
+                    "shape": "ModelCardStatus"
+                },
+                "ModelCardVersion": {
+                    "shape": "Integer"
+                },
+                "ModelId": {
+                    "shape": "String"
+                },
+                "RiskRating": {
+                    "shape": "String"
+                },
+                "SecurityConfig": {
+                    "shape": "ModelCardSecurityConfig"
+                },
+                "Tags": {
+                    "shape": "TagList"
+                }
+            },
+            "type": "structure"
+        },
+        "ModelCardArn": {
+            "max": 256,
+            "pattern": "^arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]{9,16}:[0-9]{12}:model-card/[a-zA-Z0-9](-*[a-zA-Z0-9]){0,62}$",
+            "type": "string"
+        },
+        "ModelCardContent": {
+            "max": 100000,
+            "min": 0,
+            "pattern": ".*",
+            "sensitive": true,
+            "type": "string"
+        },
+        "ModelCardExportArtifacts": {
+            "members": {
+                "S3ExportArtifacts": {
+                    "shape": "S3Uri"
+                }
+            },
+            "required": [
+                "S3ExportArtifacts"
+            ],
+            "type": "structure"
+        },
+        "ModelCardExportJobArn": {
+            "max": 256,
+            "pattern": "^arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]{9,16}:[0-9]{12}:model-card/[a-zA-Z0-9](-*[a-zA-Z0-9]){0,62}/export-job/[a-zA-Z0-9](-*[a-zA-Z0-9]){0,62}$",
+            "type": "string"
+        },
+        "ModelCardExportJobSortBy": {
+            "documentation": "Attribute by which to sort returned export jobs.",
+            "enum": [
+                "Name",
+                "CreationTime",
+                "Status"
+            ],
+            "type": "string"
+        },
+        "ModelCardExportJobSortOrder": {
+            "enum": [
+                "Ascending",
+                "Descending"
+            ],
+            "type": "string"
+        },
+        "ModelCardExportJobStatus": {
+            "enum": [
+                "InProgress",
+                "Completed",
+                "Failed"
+            ],
+            "type": "string"
+        },
+        "ModelCardExportJobSummary": {
+            "members": {
+                "CreatedAt": {
+                    "shape": "Timestamp"
+                },
+                "LastModifiedAt": {
+                    "shape": "Timestamp"
+                },
+                "ModelCardExportJobArn": {
+                    "shape": "ModelCardExportJobArn"
+                },
+                "ModelCardExportJobName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardVersion": {
+                    "shape": "Integer"
+                },
+                "Status": {
+                    "shape": "ModelCardExportJobStatus"
+                }
+            },
+            "required": [
+                "ModelCardExportJobName",
+                "ModelCardExportJobArn",
+                "Status",
+                "ModelCardName",
+                "ModelCardVersion",
+                "CreatedAt",
+                "LastModifiedAt"
+            ],
+            "type": "structure"
+        },
+        "ModelCardExportJobSummaryList": {
+            "member": {
+                "shape": "ModelCardExportJobSummary"
+            },
+            "type": "list"
+        },
+        "ModelCardExportOutputConfig": {
+            "members": {
+                "S3OutputPath": {
+                    "shape": "S3Uri"
+                }
+            },
+            "required": [
+                "S3OutputPath"
+            ],
+            "type": "structure"
+        },
+        "ModelCardProcessingStatus": {
+            "enum": [
+                "DeleteInProgress",
+                "DeletePending",
+                "ContentDeleted",
+                "ExportJobsDeleted",
+                "DeleteCompleted",
+                "DeleteFailed"
+            ],
+            "type": "string"
+        },
+        "ModelCardSecurityConfig": {
+            "members": {
+                "KmsKeyId": {
+                    "shape": "KmsKeyId"
+                }
+            },
+            "type": "structure"
+        },
+        "ModelCardSortBy": {
+            "enum": [
+                "Name",
+                "CreationTime"
+            ],
+            "type": "string"
+        },
+        "ModelCardSortOrder": {
+            "enum": [
+                "Ascending",
+                "Descending"
+            ],
+            "type": "string"
+        },
+        "ModelCardStatus": {
+            "enum": [
+                "Draft",
+                "PendingReview",
+                "Approved",
+                "Archived"
+            ],
+            "type": "string"
+        },
+        "ModelCardSummary": {
+            "members": {
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "LastModifiedTime": {
+                    "shape": "Timestamp"
+                },
+                "ModelCardArn": {
+                    "shape": "ModelCardArn"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardStatus": {
+                    "shape": "ModelCardStatus"
+                }
+            },
+            "required": [
+                "ModelCardName",
+                "ModelCardArn",
+                "ModelCardStatus",
+                "CreationTime"
+            ],
+            "type": "structure"
+        },
+        "ModelCardSummaryList": {
+            "member": {
+                "shape": "ModelCardSummary"
+            },
+            "type": "list"
+        },
+        "ModelCardVersionSortBy": {
+            "enum": [
+                "Version"
+            ],
+            "type": "string"
+        },
+        "ModelCardVersionSummary": {
+            "members": {
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "LastModifiedTime": {
+                    "shape": "Timestamp"
+                },
+                "ModelCardArn": {
+                    "shape": "ModelCardArn"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardStatus": {
+                    "shape": "ModelCardStatus"
+                },
+                "ModelCardVersion": {
+                    "shape": "Integer"
+                }
+            },
+            "required": [
+                "ModelCardName",
+                "ModelCardArn",
+                "ModelCardStatus",
+                "ModelCardVersion",
+                "CreationTime"
+            ],
+            "type": "structure"
+        },
+        "ModelCardVersionSummaryList": {
+            "member": {
+                "shape": "ModelCardVersionSummary"
+            },
+            "type": "list"
+        },
         "ModelClientConfig": {
             "documentation": "<p>Configures the timeout and maximum number of retries for processing a transform job invocation.</p>",
             "members": {
                 "InvocationsMaxRetries": {
-                    "documentation": "<p>The maximum number of retries when invocation requests are failing. The default value is 3.</p>",
+                    "documentation": "<p>The maximum number of retries when invocation requests are failing.</p>",
                     "shape": "InvocationsMaxRetries"
                 },
                 "InvocationsTimeoutInSeconds": {
-                    "documentation": "<p>The timeout value in seconds for an invocation request. The default value is 600.</p>",
+                    "documentation": "<p>The timeout value in seconds for an invocation request.</p>",
                     "shape": "InvocationsTimeoutInSeconds"
                 }
             },
             "type": "structure"
         },
         "ModelConfiguration": {
             "documentation": "<p>Defines the model configuration. Includes the specification name and environment parameters.</p>",
@@ -22967,14 +24412,160 @@
                 "InferenceSpecificationName": {
                     "documentation": "<p>The inference specification name in the model package version.</p>",
                     "shape": "InferenceSpecificationName"
                 }
             },
             "type": "structure"
         },
+        "ModelDashboardEndpoint": {
+            "members": {
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "EndpointArn": {
+                    "shape": "EndpointArn"
+                },
+                "EndpointName": {
+                    "shape": "EndpointName"
+                },
+                "EndpointStatus": {
+                    "shape": "EndpointStatus"
+                },
+                "LastModifiedTime": {
+                    "shape": "Timestamp"
+                }
+            },
+            "required": [
+                "EndpointName",
+                "EndpointArn",
+                "CreationTime",
+                "LastModifiedTime",
+                "EndpointStatus"
+            ],
+            "type": "structure"
+        },
+        "ModelDashboardEndpoints": {
+            "member": {
+                "shape": "ModelDashboardEndpoint"
+            },
+            "type": "list"
+        },
+        "ModelDashboardIndicatorAction": {
+            "members": {
+                "Enabled": {
+                    "shape": "Boolean"
+                }
+            },
+            "type": "structure"
+        },
+        "ModelDashboardModel": {
+            "members": {
+                "Endpoints": {
+                    "shape": "ModelDashboardEndpoints"
+                },
+                "LastBatchTransformJob": {
+                    "shape": "TransformJob"
+                },
+                "Model": {
+                    "shape": "Model"
+                },
+                "ModelCard": {
+                    "shape": "ModelDashboardModelCard"
+                },
+                "MonitoringSchedules": {
+                    "shape": "ModelDashboardMonitoringSchedules"
+                }
+            },
+            "type": "structure"
+        },
+        "ModelDashboardModelCard": {
+            "members": {
+                "CreatedBy": {
+                    "shape": "UserContext"
+                },
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "LastModifiedBy": {
+                    "shape": "UserContext"
+                },
+                "LastModifiedTime": {
+                    "shape": "Timestamp"
+                },
+                "ModelCardArn": {
+                    "shape": "ModelCardArn"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardStatus": {
+                    "shape": "ModelCardStatus"
+                },
+                "ModelCardVersion": {
+                    "shape": "Integer"
+                },
+                "ModelId": {
+                    "shape": "String"
+                },
+                "RiskRating": {
+                    "shape": "String"
+                },
+                "SecurityConfig": {
+                    "shape": "ModelCardSecurityConfig"
+                },
+                "Tags": {
+                    "shape": "TagList"
+                }
+            },
+            "type": "structure"
+        },
+        "ModelDashboardMonitoringSchedule": {
+            "members": {
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "EndpointName": {
+                    "shape": "EndpointName"
+                },
+                "FailureReason": {
+                    "shape": "FailureReason"
+                },
+                "LastModifiedTime": {
+                    "shape": "Timestamp"
+                },
+                "LastMonitoringExecutionSummary": {
+                    "shape": "MonitoringExecutionSummary"
+                },
+                "MonitoringAlertSummaries": {
+                    "shape": "MonitoringAlertSummaryList"
+                },
+                "MonitoringScheduleArn": {
+                    "shape": "MonitoringScheduleArn"
+                },
+                "MonitoringScheduleConfig": {
+                    "shape": "MonitoringScheduleConfig"
+                },
+                "MonitoringScheduleName": {
+                    "shape": "MonitoringScheduleName"
+                },
+                "MonitoringScheduleStatus": {
+                    "shape": "ScheduleStatus"
+                },
+                "MonitoringType": {
+                    "shape": "MonitoringType"
+                }
+            },
+            "type": "structure"
+        },
+        "ModelDashboardMonitoringSchedules": {
+            "member": {
+                "shape": "ModelDashboardMonitoringSchedule"
+            },
+            "type": "list"
+        },
         "ModelDataQuality": {
             "documentation": "<p>Data quality constraints and statistics for a model.</p>",
             "members": {
                 "Constraints": {
                     "documentation": "<p>Data quality constraints for a model.</p>",
                     "shape": "MetricsSource"
                 },
@@ -23019,15 +24610,15 @@
             },
             "type": "structure"
         },
         "ModelExplainabilityAppSpecification": {
             "documentation": "<p>Docker container image configuration object for the model explainability job.</p>",
             "members": {
                 "ConfigUri": {
-                    "documentation": "<p>JSON formatted S3 file that defines explainability parameters. For more information on this JSON configuration file, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/clarify-config-json-monitor-model-explainability-parameters.html\">Configure model explainability parameters</a>.</p>",
+                    "documentation": "<p>JSON formatted S3 file that defines explainability parameters. For more information on this JSON configuration file, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/json-model-explainability-parameter-config.html\">Configure model explainability parameters</a>.</p>",
                     "shape": "S3Uri"
                 },
                 "Environment": {
                     "documentation": "<p>Sets the environment variables in the Docker container.</p>",
                     "shape": "MonitoringEnvironmentMap"
                 },
                 "ImageUri": {
@@ -23054,23 +24645,43 @@
             },
             "type": "structure"
         },
         "ModelExplainabilityJobInput": {
             "documentation": "<p>Inputs for the model explainability job.</p>",
             "members": {
                 "BatchTransformInput": {
-                    "documentation": "<p>Input object for the batch transform job.</p>",
                     "shape": "BatchTransformInput"
                 },
                 "EndpointInput": {
                     "shape": "EndpointInput"
                 }
             },
             "type": "structure"
         },
+        "ModelInfrastructureConfig": {
+            "members": {
+                "InfrastructureType": {
+                    "shape": "ModelInfrastructureType"
+                },
+                "RealTimeInferenceConfig": {
+                    "shape": "RealTimeInferenceConfig"
+                }
+            },
+            "required": [
+                "InfrastructureType",
+                "RealTimeInferenceConfig"
+            ],
+            "type": "structure"
+        },
+        "ModelInfrastructureType": {
+            "enum": [
+                "RealTimeInference"
+            ],
+            "type": "string"
+        },
         "ModelInput": {
             "documentation": "<p>Input object for the model.</p>",
             "members": {
                 "DataInputConfig": {
                     "documentation": "<p>The input configuration object for the model.</p>",
                     "shape": "DataInputConfig"
                 }
@@ -23234,15 +24845,14 @@
                     "shape": "ApprovalDescription"
                 },
                 "CertifyForMarketplace": {
                     "documentation": "<p>Whether the model package is to be certified to be listed on Amazon Web Services Marketplace. For information about listing model packages on Amazon Web Services Marketplace, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-mkt-list.html\">List Your Algorithm or Model Package on Amazon Web Services Marketplace</a>.</p>",
                     "shape": "CertifyForMarketplace"
                 },
                 "CreatedBy": {
-                    "documentation": "<p>Information about the user who created or modified an experiment, trial, trial component, lineage group, or project.</p>",
                     "shape": "UserContext"
                 },
                 "CreationTime": {
                     "documentation": "<p>The time that the model package was created.</p>",
                     "shape": "CreationTime"
                 },
                 "CustomerMetadataProperties": {
@@ -23254,27 +24864,24 @@
                     "shape": "String"
                 },
                 "DriftCheckBaselines": {
                     "documentation": "<p>Represents the drift check baselines that can be used when the model monitor is set using the model package.</p>",
                     "shape": "DriftCheckBaselines"
                 },
                 "InferenceSpecification": {
-                    "documentation": "<p>Defines how to perform inference generation after a training job is run.</p>",
                     "shape": "InferenceSpecification"
                 },
                 "LastModifiedBy": {
-                    "documentation": "<p>Information about the user who created or modified an experiment, trial, trial component, lineage group, or project.</p>",
                     "shape": "UserContext"
                 },
                 "LastModifiedTime": {
                     "documentation": "<p>The last time the model package was modified.</p>",
                     "shape": "Timestamp"
                 },
                 "MetadataProperties": {
-                    "documentation": "<p>Metadata properties of the tracking entity, trial, or trial component.</p>",
                     "shape": "MetadataProperties"
                 },
                 "ModelApprovalStatus": {
                     "documentation": "<p>The approval status of the model. This can be one of the following values.</p> <ul> <li> <p> <code>APPROVED</code> - The model is approved</p> </li> <li> <p> <code>REJECTED</code> - The model is rejected.</p> </li> <li> <p> <code>PENDING_MANUAL_APPROVAL</code> - The model is waiting for manual approval.</p> </li> </ul>",
                     "shape": "ModelApprovalStatus"
                 },
                 "ModelMetrics": {
@@ -23298,39 +24905,36 @@
                     "shape": "EntityName"
                 },
                 "ModelPackageStatus": {
                     "documentation": "<p>The status of the model package. This can be one of the following values.</p> <ul> <li> <p> <code>PENDING</code> - The model package is pending being created.</p> </li> <li> <p> <code>IN_PROGRESS</code> - The model package is in the process of being created.</p> </li> <li> <p> <code>COMPLETED</code> - The model package was successfully created.</p> </li> <li> <p> <code>FAILED</code> - The model package failed.</p> </li> <li> <p> <code>DELETING</code> - The model package is in the process of being deleted.</p> </li> </ul>",
                     "shape": "ModelPackageStatus"
                 },
                 "ModelPackageStatusDetails": {
-                    "documentation": "<p>Specifies the validation and image scan statuses of the model package.</p>",
                     "shape": "ModelPackageStatusDetails"
                 },
                 "ModelPackageVersion": {
                     "documentation": "<p>The version number of a versioned model.</p>",
                     "shape": "ModelPackageVersion"
                 },
                 "SamplePayloadUrl": {
                     "documentation": "<p>The Amazon Simple Storage Service path where the sample payload are stored. This path must point to a single gzip compressed tar archive (.tar.gz suffix).</p>",
                     "shape": "String"
                 },
                 "SourceAlgorithmSpecification": {
-                    "documentation": "<p>A list of algorithms that were used to create a model package.</p>",
                     "shape": "SourceAlgorithmSpecification"
                 },
                 "Tags": {
                     "documentation": "<p>A list of the tags associated with the model package. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a> in the <i>Amazon Web Services General Reference Guide</i>.</p>",
                     "shape": "TagList"
                 },
                 "Task": {
                     "documentation": "<p>The machine learning task your model package accomplishes. Common machine learning tasks include object detection and image classification.</p>",
                     "shape": "String"
                 },
                 "ValidationSpecification": {
-                    "documentation": "<p>Specifies batch transform jobs that SageMaker runs to validate your model package.</p>",
                     "shape": "ModelPackageValidationSpecification"
                 }
             },
             "type": "structure"
         },
         "ModelPackageArn": {
             "max": 2048,
@@ -23362,15 +24966,15 @@
                     "shape": "String"
                 },
                 "FrameworkVersion": {
                     "documentation": "<p>The framework version of the Model Package Container Image.</p>",
                     "shape": "FrameworkVersion"
                 },
                 "Image": {
-                    "documentation": "<p>The Amazon EC2 Container Registry (Amazon ECR) path where inference code is stored.</p> <p>If you are using your own custom algorithm instead of an algorithm provided by SageMaker, the inference code must meet SageMaker requirements. SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>.</p>",
+                    "documentation": "<p>The Amazon EC2 Container Registry (Amazon ECR) path where inference code is stored.</p> <p>If you are using your own custom algorithm instead of an algorithm provided by Amazon SageMaker, the inference code must meet Amazon SageMaker requirements. Amazon SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>.</p>",
                     "shape": "ContainerImage"
                 },
                 "ImageDigest": {
                     "documentation": "<p>An MD5 hash of the training algorithm that identifies the Docker image used for training.</p>",
                     "shape": "ImageDigest"
                 },
                 "ModelDataUrl": {
@@ -23650,18 +25254,18 @@
             "member": {
                 "shape": "ModelPackageValidationProfile"
             },
             "min": 1,
             "type": "list"
         },
         "ModelPackageValidationSpecification": {
-            "documentation": "<p>Specifies batch transform jobs that SageMaker runs to validate your model package.</p>",
+            "documentation": "<p>Specifies batch transform jobs that Amazon SageMaker runs to validate your model package.</p>",
             "members": {
                 "ValidationProfiles": {
-                    "documentation": "<p>An array of <code>ModelPackageValidationProfile</code> objects, each of which specifies a batch transform job that SageMaker runs to validate your model package.</p>",
+                    "documentation": "<p>An array of <code>ModelPackageValidationProfile</code> objects, each of which specifies a batch transform job that Amazon SageMaker runs to validate your model package.</p>",
                     "shape": "ModelPackageValidationProfiles"
                 },
                 "ValidationRole": {
                     "documentation": "<p>The IAM roles to be used for the validation of the model package.</p>",
                     "shape": "RoleArn"
                 }
             },
@@ -23739,15 +25343,14 @@
             },
             "type": "structure"
         },
         "ModelQualityJobInput": {
             "documentation": "<p>The input for the model quality monitoring job. Currently endponts are supported for input for model quality monitoring jobs.</p>",
             "members": {
                 "BatchTransformInput": {
-                    "documentation": "<p>Input object for the batch transform job.</p>",
                     "shape": "BatchTransformInput"
                 },
                 "EndpointInput": {
                     "shape": "EndpointInput"
                 },
                 "GroundTruthS3Input": {
                     "documentation": "<p>The ground truth label provided for the model.</p>",
@@ -23801,14 +25404,204 @@
         },
         "ModelSummaryList": {
             "member": {
                 "shape": "ModelSummary"
             },
             "type": "list"
         },
+        "ModelVariantAction": {
+            "enum": [
+                "Retain",
+                "Remove",
+                "Promote"
+            ],
+            "type": "string"
+        },
+        "ModelVariantActionMap": {
+            "key": {
+                "shape": "ModelVariantName"
+            },
+            "max": 2,
+            "min": 1,
+            "type": "map",
+            "value": {
+                "shape": "ModelVariantAction"
+            }
+        },
+        "ModelVariantConfig": {
+            "members": {
+                "InfrastructureConfig": {
+                    "shape": "ModelInfrastructureConfig"
+                },
+                "ModelName": {
+                    "shape": "ModelName"
+                },
+                "VariantName": {
+                    "shape": "ModelVariantName"
+                }
+            },
+            "required": [
+                "ModelName",
+                "VariantName",
+                "InfrastructureConfig"
+            ],
+            "type": "structure"
+        },
+        "ModelVariantConfigList": {
+            "max": 2,
+            "member": {
+                "shape": "ModelVariantConfig"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "ModelVariantConfigSummary": {
+            "members": {
+                "InfrastructureConfig": {
+                    "shape": "ModelInfrastructureConfig"
+                },
+                "ModelName": {
+                    "shape": "ModelName"
+                },
+                "Status": {
+                    "shape": "ModelVariantStatus"
+                },
+                "VariantName": {
+                    "shape": "ModelVariantName"
+                }
+            },
+            "required": [
+                "ModelName",
+                "VariantName",
+                "InfrastructureConfig",
+                "Status"
+            ],
+            "type": "structure"
+        },
+        "ModelVariantConfigSummaryList": {
+            "member": {
+                "shape": "ModelVariantConfigSummary"
+            },
+            "type": "list"
+        },
+        "ModelVariantName": {
+            "max": 63,
+            "pattern": "^[a-zA-Z0-9]([\\-a-zA-Z0-9]*[a-zA-Z0-9])?",
+            "type": "string"
+        },
+        "ModelVariantStatus": {
+            "enum": [
+                "Creating",
+                "Updating",
+                "InService",
+                "Deleting",
+                "Deleted"
+            ],
+            "type": "string"
+        },
+        "MonitoringAlertActions": {
+            "members": {
+                "ModelDashboardIndicator": {
+                    "shape": "ModelDashboardIndicatorAction"
+                }
+            },
+            "type": "structure"
+        },
+        "MonitoringAlertHistoryList": {
+            "member": {
+                "shape": "MonitoringAlertHistorySummary"
+            },
+            "type": "list"
+        },
+        "MonitoringAlertHistorySortKey": {
+            "enum": [
+                "CreationTime",
+                "Status"
+            ],
+            "type": "string"
+        },
+        "MonitoringAlertHistorySummary": {
+            "members": {
+                "AlertStatus": {
+                    "shape": "MonitoringAlertStatus"
+                },
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "MonitoringAlertName": {
+                    "shape": "MonitoringAlertName"
+                },
+                "MonitoringScheduleName": {
+                    "shape": "MonitoringScheduleName"
+                }
+            },
+            "required": [
+                "MonitoringScheduleName",
+                "MonitoringAlertName",
+                "CreationTime",
+                "AlertStatus"
+            ],
+            "type": "structure"
+        },
+        "MonitoringAlertName": {
+            "max": 63,
+            "min": 1,
+            "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,62}$",
+            "type": "string"
+        },
+        "MonitoringAlertStatus": {
+            "enum": [
+                "InAlert",
+                "OK"
+            ],
+            "type": "string"
+        },
+        "MonitoringAlertSummary": {
+            "members": {
+                "Actions": {
+                    "shape": "MonitoringAlertActions"
+                },
+                "AlertStatus": {
+                    "shape": "MonitoringAlertStatus"
+                },
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "DatapointsToAlert": {
+                    "shape": "MonitoringDatapointsToAlert"
+                },
+                "EvaluationPeriod": {
+                    "shape": "MonitoringEvaluationPeriod"
+                },
+                "LastModifiedTime": {
+                    "shape": "Timestamp"
+                },
+                "MonitoringAlertName": {
+                    "shape": "MonitoringAlertName"
+                }
+            },
+            "required": [
+                "MonitoringAlertName",
+                "CreationTime",
+                "LastModifiedTime",
+                "AlertStatus",
+                "DatapointsToAlert",
+                "EvaluationPeriod",
+                "Actions"
+            ],
+            "type": "structure"
+        },
+        "MonitoringAlertSummaryList": {
+            "max": 100,
+            "member": {
+                "shape": "MonitoringAlertSummary"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "MonitoringAppSpecification": {
             "documentation": "<p>Container image configuration object for the monitoring job.</p>",
             "members": {
                 "ContainerArguments": {
                     "documentation": "<p>An array of arguments for the container used to run the monitoring job.</p>",
                     "shape": "MonitoringContainerArguments"
                 },
@@ -23894,36 +25687,35 @@
             "member": {
                 "shape": "ContainerArgument"
             },
             "min": 1,
             "type": "list"
         },
         "MonitoringCsvDatasetFormat": {
-            "documentation": "<p>Represents the CSV dataset format used when running a monitoring job.</p>",
             "members": {
                 "Header": {
-                    "documentation": "<p>Indicates if the CSV data has a header.</p>",
                     "shape": "Boolean"
                 }
             },
             "type": "structure"
         },
+        "MonitoringDatapointsToAlert": {
+            "max": 100,
+            "min": 1,
+            "type": "integer"
+        },
         "MonitoringDatasetFormat": {
-            "documentation": "<p>Represents the dataset format used when running a monitoring job.</p>",
             "members": {
                 "Csv": {
-                    "documentation": "<p>The CSV dataset used in the monitoring job.</p>",
                     "shape": "MonitoringCsvDatasetFormat"
                 },
                 "Json": {
-                    "documentation": "<p>The JSON dataset used in the monitoring job</p>",
                     "shape": "MonitoringJsonDatasetFormat"
                 },
                 "Parquet": {
-                    "documentation": "<p>The Parquet dataset used in the monitoring job</p>",
                     "shape": "MonitoringParquetDatasetFormat"
                 }
             },
             "type": "structure"
         },
         "MonitoringEnvironmentMap": {
             "key": {
@@ -23931,14 +25723,19 @@
             },
             "max": 50,
             "type": "map",
             "value": {
                 "shape": "ProcessingEnvironmentValue"
             }
         },
+        "MonitoringEvaluationPeriod": {
+            "max": 100,
+            "min": 1,
+            "type": "integer"
+        },
         "MonitoringExecutionSortKey": {
             "enum": [
                 "CreationTime",
                 "ScheduledTime",
                 "Status"
             ],
             "type": "string"
@@ -24012,15 +25809,14 @@
             },
             "type": "structure"
         },
         "MonitoringInput": {
             "documentation": "<p>The inputs for a monitoring job.</p>",
             "members": {
                 "BatchTransformInput": {
-                    "documentation": "<p>Input object for the batch transform job.</p>",
                     "shape": "BatchTransformInput"
                 },
                 "EndpointInput": {
                     "documentation": "<p>The endpoint for a monitoring job.</p>",
                     "shape": "EndpointInput"
                 }
             },
@@ -24132,18 +25928,16 @@
         "MonitoringJobDefinitionSummaryList": {
             "member": {
                 "shape": "MonitoringJobDefinitionSummary"
             },
             "type": "list"
         },
         "MonitoringJsonDatasetFormat": {
-            "documentation": "<p>Represents the JSON dataset format used when running a monitoring job.</p>",
             "members": {
                 "Line": {
-                    "documentation": "<p>Indicates if the file should be read as a json object per line. </p>",
                     "shape": "Boolean"
                 }
             },
             "type": "structure"
         },
         "MonitoringMaxRuntimeInSeconds": {
             "max": 86400,
@@ -24202,15 +25996,14 @@
             "member": {
                 "shape": "MonitoringOutput"
             },
             "min": 1,
             "type": "list"
         },
         "MonitoringParquetDatasetFormat": {
-            "documentation": "<p>Represents the Parquet dataset format used when running a monitoring job.</p>",
             "members": {},
             "type": "structure"
         },
         "MonitoringProblemType": {
             "enum": [
                 "BinaryClassification",
                 "MulticlassClassification",
@@ -24696,26 +26489,26 @@
                 "Failed",
                 "Deleting",
                 "Updating"
             ],
             "type": "string"
         },
         "NotebookInstanceSummary": {
-            "documentation": "<p>Provides summary information for an SageMaker notebook instance.</p>",
+            "documentation": "<p>Provides summary information for an Amazon SageMaker notebook instance.</p>",
             "members": {
                 "AdditionalCodeRepositories": {
-                    "documentation": "<p>An array of up to three Git repositories associated with the notebook instance. These can be either the names of Git repositories stored as resources in your account, or the URL of Git repositories in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. These repositories are cloned at the same level as the default repository of your notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with SageMaker Notebook Instances</a>.</p>",
+                    "documentation": "<p>An array of up to three Git repositories associated with the notebook instance. These can be either the names of Git repositories stored as resources in your account, or the URL of Git repositories in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. These repositories are cloned at the same level as the default repository of your notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with Amazon SageMaker Notebook Instances</a>.</p>",
                     "shape": "AdditionalCodeRepositoryNamesOrUrls"
                 },
                 "CreationTime": {
                     "documentation": "<p>A timestamp that shows when the notebook instance was created.</p>",
                     "shape": "CreationTime"
                 },
                 "DefaultCodeRepository": {
-                    "documentation": "<p>The Git repository associated with the notebook instance as its default code repository. This can be either the name of a Git repository stored as a resource in your account, or the URL of a Git repository in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. When you open a notebook instance, it opens in the directory that contains this repository. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with SageMaker Notebook Instances</a>.</p>",
+                    "documentation": "<p>The Git repository associated with the notebook instance as its default code repository. This can be either the name of a Git repository stored as a resource in your account, or the URL of a Git repository in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. When you open a notebook instance, it opens in the directory that contains this repository. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with Amazon SageMaker Notebook Instances</a>.</p>",
                     "shape": "CodeRepositoryNameOrUrl"
                 },
                 "InstanceType": {
                     "documentation": "<p>The type of ML compute instance that the notebook instance is running on.</p>",
                     "shape": "InstanceType"
                 },
                 "LastModifiedTime": {
@@ -24735,15 +26528,15 @@
                     "shape": "NotebookInstanceName"
                 },
                 "NotebookInstanceStatus": {
                     "documentation": "<p>The status of the notebook instance.</p>",
                     "shape": "NotebookInstanceStatus"
                 },
                 "Url": {
-                    "documentation": "<p>The URL that you use to connect to the Jupyter notebook running in your notebook instance. </p>",
+                    "documentation": "<p>The URL that you use to connect to the Jupyter instance running in your notebook instance. </p>",
                     "shape": "NotebookInstanceUrl"
                 }
             },
             "required": [
                 "NotebookInstanceName",
                 "NotebookInstanceArn"
             ],
@@ -24829,14 +26622,17 @@
                 "DisableGlueTableCreation": {
                     "documentation": "<p>Set to <code>True</code> to disable the automatic creation of an Amazon Web Services Glue table when configuring an <code>OfflineStore</code>.</p>",
                     "shape": "Boolean"
                 },
                 "S3StorageConfig": {
                     "documentation": "<p>The Amazon Simple Storage (Amazon S3) location of <code>OfflineStore</code>.</p>",
                     "shape": "S3StorageConfig"
+                },
+                "TableFormat": {
+                    "shape": "TableFormat"
                 }
             },
             "required": [
                 "S3StorageConfig"
             ],
             "type": "structure"
         },
@@ -25053,19 +26849,19 @@
             ],
             "type": "structure"
         },
         "OutputDataConfig": {
             "documentation": "<p>Provides information about how to store model training results (model artifacts).</p>",
             "members": {
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that SageMaker uses to encrypt the model artifacts at rest using Amazon S3 server-side encryption. The <code>KmsKeyId</code> can be any of the following formats: </p> <ul> <li> <p>// KMS Key ID</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// KMS Key Alias</p> <p> <code>\"alias/ExampleAlias\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key Alias</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias\"</code> </p> </li> </ul> <p>If you use a KMS key ID or an alias of your KMS key, the SageMaker execution role must include permissions to call <code>kms:Encrypt</code>. If you don't provide a KMS key ID, SageMaker uses the default KMS key for Amazon S3 for your role's account. SageMaker uses server-side encryption with KMS-managed keys for <code>OutputDataConfig</code>. If you use a bucket policy with an <code>s3:PutObject</code> permission that only allows objects with server-side encryption, set the condition key of <code>s3:x-amz-server-side-encryption</code> to <code>\"aws:kms\"</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingKMSEncryption.html\">KMS-Managed Encryption Keys</a> in the <i>Amazon Simple Storage Service Developer Guide.</i> </p> <p>The KMS key policy must grant permission to the IAM role that you specify in your <code>CreateTrainingJob</code>, <code>CreateTransformJob</code>, or <code>CreateHyperParameterTuningJob</code> requests. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html\">Using Key Policies in Amazon Web Services KMS</a> in the <i>Amazon Web Services Key Management Service Developer Guide</i>.</p>",
+                    "documentation": "<p>The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that Amazon SageMaker uses to encrypt the model artifacts at rest using Amazon S3 server-side encryption. The <code>KmsKeyId</code> can be any of the following formats: </p> <ul> <li> <p>// KMS Key ID</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// KMS Key Alias</p> <p> <code>\"alias/ExampleAlias\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key Alias</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias\"</code> </p> </li> </ul> <p>If you use a KMS key ID or an alias of your KMS key, the Amazon SageMaker execution role must include permissions to call <code>kms:Encrypt</code>. If you don't provide a KMS key ID, Amazon SageMaker uses the default KMS key for Amazon S3 for your role's account. Amazon SageMaker uses server-side encryption with KMS-managed keys for <code>OutputDataConfig</code>. If you use a bucket policy with an <code>s3:PutObject</code> permission that only allows objects with server-side encryption, set the condition key of <code>s3:x-amz-server-side-encryption</code> to <code>\"aws:kms\"</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingKMSEncryption.html\">KMS-Managed Encryption Keys</a> in the <i>Amazon Simple Storage Service Developer Guide.</i> </p> <p>The KMS key policy must grant permission to the IAM role that you specify in your <code>CreateTrainingJob</code>, <code>CreateTransformJob</code>, or <code>CreateHyperParameterTuningJob</code> requests. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html\">Using Key Policies in Amazon Web Services KMS</a> in the <i>Amazon Web Services Key Management Service Developer Guide</i>.</p>",
                     "shape": "KmsKeyId"
                 },
                 "S3OutputPath": {
-                    "documentation": "<p>Identifies the S3 path where you want SageMaker to store the model artifacts. For example, <code>s3://bucket-name/key-name-prefix</code>. </p>",
+                    "documentation": "<p>Identifies the S3 path where you want Amazon SageMaker to store the model artifacts. For example, <code>s3://bucket-name/key-name-prefix</code>. </p>",
                     "shape": "S3Uri"
                 }
             },
             "required": [
                 "S3OutputPath"
             ],
             "type": "structure"
@@ -25165,15 +26961,15 @@
                     "documentation": "<p>A <code>IntegerParameterRangeSpecification</code> object that defines the possible values for an integer hyperparameter.</p>",
                     "shape": "IntegerParameterRangeSpecification"
                 }
             },
             "type": "structure"
         },
         "ParameterRanges": {
-            "documentation": "<p>Specifies ranges of integer, continuous, and categorical hyperparameters that a hyperparameter tuning job searches. The hyperparameter tuning job launches training jobs with hyperparameter values within these ranges to find the combination of values that result in the training job with the best performance as measured by the objective metric of the hyperparameter tuning job.</p> <note> <p>The maximum number of items specified for <code>Array Members</code> refers to the maximum number of hyperparameters for each range and also the maximum for the hyperparameter tuning job itself. That is, the sum of the number of hyperparameters for all the ranges can't exceed the maximum number specified.</p> </note>",
+            "documentation": "<p>Specifies ranges of integer, continuous, and categorical hyperparameters that a hyperparameter tuning job searches. The hyperparameter tuning job launches training jobs with hyperparameter values within these ranges to find the combination of values that result in the training job with the best performance as measured by the objective metric of the hyperparameter tuning job.</p> <note> <p>You can specify a maximum of 20 hyperparameters that a hyperparameter tuning job can search over. Every possible value of a categorical parameter range counts against this limit.</p> </note>",
             "members": {
                 "CategoricalParameterRanges": {
                     "documentation": "<p>The array of <a>CategoricalParameterRange</a> objects that specify ranges of categorical hyperparameters that a hyperparameter tuning job searches.</p>",
                     "shape": "CategoricalParameterRanges"
                 },
                 "ContinuousParameterRanges": {
                     "documentation": "<p>The array of <a>ContinuousParameterRange</a> objects that specify ranges of continuous hyperparameters that a hyperparameter tuning job searches.</p>",
@@ -25253,14 +27049,17 @@
                     "documentation": "<p>The name of the endpoint configuration used in the deployment. </p>",
                     "shape": "EndpointConfigName"
                 },
                 "ProductionVariants": {
                     "documentation": "<p>List of <code>PendingProductionVariantSummary</code> objects.</p>",
                     "shape": "PendingProductionVariantSummaryList"
                 },
+                "ShadowProductionVariants": {
+                    "shape": "PendingProductionVariantSummaryList"
+                },
                 "StartTime": {
                     "documentation": "<p>The start time of the deployment.</p>",
                     "shape": "Timestamp"
                 }
             },
             "required": [
                 "EndpointConfigName"
@@ -25275,15 +27074,15 @@
                     "shape": "ProductionVariantAcceleratorType"
                 },
                 "CurrentInstanceCount": {
                     "documentation": "<p>The number of instances associated with the variant.</p>",
                     "shape": "TaskCount"
                 },
                 "CurrentServerlessConfig": {
-                    "documentation": "<p>The serverless configuration for the endpoint.</p>",
+                    "documentation": "<p>The serverless configuration for the endpoint.</p> <note> <p>Serverless Inference is in preview release for Amazon SageMaker and is subject to change. We do not recommend using this feature in production environments.</p> </note>",
                     "shape": "ProductionVariantServerlessConfig"
                 },
                 "CurrentWeight": {
                     "documentation": "<p>The weight associated with the variant.</p>",
                     "shape": "VariantWeight"
                 },
                 "DeployedImages": {
@@ -25291,15 +27090,15 @@
                     "shape": "DeployedImages"
                 },
                 "DesiredInstanceCount": {
                     "documentation": "<p>The number of instances requested in this deployment, as specified in the endpoint configuration for the endpoint. The value is taken from the request to the <code> <a>CreateEndpointConfig</a> </code> operation.</p>",
                     "shape": "TaskCount"
                 },
                 "DesiredServerlessConfig": {
-                    "documentation": "<p>The serverless configuration requested for this deployment, as specified in the endpoint configuration for the endpoint.</p>",
+                    "documentation": "<p>The serverless configuration requested for this deployment, as specified in the endpoint configuration for the endpoint.</p> <note> <p>Serverless Inference is in preview release for Amazon SageMaker and is subject to change. We do not recommend using this feature in production environments.</p> </note>",
                     "shape": "ProductionVariantServerlessConfig"
                 },
                 "DesiredWeight": {
                     "documentation": "<p>The requested weight for the variant in this deployment, as specified in the endpoint configuration for the endpoint. The value is taken from the request to the <code> <a>CreateEndpointConfig</a> </code> operation.</p>",
                     "shape": "VariantWeight"
                 },
                 "InstanceType": {
@@ -25591,14 +27390,17 @@
             },
             "min": 0,
             "type": "list"
         },
         "PipelineExecutionStepMetadata": {
             "documentation": "<p>Metadata for a step execution.</p>",
             "members": {
+                "AutoMLJob": {
+                    "shape": "AutoMLJobStepMetadata"
+                },
                 "Callback": {
                     "documentation": "<p>The URL of the Amazon SQS queue used by this step execution, the pipeline generated token, and a list of output parameters.</p>",
                     "shape": "CallbackStepMetadata"
                 },
                 "ClarifyCheck": {
                     "documentation": "<p>Container for the metadata for a Clarify check step. The configurations and outcomes of the check step execution. This includes: </p> <ul> <li> <p>The type of the check conducted,</p> </li> <li> <p>The Amazon S3 URIs of baseline constraints and statistics files to be used for the drift check.</p> </li> <li> <p>The Amazon S3 URIs of newly calculated baseline constraints and statistics.</p> </li> <li> <p>The model package group name provided.</p> </li> <li> <p>The Amazon S3 URI of the violation report if violations detected.</p> </li> <li> <p>The Amazon Resource Name (ARN) of check processing job initiated by the step execution.</p> </li> <li> <p>The boolean flags indicating if the drift check is skipped.</p> </li> <li> <p>If step property <code>BaselineUsedForDriftCheck</code> is set the same as <code>CalculatedBaseline</code>.</p> </li> </ul>",
                     "shape": "ClarifyCheckStepMetadata"
@@ -25704,14 +27506,20 @@
         },
         "PipelineName": {
             "max": 256,
             "min": 1,
             "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,255}",
             "type": "string"
         },
+        "PipelineNameOrArn": {
+            "max": 2048,
+            "min": 1,
+            "pattern": "(arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:pipeline/.*)?([a-zA-Z0-9](-*[a-zA-Z0-9]){0,255})",
+            "type": "string"
+        },
         "PipelineParameterName": {
             "max": 256,
             "min": 1,
             "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,255}$",
             "type": "string"
         },
         "PipelineStatus": {
@@ -26298,22 +28106,21 @@
         "ProductListings": {
             "member": {
                 "shape": "String"
             },
             "type": "list"
         },
         "ProductionVariant": {
-            "documentation": "<p>Identifies a model that you want to host and the resources chosen to deploy for hosting it. If you are deploying multiple models, tell SageMaker how to distribute traffic among the models by specifying variant weights. </p>",
+            "documentation": "<p>Identifies a model that you want to host and the resources chosen to deploy for hosting it. If you are deploying multiple models, tell Amazon SageMaker how to distribute traffic among the models by specifying variant weights. </p>",
             "members": {
                 "AcceleratorType": {
                     "documentation": "<p>The size of the Elastic Inference (EI) instance to use for the production variant. EI instances provide on-demand GPU computing for inference. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/ei.html\">Using Elastic Inference in Amazon SageMaker</a>.</p>",
                     "shape": "ProductionVariantAcceleratorType"
                 },
                 "ContainerStartupHealthCheckTimeoutInSeconds": {
-                    "documentation": "<p>The timeout value, in seconds, for your inference container to pass health check by SageMaker Hosting. For more information about health check, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms-inference-code.html#your-algorithms-inference-algo-ping-requests\">How Your Container Should Respond to Health Check (Ping) Requests</a>.</p>",
                     "shape": "ProductionVariantContainerStartupHealthCheckTimeoutInSeconds"
                 },
                 "CoreDumpConfig": {
                     "documentation": "<p>Specifies configuration for a core dump from the model container when the process crashes.</p>",
                     "shape": "ProductionVariantCoreDumpConfig"
                 },
                 "InitialInstanceCount": {
@@ -26325,31 +28132,29 @@
                     "shape": "VariantWeight"
                 },
                 "InstanceType": {
                     "documentation": "<p>The ML compute instance type.</p>",
                     "shape": "ProductionVariantInstanceType"
                 },
                 "ModelDataDownloadTimeoutInSeconds": {
-                    "documentation": "<p>The timeout value, in seconds, to download and extract the model that you want to host from Amazon S3 to the individual inference instance associated with this production variant.</p>",
                     "shape": "ProductionVariantModelDataDownloadTimeoutInSeconds"
                 },
                 "ModelName": {
                     "documentation": "<p>The name of the model that you want to host. This is the name that you specified when creating the model.</p>",
                     "shape": "ModelName"
                 },
                 "ServerlessConfig": {
-                    "documentation": "<p>The serverless configuration for an endpoint. Specifies a serverless endpoint configuration instead of an instance-based endpoint configuration.</p>",
+                    "documentation": "<p>The serverless configuration for an endpoint. Specifies a serverless endpoint configuration instead of an instance-based endpoint configuration.</p> <note> <p>Serverless Inference is in preview release for Amazon SageMaker and is subject to change. We do not recommend using this feature in production environments.</p> </note>",
                     "shape": "ProductionVariantServerlessConfig"
                 },
                 "VariantName": {
                     "documentation": "<p>The name of the production variant.</p>",
                     "shape": "VariantName"
                 },
                 "VolumeSizeInGB": {
-                    "documentation": "<p>The size, in GB, of the ML storage volume attached to individual inference instance associated with the production variant. Currenly only Amazon EBS gp2 storage volumes are supported.</p>",
                     "shape": "ProductionVariantVolumeSizeInGB"
                 }
             },
             "required": [
                 "VariantName",
                 "ModelName"
             ],
@@ -26375,15 +28180,15 @@
             "documentation": "<p>Specifies configuration for a core dump from the model container when the process crashes.</p>",
             "members": {
                 "DestinationS3Uri": {
                     "documentation": "<p>The Amazon S3 bucket to send the core dump to.</p>",
                     "shape": "DestinationS3Uri"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that SageMaker uses to encrypt the core dump data at rest using Amazon S3 server-side encryption. The <code>KmsKeyId</code> can be any of the following formats: </p> <ul> <li> <p>// KMS Key ID</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// KMS Key Alias</p> <p> <code>\"alias/ExampleAlias\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key Alias</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias\"</code> </p> </li> </ul> <p>If you use a KMS key ID or an alias of your KMS key, the SageMaker execution role must include permissions to call <code>kms:Encrypt</code>. If you don't provide a KMS key ID, SageMaker uses the default KMS key for Amazon S3 for your role's account. SageMaker uses server-side encryption with KMS-managed keys for <code>OutputDataConfig</code>. If you use a bucket policy with an <code>s3:PutObject</code> permission that only allows objects with server-side encryption, set the condition key of <code>s3:x-amz-server-side-encryption</code> to <code>\"aws:kms\"</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html\">KMS-Managed Encryption Keys</a> in the <i>Amazon Simple Storage Service Developer Guide.</i> </p> <p>The KMS key policy must grant permission to the IAM role that you specify in your <code>CreateEndpoint</code> and <code>UpdateEndpoint</code> requests. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html\">Using Key Policies in Amazon Web Services KMS</a> in the <i>Amazon Web Services Key Management Service Developer Guide</i>.</p>",
+                    "documentation": "<p>The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that Amazon SageMaker uses to encrypt the core dump data at rest using Amazon S3 server-side encryption. The <code>KmsKeyId</code> can be any of the following formats: </p> <ul> <li> <p>// KMS Key ID</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// KMS Key Alias</p> <p> <code>\"alias/ExampleAlias\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key Alias</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias\"</code> </p> </li> </ul> <p>If you use a KMS key ID or an alias of your KMS key, the Amazon SageMaker execution role must include permissions to call <code>kms:Encrypt</code>. If you don't provide a KMS key ID, Amazon SageMaker uses the default KMS key for Amazon S3 for your role's account. Amazon SageMaker uses server-side encryption with KMS-managed keys for <code>OutputDataConfig</code>. If you use a bucket policy with an <code>s3:PutObject</code> permission that only allows objects with server-side encryption, set the condition key of <code>s3:x-amz-server-side-encryption</code> to <code>\"aws:kms\"</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html\">KMS-Managed Encryption Keys</a> in the <i>Amazon Simple Storage Service Developer Guide.</i> </p> <p>The KMS key policy must grant permission to the IAM role that you specify in your <code>CreateEndpoint</code> and <code>UpdateEndpoint</code> requests. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html\">Using Key Policies in Amazon Web Services KMS</a> in the <i>Amazon Web Services Key Management Service Developer Guide</i>.</p>",
                     "shape": "KmsKeyId"
                 }
             },
             "required": [
                 "DestinationS3Uri"
             ],
             "type": "structure"
@@ -26543,15 +28348,15 @@
         },
         "ProductionVariantModelDataDownloadTimeoutInSeconds": {
             "max": 3600,
             "min": 60,
             "type": "integer"
         },
         "ProductionVariantServerlessConfig": {
-            "documentation": "<p>Specifies the serverless configuration for an endpoint variant.</p>",
+            "documentation": "<important> <p>Serverless Inference is in preview release for Amazon SageMaker and is subject to change. We do not recommend using this feature in production environments.</p> </important> <p>Specifies the serverless configuration for an endpoint variant.</p>",
             "members": {
                 "MaxConcurrency": {
                     "documentation": "<p>The maximum number of concurrent invocations your serverless endpoint can process.</p>",
                     "shape": "ServerlessMaxConcurrency"
                 },
                 "MemorySizeInMB": {
                     "documentation": "<p>The memory size of your serverless endpoint. Valid values are in 1 GB increments: 1024 MB, 2048 MB, 3072 MB, 4096 MB, 5120 MB, or 6144 MB.</p>",
@@ -26597,15 +28402,15 @@
             "documentation": "<p>Describes weight and capacities for a production variant associated with an endpoint. If you sent a request to the <code>UpdateEndpointWeightsAndCapacities</code> API and the endpoint status is <code>Updating</code>, you get different desired and current values. </p>",
             "members": {
                 "CurrentInstanceCount": {
                     "documentation": "<p>The number of instances associated with the variant.</p>",
                     "shape": "TaskCount"
                 },
                 "CurrentServerlessConfig": {
-                    "documentation": "<p>The serverless configuration for the endpoint.</p>",
+                    "documentation": "<p>The serverless configuration for the endpoint.</p> <note> <p>Serverless Inference is in preview release for Amazon SageMaker and is subject to change. We do not recommend using this feature in production environments.</p> </note>",
                     "shape": "ProductionVariantServerlessConfig"
                 },
                 "CurrentWeight": {
                     "documentation": "<p>The weight associated with the variant.</p>",
                     "shape": "VariantWeight"
                 },
                 "DeployedImages": {
@@ -26613,15 +28418,15 @@
                     "shape": "DeployedImages"
                 },
                 "DesiredInstanceCount": {
                     "documentation": "<p>The number of instances requested in the <code>UpdateEndpointWeightsAndCapacities</code> request. </p>",
                     "shape": "TaskCount"
                 },
                 "DesiredServerlessConfig": {
-                    "documentation": "<p>The serverless configuration requested for the endpoint update.</p>",
+                    "documentation": "<p>The serverless configuration requested for the endpoint update.</p> <note> <p>Serverless Inference is in preview release for Amazon SageMaker and is subject to change. We do not recommend using this feature in production environments.</p> </note>",
                     "shape": "ProductionVariantServerlessConfig"
                 },
                 "DesiredWeight": {
                     "documentation": "<p>The requested weight, as specified in the <code>UpdateEndpointWeightsAndCapacities</code> request. </p>",
                     "shape": "VariantWeight"
                 },
                 "VariantName": {
@@ -27110,15 +28915,15 @@
                     "shape": "Timestamp"
                 },
                 "ModifiedBefore": {
                     "documentation": "<p>Filter the lineage entities connected to the <code>StartArn</code>(s) before the last modified date.</p>",
                     "shape": "Timestamp"
                 },
                 "Properties": {
-                    "documentation": "<p>Filter the lineage entities connected to the <code>StartArn</code>(s) by a set if property key value pairs. If multiple pairs are provided, an entity is included in the results if it matches any of the provided pairs.</p>",
+                    "documentation": "<p>Filter the lineage entities connected to the <code>StartArn</code>(s) by a set if property key value pairs. If multiple pairs are provided, an entity will be included in the results if it matches any of the provided pairs.</p>",
                     "shape": "QueryProperties"
                 },
                 "Types": {
                     "documentation": "<p>Filter the lineage entities connected to the <code>StartArn</code> by type. For example: <code>DataSet</code>, <code>Model</code>, <code>Endpoint</code>, or <code>ModelDeployment</code>.</p>",
                     "shape": "QueryTypes"
                 }
             },
@@ -27131,27 +28936,27 @@
         "QueryLineageMaxResults": {
             "max": 50,
             "type": "integer"
         },
         "QueryLineageRequest": {
             "members": {
                 "Direction": {
-                    "documentation": "<p>Associations between lineage entities have a direction. This parameter determines the direction from the StartArn(s) that the query traverses.</p>",
+                    "documentation": "<p>Associations between lineage entities are directed. This parameter determines the direction from the StartArn(s) the query will look.</p>",
                     "shape": "Direction"
                 },
                 "Filters": {
                     "documentation": "<p>A set of filtering parameters that allow you to specify which entities should be returned.</p> <ul> <li> <p>Properties - Key-value pairs to match on the lineage entities' properties.</p> </li> <li> <p>LineageTypes - A set of lineage entity types to match on. For example: <code>TrialComponent</code>, <code>Artifact</code>, or <code>Context</code>.</p> </li> <li> <p>CreatedBefore - Filter entities created before this date.</p> </li> <li> <p>ModifiedBefore - Filter entities modified before this date.</p> </li> <li> <p>ModifiedAfter - Filter entities modified after this date.</p> </li> </ul>",
                     "shape": "QueryFilters"
                 },
                 "IncludeEdges": {
-                    "documentation": "<p> Setting this value to <code>True</code> retrieves not only the entities of interest but also the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/lineage-tracking-entities.html\">Associations</a> and lineage entities on the path. Set to <code>False</code> to only return lineage entities that match your query.</p>",
+                    "documentation": "<p> Setting this value to <code>True</code> will retrieve not only the entities of interest but also the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/lineage-tracking-entities.html\">Associations</a> and lineage entities on the path. Set to <code>False</code> to only return lineage entities that match your query.</p>",
                     "shape": "Boolean"
                 },
                 "MaxDepth": {
-                    "documentation": "<p>The maximum depth in lineage relationships from the <code>StartArns</code> that are traversed. Depth is a measure of the number of <code>Associations</code> from the <code>StartArn</code> entity to the matched results.</p>",
+                    "documentation": "<p>The maximum depth in lineage relationships from the <code>StartArns</code> that will be traversed. Depth is a measure of the number of <code>Associations</code> from the <code>StartArn</code> entity to the matched results.</p>",
                     "shape": "QueryLineageMaxDepth"
                 },
                 "MaxResults": {
                     "documentation": "<p>Limits the number of vertices in the results. Use the <code>NextToken</code> in a response to to retrieve the next page of results.</p>",
                     "shape": "QueryLineageMaxResults"
                 },
                 "NextToken": {
@@ -27214,15 +29019,14 @@
             },
             "type": "list"
         },
         "RSessionAppSettings": {
             "documentation": "<p>A collection of settings that apply to an <code>RSessionGateway</code> app.</p>",
             "members": {
                 "CustomImages": {
-                    "documentation": "<p>A list of custom SageMaker images that are configured to run as a RSession app.</p>",
                     "shape": "CustomImages"
                 },
                 "DefaultResourceSpec": {
                     "shape": "ResourceSpec"
                 }
             },
             "type": "structure"
@@ -27291,14 +29095,29 @@
         "RStudioServerProUserGroup": {
             "enum": [
                 "R_STUDIO_ADMIN",
                 "R_STUDIO_USER"
             ],
             "type": "string"
         },
+        "RealTimeInferenceConfig": {
+            "members": {
+                "InstanceCount": {
+                    "shape": "TaskCount"
+                },
+                "InstanceType": {
+                    "shape": "InstanceType"
+                }
+            },
+            "required": [
+                "InstanceType",
+                "InstanceCount"
+            ],
+            "type": "structure"
+        },
         "RealtimeInferenceInstanceTypes": {
             "member": {
                 "shape": "ProductionVariantInstanceType"
             },
             "type": "list"
         },
         "RecommendationFailureReason": {
@@ -27306,69 +29125,57 @@
         },
         "RecommendationJobArn": {
             "max": 256,
             "pattern": "arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:inference-recommendations-job/.*",
             "type": "string"
         },
         "RecommendationJobCompiledOutputConfig": {
-            "documentation": "<p>Provides information about the output configuration for the compiled model.</p>",
             "members": {
                 "S3OutputUri": {
-                    "documentation": "<p>Identifies the Amazon S3 bucket where you want SageMaker to store the compiled model artifacts.</p>",
                     "shape": "S3Uri"
                 }
             },
             "type": "structure"
         },
         "RecommendationJobContainerConfig": {
-            "documentation": "<p>Specifies mandatory fields for running an Inference Recommender job directly in the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateInferenceRecommendationsJob.html\">CreateInferenceRecommendationsJob</a> API. The fields specified in <code>ContainerConfig</code> override the corresponding fields in the model package. Use <code>ContainerConfig</code> if you want to specify these fields for the recommendation job but don't want to edit them in your model package.</p>",
             "members": {
                 "Domain": {
-                    "documentation": "<p>The machine learning domain of the model and its components.</p> <p>Valid Values: <code>COMPUTER_VISION | NATURAL_LANGUAGE_PROCESSING | MACHINE_LEARNING</code> </p>",
                     "shape": "String"
                 },
                 "Framework": {
-                    "documentation": "<p>The machine learning framework of the container image.</p> <p>Valid Values: <code>TENSORFLOW | PYTORCH | XGBOOST | SAGEMAKER-SCIKIT-LEARN</code> </p>",
                     "shape": "String"
                 },
                 "FrameworkVersion": {
-                    "documentation": "<p>The framework version of the container image.</p>",
                     "shape": "String"
                 },
                 "NearestModelName": {
-                    "documentation": "<p>The name of a pre-trained machine learning model benchmarked by Amazon SageMaker Inference Recommender that matches your model.</p> <p>Valid Values: <code>efficientnetb7 | unet | xgboost | faster-rcnn-resnet101 | nasnetlarge | vgg16 | inception-v3 | mask-rcnn | sagemaker-scikit-learn | densenet201-gluon | resnet18v2-gluon | xception | densenet201 | yolov4 | resnet152 | bert-base-cased | xceptionV1-keras | resnet50 | retinanet</code> </p>",
                     "shape": "String"
                 },
                 "PayloadConfig": {
-                    "documentation": "<p>Specifies the <code>SamplePayloadUrl</code> and all other sample payload-related fields.</p>",
                     "shape": "RecommendationJobPayloadConfig"
                 },
                 "SupportedInstanceTypes": {
-                    "documentation": "<p>A list of the instance types that are used to generate inferences in real-time.</p>",
                     "shape": "RecommendationJobSupportedInstanceTypes"
                 },
                 "Task": {
-                    "documentation": "<p>The machine learning task that the model accomplishes.</p> <p>Valid Values: <code>IMAGE_CLASSIFICATION | OBJECT_DETECTION | TEXT_GENERATION | IMAGE_SEGMENTATION | FILL_MASK | CLASSIFICATION | REGRESSION | OTHER</code> </p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "RecommendationJobDescription": {
             "max": 128,
             "type": "string"
         },
         "RecommendationJobInferenceBenchmark": {
-            "documentation": "<p>The details for a specific benchmark from an Inference Recommender job.</p>",
             "members": {
                 "EndpointConfiguration": {
                     "shape": "EndpointOutputConfiguration"
                 },
                 "FailureReason": {
-                    "documentation": "<p>The reason why a benchmark failed.</p>",
                     "shape": "RecommendationFailureReason"
                 },
                 "Metrics": {
                     "shape": "RecommendationMetrics"
                 },
                 "ModelConfiguration": {
                     "shape": "ModelConfiguration"
@@ -27379,23 +29186,21 @@
             ],
             "type": "structure"
         },
         "RecommendationJobInputConfig": {
             "documentation": "<p>The input configuration of the recommendation job.</p>",
             "members": {
                 "ContainerConfig": {
-                    "documentation": "<p>Specifies mandatory fields for running an Inference Recommender job. The fields specified in <code>ContainerConfig</code> override the corresponding fields in the model package.</p>",
                     "shape": "RecommendationJobContainerConfig"
                 },
                 "EndpointConfigurations": {
                     "documentation": "<p>Specifies the endpoint configuration to use for a job.</p>",
                     "shape": "EndpointInputConfigurations"
                 },
                 "Endpoints": {
-                    "documentation": "<p>Existing customer endpoints on which to run an Inference Recommender job.</p>",
                     "shape": "Endpoints"
                 },
                 "JobDurationInSeconds": {
                     "documentation": "<p>Specifies the maximum duration of the job, in seconds.&gt;</p>",
                     "shape": "JobDurationInSeconds"
                 },
                 "ModelPackageVersionArn": {
@@ -27407,15 +29212,14 @@
                     "shape": "RecommendationJobResourceLimit"
                 },
                 "TrafficPattern": {
                     "documentation": "<p>Specifies the traffic pattern of the job.</p>",
                     "shape": "TrafficPattern"
                 },
                 "VolumeKmsKeyId": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of a Amazon Web Services Key Management Service (Amazon Web Services KMS) key that Amazon SageMaker uses to encrypt data on the storage volume attached to the ML compute instance that hosts the endpoint. This key will be passed to SageMaker Hosting for endpoint creation. </p> <p>The SageMaker execution role must have <code>kms:CreateGrant</code> permission in order to encrypt data on the storage volume of the endpoints created for inference recommendation. The inference recommendation job will fail asynchronously during endpoint configuration creation if the role passed does not have <code>kms:CreateGrant</code> permission.</p> <p>The <code>KmsKeyId</code> can be any of the following formats:</p> <ul> <li> <p>// KMS Key ID</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key</p> <p> <code>\"arn:aws:kms:&lt;region&gt;:&lt;account&gt;:key/&lt;key-id-12ab-34cd-56ef-1234567890ab&gt;\"</code> </p> </li> <li> <p>// KMS Key Alias</p> <p> <code>\"alias/ExampleAlias\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key Alias</p> <p> <code>\"arn:aws:kms:&lt;region&gt;:&lt;account&gt;:alias/&lt;ExampleAlias&gt;\"</code> </p> </li> </ul> <p>For more information about key identifiers, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#key-id-key-id\">Key identifiers (KeyID)</a> in the Amazon Web Services Key Management Service (Amazon Web Services KMS) documentation.</p>",
                     "shape": "KmsKeyId"
                 }
             },
             "required": [
                 "ModelPackageVersionArn"
             ],
             "type": "structure"
@@ -27423,36 +29227,30 @@
         "RecommendationJobName": {
             "max": 64,
             "min": 1,
             "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,63}",
             "type": "string"
         },
         "RecommendationJobOutputConfig": {
-            "documentation": "<p>Provides information about the output configuration for the compiled model.</p>",
             "members": {
                 "CompiledOutputConfig": {
-                    "documentation": "<p>Provides information about the output configuration for the compiled model.</p>",
                     "shape": "RecommendationJobCompiledOutputConfig"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of a Amazon Web Services Key Management Service (Amazon Web Services KMS) key that Amazon SageMaker uses to encrypt your output artifacts with Amazon S3 server-side encryption. The SageMaker execution role must have <code>kms:GenerateDataKey</code> permission.</p> <p>The <code>KmsKeyId</code> can be any of the following formats:</p> <ul> <li> <p>// KMS Key ID</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key</p> <p> <code>\"arn:aws:kms:&lt;region&gt;:&lt;account&gt;:key/&lt;key-id-12ab-34cd-56ef-1234567890ab&gt;\"</code> </p> </li> <li> <p>// KMS Key Alias</p> <p> <code>\"alias/ExampleAlias\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key Alias</p> <p> <code>\"arn:aws:kms:&lt;region&gt;:&lt;account&gt;:alias/&lt;ExampleAlias&gt;\"</code> </p> </li> </ul> <p>For more information about key identifiers, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#key-id-key-id\">Key identifiers (KeyID)</a> in the Amazon Web Services Key Management Service (Amazon Web Services KMS) documentation.</p>",
                     "shape": "KmsKeyId"
                 }
             },
             "type": "structure"
         },
         "RecommendationJobPayloadConfig": {
-            "documentation": "<p>The configuration for the payload for a recommendation job.</p>",
             "members": {
                 "SamplePayloadUrl": {
-                    "documentation": "<p>The Amazon Simple Storage Service (Amazon S3) path where the sample payload is stored. This path must point to a single gzip compressed tar archive (.tar.gz suffix).</p>",
                     "shape": "String"
                 },
                 "SupportedContentTypes": {
-                    "documentation": "<p>The supported MIME types for the input data.</p>",
                     "shape": "RecommendationJobSupportedContentTypes"
                 }
             },
             "type": "structure"
         },
         "RecommendationJobResourceLimit": {
             "documentation": "<p>Specifies the maximum number of jobs that can run in parallel and the maximum number of jobs that can run.</p>",
@@ -27777,14 +29575,19 @@
         },
         "RepositoryCredentialsProviderArn": {
             "max": 2048,
             "min": 1,
             "pattern": ".*",
             "type": "string"
         },
+        "RepositoryUrl": {
+            "max": 1024,
+            "pattern": "^https://([.\\-_a-zA-Z0-9]+/?){3,1016}$",
+            "type": "string"
+        },
         "ResolvedAttributes": {
             "documentation": "<p>The resolved attributes.</p>",
             "members": {
                 "AutoMLJobObjective": {
                     "shape": "AutoMLJobObjective"
                 },
                 "CompletionCriteria": {
@@ -27806,44 +29609,40 @@
             "documentation": "<p>Describes the resources, including ML compute instances and ML storage volumes, to use for model training. </p>",
             "members": {
                 "InstanceCount": {
                     "documentation": "<p>The number of ML compute instances to use. For distributed training, provide a value greater than 1. </p>",
                     "shape": "TrainingInstanceCount"
                 },
                 "InstanceGroups": {
-                    "documentation": "<p>The configuration of a heterogeneous cluster in JSON format.</p>",
                     "shape": "InstanceGroups"
                 },
                 "InstanceType": {
                     "documentation": "<p>The ML compute instance type. </p>",
                     "shape": "TrainingInstanceType"
                 },
                 "KeepAlivePeriodInSeconds": {
-                    "documentation": "<p>The duration of time in seconds to retain configured resources in a warm pool for subsequent training jobs.</p>",
                     "shape": "KeepAlivePeriodInSeconds"
                 },
                 "VolumeKmsKeyId": {
-                    "documentation": "<p>The Amazon Web Services KMS key that SageMaker uses to encrypt data on the storage volume attached to the ML compute instance(s) that run the training job.</p> <note> <p>Certain Nitro-based instances include local storage, dependent on the instance type. Local storage volumes are encrypted using a hardware module on the instance. You can't request a <code>VolumeKmsKeyId</code> when using an instance type with local storage.</p> <p>For a list of instance types that support local instance storage, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html#instance-store-volumes\">Instance Store Volumes</a>.</p> <p>For more information about local instance storage encryption, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ssd-instance-store.html\">SSD Instance Store Volumes</a>.</p> </note> <p>The <code>VolumeKmsKeyId</code> can be in any of the following formats:</p> <ul> <li> <p>// KMS Key ID</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> </ul>",
+                    "documentation": "<p>The Amazon Web Services KMS key that Amazon SageMaker uses to encrypt data on the storage volume attached to the ML compute instance(s) that run the training job.</p> <note> <p>Certain Nitro-based instances include local storage, dependent on the instance type. Local storage volumes are encrypted using a hardware module on the instance. You can't request a <code>VolumeKmsKeyId</code> when using an instance type with local storage.</p> <p>For a list of instance types that support local instance storage, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html#instance-store-volumes\">Instance Store Volumes</a>.</p> <p>For more information about local instance storage encryption, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ssd-instance-store.html\">SSD Instance Store Volumes</a>.</p> </note> <p>The <code>VolumeKmsKeyId</code> can be in any of the following formats:</p> <ul> <li> <p>// KMS Key ID</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> </ul>",
                     "shape": "KmsKeyId"
                 },
                 "VolumeSizeInGB": {
-                    "documentation": "<p>The size of the ML storage volume that you want to provision. </p> <p>ML storage volumes store model artifacts and incremental states. Training algorithms might also use the ML storage volume for scratch space. If you want to store the training data in the ML storage volume, choose <code>File</code> as the <code>TrainingInputMode</code> in the algorithm specification. </p> <p>When using an ML instance with <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ssd-instance-store.html#nvme-ssd-volumes\">NVMe SSD volumes</a>, SageMaker doesn't provision Amazon EBS General Purpose SSD (gp2) storage. Available storage is fixed to the NVMe-type instance's storage capacity. SageMaker configures storage paths for training datasets, checkpoints, model artifacts, and outputs to use the entire capacity of the instance storage. For example, ML instance families with the NVMe-type instance storage include <code>ml.p4d</code>, <code>ml.g4dn</code>, and <code>ml.g5</code>. </p> <p>When using an ML instance with the EBS-only storage option and without instance storage, you must define the size of EBS volume through <code>VolumeSizeInGB</code> in the <code>ResourceConfig</code> API. For example, ML instance families that use EBS volumes include <code>ml.c5</code> and <code>ml.p2</code>. </p> <p>To look up instance types and their instance storage types and volumes, see <a href=\"http://aws.amazon.com/ec2/instance-types/\">Amazon EC2 Instance Types</a>.</p> <p>To find the default local paths defined by the SageMaker training platform, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-train-storage.html\">Amazon SageMaker Training Storage Folders for Training Datasets, Checkpoints, Model Artifacts, and Outputs</a>.</p>",
+                    "documentation": "<p>The size of the ML storage volume that you want to provision. </p> <p>ML storage volumes store model artifacts and incremental states. Training algorithms might also use the ML storage volume for scratch space. If you want to store the training data in the ML storage volume, choose <code>File</code> as the <code>TrainingInputMode</code> in the algorithm specification. </p> <p>You must specify sufficient ML storage for your scenario. </p> <note> <p> Amazon SageMaker supports only the General Purpose SSD (gp2) ML storage volume type. </p> </note> <note> <p>Certain Nitro-based instances include local storage with a fixed total size, dependent on the instance type. When using these instances for training, Amazon SageMaker mounts the local instance storage instead of Amazon EBS gp2 storage. You can't request a <code>VolumeSizeInGB</code> greater than the total size of the local instance storage.</p> <p>For a list of instance types that support local instance storage, including the total size per instance type, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html#instance-store-volumes\">Instance Store Volumes</a>.</p> </note>",
                     "shape": "VolumeSizeInGB"
                 }
             },
             "required": [
                 "VolumeSizeInGB"
             ],
             "type": "structure"
         },
         "ResourceConfigForUpdate": {
-            "documentation": "<p>The <code>ResourceConfig</code> to update <code>KeepAlivePeriodInSeconds</code>. Other fields in the <code>ResourceConfig</code> cannot be updated.</p>",
             "members": {
                 "KeepAlivePeriodInSeconds": {
-                    "documentation": "<p>The <code>KeepAlivePeriodInSeconds</code> value specified in the <code>ResourceConfig</code> to update.</p>",
                     "shape": "KeepAlivePeriodInSeconds"
                 }
             },
             "required": [
                 "KeepAlivePeriodInSeconds"
             ],
             "type": "structure"
@@ -27859,15 +29658,15 @@
                 "Message": {
                     "shape": "FailureReason"
                 }
             },
             "type": "structure"
         },
         "ResourceLimitExceeded": {
-            "documentation": "<p> You have exceeded an SageMaker resource limit. For example, you might have too many training jobs created. </p>",
+            "documentation": "<p> You have exceeded an Amazon SageMaker resource limit. For example, you might have too many training jobs created. </p>",
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "FailureReason"
                 }
             },
             "type": "structure"
@@ -27914,15 +29713,15 @@
             "min": 0,
             "type": "integer"
         },
         "ResourceSpec": {
             "documentation": "<p>Specifies the ARN's of a SageMaker image and SageMaker image version, and the instance type that the version runs on.</p>",
             "members": {
                 "InstanceType": {
-                    "documentation": "<p>The instance type that the image version runs on.</p> <note> <p> <b>JupyterServer apps</b> only support the <code>system</code> value.</p> <p>For <b>KernelGateway apps</b>, the <code>system</code> value is translated to <code>ml.t3.medium</code>. KernelGateway apps also support all other values for available instance types.</p> </note>",
+                    "documentation": "<p>The instance type that the image version runs on.</p>",
                     "shape": "AppInstanceType"
                 },
                 "LifecycleConfigArn": {
                     "documentation": "<p> The Amazon Resource Name (ARN) of the Lifecycle Configuration attached to the Resource.</p>",
                     "shape": "StudioLifecycleConfigArn"
                 },
                 "SageMakerImageArn": {
@@ -27939,22 +29738,24 @@
         "ResourceType": {
             "enum": [
                 "TrainingJob",
                 "Experiment",
                 "ExperimentTrial",
                 "ExperimentTrialComponent",
                 "Endpoint",
+                "Model",
                 "ModelPackage",
                 "ModelPackageGroup",
                 "Pipeline",
                 "PipelineExecution",
                 "FeatureGroup",
                 "Project",
                 "FeatureMetadata",
-                "HyperParameterTuningJob"
+                "HyperParameterTuningJob",
+                "ModelCard"
             ],
             "type": "string"
         },
         "ResponseMIMEType": {
             "max": 1024,
             "pattern": "^[-\\w]+\\/.+$",
             "type": "string"
@@ -28078,27 +29879,26 @@
             "documentation": "<p>Describes the S3 data source.</p>",
             "members": {
                 "AttributeNames": {
                     "documentation": "<p>A list of one or more attribute names to use that are found in a specified augmented manifest file.</p>",
                     "shape": "AttributeNames"
                 },
                 "InstanceGroupNames": {
-                    "documentation": "<p>A list of names of instance groups that get data from the S3 data source.</p>",
                     "shape": "InstanceGroupNames"
                 },
                 "S3DataDistributionType": {
-                    "documentation": "<p>If you want SageMaker to replicate the entire dataset on each ML compute instance that is launched for model training, specify <code>FullyReplicated</code>. </p> <p>If you want SageMaker to replicate a subset of data on each ML compute instance that is launched for model training, specify <code>ShardedByS3Key</code>. If there are <i>n</i> ML compute instances launched for a training job, each instance gets approximately 1/<i>n</i> of the number of S3 objects. In this case, model training on each machine uses only the subset of training data. </p> <p>Don't choose more ML compute instances for training than available S3 objects. If you do, some nodes won't get any data and you will pay for nodes that aren't getting any training data. This applies in both File and Pipe modes. Keep this in mind when developing algorithms. </p> <p>In distributed training, where you use multiple ML compute EC2 instances, you might choose <code>ShardedByS3Key</code>. If the algorithm requires copying training data to the ML storage volume (when <code>TrainingInputMode</code> is set to <code>File</code>), this copies 1/<i>n</i> of the number of objects. </p>",
+                    "documentation": "<p>If you want Amazon SageMaker to replicate the entire dataset on each ML compute instance that is launched for model training, specify <code>FullyReplicated</code>. </p> <p>If you want Amazon SageMaker to replicate a subset of data on each ML compute instance that is launched for model training, specify <code>ShardedByS3Key</code>. If there are <i>n</i> ML compute instances launched for a training job, each instance gets approximately 1/<i>n</i> of the number of S3 objects. In this case, model training on each machine uses only the subset of training data. </p> <p>Don't choose more ML compute instances for training than available S3 objects. If you do, some nodes won't get any data and you will pay for nodes that aren't getting any training data. This applies in both File and Pipe modes. Keep this in mind when developing algorithms. </p> <p>In distributed training, where you use multiple ML compute EC2 instances, you might choose <code>ShardedByS3Key</code>. If the algorithm requires copying training data to the ML storage volume (when <code>TrainingInputMode</code> is set to <code>File</code>), this copies 1/<i>n</i> of the number of objects. </p>",
                     "shape": "S3DataDistribution"
                 },
                 "S3DataType": {
-                    "documentation": "<p>If you choose <code>S3Prefix</code>, <code>S3Uri</code> identifies a key name prefix. SageMaker uses all objects that match the specified key name prefix for model training. </p> <p>If you choose <code>ManifestFile</code>, <code>S3Uri</code> identifies an object that is a manifest file containing a list of object keys that you want SageMaker to use for model training. </p> <p>If you choose <code>AugmentedManifestFile</code>, S3Uri identifies an object that is an augmented manifest file in JSON lines format. This file contains the data you want to use for model training. <code>AugmentedManifestFile</code> can only be used if the Channel's input mode is <code>Pipe</code>.</p>",
+                    "documentation": "<p>If you choose <code>S3Prefix</code>, <code>S3Uri</code> identifies a key name prefix. Amazon SageMaker uses all objects that match the specified key name prefix for model training. </p> <p>If you choose <code>ManifestFile</code>, <code>S3Uri</code> identifies an object that is a manifest file containing a list of object keys that you want Amazon SageMaker to use for model training. </p> <p>If you choose <code>AugmentedManifestFile</code>, S3Uri identifies an object that is an augmented manifest file in JSON lines format. This file contains the data you want to use for model training. <code>AugmentedManifestFile</code> can only be used if the Channel's input mode is <code>Pipe</code>.</p>",
                     "shape": "S3DataType"
                 },
                 "S3Uri": {
-                    "documentation": "<p>Depending on the value specified for the <code>S3DataType</code>, identifies either a key name prefix or a manifest. For example: </p> <ul> <li> <p> A key name prefix might look like this: <code>s3://bucketname/exampleprefix</code> </p> </li> <li> <p> A manifest might look like this: <code>s3://bucketname/example.manifest</code> </p> <p> A manifest is an S3 object which is a JSON file consisting of an array of elements. The first element is a prefix which is followed by one or more suffixes. SageMaker appends the suffix elements to the prefix to get a full set of <code>S3Uri</code>. Note that the prefix must be a valid non-empty <code>S3Uri</code> that precludes users from specifying a manifest whose individual <code>S3Uri</code> is sourced from different S3 buckets.</p> <p> The following code example shows a valid manifest format: </p> <p> <code>[ {\"prefix\": \"s3://customer_bucket/some/prefix/\"},</code> </p> <p> <code> \"relative/path/to/custdata-1\",</code> </p> <p> <code> \"relative/path/custdata-2\",</code> </p> <p> <code> ...</code> </p> <p> <code> \"relative/path/custdata-N\"</code> </p> <p> <code>]</code> </p> <p> This JSON is equivalent to the following <code>S3Uri</code> list:</p> <p> <code>s3://customer_bucket/some/prefix/relative/path/to/custdata-1</code> </p> <p> <code>s3://customer_bucket/some/prefix/relative/path/custdata-2</code> </p> <p> <code>...</code> </p> <p> <code>s3://customer_bucket/some/prefix/relative/path/custdata-N</code> </p> <p>The complete set of <code>S3Uri</code> in this manifest is the input data for the channel for this data source. The object that each <code>S3Uri</code> points to must be readable by the IAM role that SageMaker uses to perform tasks on your behalf. </p> </li> </ul>",
+                    "documentation": "<p>Depending on the value specified for the <code>S3DataType</code>, identifies either a key name prefix or a manifest. For example: </p> <ul> <li> <p> A key name prefix might look like this: <code>s3://bucketname/exampleprefix</code> </p> </li> <li> <p> A manifest might look like this: <code>s3://bucketname/example.manifest</code> </p> <p> A manifest is an S3 object which is a JSON file consisting of an array of elements. The first element is a prefix which is followed by one or more suffixes. SageMaker appends the suffix elements to the prefix to get a full set of <code>S3Uri</code>. Note that the prefix must be a valid non-empty <code>S3Uri</code> that precludes users from specifying a manifest whose individual <code>S3Uri</code> is sourced from different S3 buckets.</p> <p> The following code example shows a valid manifest format: </p> <p> <code>[ {\"prefix\": \"s3://customer_bucket/some/prefix/\"},</code> </p> <p> <code> \"relative/path/to/custdata-1\",</code> </p> <p> <code> \"relative/path/custdata-2\",</code> </p> <p> <code> ...</code> </p> <p> <code> \"relative/path/custdata-N\"</code> </p> <p> <code>]</code> </p> <p> This JSON is equivalent to the following <code>S3Uri</code> list:</p> <p> <code>s3://customer_bucket/some/prefix/relative/path/to/custdata-1</code> </p> <p> <code>s3://customer_bucket/some/prefix/relative/path/custdata-2</code> </p> <p> <code>...</code> </p> <p> <code>s3://customer_bucket/some/prefix/relative/path/custdata-N</code> </p> <p>The complete set of <code>S3Uri</code> in this manifest is the input data for the channel for this data source. The object that each <code>S3Uri</code> points to must be readable by the IAM role that Amazon SageMaker uses to perform tasks on your behalf. </p> </li> </ul>",
                     "shape": "S3Uri"
                 }
             },
             "required": [
                 "S3DataType",
                 "S3Uri"
             ],
@@ -28217,21 +30017,25 @@
                     "documentation": "<p>The properties of an experiment.</p>",
                     "shape": "Experiment"
                 },
                 "FeatureGroup": {
                     "shape": "FeatureGroup"
                 },
                 "FeatureMetadata": {
-                    "documentation": "<p>The feature metadata used to search through the features.</p>",
                     "shape": "FeatureMetadata"
                 },
                 "HyperParameterTuningJob": {
-                    "documentation": "<p>The properties of a hyperparameter tuning job.</p>",
                     "shape": "HyperParameterTuningJobSearchEntity"
                 },
+                "Model": {
+                    "shape": "ModelDashboardModel"
+                },
+                "ModelCard": {
+                    "shape": "ModelCard"
+                },
                 "ModelPackage": {
                     "shape": "ModelPackage"
                 },
                 "ModelPackageGroup": {
                     "shape": "ModelPackageGroup"
                 },
                 "Pipeline": {
@@ -28336,30 +30140,30 @@
                 "MaxWaitTimeExceeded",
                 "Updating",
                 "Restarting"
             ],
             "type": "string"
         },
         "SecondaryStatusTransition": {
-            "documentation": "<p>An array element of <a>DescribeTrainingJobResponse$SecondaryStatusTransitions</a>. It provides additional details about a status that the training job has transitioned through. A training job can be in one of several states, for example, starting, downloading, training, or uploading. Within each state, there are a number of intermediate states. For example, within the starting state, SageMaker could be starting the training job or launching the ML instances. These transitional states are referred to as the job's secondary status. </p> <p/>",
+            "documentation": "<p>An array element of <a>DescribeTrainingJobResponse$SecondaryStatusTransitions</a>. It provides additional details about a status that the training job has transitioned through. A training job can be in one of several states, for example, starting, downloading, training, or uploading. Within each state, there are a number of intermediate states. For example, within the starting state, Amazon SageMaker could be starting the training job or launching the ML instances. These transitional states are referred to as the job's secondary status. </p> <p/>",
             "members": {
                 "EndTime": {
                     "documentation": "<p>A timestamp that shows when the training job transitioned out of this secondary status state into another secondary status state or when the training job has ended.</p>",
                     "shape": "Timestamp"
                 },
                 "StartTime": {
                     "documentation": "<p>A timestamp that shows when the training job transitioned to the current secondary status state.</p>",
                     "shape": "Timestamp"
                 },
                 "Status": {
                     "documentation": "<p>Contains a secondary status information from a training job.</p> <p>Status might be one of the following secondary statuses:</p> <dl> <dt>InProgress</dt> <dd> <ul> <li> <p> <code>Starting</code> - Starting the training job.</p> </li> <li> <p> <code>Downloading</code> - An optional stage for algorithms that support <code>File</code> training input mode. It indicates that data is being downloaded to the ML storage volumes.</p> </li> <li> <p> <code>Training</code> - Training is in progress.</p> </li> <li> <p> <code>Uploading</code> - Training is complete and the model artifacts are being uploaded to the S3 location.</p> </li> </ul> </dd> <dt>Completed</dt> <dd> <ul> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> </ul> </dd> <dt>Failed</dt> <dd> <ul> <li> <p> <code>Failed</code> - The training job has failed. The reason for the failure is returned in the <code>FailureReason</code> field of <code>DescribeTrainingJobResponse</code>.</p> </li> </ul> </dd> <dt>Stopped</dt> <dd> <ul> <li> <p> <code>MaxRuntimeExceeded</code> - The job stopped because it exceeded the maximum allowed runtime.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> </dd> <dt>Stopping</dt> <dd> <ul> <li> <p> <code>Stopping</code> - Stopping the training job.</p> </li> </ul> </dd> </dl> <p>We no longer support the following secondary statuses:</p> <ul> <li> <p> <code>LaunchingMLInstances</code> </p> </li> <li> <p> <code>PreparingTrainingStack</code> </p> </li> <li> <p> <code>DownloadingTrainingImage</code> </p> </li> </ul>",
                     "shape": "SecondaryStatus"
                 },
                 "StatusMessage": {
-                    "documentation": "<p>A detailed description of the progress within a secondary status. </p> <p>SageMaker provides secondary statuses and status messages that apply to each of them:</p> <dl> <dt>Starting</dt> <dd> <ul> <li> <p>Starting the training job.</p> </li> <li> <p>Launching requested ML instances.</p> </li> <li> <p>Insufficient capacity error from EC2 while launching instances, retrying!</p> </li> <li> <p>Launched instance was unhealthy, replacing it!</p> </li> <li> <p>Preparing the instances for training.</p> </li> </ul> </dd> <dt>Training</dt> <dd> <ul> <li> <p>Downloading the training image.</p> </li> <li> <p>Training image download completed. Training in progress.</p> </li> </ul> </dd> </dl> <important> <p>Status messages are subject to change. Therefore, we recommend not including them in code that programmatically initiates actions. For examples, don't use status messages in if statements.</p> </important> <p>To have an overview of your training job's progress, view <code>TrainingJobStatus</code> and <code>SecondaryStatus</code> in <a>DescribeTrainingJob</a>, and <code>StatusMessage</code> together. For example, at the start of a training job, you might see the following:</p> <ul> <li> <p> <code>TrainingJobStatus</code> - InProgress</p> </li> <li> <p> <code>SecondaryStatus</code> - Training</p> </li> <li> <p> <code>StatusMessage</code> - Downloading the training image</p> </li> </ul>",
+                    "documentation": "<p>A detailed description of the progress within a secondary status. </p> <p>Amazon SageMaker provides secondary statuses and status messages that apply to each of them:</p> <dl> <dt>Starting</dt> <dd> <ul> <li> <p>Starting the training job.</p> </li> <li> <p>Launching requested ML instances.</p> </li> <li> <p>Insufficient capacity error from EC2 while launching instances, retrying!</p> </li> <li> <p>Launched instance was unhealthy, replacing it!</p> </li> <li> <p>Preparing the instances for training.</p> </li> </ul> </dd> <dt>Training</dt> <dd> <ul> <li> <p>Downloading the training image.</p> </li> <li> <p>Training image download completed. Training in progress.</p> </li> </ul> </dd> </dl> <important> <p>Status messages are subject to change. Therefore, we recommend not including them in code that programmatically initiates actions. For examples, don't use status messages in if statements.</p> </important> <p>To have an overview of your training job's progress, view <code>TrainingJobStatus</code> and <code>SecondaryStatus</code> in <a>DescribeTrainingJob</a>, and <code>StatusMessage</code> together. For example, at the start of a training job, you might see the following:</p> <ul> <li> <p> <code>TrainingJobStatus</code> - InProgress</p> </li> <li> <p> <code>SecondaryStatus</code> - Training</p> </li> <li> <p> <code>StatusMessage</code> - Downloading the training image</p> </li> </ul>",
                     "shape": "StatusMessage"
                 }
             },
             "required": [
                 "Status",
                 "StartTime"
             ],
@@ -28522,14 +30326,52 @@
             "type": "structure"
         },
         "SessionExpirationDurationInSeconds": {
             "max": 43200,
             "min": 1800,
             "type": "integer"
         },
+        "ShadowModeConfig": {
+            "members": {
+                "ShadowModelVariants": {
+                    "shape": "ShadowModelVariantConfigList"
+                },
+                "SourceModelVariantName": {
+                    "shape": "ModelVariantName"
+                }
+            },
+            "required": [
+                "SourceModelVariantName",
+                "ShadowModelVariants"
+            ],
+            "type": "structure"
+        },
+        "ShadowModelVariantConfig": {
+            "members": {
+                "SamplingPercentage": {
+                    "shape": "Percentage"
+                },
+                "ShadowModelVariantName": {
+                    "shape": "ModelVariantName"
+                }
+            },
+            "required": [
+                "ShadowModelVariantName",
+                "SamplingPercentage"
+            ],
+            "type": "structure"
+        },
+        "ShadowModelVariantConfigList": {
+            "max": 1,
+            "member": {
+                "shape": "ShadowModelVariantConfig"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "SharingSettings": {
             "documentation": "<p>Specifies options for sharing SageMaker Studio notebooks. These settings are specified as part of <code>DefaultUserSettings</code> when the <code>CreateDomain</code> API is called, and as part of <code>UserSettings</code> when the <code>CreateUserProfile</code> API is called. When <code>SharingSettings</code> is not specified, notebook sharing isn't allowed.</p>",
             "members": {
                 "NotebookOutputOption": {
                     "documentation": "<p>Whether to include the notebook cell output when sharing the notebook. The default is <code>Disabled</code>.</p>",
                     "shape": "NotebookOutputOption"
                 },
@@ -28607,14 +30449,22 @@
         "SortExperimentsBy": {
             "enum": [
                 "Name",
                 "CreationTime"
             ],
             "type": "string"
         },
+        "SortInferenceExperimentsBy": {
+            "enum": [
+                "Name",
+                "CreationTime",
+                "Status"
+            ],
+            "type": "string"
+        },
         "SortLineageGroupsBy": {
             "enum": [
                 "Name",
                 "CreationTime"
             ],
             "type": "string"
         },
@@ -28650,18 +30500,18 @@
             "enum": [
                 "Name",
                 "CreationTime"
             ],
             "type": "string"
         },
         "SourceAlgorithm": {
-            "documentation": "<p>Specifies an algorithm that was used to create the model package. The algorithm must be either an algorithm resource in your SageMaker account or an algorithm in Amazon Web Services Marketplace that you are subscribed to.</p>",
+            "documentation": "<p>Specifies an algorithm that was used to create the model package. The algorithm must be either an algorithm resource in your Amazon SageMaker account or an algorithm in Amazon Web Services Marketplace that you are subscribed to.</p>",
             "members": {
                 "AlgorithmName": {
-                    "documentation": "<p>The name of an algorithm that was used to create the model package. The algorithm must be either an algorithm resource in your SageMaker account or an algorithm in Amazon Web Services Marketplace that you are subscribed to.</p>",
+                    "documentation": "<p>The name of an algorithm that was used to create the model package. The algorithm must be either an algorithm resource in your Amazon SageMaker account or an algorithm in Amazon Web Services Marketplace that you are subscribed to.</p>",
                     "shape": "ArnOrName"
                 },
                 "ModelDataUrl": {
                     "documentation": "<p>The Amazon S3 path where the model artifacts, which result from model training, are stored. This path must point to a single <code>gzip</code> compressed tar archive (<code>.tar.gz</code> suffix).</p> <note> <p>The model artifacts must be in an S3 bucket that is in the same region as the algorithm.</p> </note>",
                     "shape": "Url"
                 }
             },
@@ -28709,14 +30559,80 @@
             "type": "string"
         },
         "SourceUri": {
             "max": 2048,
             "pattern": ".*",
             "type": "string"
         },
+        "SpaceArn": {
+            "max": 256,
+            "pattern": "arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:space/.*",
+            "type": "string"
+        },
+        "SpaceDetails": {
+            "members": {
+                "CreationTime": {
+                    "shape": "CreationTime"
+                },
+                "DomainId": {
+                    "shape": "DomainId"
+                },
+                "LastModifiedTime": {
+                    "shape": "LastModifiedTime"
+                },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                },
+                "Status": {
+                    "shape": "SpaceStatus"
+                }
+            },
+            "type": "structure"
+        },
+        "SpaceList": {
+            "member": {
+                "shape": "SpaceDetails"
+            },
+            "type": "list"
+        },
+        "SpaceName": {
+            "max": 63,
+            "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,62}",
+            "type": "string"
+        },
+        "SpaceSettings": {
+            "members": {
+                "JupyterServerAppSettings": {
+                    "shape": "JupyterServerAppSettings"
+                },
+                "KernelGatewayAppSettings": {
+                    "shape": "KernelGatewayAppSettings"
+                }
+            },
+            "type": "structure"
+        },
+        "SpaceSortKey": {
+            "enum": [
+                "CreationTime",
+                "LastModifiedTime"
+            ],
+            "type": "string"
+        },
+        "SpaceStatus": {
+            "enum": [
+                "Deleting",
+                "Failed",
+                "InService",
+                "Pending",
+                "Updating",
+                "Update_Failed",
+                "Delete_Failed"
+            ],
+            "type": "string"
+        },
         "SpawnRate": {
             "min": 0,
             "type": "integer"
         },
         "SplitType": {
             "enum": [
                 "None",
@@ -28738,28 +30654,48 @@
                 "STOPPED"
             ],
             "type": "string"
         },
         "StartEdgeDeploymentStageRequest": {
             "members": {
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the edge deployment plan to start.</p>",
                     "shape": "EntityName"
                 },
                 "StageName": {
-                    "documentation": "<p>The name of the stage to start.</p>",
                     "shape": "EntityName"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanName",
                 "StageName"
             ],
             "type": "structure"
         },
+        "StartInferenceExperimentRequest": {
+            "members": {
+                "Name": {
+                    "shape": "InferenceExperimentName"
+                }
+            },
+            "required": [
+                "Name"
+            ],
+            "type": "structure"
+        },
+        "StartInferenceExperimentResponse": {
+            "members": {
+                "InferenceExperimentArn": {
+                    "shape": "InferenceExperimentArn"
+                }
+            },
+            "required": [
+                "InferenceExperimentArn"
+            ],
+            "type": "structure"
+        },
         "StartMonitoringScheduleRequest": {
             "members": {
                 "MonitoringScheduleName": {
                     "documentation": "<p>The name of the schedule to start.</p>",
                     "shape": "MonitoringScheduleName"
                 }
             },
@@ -28797,15 +30733,15 @@
                 },
                 "PipelineExecutionDisplayName": {
                     "documentation": "<p>The display name of the pipeline execution.</p>",
                     "shape": "PipelineExecutionName"
                 },
                 "PipelineName": {
                     "documentation": "<p>The name of the pipeline.</p>",
-                    "shape": "PipelineName"
+                    "shape": "PipelineNameOrArn"
                 },
                 "PipelineParameters": {
                     "documentation": "<p>Contains a list of pipeline parameters. This list can be empty. </p>",
                     "shape": "ParameterList"
                 }
             },
             "required": [
@@ -28882,19 +30818,17 @@
                 "CompilationJobName"
             ],
             "type": "structure"
         },
         "StopEdgeDeploymentStageRequest": {
             "members": {
                 "EdgeDeploymentPlanName": {
-                    "documentation": "<p>The name of the edge deployment plan to stop.</p>",
                     "shape": "EntityName"
                 },
                 "StageName": {
-                    "documentation": "<p>The name of the stage to stop.</p>",
                     "shape": "EntityName"
                 }
             },
             "required": [
                 "EdgeDeploymentPlanName",
                 "StageName"
             ],
@@ -28920,14 +30854,49 @@
                 }
             },
             "required": [
                 "HyperParameterTuningJobName"
             ],
             "type": "structure"
         },
+        "StopInferenceExperimentRequest": {
+            "members": {
+                "DesiredModelVariants": {
+                    "shape": "ModelVariantConfigList"
+                },
+                "DesiredState": {
+                    "shape": "InferenceExperimentStopDesiredState"
+                },
+                "ModelVariantActions": {
+                    "shape": "ModelVariantActionMap"
+                },
+                "Name": {
+                    "shape": "InferenceExperimentName"
+                },
+                "Reason": {
+                    "shape": "InferenceExperimentStatusReason"
+                }
+            },
+            "required": [
+                "Name",
+                "ModelVariantActions"
+            ],
+            "type": "structure"
+        },
+        "StopInferenceExperimentResponse": {
+            "members": {
+                "InferenceExperimentArn": {
+                    "shape": "InferenceExperimentArn"
+                }
+            },
+            "required": [
+                "InferenceExperimentArn"
+            ],
+            "type": "structure"
+        },
         "StopInferenceRecommendationsJobRequest": {
             "members": {
                 "JobName": {
                     "documentation": "<p>The name of the job you want to stop.</p>",
                     "shape": "RecommendationJobName"
                 }
             },
@@ -29032,22 +31001,22 @@
             },
             "required": [
                 "TransformJobName"
             ],
             "type": "structure"
         },
         "StoppingCondition": {
-            "documentation": "<p>Specifies a limit to how long a model training job or model compilation job can run. It also specifies how long a managed spot training job has to complete. When the job reaches the time limit, SageMaker ends the training or compilation job. Use this API to cap model training costs.</p> <p>To stop a training job, SageMaker sends the algorithm the <code>SIGTERM</code> signal, which delays job termination for 120 seconds. Algorithms can use this 120-second window to save the model artifacts, so the results of training are not lost. </p> <p>The training algorithms provided by SageMaker automatically save the intermediate results of a model training job when possible. This attempt to save artifacts is only a best effort case as model might not be in a state from which it can be saved. For example, if training has just started, the model might not be ready to save. When saved, this intermediate data is a valid model artifact. You can use it to create a model with <code>CreateModel</code>.</p> <note> <p>The Neural Topic Model (NTM) currently does not support saving intermediate model artifacts. When training NTMs, make sure that the maximum runtime is sufficient for the training job to complete.</p> </note>",
+            "documentation": "<p>Specifies a limit to how long a model training job or model compilation job can run. It also specifies how long a managed spot training job has to complete. When the job reaches the time limit, Amazon SageMaker ends the training or compilation job. Use this API to cap model training costs.</p> <p>To stop a training job, Amazon SageMaker sends the algorithm the <code>SIGTERM</code> signal, which delays job termination for 120 seconds. Algorithms can use this 120-second window to save the model artifacts, so the results of training are not lost. </p> <p>The training algorithms provided by Amazon SageMaker automatically save the intermediate results of a model training job when possible. This attempt to save artifacts is only a best effort case as model might not be in a state from which it can be saved. For example, if training has just started, the model might not be ready to save. When saved, this intermediate data is a valid model artifact. You can use it to create a model with <code>CreateModel</code>.</p> <note> <p>The Neural Topic Model (NTM) currently does not support saving intermediate model artifacts. When training NTMs, make sure that the maximum runtime is sufficient for the training job to complete.</p> </note>",
             "members": {
                 "MaxRuntimeInSeconds": {
-                    "documentation": "<p>The maximum length of time, in seconds, that a training or compilation job can run before it is stopped.</p> <p>For compilation jobs, if the job does not complete during this time, a <code>TimeOut</code> error is generated. We recommend starting with 900 seconds and increasing as necessary based on your model.</p> <p>For all other jobs, if the job does not complete during this time, SageMaker ends the job. When <code>RetryStrategy</code> is specified in the job request, <code>MaxRuntimeInSeconds</code> specifies the maximum time for all of the attempts in total, not each individual attempt. The default value is 1 day. The maximum value is 28 days.</p> <p>The maximum time that a <code>TrainingJob</code> can run in total, including any time spent publishing metrics or archiving and uploading models after it has been stopped, is 30 days.</p>",
+                    "documentation": "<p>The maximum length of time, in seconds, that a training or compilation job can run.</p> <p>For compilation jobs, if the job does not complete during this time, you will receive a <code>TimeOut</code> error. We recommend starting with 900 seconds and increase as necessary based on your model.</p> <p>For all other jobs, if the job does not complete during this time, Amazon SageMaker ends the job. When <code>RetryStrategy</code> is specified in the job request, <code>MaxRuntimeInSeconds</code> specifies the maximum time for all of the attempts in total, not each individual attempt. The default value is 1 day. The maximum value is 28 days.</p>",
                     "shape": "MaxRuntimeInSeconds"
                 },
                 "MaxWaitTimeInSeconds": {
-                    "documentation": "<p>The maximum length of time, in seconds, that a managed Spot training job has to complete. It is the amount of time spent waiting for Spot capacity plus the amount of time the job can run. It must be equal to or greater than <code>MaxRuntimeInSeconds</code>. If the job does not complete during this time, SageMaker ends the job.</p> <p>When <code>RetryStrategy</code> is specified in the job request, <code>MaxWaitTimeInSeconds</code> specifies the maximum time for all of the attempts in total, not each individual attempt.</p>",
+                    "documentation": "<p>The maximum length of time, in seconds, that a managed Spot training job has to complete. It is the amount of time spent waiting for Spot capacity plus the amount of time the job can run. It must be equal to or greater than <code>MaxRuntimeInSeconds</code>. If the job does not complete during this time, Amazon SageMaker ends the job.</p> <p>When <code>RetryStrategy</code> is specified in the job request, <code>MaxWaitTimeInSeconds</code> specifies the maximum time for all of the attempts in total, not each individual attempt.</p>",
                     "shape": "MaxWaitTimeInSeconds"
                 }
             },
             "type": "structure"
         },
         "String": {
             "type": "string"
@@ -29215,14 +31184,21 @@
                 "PropertyNameQuery": {
                     "documentation": "<p>Defines a property name hint. Only property names that begin with the specified hint are included in the response.</p>",
                     "shape": "PropertyNameQuery"
                 }
             },
             "type": "structure"
         },
+        "TableFormat": {
+            "enum": [
+                "Glue",
+                "Iceberg"
+            ],
+            "type": "string"
+        },
         "TableName": {
             "max": 255,
             "min": 1,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
             "type": "string"
         },
         "Tag": {
@@ -29462,22 +31438,19 @@
         },
         "ThingName": {
             "max": 128,
             "pattern": "[a-zA-Z0-9:_-]+",
             "type": "string"
         },
         "TimeSeriesForecastingSettings": {
-            "documentation": "<p>Time series forecast settings for the SageMaker Canvas app.</p>",
             "members": {
                 "AmazonForecastRoleArn": {
-                    "documentation": "<p>The IAM role that Canvas passes to Amazon Forecast for time series forecasting. By default, Canvas uses the execution role specified in the <code>UserProfile</code> that launches the Canvas app. If an execution role is not specified in the <code>UserProfile</code>, Canvas uses the execution role specified in the Domain that owns the <code>UserProfile</code>. To allow time series forecasting, this IAM role should have the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/security-iam-awsmanpol-canvas.html#security-iam-awsmanpol-AmazonSageMakerCanvasForecastAccess\"> AmazonSageMakerCanvasForecastAccess</a> policy attached and <code>forecast.amazonaws.com</code> added in the trust relationship as a service principal.</p>",
                     "shape": "RoleArn"
                 },
                 "Status": {
-                    "documentation": "<p>Describes whether time series forecasting is enabled or disabled in the Canvas app.</p>",
                     "shape": "FeatureStatus"
                 }
             },
             "type": "structure"
         },
         "Timestamp": {
             "type": "timestamp"
@@ -29643,15 +31616,17 @@
                 "ml.g5.xlarge",
                 "ml.g5.2xlarge",
                 "ml.g5.4xlarge",
                 "ml.g5.8xlarge",
                 "ml.g5.16xlarge",
                 "ml.g5.12xlarge",
                 "ml.g5.24xlarge",
-                "ml.g5.48xlarge"
+                "ml.g5.48xlarge",
+                "ml.trn1.2xlarge",
+                "ml.trn1.32xlarge"
             ],
             "type": "string"
         },
         "TrainingInstanceTypes": {
             "member": {
                 "shape": "TrainingInstanceType"
             },
@@ -29734,15 +31709,15 @@
                     "shape": "Timestamp"
                 },
                 "ModelArtifacts": {
                     "documentation": "<p>Information about the Amazon S3 location that is configured for storing model artifacts.</p>",
                     "shape": "ModelArtifacts"
                 },
                 "OutputDataConfig": {
-                    "documentation": "<p>The S3 path where model artifacts that you configured when creating the job are stored. SageMaker creates subfolders for model artifacts.</p>",
+                    "documentation": "<p>The S3 path where model artifacts that you configured when creating the job are stored. Amazon SageMaker creates subfolders for model artifacts.</p>",
                     "shape": "OutputDataConfig"
                 },
                 "ResourceConfig": {
                     "documentation": "<p>Resources, including ML compute instances and ML storage volumes, that are configured for model training.</p>",
                     "shape": "ResourceConfig"
                 },
                 "RetryStrategy": {
@@ -29750,34 +31725,34 @@
                     "shape": "RetryStrategy"
                 },
                 "RoleArn": {
                     "documentation": "<p>The Amazon Web Services Identity and Access Management (IAM) role configured for the training job.</p>",
                     "shape": "RoleArn"
                 },
                 "SecondaryStatus": {
-                    "documentation": "<p> Provides detailed information about the state of the training job. For detailed information about the secondary status of the training job, see <code>StatusMessage</code> under <a>SecondaryStatusTransition</a>.</p> <p>SageMaker provides primary statuses and secondary statuses that apply to each of them:</p> <dl> <dt>InProgress</dt> <dd> <ul> <li> <p> <code>Starting</code> - Starting the training job.</p> </li> <li> <p> <code>Downloading</code> - An optional stage for algorithms that support <code>File</code> training input mode. It indicates that data is being downloaded to the ML storage volumes.</p> </li> <li> <p> <code>Training</code> - Training is in progress.</p> </li> <li> <p> <code>Uploading</code> - Training is complete and the model artifacts are being uploaded to the S3 location.</p> </li> </ul> </dd> <dt>Completed</dt> <dd> <ul> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> </ul> </dd> <dt>Failed</dt> <dd> <ul> <li> <p> <code>Failed</code> - The training job has failed. The reason for the failure is returned in the <code>FailureReason</code> field of <code>DescribeTrainingJobResponse</code>.</p> </li> </ul> </dd> <dt>Stopped</dt> <dd> <ul> <li> <p> <code>MaxRuntimeExceeded</code> - The job stopped because it exceeded the maximum allowed runtime.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> </dd> <dt>Stopping</dt> <dd> <ul> <li> <p> <code>Stopping</code> - Stopping the training job.</p> </li> </ul> </dd> </dl> <important> <p>Valid values for <code>SecondaryStatus</code> are subject to change. </p> </important> <p>We no longer support the following secondary statuses:</p> <ul> <li> <p> <code>LaunchingMLInstances</code> </p> </li> <li> <p> <code>PreparingTrainingStack</code> </p> </li> <li> <p> <code>DownloadingTrainingImage</code> </p> </li> </ul>",
+                    "documentation": "<p> Provides detailed information about the state of the training job. For detailed information about the secondary status of the training job, see <code>StatusMessage</code> under <a>SecondaryStatusTransition</a>.</p> <p>Amazon SageMaker provides primary statuses and secondary statuses that apply to each of them:</p> <dl> <dt>InProgress</dt> <dd> <ul> <li> <p> <code>Starting</code> - Starting the training job.</p> </li> <li> <p> <code>Downloading</code> - An optional stage for algorithms that support <code>File</code> training input mode. It indicates that data is being downloaded to the ML storage volumes.</p> </li> <li> <p> <code>Training</code> - Training is in progress.</p> </li> <li> <p> <code>Uploading</code> - Training is complete and the model artifacts are being uploaded to the S3 location.</p> </li> </ul> </dd> <dt>Completed</dt> <dd> <ul> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> </ul> </dd> <dt>Failed</dt> <dd> <ul> <li> <p> <code>Failed</code> - The training job has failed. The reason for the failure is returned in the <code>FailureReason</code> field of <code>DescribeTrainingJobResponse</code>.</p> </li> </ul> </dd> <dt>Stopped</dt> <dd> <ul> <li> <p> <code>MaxRuntimeExceeded</code> - The job stopped because it exceeded the maximum allowed runtime.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> </dd> <dt>Stopping</dt> <dd> <ul> <li> <p> <code>Stopping</code> - Stopping the training job.</p> </li> </ul> </dd> </dl> <important> <p>Valid values for <code>SecondaryStatus</code> are subject to change. </p> </important> <p>We no longer support the following secondary statuses:</p> <ul> <li> <p> <code>LaunchingMLInstances</code> </p> </li> <li> <p> <code>PreparingTrainingStack</code> </p> </li> <li> <p> <code>DownloadingTrainingImage</code> </p> </li> </ul>",
                     "shape": "SecondaryStatus"
                 },
                 "SecondaryStatusTransitions": {
                     "documentation": "<p>A history of all of the secondary statuses that the training job has transitioned through.</p>",
                     "shape": "SecondaryStatusTransitions"
                 },
                 "StoppingCondition": {
-                    "documentation": "<p>Specifies a limit to how long a model training job can run. It also specifies how long a managed Spot training job has to complete. When the job reaches the time limit, SageMaker ends the training job. Use this API to cap model training costs.</p> <p>To stop a job, SageMaker sends the algorithm the <code>SIGTERM</code> signal, which delays job termination for 120 seconds. Algorithms can use this 120-second window to save the model artifacts, so the results of training are not lost. </p>",
+                    "documentation": "<p>Specifies a limit to how long a model training job can run. It also specifies how long a managed Spot training job has to complete. When the job reaches the time limit, Amazon SageMaker ends the training job. Use this API to cap model training costs.</p> <p>To stop a job, Amazon SageMaker sends the algorithm the <code>SIGTERM</code> signal, which delays job termination for 120 seconds. Algorithms can use this 120-second window to save the model artifacts, so the results of training are not lost. </p>",
                     "shape": "StoppingCondition"
                 },
                 "Tags": {
                     "documentation": "<p>An array of key-value pairs. You can use tags to categorize your Amazon Web Services resources in different ways, for example, by purpose, owner, or environment. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a>.</p>",
                     "shape": "TagList"
                 },
                 "TensorBoardOutputConfig": {
                     "shape": "TensorBoardOutputConfig"
                 },
                 "TrainingEndTime": {
-                    "documentation": "<p>Indicates the time when the training job ends on training instances. You are billed for the time interval between the value of <code>TrainingStartTime</code> and this time. For successful jobs and stopped jobs, this is the time after model artifacts are uploaded. For failed jobs, this is the time when SageMaker detects a job failure.</p>",
+                    "documentation": "<p>Indicates the time when the training job ends on training instances. You are billed for the time interval between the value of <code>TrainingStartTime</code> and this time. For successful jobs and stopped jobs, this is the time after model artifacts are uploaded. For failed jobs, this is the time when Amazon SageMaker detects a job failure.</p>",
                     "shape": "Timestamp"
                 },
                 "TrainingJobArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the training job.</p>",
                     "shape": "TrainingJobArn"
                 },
                 "TrainingJobName": {
@@ -29820,23 +31795,23 @@
                     "shape": "HyperParameters"
                 },
                 "InputDataConfig": {
                     "documentation": "<p>An array of <code>Channel</code> objects, each of which specifies an input source.</p>",
                     "shape": "InputDataConfig"
                 },
                 "OutputDataConfig": {
-                    "documentation": "<p>the path to the S3 bucket where you want to store model artifacts. SageMaker creates subfolders for the artifacts.</p>",
+                    "documentation": "<p>the path to the S3 bucket where you want to store model artifacts. Amazon SageMaker creates subfolders for the artifacts.</p>",
                     "shape": "OutputDataConfig"
                 },
                 "ResourceConfig": {
                     "documentation": "<p>The resources, including the ML compute instances and ML storage volumes, to use for model training.</p>",
                     "shape": "ResourceConfig"
                 },
                 "StoppingCondition": {
-                    "documentation": "<p>Specifies a limit to how long a model training job can run. It also specifies how long a managed Spot training job has to complete. When the job reaches the time limit, SageMaker ends the training job. Use this API to cap model training costs.</p> <p>To stop a job, SageMaker sends the algorithm the SIGTERM signal, which delays job termination for 120 seconds. Algorithms can use this 120-second window to save the model artifacts.</p>",
+                    "documentation": "<p>Specifies a limit to how long a model training job can run. It also specifies how long a managed Spot training job has to complete. When the job reaches the time limit, Amazon SageMaker ends the training job. Use this API to cap model training costs.</p> <p>To stop a job, Amazon SageMaker sends the algorithm the SIGTERM signal, which delays job termination for 120 seconds. Algorithms can use this 120-second window to save the model artifacts.</p>",
                     "shape": "StoppingCondition"
                 },
                 "TrainingInputMode": {
                     "shape": "TrainingInputMode"
                 }
             },
             "required": [
@@ -29950,15 +31925,14 @@
                     "shape": "TrainingJobName"
                 },
                 "TrainingJobStatus": {
                     "documentation": "<p>The status of the training job.</p>",
                     "shape": "TrainingJobStatus"
                 },
                 "WarmPoolStatus": {
-                    "documentation": "<p>The status of the warm pool associated with the training job.</p>",
                     "shape": "WarmPoolStatus"
                 }
             },
             "required": [
                 "TrainingJobName",
                 "TrainingJobArn",
                 "CreationTime",
@@ -30327,15 +32301,15 @@
                     "shape": "Accept"
                 },
                 "AssembleWith": {
                     "documentation": "<p>Defines how to assemble the results of the transform job as a single S3 object. Choose a format that is most convenient to you. To concatenate the results in binary format, specify <code>None</code>. To add a newline character at the end of every transformed record, specify <code>Line</code>.</p>",
                     "shape": "AssemblyType"
                 },
                 "KmsKeyId": {
-                    "documentation": "<p>The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that Amazon SageMaker uses to encrypt the model artifacts at rest using Amazon S3 server-side encryption. The <code>KmsKeyId</code> can be any of the following formats: </p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias name ARN: <code>arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>If you don't provide a KMS key ID, Amazon SageMaker uses the default KMS key for Amazon S3 for your role's account. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html\">KMS-Managed Encryption Keys</a> in the <i>Amazon Simple Storage Service Developer Guide.</i> </p> <p>The KMS key policy must grant permission to the IAM role that you specify in your <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateModel.html\">CreateModel</a> request. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html\">Using Key Policies in Amazon Web Services KMS</a> in the <i>Amazon Web Services Key Management Service Developer Guide</i>.</p>",
+                    "documentation": "<p>The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that Amazon SageMaker uses to encrypt the model artifacts at rest using Amazon S3 server-side encryption. The <code>KmsKeyId</code> can be any of the following formats: </p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias name ARN: <code>arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>If you don't provide a KMS key ID, Amazon SageMaker uses the default KMS key for Amazon S3 for your role's account. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html\">KMS-Managed Encryption Keys</a> in the <i>Amazon Simple Storage Service Developer Guide.</i> </p> <p>The KMS key policy must grant permission to the IAM role that you specify in your <a>CreateModel</a> request. For more information, see <a href=\"http://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html\">Using Key Policies in Amazon Web Services KMS</a> in the <i>Amazon Web Services Key Management Service Developer Guide</i>.</p>",
                     "shape": "KmsKeyId"
                 },
                 "S3OutputPath": {
                     "documentation": "<p>The Amazon S3 path where you want Amazon SageMaker to store the results of the transform job. For example, <code>s3://bucket-name/key-name-prefix</code>.</p> <p>For every S3 object used as input for the transform job, batch transform stores the transformed data with an .<code>out</code> suffix in a corresponding subfolder in the location in the output prefix. For example, for the input data stored at <code>s3://bucket-name/input-name-prefix/dataset01/data.csv</code>, batch transform stores the transformed data at <code>s3://bucket-name/output-name-prefix/input-name-prefix/data.csv.out</code>. Batch transform doesn't upload partially processed objects. For an input S3 object that contains multiple records, it creates an .<code>out</code> file only if the transform job succeeds on the entire file. When the input contains multiple S3 objects, the batch transform job processes the listed S3 objects and uploads only the output for successfully processed objects. If any object fails in the transform job batch transform marks the job as failed to prompt investigation.</p>",
                     "shape": "S3Uri"
                 }
             },
@@ -30344,15 +32318,15 @@
             ],
             "type": "structure"
         },
         "TransformResources": {
             "documentation": "<p>Describes the resources, including ML instance types and ML instance count, to use for transform job.</p>",
             "members": {
                 "InstanceCount": {
-                    "documentation": "<p>The number of ML compute instances to use in the transform job. The default value is <code>1</code>, and the maximum is <code>100</code>. For distributed transform jobs, specify a value greater than <code>1</code>.</p>",
+                    "documentation": "<p>The number of ML compute instances to use in the transform job. For distributed transform jobs, specify a value greater than 1. The default value is <code>1</code>.</p>",
                     "shape": "TransformInstanceCount"
                 },
                 "InstanceType": {
                     "documentation": "<p>The ML compute instance type for the transform job. If you are using built-in algorithms to transform moderately sized datasets, we recommend using ml.m4.xlarge or <code>ml.m5.large</code>instance types.</p>",
                     "shape": "TransformInstanceType"
                 },
                 "VolumeKmsKeyId": {
@@ -30489,14 +32463,17 @@
                     "documentation": "<p>The hyperparameters of the component.</p>",
                     "shape": "TrialComponentParameters"
                 },
                 "Parents": {
                     "documentation": "<p>An array of the parents of the component. A parent is a trial the component is associated with and the experiment the trial is part of. A component might not have any parents.</p>",
                     "shape": "Parents"
                 },
+                "RunName": {
+                    "shape": "ExperimentEntityName"
+                },
                 "Source": {
                     "documentation": "<p>The Amazon Resource Name (ARN) and job type of the source of the component.</p>",
                     "shape": "TrialComponentSource"
                 },
                 "SourceDetail": {
                     "documentation": "<p>Details of the source of the component.</p>",
                     "shape": "TrialComponentSourceDetail"
@@ -30722,14 +32699,20 @@
                 "TransformJob": {
                     "documentation": "<p>Information about a transform job that's the source of a trial component.</p>",
                     "shape": "TransformJob"
                 }
             },
             "type": "structure"
         },
+        "TrialComponentSources": {
+            "member": {
+                "shape": "TrialComponentSource"
+            },
+            "type": "list"
+        },
         "TrialComponentStatus": {
             "documentation": "<p>The status of the trial component.</p>",
             "members": {
                 "Message": {
                     "documentation": "<p>If the component failed, a message describing why.</p>",
                     "shape": "TrialComponentStatusMessage"
                 },
@@ -31139,14 +33122,17 @@
                 "DeviceFleetName",
                 "Devices"
             ],
             "type": "structure"
         },
         "UpdateDomainRequest": {
             "members": {
+                "DefaultSpaceSettings": {
+                    "shape": "DefaultSpaceSettings"
+                },
                 "DefaultUserSettings": {
                     "documentation": "<p>A collection of settings.</p>",
                     "shape": "UserSettings"
                 },
                 "DomainId": {
                     "documentation": "<p>The ID of the domain to be updated.</p>",
                     "shape": "DomainId"
@@ -31218,15 +33204,15 @@
         "UpdateEndpointWeightsAndCapacitiesInput": {
             "members": {
                 "DesiredWeightsAndCapacities": {
                     "documentation": "<p>An object that provides new capacity and weight values for a variant.</p>",
                     "shape": "DesiredWeightAndCapacityList"
                 },
                 "EndpointName": {
-                    "documentation": "<p>The name of an existing SageMaker endpoint.</p>",
+                    "documentation": "<p>The name of an existing Amazon SageMaker endpoint.</p>",
                     "shape": "EndpointName"
                 }
             },
             "required": [
                 "EndpointName",
                 "DesiredWeightsAndCapacities"
             ],
@@ -31272,59 +33258,51 @@
                 }
             },
             "type": "structure"
         },
         "UpdateFeatureGroupRequest": {
             "members": {
                 "FeatureAdditions": {
-                    "documentation": "<p>Updates the feature group. Updating a feature group is an asynchronous operation. When you get an HTTP 200 response, you've made a valid request. It takes some time after you've made a valid request for Feature Store to update the feature group.</p>",
                     "shape": "FeatureAdditions"
                 },
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group that you're updating.</p>",
                     "shape": "FeatureGroupName"
                 }
             },
             "required": [
                 "FeatureGroupName"
             ],
             "type": "structure"
         },
         "UpdateFeatureGroupResponse": {
             "members": {
                 "FeatureGroupArn": {
-                    "documentation": "<p>The Amazon Resource Number (ARN) of the feature group that you're updating.</p>",
                     "shape": "FeatureGroupArn"
                 }
             },
             "required": [
                 "FeatureGroupArn"
             ],
             "type": "structure"
         },
         "UpdateFeatureMetadataRequest": {
             "members": {
                 "Description": {
-                    "documentation": "<p>A description that you can write to better describe the feature.</p>",
                     "shape": "FeatureDescription"
                 },
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group containing the feature that you're updating.</p>",
                     "shape": "FeatureGroupName"
                 },
                 "FeatureName": {
-                    "documentation": "<p>The name of the feature that you're updating.</p>",
                     "shape": "FeatureName"
                 },
                 "ParameterAdditions": {
-                    "documentation": "<p>A list of key-value pairs that you can add to better describe the feature.</p>",
                     "shape": "FeatureParameterAdditions"
                 },
                 "ParameterRemovals": {
-                    "documentation": "<p>A list of parameter keys that you can specify to remove parameters that describe your feature.</p>",
                     "shape": "FeatureParameterRemovals"
                 }
             },
             "required": [
                 "FeatureGroupName",
                 "FeatureName"
             ],
@@ -31363,14 +33341,79 @@
                 "ImageArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the image.</p>",
                     "shape": "ImageArn"
                 }
             },
             "type": "structure"
         },
+        "UpdateInferenceExperimentRequest": {
+            "members": {
+                "DataStorageConfig": {
+                    "shape": "InferenceExperimentDataStorageConfig"
+                },
+                "Description": {
+                    "shape": "InferenceExperimentDescription"
+                },
+                "ModelVariants": {
+                    "shape": "ModelVariantConfigList"
+                },
+                "Name": {
+                    "shape": "InferenceExperimentName"
+                },
+                "Schedule": {
+                    "shape": "InferenceExperimentSchedule"
+                },
+                "ShadowModeConfig": {
+                    "shape": "ShadowModeConfig"
+                }
+            },
+            "required": [
+                "Name"
+            ],
+            "type": "structure"
+        },
+        "UpdateInferenceExperimentResponse": {
+            "members": {
+                "InferenceExperimentArn": {
+                    "shape": "InferenceExperimentArn"
+                }
+            },
+            "required": [
+                "InferenceExperimentArn"
+            ],
+            "type": "structure"
+        },
+        "UpdateModelCardRequest": {
+            "members": {
+                "Content": {
+                    "shape": "ModelCardContent"
+                },
+                "ModelCardName": {
+                    "shape": "EntityName"
+                },
+                "ModelCardStatus": {
+                    "shape": "ModelCardStatus"
+                }
+            },
+            "required": [
+                "ModelCardName"
+            ],
+            "type": "structure"
+        },
+        "UpdateModelCardResponse": {
+            "members": {
+                "ModelCardArn": {
+                    "shape": "ModelCardArn"
+                }
+            },
+            "required": [
+                "ModelCardArn"
+            ],
+            "type": "structure"
+        },
         "UpdateModelPackageInput": {
             "members": {
                 "AdditionalInferenceSpecificationsToAdd": {
                     "documentation": "<p>An array of additional Inference Specification objects to be added to the existing array additional Inference Specification. Total number of additional Inference Specifications can not exceed 15. Each additional Inference Specification specifies artifacts based on this model package that can be used on inference endpoints. Generally used with SageMaker Neo to store the compiled artifacts.</p>",
                     "shape": "AdditionalInferenceSpecifications"
                 },
                 "ApprovalDescription": {
@@ -31407,14 +33450,51 @@
                 }
             },
             "required": [
                 "ModelPackageArn"
             ],
             "type": "structure"
         },
+        "UpdateMonitoringAlertRequest": {
+            "members": {
+                "DatapointsToAlert": {
+                    "shape": "MonitoringDatapointsToAlert"
+                },
+                "EvaluationPeriod": {
+                    "shape": "MonitoringEvaluationPeriod"
+                },
+                "MonitoringAlertName": {
+                    "shape": "MonitoringAlertName"
+                },
+                "MonitoringScheduleName": {
+                    "shape": "MonitoringScheduleName"
+                }
+            },
+            "required": [
+                "MonitoringScheduleName",
+                "MonitoringAlertName",
+                "DatapointsToAlert",
+                "EvaluationPeriod"
+            ],
+            "type": "structure"
+        },
+        "UpdateMonitoringAlertResponse": {
+            "members": {
+                "MonitoringAlertName": {
+                    "shape": "MonitoringAlertName"
+                },
+                "MonitoringScheduleArn": {
+                    "shape": "MonitoringScheduleArn"
+                }
+            },
+            "required": [
+                "MonitoringScheduleArn"
+            ],
+            "type": "structure"
+        },
         "UpdateMonitoringScheduleRequest": {
             "members": {
                 "MonitoringScheduleConfig": {
                     "documentation": "<p>The configuration object that specifies the monitoring schedule and defines the monitoring job.</p>",
                     "shape": "MonitoringScheduleConfig"
                 },
                 "MonitoringScheduleName": {
@@ -31443,19 +33523,19 @@
         "UpdateNotebookInstanceInput": {
             "members": {
                 "AcceleratorTypes": {
                     "documentation": "<p>A list of the Elastic Inference (EI) instance types to associate with this notebook instance. Currently only one EI instance type can be associated with a notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/ei.html\">Using Elastic Inference in Amazon SageMaker</a>.</p>",
                     "shape": "NotebookInstanceAcceleratorTypes"
                 },
                 "AdditionalCodeRepositories": {
-                    "documentation": "<p>An array of up to three Git repositories to associate with the notebook instance. These can be either the names of Git repositories stored as resources in your account, or the URL of Git repositories in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. These repositories are cloned at the same level as the default repository of your notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with SageMaker Notebook Instances</a>.</p>",
+                    "documentation": "<p>An array of up to three Git repositories to associate with the notebook instance. These can be either the names of Git repositories stored as resources in your account, or the URL of Git repositories in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. These repositories are cloned at the same level as the default repository of your notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with Amazon SageMaker Notebook Instances</a>.</p>",
                     "shape": "AdditionalCodeRepositoryNamesOrUrls"
                 },
                 "DefaultCodeRepository": {
-                    "documentation": "<p>The Git repository to associate with the notebook instance as its default code repository. This can be either the name of a Git repository stored as a resource in your account, or the URL of a Git repository in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. When you open a notebook instance, it opens in the directory that contains this repository. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with SageMaker Notebook Instances</a>.</p>",
+                    "documentation": "<p>The Git repository to associate with the notebook instance as its default code repository. This can be either the name of a Git repository stored as a resource in your account, or the URL of a Git repository in <a href=\"https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html\">Amazon Web Services CodeCommit</a> or in any other Git repository. When you open a notebook instance, it opens in the directory that contains this repository. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html\">Associating Git Repositories with Amazon SageMaker Notebook Instances</a>.</p>",
                     "shape": "CodeRepositoryNameOrUrl"
                 },
                 "DisassociateAcceleratorTypes": {
                     "documentation": "<p>A list of the Elastic Inference (EI) instance types to remove from this notebook instance. This operation is idempotent. If you specify an accelerator type that is not associated with the notebook instance when you call this method, it does not throw an error.</p>",
                     "shape": "DisassociateNotebookInstanceAcceleratorTypes"
                 },
                 "DisassociateAdditionalCodeRepositories": {
@@ -31467,15 +33547,14 @@
                     "shape": "DisassociateDefaultCodeRepository"
                 },
                 "DisassociateLifecycleConfig": {
                     "documentation": "<p>Set to <code>true</code> to remove the notebook instance lifecycle configuration currently associated with the notebook instance. This operation is idempotent. If you specify a lifecycle configuration that is not associated with the notebook instance when you call this method, it does not throw an error.</p>",
                     "shape": "DisassociateNotebookInstanceLifecycleConfig"
                 },
                 "InstanceMetadataServiceConfiguration": {
-                    "documentation": "<p>Information on the IMDS configuration of the notebook instance</p>",
                     "shape": "InstanceMetadataServiceConfiguration"
                 },
                 "InstanceType": {
                     "documentation": "<p>The Amazon ML compute instance type.</p>",
                     "shape": "InstanceType"
                 },
                 "LifecycleConfigName": {
@@ -31483,23 +33562,23 @@
                     "shape": "NotebookInstanceLifecycleConfigName"
                 },
                 "NotebookInstanceName": {
                     "documentation": "<p>The name of the notebook instance to update.</p>",
                     "shape": "NotebookInstanceName"
                 },
                 "RoleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that SageMaker can assume to access the notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html\">SageMaker Roles</a>. </p> <note> <p>To be able to pass this role to SageMaker, the caller of this API must have the <code>iam:PassRole</code> permission.</p> </note>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that Amazon SageMaker can assume to access the notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html\">Amazon SageMaker Roles</a>. </p> <note> <p>To be able to pass this role to Amazon SageMaker, the caller of this API must have the <code>iam:PassRole</code> permission.</p> </note>",
                     "shape": "RoleArn"
                 },
                 "RootAccess": {
                     "documentation": "<p>Whether root access is enabled or disabled for users of the notebook instance. The default value is <code>Enabled</code>.</p> <note> <p>If you set this to <code>Disabled</code>, users don't have root access on the notebook instance, but lifecycle configuration scripts still run with root permissions.</p> </note>",
                     "shape": "RootAccess"
                 },
                 "VolumeSizeInGB": {
-                    "documentation": "<p>The size, in GB, of the ML storage volume to attach to the notebook instance. The default value is 5 GB. ML storage volumes are encrypted, so SageMaker can't determine the amount of available free space on the volume. Because of this, you can increase the volume size when you update a notebook instance, but you can't decrease the volume size. If you want to decrease the size of the ML storage volume in use, create a new notebook instance with the desired size.</p>",
+                    "documentation": "<p>The size, in GB, of the ML storage volume to attach to the notebook instance. The default value is 5 GB. ML storage volumes are encrypted, so Amazon SageMaker can't determine the amount of available free space on the volume. Because of this, you can increase the volume size when you update a notebook instance, but you can't decrease the volume size. If you want to decrease the size of the ML storage volume in use, create a new notebook instance with the desired size.</p>",
                     "shape": "NotebookInstanceVolumeSizeInGB"
                 }
             },
             "required": [
                 "NotebookInstanceName"
             ],
             "type": "structure"
@@ -31621,15 +33700,15 @@
                     "shape": "ProjectEntityName"
                 },
                 "ServiceCatalogProvisioningUpdateDetails": {
                     "documentation": "<p>The product ID and provisioning artifact ID to provision a service catalog. The provisioning artifact ID will default to the latest provisioning artifact ID of the product, if you don't provide the provisioning artifact ID. For more information, see <a href=\"https://docs.aws.amazon.com/servicecatalog/latest/adminguide/introduction.html\">What is Amazon Web Services Service Catalog</a>. </p>",
                     "shape": "ServiceCatalogProvisioningUpdateDetails"
                 },
                 "Tags": {
-                    "documentation": "<p>An array of key-value pairs. You can use tags to categorize your Amazon Web Services resources in different ways, for example, by purpose, owner, or environment. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a>. In addition, the project must have tag update constraints set in order to include this parameter in the request. For more information, see <a href=\"https://docs.aws.amazon.com/servicecatalog/latest/adminguide/constraints-resourceupdate.html\">Amazon Web Services Service Catalog Tag Update Constraints</a>.</p>",
+                    "documentation": "<p>An array of key-value pairs. You can use tags to categorize your Amazon Web Services resources in different ways, for example, by purpose, owner, or environment. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a>.</p>",
                     "shape": "TagList"
                 }
             },
             "required": [
                 "ProjectName"
             ],
             "type": "structure"
@@ -31642,26 +33721,51 @@
                 }
             },
             "required": [
                 "ProjectArn"
             ],
             "type": "structure"
         },
+        "UpdateSpaceRequest": {
+            "members": {
+                "DomainId": {
+                    "shape": "DomainId"
+                },
+                "SpaceName": {
+                    "shape": "SpaceName"
+                },
+                "SpaceSettings": {
+                    "shape": "SpaceSettings"
+                }
+            },
+            "required": [
+                "DomainId",
+                "SpaceName"
+            ],
+            "type": "structure"
+        },
+        "UpdateSpaceResponse": {
+            "members": {
+                "SpaceArn": {
+                    "shape": "SpaceArn"
+                }
+            },
+            "type": "structure"
+        },
         "UpdateTrainingJobRequest": {
             "members": {
                 "ProfilerConfig": {
                     "documentation": "<p>Configuration information for Debugger system monitoring, framework profiling, and storage paths.</p>",
                     "shape": "ProfilerConfigForUpdate"
                 },
                 "ProfilerRuleConfigurations": {
                     "documentation": "<p>Configuration information for Debugger rules for profiling system and framework metrics.</p>",
                     "shape": "ProfilerRuleConfigurations"
                 },
                 "ResourceConfig": {
-                    "documentation": "<p>The training job <code>ResourceConfig</code> to update warm pool retention length.</p>",
                     "shape": "ResourceConfigForUpdate"
                 },
                 "TrainingJobName": {
                     "documentation": "<p>The name of a training job to update the Debugger profiling configuration.</p>",
                     "shape": "TrainingJobName"
                 }
             },
@@ -31809,15 +33913,14 @@
                     "shape": "SourceIpConfig"
                 },
                 "WorkforceName": {
                     "documentation": "<p>The name of the private workforce that you want to update. You can find your workforce name by using the operation.</p>",
                     "shape": "WorkforceName"
                 },
                 "WorkforceVpcConfig": {
-                    "documentation": "<p>Use this parameter to update your VPC configuration for a workforce.</p>",
                     "shape": "WorkforceVpcConfigRequest"
                 }
             },
             "required": [
                 "WorkforceName"
             ],
             "type": "structure"
@@ -31954,15 +34057,14 @@
             ],
             "type": "string"
         },
         "UserSettings": {
             "documentation": "<p>A collection of settings that apply to users of Amazon SageMaker Studio. These settings are specified when the <code>CreateUserProfile</code> API is called, and as <code>DefaultUserSettings</code> when the <code>CreateDomain</code> API is called.</p> <p> <code>SecurityGroups</code> is aggregated when specified in both calls. For all other settings in <code>UserSettings</code>, the values specified in <code>CreateUserProfile</code> take precedence over those specified in <code>CreateDomain</code>.</p>",
             "members": {
                 "CanvasAppSettings": {
-                    "documentation": "<p>The Canvas app settings.</p>",
                     "shape": "CanvasAppSettings"
                 },
                 "ExecutionRole": {
                     "documentation": "<p>The execution role for the user.</p>",
                     "shape": "RoleArn"
                 },
                 "JupyterServerAppSettings": {
@@ -32135,26 +34237,22 @@
                 "Terminated",
                 "Reused",
                 "InUse"
             ],
             "type": "string"
         },
         "WarmPoolStatus": {
-            "documentation": "<p>Status and billing information about the warm pool.</p>",
             "members": {
                 "ResourceRetainedBillableTimeInSeconds": {
-                    "documentation": "<p>The billable time in seconds used by the warm pool. Billable time refers to the absolute wall-clock time.</p> <p>Multiply <code>ResourceRetainedBillableTimeInSeconds</code> by the number of instances (<code>InstanceCount</code>) in your training cluster to get the total compute time SageMaker bills you if you run warm pool training. The formula is as follows: <code>ResourceRetainedBillableTimeInSeconds * InstanceCount</code>.</p>",
                     "shape": "ResourceRetainedBillableTimeInSeconds"
                 },
                 "ReusedByJob": {
-                    "documentation": "<p>The name of the matching training job that reused the warm pool.</p>",
                     "shape": "TrainingJobName"
                 },
                 "Status": {
-                    "documentation": "<p>The status of the warm pool.</p> <ul> <li> <p> <code>InUse</code>: The warm pool is in use for the training job.</p> </li> <li> <p> <code>Available</code>: The warm pool is available to reuse for a matching training job.</p> </li> <li> <p> <code>Reused</code>: The warm pool moved to a matching training job for reuse.</p> </li> <li> <p> <code>Terminated</code>: The warm pool is no longer available. Warm pools are unavailable if they are terminated by a user, terminated for a patch update, or terminated for exceeding the specified <code>KeepAlivePeriodInSeconds</code>.</p> </li> </ul>",
                     "shape": "WarmPoolResourceStatus"
                 }
             },
             "required": [
                 "Status"
             ],
             "type": "structure"
@@ -32167,15 +34265,14 @@
                     "shape": "CognitoConfig"
                 },
                 "CreateDate": {
                     "documentation": "<p>The date that the workforce is created.</p>",
                     "shape": "Timestamp"
                 },
                 "FailureReason": {
-                    "documentation": "<p>The reason your workforce failed.</p>",
                     "shape": "WorkforceFailureReason"
                 },
                 "LastUpdatedDate": {
                     "documentation": "<p>The most recent date that was used to successfully add one or more IP address ranges (<a href=\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html\">CIDRs</a>) to a private workforce's allow list.</p>",
                     "shape": "Timestamp"
                 },
                 "OidcConfig": {
@@ -32183,15 +34280,14 @@
                     "shape": "OidcConfigForResponse"
                 },
                 "SourceIpConfig": {
                     "documentation": "<p>A list of one to ten IP address ranges (<a href=\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html\">CIDRs</a>) to be added to the workforce allow list. By default, a workforce isn't restricted to specific IP addresses.</p>",
                     "shape": "SourceIpConfig"
                 },
                 "Status": {
-                    "documentation": "<p>The status of your workforce.</p>",
                     "shape": "WorkforceStatus"
                 },
                 "SubDomain": {
                     "documentation": "<p>The subdomain for your OIDC Identity Provider.</p>",
                     "shape": "String"
                 },
                 "WorkforceArn": {
@@ -32199,15 +34295,14 @@
                     "shape": "WorkforceArn"
                 },
                 "WorkforceName": {
                     "documentation": "<p>The name of the private workforce.</p>",
                     "shape": "WorkforceName"
                 },
                 "WorkforceVpcConfig": {
-                    "documentation": "<p>The configuration of a VPC workforce.</p>",
                     "shape": "WorkforceVpcConfigResponse"
                 }
             },
             "required": [
                 "WorkforceName",
                 "WorkforceArn"
             ],
@@ -32263,48 +34358,39 @@
             "member": {
                 "shape": "WorkforceSubnetId"
             },
             "min": 1,
             "type": "list"
         },
         "WorkforceVpcConfigRequest": {
-            "documentation": "<p>The VPC object you use to create or update a workforce.</p>",
             "members": {
                 "SecurityGroupIds": {
-                    "documentation": "<p>The VPC security group IDs, in the form sg-xxxxxxxx. The security groups must be for the same VPC as specified in the subnet.</p>",
                     "shape": "WorkforceSecurityGroupIds"
                 },
                 "Subnets": {
-                    "documentation": "<p>The ID of the subnets in the VPC that you want to connect.</p>",
                     "shape": "WorkforceSubnets"
                 },
                 "VpcId": {
-                    "documentation": "<p>The ID of the VPC that the workforce uses for communication.</p>",
                     "shape": "WorkforceVpcId"
                 }
             },
             "type": "structure"
         },
         "WorkforceVpcConfigResponse": {
-            "documentation": "<p>A VpcConfig object that specifies the VPC that you want your workforce to connect to.</p>",
             "members": {
                 "SecurityGroupIds": {
-                    "documentation": "<p>The VPC security group IDs, in the form sg-xxxxxxxx. The security groups must be for the same VPC as specified in the subnet.</p>",
                     "shape": "WorkforceSecurityGroupIds"
                 },
                 "Subnets": {
-                    "documentation": "<p>The ID of the subnets in the VPC that you want to connect.</p>",
                     "shape": "WorkforceSubnets"
                 },
                 "VpcEndpointId": {
-                    "documentation": "<p>The IDs for the VPC service endpoints of your VPC workforce when it is created and updated.</p>",
                     "shape": "WorkforceVpcEndpointId"
                 },
                 "VpcId": {
-                    "documentation": "<p>The ID of the VPC that the workforce uses for communication.</p>",
                     "shape": "WorkforceVpcId"
                 }
             },
             "required": [
                 "VpcId",
                 "SecurityGroupIds",
                 "Subnets"
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/clients.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/clients.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/cron_util.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/cron_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/deletable_resource.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/deletable_resource.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/environment_detector.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/environment_detector.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/environments.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/error_util.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/error_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/extension.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/extension.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/file_uploader.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/file_uploader.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/handlers.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/handlers.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/package.json` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9659722222222222%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9f672e548acd2153a221.js'}}",*

 * * "'version'": "'2.0.2'"}*

```diff
@@ -61,15 +61,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a68376e83adb25bf29b1.js"
+            "load": "static/remoteEntry.9f672e548acd2153a221.js"
         },
         "disabledExtensions": [
             "@jupyterlab/scheduler:IAdvancedOptions"
         ],
         "extension": true,
         "outputDir": "amazon_sagemaker_jupyter_scheduler/labextension",
         "schemaDir": "schema",
@@ -110,9 +110,9 @@
         "test": "jest",
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "2.0.1"
+    "version": "2.0.2"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'2.0.2'"}*

```diff
@@ -106,9 +106,9 @@
         "test": "jest",
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "2.0.1"
+    "version": "2.0.2"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/993.faa5510ce9696a850c76.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/993.faa5510ce9696a850c76.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.a68376e83adb25bf29b1.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.9f672e548acd2153a221.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, i, u, l, f, d, s, c, p, h, b, m, v, g = {
-            8184: (e, r, t) => {
+            5700: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(349), t.e(509), t.e(86), t.e(271), t.e(456), t.e(993)]).then((() => () => t(7993))),
                         "./extension": () => Promise.all([t.e(349), t.e(509), t.e(86), t.e(271), t.e(456), t.e(993)]).then((() => () => t(7993)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
@@ -123,15 +123,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("@amzn/sagemaker-jupyter-scheduler", "2.0.1", (() => Promise.all([w.e(349), w.e(509), w.e(86), w.e(271), w.e(456), w.e(993)]).then((() => () => w(7993))))), u("@emotion/css", "11.10.5", (() => Promise.all([w.e(509), w.e(615)]).then((() => () => w(4615))))), u("@material-ui/core", "4.12.4", (() => Promise.all([w.e(193), w.e(349), w.e(271), w.e(456)]).then((() => () => w(3193))))), u("react-router-dom", "5.3.4", (() => Promise.all([w.e(240), w.e(271), w.e(915)]).then((() => () => w(7240)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@amzn/sagemaker-jupyter-scheduler", "2.0.2", (() => Promise.all([w.e(349), w.e(509), w.e(86), w.e(271), w.e(456), w.e(993)]).then((() => () => w(7993))))), u("@emotion/css", "11.10.5", (() => Promise.all([w.e(509), w.e(615)]).then((() => () => w(4615))))), u("@material-ui/core", "4.12.4", (() => Promise.all([w.e(193), w.e(349), w.e(271), w.e(456)]).then((() => () => w(3193))))), u("react-router-dom", "5.3.4", (() => Promise.all([w.e(240), w.e(271), w.e(915)]).then((() => () => w(7240)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -299,10 +299,10 @@
                     u && u(w)
                 }
                 for (r && r(t); l < o.length; l++) n = o[l], w.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyter_scheduler = self.webpackChunk_amzn_sagemaker_jupyter_scheduler || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var j = w(8184);
+    var j = w(5700);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyter-scheduler"] = j
 })();
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/logging.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/logging.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/model_converter.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/model_converter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/models.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/models.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/revenue.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/revenue.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/providers/tags.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/tags.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/scheduler.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler/utils.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-sagemaker-jupyter-scheduler
-Version: 2.0.1
+Version: 2.0.2
 Summary: Amazon SageMaker Jupyter Scheduler based on the https://pypi.org/project/jupyter-scheduler/
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Scheduling Notebooks,Notebooks,Amazon Sagemaker
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt` & `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt
 amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js.LICENSE.txt
 amazon_sagemaker_jupyter_scheduler/labextension/static/993.faa5510ce9696a850c76.js
-amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.a68376e83adb25bf29b1.js
+amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.9f672e548acd2153a221.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
 amazon_sagemaker_jupyter_scheduler/providers/__init__.py
 amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
 amazon_sagemaker_jupyter_scheduler/providers/revenue.py
 amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
 amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/jest.config.base.js` & `amazon_sagemaker_jupyter_scheduler-2.0.2/jest.config.base.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/package-lock.json` & `amazon_sagemaker_jupyter_scheduler-2.0.2/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.916663640764948%*

 * *Differences: {"'packages'": "{'': {'version': '2.0.2'}}", "'version'": "'2.0.2'"}*

```diff
@@ -11856,15 +11856,15 @@
                 "jest": "^27.2.4",
                 "npm-run-all": "^4.1.5",
                 "ts-jest": "^27.0.5",
                 "typescript": "^4.9.5"
             },
             "license": "Apache 2.0",
             "name": "@amzn/sagemaker-jupyter-scheduler",
-            "version": "2.0.1"
+            "version": "2.0.2"
         },
         "node_modules/@adobe/css-tools": {
             "dev": true,
             "integrity": "sha512-E09FiIft46CmH5Qnjb0wsW54/YQd69LsxeKUOWawmws1XWvyFGURnAChH0mlr7YPFR1ofwvUQfcL0J3lMxXqPA==",
             "license": "MIT",
             "version": "4.2.0"
         },
@@ -29020,9 +29020,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "license": "MIT",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "2.0.1"
+    "version": "2.0.2"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/package.json` & `amazon_sagemaker_jupyter_scheduler-2.0.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'2.0.2'"}*

```diff
@@ -106,9 +106,9 @@
         "test": "jest",
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "2.0.1"
+    "version": "2.0.2"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/setup.py` & `amazon_sagemaker_jupyter_scheduler-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/__tests__/CreateNotebookJobForm.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/CreateNotebookJobForm.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/__tests__/VpcCheckbox.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/VpcCheckbox.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/__tests__/initalValueHelpers.spec.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/initalValueHelpers.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/__tests__/validationHelpers.spec.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/validationHelpers.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/Link.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/Link.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/RouterLink.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/RouterLink.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/__test__/Link.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/__test__/Link.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/link/__test__/RouterLink.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/__test__/RouterLink.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/selectinput/SelectInput.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/SelectInput.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/selectinput/types.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/types.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/textinput/TextInput.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/TextInput.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/textinput/__tests__/TextInput.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/__tests__/TextInput.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/textinput/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/tooltip/Tooltip.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/tooltip/__tests__/Tooltip.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/__tests__/Tooltip.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/components/tooltip/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/constants/common.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/constants/common.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/plugins/ScheduleNotebookDisablerPlugin.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/ScheduleNotebookDisablerPlugin.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/plugins/ScheduleNotebookPlugin.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/ScheduleNotebookPlugin.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/themeProvider.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/themeProvider.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/PluginEnvironmentProvider.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/PluginEnvironmentProvider.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/images.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/images.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/kernels.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/kernels.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/utils/rendering.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/rendering.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJob.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJob.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/InputContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/InputContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/CreateNotebookJobForm/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/mockResponses.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/mockResponses.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/src/widgets/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.1/tsconfig.base.json` & `amazon_sagemaker_jupyter_scheduler-2.0.2/tsconfig.base.json`

 * *Files identical despite different names*

