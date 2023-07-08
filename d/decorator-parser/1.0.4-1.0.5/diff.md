# Comparing `tmp/decorator_parser-1.0.4.tar.gz` & `tmp/decorator_parser-1.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorator_parser-1.0.4.tar", last modified: Mon Jun 26 10:31:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

