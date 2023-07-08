# Comparing `tmp/sqd-song-edit-1.1.0.tar.gz` & `tmp/sqd-song-edit-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqd-song-edit-1.1.0.tar", last modified: Sat Jul  8 18:52:56 2023, max compression
+gzip compressed data, was "sqd-song-edit-1.1.1.tar", last modified: Sat Jul  8 19:03:12 2023, max compression
```

## Comparing `sqd-song-edit-1.1.0.tar` & `sqd-song-edit-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 18:52:56.216293 sqd-song-edit-1.1.0/
--rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:16.000000 sqd-song-edit-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       33 2022-10-15 13:34:48.000000 sqd-song-edit-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1774 2023-07-08 18:52:56.211784 sqd-song-edit-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-07-08 09:59:58.000000 sqd-song-edit-1.1.0/README.md
--rw-rw-rw-   0        0        0      712 2023-07-08 18:51:41.000000 sqd-song-edit-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 18:52:56.219326 sqd-song-edit-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0       36 2022-10-14 07:04:08.000000 sqd-song-edit-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 18:52:56.006806 sqd-song-edit-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 18:52:56.146908 sqd-song-edit-1.1.0/src/sqd_song_edit/
--rw-rw-rw-   0        0        0      402 2023-07-08 18:51:34.000000 sqd-song-edit-1.1.0/src/sqd_song_edit/__init__.py
--rw-rw-rw-   0        0        0     2860 2023-07-08 18:48:23.000000 sqd-song-edit-1.1.0/src/sqd_song_edit/__main__.py
--rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqd-song-edit-1.1.0/src/sqd_song_edit/color.py
--rw-rw-rw-   0        0        0      484 2023-07-08 10:44:24.000000 sqd-song-edit-1.1.0/src/sqd_song_edit/errors.py
--rw-rw-rw-   0        0        0     7414 2023-07-08 18:24:45.000000 sqd-song-edit-1.1.0/src/sqd_song_edit/start.py
--rw-rw-rw-   0        0        0      291 2023-07-08 10:45:12.000000 sqd-song-edit-1.1.0/src/sqd_song_edit/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 18:52:56.199706 sqd-song-edit-1.1.0/src/sqd_song_edit.egg-info/
--rw-rw-rw-   0        0        0     1774 2023-07-08 18:52:55.000000 sqd-song-edit-1.1.0/src/sqd_song_edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-07-08 18:52:55.000000 sqd-song-edit-1.1.0/src/sqd_song_edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 18:52:55.000000 sqd-song-edit-1.1.0/src/sqd_song_edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-08 18:52:55.000000 sqd-song-edit-1.1.0/src/sqd_song_edit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2023-07-08 18:52:55.000000 sqd-song-edit-1.1.0/src/sqd_song_edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-08 18:52:55.000000 sqd-song-edit-1.1.0/src/sqd_song_edit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 19:03:12.265355 sqd-song-edit-1.1.1/
+-rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:16.000000 sqd-song-edit-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       33 2022-10-15 13:34:48.000000 sqd-song-edit-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1774 2023-07-08 19:03:12.262397 sqd-song-edit-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-07-08 09:59:58.000000 sqd-song-edit-1.1.1/README.md
+-rw-rw-rw-   0        0        0      712 2023-07-08 19:02:09.000000 sqd-song-edit-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 19:03:12.267372 sqd-song-edit-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       36 2022-10-14 07:04:08.000000 sqd-song-edit-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 19:03:12.113556 sqd-song-edit-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 19:03:12.215587 sqd-song-edit-1.1.1/src/sqd_song_edit/
+-rw-rw-rw-   0        0        0      398 2023-07-08 19:02:04.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/__init__.py
+-rw-rw-rw-   0        0        0     2932 2023-07-08 19:01:54.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/__main__.py
+-rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/color.py
+-rw-rw-rw-   0        0        0      484 2023-07-08 10:44:24.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/errors.py
+-rw-rw-rw-   0        0        0     7414 2023-07-08 18:24:45.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/start.py
+-rw-rw-rw-   0        0        0      291 2023-07-08 10:45:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 19:03:12.257010 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/
+-rw-rw-rw-   0        0        0     1774 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-08 19:03:12.000000 sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/top_level.txt
```

### Comparing `sqd-song-edit-1.1.0/LICENSE` & `sqd-song-edit-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqd-song-edit-1.1.0/PKG-INFO` & `sqd-song-edit-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqd-song-edit
-Version: 1.1.0
+Version: 1.1.1
 Summary: edit song cover art and metadeta easily!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

### Comparing `sqd-song-edit-1.1.0/pyproject.toml` & `sqd-song-edit-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqd-song-edit"
-version = "1.1.0"
+version = "1.1.1"
 description = "edit song cover art and metadeta easily!"
 authors = [
     { name="sqdnoises" }
 ]
 
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `sqd-song-edit-1.1.0/src/sqd_song_edit/__main__.py` & `sqd-song-edit-1.1.1/src/sqd_song_edit/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import luddite
 import argparse
 
 from . import (
-    __name__ as name,
+    __title__ as title,
+    __full_title__ as full_title,
     __description__ as description,
     __copyright__ as copyright,
     __version__ as version
 )
 from . import color
 from .start import main as start
 
@@ -17,64 +18,64 @@
     readline = Readline()
 else:
     # macOS/linux
     import readline
 
 def main():
     parser = argparse.ArgumentParser(
-        prog = name,
+        prog = title,
         description = description,
-        epilog = "Example: song-edit -f audio_file.mp3"
+        epilog = f"Example: {title} -f audio_file.mp3"
     )
 
     parser.add_argument("-f", "--file",
                         help="audio file to edit")
     parser.add_argument("-i", "--interactive",
                         action="store_true", help="start an interactive conversion")
     parser.add_argument("-v", "--verbose",
                         action="store_true", help="print more output")
     parser.add_argument("-V", "--version",
-                        action="version", version=name+" "+version)
+                        action="version", version=full_title+" "+version)
     parser.add_argument("-l", "--license",
                         action="version", version=copyright+" - MIT License. For more information see: https://opensource.org/license/mit/",
                         help="show program's license and exit")
     parser.add_argument("-r", "--remove-metadata",
                         action="store_true", help="remove every song metadata and then show the options")
     parser.add_argument("-u", "--update",
                         action="store_true", help="show update program command and exit")
 
     args = parser.parse_args()
 
     if args.update:
         try:
-            new_version = luddite.get_version_pypi(name)
+            new_version = luddite.get_version_pypi(full_title)
         except:
             new_version = None
 
         print(f"Installed version: {version}")
         print(f"PyPi version: {new_version}")
         print()
 
         if new_version and version != new_version:
             print(f"{color.bright_blue}{version} {color.bright_green}>> {color.bright_blue}{new_version}{color.reset}")
         
-        print(f"{color.bright_white}Use {color.bright_red}pip install -U {name}{color.bright_white} to update!{color.reset}")
+        print(f"{color.bright_white}Use {color.bright_red}pip install -U {full_title}{color.bright_white} to update!{color.reset}")
         exit()
 
     if not args.interactive and not args.file:
         parser.error("Specify either a file or pass `-i` for an interactive session.")
 
     start(args)
 
     try:
-        new_version = luddite.get_version_pypi(name)
+        new_version = luddite.get_version_pypi(full_title)
     except:
         new_version = None
     
     if new_version and version != new_version:
         print()
-        print(f"{color.bright_green}New version for {color.bright_yellow}{name}{color.bright_green} is available.{color.reset}")
+        print(f"{color.bright_green}New version for {color.bright_yellow}{full_title}{color.bright_green} is available.{color.reset}")
         print(f"{color.bright_blue}{version} {color.bright_green}>> {color.bright_blue}{new_version}{color.reset}")
-        print(f"{color.bright_white}Use {color.bright_red}pip install -U {name}{color.bright_white} to update!{color.reset}")
+        print(f"{color.bright_white}Use {color.bright_red}pip install -U {full_title}{color.bright_white} to update!{color.reset}")
 
 if __name__ == "__main__":
     main()
```

### Comparing `sqd-song-edit-1.1.0/src/sqd_song_edit/color.py` & `sqd-song-edit-1.1.1/src/sqd_song_edit/color.py`

 * *Files identical despite different names*

### Comparing `sqd-song-edit-1.1.0/src/sqd_song_edit/start.py` & `sqd-song-edit-1.1.1/src/sqd_song_edit/start.py`

 * *Files identical despite different names*

### Comparing `sqd-song-edit-1.1.0/src/sqd_song_edit.egg-info/PKG-INFO` & `sqd-song-edit-1.1.1/src/sqd_song_edit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqd-song-edit
-Version: 1.1.0
+Version: 1.1.1
 Summary: edit song cover art and metadeta easily!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```
