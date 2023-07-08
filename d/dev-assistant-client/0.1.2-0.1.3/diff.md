# Comparing `tmp/dev-assistant-client-0.1.2.tar.gz` & `tmp/dev_assistant_client-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-assistant-client-0.1.2.tar", last modified: Fri Jun 30 21:51:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

