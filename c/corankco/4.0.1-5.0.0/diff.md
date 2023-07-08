# Comparing `tmp/corankco-4.0.1.tar.gz` & `tmp/corankco-5.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corankco-4.0.1.tar", last modified: Thu Dec  2 00:57:35 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

