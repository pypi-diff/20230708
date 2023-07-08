# Comparing `tmp/swanapi-0.1.2-py3-none-any.whl.zip` & `tmp/swanapi-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7456 bytes, number of entries: 12
--rw-r--r--  2.0 unx      114 b- defN 23-Jul-08 10:57 swanapi/__init__.py
+Zip file size: 7406 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       62 b- defN 23-Jul-08 12:12 swanapi/__init__.py
 -rw-r--r--  2.0 unx     6378 b- defN 23-Jul-08 08:54 swanapi/base_inference.py
 -rw-r--r--  2.0 unx      833 b- defN 23-Jul-08 11:33 swanapi/make_build.py
 -rw-r--r--  2.0 unx     1897 b- defN 23-Jul-08 09:00 swanapi/server.py
 -rw-r--r--  2.0 unx      572 b- defN 23-Jul-08 07:57 swanapi/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
--rw-r--r--  2.0 unx     4878 b- defN 23-Jul-08 11:13 swanapi/docker_builder/runner.py
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-08 11:57 swanapi-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 11:57 swanapi-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-08 11:57 swanapi-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-08 11:57 swanapi-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      948 b- defN 23-Jul-08 11:57 swanapi-0.1.2.dist-info/RECORD
-12 files, 16130 bytes uncompressed, 5858 bytes compressed:  63.7%
+-rw-r--r--  2.0 unx     4869 b- defN 23-Jul-08 12:12 swanapi/docker_builder/runner.py
+-rw-r--r--  2.0 unx      347 b- defN 23-Jul-08 12:13 swanapi-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 12:13 swanapi-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-08 12:13 swanapi-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-08 12:13 swanapi-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      947 b- defN 23-Jul-08 12:13 swanapi-0.1.3.dist-info/RECORD
+12 files, 16058 bytes uncompressed, 5808 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: swanapi/docker_builder/__init__.py
 Comment: 
 
 Filename: swanapi/docker_builder/runner.py
 Comment: 
 
-Filename: swanapi-0.1.2.dist-info/METADATA
+Filename: swanapi-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.1.2.dist-info/WHEEL
+Filename: swanapi-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.1.2.dist-info/entry_points.txt
+Filename: swanapi-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.1.2.dist-info/top_level.txt
+Filename: swanapi-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.1.2.dist-info/RECORD
+Filename: swanapi-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swanapi/__init__.py

```diff
@@ -1,4 +1,3 @@
 from .server import SwanInference
-from .docker_builder.runner import Runner
 
-__all__ = ["SwanInference", "Runner"]
+__all__ = ["SwanInference"]
```

## swanapi/docker_builder/runner.py

```diff
@@ -70,15 +70,15 @@
             data = yaml.load(file, Loader=yaml.FullLoader)
         return data
 
 
 class DockerfileBuild:
     def __init__(self, configs: SwanConfig):
         self.config = configs
-        self.python_prepackage = ["flask", "swanapi"]
+        self.python_prepackage = ["swanapi"]
 
     def get_dockerfile(self):
         # 根据build中的信息，构建一个Dockerfile
         dockerfile_text = """"""
         dockerfile_text += self.get_FORM()
         prefile_apt, prefile_python = self.get_prefile()
         dockerfile_text += prefile_apt
```

## Comparing `swanapi-0.1.2.dist-info/RECORD` & `swanapi-0.1.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-swanapi/__init__.py,sha256=__DTCQHLsUk0EWb3dRlDzzS51JbKQw2b-WsLOaMP3TQ,114
+swanapi/__init__.py,sha256=T69A5YM84uwabbMeLbIZuDpk6R7ZcA51IrNFJOfRyq8,62
 swanapi/base_inference.py,sha256=Wp2jIC2SeAgS5TDjj0u1QG8S_ZKlOYi81LryF1PdltU,6378
 swanapi/make_build.py,sha256=eetDgQdCyQzsCVCniHPTee29bo0j4rfENxsVQMzeSys,833
 swanapi/server.py,sha256=ewk3Wt3GMOXJLNzAi_6C86LoDgiqWlZP9TPr8T5IdPA,1897
 swanapi/utils.py,sha256=YlXVC6k_5yeZ1EuUR-LpF5DOEpcLG00Uks4LEYPLwRo,572
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-swanapi/docker_builder/runner.py,sha256=WJaKffeXAJujX0s9fOe5D0Bq1PAzzFEy6961EHancAA,4878
-swanapi-0.1.2.dist-info/METADATA,sha256=vMm5tPv5DOqVGrjV70Hv2cknuTcZFW1QPyREnISv8FI,357
-swanapi-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.1.2.dist-info/entry_points.txt,sha256=fgN0mUcvpscd5X6ZbWlK1FYJPU2l89EDR5qkKLNg1b4,53
-swanapi-0.1.2.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.1.2.dist-info/RECORD,,
+swanapi/docker_builder/runner.py,sha256=uknif9LNfCgAnVgb_kNpTvk_GMu4wdkkYV6jK0vG1Lc,4869
+swanapi-0.1.3.dist-info/METADATA,sha256=VUMI8xncyU-usn-rfwa0d097nXknnV_K02-ZLljsk-E,347
+swanapi-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.1.3.dist-info/entry_points.txt,sha256=fgN0mUcvpscd5X6ZbWlK1FYJPU2l89EDR5qkKLNg1b4,53
+swanapi-0.1.3.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.1.3.dist-info/RECORD,,
```

