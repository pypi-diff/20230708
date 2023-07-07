# Comparing `tmp/wiki_as_base-0.5.7.tar.gz` & `tmp/wiki_as_base-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiki_as_base-0.5.7.tar", last modified: Thu Jun 29 03:54:28 2023, max compression
+gzip compressed data, was "wiki_as_base-0.5.8.tar", last modified: Fri Jul  7 22:21:44 2023, max compression
```

## Comparing `wiki_as_base-0.5.7.tar` & `wiki_as_base-0.5.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-29 03:54:28.242873 wiki_as_base-0.5.7/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1211 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/LICENSE
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10719 2023-06-29 03:54:28.242873 wiki_as_base-0.5.7/PKG-INFO
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10114 2023-06-28 23:37:08.000000 wiki_as_base-0.5.7/README.md
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      104 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/pyproject.toml
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      872 2023-06-29 03:54:28.242873 wiki_as_base-0.5.7/setup.cfg
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-29 03:54:28.238873 wiki_as_base-0.5.7/src/
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-29 03:54:28.242873 wiki_as_base-0.5.7/src/wiki_as_base/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      158 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/src/wiki_as_base/__init__.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     5203 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/src/wiki_as_base/cli.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1583 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/src/wiki_as_base/constants.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    13883 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/src/wiki_as_base/parser.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    49224 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/src/wiki_as_base/wiki_as_base.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-29 03:54:28.242873 wiki_as_base-0.5.7/src/wiki_as_base.egg-info/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10719 2023-06-29 03:54:28.000000 wiki_as_base-0.5.7/src/wiki_as_base.egg-info/PKG-INFO
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      531 2023-06-29 03:54:28.000000 wiki_as_base-0.5.7/src/wiki_as_base.egg-info/SOURCES.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        1 2023-06-29 03:54:28.000000 wiki_as_base-0.5.7/src/wiki_as_base.egg-info/dependency_links.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       76 2023-06-29 03:54:28.000000 wiki_as_base-0.5.7/src/wiki_as_base.egg-info/entry_points.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       39 2023-06-29 03:54:28.000000 wiki_as_base-0.5.7/src/wiki_as_base.egg-info/requires.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       13 2023-06-29 03:54:28.000000 wiki_as_base-0.5.7/src/wiki_as_base.egg-info/top_level.txt
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-29 03:54:28.242873 wiki_as_base-0.5.7/tests/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      774 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/tests/test_internals.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1258 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/tests/test_tables.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     3394 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/tests/test_wikitext.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2211 2023-04-25 05:51:41.000000 wiki_as_base-0.5.7/tests/test_wikitext_with_network.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1211 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/LICENSE
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10704 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/PKG-INFO
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10099 2023-07-07 22:20:12.000000 wiki_as_base-0.5.8/README.md
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      104 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/pyproject.toml
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      872 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/setup.cfg
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/src/
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/src/wiki_as_base/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      158 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/src/wiki_as_base/__init__.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     6367 2023-07-05 07:29:06.000000 wiki_as_base-0.5.8/src/wiki_as_base/cli.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1583 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/src/wiki_as_base/constants.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    15993 2023-07-07 06:01:14.000000 wiki_as_base-0.5.8/src/wiki_as_base/parser.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    53110 2023-07-07 06:39:57.000000 wiki_as_base-0.5.8/src/wiki_as_base/wiki_as_base.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10704 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/PKG-INFO
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      531 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/SOURCES.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        1 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/dependency_links.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       76 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/entry_points.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       39 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/requires.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       13 2023-07-07 22:21:44.000000 wiki_as_base-0.5.8/src/wiki_as_base.egg-info/top_level.txt
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-07-07 22:21:44.877906 wiki_as_base-0.5.8/tests/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      774 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/tests/test_internals.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1258 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/tests/test_tables.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     3394 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/tests/test_wikitext.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2211 2023-04-25 05:51:41.000000 wiki_as_base-0.5.8/tests/test_wikitext_with_network.py
```

### Comparing `wiki_as_base-0.5.7/LICENSE` & `wiki_as_base-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.7/PKG-INFO` & `wiki_as_base-0.5.8/src/wiki_as_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wiki_as_base
-Version: 0.5.7
+Name: wiki-as-base
+Version: 0.5.8
 Summary: Use MediaWiki Wiki page content as read-only database
 Home-page: https://github.com/fititnt/wiki_as_base-py
 Author: Emerson Rocha
 Author-email: rocha@ieee.org
 Project-URL: Bug Tracker, https://github.com/fititnt/wiki_as_base-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -45,20 +45,16 @@
 ---
 
 ## Installing
 
 ```bash
 pip install wiki_as_base --upgrade
 
-## Alternative: 
-# pip install wiki-as-base==0.5.6
-```
-
-```nasj
-
+## Alternative:
+# pip install wiki_as_base==0.5.8
 ```
 
 ### Environment variables
 Customize for your needs. They're shared between command line and the library.
 
 ```bash
 export WIKI_API='https://wiki.openstreetmap.org/w/api.php'
@@ -215,15 +211,15 @@
 > **NOTE**: for production usage (if you can't review releases or are not locked into Docker images)
 > consider enforce a very specific release
 
 
 **Production usage**
 ```txt
 # requirements.txt
-wiki_as_base==0.5.5
+wiki_as_base==0.5.8
 ```
 
 **Other cases (or use in your local machine)**
 
 ```bash
 # Run this via cli for force redownload lastest. Do not use --pre (pre-releases)
 pip install wiki_as_base --upgrade
```

### Comparing `wiki_as_base-0.5.7/README.md` & `wiki_as_base-0.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,16 @@
 ---
 
 ## Installing
 
 ```bash
 pip install wiki_as_base --upgrade
 
-## Alternative: 
-# pip install wiki-as-base==0.5.6
-```
-
-```nasj
-
+## Alternative:
+# pip install wiki_as_base==0.5.8
 ```
 
 ### Environment variables
 Customize for your needs. They're shared between command line and the library.
 
 ```bash
 export WIKI_API='https://wiki.openstreetmap.org/w/api.php'
@@ -198,15 +194,15 @@
 > **NOTE**: for production usage (if you can't review releases or are not locked into Docker images)
 > consider enforce a very specific release
 
 
 **Production usage**
 ```txt
 # requirements.txt
-wiki_as_base==0.5.5
+wiki_as_base==0.5.8
 ```
 
 **Other cases (or use in your local machine)**
 
 ```bash
 # Run this via cli for force redownload lastest. Do not use --pre (pre-releases)
 pip install wiki_as_base --upgrade
```

### Comparing `wiki_as_base-0.5.7/setup.cfg` & `wiki_as_base-0.5.8/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wiki_as_base
-version = 0.5.7
+version = 0.5.8
 author = Emerson Rocha
 author_email = rocha@ieee.org
 description = Use MediaWiki Wiki page content as read-only database
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fititnt/wiki_as_base-py
 project_urls =
```

### Comparing `wiki_as_base-0.5.7/src/wiki_as_base/cli.py` & `wiki_as_base-0.5.8/src/wiki_as_base/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 # Examples
 #   wiki_as_base --page-title 'User:EmericusPetro/sandbox/Wiki-as-base' | jq .data[1].data_raw
 #   wiki_as_base --input-stdin < tests/data/multiple.wiki.txt | jq .data[1].data_raw
 #   cat tests/data/multiple.wiki.txt | wiki_as_base --input-stdin | jq .data[1].data_raw
 
 
 def main():
-
     parser = argparse.ArgumentParser(
         prog="wiki_as_base",
         description="Use MediaWiki Wiki page content as read-only database",
     )
 
     # parser.add_argument(
     #     'integers', metavar='N', type=int, nargs='+',
@@ -49,31 +48,37 @@
     parser.add_argument("--pageids", help="Pageids of input, Use | as separator")
 
     parser.add_argument("--revids", help="Revision IDs of input, Use | as separator")
 
     parser.add_argument(
         "--input-autodetect",
         # action="store_true",
-        help="Page titles or pageids (not both). "
+        help="Page titles, pageids (not both). "
         "Syntax sugar for --titles or --pageids. "
-        "Use | as separator",
+        "Use | as separator. (experimental) by category content fetch",
     )
 
     parser.add_argument(
         "--input-stdin",
         action="store_true",
-        help="Use STDIN (data piped from other tools)" "instead of remote API",
+        help="Use STDIN (data piped from other tools) instead of remote API",
     )
 
     parser.add_argument(
         "--output-raw",
         action="store_true",
         help="Output RAW, unedited Wiki markup (or API response if remote call)",
     )
 
+    parser.add_argument(
+        "--output-streaming",
+        action="store_true",
+        help="Output JSON Text Sequences (RFC 7464 application/json-seq)",
+    )
+
     # parser.add_argument(
     #     "--output-dir",
     #     help="Output inferred files to a directory. "
     #     "With --verbose will save input text and JSON-LD metadata",
     # )
 
     parser.add_argument(
@@ -86,14 +91,28 @@
     parser.add_argument(
         "--output-zip-file",
         # action="store_true",
         help="Output inferred files to a zip (file)"
         "With --verbose will save input text and JSON-LD metadata",
     )
 
+    parser.add_argument(
+        "--filter-item-type",
+        # action="store_true",
+        help="(experimental) Filter item @type. Python REGEX value",
+        default=None,
+    )
+
+    parser.add_argument(
+        "--filter-item-id",
+        # action="store_true",
+        help="(experimental) Filter item @id. Python REGEX value",
+        default=None,
+    )
+
     parser.add_argument("-v", "--verbose", action="store_true", help="Verbose")
 
     args = parser.parse_args()
 
     # print(args)
 
     wikitext = None
@@ -127,14 +146,25 @@
     elif args.page_title:
         wtdata = wiki_as_base.WikitextAsData().set_titles(args.page_title)
     elif args.pageids:
         wtdata = wiki_as_base.WikitextAsData().set_pageids(args.pageids)
     elif args.revids:
         wtdata = wiki_as_base.WikitextAsData().set_revids(args.revids)
 
+    if args.filter_item_type or args.filter_item_id:
+        # filters = {
+        #     "item_type": args.filter_item_type,
+        #     "item_id": args.filter_item_id,
+        # }
+        # print(args, filters)
+        wtdata.set_filters(item_type=args.filter_item_type, item_id=args.filter_item_id)
+
+    # print(args, filters)
+
+    # sys.exit()
     wtdata.prepare()
 
     if args.output_raw:
         # If multiple pages, behavior may be undefined
         # @TODO use wtdata.is_success()
 
         api_response = wtdata.get("api_response", strict=False)
@@ -144,14 +174,20 @@
         elif errors:
             print({"error": errors})
         else:
             print(wtdata.get("wikitext"))
 
         return EXIT_OK if wtdata.is_success() else EXIT_ERROR
 
+    elif args.output_streaming:
+        # @TODO maybe hint about errors? But JSON-SEQ allow individual items fail
+        #       if malformated, but we could have a full error at input data
+        wtdata.output_jsonseq()
+        # print("TODO")
+
     elif args.output_zip_file:
         # result = wtdata.output_zip(args.output_zip_file)
         wtdata.output_zip(args.output_zip_file)
         return EXIT_OK if wtdata.is_success() else EXIT_ERROR
         # if result:
         #     return EXIT_OK
         # else:
```

### Comparing `wiki_as_base-0.5.7/src/wiki_as_base/constants.py` & `wiki_as_base-0.5.8/src/wiki_as_base/constants.py`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.7/src/wiki_as_base/parser.py` & `wiki_as_base-0.5.8/src/wiki_as_base/parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,14 +43,39 @@
 
 
 @dataclass
 class WikisiteContext:
     ns: str
 
 
+class WikitextOutputFilter:
+    # item_type: str = field(init=False)
+    # item_id: str = field(init=False)
+    item_type: str
+    item_id: str
+
+    def __init__(self, item_type: str = None, item_id: str = None) -> None:
+        self.item_type = item_type
+        self.item_id = item_id
+        # pass
+
+    def allowed_id(self, id: str) -> bool:
+        # @TODO
+        return True
+
+    def allowed_type(self, item_type: str) -> bool:
+        # return False
+        # print(self.item_type, item_type)
+        if self.item_type:
+            if self.item_type != item_type:
+                return False
+
+        return True
+
+
 @dataclass
 class WikitextTemplateContext:
     name: str
     literal: str
     arguments: dict
     pagectx: WikipageContext
     # meta: dict
@@ -148,37 +173,42 @@
     extension_norm = extension
     if extension in _default_langs:
         extension_norm = _default_langs[extension]
 
     return extension_norm
 
 
-def parse_all(pagectx: WikipageContext, sitectx: WikisiteContext) -> list:
+def parse_all(
+    pagectx: WikipageContext,
+    sitectx: WikisiteContext,
+    itemfilter: WikitextOutputFilter = None,
+) -> list:
     page_data = []
 
-    tcorpus = wtxt_text_corpus(pagectx.wikitext)
-    if tcorpus:
-        page_data.append(
-            {
-                # "@type": "wiki/outline",
-                # "@type": "wtxt:DataCollectionOutline",
-                "@type": "wtxt:TextCorpus",
-                "@id": f"{sitectx.ns}:{pagectx.title_norm}#__textcorpus",
-                "wtxt:inWikipage": f"{sitectx.ns}:{pagectx.title_norm}",
-                # @TODO remove prefix outline/ from here
-                #       and implement on zip output only
-                "wtxt:suggestedFilename": f"corpora/{sitectx.ns}:{pagectx.title_norm}.txt",
-                "wtxt:uniqueFilename": f"corpora/{sitectx.ns}_pageid{pagectx.pageid}.txt",
-                "wtxt:timestamp": pagectx.timestamp,
-                "wtxt:user": pagectx.user,
-                # 'data_raw': outline,
-                # data_raw_key: outline,
-                "wtxt:literalData": tcorpus,
-            }
-        )
+    if not itemfilter or itemfilter.allowed_type("wtxt:TextCorpus"):
+        tcorpus = wtxt_text_corpus(pagectx.wikitext)
+        if tcorpus:
+            page_data.append(
+                {
+                    # "@type": "wiki/outline",
+                    # "@type": "wtxt:DataCollectionOutline",
+                    "@type": "wtxt:TextCorpus",
+                    "@id": f"{sitectx.ns}:{pagectx.title_norm}#__textcorpus",
+                    "wtxt:inWikipage": f"{sitectx.ns}:{pagectx.title_norm}",
+                    # @TODO remove prefix outline/ from here
+                    #       and implement on zip output only
+                    "wtxt:suggestedFilename": f"corpora/{sitectx.ns}:{pagectx.title_norm}.txt",
+                    "wtxt:uniqueFilename": f"corpora/{sitectx.ns}_pageid{pagectx.pageid}.txt",
+                    "wtxt:timestamp": pagectx.timestamp,
+                    "wtxt:user": pagectx.user,
+                    # 'data_raw': outline,
+                    # data_raw_key: outline,
+                    "wtxt:literalData": tcorpus,
+                }
+            )
 
     parsed = wtp.parse(pagectx.wikitext)
 
     total_tables = len(parsed.tables)
     tables_counter = 0
 
     # hstack = None
@@ -192,15 +222,25 @@
         hstack = _headings(pagectx.title, section.level, title, hstack)
 
         # Lets get only relevant contents for this header
         parsed_now = wtp.parse(contents)
         if len(parsed_now.sections) > 1:
             contents = parsed_now.sections[0].contents
 
-        contents_raw = wtp.remove_markup(contents.strip())
+        if len(contents.strip()) == 0:
+            continue
+
+        try:
+            contents_raw = wtp.remove_markup(contents.strip())
+        except TypeError:
+            # TypeError: unsupported format string passed to NoneType.__format__
+            # tcorpus = "wiki text parsing error"
+            continue
+
+        # contents_raw = wtp.remove_markup(contents.strip())
         if len(contents_raw) == 0:
             continue
 
         parsed_now_again = wtp.parse(contents)
 
         # # print(hstack)
         # # print(type(hstack))
@@ -211,81 +251,89 @@
         #         "title": title,
         #         "level": section.level,
         #         "contents": contents,
         #         "__templates": repr(parsed_now_again.templates),
         #     }
         # )
 
-        if len(parsed_now_again.tables):
-            for table in parsed_now_again.tables:
-                tables_counter += 1
-                page_data.append(
-                    {
-                        "@type": "wtxt:Table",
-                        "@id": f"{sitectx.ns}:{pagectx.title_norm}#__table{tables_counter}",
-                        "wtxt:titleContext": "\n".join(hstack),
-                        "wtxt:uniqueFilename": f"{sitectx.ns}_pageid{pagectx.pageid}_item{tables_counter}.csv",
-                        "wtxt:tableData": table.data(),
-                        # "_is_complete": True,
-                        # "_errors": None,
-                    }
-                )
+        if not itemfilter or itemfilter.allowed_type("wtxt:Table"):
+            if len(parsed_now_again.tables):
+                for table in parsed_now_again.tables:
+                    tables_counter += 1
+
+                    try:
+                        page_data.append(
+                            {
+                                "@type": "wtxt:Table",
+                                "@id": f"{sitectx.ns}:{pagectx.title_norm}#__table{tables_counter}",
+                                "wtxt:titleContext": "\n".join(hstack),
+                                "wtxt:uniqueFilename": f"{sitectx.ns}_pageid{pagectx.pageid}_item{tables_counter}.csv",
+                                "wtxt:tableData": table.data(),
+                                # "_is_complete": True,
+                                # "_errors": None,
+                            }
+                        )
+                    except AttributeError:
+                        # @TODO improve error handling
+                        continue
 
         # raise ValueError(contents)
 
-        templates = parse_templates(contents, pagectx)
-        if templates:
-            for template in templates:
-                # tables_counter += 1
-                page_data.append(
-                    {
-                        "@type": "wtxt:Template",
-                        "@id": f"{sitectx.ns}:Template:{template.name}#{template.local_id}",
-                        "wtxt:titleContext": "\n".join(hstack),
-                        # "wtxt:uniqueFilename": f"{sitectx.ns}_pageid{pagectx.pageid}_table{index_syntax}.csv",
-                        # "wtxt:uniqueFilename": f"{sitectx.ns}:Template:{template.name}#{template.local_id}",
-                        # # @TODO maybe enable wtxt:literalData (if debug on)
-                        # "wtxt:literalData": template.literal,
-                        "wtxt:templateData": template.arguments,
-                    }
-                )
-
-        index_syntax = 0
-        for item in WIKI_DATA_LANGS.splitlines():
-            results = wiki_as_base_from_syntaxhighlight_v2(contents, item)
-            if not results:
-                continue
-
-            for result in results:
-                if not result:
-                    continue
-                index_syntax += 1
-                fileextension = _fileextension(result[1])
-                if result[2]:
-                    page_data.append(
-                        {
-                            "@type": "wtxt:PreformattedCode",
-                            "wtxt:syntaxLang": result[1],
-                            "wtxt:suggestedFilename": result[2],
-                            "wtxt:uniqueFilename": f"{sitectx.ns}_pageid{pagectx.pageid}_item{index_syntax}.{fileextension}",
-                            "wtxt:inWikipage": f"{sitectx.ns}:{pagectx.title_norm}",
-                            "wtxt:literalData": result[0],
-                        }
-                    )
-                else:
+        if not itemfilter or itemfilter.allowed_type("wtxt:Template"):
+            templates = parse_templates(contents, pagectx)
+            if templates:
+                for template in templates:
+                    # tables_counter += 1
                     page_data.append(
                         {
-                            "@type": "wtxt:PreformattedCode",
-                            "wtxt:syntaxLang": result[1],
-                            "wtxt:uniqueFilename": f"{sitectx.ns}_pageid{pagectx.pageid}_item{index_syntax}.{fileextension}",
-                            "wtxt:inWikipage": f"{sitectx.ns}:{pagectx.title_norm}",
-                            "wtxt:literalData": result[0],
+                            "@type": "wtxt:Template",
+                            "@id": f"{sitectx.ns}:Template:{template.name}#{template.local_id}",
+                            "wtxt:titleContext": "\n".join(hstack),
+                            # "wtxt:uniqueFilename": f"{sitectx.ns}_pageid{pagectx.pageid}_table{index_syntax}.csv",
+                            # "wtxt:uniqueFilename": f"{sitectx.ns}:Template:{template.name}#{template.local_id}",
+                            # # @TODO maybe enable wtxt:literalData (if debug on)
+                            # "wtxt:literalData": template.literal,
+                            "wtxt:templateData": template.arguments,
                         }
                     )
 
+        if not itemfilter or itemfilter.allowed_type("wtxt:PreformattedCode"):
+            index_syntax = 0
+            for item in WIKI_DATA_LANGS.splitlines():
+                results = wiki_as_base_from_syntaxhighlight_v2(contents, item)
+                if not results:
+                    continue
+
+                for result in results:
+                    if not result:
+                        continue
+                    index_syntax += 1
+                    fileextension = _fileextension(result[1])
+                    if result[2]:
+                        page_data.append(
+                            {
+                                "@type": "wtxt:PreformattedCode",
+                                "wtxt:syntaxLang": result[1],
+                                "wtxt:suggestedFilename": result[2],
+                                "wtxt:uniqueFilename": f"{sitectx.ns}_pageid{pagectx.pageid}_item{index_syntax}.{fileextension}",
+                                "wtxt:inWikipage": f"{sitectx.ns}:{pagectx.title_norm}",
+                                "wtxt:literalData": result[0],
+                            }
+                        )
+                    else:
+                        page_data.append(
+                            {
+                                "@type": "wtxt:PreformattedCode",
+                                "wtxt:syntaxLang": result[1],
+                                "wtxt:uniqueFilename": f"{sitectx.ns}_pageid{pagectx.pageid}_item{index_syntax}.{fileextension}",
+                                "wtxt:inWikipage": f"{sitectx.ns}:{pagectx.title_norm}",
+                                "wtxt:literalData": result[0],
+                            }
+                        )
+
     return page_data
 
 
 def parse_sections(wikitext: str):
     return wtp.parse(wikitext).sections
 
 
@@ -297,15 +345,14 @@
     wikitext: str, pagectx: WikipageContext
 ) -> List[WikitextTemplateContext]:
     results = []
 
     parsed = wtp.parse(wikitext)
     if parsed.templates:
         for template in parsed.templates:
-
             if template.name.strip() not in WIKI_TEMPLATES:
                 # if WIKI_TEMPLATES.find(template.name.strip()) == -1:
                 # print('continue', template.name)
                 continue
 
             # raise ValueError(WIKI_TEMPLATES, template.name.strip())
             template.normal_name
@@ -331,15 +378,25 @@
             results.append(tpl)
 
     return results if len(results) > 0 else None
 
 
 def wtxt_text_corpus(wikitext: str) -> str:
     # @TODO remove <syntaxhighlight> and <source> blocks
-    tcorpus = wtp.remove_markup(wikitext)
+    # print("wtxt_text_corpus", wikitext)
+    # if not wikitext:
+    #     return False
+
+    try:
+        tcorpus = wtp.remove_markup(wikitext)
+    except TypeError:
+        # TypeError: unsupported format string passed to NoneType.__format__
+        # tcorpus = "wiki text parsing error"
+        tcorpus = "<!-- wiki text parsing error -->"
+
     return tcorpus
 
 
 def wiki_as_base_from_syntaxhighlight_v2(
     wikitext: str, lang: str = None, has_text: str = None, match_regex: str = None
 ) -> List[tuple]:
     """wiki_as_base_get_syntaxhighlight _summary_
```

### Comparing `wiki_as_base-0.5.7/src/wiki_as_base/wiki_as_base.py` & `wiki_as_base-0.5.8/src/wiki_as_base/wiki_as_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #                 SPDX-License-Identifier: Unlicense OR 0BSD
 #       VERSION:  ---
 #       CREATED:  ---
 # ==============================================================================
 
 # import copy
 from abc import ABC
+from ast import Tuple
 import csv
 
 # from ctypes import Union
 import datetime
 import io
 import json
 import os
@@ -38,38 +39,40 @@
 import zipfile
 import requests
 import requests_cache
 
 from .parser import (
     WikipageContext,
     WikisiteContext,
+    WikitextOutputFilter,
     parse_all,
     # parse_sections,
     # parse_tables,
     wtxt_text_corpus,
 )
 
 from .constants import WIKI_DATA_LANGS
 
-_REFVER = "0.5.6"
+_REFVER = "0.5.8"
 
 USER_AGENT = os.getenv("USER_AGENT", "wiki-as-base/" + _REFVER)
 WIKI_API = os.getenv("WIKI_API", "https://wiki.openstreetmap.org/w/api.php")
 
 # Consider using prefix like https://dumps.wikimedia.org/backup-index.html
 WIKI_NS = os.getenv("WIKI_NS", "osmwiki")
 WIKI_BASE = os.getenv("WIKI_BASE", lambda x: WIKI_API.replace("/w/api.php", "/wiki/"))
 
 # @TODO document better this part
 WTXT_PAGE_LIMIT = int(os.getenv("WTXT_PAGE_LIMIT", "50"))
 WTXT_PAGE_OFFSET = int(os.getenv("WTXT_PAGE_OFFSET", "0"))
 
 CACHE_DRIVER = os.getenv("CACHE_DRIVER", "sqlite")
-# @TODO increate default to 23 hours
-CACHE_TTL = os.getenv("CACHE_TTL", "3600")  # 1 hour
+
+# CACHE_TTL = int(os.getenv("CACHE_TTL", "3600"))  # 1 hour
+CACHE_TTL = int(os.getenv("CACHE_TTL", "82800"))  # 23 hours
 
 # @see https://requests-cache.readthedocs.io/en/stable/
 requests_cache.install_cache(
     "wikiasbase",
     # /tmp OpenFaaS allow /tmp be writtable even in read-only mode
     # However, is not granted that changes will persist or shared
     db_path="/tmp/wikiasbase_cache.sqlite",
@@ -222,15 +225,14 @@
                         )
 
     wmt = WikitextTable(wikitext)
     tables = wmt.get_tables()
     if tables and len(tables) > 0:
         index = 1
         for table in tables:
-
             table_data = [table["header"]] + table["data"]
 
             _tbl = {
                 "@type": "wtxt:Table",
                 "@id": f"t{index}",
                 "wtxt:tableData": table_data,
                 "_is_complete": table["_is_complete"],
@@ -569,15 +571,14 @@
             # print("test content" + type(content), file=sys.stderr)
             if filename is not None and content is not None:
                 # print("saved! filename " + filename, file=sys.stderr)
                 self.file_and_data[filename] = content
 
     def output(self, zip_path: str = None):
         if zip_path:
-
             if isinstance(zip_path, str) and os.path.isfile(zip_path):
                 os.remove(zip_path)
 
             with zipfile.ZipFile(
                 zip_path, "a", zipfile.ZIP_DEFLATED, False
             ) as zip_file:
                 for file_name, file_data in self.file_and_data.items():
@@ -602,30 +603,35 @@
 
     wikitext: str
     api_response: dict
     errors: list
     is_fetch_required: bool
     _wikiapi_meta: dict
     _req_params: dict
+    _req_params_rest: dict
     _reloaded: bool
+    # _filters: dict
+    _filters: WikitextOutputFilter = None
 
     # # The individual resources to add on the JSON-LD data field
     _resources: list
 
-    def __init__(self, api_params: dict = None) -> None:
+    def __init__(self, api_params: dict = None, filters: dict = None) -> None:
         """Initialize
 
         Instead of defining api_params, consider use set_wikitext() or
         set_titles
 
         Args:
             api_params (dict, optional): (advanced use)customize default_params.
                                          Defaults to None.
         """
 
+        # self._filters = dict
+
         default_params = {
             "action": "query",
             # "prop": "revisions",
             # "prop": "revisions|categories|templates",
             "prop": "revisions|categories",
             # "rvprop": "content",
             "rvprop": "content|timestamp|user",
@@ -667,43 +673,51 @@
         #     }
         # }
 
         if api_params is not None:
             default_params.update(api_params)
 
         self._req_params = default_params
+        self._req_params_rest = {
+            "titles": None,
+            "pageids": None,
+            "revids": None,
+        }
 
         # @TODO deal better with reset of the class to avoid reuse
         self.wikitext = None
         self.api_response = None
         self.errors = []
         self.is_fetch_required = None
+        self.is_fetch_incomplete = None
         self._wikiapi_meta = None
         self._reloaded = None
         self._resources = []
 
     def _add_resource(self, resource: dict):
         self._resources.append(resource)
 
     # def _pagination(self, pages: Union[list, str]):
-    def _pagination(self, pages: str) -> str:
-
+    def _pagination(self, pages: str) -> Tuple(str, str):
         parts = pages.split("|")
 
+        # return pages
+        # WTXT_PAGE_LIMIT = 9999999999
+
         if len(parts) <= WTXT_PAGE_LIMIT:
-            return pages
+            return pages, None
         else:
             # @TODO implement offset
             # @TODO implement offset and WTXT_PAGE_LIMIT without env vars
             # @TODO add note on generated JSON-LD about being paginated result
             sliced = parts[0:WTXT_PAGE_LIMIT]
-            return "|".join(sliced)
+            rest = parts[WTXT_PAGE_LIMIT:]
+            return "|".join(sliced), "|".join(rest)
 
     def _request_api(self):
-
         # Reset values
         self.wikitext = None
         self._wikiapi_meta = None
 
         # @TODO refactor this part to allow fetch several pages at once
 
         res = None
@@ -742,32 +756,30 @@
 
         if self.api_response is not None:
             self._request_api_post()
 
         # return (wikitext, wikiapi_meta)
 
     def _request_api_post(self):
-
         # # Initialize some checks
         # @TODO finish the refactoring of this part
         template_keys = WIKI_INFOBOXES.splitlines()
         syntaxhighlight_langs = WIKI_DATA_LANGS.splitlines()
 
         wsite = WikisiteContext(ns=WIKI_NS)
 
         for page in self.api_response["query"]["pages"]:
-
             wpage = WikipageContext(
                 wikitext=page["revisions"][0]["slots"]["main"]["content"],
                 pageid=page["pageid"],
                 title=page["title"],
                 user=page["revisions"][0]["user"],
                 timestamp=page["revisions"][0]["timestamp"],
             )
-            self._resources.extend(parse_all(wpage, wsite))
+            self._resources.extend(parse_all(wpage, wsite, self._filters))
             continue
 
         return True
 
         for page in self.api_response["query"]["pages"]:
             _pageid = page["pageid"]
             _title = page["title"]
@@ -868,15 +880,14 @@
                                 )
 
             wmt = WikitextTable(_wikitext)
             tables = wmt.get_tables()
             if tables and len(tables) > 0:
                 index = 1
                 for table in tables:
-
                     table_data = [table["header"]] + table["data"]
 
                     _tbl = {
                         "@type": "wtxt:Table",
                         # "@id": f"t{index}",
                         "@id": f"{WIKI_NS}_pageid{_pageid}_table{index}",
                         # "wtxt:uniqueFilename": f"{WIKI_NS}_pageid{_pageid}_table{index}.csv",
@@ -934,14 +945,38 @@
             }
             return _jsonld
 
         else:
             # @TODO filter better the errors, in special the ones from API
             return {"error": self.errors}
 
+    def output_jsonseq(self):
+        # @see https://datatracker.ietf.org/doc/html/rfc7464
+
+        if not self._reloaded:
+            self.prepare()
+
+        # if not self.errors:
+        if self.is_success():
+            # return wiki_as_base_all(self.wikitext, _next_release=True)
+
+            for item in self._resources:
+                # print("␞" + json.dumps(item, ensure_ascii=False), end="\n", file=os.stdout)
+                # sys.stdout.write("␞" + json.dumps(item, ensure_ascii=False) + "\n")
+                item_str = json.dumps(item, ensure_ascii=False)
+
+                sys.stdout.write("\x1e" + item_str + "\n")
+                # print(json.dumps(wtdata.output_jsonld(), ensure_ascii=False, indent=2))
+            # return _jsonld
+
+        else:
+            # @TODO filter better the errors, in special the ones from API
+            # return {"error": self.errors}
+            raise SyntaxError({"error": self.errors})
+
     def output_zip(self, zip_path: str = None) -> str:
         """output_zip Output as zip (either raw data or path to output)
 
         _extended_summary_
 
         Args:
             zip_path (str, optional): The path to save on disk. Defaults to None.
@@ -993,31 +1028,66 @@
                         }
                     ]
                 }
             }
             # Now, we can continue with post API :)
             self._request_api_post()
 
+        if self.is_fetch_incomplete:
+            if self._req_params_rest["pageids"] is not None:
+                self.set_pageids(self._req_params_rest["pageids"])
+
+            elif self._req_params_rest["revids"] is not None:
+                self.set_revids(self._req_params_rest["revids"])
+
+            elif self._req_params_rest["titles"] is not None:
+                self.set_titles(self._req_params_rest["titles"])
+            else:
+                raise NotImplemented
+
+            # Move this to somewhere else
+            print("loop...", file=sys.stderr)
+            return self.prepare()
+
         self._reloaded = True
 
         return self
 
+    # def set_filters(self, filters: dict):
+    def set_filters(self, item_type: str = None, item_id: str = None) -> None:
+        # self.item_type = item_type
+        # self.item_id = item_id
+        # pass
+        # if filters:
+        filters = WikitextOutputFilter(item_type=item_type, item_id=item_id)
+
+        self._filters = filters
+        return self
+
     def set_pageids(self, pageids: str):
         """set_pageids set pageids for remote call
 
         Args:
             pageids (str): The Pageids. Use | as separator
         """
-        self._req_params["pageids"] = self._pagination(pageids)
+        # self._req_params["pageids"] = self._pagination(pageids)
+        (
+            self._req_params["pageids"],
+            self._req_params_rest["pageids"],
+        ) = self._pagination(pageids)
 
         # If user define pageids directly, we assume wants remote call and
         # unset titles and revids
         self.is_fetch_required = True
-        del self._req_params["titles"]
-        del self._req_params["revids"]
+        self.is_fetch_incomplete = bool(self._req_params_rest["pageids"])
+
+        if "titles" in self._req_params:
+            del self._req_params["titles"]
+        if "revids" in self._req_params:
+            del self._req_params["revids"]
 
         return self
 
     def set_pages_autodetect(self, pages_auto: str):
         """set_pages_autodetect autodetect set_pageids() or set_titles()
 
         Args:
@@ -1049,35 +1119,42 @@
 
     def set_revids(self, revids: str):
         """set_revids set revision IDs for remote call
 
         Args:
             revids (str): The Revision IDs. Use | as separator
         """
-        self._req_params["revids"] = self._pagination(revids)
+        self._req_params["revids"], self._req_params_rest["revids"] = self._pagination(
+            revids
+        )
 
         # If user define revids directly, we assume wants remote call and
         # unset pageids and titles
         self.is_fetch_required = True
+        self.is_fetch_incomplete = bool(self._req_params_rest["revids"])
         del self._req_params["pageids"]
         del self._req_params["titles"]
 
         return self
 
     def set_titles(self, titles: str):
         """set_pageids set page titles for remote call
 
         Args:
             pageids (str): The titles. Use | as separator
         """
-        self._req_params["titles"] = self._pagination(titles)
+        # self._req_params["titles"] = self._pagination(titles)
+        self._req_params["titles"], self._req_params_rest["titles"] = self._pagination(
+            titles
+        )
 
         # If user define titles directly, we assume wants remote call and
         # unset pageids and revids
         self.is_fetch_required = True
+        self.is_fetch_incomplete = bool(self._req_params_rest["titles"])
         del self._req_params["pageids"]
         del self._req_params["revids"]
 
         return self
 
     def set_wikitext(self, wikitext: str):
         """set_wikitext set Wikitext directly instead of make API request
@@ -1201,14 +1278,19 @@
         headings = self.get_headings()
         return "<article>\n" + headings + "</article>"
 
 
 # Two example queries
 # - https://wiki.openstreetmap.org/w/api.php?action=query&generator=categorymembers&gcmtitle=Category:External_reference_tag&prop=info
 # - https://wiki.openstreetmap.org/w/api.php?action=query&cmtitle=Category:External_reference_tag&list=categorymembers&format=json&formatversion=2
+#  - Web preview
+#    - https://wiki.openstreetmap.org/wiki/Special:ApiSandbox#action=query&format=json&prop=&list=categorymembers&continue=-%7C%7C&formatversion=2&cmtitle=Category%3AExternal_reference_tag&cmcontinue=page%7C4b45593a4e4554574f524b3a57494b4944415441%7C186683
+#    - https://wiki.openstreetmap.org/w/api.php?action=query&format=json&prop=&list=categorymembers&continue=-%7C%7C&formatversion=2&cmtitle=Category%3AExternal_reference_tag&cmcontinue=page%7C4b45593a4e4554574f524b3a57494b4944415441%7C186683&cmlimit=500
+# - Category:Tagging_Mistakes
+#   - https://wiki.openstreetmap.org/wiki/Special:ApiSandbox#action=query&format=json&prop=&list=categorymembers&continue=-%7C%7C&formatversion=2&cmtitle=Category%3ATagging_Mistakes&cmcontinue=page%7C4b45593a4e4554574f524b3a57494b4944415441%7C186683&cmlimit=500
 class WikitextPagesFromCategory(WikitextGenericPart):
     """Return page IDs from category name
 
     @see https://www.mediawiki.org/wiki/API:Categorymembers
 
     For openstreetap categories:
     https://wiki.openstreetmap.org/wiki/Special:Categories
@@ -1216,15 +1298,14 @@
 
     errors: list
     _pageids: list
     _req_params: dict
     _is_done: bool
 
     def __init__(self, api_params: dict = None) -> None:
-
         # @see https://www.mediawiki.org/wiki/API:Categorymembers
         default_params = {
             "action": "query",
             "list": "categorymembers",
             "cmprop": "ids|title|timestamp",
             "cmlimit": "500",
             "cmtitle": None,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wiki_as_base-0.5.7/src/wiki_as_base.egg-info/PKG-INFO` & `wiki_as_base-0.5.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wiki-as-base
-Version: 0.5.7
+Name: wiki_as_base
+Version: 0.5.8
 Summary: Use MediaWiki Wiki page content as read-only database
 Home-page: https://github.com/fititnt/wiki_as_base-py
 Author: Emerson Rocha
 Author-email: rocha@ieee.org
 Project-URL: Bug Tracker, https://github.com/fititnt/wiki_as_base-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -45,20 +45,16 @@
 ---
 
 ## Installing
 
 ```bash
 pip install wiki_as_base --upgrade
 
-## Alternative: 
-# pip install wiki-as-base==0.5.6
-```
-
-```nasj
-
+## Alternative:
+# pip install wiki_as_base==0.5.8
 ```
 
 ### Environment variables
 Customize for your needs. They're shared between command line and the library.
 
 ```bash
 export WIKI_API='https://wiki.openstreetmap.org/w/api.php'
@@ -215,15 +211,15 @@
 > **NOTE**: for production usage (if you can't review releases or are not locked into Docker images)
 > consider enforce a very specific release
 
 
 **Production usage**
 ```txt
 # requirements.txt
-wiki_as_base==0.5.5
+wiki_as_base==0.5.8
 ```
 
 **Other cases (or use in your local machine)**
 
 ```bash
 # Run this via cli for force redownload lastest. Do not use --pre (pre-releases)
 pip install wiki_as_base --upgrade
```

### Comparing `wiki_as_base-0.5.7/src/wiki_as_base.egg-info/SOURCES.txt` & `wiki_as_base-0.5.8/src/wiki_as_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.7/tests/test_internals.py` & `wiki_as_base-0.5.8/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.7/tests/test_tables.py` & `wiki_as_base-0.5.8/tests/test_tables.py`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.7/tests/test_wikitext.py` & `wiki_as_base-0.5.8/tests/test_wikitext.py`

 * *Files identical despite different names*

### Comparing `wiki_as_base-0.5.7/tests/test_wikitext_with_network.py` & `wiki_as_base-0.5.8/tests/test_wikitext_with_network.py`

 * *Files identical despite different names*

