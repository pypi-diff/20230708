# Comparing `tmp/gsclinks-1.0.1-py3-none-any.whl.zip` & `tmp/gsclinks-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 4343 bytes, number of entries: 7
+Zip file size: 5443 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       73 b- defN 23-Jul-08 10:27 gsclinks/__init__.py
 -rw-r--r--  2.0 unx     4279 b- defN 23-Jul-08 10:26 gsclinks/links.py
 -rw-r--r--  2.0 unx      873 b- defN 23-Jul-08 10:25 gsclinks/utils.py
--rw-r--r--  2.0 unx     3087 b- defN 23-Jul-08 12:34 gsclinks-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 12:34 gsclinks-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-08 12:34 gsclinks-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      523 b- defN 23-Jul-08 12:34 gsclinks-1.0.1.dist-info/RECORD
-7 files, 8936 bytes uncompressed, 3417 bytes compressed:  61.8%
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jul-08 13:53 gsclinks-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3750 b- defN 23-Jul-08 13:53 gsclinks-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 13:53 gsclinks-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-08 13:53 gsclinks-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      612 b- defN 23-Jul-08 13:53 gsclinks-1.0.2.dist-info/RECORD
+8 files, 10764 bytes uncompressed, 4377 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -3,20 +3,23 @@
 
 Filename: gsclinks/links.py
 Comment: 
 
 Filename: gsclinks/utils.py
 Comment: 
 
-Filename: gsclinks-1.0.1.dist-info/METADATA
+Filename: gsclinks-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: gsclinks-1.0.1.dist-info/WHEEL
+Filename: gsclinks-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: gsclinks-1.0.1.dist-info/top_level.txt
+Filename: gsclinks-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: gsclinks-1.0.1.dist-info/RECORD
+Filename: gsclinks-1.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: gsclinks-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gsclinks-1.0.1.dist-info/METADATA` & `gsclinks-1.0.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: gsclinks
-Version: 1.0.1
+Version: 1.0.2
 Summary: Scrape backlink data from Google Search Console
 Home-page: https://github.com/tranngocminhhieu/google-search-console-links
 Author: Tran Ngoc Minh Hieu
 Author-email: tnmhieu@gmail.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 # Google Search Console Links (GSCLinks)
-Website administrators and SEOers will often monitor backlink data to know which websites are linking to their websites. From there, they can filter out bad backlinks to send to Google Disavow Links.
+[![PyPI](https://img.shields.io/pypi/v/gsclinks)](https://pypi.org/project/gsclinks/) [![GitHub](https://img.shields.io/github/license/tranngocminhhieu/google-search-console-links)](https://github.com/tranngocminhhieu/google-search-console-links/blob/main/LICENSE)
+
+
+Website administrators and SEOers will often monitor backlink data to know which websites are linking to their websites. From there, they can filter out bad backlinks to send to Google Disavow Links. This will help their website not be affected by bad backlinks and keep a good position on Google Search.
 
 This package will help you scrape backlink data from Google Search Console with cookies.
 
-![GSC](https://github.com/tranngocminhhieu/google-search-console-links/blob/main/images/thumb.jpg?raw=true)
+![GSC](images/thumb.jpg?raw=true)
+
 ## Installation
 GSCLinks is available on PyPI. You can install it through pip:
 ```commandline
 pip install gsclinks
 ```
 
 ## Usage
@@ -50,23 +55,35 @@
 user_number = None # or maybe 0, 1, 2, ...
 console = SearchConsoleLinks(cookies=cookies, resource_id=resource_id, user_number=user_number)
 ```
 
 ### Get backlink data
 If you want the entire backlink data in a simple way then use this method.
 ```python
-backlinks = console.get_all_links(sleep=10)
+all_linking_pages = console.get_all_links(sleep=10)
 # sleep: time to rest between each request sending (seconds).
 ```
 
 You can get backlink data step by step to be able to intervene in the process. For example, you may want to remove some sites that you no longer need to get data.
 ```python
 # Get sites
 sites = console.get_sites()
 
+# Filter out the sites you want to continue to get data from.
+
 # Get all target pages
 all_target_pages = console.get_all_target_pages(sites=sites, sleep=5)
 
 # Get all linking pages
 all_linking_pages = console.get_all_linking_pages(all_target_pages=all_target_pages, sleep=5)
 ```
 
+Finally, you can convert the backlink data to a frame using Pandas for analysis, or export the backlink data to a CSV (Excel) file.
+
+```python
+import pandas as pd
+
+df = pd.DataFrame(all_linking_pages)
+df.to_csv('backlinks.csv', index=False)
+```
+
+*Thank you for reading!*
```

