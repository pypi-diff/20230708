# Comparing `tmp/gsclinks-1.0.0-py3-none-any.whl.zip` & `tmp/gsclinks-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4320 bytes, number of entries: 7
+Zip file size: 4343 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       73 b- defN 23-Jul-08 10:27 gsclinks/__init__.py
 -rw-r--r--  2.0 unx     4279 b- defN 23-Jul-08 10:26 gsclinks/links.py
 -rw-r--r--  2.0 unx      873 b- defN 23-Jul-08 10:25 gsclinks/utils.py
--rw-r--r--  2.0 unx     2838 b- defN 23-Jul-08 12:25 gsclinks-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 12:25 gsclinks-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-08 12:25 gsclinks-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      523 b- defN 23-Jul-08 12:25 gsclinks-1.0.0.dist-info/RECORD
-7 files, 8687 bytes uncompressed, 3394 bytes compressed:  60.9%
+-rw-r--r--  2.0 unx     3087 b- defN 23-Jul-08 12:34 gsclinks-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 12:34 gsclinks-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-08 12:34 gsclinks-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      523 b- defN 23-Jul-08 12:34 gsclinks-1.0.1.dist-info/RECORD
+7 files, 8936 bytes uncompressed, 3417 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: gsclinks/links.py
 Comment: 
 
 Filename: gsclinks/utils.py
 Comment: 
 
-Filename: gsclinks-1.0.0.dist-info/METADATA
+Filename: gsclinks-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: gsclinks-1.0.0.dist-info/WHEEL
+Filename: gsclinks-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: gsclinks-1.0.0.dist-info/top_level.txt
+Filename: gsclinks-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gsclinks-1.0.0.dist-info/RECORD
+Filename: gsclinks-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gsclinks-1.0.0.dist-info/METADATA` & `gsclinks-1.0.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: gsclinks
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scrape backlink data from Google Search Console
 Home-page: https://github.com/tranngocminhhieu/google-search-console-links
 Author: Tran Ngoc Minh Hieu
 Author-email: tnmhieu@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 # Google Search Console Links (GSCLinks)
 Website administrators and SEOers will often monitor backlink data to know which websites are linking to their websites. From there, they can filter out bad backlinks to send to Google Disavow Links.
 
 This package will help you scrape backlink data from Google Search Console with cookies.
 
-![GSC](images/thumb.jpg)
+![GSC](https://github.com/tranngocminhhieu/google-search-console-links/blob/main/images/thumb.jpg?raw=true)
 ## Installation
 GSCLinks is available on PyPI. You can install it through pip:
 ```commandline
 pip install gsclinks
 ```
 
 ## Usage
 ### Get raw cookie
 **Method 1:** Open Chrome Developer Tool (F12), then go to Network tab, then visit Google Search Console, and then copy the Cookie's value in Request Header.
 
-![Cookie value in F12](images/cookie-value-f12.png)
+![Cookie value in F12](https://github.com/tranngocminhhieu/google-search-console-links/blob/main/images/cookie-value-f12.png?raw=true)
 
 **Method 2:** Use [Cookie-Editor](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) extension on Chrome, visit Google Search Console, then open Cookie-Editor, and then export cookie as JSON.
 
-![Cookie value in Cookie-Editor](images/cookie-editor.png)
+![Cookie value in Cookie-Editor](https://github.com/tranngocminhhieu/google-search-console-links/blob/main/images/cookie-editor.png?raw=true)
 
 Save the raw cookie in text file, such as `cookie.txt`.
 
 ### Import packages and set variables
 Import packages:
 ```python
 from gsclinks import parse_raw_cookie, SearchConsoleLinks
```

