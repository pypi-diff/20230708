# Comparing `tmp/idownload-0.1.0-py3-none-any.whl.zip` & `tmp/idownload-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 4955 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-07 18:31 idownload/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-07 18:31 idownload/__main__.py
--rw-r--r--  2.0 unx      665 b- defN 23-Jul-07 18:31 idownload/cli.py
--rw-r--r--  2.0 unx      190 b- defN 23-Jul-07 18:31 idownload/exceptions.py
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-07 18:31 idownload/sources/__init__.py
--rw-r--r--  2.0 unx     2390 b- defN 23-Jul-07 18:31 idownload/sources/pinterest.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-07 18:32 idownload-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1084 b- defN 23-Jul-07 18:32 idownload-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 18:32 idownload-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jul-07 18:32 idownload-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-07 18:32 idownload-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 23-Jul-07 18:32 idownload-0.1.0.dist-info/RECORD
-12 files, 6635 bytes uncompressed, 3319 bytes compressed:  50.0%
+Zip file size: 5092 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-07 22:09 idownload/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-07 22:09 idownload/__main__.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Jul-07 22:09 idownload/cli.py
+-rw-r--r--  2.0 unx      190 b- defN 23-Jul-07 22:09 idownload/exceptions.py
+-rw-r--r--  2.0 unx       69 b- defN 23-Jul-07 22:09 idownload/sources/__init__.py
+-rw-r--r--  2.0 unx     2907 b- defN 23-Jul-07 22:09 idownload/sources/pinterest.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1112 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/RECORD
+12 files, 7180 bytes uncompressed, 3456 bytes compressed:  51.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: idownload/sources/__init__.py
 Comment: 
 
 Filename: idownload/sources/pinterest.py
 Comment: 
 
-Filename: idownload-0.1.0.dist-info/LICENSE
+Filename: idownload-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: idownload-0.1.0.dist-info/METADATA
+Filename: idownload-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: idownload-0.1.0.dist-info/WHEEL
+Filename: idownload-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: idownload-0.1.0.dist-info/entry_points.txt
+Filename: idownload-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: idownload-0.1.0.dist-info/top_level.txt
+Filename: idownload-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: idownload-0.1.0.dist-info/RECORD
+Filename: idownload-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## idownload/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

## idownload/sources/pinterest.py

```diff
@@ -2,14 +2,15 @@
 import urllib.request
 import urllib.error
 from datetime import datetime
 from pathlib import Path
 from contextlib import contextmanager
 import feedparser
 from imeta import ImageMetadata
+from fnum import FnumMetadata
 
 from ..exceptions import ImageDownloadException
 
 
 class PinterestSource:
     COMMAND = "pinterest"
     ARGS = ("username", "board", "dirpath")
@@ -18,48 +19,61 @@
     def download(cls, username, board, dirpath, progressbar=None):
         url = f"https://www.pinterest.com/{username}/{board}.rss"
         feed = feedparser.parse(url)
         if not progressbar:
 
             @contextmanager
             def noop_progressbar(*args, **kwargs):
-                yield files
+                yield args[0]
 
             progressbar = noop_progressbar
 
         with progressbar(feed["items"], label="Downloading images") as bar:
             for item in bar:
                 source_name = item["title"]
                 source_id = re.match(
-                    "^https:\/\/www\.pinterest\.com\/pin\/(\d+)\/$", item["guid"]
+                    "^https:\\/\\/www\\.pinterest\\.com\\/pin\\/(\\d+)\\/$",
+                    item["guid"],
                 ).groups()[0]
                 metadata = {
                     "$version": "1.0",
                     "source_url": item["link"],
                     "source_id": source_id,
                     "source_name": source_name,
                     "access_date": int(datetime.now().timestamp()),
                     "tags": ["source:pinterest"],
                 }
 
-                image_url = re.search(
-                    '<img src="(.+?)\.jpg" \/>', item["description"]
+                url_start = re.search(
+                    '<img src="(.+?)\\.jpg" \\/>', item["description"]
                 ).groups()[0]
-                image_url = image_url.replace("236x", "originals")
+                url_start = url_start.replace("236x", "originals")
 
-                suffixes = [".jpg", ".png"]
-                while suffixes:
-                    suffix = suffixes.pop(0)
+                suffixes = (".jpg", ".png")
+                dirpath = Path(dirpath)
+                possible_urls = list(f"{url_start}{suffix}" for suffix in suffixes)
+
+                if any((dirpath / Path(url).name).exists() for url in possible_urls):
+                    continue
+                try:
+                    fnum_metadata = FnumMetadata.from_file(dirpath)
+                    if any(
+                        fnum_metadata.contains(str(Path(url).name))
+                        for url in possible_urls
+                    ):
+                        continue
+                except FileNotFoundError:
+                    pass
+
+                while possible_urls:
+                    image_url = possible_urls.pop(0)
                     try:
-                        request = urllib.request.Request(f"{image_url}{suffix}")
+                        request = urllib.request.Request(image_url)
                         data = urllib.request.urlopen(request).read()
-                        image_url += suffix
                         break
                     except urllib.error.HTTPError as e:
-                        if e.getcode() != 403 or not suffixes:
+                        if e.getcode() != 403 or not possible_urls:
                             raise ImageDownloadException(image_url, e)
 
-                dirpath = Path(dirpath)
-                filepath = Path(image_url)
-                (dirpath / filepath.name).write_bytes(data)
-                # use to_image instead
-                ImageMetadata(metadata).to_file(str(dirpath / f"{filepath.stem}.json"))
+                filepath = dirpath / Path(image_url).name
+                filepath.write_bytes(data)
+                ImageMetadata(metadata).to_image(str(filepath))
```

## Comparing `idownload-0.1.0.dist-info/LICENSE` & `idownload-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `idownload-0.1.0.dist-info/METADATA` & `idownload-0.2.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idownload
-Version: 0.1.0
+Version: 0.2.0
 Summary: Downloads images and stores metadata about them in a JSON file
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/idownload
 Keywords: idownload,cli,utility,image,download,backup,archive,pinterest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,9 +19,10 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8.0
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: feedparser (~=6.0)
-Requires-Dist: imeta (~=1.0)
+Requires-Dist: imeta (~=1.1)
+Requires-Dist: fnum (~=1.2)
```

