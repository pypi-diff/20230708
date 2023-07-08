# Comparing `tmp/noiseflow-0.0.6b0.tar.gz` & `tmp/noiseflow-0.0.7a2-cp311-cp311-manylinux_2_35_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noiseflow-0.0.6b0.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

