# Comparing `tmp/imagecodecs_numcodecs-2023.3.16-py3-none-any.whl.zip` & `tmp/imagecodecs_numcodecs-2023.7.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2140 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1009 b- defN 23-Mar-17 01:20 imagecodecs_numcodecs-2023.3.16.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-17 01:20 imagecodecs_numcodecs-2023.3.16.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2367 b- defN 23-Mar-17 01:20 imagecodecs_numcodecs-2023.3.16.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Mar-17 01:20 imagecodecs_numcodecs-2023.3.16.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      484 b- defN 23-Mar-17 01:20 imagecodecs_numcodecs-2023.3.16.dist-info/RECORD
-5 files, 3953 bytes uncompressed, 1222 bytes compressed:  69.1%
+Zip file size: 2639 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     3889 b- defN 23-Jul-08 01:13 imagecodecs_numcodecs-2023.7.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-08 01:13 imagecodecs_numcodecs-2023.7.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2411 b- defN 23-Jul-08 01:13 imagecodecs_numcodecs-2023.7.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-08 01:13 imagecodecs_numcodecs-2023.7.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      479 b- defN 23-Jul-08 01:13 imagecodecs_numcodecs-2023.7.4.dist-info/RECORD
+5 files, 6872 bytes uncompressed, 1731 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: imagecodecs_numcodecs-2023.3.16.dist-info/METADATA
+Filename: imagecodecs_numcodecs-2023.7.4.dist-info/METADATA
 Comment: 
 
-Filename: imagecodecs_numcodecs-2023.3.16.dist-info/WHEEL
+Filename: imagecodecs_numcodecs-2023.7.4.dist-info/WHEEL
 Comment: 
 
-Filename: imagecodecs_numcodecs-2023.3.16.dist-info/entry_points.txt
+Filename: imagecodecs_numcodecs-2023.7.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: imagecodecs_numcodecs-2023.3.16.dist-info/top_level.txt
+Filename: imagecodecs_numcodecs-2023.7.4.dist-info/top_level.txt
 Comment: 
 
-Filename: imagecodecs_numcodecs-2023.3.16.dist-info/RECORD
+Filename: imagecodecs_numcodecs-2023.7.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `imagecodecs_numcodecs-2023.3.16.dist-info/entry_points.txt` & `imagecodecs_numcodecs-2023.7.4.dist-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 imagecodecs_bitshuffle = imagecodecs.numcodecs:Bitshuffle
 imagecodecs_blosc = imagecodecs.numcodecs:Blosc
 imagecodecs_blosc2 = imagecodecs.numcodecs:Blosc2
 imagecodecs_brotli = imagecodecs.numcodecs:Brotli
 imagecodecs_byteshuffle = imagecodecs.numcodecs:Byteshuffle
 imagecodecs_bz2 = imagecodecs.numcodecs:Bz2
 imagecodecs_cms = imagecodecs.numcodecs:Cms
+imagecodecs_dds = imagecodecs.numcodecs:Dds
 imagecodecs_deflate = imagecodecs.numcodecs:Deflate
 imagecodecs_delta = imagecodecs.numcodecs:Delta
 imagecodecs_float24 = imagecodecs.numcodecs:Float24
 imagecodecs_floatpred = imagecodecs.numcodecs:Floatpred
 imagecodecs_gif = imagecodecs.numcodecs:Gif
 imagecodecs_heif = imagecodecs.numcodecs:Heif
 imagecodecs_jetraw = imagecodecs.numcodecs:Jetraw
```

