# Comparing `tmp/BLACKFORGE2-0.2.6.tar.gz` & `tmp/BLACKFORGE2-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLACKFORGE2-0.2.6.tar", last modified: Thu Jul  6 10:24:43 2023, max compression
+gzip compressed data, was "BLACKFORGE2-0.2.7.tar", last modified: Fri Jul  7 23:05:11 2023, max compression
```

## Comparing `BLACKFORGE2-0.2.6.tar` & `BLACKFORGE2-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 10:24:43.312932 BLACKFORGE2-0.2.6/
-drwxrwxrwx   0        0        0        0 2023-07-06 10:24:43.298944 BLACKFORGE2-0.2.6/BLACKFORGE2/
--rw-rw-rw-   0        0        0    14607 2023-07-06 10:22:14.000000 BLACKFORGE2-0.2.6/BLACKFORGE2/FORGE.py
--rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.2.6/BLACKFORGE2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 10:24:43.309939 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/
--rw-rw-rw-   0        0        0      312 2023-07-06 10:24:43.000000 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-06 10:24:43.000000 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:24:43.000000 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 10:24:43.000000 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-06 10:24:43.000000 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      312 2023-07-06 10:24:43.311935 BLACKFORGE2-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     8967 2023-06-16 21:39:12.000000 BLACKFORGE2-0.2.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-06 10:24:43.312932 BLACKFORGE2-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-07-06 10:24:24.000000 BLACKFORGE2-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 23:05:11.094040 BLACKFORGE2-0.2.7/
+drwxrwxrwx   0        0        0        0 2023-07-07 23:05:11.082639 BLACKFORGE2-0.2.7/BLACKFORGE2/
+-rw-rw-rw-   0        0        0    14941 2023-07-07 23:04:13.000000 BLACKFORGE2-0.2.7/BLACKFORGE2/FORGE.py
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.2.7/BLACKFORGE2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 23:05:11.092043 BLACKFORGE2-0.2.7/BLACKFORGE2.egg-info/
+-rw-rw-rw-   0        0        0      312 2023-07-07 23:05:10.000000 BLACKFORGE2-0.2.7/BLACKFORGE2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-07 23:05:10.000000 BLACKFORGE2-0.2.7/BLACKFORGE2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 23:05:10.000000 BLACKFORGE2-0.2.7/BLACKFORGE2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 23:05:10.000000 BLACKFORGE2-0.2.7/BLACKFORGE2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 23:05:10.000000 BLACKFORGE2-0.2.7/BLACKFORGE2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      312 2023-07-07 23:05:11.093041 BLACKFORGE2-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8967 2023-06-16 21:39:12.000000 BLACKFORGE2-0.2.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-07 23:05:11.094040 BLACKFORGE2-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-07-07 23:04:48.000000 BLACKFORGE2-0.2.7/setup.py
```

### Comparing `BLACKFORGE2-0.2.6/BLACKFORGE2/FORGE.py` & `BLACKFORGE2-0.2.7/BLACKFORGE2/FORGE.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,16 +325,23 @@
 
 """ SUPPORT FUNCTIONS """
 def clamp(num:int, min_value:int, max_value:int):
 	return max(min(num, max_value), min_value)
 
 def import_folder(path:str) -> list:	
 	surface_list = []
+	file_list = []
 	for _, __, image_files in walk(path):
-		for image in image_files:
+		for index, image in enumerate(image_files):
+			file_list.append(image)
+
+		# sort images based on numerical values in the image names: run1.png will always come before run12.png as walk doesnt sort files returned.
+		file_list.sort(key=lambda image: int(''.join(filter(str.isdigit, image))))
+		
+		for index, image in enumerate(file_list):
 			full_path = path + '/' + image
 			image_surf =get_image(full_path).convert_alpha()
 			surface_list.append(image_surf)
 
 	return surface_list
 
 def import_csv_layout(path:str) -> list:
```

### Comparing `BLACKFORGE2-0.2.6/LICENSE` & `BLACKFORGE2-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BLACKFORGE2-0.2.6/README.rst` & `BLACKFORGE2-0.2.7/README.rst`

 * *Files identical despite different names*

