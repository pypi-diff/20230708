# Comparing `tmp/clubcpg-0.2.5.tar.gz` & `tmp/clubcpg-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/com.docker.devenvironments.code/dist/tmp41ebi4fu/clubcpg-0.2.5.tar", last modified: Tue Apr  5 20:08:46 2022, max compression
+gzip compressed data, was "clubcpg-0.3.0a0.tar", max compression
```

## Comparing `clubcpg-0.2.5.tar` & `clubcpg-0.3.0a0.tar`

### file list

```diff
@@ -1,29 +1,22 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-04-05 20:08:46.000000 clubcpg-0.2.5/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2022-04-05 19:57:04.000000 clubcpg-0.2.5/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2329 2022-04-05 20:08:46.000000 clubcpg-0.2.5/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1626 2022-04-05 17:43:11.000000 clubcpg-0.2.5/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-04-05 20:08:46.000000 clubcpg-0.2.5/bin/
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     6067 2022-04-05 19:57:04.000000 clubcpg-0.2.5/bin/clubcpg-cluster
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     3940 2022-04-05 17:43:11.000000 clubcpg-0.2.5/bin/clubcpg-coverage
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     6455 2022-04-05 19:57:04.000000 clubcpg-0.2.5/bin/clubcpg-impute-cluster
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4926 2022-04-05 17:43:11.000000 clubcpg-0.2.5/bin/clubcpg-impute-coverage
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     2575 2022-04-05 17:43:11.000000 clubcpg-0.2.5/bin/clubcpg-impute-train
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-04-05 20:08:46.000000 clubcpg-0.2.5/clubcpg/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7320 2022-04-05 17:43:11.000000 clubcpg-0.2.5/clubcpg/CalculateBinCoverage.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24224 2022-04-05 17:43:11.000000 clubcpg-0.2.5/clubcpg/ClusterReads.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1701 2022-04-05 17:43:11.000000 clubcpg-0.2.5/clubcpg/ConnectToCpGNet.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7814 2022-04-05 17:43:11.000000 clubcpg-0.2.5/clubcpg/Imputation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1114 2022-04-05 17:43:11.000000 clubcpg-0.2.5/clubcpg/OutputComparisonResults.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13004 2022-04-05 17:43:11.000000 clubcpg-0.2.5/clubcpg/ParseBam.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      117 2022-04-05 19:57:04.000000 clubcpg-0.2.5/clubcpg/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-04-05 20:08:46.000000 clubcpg-0.2.5/clubcpg.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2329 2022-04-05 20:08:45.000000 clubcpg-0.2.5/clubcpg.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      533 2022-04-05 20:08:46.000000 clubcpg-0.2.5/clubcpg.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2022-04-05 20:08:45.000000 clubcpg-0.2.5/clubcpg.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      108 2022-04-05 20:08:45.000000 clubcpg-0.2.5/clubcpg.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       23 2022-04-05 20:08:46.000000 clubcpg-0.2.5/clubcpg.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2022-04-05 20:08:46.000000 clubcpg-0.2.5/clubcpg_prelim/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13745 2022-04-05 17:43:11.000000 clubcpg-0.2.5/clubcpg_prelim/PReLIM.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       78 2022-04-05 17:43:11.000000 clubcpg-0.2.5/clubcpg_prelim/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2022-04-05 20:08:46.000000 clubcpg-0.2.5/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1402 2022-04-05 19:57:04.000000 clubcpg-0.2.5/setup.py
+-rw-r--r--   0        0        0     1073 2023-07-07 22:26:42.543324 clubcpg-0.3.0a0/LICENSE
+-rw-r--r--   0        0        0     2402 2023-07-07 22:26:42.543324 clubcpg-0.3.0a0/README.md
+-rw-r--r--   0        0        0     7320 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/CalculateBinCoverage.py
+-rw-r--r--   0        0        0    24592 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/ClusterReads.py
+-rw-r--r--   0        0        0     1888 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/ConnectToCpGNet.py
+-rw-r--r--   0        0        0     7816 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/Imputation.py
+-rw-r--r--   0        0        0     1114 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/OutputComparisonResults.py
+-rw-r--r--   0        0        0    13004 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/ParseBam.py
+-rw-r--r--   0        0        0      117 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/tests/__init__.py
+-rw-r--r--   0        0        0     7045 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg/tests/test_Module.py
+-rw-r--r--   0        0        0        0 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/__init__.py
+-rwxr-xr-x   0        0        0     6095 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/clubcpg_cluster.py
+-rwxr-xr-x   0        0        0     3963 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/clubcpg_coverage.py
+-rwxr-xr-x   0        0        0     6476 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_cluster.py
+-rwxr-xr-x   0        0        0     5111 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_coverage.py
+-rwxr-xr-x   0        0        0     2614 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_train.py
+-rw-r--r--   0        0        0    13821 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_prelim/PReLIM.py
+-rw-r--r--   0        0        0       78 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_prelim/__init__.py
+-rw-r--r--   0        0        0     2303 2023-07-07 22:26:42.551324 clubcpg-0.3.0a0/clubcpg_prelim/util/CpG_Bin.py
+-rw-r--r--   0        0        0     1518 2023-07-07 22:26:42.619326 clubcpg-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 clubcpg-0.3.0a0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `clubcpg-0.2.5/LICENSE` & `clubcpg-0.3.0a0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 C. Anthony Scott
+Copyright (c) 2023 C. Anthony Scott
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `clubcpg-0.2.5/PKG-INFO` & `clubcpg-0.3.0a0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,44 @@
-Metadata-Version: 2.1
-Name: clubcpg
-Version: 0.2.5
-Summary: CluBCpG is a software package built to analyze whole genome bisulfite sequencing (WGBS) data
-Home-page: https://github.com/waterlandlab/CluBCpG
-Author: C. Anthony Scott, PhD
-Author-email: charles.scott@bcm.edu
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: POSIX
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CluBCpG: Cluster-Based analysis of CpG methylation
 
-[![Build Status](https://travis-ci.com/waterlandlab/CluBCpG.svg?branch=master)](https://travis-ci.com/waterlandlab/CluBCpG)
 [![Documentation Status](https://readthedocs.org/projects/clubcpg/badge/?version=latest)](https://clubcpg.readthedocs.io/en/latest/?badge=latest)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/waterlandlab/CluBCpG.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/waterlandlab/CluBCpG/context:python)
 [![DOI](https://zenodo.org/badge/179135025.svg)](https://zenodo.org/badge/latestdoi/179135025)
 
+## Whats new?
+### v0.3.0
+* A major overhaul and modernization of the ClubCpG dependencies.
+* `setup.py` removed in favor of a `pyproject.toml`
+* All project dependencies updated to modern versions
+* Support of python 3.5, 3.6, 3.7, and 3.8 dropped
+* Minimum version of python is now 3.9
+* Added GitHub Actions workflows to automate testing of python 3.9 and 3.10
+* Updated readthedocs build configuration ahead of deprecation of old method
+
 
 ## What is CluBCpG?
 CluBCpG is a software package built to analyze whole genome bisulfite sequencing (WGBS) data. This toolkit will divide each chromosome into small user-defined intervals, extract all WGBS reads within those intervals, cluster them based on identity, and write a final report to the use containing all identified CpG methylation patterns.
 
 ## How do I use this?
 Full documentation is available on [ReadTheDocs](https://clubcpg.readthedocs.io/en/latest/index.html)
 
 ### Requirements
-* Python >= 3.5
+* Python >= 3.9, <3.11
 * Installation of Samtools on your PATH
 
 ### Install
 * __(Optional, but HIGHLY recommended)__ Create a new python virtual environment and activate that virualenv
 * Execute `pip install clubcpg` to install the package. Requirements will automatically be installed if not already present.
 
+### Developer Install
+* Ensure all dependencies in `ubuntu-preinsatll.sh` are installed on the system. (Or equivilant packages if using fedora based system)
+* Install samtools, use `install-samtools.sh`
+* Make sure you have a compatible version of python installed
+* Install Poetry `pip3 install poetry`
+* Run `poetry install` to install required packages and clubcpg
+* To install optional packages for docs building. Run `poetry install --with docs`
+
 ## Help! This isnt working.
 Open an [Issue](https://github.com/waterlandlab/CluBCpG/issues/new/choose)
 
 ## Can you make it do this?
 Open a [Feature Request](https://github.com/waterlandlab/CluBCpG/issues/new/choose)
-
-
```

### Comparing `clubcpg-0.2.5/bin/clubcpg-cluster` & `clubcpg-0.3.0a0/clubcpg_bin/clubcpg_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
                         help="Any additional info to include in the output file name, chromosome for example",
                         default=None)
 
 arg_parser.add_argument("--permute", help="Randomly shuffle the input file label on the reads prior to clustering. "
                                           "Has no effect if only analyzing one file",
                         default='False', type=str2bool, const=False, nargs="?")
 
-if __name__ == "__main__":
 
+def cli():
     args = arg_parser.parse_args()
 
     # Assign arg parser vars to new variables, not necessary, but I like it
     input_bam_a = args.input_bam_A
     input_bam_b = args.input_bam_B
     bins_file = args.bins
     bin_size = int(args.bin_size)
@@ -144,7 +144,12 @@
 
     logging.info(args)
 
     cluster_reads.execute()
 
 
     logging.info("Done")
+
+    
+if __name__ == "__main__":
+    cli()
+
```

### Comparing `clubcpg-0.2.5/bin/clubcpg-coverage` & `clubcpg-0.3.0a0/clubcpg_bin/clubcpg_coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 arg_parser.add_argument("--read1_3", help="integer, read1 3' m-bias ignore bp, default=0", default=0)
 arg_parser.add_argument("--read2_5", help="integer, read2 5' m-bias ignore bp, default=0", default=0)
 arg_parser.add_argument("--read2_3", help="integer, read2 3' m-bias ignore bp, default=0", default=0)
 arg_parser.add_argument("--no_overlap", help="bool, remove any overlap between paired reads and stitch"
                                              " reads together when possible, default=True",
                         type=str2bool, const=True, default='True', nargs='?')
 
-if __name__ == "__main__":
 
-    # Extract arguments from command line and set as correct types
+def cli():
+        # Extract arguments from command line and set as correct types
     args = arg_parser.parse_args()
 
     input_bam_file = args.input_bam_A
     num_of_processors = int(args.num_processors)
     bin_size = int(args.bin_size)
     no_overlap = args.no_overlap
 
@@ -93,8 +93,9 @@
                  "read1 3': {}bp\nread2 5: {}bp\nread2 3': {}bp".format(mbias_read1_5, mbias_read1_3, mbias_read2_5, mbias_read2_3))
 
     # Perform the analysis
     calc = CalculateCompleteBins(input_bam_file, bin_size, BASE_DIR, num_of_processors,
                                  mbias_read1_5, mbias_read1_3, mbias_read2_5, mbias_read2_3)
     output_file = calc.analyze_bins(chrom_of_interest)
 
-
+if __name__ == "__main__":
+    cli()
```

### Comparing `clubcpg-0.2.5/bin/clubcpg-impute-cluster` & `clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,17 +55,15 @@
                         default=None)
 arg_parser.add_argument("--models_A", help="Models to impute for input_bam_A, OPTIONAL", default=None)
 arg_parser.add_argument("--models_B", help="Models to impute for imput_bam_B, OPTIONAL", default=None)
 arg_parser.add_argument("--chunksize",
                         help="How large of chunks to split bins into during imputation. Higher will go faster, but uses more memory",
                         default=10000)
 
-if __name__ == "__main__":
-
-
+def cli():
     args = arg_parser.parse_args()
 
     # Assign arg parser vars to new variables, not necessary, but I like it
     input_bam_a = args.input_bam_A
     input_bam_b = args.input_bam_B
     bins_file = args.bins
     bin_size = int(args.bin_size)
@@ -155,7 +153,11 @@
 
     # Perform clustering
     cluster_reads.execute()
 
 
     logging.info("Done")
     print("Complete")
+
+if __name__ == "__main__":
+    cli()
+
```

### Comparing `clubcpg-0.2.5/bin/clubcpg-impute-coverage` & `clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_coverage.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,16 @@
                                       "Default=all chromosomes provided in -c. Example: 'chr7'",
                         default=None)
 arg_parser.add_argument("--read1_5", help="integer, read1 5' m-bias ignore bp, default=0", default=0)
 arg_parser.add_argument("--read1_3", help="integer, read1 3' m-bias ignore bp, default=0", default=0)
 arg_parser.add_argument("--read2_5", help="integer, read2 5' m-bias ignore bp, default=0", default=0)
 arg_parser.add_argument("--read2_3", help="integer, read2 3' m-bias ignore bp, default=0", default=0)
 
-if __name__ == "__main__":
+
+def cli():
     # Extract arguments from command line and set as correct types
     args = arg_parser.parse_args()
 
     # Set output dir
     if not args.output:
         output_folder = os.path.dirname(args.input_bam_file)
     else:
@@ -83,17 +84,20 @@
         # Get matrices with unknowns as -1
         print("Extracting cpg matrices from genome...", flush=True)
         bins, matrices = imputer.extract_matrices(coverage_data, return_bins=True)
 
         data_dict = create_dictionary(bins, matrices)
 
         print("Beginning imputation...", flush=True)
-        imputed_matrices = imputer.impute_from_model(models_folder=models, matrices=list(data_dict.values()), postprocess=True)
-
-        data_dict = create_dictionary(data_dict.keys(), imputed_matrices)
+        try:
+            imputed_matrices = imputer.impute_from_model(models_folder=models, matrices=list(data_dict.values()), postprocess=True)
+            data_dict = create_dictionary(data_dict.keys(), imputed_matrices)
+        except FileNotFoundError:
+            print(f"Could not find model file for {i} cpgs . Skipping...", flush=True)
+            continue
 
         for b, m in zip(data_dict.keys(), data_dict.values()):
             m2 = m[~np.isnan(m).any(axis=1)]
             line = "{},{},{}\n".format(b, m2.shape[0], m2.shape[1])
             tfile.write(line)
         
     ### Update Coverage File and Save New ###
@@ -116,7 +120,10 @@
     else:
         outfile = os.path.join(output_folder, os.path.basename(args.coverage) + ".IMPUTED.csv")
 
     print("Saving updated data to file...", flush=True)
     before.to_csv(outfile, header=False)
 
     print("done")
+
+if __name__ == "__main__":
+    cli()
```

### Comparing `clubcpg-0.2.5/bin/clubcpg-impute-train` & `clubcpg-0.3.0a0/clubcpg_bin/clubcpg_impute_train.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 arg_parser.add_argument("-l", "--limit_samples", help="Limit the number of samples used to train the model, "
                                                       "this will speed up training. default=10000", default=10000)
 arg_parser.add_argument("--read1_5", help="integer, read1 5' m-bias ignore bp, default=0", default=0)
 arg_parser.add_argument("--read1_3", help="integer, read1 3' m-bias ignore bp, default=0", default=0)
 arg_parser.add_argument("--read2_5", help="integer, read2 5' m-bias ignore bp, default=0", default=0)
 arg_parser.add_argument("--read2_3", help="integer, read2 3' m-bias ignore bp, default=0", default=0)
 
-if __name__ == "__main__":
 
+def cli():
     # Extract arguments from command line and set as correct types
     args = arg_parser.parse_args()
 
     # Get the mbias inputs and adjust to work correctly, 0s should be converted to None
     mbias_read1_5 = int(args.read1_5)
     mbias_read1_3 = int(args.read1_3)
     mbias_read2_5 = int(args.read2_5)
@@ -45,24 +45,17 @@
         print("Output folder already exists... no need to create it...")
 
     # Read in coverage file
     coverage_data = pd.read_csv(args.coverage, header=None)
     coverage_data.columns = ['bin', 'reads', 'cpgs']
 
     # Train models
-    for i in range(2,6):
+    for i in range(2,6):  #TODO TEMP CHANGE FOR TESTING
         print("Starting training cpg density: {}".format(i))
         trainer = Imputation(i, args.input_bam_file, mbias_read1_5, mbias_read1_3, mbias_read2_5, mbias_read2_3, processes)
         matrices = trainer.extract_matrices(coverage_data, sample_limit=sample_limit)
         model = trainer.train_model(output_folder, matrices)
 
     print("done")
 
-
-
-
-
-
-
-    
-
-
+if __name__ == "__main__":
+    cli()
```

### Comparing `clubcpg-0.2.5/clubcpg/CalculateBinCoverage.py` & `clubcpg-0.3.0a0/clubcpg/CalculateBinCoverage.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.2.5/clubcpg/ClusterReads.py` & `clubcpg-0.3.0a0/clubcpg/ClusterReads.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,18 +451,26 @@
                 print("Imputing chunk {}/{}...".format(j+1, n_chunks), flush=True)
                 imputed_matrices_A = imputer_A.impute_from_model(self.models_A, list(data_A_dict.values()))
                 if self.bam_b:
                     imputed_matrices_B = imputer_B.impute_from_model(self.models_B, data_B_dict.values())
                 else:
                     imputed_matrices_B = None
 
-                data_imputed_A_dict = self.create_dictionary(data_A_dict.keys(), imputed_matrices_A)
+                try:
+                    data_imputed_A_dict = self.create_dictionary(data_A_dict.keys(), imputed_matrices_A)
+                except FileNotFoundError:
+                    print(f"Could not find model file for {i} cpgs. Skipping.")
+                    continue
 
                 if self.bam_b:
-                    data_imputed_B_dict = self.create_dictionary(data_B_dict.keys(), imputed_matrices_B)
+                    try:
+                        data_imputed_B_dict = self.create_dictionary(data_B_dict.keys(), imputed_matrices_B)
+                    except FileNotFoundError:
+                        print(f"Could not find model file for {i} cpgs. Skipping.")
+                        continue
 
                 # Combine and cluster as normal
                 # Maybe do this in the future
                 # def _multiprocess_cluster_work(bin_):
                 #     pass
 
                 for bin_ in data_imputed_A_dict.keys():
```

### Comparing `clubcpg-0.2.5/clubcpg/ConnectToCpGNet.py` & `clubcpg-0.3.0a0/clubcpg/ConnectToCpGNet.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,11 +44,16 @@
         """
         Train the CpGNet model on a list of provided bins
 
         :param bins: iterable containing CpG matrices of 1 (methylated), 0 (unmethylated), and -1 (unknown)
         :return: Path to the saved model file
         """
         self.model.train(bins, model_file="no")
-        output = self.save_net(self.model.model)
+        
+        # Only save model if trained successfully. This prevents failures in cases which too little data
+        if self.model.model:
+            output = self.save_net(self.model.model)
+        else:
+            output = None
 
         return output
```

### Comparing `clubcpg-0.2.5/clubcpg/Imputation.py` & `clubcpg-0.3.0a0/clubcpg/Imputation.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,16 +91,15 @@
             except IndexError as e:
                 logging.info("Index error at bin {}".format(bin_))
                 logging.error(str(e))
                 continue
 
         # if len(clean_matrices) > 0:
         #     clean_matrices = np.array(clean_matrices)
-
-        clean_matrices = np.array(clean_matrices)
+        # clean_matrices = np.array(clean_matrices)
 
         if return_bins:
             return clean_bins, clean_matrices
         else:
             return clean_matrices
 
 
@@ -189,17 +188,18 @@
         Keyword Arguments:
             postprocess {bool} -- Round imputed values to 1s and 0s  (default: {True})
         """
 
         model_path = os.path.join(models_folder, "saved_model_{}_cpgs.prelim".format(self.cpg_density))
 
         trained_model = PReLIM(cpgDensity=self.cpg_density)
-        print("Successfully loaded model: {}".format(model_path), flush=True)
         trained_model.model = load(model_path)
 
+
+        print("Successfully loaded model: {}".format(model_path), flush=True)
         for m in matrices:
             # only impute if there is an unknown
             if -1 in m:
                 m = m.astype(float)
                 pm = trained_model.impute(m)
                 if postprocess:
                     pm = self.postprocess_predictions(pm)
```

### Comparing `clubcpg-0.2.5/clubcpg/OutputComparisonResults.py` & `clubcpg-0.3.0a0/clubcpg/OutputComparisonResults.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.2.5/clubcpg/ParseBam.py` & `clubcpg-0.3.0a0/clubcpg/ParseBam.py`

 * *Files identical despite different names*

### Comparing `clubcpg-0.2.5/clubcpg_prelim/PReLIM.py` & `clubcpg-0.3.0a0/clubcpg_prelim/PReLIM.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 		:param species: string, the speices this bin belongs too.
 		:param verbose: boolean, print warnings, set to "false" for no error checking and faster speed
 		:param tag1: anything, for custom use.
 		:param tag2: anything, for custom use.
 
 		"""
 
-
 		self.cpgDensity = matrix.shape[1]
 		self.readDepth = matrix.shape[0]
 		
 		
 
 		self.matrix = np.array(matrix, dtype=float)
 		self.binStartInc = binStartInc
@@ -141,16 +140,16 @@
 		Inputs: 
 		1. X_train,     numpy array, Contains feature vectors.
 		2. y_train,     numpy array, Contains labels for training data.
 		3. n_estimators, list, the number of estimators to try during a grid search.
 		4. max_depths, list, the maximum depths of trees to try during a grid search.
 		5. cores, the number of cores to use during training, helpful for grid search.
 		6. model_file, string,      The name of the file to save the model to. 
-			If None, then create a file name that includes a timestamp.
-			If you don't want to save a file, set this to "no"
+		If None, then create a file name that includes a timestamp.
+		If you don't want to save a file, set this to "no"
 	
 		5-fold validation is built into the grid search
 
 		Outputs: 
 		The trained model
 
 		Usage: 
@@ -163,28 +162,30 @@
 		  "max_depth": max_depths,
 		}
 
 		# Note: let the grid search use a lot of cores, but only use 1 for each forest
 		# since dispatching can take a lot of time
 		rf = RandomForestClassifier(n_jobs=1)
 		self.model = GridSearchCV(rf, grid_param, n_jobs=cores, cv=5, verbose=verbose)
-		self.model.fit(X_train, y_train)
-
+		if len(X_train) > 0:
+			self.model.fit(X_train, y_train)
 
-		# save the model
+			# save the model
+			if model_file == "no":
+				return self.model
 
-		if model_file == "no":
-			return self.model
-
-		if not model_file:
-			model_file = "PReLIM_model" + str(time.time())
+			if not model_file:
+				model_file = "PReLIM_model" + str(time.time())
 
-		p.dump(self.model, open(model_file,"wb"))
+			p.dump(self.model, open(model_file,"wb"))
 
-		return self.model
+			return self.model
+		else:
+			self.model = None
+			return self.model
 
 
 
 
 	# Feature collection directly from bins
 	def get_X_y(self, bin_matrices, model_file=None, verbose=False):
 		bins = []
```

