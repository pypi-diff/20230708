# Comparing `tmp/datarobot_mlflow-0.1.dev1-py3-none-any.whl.zip` & `tmp/datarobot_mlflow-0.1.dev2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,12 @@
-Zip file size: 12431 bytes, number of entries: 12
+Zip file size: 12176 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     1008 b- defN 23-Jun-27 16:09 datarobot_mlflow/__init__.py
--rw-r--r--  2.0 unx     2165 b- defN 23-Jun-27 16:09 datarobot_mlflow/azure_helper.py
+-rw-r--r--  2.0 unx     2165 b- defN 23-Jul-07 22:27 datarobot_mlflow/azure_helper.py
 -rw-r--r--  2.0 unx     6635 b- defN 23-Jun-27 16:09 datarobot_mlflow/datarobot_kv_helper.py
 -rw-r--r--  2.0 unx     8030 b- defN 23-Jun-27 16:09 datarobot_mlflow/dr_mlflow_integration.py
 -rw-r--r--  2.0 unx    10401 b- defN 23-Jun-27 16:09 datarobot_mlflow/drflow_cli.py
--rwxr-xr-x  2.0 unx      430 b- defN 23-Jun-14 00:29 datarobot_mlflow-0.1.dev1.data/scripts/run.sh
--rwxr-xr-x  2.0 unx      433 b- defN 23-Jun-27 16:09 datarobot_mlflow-0.1.dev1.data/scripts/validate-auth.sh
--rw-r--r--  2.0 unx     2825 b- defN 23-Jul-03 22:27 datarobot_mlflow-0.1.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 22:27 datarobot_mlflow-0.1.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 23-Jul-03 22:27 datarobot_mlflow-0.1.dev1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-03 22:27 datarobot_mlflow-0.1.dev1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1121 b- defN 23-Jul-03 22:27 datarobot_mlflow-0.1.dev1.dist-info/RECORD
-12 files, 33221 bytes uncompressed, 10501 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx     5231 b- defN 23-Jul-07 22:27 datarobot_mlflow-0.1.dev2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 22:27 datarobot_mlflow-0.1.dev2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-07 22:27 datarobot_mlflow-0.1.dev2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-07 22:27 datarobot_mlflow-0.1.dev2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      909 b- defN 23-Jul-07 22:27 datarobot_mlflow-0.1.dev2.dist-info/RECORD
+10 files, 34552 bytes uncompressed, 10598 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -9,29 +9,23 @@
 
 Filename: datarobot_mlflow/dr_mlflow_integration.py
 Comment: 
 
 Filename: datarobot_mlflow/drflow_cli.py
 Comment: 
 
-Filename: datarobot_mlflow-0.1.dev1.data/scripts/run.sh
+Filename: datarobot_mlflow-0.1.dev2.dist-info/METADATA
 Comment: 
 
-Filename: datarobot_mlflow-0.1.dev1.data/scripts/validate-auth.sh
+Filename: datarobot_mlflow-0.1.dev2.dist-info/WHEEL
 Comment: 
 
-Filename: datarobot_mlflow-0.1.dev1.dist-info/METADATA
+Filename: datarobot_mlflow-0.1.dev2.dist-info/entry_points.txt
 Comment: 
 
-Filename: datarobot_mlflow-0.1.dev1.dist-info/WHEEL
+Filename: datarobot_mlflow-0.1.dev2.dist-info/top_level.txt
 Comment: 
 
-Filename: datarobot_mlflow-0.1.dev1.dist-info/entry_points.txt
-Comment: 
-
-Filename: datarobot_mlflow-0.1.dev1.dist-info/top_level.txt
-Comment: 
-
-Filename: datarobot_mlflow-0.1.dev1.dist-info/RECORD
+Filename: datarobot_mlflow-0.1.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `datarobot_mlflow-0.1.dev1.dist-info/RECORD` & `datarobot_mlflow-0.1.dev2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 datarobot_mlflow/__init__.py,sha256=zFbnKcv7WHdTTuzf3Y2JxbwaFLnJEmb0api-t9mhifc,1008
 datarobot_mlflow/azure_helper.py,sha256=jN6WahTx0nFoxwO2u6M_9PMF3JwlmsVFkp0pnAzBNww,2165
 datarobot_mlflow/datarobot_kv_helper.py,sha256=Q69vN00ums_DDW7IrrC3jZZeH2APx67oYlHCi2GBEjM,6635
 datarobot_mlflow/dr_mlflow_integration.py,sha256=vTxmnvrQ9E5N75q-Hy2bucCLFZL9sCrny0cpSwG6qrE,8030
 datarobot_mlflow/drflow_cli.py,sha256=SzlqEAq9kBikCHvjiTlunTURH3KkKxeY8gybrFjGuGU,10401
-datarobot_mlflow-0.1.dev1.data/scripts/run.sh,sha256=ynorz2TdC1eN5f7VXvC2wUoYy-jHIgmB55IyIvCCrUs,430
-datarobot_mlflow-0.1.dev1.data/scripts/validate-auth.sh,sha256=KmzoN2a1atd8ZQlXegGvSDAooJrzvDUMTNAUeakZMvo,433
-datarobot_mlflow-0.1.dev1.dist-info/METADATA,sha256=saZRstpRskW4SkIzkQZsI9e144HsH5U4Vm8AWHQK4Zw,2825
-datarobot_mlflow-0.1.dev1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-datarobot_mlflow-0.1.dev1.dist-info/entry_points.txt,sha256=-I3ZjDOaYtxutkE8gxdvDLSG4O32s0Qpv__-ANWTpEw,64
-datarobot_mlflow-0.1.dev1.dist-info/top_level.txt,sha256=KOC-4XhaSCZg39AIkmUyzLN_EB_fOADgS9u_N3IzB9w,17
-datarobot_mlflow-0.1.dev1.dist-info/RECORD,,
+datarobot_mlflow-0.1.dev2.dist-info/METADATA,sha256=Y5Kjwx_RAc2vTM2mXaVug7gWYH0uJOAS-a1DW687eCs,5231
+datarobot_mlflow-0.1.dev2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+datarobot_mlflow-0.1.dev2.dist-info/entry_points.txt,sha256=-I3ZjDOaYtxutkE8gxdvDLSG4O32s0Qpv__-ANWTpEw,64
+datarobot_mlflow-0.1.dev2.dist-info/top_level.txt,sha256=KOC-4XhaSCZg39AIkmUyzLN_EB_fOADgS9u_N3IzB9w,17
+datarobot_mlflow-0.1.dev2.dist-info/RECORD,,
```

