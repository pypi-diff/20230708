# Comparing `tmp/impose_cli-0.1.41rc4-py3-none-any.whl.zip` & `tmp/impose_cli-0.1.41rc5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8820 bytes, number of entries: 14
+Zip file size: 8835 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 14:49 impose_cli/__init__.py
--rw-r--r--  2.0 unx    12270 b- defN 23-Jul-08 17:10 impose_cli/_utils.py
+-rw-r--r--  2.0 unx    12303 b- defN 23-Jul-08 17:18 impose_cli/_utils.py
 -rw-r--r--  2.0 unx      149 b- defN 23-Jul-08 17:10 impose_cli/decorators.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 14:42 impose_cli/errors.py
 -rw-r--r--  2.0 unx     1237 b- defN 23-Jul-08 14:42 impose_cli/impose_cli.py
 -rw-r--r--  2.0 unx     5029 b- defN 23-Jul-08 14:42 impose_cli/impose_cli_2.py
 -rw-r--r--  2.0 unx      197 b- defN 23-Jul-08 14:42 impose_cli/types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 04:10 tests/__init__.py
 -rw-r--r--  2.0 unx      446 b- defN 23-Jul-08 14:42 tests/test.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Jul-08 17:11 impose_cli-0.1.41rc4.dist-info/LICENSE
--rw-r--r--  2.0 unx      358 b- defN 23-Jul-08 17:11 impose_cli-0.1.41rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 17:11 impose_cli-0.1.41rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 17:11 impose_cli-0.1.41rc4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1107 b- defN 23-Jul-08 17:11 impose_cli-0.1.41rc4.dist-info/RECORD
-14 files, 21973 bytes uncompressed, 6976 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jul-08 17:18 impose_cli-0.1.41rc5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      358 b- defN 23-Jul-08 17:18 impose_cli-0.1.41rc5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 17:18 impose_cli-0.1.41rc5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 17:18 impose_cli-0.1.41rc5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1107 b- defN 23-Jul-08 17:18 impose_cli-0.1.41rc5.dist-info/RECORD
+14 files, 22006 bytes uncompressed, 6991 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test.py
 Comment: 
 
-Filename: impose_cli-0.1.41rc4.dist-info/LICENSE
+Filename: impose_cli-0.1.41rc5.dist-info/LICENSE
 Comment: 
 
-Filename: impose_cli-0.1.41rc4.dist-info/METADATA
+Filename: impose_cli-0.1.41rc5.dist-info/METADATA
 Comment: 
 
-Filename: impose_cli-0.1.41rc4.dist-info/WHEEL
+Filename: impose_cli-0.1.41rc5.dist-info/WHEEL
 Comment: 
 
-Filename: impose_cli-0.1.41rc4.dist-info/top_level.txt
+Filename: impose_cli-0.1.41rc5.dist-info/top_level.txt
 Comment: 
 
-Filename: impose_cli-0.1.41rc4.dist-info/RECORD
+Filename: impose_cli-0.1.41rc5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## impose_cli/_utils.py

```diff
@@ -266,15 +266,15 @@
         @router.get(("/{}".format(function.name) if not function.name.startswith("/") else function.name))
         def dynamic_route():
             return function.reference
 
         return router
 
     def handle_child(child, parent_group):
-        child_group = fastapi.APIRouter(prefix=child.name)
+        child_group = fastapi.APIRouter(prefix="/{}".format(child.name).replace("//", "/"))
         parent_group.add_command(child_group)
         child.external_object = child_group
         for function in child.functions:
             pass
         if child is not None and child.children is not None and len(child.children) > 0:
             child.alter_children(handle_child)
```

## Comparing `impose_cli-0.1.41rc4.dist-info/LICENSE` & `impose_cli-0.1.41rc5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `impose_cli-0.1.41rc4.dist-info/RECORD` & `impose_cli-0.1.41rc5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 impose_cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-impose_cli/_utils.py,sha256=YOBzfUAy0Hs_r6iQXtukGpptkEfpsz0gtBNwgCQT4uc,12270
+impose_cli/_utils.py,sha256=Xhd7y6bbgovydyJvNL6UMQCIQ3SIrtOOyq4gABVBtd0,12303
 impose_cli/decorators.py,sha256=ArmkwmkTPhGYuCJ52wNnqgcmfAl1a0xryoU4iDwTW48,149
 impose_cli/errors.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 impose_cli/impose_cli.py,sha256=CbJu9so1U6Cuwe2b75_5uqemxNur9-rmNF4Vbi3aAd4,1237
 impose_cli/impose_cli_2.py,sha256=YaQv41Ee5NfxV81rMmELEcx8eFmVNMP69MKR3cAiwj0,5029
 impose_cli/types.py,sha256=80g42_q9bbai8byU-TIXnoLKziTJD0nfkek-WFRwkYo,197
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test.py,sha256=rFszJ_8zyb7YX6NbVaPDMzrKgof7olFgbFIO-FCS4lk,446
-impose_cli-0.1.41rc4.dist-info/LICENSE,sha256=zbz0DcNhgXN5XVIbf__i0DoJPXOL9ybrCwGb2x4Z-tY,1071
-impose_cli-0.1.41rc4.dist-info/METADATA,sha256=XYZnJbTU58fe0foGEWFOArsUtwEbE_4AgwOP8GdqxCk,358
-impose_cli-0.1.41rc4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-impose_cli-0.1.41rc4.dist-info/top_level.txt,sha256=mF0ZPzXJ1dKbHYbVkC04Bj0o60Pwq0WeyEDbIeIN_EA,17
-impose_cli-0.1.41rc4.dist-info/RECORD,,
+impose_cli-0.1.41rc5.dist-info/LICENSE,sha256=zbz0DcNhgXN5XVIbf__i0DoJPXOL9ybrCwGb2x4Z-tY,1071
+impose_cli-0.1.41rc5.dist-info/METADATA,sha256=NwsKCNlro-Voxxrwd0X9ixMleBynUV3G4mrF7r2cZQU,358
+impose_cli-0.1.41rc5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+impose_cli-0.1.41rc5.dist-info/top_level.txt,sha256=mF0ZPzXJ1dKbHYbVkC04Bj0o60Pwq0WeyEDbIeIN_EA,17
+impose_cli-0.1.41rc5.dist-info/RECORD,,
```

