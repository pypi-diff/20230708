# Comparing `tmp/gsclinks-1.0.3-py3-none-any.whl.zip` & `tmp/gsclinks-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 5445 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       73 b- defN 23-Jul-08 10:27 gsclinks/__init__.py
--rw-r--r--  2.0 unx     4279 b- defN 23-Jul-08 10:26 gsclinks/links.py
+-rw-r--r--  2.0 unx     4267 b- defN 23-Jul-08 17:13 gsclinks/links.py
 -rw-r--r--  2.0 unx      873 b- defN 23-Jul-08 10:25 gsclinks/utils.py
--rw-r--r--  2.0 unx     1076 b- defN 23-Jul-08 13:56 gsclinks-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3824 b- defN 23-Jul-08 13:56 gsclinks-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 13:56 gsclinks-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-08 13:56 gsclinks-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      612 b- defN 23-Jul-08 13:56 gsclinks-1.0.3.dist-info/RECORD
-8 files, 10838 bytes uncompressed, 4379 bytes compressed:  59.6%
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jul-08 17:16 gsclinks-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3820 b- defN 23-Jul-08 17:16 gsclinks-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 17:16 gsclinks-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-08 17:16 gsclinks-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      612 b- defN 23-Jul-08 17:16 gsclinks-1.0.4.dist-info/RECORD
+8 files, 10822 bytes uncompressed, 4379 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: gsclinks/links.py
 Comment: 
 
 Filename: gsclinks/utils.py
 Comment: 
 
-Filename: gsclinks-1.0.3.dist-info/LICENSE
+Filename: gsclinks-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: gsclinks-1.0.3.dist-info/METADATA
+Filename: gsclinks-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: gsclinks-1.0.3.dist-info/WHEEL
+Filename: gsclinks-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: gsclinks-1.0.3.dist-info/top_level.txt
+Filename: gsclinks-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: gsclinks-1.0.3.dist-info/RECORD
+Filename: gsclinks-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gsclinks/links.py

```diff
@@ -83,23 +83,23 @@
         for site in tqdm(sites, desc='Get target pages'):
             target_pages = self.get_target_pages(site)
             data = [{'site': site, 'target_page': target_page} for target_page in target_pages]
             all_target_pages += data
             time.sleep(sleep)
         return all_target_pages
 
-    def get_all_linking_pages(self, all_target_pages, sleep=5):
+    def get_all_linking_pages(self, target_pages, sleep=5):
         '''
 
-        :param all_target_pages: a list of dict, it is the get_all_target_pages function result
+        :param target_pages: a list of dict, it is the get_all_target_pages function result
         :param sleep: time to rest between each request sending (seconds)
         :return: a list of dict
         '''
         all_linking_pages = []
-        for page in tqdm(all_target_pages, desc='Get linking pages'):
+        for page in tqdm(target_pages, desc='Get linking pages'):
             site = page['site']
             target_page = page['target_page']
             linking_pages = self.get_linking_pages(site=site, target_page=target_page)
             data = [{'site': site, 'target_page': target_page, 'linking_page': linking_page} for linking_page in linking_pages]
             all_linking_pages += data
             time.sleep(sleep)
         return all_linking_pages
```

## Comparing `gsclinks-1.0.3.dist-info/LICENSE` & `gsclinks-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gsclinks-1.0.3.dist-info/METADATA` & `gsclinks-1.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsclinks
-Version: 1.0.3
+Version: 1.0.4
 Summary: Scrape backlink data from Google Search Console
 Home-page: https://github.com/tranngocminhhieu/google-search-console-links
 Author: Tran Ngoc Minh Hieu
 Author-email: tnmhieu@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
@@ -70,15 +70,15 @@
 
 # Filter out the sites you want to continue to get data from.
 
 # Get all target pages
 all_target_pages = console.get_all_target_pages(sites=sites, sleep=5)
 
 # Get all linking pages
-all_linking_pages = console.get_all_linking_pages(all_target_pages=all_target_pages, sleep=5)
+all_linking_pages = console.get_all_linking_pages(target_pages=all_target_pages, sleep=5)
 ```
 
 Finally, you can convert the backlink data to a frame using Pandas for analysis, or export the backlink data to a CSV (Excel) file.
 
 ```python
 import pandas as pd
```

## Comparing `gsclinks-1.0.3.dist-info/RECORD` & `gsclinks-1.0.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gsclinks/__init__.py,sha256=MFcvBgfYYlaTO_zRBmNhNmjN1n2Ju6kM-jMIHp4UzIo,73
-gsclinks/links.py,sha256=TI6hdmJaV1BQrzoFtyc3J30v0TGWqvMuqk8Lon8dsrM,4279
+gsclinks/links.py,sha256=_RNHeCUVp4XKe17DiVq_L5-4jk9mS5_Fp4w76oWfBio,4267
 gsclinks/utils.py,sha256=luFShnkIqQjOfV3QrhnL8KvfbUJknMvvE8OqlaNsYG4,873
-gsclinks-1.0.3.dist-info/LICENSE,sha256=do2v2Zr9PKexWB6RWWOZVRJi73GgCDowDBwt6EZLnmg,1076
-gsclinks-1.0.3.dist-info/METADATA,sha256=obK4SJKXiIGjXTlXfJdLx6tXacJSdBiaQviFD4snwFI,3824
-gsclinks-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gsclinks-1.0.3.dist-info/top_level.txt,sha256=INqFtPlk8M46hNtCYnfRXxENy5xGqnI_gscJyovJKSM,9
-gsclinks-1.0.3.dist-info/RECORD,,
+gsclinks-1.0.4.dist-info/LICENSE,sha256=do2v2Zr9PKexWB6RWWOZVRJi73GgCDowDBwt6EZLnmg,1076
+gsclinks-1.0.4.dist-info/METADATA,sha256=tGyS1R1PWrTbbMIwTiejVwlhOm7CbYnnK8TYSKmUOhU,3820
+gsclinks-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gsclinks-1.0.4.dist-info/top_level.txt,sha256=INqFtPlk8M46hNtCYnfRXxENy5xGqnI_gscJyovJKSM,9
+gsclinks-1.0.4.dist-info/RECORD,,
```

