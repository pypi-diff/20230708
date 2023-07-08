# Comparing `tmp/cvmblaster-0.4.0.tar.gz` & `tmp/cvmblaster-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvmblaster-0.4.0.tar", last modified: Sun Jun 25 06:28:42 2023, max compression
+gzip compressed data, was "cvmblaster-0.4.1.tar", last modified: Sat Jul  8 11:37:51 2023, max compression
```

## Comparing `cvmblaster-0.4.0.tar` & `cvmblaster-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:28:42.286386 cvmblaster-0.4.0/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-25 06:14:42.000000 cvmblaster-0.4.0/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      904 2023-06-25 06:28:42.286270 cvmblaster-0.4.0/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      152 2022-06-30 20:46:05.000000 cvmblaster-0.4.0/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:28:42.284788 cvmblaster-0.4.0/cvmblaster/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:14:42.000000 cvmblaster-0.4.0/cvmblaster/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      291 2023-06-25 06:15:08.000000 cvmblaster-0.4.0/cvmblaster/__init__.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:28:42.286020 cvmblaster-0.4.0/cvmblaster/__pycache__/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      263 2022-06-20 07:36:18.000000 cvmblaster-0.4.0/cvmblaster/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5071 2022-06-20 07:36:18.000000 cvmblaster-0.4.0/cvmblaster/__pycache__/blaster.cpython-39.pyc
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    14612 2023-06-25 06:14:50.000000 cvmblaster-0.4.0/cvmblaster/blaster.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:28:42.285541 cvmblaster-0.4.0/cvmblaster.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      904 2023-06-25 06:28:42.000000 cvmblaster-0.4.0/cvmblaster.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      373 2023-06-25 06:28:42.000000 cvmblaster-0.4.0/cvmblaster.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-25 06:28:42.000000 cvmblaster-0.4.0/cvmblaster.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       22 2023-06-25 06:28:42.000000 cvmblaster-0.4.0/cvmblaster.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       11 2023-06-25 06:28:42.000000 cvmblaster-0.4.0/cvmblaster.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2022-04-25 09:43:02.000000 cvmblaster-0.4.0/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-25 06:28:42.286425 cvmblaster-0.4.0/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2139 2022-09-05 06:58:01.000000 cvmblaster-0.4.0/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-08 11:37:51.616987 cvmblaster-0.4.1/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-07-08 11:21:40.000000 cvmblaster-0.4.1/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      904 2023-07-08 11:37:51.616873 cvmblaster-0.4.1/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      152 2022-06-30 20:46:05.000000 cvmblaster-0.4.1/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-08 11:37:51.615125 cvmblaster-0.4.1/cvmblaster/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-07-08 11:21:40.000000 cvmblaster-0.4.1/cvmblaster/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      291 2023-07-08 11:35:42.000000 cvmblaster-0.4.1/cvmblaster/__init__.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-08 11:37:51.616546 cvmblaster-0.4.1/cvmblaster/__pycache__/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      263 2022-06-20 07:36:18.000000 cvmblaster-0.4.1/cvmblaster/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5071 2022-06-20 07:36:18.000000 cvmblaster-0.4.1/cvmblaster/__pycache__/blaster.cpython-39.pyc
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    14653 2023-07-08 11:35:28.000000 cvmblaster-0.4.1/cvmblaster/blaster.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-07-08 11:37:51.615910 cvmblaster-0.4.1/cvmblaster.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      904 2023-07-08 11:37:51.000000 cvmblaster-0.4.1/cvmblaster.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      373 2023-07-08 11:37:51.000000 cvmblaster-0.4.1/cvmblaster.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-07-08 11:37:51.000000 cvmblaster-0.4.1/cvmblaster.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       22 2023-07-08 11:37:51.000000 cvmblaster-0.4.1/cvmblaster.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       11 2023-07-08 11:37:51.000000 cvmblaster-0.4.1/cvmblaster.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2022-04-25 09:43:02.000000 cvmblaster-0.4.1/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-07-08 11:37:51.617046 cvmblaster-0.4.1/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2139 2022-09-05 06:58:01.000000 cvmblaster-0.4.1/setup.py
```

### Comparing `cvmblaster-0.4.0/.DS_Store` & `cvmblaster-0.4.1/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -275,16 +275,16 @@
 00001120: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
 00001130: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
 00001140: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
 00001150: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 00001160: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 00001170: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
 00001180: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
-00001190: 7b37 3335 2c20 3436 327d 2c20 7b39 3230  {735, 462}, {920
-000011a0: 2c20 3433 367d 7d09 0815 232f 3b52 5f6b  , 436}}...#/;R_k
+00001190: 7b36 3433 2c20 3235 317d 2c20 7b39 3230  {643, 251}, {920
+000011a0: 2c20 3436 347d 7d09 0815 232f 3b52 5f6b  , 464}}...#/;R_k
 000011b0: 6c6d 6e6f 8a00 0000 0000 0001 0100 0000  lmno............
 000011c0: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
 000011d0: 0000 0000 8b00 0000 0a00 6300 7600 6d00  ..........c.v.m.
 000011e0: 6200 6c00 6100 7300 7400 6500 726c 6731  b.l.a.s.t.e.rlg1
 000011f0: 5363 6f6d 7000 0000 0000 0000 0000 0000  Scomp...........
 00001200: 0a00 6300 7600 6d00 6200 6c00 6100 7300  ..c.v.m.b.l.a.s.
 00001210: 7400 6500 726c 7376 4362 6c6f 6200 0002  t.e.rlsvCblob...
```

### Comparing `cvmblaster-0.4.0/PKG-INFO` & `cvmblaster-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvmblaster
-Version: 0.4.0
+Version: 0.4.1
 Summary: find antimcirobial resistance genes
 Home-page: https://github.com/hbucqp/cvmblaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,resfinder
 Platform: any
```

### Comparing `cvmblaster-0.4.0/cvmblaster/.DS_Store` & `cvmblaster-0.4.1/cvmblaster/.DS_Store`

 * *Files identical despite different names*

### Comparing `cvmblaster-0.4.0/cvmblaster/__pycache__/blaster.cpython-39.pyc` & `cvmblaster-0.4.1/cvmblaster/__pycache__/blaster.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cvmblaster-0.4.0/cvmblaster/blaster.py` & `cvmblaster-0.4.1/cvmblaster/blaster.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,20 +49,21 @@
             for alignment in blast_record.alignments:
                 for hsp in alignment.hsps:
                     strand = 0
 
                     query_name = blast_record.query
                     # print(query_name)
                     # print(alignment.title)
-                    target_gene = alignment.title.split(' ')[1]
+                    target_gene = alignment.title.partition(' ')[2]
 
                     # Get gene name and accession number from target_gene
                     gene = target_gene.split('___')[0]
                     accession = target_gene.split('___')[2]
                     classes = target_gene.split('___')[3]  # 增加种类
+                    # print(classes)
                     # print(target_gene)
                     sbjct_length = alignment.length  # The length of matched gene
                     # print(sbjct_length)
                     sbjct_start = hsp.sbjct_start
                     sbjct_end = hsp.sbjct_end
                     gaps = hsp.gaps  # gaps of alignment
                     query_string = str(hsp.query)  # Get the query string
```

### Comparing `cvmblaster-0.4.0/cvmblaster.egg-info/PKG-INFO` & `cvmblaster-0.4.1/cvmblaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvmblaster
-Version: 0.4.0
+Version: 0.4.1
 Summary: find antimcirobial resistance genes
 Home-page: https://github.com/hbucqp/cvmblaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,resfinder
 Platform: any
```

### Comparing `cvmblaster-0.4.0/setup.py` & `cvmblaster-0.4.1/setup.py`

 * *Files identical despite different names*

