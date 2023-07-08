# Comparing `tmp/scutls-0.2.8.tar.gz` & `tmp/scutls-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.2.8.tar", max compression
+gzip compressed data, was "scutls-0.3.0.tar", max compression
```

## Comparing `scutls-0.2.8.tar` & `scutls-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      583 2023-06-29 04:36:28.104673 scutls-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-29 04:36:39.580824 scutls-0.2.8/scutls/__init__.py
--rw-r--r--   0        0        0     6777 2023-06-29 04:13:01.147316 scutls-0.2.8/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.2.8/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.2.8/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.2.8/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.2.8/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0     5820 2023-06-21 04:19:39.366335 scutls-0.2.8/scutls/barcode.py
--rw-r--r--   0        0        0     1144 2023-06-29 03:55:55.590164 scutls-0.2.8/scutls/cli.py
--rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.2.8/scutls/download.py
--rw-r--r--   0        0        0     4984 2023-06-29 04:31:23.564846 scutls-0.2.8/scutls/fastq.py
--rw-r--r--   0        0        0     9764 2023-06-29 04:30:12.222859 scutls-0.2.8/scutls/util.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 scutls-0.2.8/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 scutls-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      601 2023-07-08 04:36:59.598732 scutls-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-08 04:37:16.305738 scutls-0.3.0/scutls/__init__.py
+-rw-r--r--   0        0        0     7561 2023-07-08 04:25:06.015042 scutls-0.3.0/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.3.0/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.3.0/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.3.0/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.3.0/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     2269 2023-07-08 04:35:05.254780 scutls-0.3.0/scutls/bam.py
+-rw-r--r--   0        0        0     5820 2023-06-21 04:19:39.366335 scutls-0.3.0/scutls/barcode.py
+-rw-r--r--   0        0        0     1381 2023-07-08 04:30:45.312955 scutls-0.3.0/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.3.0/scutls/download.py
+-rw-r--r--   0        0        0     4984 2023-06-29 04:31:23.564846 scutls-0.3.0/scutls/fastq.py
+-rw-r--r--   0        0        0    14058 2023-07-08 03:33:01.924697 scutls-0.3.0/scutls/util.py
+-rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 scutls-0.3.0/setup.py
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 scutls-0.3.0/PKG-INFO
```

### Comparing `scutls-0.2.8/pyproject.toml` & `scutls-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "scutls"
-version = "0.2.8"
+version = "0.3.0"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
 bs4 = "^0.0.1"
 urllib3 = "^1.26.10"
 GEOparse = "^2.0.3"
 biopython = "^1.80"
 regex = "^2023.5.5"
+pysam = "^0.21.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `scutls-0.2.8/scutls/arguments.py` & `scutls-0.3.0/scutls/arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,41 @@
     "-fq", "--filter_q",
     help = "filter reads based on mean read quality cutoff (--filter_q). Default to 25. Reads failed to pass this filter will be saved into no_pass_xxx.fastq.gz where xxx represents the name specified with --output flag.",
     required = False, type = int, default = 25
 )
 ## set default values
 parser_fastq.set_defaults(func = cli.run_fastq)
 
+# sub-command: bam
+parser_bam = subparsers.add_parser(
+    "bam", description = "process bam files")
+parser_bam.add_argument(
+    "-i", "--input",
+    help = "input bam, must end with .bam",
+    required = True, type = str, default = None
+)
+parser_bam.add_argument(
+    "-o", "--output",
+    help = "output file name",
+    required = False, type = str, default = None
+)
+parser_bam.add_argument(
+    "-nproc", "--num_processor",
+    help = "number of parallel jobs",
+    required = False, type = int, default = 1
+)
+parser_bam.add_argument(
+    "-lpir", "--locate_pos_in_read",
+    help = "reference coordinate to be located in each read",
+    required = False, type = int, default = 1
+)
+## add mutually exclusive groups
+## set default values
+parser_bam.set_defaults(func = cli.run_bam)
+
 # sub-command: barcode
 parser_barcode = subparsers.add_parser(
     "barcode", description = "handle barcode file")
 parser_barcode.add_argument(
     "-i", "--input",
     help = "input fastq, can end with .gz",
     required = True, type = str, default = None)
@@ -136,16 +163,14 @@
     required = False, type = str, default = None
 )
 parser_barcode.add_argument(
     "-o2", "--output2",
     help = "output fastq name for non-hit reads, can end with .gz",
     required = False, type = str, default = None
 )
-
-
 ## add mutually exclusive groups
 parser_barcode_group = parser_barcode.add_mutually_exclusive_group()
 parser_barcode_group.add_argument(
     "-c", "--contain",
     help = "barcode string to search against the fastq, seperate by comma if multiple. e.g. 'AACCC,GTCCC,CAAA'",
     required = False, type = str, default = None
 )
```

### Comparing `scutls-0.2.8/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.3.0/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.8/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.3.0/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.2.8/scutls/assets/genome_ucsc.json` & `scutls-0.3.0/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.2.8/scutls/barcode.py` & `scutls-0.3.0/scutls/barcode.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.8/scutls/cli.py` & `scutls-0.3.0/scutls/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from scutls import download, fastq, barcode
+from scutls import download, fastq, barcode, bam
 
 # the default values are specified via the arguments.py file
+# should use full argument name for both left and right side
 
 def run_download(args):
     download.download(
     list_genome_ucsc = args.list_genome_ucsc,
     genome_ucsc = args.genome_ucsc,
     list_genome_ensembl = args.list_genome_ensembl,
     genome_ensembl = args.genome_ensembl,
@@ -21,14 +22,22 @@
     input  = args.input,
     output = args.output,
     unique = args.unique,
     join   = args.join,
     filter_q = args.filter_q
     )
 
+def run_bam(args):
+    bam.bam(
+    input  = args.input,
+    output = args.output,
+    locate_pos_in_read = args.locate_pos_in_read,
+    nproc = args.num_processor
+    )
+
 def run_barcode(args):
     barcode.barcode(
     input  = args.input,
     output = args.output,
     output2 = args.output2,
     contain = args.contain,
     locate = args.locate,
```

### Comparing `scutls-0.2.8/scutls/download.py` & `scutls-0.3.0/scutls/download.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.8/scutls/fastq.py` & `scutls-0.3.0/scutls/fastq.py`

 * *Files identical despite different names*

### Comparing `scutls-0.2.8/setup.py` & `scutls-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 {'': ['*'], 'scutls': ['assets/*']}
 
 install_requires = \
 ['GEOparse>=2.0.3,<3.0.0',
  'biopython>=1.80,<2.0',
  'bs4>=0.0.1,<0.0.2',
  'importlib-resources>=5.8.0,<6.0.0',
+ 'pysam>=0.21.0,<0.22.0',
  'regex>=2023.5.5,<2024.0.0',
  'urllib3>=1.26.10,<2.0.0',
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.2.8',
+    'version': '0.3.0',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.2.8/PKG-INFO` & `scutls-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.2.8
+Version: 0.3.0
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GEOparse (>=2.0.3,<3.0.0)
 Requires-Dist: biopython (>=1.80,<2.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: importlib-resources (>=5.8.0,<6.0.0)
+Requires-Dist: pysam (>=0.21.0,<0.22.0)
 Requires-Dist: regex (>=2023.5.5,<2024.0.0)
 Requires-Dist: urllib3 (>=1.26.10,<2.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
```

