# Comparing `tmp/sqd-song-edit-1.0.0.tar.gz` & `tmp/sqd-song-edit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqd-song-edit-1.0.0.tar", last modified: Sat Jul  8 18:00:24 2023, max compression
+gzip compressed data, was "sqd-song-edit-1.0.1.tar", last modified: Sat Jul  8 18:41:08 2023, max compression
```

## Comparing `sqd-song-edit-1.0.0.tar` & `sqd-song-edit-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 18:00:24.107551 sqd-song-edit-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:16.000000 sqd-song-edit-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       33 2022-10-15 13:34:48.000000 sqd-song-edit-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1774 2023-07-08 18:00:24.099001 sqd-song-edit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-07-08 09:59:58.000000 sqd-song-edit-1.0.0/README.md
--rw-rw-rw-   0        0        0      712 2023-07-08 17:02:26.000000 sqd-song-edit-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 18:00:24.109553 sqd-song-edit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       36 2022-10-14 07:04:08.000000 sqd-song-edit-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 18:00:23.751623 sqd-song-edit-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 18:00:23.939267 sqd-song-edit-1.0.0/src/sqd_song_edit/
--rw-rw-rw-   0        0        0      402 2023-07-08 14:33:11.000000 sqd-song-edit-1.0.0/src/sqd_song_edit/__init__.py
--rw-rw-rw-   0        0        0     2162 2023-07-08 17:27:02.000000 sqd-song-edit-1.0.0/src/sqd_song_edit/__main__.py
--rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqd-song-edit-1.0.0/src/sqd_song_edit/color.py
--rw-rw-rw-   0        0        0      484 2023-07-08 10:44:24.000000 sqd-song-edit-1.0.0/src/sqd_song_edit/errors.py
--rw-rw-rw-   0        0        0     7412 2023-07-08 17:48:31.000000 sqd-song-edit-1.0.0/src/sqd_song_edit/start.py
--rw-rw-rw-   0        0        0      291 2023-07-08 10:45:12.000000 sqd-song-edit-1.0.0/src/sqd_song_edit/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 18:00:24.083901 sqd-song-edit-1.0.0/src/sqd_song_edit.egg-info/
--rw-rw-rw-   0        0        0     1774 2023-07-08 18:00:23.000000 sqd-song-edit-1.0.0/src/sqd_song_edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-07-08 18:00:23.000000 sqd-song-edit-1.0.0/src/sqd_song_edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 18:00:23.000000 sqd-song-edit-1.0.0/src/sqd_song_edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-08 18:00:23.000000 sqd-song-edit-1.0.0/src/sqd_song_edit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2023-07-08 18:00:23.000000 sqd-song-edit-1.0.0/src/sqd_song_edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-08 18:00:23.000000 sqd-song-edit-1.0.0/src/sqd_song_edit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 18:41:08.695776 sqd-song-edit-1.0.1/
+-rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:16.000000 sqd-song-edit-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       33 2022-10-15 13:34:48.000000 sqd-song-edit-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1774 2023-07-08 18:41:08.691230 sqd-song-edit-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-07-08 09:59:58.000000 sqd-song-edit-1.0.1/README.md
+-rw-rw-rw-   0        0        0      712 2023-07-08 18:39:40.000000 sqd-song-edit-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 18:41:08.696811 sqd-song-edit-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       36 2022-10-14 07:04:08.000000 sqd-song-edit-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:41:08.461633 sqd-song-edit-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 18:41:08.613235 sqd-song-edit-1.0.1/src/sqd_song_edit/
+-rw-rw-rw-   0        0        0      402 2023-07-08 18:39:34.000000 sqd-song-edit-1.0.1/src/sqd_song_edit/__init__.py
+-rw-rw-rw-   0        0        0     2162 2023-07-08 17:27:02.000000 sqd-song-edit-1.0.1/src/sqd_song_edit/__main__.py
+-rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqd-song-edit-1.0.1/src/sqd_song_edit/color.py
+-rw-rw-rw-   0        0        0      484 2023-07-08 10:44:24.000000 sqd-song-edit-1.0.1/src/sqd_song_edit/errors.py
+-rw-rw-rw-   0        0        0     7414 2023-07-08 18:24:45.000000 sqd-song-edit-1.0.1/src/sqd_song_edit/start.py
+-rw-rw-rw-   0        0        0      291 2023-07-08 10:45:12.000000 sqd-song-edit-1.0.1/src/sqd_song_edit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:41:08.680677 sqd-song-edit-1.0.1/src/sqd_song_edit.egg-info/
+-rw-rw-rw-   0        0        0     1774 2023-07-08 18:41:08.000000 sqd-song-edit-1.0.1/src/sqd_song_edit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-07-08 18:41:08.000000 sqd-song-edit-1.0.1/src/sqd_song_edit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:41:08.000000 sqd-song-edit-1.0.1/src/sqd_song_edit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-08 18:41:08.000000 sqd-song-edit-1.0.1/src/sqd_song_edit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2023-07-08 18:41:08.000000 sqd-song-edit-1.0.1/src/sqd_song_edit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-08 18:41:08.000000 sqd-song-edit-1.0.1/src/sqd_song_edit.egg-info/top_level.txt
```

### Comparing `sqd-song-edit-1.0.0/LICENSE` & `sqd-song-edit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqd-song-edit-1.0.0/PKG-INFO` & `sqd-song-edit-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqd-song-edit
-Version: 1.0.0
+Version: 1.0.1
 Summary: edit song cover art and metadeta easily!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

### Comparing `sqd-song-edit-1.0.0/pyproject.toml` & `sqd-song-edit-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqd-song-edit"
-version = "1.0.0"
+version = "1.0.1"
 description = "edit song cover art and metadeta easily!"
 authors = [
     { name="sqdnoises" }
 ]
 
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `sqd-song-edit-1.0.0/src/sqd_song_edit/__main__.py` & `sqd-song-edit-1.0.1/src/sqd_song_edit/__main__.py`

 * *Files identical despite different names*

### Comparing `sqd-song-edit-1.0.0/src/sqd_song_edit/color.py` & `sqd-song-edit-1.0.1/src/sqd_song_edit/color.py`

 * *Files identical despite different names*

### Comparing `sqd-song-edit-1.0.0/src/sqd_song_edit/start.py` & `sqd-song-edit-1.0.1/src/sqd_song_edit/start.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 
 def main(args: argparse.ArgumentParser) -> None:
     try:
         saved = None
 
         if args.interactive:
-            args.file = input(f"{color.bright_blue}File to convert: {color.bright_white}").strip()
+            args.file = input(f"{color.bright_blue}Song file to edit: {color.bright_white}").strip()
 
             if args.file.startswith('"') and args.file.endswith('"'):
                 args.file = args.file.split('"', 1)[1].rsplit('"', 1)[0]
             elif args.file.startswith("'") and args.file.endswith("'"):
                 args.file = args.file.split("'", 1)[1].rsplit("'", 1)[0]
 
         inp = os.path.normpath(args.file)
```

### Comparing `sqd-song-edit-1.0.0/src/sqd_song_edit.egg-info/PKG-INFO` & `sqd-song-edit-1.0.1/src/sqd_song_edit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqd-song-edit
-Version: 1.0.0
+Version: 1.0.1
 Summary: edit song cover art and metadeta easily!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

