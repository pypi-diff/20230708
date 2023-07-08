# Comparing `tmp/botocore-a-la-carte-snow-device-management-1.31.0.tar.gz` & `tmp/botocore_a_la_carte_snow_device_management-1.31.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-snow-device-management-1.31.0.tar", last modified: Fri Jul  7 01:44:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

