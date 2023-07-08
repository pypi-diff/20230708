# Comparing `tmp/impose_cli-0.1.41rc2-py3-none-any.whl.zip` & `tmp/impose_cli-0.1.41rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8858 bytes, number of entries: 14
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-08 14:42 impose_cli/__init__.py
+Zip file size: 8766 bytes, number of entries: 14
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 14:49 impose_cli/__init__.py
 -rw-r--r--  2.0 unx    12087 b- defN 23-Jul-08 14:42 impose_cli/_utils.py
 -rw-r--r--  2.0 unx      112 b- defN 23-Jul-08 14:42 impose_cli/decorators.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 14:42 impose_cli/errors.py
 -rw-r--r--  2.0 unx     1237 b- defN 23-Jul-08 14:42 impose_cli/impose_cli.py
 -rw-r--r--  2.0 unx     5029 b- defN 23-Jul-08 14:42 impose_cli/impose_cli_2.py
 -rw-r--r--  2.0 unx      197 b- defN 23-Jul-08 14:42 impose_cli/types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 04:10 tests/__init__.py
 -rw-r--r--  2.0 unx      446 b- defN 23-Jul-08 14:42 tests/test.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Jul-08 14:47 impose_cli-0.1.41rc2.dist-info/LICENSE
--rw-r--r--  2.0 unx      358 b- defN 23-Jul-08 14:47 impose_cli-0.1.41rc2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 14:47 impose_cli-0.1.41rc2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 14:47 impose_cli-0.1.41rc2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1108 b- defN 23-Jul-08 14:47 impose_cli-0.1.41rc2.dist-info/RECORD
-14 files, 21823 bytes uncompressed, 7014 bytes compressed:  67.9%
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jul-08 14:49 impose_cli-0.1.41rc3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      358 b- defN 23-Jul-08 14:49 impose_cli-0.1.41rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 14:49 impose_cli-0.1.41rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 14:49 impose_cli-0.1.41rc3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1107 b- defN 23-Jul-08 14:49 impose_cli-0.1.41rc3.dist-info/RECORD
+14 files, 21753 bytes uncompressed, 6922 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test.py
 Comment: 
 
-Filename: impose_cli-0.1.41rc2.dist-info/LICENSE
+Filename: impose_cli-0.1.41rc3.dist-info/LICENSE
 Comment: 
 
-Filename: impose_cli-0.1.41rc2.dist-info/METADATA
+Filename: impose_cli-0.1.41rc3.dist-info/METADATA
 Comment: 
 
-Filename: impose_cli-0.1.41rc2.dist-info/WHEEL
+Filename: impose_cli-0.1.41rc3.dist-info/WHEEL
 Comment: 
 
-Filename: impose_cli-0.1.41rc2.dist-info/top_level.txt
+Filename: impose_cli-0.1.41rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: impose_cli-0.1.41rc2.dist-info/RECORD
+Filename: impose_cli-0.1.41rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## impose_cli/__init__.py

```diff
@@ -1,5 +0,0 @@
-00000000: 6672 6f6d 2069 6d70 6f73 655f 636c 6920  from impose_cli 
-00000010: 696d 706f 7274 2064 6563 6f72 6174 6f72  import decorator
-00000020: 732c 2065 7272 6f72 732c 2069 6d70 6f73  s, errors, impos
-00000030: 655f 636c 692c 2074 7970 6573 2c20 5f75  e_cli, types, _u
-00000040: 7469 6c73 0a                             tils.
```

## Comparing `impose_cli-0.1.41rc2.dist-info/LICENSE` & `impose_cli-0.1.41rc3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `impose_cli-0.1.41rc2.dist-info/RECORD` & `impose_cli-0.1.41rc3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-impose_cli/__init__.py,sha256=X-1zE-muDyz3kD8q5rQ3pDI7Zxv6GPCUrIO2ajalYSE,69
+impose_cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 impose_cli/_utils.py,sha256=eZRxMO7T9LYrr5kr8WTZ1N50Cegc2Rxl5VtT7Oo5CLc,12087
 impose_cli/decorators.py,sha256=dtCX2DgpHDxLlFsKst7Prf3Ys-y5EVMo48mJoRGYmxo,112
 impose_cli/errors.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 impose_cli/impose_cli.py,sha256=CbJu9so1U6Cuwe2b75_5uqemxNur9-rmNF4Vbi3aAd4,1237
 impose_cli/impose_cli_2.py,sha256=YaQv41Ee5NfxV81rMmELEcx8eFmVNMP69MKR3cAiwj0,5029
 impose_cli/types.py,sha256=80g42_q9bbai8byU-TIXnoLKziTJD0nfkek-WFRwkYo,197
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test.py,sha256=rFszJ_8zyb7YX6NbVaPDMzrKgof7olFgbFIO-FCS4lk,446
-impose_cli-0.1.41rc2.dist-info/LICENSE,sha256=zbz0DcNhgXN5XVIbf__i0DoJPXOL9ybrCwGb2x4Z-tY,1071
-impose_cli-0.1.41rc2.dist-info/METADATA,sha256=sFAmHjMcC9zD0mtBvMzPF2X9CWVkgoKvG9Xf5PNPz-U,358
-impose_cli-0.1.41rc2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-impose_cli-0.1.41rc2.dist-info/top_level.txt,sha256=mF0ZPzXJ1dKbHYbVkC04Bj0o60Pwq0WeyEDbIeIN_EA,17
-impose_cli-0.1.41rc2.dist-info/RECORD,,
+impose_cli-0.1.41rc3.dist-info/LICENSE,sha256=zbz0DcNhgXN5XVIbf__i0DoJPXOL9ybrCwGb2x4Z-tY,1071
+impose_cli-0.1.41rc3.dist-info/METADATA,sha256=j60zc2ksxx-wnnabn-MtLrQSX0iyCewNu_gfZcYJLQE,358
+impose_cli-0.1.41rc3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+impose_cli-0.1.41rc3.dist-info/top_level.txt,sha256=mF0ZPzXJ1dKbHYbVkC04Bj0o60Pwq0WeyEDbIeIN_EA,17
+impose_cli-0.1.41rc3.dist-info/RECORD,,
```

