# Comparing `tmp/sqd-song-edit-1.1.1.tar.gz` & `tmp/sqd-song-edit-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqd-song-edit-1.1.1.tar", last modified: Sat Jul  8 19:03:12 2023, max compression
+gzip compressed data, was "sqd-song-edit-1.1.2.tar", last modified: Sat Jul  8 19:14:51 2023, max compression
```

## Comparing `sqd-song-edit-1.1.1.tar` & `sqd-song-edit-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 19:03:12.265355 sqd-song-edit-1.1.1/
--rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:16.000000 sqd-song-edit-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       33 2022-10-15 13:34:48.000000 sqd-song-edit-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1774 2023-07-08 19:03:12.262397 sqd-song-edit-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-07-08 09:59:58.000000 sqd-song-edit-1.1.1/README.md
--rw-rw-rw-   0        0        0      712 2023-07-08 19:02:09.000000 sqd-song-edit-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 19:03:12.267372 sqd-song-edit-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0       36 2022-10-14 07:04:08.000000 sqd-song-edit-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 19:03:12.113556 sqd-song-edit-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 19:03:12.215587 sqd-song-edit-1.1.1/src/sqd_song_edit/
--rw-rw-rw-   0        0        0      398 2023-07-08 19:02:04.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/__init__.py
--rw-rw-rw-   0        0        0     2932 2023-07-08 19:01:54.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/__main__.py
--rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/color.py
--rw-rw-rw-   0        0        0      484 2023-07-08 10:44:24.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/errors.py
--rw-rw-rw-   0        0        0     7414 2023-07-08 18:24:45.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/start.py
--rw-rw-rw-   0        0        0      291 2023-07-08 10:45:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 19:03:12.257010 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/
--rw-rw-rw-   0        0        0     1774 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 19:14:51.481880 sqd-song-edit-1.1.2/
+-rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:16.000000 sqd-song-edit-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0       33 2022-10-15 13:34:48.000000 sqd-song-edit-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1774 2023-07-08 19:14:51.475277 sqd-song-edit-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-07-08 09:59:58.000000 sqd-song-edit-1.1.2/README.md
+-rw-rw-rw-   0        0        0      712 2023-07-08 19:13:37.000000 sqd-song-edit-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 19:14:51.482878 sqd-song-edit-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       36 2022-10-14 07:04:08.000000 sqd-song-edit-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 19:14:51.227896 sqd-song-edit-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 19:14:51.386795 sqd-song-edit-1.1.2/src/sqd_song_edit/
+-rw-rw-rw-   0        0        0      398 2023-07-08 19:13:32.000000 sqd-song-edit-1.1.2/src/sqd_song_edit/__init__.py
+-rw-rw-rw-   0        0        0     2932 2023-07-08 19:13:23.000000 sqd-song-edit-1.1.2/src/sqd_song_edit/__main__.py
+-rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqd-song-edit-1.1.2/src/sqd_song_edit/color.py
+-rw-rw-rw-   0        0        0      484 2023-07-08 10:44:24.000000 sqd-song-edit-1.1.2/src/sqd_song_edit/errors.py
+-rw-rw-rw-   0        0        0     7414 2023-07-08 18:24:45.000000 sqd-song-edit-1.1.2/src/sqd_song_edit/start.py
+-rw-rw-rw-   0        0        0      291 2023-07-08 10:45:12.000000 sqd-song-edit-1.1.2/src/sqd_song_edit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 19:14:51.459717 sqd-song-edit-1.1.2/src/sqd_song_edit.egg-info/
+-rw-rw-rw-   0        0        0     1774 2023-07-08 19:14:50.000000 sqd-song-edit-1.1.2/src/sqd_song_edit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-07-08 19:14:51.000000 sqd-song-edit-1.1.2/src/sqd_song_edit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 19:14:50.000000 sqd-song-edit-1.1.2/src/sqd_song_edit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-08 19:14:50.000000 sqd-song-edit-1.1.2/src/sqd_song_edit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2023-07-08 19:14:51.000000 sqd-song-edit-1.1.2/src/sqd_song_edit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-08 19:14:51.000000 sqd-song-edit-1.1.2/src/sqd_song_edit.egg-info/top_level.txt
```

### Comparing `sqd-song-edit-1.1.1/LICENSE` & `sqd-song-edit-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqd-song-edit-1.1.1/PKG-INFO` & `sqd-song-edit-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqd-song-edit
-Version: 1.1.1
+Version: 1.1.2
 Summary: edit song cover art and metadeta easily!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

### Comparing `sqd-song-edit-1.1.1/pyproject.toml` & `sqd-song-edit-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqd-song-edit"
-version = "1.1.1"
+version = "1.1.2"
 description = "edit song cover art and metadeta easily!"
 authors = [
     { name="sqdnoises" }
 ]
 
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `sqd-song-edit-1.1.1/src/sqd_song_edit/__main__.py` & `sqd-song-edit-1.1.2/src/sqd_song_edit/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     parser.add_argument("-V", "--version",
                         action="version", version=full_title+" "+version)
     parser.add_argument("-l", "--license",
                         action="version", version=copyright+" - MIT License. For more information see: https://opensource.org/license/mit/",
                         help="show program's license and exit")
     parser.add_argument("-r", "--remove-metadata",
                         action="store_true", help="remove every song metadata and then show the options")
-    parser.add_argument("-u", "--update",
+    parser.add_argument("-U", "--update",
                         action="store_true", help="show update program command and exit")
 
     args = parser.parse_args()
 
     if args.update:
         try:
             new_version = luddite.get_version_pypi(full_title)
```

### Comparing `sqd-song-edit-1.1.1/src/sqd_song_edit/color.py` & `sqd-song-edit-1.1.2/src/sqd_song_edit/color.py`

 * *Files identical despite different names*

### Comparing `sqd-song-edit-1.1.1/src/sqd_song_edit/start.py` & `sqd-song-edit-1.1.2/src/sqd_song_edit/start.py`

 * *Files identical despite different names*

### Comparing `sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/PKG-INFO` & `sqd-song-edit-1.1.2/src/sqd_song_edit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqd-song-edit
-Version: 1.1.1
+Version: 1.1.2
 Summary: edit song cover art and metadeta easily!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

