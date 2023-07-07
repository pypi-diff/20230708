# Comparing `tmp/seismic-rna-0.1.2.tar.gz` & `tmp/seismic-rna-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic-rna-0.1.2.tar", last modified: Fri Jul  7 00:57:40 2023, max compression
+gzip compressed data, was "seismic-rna-0.1.3.tar", last modified: Fri Jul  7 23:32:23 2023, max compression
```

## Comparing `seismic-rna-0.1.2.tar` & `seismic-rna-0.1.3.tar`

### file list

```diff
@@ -1,116 +1,114 @@
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.517778 seismic-rna-0.1.2/
--rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.1.2/LICENSE
--rw-r--r--   0 mfa        (503) staff       (20)     1831 2023-07-07 00:57:40.517277 seismic-rna-0.1.2/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     1268 2023-07-06 00:54:05.000000 seismic-rna-0.1.2/README.md
--rw-r--r--   0 mfa        (503) staff       (20)      997 2023-07-07 00:56:15.000000 seismic-rna-0.1.2/pyproject.toml
--rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-07 00:57:40.517926 seismic-rna-0.1.2/setup.cfg
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.416199 seismic-rna-0.1.2/src/
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.427486 seismic-rna-0.1.2/src/seismic_rna.egg-info/
--rw-r--r--   0 mfa        (503) staff       (20)     1831 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     3013 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/SOURCES.txt
--rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/dependency_links.txt
--rw-r--r--   0 mfa        (503) staff       (20)       50 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/entry_points.txt
--rw-r--r--   0 mfa        (503) staff       (20)      153 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/requires.txt
--rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-07 00:57:40.000000 seismic-rna-0.1.2/src/seismic_rna.egg-info/top_level.txt
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.429591 seismic-rna-0.1.2/src/seismicrna/
--rw-r--r--   0 mfa        (503) staff       (20)      201 2023-06-29 18:12:04.000000 seismic-rna-0.1.2/src/seismicrna/__init__.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.434126 seismic-rna-0.1.2/src/seismicrna/align/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/align/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.1.2/src/seismicrna/align/fq2bam.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/align/fqutil.py
--rw-r--r--   0 mfa        (503) staff       (20)     7709 2023-06-29 21:22:27.000000 seismic-rna-0.1.2/src/seismicrna/align/main.py
--rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/align/strandedness.py
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/align/test.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.440368 seismic-rna-0.1.2/src/seismicrna/cluster/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     9128 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/compare.py
--rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/em.py
--rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/krun.py
--rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1874 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/main.py
--rw-r--r--   0 mfa        (503) staff       (20)      384 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/names.py
--rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/cluster/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.471892 seismic-rna-0.1.2/src/seismicrna/core/
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.1.2/src/seismicrna/core/bitcall.py
--rw-r--r--   0 mfa        (503) staff       (20)    18415 2023-07-07 00:40:09.000000 seismic-rna-0.1.2/src/seismicrna/core/bitvect.py
--rw-r--r--   0 mfa        (503) staff       (20)    24043 2023-07-06 23:44:48.000000 seismic-rna-0.1.2/src/seismicrna/core/cli.py
--rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.1.2/src/seismicrna/core/depend.py
--rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/docdef.py
--rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/docstring.py
--rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/dump.py
--rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/files.py
--rw-r--r--   0 mfa        (503) staff       (20)    14191 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/files_sanity.py
--rw-r--r--   0 mfa        (503) staff       (20)     7851 2023-06-29 19:57:01.000000 seismic-rna-0.1.2/src/seismicrna/core/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     2867 2023-06-29 17:37:52.000000 seismic-rna-0.1.2/src/seismicrna/core/logs.py
--rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/mu.py
--rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.1.2/src/seismicrna/core/mu_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-06-29 19:37:32.000000 seismic-rna-0.1.2/src/seismicrna/core/parallel.py
--rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.1.2/src/seismicrna/core/path.py
--rw-r--r--   0 mfa        (503) staff       (20)    29386 2023-06-29 17:35:09.000000 seismic-rna-0.1.2/src/seismicrna/core/rel.py
--rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.1.2/src/seismicrna/core/rel_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    29463 2023-06-29 19:57:29.000000 seismic-rna-0.1.2/src/seismicrna/core/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/rna.py
--rw-r--r--   0 mfa        (503) staff       (20)    26188 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/sect.py
--rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.1.2/src/seismicrna/core/sect_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.1.2/src/seismicrna/core/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.1.2/src/seismicrna/core/seq_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.1.2/src/seismicrna/core/shell.py
--rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.1.2/src/seismicrna/core/sim.py
--rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.1.2/src/seismicrna/core/sim_test.py
--rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/core/types.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.1.2/src/seismicrna/core/xam.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.475172 seismic-rna-0.1.2/src/seismicrna/demult/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/demult/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    42588 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/demult/demultiplex.py
--rw-r--r--   0 mfa        (503) staff       (20)     2073 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/demult/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.485826 seismic-rna-0.1.2/src/seismicrna/draw/
--rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.1.2/src/seismicrna/draw/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/draw/load_dataset.py
--rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/draw/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/draw/manipulator.py
--rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.1.2/src/seismicrna/draw/plotter.py
--rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/draw/study.py
--rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/draw/util.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.494134 seismic-rna-0.1.2/src/seismicrna/graph/
--rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     8667 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     3249 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/color.py
--rw-r--r--   0 mfa        (503) staff       (20)     2700 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/default.py
--rw-r--r--   0 mfa        (503) staff       (20)     7441 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/hist.py
--rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     8608 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/graph/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     9744 2023-06-30 04:08:02.000000 seismic-rna-0.1.2/src/seismicrna/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.498861 seismic-rna-0.1.2/src/seismicrna/mask/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/mask/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     4083 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/mask/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     4321 2023-07-06 23:44:35.000000 seismic-rna-0.1.2/src/seismicrna/mask/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/mask/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    14001 2023-07-06 23:57:39.000000 seismic-rna-0.1.2/src/seismicrna/mask/write.py
--rw-r--r--   0 mfa        (503) staff       (20)       47 2023-07-07 00:56:58.000000 seismic-rna-0.1.2/src/seismicrna/meta.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.507569 seismic-rna-0.1.2/src/seismicrna/relate/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/export.py
--rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     3175 2023-06-30 04:06:44.000000 seismic-rna-0.1.2/src/seismicrna/relate/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/relate.py
--rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.1.2/src/seismicrna/relate/sam.py
--rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/seqpos.py
--rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/relate/test.py
--rw-r--r--   0 mfa        (503) staff       (20)    15021 2023-06-30 04:03:22.000000 seismic-rna-0.1.2/src/seismicrna/relate/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.510081 seismic-rna-0.1.2/src/seismicrna/struct/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/struct/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     3905 2023-06-29 20:47:08.000000 seismic-rna-0.1.2/src/seismicrna/struct/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1862 2023-06-29 20:23:36.000000 seismic-rna-0.1.2/src/seismicrna/struct/rnastructure.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.514991 seismic-rna-0.1.2/src/seismicrna/table/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     7405 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     5929 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1520 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    14642 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/tabulate.py
--rw-r--r--   0 mfa        (503) staff       (20)     4841 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/table/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 00:57:40.516620 seismic-rna-0.1.2/src/seismicrna/test/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.2/src/seismicrna/test/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.1.2/src/seismicrna/test/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.157153 seismic-rna-0.1.3/
+-rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.1.3/LICENSE
+-rw-r--r--   0 mfa        (503) staff       (20)     1882 2023-07-07 23:32:23.156853 seismic-rna-0.1.3/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     1319 2023-07-07 17:58:57.000000 seismic-rna-0.1.3/README.md
+-rw-r--r--   0 mfa        (503) staff       (20)     1015 2023-07-07 19:47:31.000000 seismic-rna-0.1.3/pyproject.toml
+-rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-07 23:32:23.157233 seismic-rna-0.1.3/setup.cfg
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:01.684454 seismic-rna-0.1.3/src/
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:22.807356 seismic-rna-0.1.3/src/seismic_rna.egg-info/
+-rw-r--r--   0 mfa        (503) staff       (20)     1882 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     2954 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/SOURCES.txt
+-rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/dependency_links.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       50 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/entry_points.txt
+-rw-r--r--   0 mfa        (503) staff       (20)      164 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/requires.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-07 23:32:22.000000 seismic-rna-0.1.3/src/seismic_rna.egg-info/top_level.txt
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:01.699011 seismic-rna-0.1.3/src/seismicrna/
+-rw-r--r--   0 mfa        (503) staff       (20)      171 2023-07-07 22:10:20.000000 seismic-rna-0.1.3/src/seismicrna/__init__.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:01.735159 seismic-rna-0.1.3/src/seismicrna/align/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/align/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.1.3/src/seismicrna/align/fq2bam.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/align/fqutil.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7709 2023-06-29 21:22:27.000000 seismic-rna-0.1.3/src/seismicrna/align/main.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/align/strandedness.py
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/align/test.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:01.794325 seismic-rna-0.1.3/src/seismicrna/cluster/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9128 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/compare.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/em.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/krun.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1874 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)      384 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/names.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/cluster/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:22.866107 seismic-rna-0.1.3/src/seismicrna/core/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.1.3/src/seismicrna/core/bitcall.py
+-rw-r--r--   0 mfa        (503) staff       (20)    19264 2023-07-07 22:07:51.000000 seismic-rna-0.1.3/src/seismicrna/core/bitvect.py
+-rw-r--r--   0 mfa        (503) staff       (20)    23907 2023-07-07 02:41:42.000000 seismic-rna-0.1.3/src/seismicrna/core/cli.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.1.3/src/seismicrna/core/depend.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/docdef.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/docstring.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/dump.py
+-rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/files.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7933 2023-07-07 22:47:51.000000 seismic-rna-0.1.3/src/seismicrna/core/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2837 2023-07-07 02:37:13.000000 seismic-rna-0.1.3/src/seismicrna/core/logs.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/mu.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.1.3/src/seismicrna/core/mu_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-06-29 19:37:32.000000 seismic-rna-0.1.3/src/seismicrna/core/parallel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.1.3/src/seismicrna/core/path.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29386 2023-06-29 17:35:09.000000 seismic-rna-0.1.3/src/seismicrna/core/rel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.1.3/src/seismicrna/core/rel_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29608 2023-07-07 22:47:17.000000 seismic-rna-0.1.3/src/seismicrna/core/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/rna.py
+-rw-r--r--   0 mfa        (503) staff       (20)    26188 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/sect.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.1.3/src/seismicrna/core/sect_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.1.3/src/seismicrna/core/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.1.3/src/seismicrna/core/seq_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.1.3/src/seismicrna/core/shell.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.1.3/src/seismicrna/core/sim.py
+-rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.1.3/src/seismicrna/core/sim_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/core/types.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.1.3/src/seismicrna/core/xam.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:22.886709 seismic-rna-0.1.3/src/seismicrna/demult/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/demult/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    42588 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/demult/demultiplex.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2073 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/demult/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:22.938855 seismic-rna-0.1.3/src/seismicrna/draw/
+-rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.1.3/src/seismicrna/draw/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/draw/load_dataset.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/draw/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/draw/manipulator.py
+-rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.1.3/src/seismicrna/draw/plotter.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/draw/study.py
+-rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/draw/util.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:22.986300 seismic-rna-0.1.3/src/seismicrna/graph/
+-rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8667 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3249 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/color.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2700 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/default.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7441 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/hist.py
+-rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8608 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/graph/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9491 2023-07-07 17:48:44.000000 seismic-rna-0.1.3/src/seismicrna/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.013069 seismic-rna-0.1.3/src/seismicrna/mask/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/mask/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4068 2023-07-07 22:49:27.000000 seismic-rna-0.1.3/src/seismicrna/mask/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4321 2023-07-06 23:44:35.000000 seismic-rna-0.1.3/src/seismicrna/mask/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/mask/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14001 2023-07-06 23:57:39.000000 seismic-rna-0.1.3/src/seismicrna/mask/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.079074 seismic-rna-0.1.3/src/seismicrna/relate/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/export.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3175 2023-06-30 04:06:44.000000 seismic-rna-0.1.3/src/seismicrna/relate/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/relate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.1.3/src/seismicrna/relate/sam.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/seqpos.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/relate/test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15021 2023-06-30 04:03:22.000000 seismic-rna-0.1.3/src/seismicrna/relate/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.099741 seismic-rna-0.1.3/src/seismicrna/struct/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/struct/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3905 2023-06-29 20:47:08.000000 seismic-rna-0.1.3/src/seismicrna/struct/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1862 2023-06-29 20:23:36.000000 seismic-rna-0.1.3/src/seismicrna/struct/rnastructure.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.144297 seismic-rna-0.1.3/src/seismicrna/table/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7405 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     5929 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1520 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14642 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/tabulate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4841 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/table/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-07 23:32:23.156415 seismic-rna-0.1.3/src/seismicrna/test/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.1.3/src/seismicrna/test/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.1.3/src/seismicrna/test/main.py
```

### Comparing `seismic-rna-0.1.2/LICENSE` & `seismic-rna-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/PKG-INFO` & `seismic-rna-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.1.2
+Version: 0.1.3
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# SEISMIC RNA
+# SEISMIC-RNA
 
 RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and
 Clustering
 
 
 ## About
 
-SEISMIC RNA analyzes deep sequencing datasets from RNA mutational profiling
+SEISMIC-RNA analyzes deep sequencing datasets from RNA mutational profiling
 experiments, such as [DMS-MaPseq](https://www.nature.com/articles/nmeth.4057)
 and [SHAPE-MaP](https://www.nature.com/articles/nmeth.3029).
 This software introduces an optimized implementation of the original algorithm
 [DREEM](https://www.nature.com/articles/s41586-020-2253-5) for quantifying and
 clustering mutations to infer RNA structural ensembles.
 
 
@@ -38,15 +38,15 @@
 - [Yves Martin](https://github.com/yvesmartindestaillades)
 - [Scott Grote](https://github.com/heWhosShouldersBlockTheSun)
 - [Albéric de Lajarte](https://github.com/AlbericDeLajarte)
 
 
 ## Installation
 
-Write me.
+Instructions for installing SEISMIC-RNA are in `INSTALL.md`.
 
 
 ## Usage
 
 Write me.
```

### Comparing `seismic-rna-0.1.2/README.md` & `seismic-rna-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
-# SEISMIC RNA
+# SEISMIC-RNA
 
 RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and
 Clustering
 
 
 ## About
 
-SEISMIC RNA analyzes deep sequencing datasets from RNA mutational profiling
+SEISMIC-RNA analyzes deep sequencing datasets from RNA mutational profiling
 experiments, such as [DMS-MaPseq](https://www.nature.com/articles/nmeth.4057)
 and [SHAPE-MaP](https://www.nature.com/articles/nmeth.3029).
 This software introduces an optimized implementation of the original algorithm
 [DREEM](https://www.nature.com/articles/s41586-020-2253-5) for quantifying and
 clustering mutations to infer RNA structural ensembles.
 
 
@@ -24,15 +24,15 @@
 - [Yves Martin](https://github.com/yvesmartindestaillades)
 - [Scott Grote](https://github.com/heWhosShouldersBlockTheSun)
 - [Albéric de Lajarte](https://github.com/AlbericDeLajarte)
 
 
 ## Installation
 
-Write me.
+Instructions for installing SEISMIC-RNA are in `INSTALL.md`.
 
 
 ## Usage
 
 Write me.
```

### Comparing `seismic-rna-0.1.2/pyproject.toml` & `seismic-rna-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seismic-rna"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name="Matty Allan"},
     {name="Yves Martin"},
     {name="Scott Grote"},
     {name="Alberic de Lajarte"},
 ]
 description = "RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering"
@@ -16,14 +16,15 @@
 requires-python = ">=3.10"
 license = {text = "GPL-3.0-only"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+    "click>=8.1",
     "cutadapt>=4.4",
     "fastqsplitter>=1.2",
     "matplotlib>=3.6",
     "numpy>=1.23",
     "pandas>=1.5",
     "plotly>=5.11",
     "pyarrow>=10.0",
```

### Comparing `seismic-rna-0.1.2/src/seismic_rna.egg-info/PKG-INFO` & `seismic-rna-0.1.3/src/seismic_rna.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.1.2
+Version: 0.1.3
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# SEISMIC RNA
+# SEISMIC-RNA
 
 RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and
 Clustering
 
 
 ## About
 
-SEISMIC RNA analyzes deep sequencing datasets from RNA mutational profiling
+SEISMIC-RNA analyzes deep sequencing datasets from RNA mutational profiling
 experiments, such as [DMS-MaPseq](https://www.nature.com/articles/nmeth.4057)
 and [SHAPE-MaP](https://www.nature.com/articles/nmeth.3029).
 This software introduces an optimized implementation of the original algorithm
 [DREEM](https://www.nature.com/articles/s41586-020-2253-5) for quantifying and
 clustering mutations to infer RNA structural ensembles.
 
 
@@ -38,15 +38,15 @@
 - [Yves Martin](https://github.com/yvesmartindestaillades)
 - [Scott Grote](https://github.com/heWhosShouldersBlockTheSun)
 - [Albéric de Lajarte](https://github.com/AlbericDeLajarte)
 
 
 ## Installation
 
-Write me.
+Instructions for installing SEISMIC-RNA are in `INSTALL.md`.
 
 
 ## Usage
 
 Write me.
```

### Comparing `seismic-rna-0.1.2/src/seismic_rna.egg-info/SOURCES.txt` & `seismic-rna-0.1.3/src/seismic_rna.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 src/seismic_rna.egg-info/SOURCES.txt
 src/seismic_rna.egg-info/dependency_links.txt
 src/seismic_rna.egg-info/entry_points.txt
 src/seismic_rna.egg-info/requires.txt
 src/seismic_rna.egg-info/top_level.txt
 src/seismicrna/__init__.py
 src/seismicrna/main.py
-src/seismicrna/meta.py
 src/seismicrna/align/__init__.py
 src/seismicrna/align/fq2bam.py
 src/seismicrna/align/fqutil.py
 src/seismicrna/align/main.py
 src/seismicrna/align/strandedness.py
 src/seismicrna/align/test.py
 src/seismicrna/cluster/__init__.py
@@ -30,15 +29,14 @@
 src/seismicrna/core/bitvect.py
 src/seismicrna/core/cli.py
 src/seismicrna/core/depend.py
 src/seismicrna/core/docdef.py
 src/seismicrna/core/docstring.py
 src/seismicrna/core/dump.py
 src/seismicrna/core/files.py
-src/seismicrna/core/files_sanity.py
 src/seismicrna/core/load.py
 src/seismicrna/core/logs.py
 src/seismicrna/core/mu.py
 src/seismicrna/core/mu_test.py
 src/seismicrna/core/parallel.py
 src/seismicrna/core/path.py
 src/seismicrna/core/rel.py
```

### Comparing `seismic-rna-0.1.2/src/seismicrna/align/fq2bam.py` & `seismic-rna-0.1.3/src/seismicrna/align/fq2bam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/align/fqutil.py` & `seismic-rna-0.1.3/src/seismicrna/align/fqutil.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/align/main.py` & `seismic-rna-0.1.3/src/seismicrna/align/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/align/strandedness.py` & `seismic-rna-0.1.3/src/seismicrna/align/strandedness.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/cluster/compare.py` & `seismic-rna-0.1.3/src/seismicrna/cluster/compare.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/cluster/em.py` & `seismic-rna-0.1.3/src/seismicrna/cluster/em.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/cluster/krun.py` & `seismic-rna-0.1.3/src/seismicrna/cluster/krun.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/cluster/load.py` & `seismic-rna-0.1.3/src/seismicrna/cluster/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/cluster/main.py` & `seismic-rna-0.1.3/src/seismicrna/cluster/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/cluster/report.py` & `seismic-rna-0.1.3/src/seismicrna/cluster/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/cluster/write.py` & `seismic-rna-0.1.3/src/seismicrna/cluster/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/bitcall.py` & `seismic-rna-0.1.3/src/seismicrna/core/bitcall.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/bitvect.py` & `seismic-rna-0.1.3/src/seismicrna/core/bitvect.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections import Counter
 from functools import cached_property
+from itertools import chain
 from logging import getLogger
 from typing import Callable, Iterable
 
 import numpy as np
 import pandas as pd
 
 from .sect import Section
@@ -392,16 +393,33 @@
         return self._masked
 
     @property
     def nbatches(self):
         """ Number of batches given to the accumulator. """
         return self._nbatches
 
+    @property
+    @abstractmethod
+    def _accum_info(self):
+        """ Return the accumulated informative bits. """
+
+    def _get_accum_read_names(self):
+        """ Names of the reads accumulated so far. """
+        if isinstance(self._accum_info, pd.DataFrame):
+            # The read names are the index of the DataFrame.
+            return self._accum_info.index.to_list()
+        if self.nbatches > 0:
+            # At least one batch of reads has been given.
+            return list(chain.from_iterable(batch.index for batch
+                                            in self._accum_info))
+        # No reads have been given.
+        return list()
+
     def _drop_duplicate_reads(self, batch: BitBatch):
-        dups = batch.reads.intersection(self.reads)
+        dups = batch.reads.intersection(self._get_accum_read_names())
         if batch.drop_reads(dups):
             logger.warning(f"{self} got read(s) in {batch} with name(s) seen "
                            f"in a previous batch: {dups.to_list()}")
         return dups
 
 
 class BitMonolith(BitAccum, BitMatrix):
@@ -429,14 +447,18 @@
     def _count_info_affi(self, batch: BitBatch):
         # Add the informative and affirmative bits from this batch to
         # the totals among all batches.
         self._info.append(batch.info)
         self._affi.append(batch.affi)
 
     @property
+    def _accum_info(self):
+        return self._info
+
+    @property
     def info(self) -> pd.DataFrame:
         return self._info
 
     @property
     def affi(self) -> pd.DataFrame:
         return self._affi
 
@@ -469,14 +491,18 @@
         self._affi_per_pos += batch.n_affi_per_pos
         self._info_per_read.append(batch.n_info_per_read)
         self._affi_per_read.append(batch.n_affi_per_read)
         logger.debug(f"Added batch {len(self._info_per_read)} to {self}")
         logger.debug(f"Counts:\n{self._info_per_pos}\n{self._affi_per_pos}")
 
     @property
+    def _accum_info(self):
+        return self._info_per_read
+
+    @property
     def n_info_per_pos(self):
         return self._info_per_pos
 
     @cached_property
     def n_info_per_read(self):
         if self.nbatches == 0:
             # No batches were given.
```

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/cli.py` & `seismic-rna-0.1.3/src/seismicrna/core/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,19 +532,14 @@
                      "seismic-rna_%Y-%m-%d_%H-%M-%S.log")),
                  help="File in which to log all messages (except profiling)")
 opt_profile = Option(("--profile",),
                      type=Path(exists=False, dir_okay=False),
                      default="",
                      help="Profile code performance and log results to the given file")
 
-# Misc
-opt_version = Option(("--version",),
-                     is_flag=True,
-                     help="Show the version and exit.")
-
 
 def merge_params(*param_lists: list[Parameter]):
     """ Merge lists of Click parameters, dropping duplicates. """
     params = list()
     names = set()
     for param_list in param_lists:
         for param in param_list:
```

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/depend.py` & `seismic-rna-0.1.3/src/seismicrna/core/depend.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/docdef.py` & `seismic-rna-0.1.3/src/seismicrna/core/docdef.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/docstring.py` & `seismic-rna-0.1.3/src/seismicrna/core/docstring.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/dump.py` & `seismic-rna-0.1.3/src/seismicrna/core/dump.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/files.py` & `seismic-rna-0.1.3/src/seismicrna/core/files.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/load.py` & `seismic-rna-0.1.3/src/seismicrna/core/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,18 @@
             return NotImplemented
         return self._report == other._report
 
 
 class BatchLoader(DataLoader, ABC):
     """ Load a dataset that is split into batches. """
 
+    @property
+    def num_batches(self):
+        return self._report.num_batches
+
     def build_batch_path(self, batch: int):
         """ Path to the batch with the given number. """
         return self._report.build_batch_path(self.out_dir, batch,
                                              **self._report.path_fields())
 
     @classmethod
     @abstractmethod
```

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/logs.py` & `seismic-rna-0.1.3/src/seismicrna/core/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 Purpose
 -------
 Central manager of logging.
 """
 
 import logging
 
-
 MAX_VERBOSE = 2
 MAX_QUIET = 2
 FILE_MSG_FORMAT = "LOGMSG>\t%(asctime)s\t%(name)s\t%(levelname)s\n%(message)s\n"
 STREAM_MSG_FORMAT = "%(levelname)s\t%(message)s"
 
 
 def get_top_logger():
@@ -59,15 +58,15 @@
         return logging.WARNING
     if (verbose, quiet) == (0, 1):
         return logging.ERROR
     if (verbose, quiet) == (0, 2):
         return logging.CRITICAL
 
     get_top_logger().warning(f"Invalid options: verbose={verbose}, "
-                               f"quiet={quiet}. Setting both to 0")
+                             f"quiet={quiet}. Setting both to 0")
     return get_verbosity(0, 0)
 
 
 def config(verbose: int, quiet: int, log_file: str | None = None):
     """ Configure the main logger with handlers and verbosity. """
     # Set up logger.
     logger = get_top_logger()
@@ -79,8 +78,7 @@
     logger.addHandler(stream_handler)
     # Add file handler.
     if log_file is not None:
         file_handler = logging.FileHandler(log_file, "a")
         file_handler.setLevel(get_verbosity(verbose=MAX_VERBOSE))
         file_handler.setFormatter(logging.Formatter(FILE_MSG_FORMAT))
         logger.addHandler(file_handler)
-    # logger.info(WELCOME)
```

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/mu.py` & `seismic-rna-0.1.3/src/seismicrna/core/mu.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/mu_test.py` & `seismic-rna-0.1.3/src/seismicrna/core/mu_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/parallel.py` & `seismic-rna-0.1.3/src/seismicrna/core/parallel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/path.py` & `seismic-rna-0.1.3/src/seismicrna/core/path.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/rel.py` & `seismic-rna-0.1.3/src/seismicrna/core/rel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/rel_test.py` & `seismic-rna-0.1.3/src/seismicrna/core/rel_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/report.py` & `seismic-rna-0.1.3/src/seismicrna/core/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,14 +714,19 @@
             files = list(map(report.get_batch_path, missing))
             raise FileNotFoundError(f"Missing batches: {files}")
         if badsum:
             files = list(map(report.get_batch_path, badsum))
             raise ValueError(f"Invalid MD5 checksums: {files}")
         return report
 
+    @property
+    def num_batches(self):
+        """ Number of batches associated with the report. """
+        return self.get_field(NumBatchF)
+
     @classmethod
     @abstractmethod
     def get_batch_seg(cls):
         """ Type of the path segment of each batch file. """
         return path.Segment("", dict())
 
     @classmethod
```

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/rna.py` & `seismic-rna-0.1.3/src/seismicrna/core/rna.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/sect.py` & `seismic-rna-0.1.3/src/seismicrna/core/sect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/sect_test.py` & `seismic-rna-0.1.3/src/seismicrna/core/sect_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/seq.py` & `seismic-rna-0.1.3/src/seismicrna/core/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/seq_test.py` & `seismic-rna-0.1.3/src/seismicrna/core/seq_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/shell.py` & `seismic-rna-0.1.3/src/seismicrna/core/shell.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/sim.py` & `seismic-rna-0.1.3/src/seismicrna/core/sim.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/sim_test.py` & `seismic-rna-0.1.3/src/seismicrna/core/sim_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/types.py` & `seismic-rna-0.1.3/src/seismicrna/core/types.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/core/xam.py` & `seismic-rna-0.1.3/src/seismicrna/core/xam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/demult/demultiplex.py` & `seismic-rna-0.1.3/src/seismicrna/demult/demultiplex.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/demult/main.py` & `seismic-rna-0.1.3/src/seismicrna/demult/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/draw/main.py` & `seismic-rna-0.1.3/src/seismicrna/draw/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/draw/manipulator.py` & `seismic-rna-0.1.3/src/seismicrna/draw/manipulator.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/draw/plotter.py` & `seismic-rna-0.1.3/src/seismicrna/draw/plotter.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/draw/study.py` & `seismic-rna-0.1.3/src/seismicrna/draw/study.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/draw/util.py` & `seismic-rna-0.1.3/src/seismicrna/draw/util.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/graph/base.py` & `seismic-rna-0.1.3/src/seismicrna/graph/base.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/graph/color.py` & `seismic-rna-0.1.3/src/seismicrna/graph/color.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/graph/default.py` & `seismic-rna-0.1.3/src/seismicrna/graph/default.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/graph/hist.py` & `seismic-rna-0.1.3/src/seismicrna/graph/hist.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/graph/seq.py` & `seismic-rna-0.1.3/src/seismicrna/graph/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/main.py` & `seismic-rna-0.1.3/src/seismicrna/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 import cProfile
 import os
 
-from click import Context, command, group, pass_context
+from click import Context, command, group, pass_context, version_option
 
 from . import (demult as demultiplex_mod,
                align as align_mod,
                relate as relate_mod,
                mask as mask_mod,
                cluster as cluster_mod,
                table as table_mod,
                struct as fold_mod,
                graph as graph_mod,
                test as test_mod)
 from .core import docdef, logs
 from .core.cli import (merge_params, opt_demultiplex,
-                       opt_verbose, opt_quiet, opt_log, opt_profile,
-                       opt_version, opt_fold)
-from .meta import __version__
-
-misc_params = [
-    opt_version,
-]
+                       opt_verbose, opt_quiet, opt_log, opt_profile, opt_fold)
 
 all_params = merge_params([opt_demultiplex],
                           demultiplex_mod.params,
                           align_mod.params,
                           relate_mod.params,
                           mask_mod.params,
                           cluster_mod.params,
                           table_mod.params,
                           [opt_fold],
-                          fold_mod.params,
-                          misc_params)
+                          fold_mod.params)
 
 
 @command("all", params=all_params)
 def all_cli(*args, **kwargs):
     """ Run 'align', 'relate', 'mask', (optionally) 'cluster', 'table',
     (optionally) 'fold', and (optionally) 'graph', in that order. """
     return run(*args, **kwargs)
@@ -132,22 +125,16 @@
         min_em_iter: int,
         max_em_iter: int,
         em_thresh: float,
         # Tabulation
         table_cols: str,
         # Folding
         fold: bool,
-        dms_quantile: float,
-        # Misc
-        version: bool):
+        dms_quantile: float):
     """ Run entire pipeline. """
-    if version:
-        # Just print the version and exit.
-        print(__version__)
-        return
     # Demultiplexing
     if demult_on:
         for dms, dmi, dmm in demultiplex_mod.run(
                 fasta=fasta,
                 library=library,
                 out_dir=out_dir,
                 temp_dir=temp_dir,
@@ -295,16 +282,16 @@
     opt_quiet,
     opt_log,
     opt_profile,
 ]
 
 
 # Group for main commands
-@group(params=main_params,
-       context_settings={"show_default": True})
+@group(params=main_params, context_settings={"show_default": True})
+@version_option()
 @pass_context
 def main_cli(ctx: Context, verbose: int, quiet: int, log: str, profile: str,
              **kwargs):
     """ SEISMIC-RNA command line interface """
     # Configure logging.
     os.makedirs(os.path.dirname(log), exist_ok=True)
     logs.config(verbose, quiet, log_file=log)
```

### Comparing `seismic-rna-0.1.2/src/seismicrna/mask/load.py` & `seismic-rna-0.1.3/src/seismicrna/mask/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,20 +69,19 @@
     def iter_read_batches(self):
         """ Yield the read names that were kept in every batch. """
         for batch in self.iter_batches_personal():
             yield batch.values
 
     def get_read_names(self):
         """ Return an array naming all reads that were kept. """
-        try:
+        if self.num_batches > 0:
             # Concatenate all indexes, which have the read names.
             return np.hstack(self.iter_read_batches())
-        except ValueError:
-            # If there are no batches, return an empty array.
-            return np.array([], dtype=str)
+        # If there are no batches, return an empty array.
+        return np.array([], dtype=str)
 
     def process_batch(self, imported_batch: pd.DataFrame,
                       private_batch: pd.Series, *,
                       bit_caller: BitCaller | None = None,
                       merge: bool = False, invert: bool = False):
         if bit_caller is None:
             # If no BitCaller was given, then use the mask's bit caller.
```

### Comparing `seismic-rna-0.1.2/src/seismicrna/mask/main.py` & `seismic-rna-0.1.3/src/seismicrna/mask/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/mask/report.py` & `seismic-rna-0.1.3/src/seismicrna/mask/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/mask/write.py` & `seismic-rna-0.1.3/src/seismicrna/mask/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/relate/export.py` & `seismic-rna-0.1.3/src/seismicrna/relate/export.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/relate/load.py` & `seismic-rna-0.1.3/src/seismicrna/relate/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/relate/main.py` & `seismic-rna-0.1.3/src/seismicrna/relate/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/relate/relate.py` & `seismic-rna-0.1.3/src/seismicrna/relate/relate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/relate/report.py` & `seismic-rna-0.1.3/src/seismicrna/relate/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/relate/sam.py` & `seismic-rna-0.1.3/src/seismicrna/relate/sam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/relate/seqpos.py` & `seismic-rna-0.1.3/src/seismicrna/relate/seqpos.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/relate/test.py` & `seismic-rna-0.1.3/src/seismicrna/relate/test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/relate/write.py` & `seismic-rna-0.1.3/src/seismicrna/relate/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/struct/main.py` & `seismic-rna-0.1.3/src/seismicrna/struct/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/struct/rnastructure.py` & `seismic-rna-0.1.3/src/seismicrna/struct/rnastructure.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/table/base.py` & `seismic-rna-0.1.3/src/seismicrna/table/base.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/table/load.py` & `seismic-rna-0.1.3/src/seismicrna/table/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/table/main.py` & `seismic-rna-0.1.3/src/seismicrna/table/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/table/tabulate.py` & `seismic-rna-0.1.3/src/seismicrna/table/tabulate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/table/write.py` & `seismic-rna-0.1.3/src/seismicrna/table/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.1.2/src/seismicrna/test/main.py` & `seismic-rna-0.1.3/src/seismicrna/test/main.py`

 * *Files identical despite different names*

