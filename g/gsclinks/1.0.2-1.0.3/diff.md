# Comparing `tmp/gsclinks-1.0.2-py3-none-any.whl.zip` & `tmp/gsclinks-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5443 bytes, number of entries: 8
+Zip file size: 5445 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       73 b- defN 23-Jul-08 10:27 gsclinks/__init__.py
 -rw-r--r--  2.0 unx     4279 b- defN 23-Jul-08 10:26 gsclinks/links.py
 -rw-r--r--  2.0 unx      873 b- defN 23-Jul-08 10:25 gsclinks/utils.py
--rw-r--r--  2.0 unx     1076 b- defN 23-Jul-08 13:53 gsclinks-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3750 b- defN 23-Jul-08 13:53 gsclinks-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 13:53 gsclinks-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-08 13:53 gsclinks-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      612 b- defN 23-Jul-08 13:53 gsclinks-1.0.2.dist-info/RECORD
-8 files, 10764 bytes uncompressed, 4377 bytes compressed:  59.3%
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jul-08 13:56 gsclinks-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3824 b- defN 23-Jul-08 13:56 gsclinks-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 13:56 gsclinks-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-08 13:56 gsclinks-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      612 b- defN 23-Jul-08 13:56 gsclinks-1.0.3.dist-info/RECORD
+8 files, 10838 bytes uncompressed, 4379 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: gsclinks/links.py
 Comment: 
 
 Filename: gsclinks/utils.py
 Comment: 
 
-Filename: gsclinks-1.0.2.dist-info/LICENSE
+Filename: gsclinks-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: gsclinks-1.0.2.dist-info/METADATA
+Filename: gsclinks-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: gsclinks-1.0.2.dist-info/WHEEL
+Filename: gsclinks-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: gsclinks-1.0.2.dist-info/top_level.txt
+Filename: gsclinks-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: gsclinks-1.0.2.dist-info/RECORD
+Filename: gsclinks-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gsclinks-1.0.2.dist-info/LICENSE` & `gsclinks-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gsclinks-1.0.2.dist-info/METADATA` & `gsclinks-1.0.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsclinks
-Version: 1.0.2
+Version: 1.0.3
 Summary: Scrape backlink data from Google Search Console
 Home-page: https://github.com/tranngocminhhieu/google-search-console-links
 Author: Tran Ngoc Minh Hieu
 Author-email: tnmhieu@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
@@ -15,15 +15,15 @@
 [![PyPI](https://img.shields.io/pypi/v/gsclinks)](https://pypi.org/project/gsclinks/) [![GitHub](https://img.shields.io/github/license/tranngocminhhieu/google-search-console-links)](https://github.com/tranngocminhhieu/google-search-console-links/blob/main/LICENSE)
 
 
 Website administrators and SEOers will often monitor backlink data to know which websites are linking to their websites. From there, they can filter out bad backlinks to send to Google Disavow Links. This will help their website not be affected by bad backlinks and keep a good position on Google Search.
 
 This package will help you scrape backlink data from Google Search Console with cookies.
 
-![GSC](images/thumb.jpg?raw=true)
+![GSC](https://github.com/tranngocminhhieu/google-search-console-links/blob/main/images/thumb.jpg?raw=true)
 
 ## Installation
 GSCLinks is available on PyPI. You can install it through pip:
 ```commandline
 pip install gsclinks
 ```
```

## Comparing `gsclinks-1.0.2.dist-info/RECORD` & `gsclinks-1.0.3.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gsclinks/__init__.py,sha256=MFcvBgfYYlaTO_zRBmNhNmjN1n2Ju6kM-jMIHp4UzIo,73
 gsclinks/links.py,sha256=TI6hdmJaV1BQrzoFtyc3J30v0TGWqvMuqk8Lon8dsrM,4279
 gsclinks/utils.py,sha256=luFShnkIqQjOfV3QrhnL8KvfbUJknMvvE8OqlaNsYG4,873
-gsclinks-1.0.2.dist-info/LICENSE,sha256=do2v2Zr9PKexWB6RWWOZVRJi73GgCDowDBwt6EZLnmg,1076
-gsclinks-1.0.2.dist-info/METADATA,sha256=Hd4C3omXsvVZxpmFAgILEA5seCoCvuWj1gmUnIMW1vU,3750
-gsclinks-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gsclinks-1.0.2.dist-info/top_level.txt,sha256=INqFtPlk8M46hNtCYnfRXxENy5xGqnI_gscJyovJKSM,9
-gsclinks-1.0.2.dist-info/RECORD,,
+gsclinks-1.0.3.dist-info/LICENSE,sha256=do2v2Zr9PKexWB6RWWOZVRJi73GgCDowDBwt6EZLnmg,1076
+gsclinks-1.0.3.dist-info/METADATA,sha256=obK4SJKXiIGjXTlXfJdLx6tXacJSdBiaQviFD4snwFI,3824
+gsclinks-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gsclinks-1.0.3.dist-info/top_level.txt,sha256=INqFtPlk8M46hNtCYnfRXxENy5xGqnI_gscJyovJKSM,9
+gsclinks-1.0.3.dist-info/RECORD,,
```

