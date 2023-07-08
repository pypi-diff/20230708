# Comparing `tmp/ar_filters-0.0.7.tar.gz` & `tmp/ar_filters-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ar_filters-0.0.7.tar", last modified: Fri Jun 16 08:11:21 2023, max compression
+gzip compressed data, was "ar_filters-0.0.8.tar", last modified: Sat Jul  8 05:05:25 2023, max compression
```

## Comparing `ar_filters-0.0.7.tar` & `ar_filters-0.0.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 08:11:21.093558 ar_filters-0.0.7/
--rw-rw-rw-   0        0        0     1093 2023-06-10 13:07:48.000000 ar_filters-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-16 06:53:45.000000 ar_filters-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     9425 2023-06-16 08:11:21.093558 ar_filters-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     8990 2023-06-10 13:11:14.000000 ar_filters-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 08:11:20.594699 ar_filters-0.0.7/ar_filters/
--rw-rw-rw-   0        0        0        0 2023-06-15 16:56:34.000000 ar_filters-0.0.7/ar_filters/_init_.py
--rw-rw-rw-   0        0        0    20570 2023-06-16 08:09:55.000000 ar_filters-0.0.7/ar_filters/apply_filter.py
--rw-rw-rw-   0        0        0      111 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/create_points_labels.py
--rw-rw-rw-   0        0        0     4784 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/faceBlendCommon.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:11:21.079236 ar_filters-0.0.7/ar_filters/filters/
--rw-rw-rw-   0        0        0   142060 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/Mask.png
--rw-rw-rw-   0        0        0       56 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/Mask1.csv
--rw-rw-rw-   0        0        0       24 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/Mask_annotations.csv
--rw-rw-rw-   0        0        0   111740 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/Squid-Game-Front-Man-Mask.png
--rw-rw-rw-   0        0        0   437010 2023-06-04 10:57:04.000000 ar_filters-0.0.7/ar_filters/filters/Squid-Game-Front-Man-Mask2.png
--rw-rw-rw-   0        0        0     3721 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/Squid-Game-Front-Man-Mask_annotations.csv
--rw-rw-rw-   0        0        0   376499 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/Squid-Game-Guard-Mask.png
--rw-rw-rw-   0        0        0     3421 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/Squid-Game-Guard-Mask_annotations.csv
--rw-rw-rw-   0        0        0    33884 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/anime.png
--rw-rw-rw-   0        0        0     2153 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/anime_annotations.csv
--rw-rw-rw-   0        0        0   373231 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/anonymous.png
--rw-rw-rw-   0        0        0     2519 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/anonymous_annotations.csv
--rw-rw-rw-   0        0        0    27023 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/cat-ears.png
--rw-rw-rw-   0        0        0       21 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/cat-ears_annotations.csv
--rw-rw-rw-   0        0        0    34195 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/cat-nose.png
--rw-rw-rw-   0        0        0       21 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/cat-nose_annotations.csv
--rw-rw-rw-   0        0        0    42558 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/dog-ears.png
--rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/dog-ears_annotations.csv
--rw-rw-rw-   0        0        0    28892 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/dog-nose.png
--rw-rw-rw-   0        0        0       20 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/dog-nose_annotations - Copy.csv
--rw-rw-rw-   0        0        0       20 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/dog-nose_annotations.csv
--rw-rw-rw-   0        0        0       19 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/dog-tongue_annotations.csv
--rw-rw-rw-   0        0        0   141331 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/flower-crown.png
--rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/flower-crown_annotations.csv
--rw-rw-rw-   0        0        0   327097 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/glasses.png
--rw-rw-rw-   0        0        0    88167 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/gold-crown.png
--rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/gold-crown_annotations.csv
--rw-rw-rw-   0        0        0      818 2022-05-11 21:23:23.000000 ar_filters-0.0.7/ar_filters/filters/green-carnival.csv
--rw-rw-rw-   0        0        0   237110 2022-05-11 21:23:23.000000 ar_filters-0.0.7/ar_filters/filters/green-carnival.png
--rw-rw-rw-   0        0        0      832 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/green-carnival_annotations.csv
--rw-rw-rw-   0        0        0     2604 2022-05-11 21:23:23.000000 ar_filters-0.0.7/ar_filters/filters/jason-joker.csv
--rw-rw-rw-   0        0        0   413158 2022-05-11 21:23:23.000000 ar_filters-0.0.7/ar_filters/filters/jason-joker.png
--rw-rw-rw-   0        0        0     2671 2023-06-04 11:02:05.000000 ar_filters-0.0.7/ar_filters/filters/jason-joker_annotations.csv
--rw-rw-rw-   0        0        0    28916 2023-06-04 09:58:00.000000 ar_filters-0.0.7/ar_filters/filters/mustache.png
--rw-rw-rw-   0        0        0     7431 2023-06-16 07:22:22.000000 ar_filters-0.0.7/ar_filters/main2.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:11:20.690442 ar_filters-0.0.7/ar_filters.egg-info/
--rw-rw-rw-   0        0        0     9425 2023-06-16 08:11:18.000000 ar_filters-0.0.7/ar_filters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1718 2023-06-16 08:11:19.000000 ar_filters-0.0.7/ar_filters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 08:11:18.000000 ar_filters-0.0.7/ar_filters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 08:11:18.000000 ar_filters-0.0.7/ar_filters.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 08:11:18.000000 ar_filters-0.0.7/ar_filters.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 08:11:21.093558 ar_filters-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1366 2023-06-16 08:10:00.000000 ar_filters-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 05:05:25.571557 ar_filters-0.0.8/
+-rw-rw-rw-   0        0        0     1093 2023-06-10 13:07:48.000000 ar_filters-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-16 06:53:45.000000 ar_filters-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      455 2023-07-08 05:05:25.569562 ar_filters-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-07-08 05:04:36.000000 ar_filters-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 05:05:24.697889 ar_filters-0.0.8/ar_filters/
+-rw-rw-rw-   0        0        0        0 2023-06-15 16:56:34.000000 ar_filters-0.0.8/ar_filters/_init_.py
+-rw-rw-rw-   0        0        0    20570 2023-06-16 08:09:55.000000 ar_filters-0.0.8/ar_filters/apply_filter.py
+-rw-rw-rw-   0        0        0      111 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/create_points_labels.py
+-rw-rw-rw-   0        0        0     4784 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/faceBlendCommon.py
+drwxrwxrwx   0        0        0        0 2023-07-08 05:05:25.566570 ar_filters-0.0.8/ar_filters/filters/
+-rw-rw-rw-   0        0        0   142060 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/Mask.png
+-rw-rw-rw-   0        0        0       56 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/Mask1.csv
+-rw-rw-rw-   0        0        0       24 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/Mask_annotations.csv
+-rw-rw-rw-   0        0        0   111740 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/Squid-Game-Front-Man-Mask.png
+-rw-rw-rw-   0        0        0   437010 2023-06-04 10:57:04.000000 ar_filters-0.0.8/ar_filters/filters/Squid-Game-Front-Man-Mask2.png
+-rw-rw-rw-   0        0        0     3721 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/Squid-Game-Front-Man-Mask_annotations.csv
+-rw-rw-rw-   0        0        0   376499 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/Squid-Game-Guard-Mask.png
+-rw-rw-rw-   0        0        0     3421 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/Squid-Game-Guard-Mask_annotations.csv
+-rw-rw-rw-   0        0        0    33884 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/anime.png
+-rw-rw-rw-   0        0        0     2153 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/anime_annotations.csv
+-rw-rw-rw-   0        0        0   373231 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/anonymous.png
+-rw-rw-rw-   0        0        0     2519 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/anonymous_annotations.csv
+-rw-rw-rw-   0        0        0    27023 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/cat-ears.png
+-rw-rw-rw-   0        0        0       21 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/cat-ears_annotations.csv
+-rw-rw-rw-   0        0        0    34195 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/cat-nose.png
+-rw-rw-rw-   0        0        0       21 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/cat-nose_annotations.csv
+-rw-rw-rw-   0        0        0    42558 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/dog-ears.png
+-rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/dog-ears_annotations.csv
+-rw-rw-rw-   0        0        0    28892 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/dog-nose.png
+-rw-rw-rw-   0        0        0       20 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/dog-nose_annotations - Copy.csv
+-rw-rw-rw-   0        0        0       20 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/dog-nose_annotations.csv
+-rw-rw-rw-   0        0        0       19 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/dog-tongue_annotations.csv
+-rw-rw-rw-   0        0        0   141331 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/flower-crown.png
+-rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/flower-crown_annotations.csv
+-rw-rw-rw-   0        0        0   327097 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/glasses.png
+-rw-rw-rw-   0        0        0    88167 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/gold-crown.png
+-rw-rw-rw-   0        0        0       22 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/gold-crown_annotations.csv
+-rw-rw-rw-   0        0        0      818 2022-05-11 21:23:23.000000 ar_filters-0.0.8/ar_filters/filters/green-carnival.csv
+-rw-rw-rw-   0        0        0   237110 2022-05-11 21:23:23.000000 ar_filters-0.0.8/ar_filters/filters/green-carnival.png
+-rw-rw-rw-   0        0        0      832 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/green-carnival_annotations.csv
+-rw-rw-rw-   0        0        0     2604 2022-05-11 21:23:23.000000 ar_filters-0.0.8/ar_filters/filters/jason-joker.csv
+-rw-rw-rw-   0        0        0   413158 2022-05-11 21:23:23.000000 ar_filters-0.0.8/ar_filters/filters/jason-joker.png
+-rw-rw-rw-   0        0        0     2671 2023-06-04 11:02:05.000000 ar_filters-0.0.8/ar_filters/filters/jason-joker_annotations.csv
+-rw-rw-rw-   0        0        0    28916 2023-06-04 09:58:00.000000 ar_filters-0.0.8/ar_filters/filters/mustache.png
+-rw-rw-rw-   0        0        0     7431 2023-06-16 07:22:22.000000 ar_filters-0.0.8/ar_filters/main2.py
+drwxrwxrwx   0        0        0        0 2023-07-08 05:05:24.760722 ar_filters-0.0.8/ar_filters.egg-info/
+-rw-rw-rw-   0        0        0      455 2023-07-08 05:05:23.000000 ar_filters-0.0.8/ar_filters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1718 2023-07-08 05:05:24.000000 ar_filters-0.0.8/ar_filters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 05:05:23.000000 ar_filters-0.0.8/ar_filters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 05:05:23.000000 ar_filters-0.0.8/ar_filters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-08 05:05:23.000000 ar_filters-0.0.8/ar_filters.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 05:05:25.571557 ar_filters-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2023-07-08 05:02:37.000000 ar_filters-0.0.8/setup.py
```

### Comparing `ar_filters-0.0.7/LICENSE` & `ar_filters-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/apply_filter.py` & `ar_filters-0.0.8/ar_filters/apply_filter.py`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/faceBlendCommon.py` & `ar_filters-0.0.8/ar_filters/faceBlendCommon.py`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/Mask.png` & `ar_filters-0.0.8/ar_filters/filters/Mask.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/Squid-Game-Front-Man-Mask.png` & `ar_filters-0.0.8/ar_filters/filters/Squid-Game-Front-Man-Mask.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/Squid-Game-Front-Man-Mask2.png` & `ar_filters-0.0.8/ar_filters/filters/Squid-Game-Front-Man-Mask2.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/Squid-Game-Front-Man-Mask_annotations.csv` & `ar_filters-0.0.8/ar_filters/filters/Squid-Game-Front-Man-Mask_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/Squid-Game-Guard-Mask.png` & `ar_filters-0.0.8/ar_filters/filters/Squid-Game-Guard-Mask.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/Squid-Game-Guard-Mask_annotations.csv` & `ar_filters-0.0.8/ar_filters/filters/Squid-Game-Guard-Mask_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/anime.png` & `ar_filters-0.0.8/ar_filters/filters/anime.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/anime_annotations.csv` & `ar_filters-0.0.8/ar_filters/filters/anime_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/anonymous.png` & `ar_filters-0.0.8/ar_filters/filters/anonymous.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/anonymous_annotations.csv` & `ar_filters-0.0.8/ar_filters/filters/anonymous_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/cat-ears.png` & `ar_filters-0.0.8/ar_filters/filters/cat-ears.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/cat-nose.png` & `ar_filters-0.0.8/ar_filters/filters/cat-nose.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/dog-ears.png` & `ar_filters-0.0.8/ar_filters/filters/dog-ears.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/dog-nose.png` & `ar_filters-0.0.8/ar_filters/filters/dog-nose.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/flower-crown.png` & `ar_filters-0.0.8/ar_filters/filters/flower-crown.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/glasses.png` & `ar_filters-0.0.8/ar_filters/filters/glasses.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/gold-crown.png` & `ar_filters-0.0.8/ar_filters/filters/gold-crown.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/green-carnival.csv` & `ar_filters-0.0.8/ar_filters/filters/green-carnival.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/green-carnival.png` & `ar_filters-0.0.8/ar_filters/filters/green-carnival.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/green-carnival_annotations.csv` & `ar_filters-0.0.8/ar_filters/filters/green-carnival_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/jason-joker.csv` & `ar_filters-0.0.8/ar_filters/filters/jason-joker.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/jason-joker.png` & `ar_filters-0.0.8/ar_filters/filters/jason-joker.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/jason-joker_annotations.csv` & `ar_filters-0.0.8/ar_filters/filters/jason-joker_annotations.csv`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/filters/mustache.png` & `ar_filters-0.0.8/ar_filters/filters/mustache.png`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters/main2.py` & `ar_filters-0.0.8/ar_filters/main2.py`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/ar_filters.egg-info/SOURCES.txt` & `ar_filters-0.0.8/ar_filters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ar_filters-0.0.7/setup.py` & `ar_filters-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools #导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ar_filters", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.7",    #包版本号，便于维护版本
+    version="0.0.8",    #包版本号，便于维护版本
     author="Eric",    #作者，可以写自己的姓名
     author_email="koke8756@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small example package",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/EricLee2021-72324/handpose_x",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_namespace_packages(include=["ar_filters", "ar_filters.*","filters"], ),
```

