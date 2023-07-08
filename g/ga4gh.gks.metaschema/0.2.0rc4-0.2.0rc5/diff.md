# Comparing `tmp/ga4gh.gks.metaschema-0.2.0rc4.tar.gz` & `tmp/ga4gh.gks.metaschema-0.2.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga4gh.gks.metaschema-0.2.0rc4.tar", last modified: Fri Oct  7 14:56:45 2022, max compression
+gzip compressed data, was "ga4gh.gks.metaschema-0.2.0rc5.tar", last modified: Sat Jul  8 04:53:00 2023, max compression
```

## Comparing `ga4gh.gks.metaschema-0.2.0rc4.tar` & `ga4gh.gks.metaschema-0.2.0rc5.tar`

### file list

```diff
@@ -1,38 +1,72 @@
-drwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        0 2022-10-07 14:56:45.348089 ga4gh.gks.metaschema-0.2.0rc4/
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)     1819 2021-11-07 01:52:00.000000 ga4gh.gks.metaschema-0.2.0rc4/.gitignore
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)    11357 2021-11-07 01:33:45.000000 ga4gh.gks.metaschema-0.2.0rc4/LICENSE
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)      636 2022-10-07 14:56:45.348384 ga4gh.gks.metaschema-0.2.0rc4/PKG-INFO
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)       77 2021-11-07 01:33:45.000000 ga4gh.gks.metaschema-0.2.0rc4/README.md
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)      131 2021-11-06 14:41:45.000000 ga4gh.gks.metaschema-0.2.0rc4/pyproject.toml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)      963 2022-10-07 14:56:45.349326 ga4gh.gks.metaschema-0.2.0rc4/setup.cfg
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)       38 2021-11-06 14:41:45.000000 ga4gh.gks.metaschema-0.2.0rc4/setup.py
-drwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        0 2022-10-07 14:56:45.336575 ga4gh.gks.metaschema-0.2.0rc4/src/
-drwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        0 2022-10-07 14:56:45.336685 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/
-drwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        0 2022-10-07 14:56:45.336830 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/
-drwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        0 2022-10-07 14:56:45.337336 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/metaschema/
-drwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        0 2022-10-07 14:56:45.342702 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/metaschema/scripts/
--rwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)      164 2021-11-06 14:41:45.000000 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/metaschema/scripts/jsy2js.py
--rwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)      226 2022-08-16 14:57:14.000000 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/metaschema/scripts/source2jsy.py
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)      245 2022-08-16 14:57:14.000000 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/metaschema/scripts/source2mergedjsy.py
--rwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)     4424 2022-08-16 14:57:14.000000 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/metaschema/scripts/y2t.py
-drwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        0 2022-10-07 14:56:45.343109 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/metaschema/tools/
--rwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)    17125 2022-10-07 14:48:33.000000 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/metaschema/tools/source_proc.py
-drwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        0 2022-10-07 14:56:45.341213 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh.gks.metaschema.egg-info/
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)      636 2022-10-07 14:56:45.000000 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh.gks.metaschema.egg-info/PKG-INFO
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)      797 2022-10-07 14:56:45.000000 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh.gks.metaschema.egg-info/SOURCES.txt
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        1 2022-10-07 14:56:45.000000 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh.gks.metaschema.egg-info/dependency_links.txt
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)       17 2022-10-07 14:56:45.000000 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh.gks.metaschema.egg-info/requires.txt
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        6 2022-10-07 14:56:45.000000 ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh.gks.metaschema.egg-info/top_level.txt
-drwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        0 2022-10-07 14:56:45.343754 ga4gh.gks.metaschema-0.2.0rc4/tests/
-drwxr-xr-x   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)        0 2022-10-07 14:56:45.347682 ga4gh.gks.metaschema-0.2.0rc4/tests/data/
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)     2549 2022-08-17 17:07:26.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/data/catvars-source.yaml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)     2755 2022-08-17 17:53:00.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/data/catvars.yaml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)     7280 2022-08-17 17:00:05.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/data/core-source.yaml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)     8628 2022-08-17 17:54:30.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/data/core.yaml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)     9725 2022-08-17 17:11:45.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/data/vod-source.yaml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)    16965 2022-08-17 17:53:00.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/data/vod.yaml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)    21036 2022-08-17 17:04:42.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/data/vrs-source.yaml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)    21446 2022-08-17 17:52:51.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/data/vrs.yaml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)    25339 2022-10-07 13:26:07.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/data/vrs1-source.yaml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)    22622 2022-10-07 14:48:37.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/data/vrs1.yaml
--rw-r--r--   0 ahw001   (1186363539) RESEARCH\Domain Users (1287271524)      796 2022-10-07 14:02:13.000000 ga4gh.gks.metaschema-0.2.0rc4/tests/test_basic.py
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.110248 ga4gh.gks.metaschema-0.2.0rc5/
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1819 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/.gitignore
+-rw-r--r--   0 ahw001   (1186363539) 1287271524    11357 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/LICENSE
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      636 2023-07-08 04:53:00.110351 ga4gh.gks.metaschema-0.2.0rc5/PKG-INFO
+-rw-r--r--   0 ahw001   (1186363539) 1287271524       77 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/README.md
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      131 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/pyproject.toml
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1023 2023-07-08 04:53:00.110833 ga4gh.gks.metaschema-0.2.0rc5/setup.cfg
+-rw-r--r--   0 ahw001   (1186363539) 1287271524       38 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/setup.py
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.090425 ga4gh.gks.metaschema-0.2.0rc5/src/
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.090652 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.090804 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.091065 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.095668 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/scripts/
+-rwxr-xr-x   0 ahw001   (1186363539) 1287271524      164 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/scripts/jsy2js.py
+-rwxr-xr-x   0 ahw001   (1186363539) 1287271524      226 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/scripts/source2jsy.py
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      245 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/scripts/source2mergedjsy.py
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      220 2023-04-17 15:03:13.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/scripts/source2splitjs.py
+-rwxr-xr-x   0 ahw001   (1186363539) 1287271524     4424 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/scripts/y2t.py
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.095898 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/tools/
+-rwxr-xr-x   0 ahw001   (1186363539) 1287271524    20357 2023-07-08 04:38:20.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/tools/source_proc.py
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.094374 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh.gks.metaschema.egg-info/
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      636 2023-07-08 04:52:59.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh.gks.metaschema.egg-info/PKG-INFO
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     2241 2023-07-08 04:53:00.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh.gks.metaschema.egg-info/SOURCES.txt
+-rw-r--r--   0 ahw001   (1186363539) 1287271524        1 2023-07-08 04:52:59.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh.gks.metaschema.egg-info/dependency_links.txt
+-rw-r--r--   0 ahw001   (1186363539) 1287271524       24 2023-07-08 04:52:59.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh.gks.metaschema.egg-info/requires.txt
+-rw-r--r--   0 ahw001   (1186363539) 1287271524        6 2023-07-08 04:52:59.000000 ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh.gks.metaschema.egg-info/top_level.txt
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.096292 ga4gh.gks.metaschema-0.2.0rc5/tests/
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.099953 ga4gh.gks.metaschema-0.2.0rc5/tests/data/
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     2583 2023-04-17 14:22:22.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/catvars-source.yaml
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     2755 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/catvars.yaml
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     6734 2023-07-08 04:41:37.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/core-source.yaml
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     3100 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/core.yaml
+drwxr-xr-x   0 ahw001   (1186363539) 1287271524        0 2023-07-08 04:53:00.110045 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1734 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/AbsoluteCopyNumber.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1922 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/Allele.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1841 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/ChromosomeLocation.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1365 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/ComposedSequenceExpression.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     2418 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/CopyNumberChange.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     2036 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/CopyNumberCount.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      676 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/DefiniteRange.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1193 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/DerivedSequenceExpression.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     2236 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/Genotype.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1697 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/GenotypeMember.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1838 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/Haplotype.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      401 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/HumanCytoband.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1030 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/IndefiniteRange.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1216 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/LiteralSequenceExpression.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      313 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/Location.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      358 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/MolecularVariation.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      537 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/Number.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      414 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/Range.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1684 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/ReferenceLengthExpression.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1779 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/RelativeCopyNumber.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     2707 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/RepeatedSequenceExpression.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      486 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/Residue.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      408 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/Sequence.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      392 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/SequenceExpression.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     2452 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/SequenceLocation.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1765 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/SequenceReference.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      450 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/SequenceString.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      500 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/SystemicVariation.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      967 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/Text.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      483 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/UtilityVariation.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      544 2023-07-08 04:41:46.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/Variation.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     1823 2023-07-07 20:58:19.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/json_schema/VariationSet.json
+-rw-r--r--   0 ahw001   (1186363539) 1287271524     9861 2023-04-17 14:24:36.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/vod-source.yaml
+-rw-r--r--   0 ahw001   (1186363539) 1287271524    16965 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/vod.yaml
+-rw-r--r--   0 ahw001   (1186363539) 1287271524    24195 2023-07-08 04:41:37.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/vrs-source.yaml
+-rw-r--r--   0 ahw001   (1186363539) 1287271524    17572 2023-07-08 04:41:45.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/vrs.yaml
+-rw-r--r--   0 ahw001   (1186363539) 1287271524    25339 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/vrs1-source.yaml
+-rw-r--r--   0 ahw001   (1186363539) 1287271524    22622 2023-04-17 14:01:17.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/data/vrs1.yaml
+-rw-r--r--   0 ahw001   (1186363539) 1287271524      916 2023-07-08 04:19:05.000000 ga4gh.gks.metaschema-0.2.0rc5/tests/test_basic.py
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/.gitignore` & `ga4gh.gks.metaschema-0.2.0rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/LICENSE` & `ga4gh.gks.metaschema-0.2.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/PKG-INFO` & `ga4gh.gks.metaschema-0.2.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4gh.gks.metaschema
-Version: 0.2.0rc4
+Version: 0.2.0rc5
 Summary: GA4GH Genomic Knowledge Standards meta-schema tools
 Home-page: https://github.com/ga4gh/gks-metaschema
 Author: Alex Wagner, PhD
 Author-email: Alex.Wagner@nationwidechildrens.org
 Project-URL: Bug Tracker, https://github.com/ga4gh/gks-metaschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/setup.cfg` & `ga4gh.gks.metaschema-0.2.0rc5/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ga4gh.gks.metaschema
-version = 0.2.0rc4
+version = 0.2.0rc5
 author = Alex Wagner, PhD
 author_email = Alex.Wagner@nationwidechildrens.org
 description = GA4GH Genomic Knowledge Standards meta-schema tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ga4gh/gks-metaschema
 project_urls = 
@@ -20,17 +20,19 @@
 packages = find_namespace:
 python_requires = >=3.6
 scripts = 
 	src/ga4gh/gks/metaschema/scripts/jsy2js.py
 	src/ga4gh/gks/metaschema/scripts/source2jsy.py
 	src/ga4gh/gks/metaschema/scripts/y2t.py
 	src/ga4gh/gks/metaschema/scripts/source2mergedjsy.py
+	src/ga4gh/gks/metaschema/scripts/source2splitjs.py
 install_requires = 
 	inflector
 	pyyaml
+	pytest
 setup_requires = 
 	build
 	twine
 
 [options.packages.find]
 where = src
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/metaschema/scripts/y2t.py` & `ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/scripts/y2t.py`

 * *Files identical despite different names*

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh/gks/metaschema/tools/source_proc.py` & `ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh/gks/metaschema/tools/source_proc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 """convert yaml on stdin to json on stdout"""
 import copy
 import json
 import yaml
 import re
 from pathlib import Path
+import os
 
 SCHEMA_DEF_KEYWORD_BY_VERSION = {
     "http://json-schema.org/draft-07/schema": "definitions",
     "http://json-schema.org/draft/2020-12/schema": "$defs"
 }
 
 
@@ -167,21 +168,29 @@
         for schema_class in self.defs:
             self.process_schema_class(schema_class)
 
     def class_is_abstract(self, schema_class):
         schema_class_def, _ = self.get_local_or_inherited_class(schema_class, raw=True)
         return 'properties' not in schema_class_def and not self.class_is_primitive(schema_class)
 
+    def class_is_private(self, schema_class):
+        schema_class_def, _ = self.get_local_or_inherited_class(schema_class, raw=True)
+        return 'privateTo' in schema_class_def
+
+    def class_is_digestible(self, schema_class):
+        schema_class_def, _ = self.get_local_or_inherited_class(schema_class, raw=True)
+        return 'ga4ghDigest' in schema_class_def and not self.class_is_abstract(schema_class)
+
     def class_is_passthrough(self, schema_class):
         if not self.class_is_abstract(schema_class):
             return False
-        raw_class_definition = self.get_local_or_inherited_class(schema_class, raw=True)
+        raw_class_definition, _ = self.get_local_or_inherited_class(schema_class, raw=True)
         if 'heritable_properties' not in raw_class_definition \
                 and 'properties' not in raw_class_definition \
-                and raw_class_definition[0].get('inherits'):
+                and raw_class_definition.get('inherits', False):
             return True
         return False
 
     def class_is_primitive(self, schema_class):
         schema_class_def, _ = self.get_local_or_inherited_class(schema_class, raw=True)
         schema_class_type = schema_class_def.get('type', 'abstract')
         if schema_class_type not in ['abstract', 'object']:
@@ -190,14 +199,32 @@
 
     def js_json_dump(self, stream):
         json.dump(self.for_js, stream, indent=3, sort_keys=False)
 
     def js_yaml_dump(self, stream):
         yaml.dump(self.for_js, stream, sort_keys=False)
 
+    def split_defs_to_js(self, fp=None):
+        if fp is None:
+            fp = self.schema_fp.parent / 'json_schema'
+        else:
+            assert isinstance(fp, Path)
+        if not fp.exists():
+            os.mkdir(fp)
+        kw = self.schema_def_keyword
+        for cls in self.for_js[kw].keys():
+            class_def = self.for_js[kw][cls]
+            target_path = fp / f'{cls}.json'
+            out_doc = copy.deepcopy(self.for_js)
+            out_doc.pop(kw, None)
+            out_doc.update(class_def)
+            out_doc['title'] = cls
+            with open(target_path, 'w') as f:
+                json.dump(out_doc, f, indent=3, sort_keys=False)
+
     def resolve_curie(self, curie):
         namespace, identifier = curie.split(':')
         base_url = self.processed_schema['namespaces'][namespace]
         return base_url + identifier
 
     def process_property_tree_refs(self, raw_node, processed_node):
         if isinstance(raw_node, dict):
@@ -239,28 +266,47 @@
             raise ValueError
         return inherited_class, proc
 
     def process_schema_class(self, schema_class):
         raw_class_def = self.raw_schema[self.schema_def_keyword][schema_class]
         if schema_class in self.processed_classes:
             return
+        processed_class_def = self.processed_schema[self.schema_def_keyword][schema_class]
+
+        # Check GKS maturity model on all public, concrete classes
+        if not (self.class_is_private(schema_class) or self.class_is_abstract(schema_class)):
+            assert 'maturity' in processed_class_def, schema_class
+            assert processed_class_def['maturity'] in ['Alpha', 'Beta', 'RC', 'Stable'], schema_class
+
         if self.class_is_primitive(schema_class):
             self.processed_classes.add(schema_class)
             return
-        processed_class_def = self.processed_schema[self.schema_def_keyword][schema_class]
         inherited_properties = dict()
         inherited_required = set()
         inherits = processed_class_def.get('inherits', None)
         if inherits is not None:
             inherited_class, proc = self.get_local_or_inherited_class(inherits)
             # extract properties / heritable_properties and required / heritable_required from inherited_class
             # currently assumes inheritance from abstract classes only–will break otherwise
             inherited_properties |= copy.deepcopy(inherited_class['heritable_properties'])
             inherited_required |= set(inherited_class.get('heritable_required', list()))
 
+            # inherit ga4ghDigest keys
+            if 'ga4ghDigest' in processed_class_def or 'ga4ghDigest' in inherited_class:
+                if 'ga4ghDigest' not in processed_class_def:
+                    assert self.class_is_abstract(schema_class), \
+                        f'{schema_class} is missing a defined prefix.'
+                    processed_class_def['ga4ghDigest'] = copy.deepcopy(inherited_class['ga4ghDigest'])
+                elif 'ga4ghDigest' not in inherited_class:
+                    pass
+                else:
+                    ga4ghDigest_keys = set(inherited_class['ga4ghDigest']['keys'])
+                    ga4ghDigest_keys |= set(processed_class_def['ga4ghDigest'].get('keys', list()))
+                    processed_class_def['ga4ghDigest']['keys'] = sorted(list(ga4ghDigest_keys))
+
         if self.class_is_abstract(schema_class):
             prop_k = 'heritable_properties'
             req_k = 'heritable_required'
         else:
             prop_k = 'properties'
             req_k = 'required'
         raw_class_properties = raw_class_def.get(prop_k, dict())  # Nested inheritance!
@@ -294,19 +340,30 @@
                     inherited_required.remove(extended_property)
                     processed_class_required.add(prop)
             # Validate required array attribute for GKS specs
             if self.enforce_ordered and prop_attribs.get('type', '') == 'array':
                 assert 'ordered' in prop_attribs, f'{schema_class}.{prop} missing ordered attribute.'
                 assert isinstance(prop_attribs['ordered'], bool)
 
+        # Validate class structures for GKS specs
         if self.class_is_abstract(schema_class):
             assert 'type' not in processed_class_def, schema_class
         else:
             assert 'type' in processed_class_def, schema_class
             assert processed_class_def['type'] == 'object', schema_class
+            if self.class_is_digestible(schema_class):
+                assert isinstance(processed_class_def['ga4ghDigest']['prefix'], str), schema_class
+                assert processed_class_def['ga4ghDigest']['prefix'] != '', schema_class
+                l = len(processed_class_def['ga4ghDigest']['keys'])
+                assert l >= 2, \
+                    f'GA4GH digests are expected to be defined by at least 2 properties, {schema_class} has {l}.'
+                assert 'type' in processed_class_def['ga4ghDigest']['keys'], \
+                    f'GA4GH digests are expected to include the class type but not included for {schema_class}.'
+                    # Two properites should be `type` and at least one other field
+
         processed_class_def[prop_k] = inherited_properties | processed_class_properties
         processed_class_def[req_k] = sorted(list(inherited_required | processed_class_required))
         if self.strict and not self.class_is_abstract(schema_class):
             processed_class_def['additionalProperties'] = False
         self.processed_classes.add(schema_class)
 
     @staticmethod
@@ -323,14 +380,15 @@
         self.for_js.pop('imports', None)
         abstract_class_removals = list()
         for schema_class, schema_definition in self.for_js.get(self.schema_def_keyword, dict()).items():
             schema_definition.pop('inherits', None)
             if self.class_is_abstract(schema_class):
                 schema_definition.pop('heritable_properties', None)
                 schema_definition.pop('heritable_required', None)
+                schema_definition.pop('ga4ghDigest', None)
                 schema_definition.pop('header_level', None)
                 self.concretize_js_object(schema_definition)
                 if 'oneOf' not in schema_definition:
                     abstract_class_removals.append(schema_class)
             if 'description' in schema_definition:
                 schema_definition['description'] = \
                     self._scrub_rst_markup(schema_definition['description'])
@@ -350,19 +408,23 @@
             if descendents != {js_obj['$ref']}:
                 js_obj.pop('$ref')
                 js_obj['oneOf'] = self._build_ref_list(descendents)
         elif 'oneOf' in js_obj:
             # do the same check for each member
             ref_list = js_obj['oneOf']
             descendents = set()
+            inlined = list()
             for ref in ref_list:
-                descendents.update(self.concretize_class_ref(ref['$ref']))
-            js_obj['oneOf'] = self._build_ref_list(descendents)
+                if '$ref' not in ref:
+                    inlined.append(ref)
+                else:
+                    descendents.update(self.concretize_class_ref(ref['$ref']))
+            js_obj['oneOf'] = self._build_ref_list(descendents) + inlined
         elif js_obj.get('type', '') == 'array':
-            self.concretize_js_object(js_obj['items'])
+                self.concretize_js_object(js_obj['items'])
 
     def concretize_class_ref(self, cls_url):
         children = self.has_children.get(cls_url, None)
         if children is None:
             return {cls_url}
         out = set()
         for child in children:
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/src/ga4gh.gks.metaschema.egg-info/PKG-INFO` & `ga4gh.gks.metaschema-0.2.0rc5/src/ga4gh.gks.metaschema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4gh.gks.metaschema
-Version: 0.2.0rc4
+Version: 0.2.0rc5
 Summary: GA4GH Genomic Knowledge Standards meta-schema tools
 Home-page: https://github.com/ga4gh/gks-metaschema
 Author: Alex Wagner, PhD
 Author-email: Alex.Wagner@nationwidechildrens.org
 Project-URL: Bug Tracker, https://github.com/ga4gh/gks-metaschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/tests/data/catvars-source.yaml` & `ga4gh.gks.metaschema-0.2.0rc5/tests/data/catvars-source.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
   ComplexVariation:
     ga4gh_prefix: CXV
     inherits: CategoricalVariation
     description: >-
       A categorical variation domain jointly characterized by two or more other categorical 
       variation domains.
+    type: object
     properties:
       type:
         type: string
         description: MUST be "ComplexVariation".
         const: ComplexVariation
       operands:
         type: array
@@ -54,14 +55,15 @@
           The logical operation applied to evaluating the object *operands*. MUST
           be "AND" or "OR".
     required: ["operands", "operator"]
 
   CanonicalVariation:
     ga4gh_prefix: CLV
     inherits: CategoricalVariation
+    type: object
     description: >-
       A categorical variation domain characterized by a representative Variation context 
       to which members lift-over, project, translate, or otherwise directly align.
     properties:
       type:
         type: string
         const: CanonicalVariation
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/tests/data/catvars.yaml` & `ga4gh.gks.metaschema-0.2.0rc5/tests/data/catvars.yaml`

 * *Files identical despite different names*

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/tests/data/core-source.yaml` & `ga4gh.gks.metaschema-0.2.0rc5/tests/data/core-source.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -12,94 +12,58 @@
     heritable_properties:
       id:
         type: string
         description: >-
           The 'logical' identifier of the entity in the system of record, e.g. a UUID. This 'id' is 
           unique within a given system. The identified entity may have a different 'id' in a different 
           system, or may refer to an 'id' for the shared concept in another system (e.g. a CURIE).
-      type:
-        type: string
-        description: >-
-          The schema class that is instantiated by the data object. Must be the name of a class from 
-          the VA schema.
-    heritable_required: [ "type" ]
-    discriminator:
-      propertyName: type
-
-  ValueEntity:
-    inherits: Entity
-    description: >-
-      ValueEntity is the root class for classes that instantiate Value Objects. ValueEntity classes
-      are not extensible and MUST NOT have optional properties.
-    heritable_properties:
-      id:
-        $ref: "#/$defs/CURIE"
-        description: >-
-          The 'logical' identifier of the entity in the system of record, and MUST be represented as a CURIE.
-          This 'id' is unique within a given system, but may also refer to an 'id' for the shared concept in 
-          another system (represented by namespace, accordingly).
-
-  DomainEntity:
-    inherits: ValueEntity
-    description: >-
-      An abstract :ref:`ValueEntity` class extended to capture specific domain entities by reference
-      to an external identifier.
-    heritable_required:
-      [ "id" ]
-
-  ExtensibleEntity:
-    inherits: Entity
-    description: >-
-      ExtensibleEntity is the root class for classes that instantiate Extensible Objects. Extensible
-      Objects are extensible using the extensions property and MAY have optional properties.
-    heritable_properties:
       label:
         type: string
       extensions:
         type: array
         ordered: true
         items:
           $ref: "#/$defs/Extension"
+    discriminator:
+      propertyName: type
 
-  RecordMetadata:
-    inherits: ExtensibleEntity
+  Mapping:
+    type: object
+    inherits: Entity
+    maturity: Alpha
     description: >-
-      A re-usable structure that encapsulates provenance metadata that applies to a specific
-      concrete record of information as encoded in a particular system, as opposed to 
-      provenance of the abstract information content/knowledge the record represents.
+      A mapping to a concept in a terminology system.
     properties:
-      type:
+      system:
         type: string
-        const: RecordMetadata
-        default: RecordMetadata
-        description: MUST be "RecordMetadata".
-      is_version_of:
-        $ref: "#/$defs/CURIE"
+        description: Identity of the terminology system.
       version:
         type: string
-
-  Coding:
-    inherits: ExtensibleEntity
-    description: >-
-      A `coding` is an extensible entity for labeling or otherwise annotating globally 
-      namespaced identifiers known as "codes".
-    properties:
-      type:
-        type: string
-        const: Coding
-        default: Coding
-        description: MUST be "Coding".
-      id:
-        $ref: "#/$defs/CURIE"
+        description: Version of the terminology system.
+      code:
+        $ref: '#/$defs/Code'
+        description: Symbol in syntax defined by the terminology system.
+      mapping:
         description: >-
-          The `coding.id` field is used to capture the code as a CURIE.
-      record_metadata:
-        $ref: "#/$defs/RecordMetadata"
+          A mapping between concepts as defined by the Simple Knowledge Organization System (SKOS).
+        type: string
+        enum:
+          - closeMatch
+          - exactMatch
+          - broadMatch
+          - narrowMatch
+          - relatedMatch
+    required:
+      - mapping
+      - code
+      - system
 
   Extension:
+    type: object
+    maturity: Alpha
     description: >-
       The Extension class provides VODs with a means to extend descriptions
       with other attributes unique to a content provider. These extensions
       are not expected to be natively understood under VRSATILE, but may be
       used for pre-negotiated exchange of message attributes when needed.
     properties:
       type:
@@ -110,115 +74,138 @@
         type: string
         description: A name for the Extension
       value:
         type: [ "number", "string", "boolean", "object", "array", "null" ]
         description: Any primitive or structured object
     required: [ "name" ]
 
-  CURIE:
+  Code:
+    maturity: Alpha
     description: >-
-      A `W3C Compact URI <https://www.w3.org/TR/curie/>`_ formatted string.
-      A CURIE string has the structure ``prefix``:``reference``, as defined by
-      the W3C syntax.
+      Indicates that the value is taken from a set of controlled strings defined elsewhere.
+      Technically, a code is restricted to a string which has at least one character and no leading or 
+      trailing whitespace, and where there is no whitespace other than single spaces in the contents.
     type: string
-    pattern: '^\w[^:]*:.+$'
-    example: "ensembl:ENSG00000139618"
-
-  Disease:
-    inherits: DomainEntity
-    description: >-
-      A reference to a Disease as defined by an authority. For human diseases,
-      the use of `MONDO <https://registry.identifiers.org/registry/mondo>`_
-      as the disease authority is RECOMMENDED.
-    properties:
-      type:
-        type: string
-        const: Disease
-        default: Disease
-        description: MUST be "Disease".
-
-  Phenotype:
-    inherits: DomainEntity
-    description: >-
-      A reference to a Phenotype as defined by an authority. For human phenotypes,
-      the use of `HPO <https://registry.identifiers.org/registry/hpo>`_
-      as the disease authority is RECOMMENDED.
-    properties:
-      type:
-        type: string
-        const: Phenotype
-        default: Phenotype
-        description: MUST be "Phenotype".
-
-  Gene:
-    inherits: DomainEntity
-    description: >-
-      A reference to a Gene as defined by an authority. For human genes,
-      the use of `hgnc <https://registry.identifiers.org/registry/hgnc>`_
-      as the gene authority is RECOMMENDED.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "Gene"
-        default: "Gene"
-        description: MUST be "Gene"
-
-  Condition:
-    description: A set of phenotype and/or disease concepts that constitute a condition.
-    inherits: ValueEntity
-    properties:
-      members:
-        type: array
-        ordered: false
-        items:
-          anyOf:
-            - $ref: "#/$defs/Disease"
-            - $ref: "#/$defs/Phenotype"
-        minItems: 2
-    required: [ "members" ]
-
-  Therapeutic:
-    inherits: DomainEntity
-    description: A treatment, therapy, or drug.
-    properties:
-      type:
-        type: string
-        const: Therapeutic
-        default: Therapeutic
-        description: MUST be "Therapeutic".
-
-  TherapeuticsCollection:
-    inherits: ValueEntity
-    description: A collection of therapeutics.
-    heritable_properties:
-      members:
-        type: array
-        ordered: false
-        description: >-
-          The therapeutics that constitute the described collection.
-        items:
-          $ref: "#/$defs/Therapeutic"
-        minItems: 2
-    heritable_required: [ "members" ]
+    pattern: '\S+( \S+)*'
+    example: ENSG00000139618
 
-  CombinationTherapeutics:
-    inherits: TherapeuticsCollection
+  IRI:
+    maturity: Alpha
     description: >-
-      A collection of therapeutics that are taken during a course of treatment.
-    properties:
-      type:
-        type: string
-        const: CombinationTherapeutics
-        default: CombinationTherapeutics
-        description: MUST be "CombinationTherapeutics"
+      An IRI Reference (either an IRI or a relative-reference), according to `RFC3986 section 4.1 
+      <https://datatracker.ietf.org/doc/html/rfc3986#section-4.1>` and `RFC3987 section 2.1
+      <https://datatracker.ietf.org/doc/html/rfc3987#section-2.1>`. MAY be a JSON Pointer as an IRI fragment, as 
+      described by `RFC6901 section 6 <https://datatracker.ietf.org/doc/html/rfc6901#section-6>`.
+    type: string
+    format: iri-reference
 
-  SubstituteTherapeutics:
-    inherits: TherapeuticsCollection
-    description: >-
-      A collection of therapeutics that are considered as valid alternative entities.
-    properties:
-      type:
-        type: string
-        const: SubstituteTherapeutics
-        default: SubstituteTherapeutics
-        description: MUST be "SubstituteTherapeutics"
+#  CodeableEntity:  # TODO: Discussion on CodeableConcept analog pending
+#    inherits: Entity
+#    description: >-
+#      An entity that may be associated with codes in one or more systems.
+#    properties:
+
+#  Disease:
+#    type: object
+#    inherits: DomainEntity
+#    description: >-
+#      A reference to a Disease as defined by an authority. For human diseases,
+#      the use of `MONDO <https://registry.identifiers.org/registry/mondo>`_
+#      as the disease authority is RECOMMENDED.
+#    properties:
+#      type:
+#        type: string
+#        const: Disease
+#        default: Disease
+#        description: MUST be "Disease".
+#
+#  Phenotype:
+#    type: object
+#    inherits: DomainEntity
+#    description: >-
+#      A reference to a Phenotype as defined by an authority. For human phenotypes,
+#      the use of `HPO <https://registry.identifiers.org/registry/hpo>`_
+#      as the disease authority is RECOMMENDED.
+#    properties:
+#      type:
+#        type: string
+#        const: Phenotype
+#        default: Phenotype
+#        description: MUST be "Phenotype".
+#
+#  Gene:
+#    inherits: DomainEntity
+#    description: >-
+#      A reference to a Gene as defined by an authority. For human genes,
+#      the use of `hgnc <https://registry.identifiers.org/registry/hgnc>`_
+#      as the gene authority is RECOMMENDED.
+#    type: object
+#    properties:
+#      type:
+#        type: string
+#        const: "Gene"
+#        default: "Gene"
+#        description: MUST be "Gene"
+#
+#  Condition:
+#    type: object
+#    description: A set of phenotype and/or disease concepts that constitute a condition.
+#    inherits: ValueEntity
+#    properties:
+#      members:
+#        type: array
+#        ordered: false
+#        items:
+#          anyOf:
+#            - $ref: "#/$defs/Disease"
+#            - $ref: "#/$defs/Phenotype"
+#        minItems: 2
+#    required: [ "members" ]
+#
+#  Therapeutic:
+#    type: object
+#    inherits: DomainEntity
+#    description: A treatment, therapy, or drug.
+#    properties:
+#      type:
+#        type: string
+#        const: Therapeutic
+#        default: Therapeutic
+#        description: MUST be "Therapeutic".
+#
+#  TherapeuticCollection:
+#    inherits: ValueEntity
+#    description: A collection of therapeutics.
+#    heritable_properties:
+#      members:
+#        type: array
+#        ordered: false
+#        description: >-
+#          The therapeutics that constitute the described collection.
+#        items:
+#          $ref: "#/$defs/Therapeutic"
+#        minItems: 2
+#    heritable_required: [ "members" ]
+#
+#  CombinationTherapeuticCollection:
+#    type: object
+#    inherits: TherapeuticCollection
+#    description: >-
+#      A collection of therapeutics that are taken during a course of treatment.
+#    properties:
+#      type:
+#        type: string
+#        const: CombinationTherapeutics
+#        default: CombinationTherapeutics
+#        description: MUST be "CombinationTherapeutics"
+#
+#  SubstituteTherapeuticCollection:
+#    type: object
+#    inherits: TherapeuticCollection
+#    description: >-
+#      A collection of therapeutics that are considered as valid alternative entities.
+#    properties:
+#      type:
+#        type: string
+#        const: SubstituteTherapeutics
+#        default: SubstituteTherapeutics
+#        description: MUST be "SubstituteTherapeutics"
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/tests/data/vod-source.yaml` & `ga4gh.gks.metaschema-0.2.0rc5/tests/data/vod-source.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
           Genotype Ontology (GENO). These SHOULD descend from concept
           `GENO:0000875 <http://purl.obolibrary.org/obo/GENO_0000875>`.
 
   ConditionDescriptor:
     inherits: ValueObjectDescriptor
     description: >-
       This descriptor class is used for describing Condition domain entities.
+    type: object
     properties:
       type:
         type: string
         const: ConditionDescriptor
         default: ConditionDescriptor
         description: MUST be "ConditionDescriptor".
       condition:
@@ -132,14 +133,15 @@
             - $ref: "#/definitions/DiseaseDescriptor"
             - $ref: "#/definitions/PhenotypeDescriptor"
 
   GeneDescriptor:
     inherits: ValueObjectDescriptor
     description: >-
       This descriptor class is used for describing Gene domain entities.
+    type: object
     properties:
       type:
         type: string
         const: GeneDescriptor
         default: GeneDescriptor
         description: MUST be "GeneDescriptor".
       gene:
@@ -148,14 +150,15 @@
       gene_id:
         extends: value_id
 
   DiseaseDescriptor:
     inherits: ValueObjectDescriptor
     description: >-
       This descriptor class is used for describing Disease domain entities.
+    type: object
     properties:
       type:
         type: string
         const: DiseaseDescriptor
         default: DiseaseDescriptor
         description: MUST be "DiseaseDescriptor".
       disease:
@@ -164,14 +167,15 @@
       disease_id:
         extends: value_id
 
   PhenotypeDescriptor:
     inherits: ValueObjectDescriptor
     description: >-
       This descriptor class is used for describing Disease domain entities.
+    type: object
     properties:
       type:
         type: string
         const: PhenotypeDescriptor
         default: PhenotypeDescriptor
         description: MUST be "PhenotypeDescriptor".
       phenotype:
@@ -180,14 +184,15 @@
       phenotype_id:
         extends: value_id
 
   TherapeuticDescriptor:
     inherits: ValueObjectDescriptor
     description: >-
       This descriptor class is used for describing Therapeutic domain entities.
+    type: object
     properties:
       type:
         type: string
         const: TherapeuticDescriptor
         default: TherapeuticDescriptor
         description: MUST be "TherapeuticDescriptor".
       therapeutic:
@@ -196,14 +201,15 @@
       therapeutic_id:
         extends: value_id
 
   TherapeuticsCollectionDescriptor:
     inherits: ValueObjectDescriptor
     description: >-
       This descriptor class is used for describing TherapeuticsCollection domain entities.
+    type: object
     properties:
       type:
         type: string
         const: TherapeuticsCollectionDescriptor
         default: TherapeuticsCollectionDescriptor
         description: MUST be "TherapeuticsCollectionDescriptor".
       therapeutics_collection:
@@ -216,17 +222,18 @@
       member_descriptors:
         type: array
         ordered: false
         items:
           $ref: "#/definitions/TherapeuticDescriptor"
 
   Expression:
-    maturity: draft
+    maturity: Alpha
     description: >-
       Representation of a variation by a specified nomenclature or syntax for a Variation object. Common examples of expressions for the description of molecular variation include the HGVS and ISCN nomenclatures.
+    type: object
     properties:
       type:
         type: string
         const: Expression
       syntax:
         type: string
         enum: ["hgvs.c", "hgvs.p", "hgvs.g", "hgvs.m", "hgvs.n", "hgvs.r", "iscn", "gnomad", "spdi"]
@@ -236,15 +243,14 @@
         type: string
     required: ['type', 'syntax', 'value']
 
   CategoricalVariationDescriptor:
     inherits: ValueObjectDescriptor
     description: >-
       This descriptor class is used for describing Categorical Variation value objects.
-    type: object
     oneOf:
       - $ref: "#/definitions/CanonicalVariationDescriptor"
     heritable_properties:
       categorical_variation_id:
         extends: value_id
         $ref_curie: gks.core:CURIE
         description: >-
@@ -263,14 +269,15 @@
         items:
           $ref: "#/definitions/VariationMember"
 
   CanonicalVariationDescriptor:
     inherits: CategoricalVariationDescriptor
     description: >-
       This descriptor class is used for describing Canonical Variation value objects.
+    type: object
     properties:
       type:
         type: string
         const: CanonicalVariationDescriptor
         default: CanonicalVariationDescriptor
         description: MUST be "CanonicalVariationDescriptor".
       subject_variation_descriptor:
@@ -282,14 +289,15 @@
         $ref_curie: catvars:CanonicalVariation
 
   VariationMember:
     description: >-
       A compact class for representing a variation context that is a member of a
       Categorical Variation. It supports one or more Expressions of a Variation
       and optionally an associated VRS ID.
+    type: object
     properties:
       type:
         type: string
         const: VariationMember
         description: MUST be "VariationMember"
       expressions:
         type: array
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/tests/data/vod.yaml` & `ga4gh.gks.metaschema-0.2.0rc5/tests/data/vod.yaml`

 * *Files identical despite different names*

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/tests/data/vrs-source.yaml` & `ga4gh.gks.metaschema-0.2.0rc5/tests/data/vrs1-source.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -9,37 +9,40 @@
 
 # https://json-schema.org/understanding-json-schema/reference/schema.html
 $schema: "http://json-schema.org/draft-07/schema"
 title: "GA4GH-VRS-Definitions"
 type: object
 strict: true
 
-imports:
-  gks.core: core-source.yaml
-
-namespaces:
-  gks.core: core.json#/$defs/
-
 definitions:
   # VRS definitions are presented top-down.  Everything rolls up to
   # Variation, which is a polymorphic abstraction of many kinds of
   # variation.
 
   # =============================================================================
   # Kinds of Variation
   # =============================================================================
 
   Variation:
-    inherits: gks.core:ValueEntity
     description: >-
       A representation of the state of one or more biomolecules.
     oneOf:
       - $ref: "#/definitions/MolecularVariation"
       - $ref: "#/definitions/SystemicVariation"
       - $ref: "#/definitions/UtilityVariation"
+    heritable_properties:
+      _id:
+        $ref: "#/definitions/CURIE"
+        description: >-
+          Variation Id. MUST be unique within document.
+      type:
+        type: string
+        description: >-
+          The Variation class type. MUST match child class type.
+    heritable_required: ["type"]
 
     discriminator:
       propertyName: type
 
   MolecularVariation:
     inherits: Variation
     description: >-
@@ -64,84 +67,85 @@
 
   SystemicVariation:
     inherits: Variation
     description: >-
       A Variation of multiple molecules in the context of a system, e.g.
       a genome, sample, or homologous chromosomes.
     oneOf:
+      - $ref: "#/definitions/CopyNumber"
       - $ref: "#/definitions/Genotype"
-      - $ref: "#/definitions/AbsoluteCopyNumber"
-      - $ref: "#/definitions/RelativeCopyNumber"
     discriminator:
       propertyName: type
 
   # =============================================================================
   # IDENTIFIABLE TYPES
   # Have a `type` and `_id` attribute
   # =============================================================================
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # Molecular Variation
 
   Allele:
-    ga4gh_prefix: VA
     inherits: MolecularVariation
     description: >-
       The state of a molecule at a :ref:`Location`.
     type: object
     properties:
       type:
         type: string
         const: "Allele"
         default: "Allele"
         description: >-
           MUST be "Allele"
       location:
         oneOf:
-          - $ref_curie: gks.core:CURIE
+          - $ref: "#/definitions/CURIE"
           - $ref: "#/definitions/Location"
         description: >-
           Where Allele is located
       state:
-        $ref: "#/definitions/SequenceExpression"
+        oneOf:
+          - $ref: "#/definitions/SequenceExpression"
+          - $ref: "#/definitions/SequenceState" # DEPRECATED; remove in 2.0
         description: >-
           An expression of the sequence state
+        deprecated:
+          - $ref: "#/definitions/SequenceState"
     required: [ "location", "state" ]
 
   Haplotype:
-    ga4gh_prefix: HT
     inherits: MolecularVariation
     description: >-
       A set of non-overlapping :ref:`Allele` members that co-occur on the same molecule.
     type: "object"
     properties:
       type:
         type: string
         const: "Haplotype"
         default: "Haplotype"
         description: >-
           MUST be "Haplotype"
       members:
         type: array
-        ordered: false
         minItems: 2
         uniqueItems: true
+        ordered: false
         items:
           oneOf:
             - $ref: "#/definitions/Allele"
-            - $ref_curie: gks.core:CURIE
+            - $ref: "#/definitions/CURIE"
         description: >-
           List of Alleles, or references to Alleles, that comprise this Haplotype.
     required: [ "members" ]
 
+
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # UtilityVariation
 
   Text:
-    ga4gh_prefix: VT
     inherits: UtilityVariation
     description: >-
       A free-text definition of variation.
     type: object
     properties:
       type:
         type: string
@@ -152,230 +156,282 @@
         type: string
         description: >-
           A textual representation of variation not representable by
           other subclasses of Variation.
     required: [ "definition" ]
 
   VariationSet:
-    ga4gh_prefix: VS
     inherits: UtilityVariation
     description: >-
       An unconstrained set of Variation members.
     type: object
     properties:
       type:
         type: string
         const: "VariationSet"
         default: "VariationSet"
         description: MUST be "VariationSet"
       members:
         type: array
-        ordered: false
         uniqueItems: true
+        ordered: false
         items:
           oneOf:
-            - $ref_curie: gks.core:CURIE
+            - $ref: "#/definitions/CURIE"
             - $ref: "#/definitions/Variation"
         description: >-
           List of Variation objects or identifiers. Attribute is
           required, but MAY be empty.
     required: [ "members" ]
 
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # SystemicVariation
 
   CopyNumber:
     inherits: SystemicVariation
-    type: object
     description: >-
-      A measure of the copies of a :ref:`Location` within a system (e.g. a genome)
+      The copies of :ref:`Location` in a system, expressed as an absolute integer
+      quantity (:ref:`AbsoluteCopyNumber`) or a qualitative description of copies 
+      relative to a baseline state (:ref:`RelativeCopyNumber`).
     heritable_properties:
-      location:
+      subject:
         oneOf:
-          - $ref_curie: gks.core:CURIE
           - $ref: "#/definitions/Location"
+          - $ref: "#/definitions/CURIE"
         description: >-
-          The location within the system.
-    heritable_required: [ "location" ]
+          A location for which the number of systemic copies is described.
+    heritable_required: [ "subject" ]
 
   AbsoluteCopyNumber:
-    ga4gh_prefix: ACN
     inherits: CopyNumber
     type: object
+    maturity: draft
     description: >-
-      The absolute count of discrete copies of a :ref:`MolecularVariation`,
-      :ref:`Feature`, :ref:`SequenceExpression`, or a :ref:`CURIE` reference
+      The absolute count of discrete copies of a :ref:`Location`,
       within a system (e.g. genome, cell, etc.).
     properties:
       type:
         type: string
         const: "AbsoluteCopyNumber"
         default: "AbsoluteCopyNumber"
         description: >-
-          MUST be "AbsoluteCopyNumber".
+          MUST be "AbsoluteCopyNumber"
       copies:
         oneOf:
           - $ref: "#/definitions/Number"
           - $ref: "#/definitions/IndefiniteRange"
           - $ref: "#/definitions/DefiniteRange"
         description: >-
-          The integral number of copies of the subject in a system.
+          The integral number of copies of the subject in a system
     required: [ "copies" ]
 
   RelativeCopyNumber:
-    ga4gh_prefix: RCN
     inherits: CopyNumber
     type: object
     maturity: draft
     description: >-
-      The relative copies of a :ref:`MolecularVariation`,
-      :ref:`Feature`, :ref:`SequenceExpression`, or a :ref:`CURIE` reference
-      against an unspecified baseline in a system (e.g. genome, cell, etc.).
+      The copies of a :ref:`Location` within a system (e.g. genome, cell, etc.)
+      relative to a baseline state.
     properties:
       type:
         type: string
         const: "RelativeCopyNumber"
         default: "RelativeCopyNumber"
         description: >-
           MUST be "RelativeCopyNumber"
       relative_copy_class:
         type: string
         enum: [ "complete loss", "partial loss", "copy neutral", "low-level gain", "high-level gain" ]
         description: >-
           MUST be one of "complete loss", "partial loss", "copy neutral", "low-level gain" or "high-level gain".
-    required: [ "relative_copy_class" ]
+    required: [  "relative_copy_class" ]
 
   Genotype:
-    ga4gh_prefix: GT
     inherits: SystemicVariation
     description: >-
-      A quantified set of _in-trans_ :ref:`MolecularVariation` at a genomic locus.
+      A quantified set of :ref:`MolecularVariation` associated with a genomic locus.
     type: object
     properties:
       type:
         type: string
         const: "Genotype"
         default: "Genotype"
         description: >-
           MUST be "Genotype"
       members:
         type: array
-        ordered: false
         uniqueItems: true
         minItems: 1
+        ordered: false
         items:
           $ref: "#/definitions/GenotypeMember"
         description: >-
           Each GenotypeMember in `members` describes a :ref:`MolecularVariation`
           and the count of that variation at the locus.
       count:
         oneOf:
           - $ref: "#/definitions/Number"
           - $ref: "#/definitions/IndefiniteRange"
           - $ref: "#/definitions/DefiniteRange"
         description: >-
           The total number of copies of all :ref:`MolecularVariation` at this locus,
-          MUST be greater than or equal to the sum of :ref:`GenotypeMember` copy counts.
-          If greater than the total counts, this implies additional 
-          :ref:`MolecularVariation` that are expected to exist but are not explicitly
-          indicated.
+          MUST be greater than or equal to the sum of :ref:`GenotypeMember` copy counts
+          and MUST be greater than or equal to 1.
+          If greater than the total of GenotypeMember counts, this field describes 
+          additional :ref:`MolecularVariation` that exist but are not 
+          explicitly described.
     required: [ "members", "count" ]
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # Locations
 
   Location:
-    inherits: gks.core:ValueEntity
     description: >-
       A contiguous segment of a biological sequence.
     oneOf:
       - $ref: "#/definitions/ChromosomeLocation"
       - $ref: "#/definitions/SequenceLocation"
+    heritable_properties:
+      _id:
+        $ref: "#/definitions/CURIE"
+        description: >-
+          Location Id. MUST be unique within document.
+      type:
+        type: string
+        description: >-
+          The Location class type. MUST match child class type.
+    heritable_required: ["type"]
     discriminator:
       propertyName: type
 
   ChromosomeLocation:
-    ga4gh_prefix: CL
     inherits: Location
     description: >-
       A Location on a chromosome defined by a species and chromosome name.
     type: object
     properties:
       type:
         type: string
         const: "ChromosomeLocation"
         default: "ChromosomeLocation"
         description: MUST be "ChromosomeLocation"
       species_id:
-        $ref_curie: gks.core:CURIE
+        $ref: "#/definitions/CURIE"
         default: "taxonomy:9606"
         description: >-
           :ref:`CURIE` representing a species from the
           `NCBI species taxonomy <https://registry.identifiers.org/registry/taxonomy>`_.
           Default: "taxonomy:9606" (human)
       chr:
         type: string
         description: >-
           The symbolic chromosome name. For humans, For humans,
           chromosome names MUST be one of 1..22, X, Y (case-sensitive)
-      start:
-        $ref: "#/definitions/HumanCytoband"
-        description: >-
-          The start cytoband region. MUST specify a region nearer the
-          terminal end (telomere) of the chromosome p-arm than `end`.
-      end:
-        $ref: "#/definitions/HumanCytoband"
+      interval:
+        $ref: "#/definitions/CytobandInterval"
         description: >-
-          The start cytoband region. MUST specify a region nearer the
-          terminal end (telomere) of the chromosome q-arm than `start`.
-    required: [ "species_id", "chr", "start", "end" ]
+          The chromosome region defined by a :ref:`CytobandInterval`
+    required: [ "species_id", "chr", "interval" ]
 
   SequenceLocation:
-    ga4gh_prefix: SL
     inherits: Location
     description: >-
       A :ref:`Location` defined by an interval on a referenced :ref:`Sequence`.
     type: object
     properties:
       type:
         type: string
         const: "SequenceLocation"
         default: "SequenceLocation"
         description: MUST be "SequenceLocation"
       sequence_id:
-        $ref_curie: gks.core:CURIE
+        $ref: "#/definitions/CURIE"
         description: >-
           A VRS :ref:`Computed Identifier <computed-identifiers>`
           for the reference :ref:`Sequence`.
+      interval:
+        oneOf:
+          - $ref: "#/definitions/SequenceInterval"
+          - $ref: "#/definitions/SimpleInterval"
+        description: >-
+          Reference sequence region defined by a :ref:`SequenceInterval`.
+    required: [ "sequence_id", "interval" ]
+
+
+  # =============================================================================
+  # NON-IDENTIFIABLE TYPES
+  # These types have a `type` attribute
+  # =============================================================================
+
+  # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+  # Intervals
+
+  SequenceInterval:
+    description: >-
+      A SequenceInterval represents a span on a :ref:`Sequence`. Positions are
+      always represented by contiguous spans using interbase coordinates or
+      coordinate ranges.
+    type: object
+    properties:
+      type:
+        type: string
+        const: "SequenceInterval"
+        default: "SequenceInterval"
+        description: MUST be "SequenceInterval"
       start:
         oneOf:
           - $ref: "#/definitions/Number"
           - $ref: "#/definitions/IndefiniteRange"
           - $ref: "#/definitions/DefiniteRange"
         description: >-
-          The start coordinate or range of the SequenceLocation.
+          The start coordinate or range of the interval.
           The minimum value of this coordinate or range is 0.
           MUST represent a coordinate or range less than the value of `end`.
       end:
         oneOf:
           - $ref: "#/definitions/Number"
           - $ref: "#/definitions/IndefiniteRange"
           - $ref: "#/definitions/DefiniteRange"
         description: >-
-          The end coordinate or range of the SequenceLocation.
+          The end coordinate or range of the interval.
           The minimum value of this coordinate or range is 0.
           MUST represent a coordinate or range greater than the value of `start`.
-    required: [ "sequence_id", "start", "end" ]
+    required: [ "type", "start", "end" ]
 
+  # SimpleInterval has been moved to DEPRECATED section at bottom.
+
+  CytobandInterval:
+    description: >-
+      A contiguous span on a chromosome defined by cytoband features.
+      The span includes the constituent regions described by the start and
+      end cytobands, as well as any intervening regions.
+    type: object
+    properties:
+      type:
+        type: string
+        const: "CytobandInterval"
+        default: "CytobandInterval"
+        description: MUST be "CytobandInterval"
+      start:
+        $ref: "#/definitions/HumanCytoband"
+        description: >-
+          The start cytoband region. MUST specify a region nearer the
+          terminal end (telomere) of the chromosome p-arm than `end`.
+      end:
+        $ref: "#/definitions/HumanCytoband"
+        description: >-
+          The start cytoband region. MUST specify a region nearer the
+          terminal end (telomere) of the chromosome q-arm than `start`.
+    example:
+      type: CytobandInterval
+      start: q22.2
+      end: q22.3
+    required: [ "type", "start", "end" ]
 
-  # =============================================================================
-  # NON-IDENTIFIABLE TYPES
-  # These types have a `type` attribute
-  # =============================================================================
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # SequenceExpression
 
   SequenceExpression:
     description: >-
       An expression describing a :ref:`Sequence`.
@@ -387,15 +443,15 @@
     discriminator:
       propertyName: type
     heritable_properties:
       type:
         type: string
         description: >-
           The SequenceExpression class type. MUST match child class type.
-    heritable_required: [ "type" ]
+    heritable_required: ["type"]
 
   LiteralSequenceExpression:
     inherits: SequenceExpression
     description: >-
       An explicit expression of a Sequence.
     type: object
     properties:
@@ -456,47 +512,14 @@
       count:
         oneOf:
           - $ref: "#/definitions/Number"
           - $ref: "#/definitions/IndefiniteRange"
           - $ref: "#/definitions/DefiniteRange"
         description: >-
           The count of repeated units, as an integer or inclusive range
-    allOf:
-      - if:
-          properties:
-            count:
-              $ref: "#/definitions/Number"
-        then:
-          properties:
-            count:
-              properties:
-                value:
-                  minimum: 0
-      - if:
-          properties:
-            count:
-              $ref: "#/definitions/IndefiniteRange"
-        then:
-          properties:
-            count:
-              properties:
-                value:
-                  minimum: 0
-      - if:
-          properties:
-            count:
-              $ref: "#/definitions/DefiniteRange"
-        then:
-          properties:
-            count:
-              properties:
-                min:
-                  minimum: 0
-                max:
-                  minimum: 0
     required: [ "seq_expr", "count" ]
 
   ComposedSequenceExpression:
     description: >-
       An expression of a sequence composed from multiple other
       :ref:`Sequence Expressions<SequenceExpression>`
       objects. MUST have at least one component that is not a
@@ -508,35 +531,38 @@
       type:
         type: string
         const: "ComposedSequenceExpression"
         default: "ComposedSequenceExpression"
         description: MUST be "ComposedSequenceExpression"
       components:
         type: array
-        ordered: true
         uniqueItems: true
         minItems: 2
+        ordered: true
         items:
-          anyOf:
+          oneOf:
             - $ref: "#/definitions/LiteralSequenceExpression"
             - $ref: "#/definitions/RepeatedSequenceExpression"
             - $ref: "#/definitions/DerivedSequenceExpression"
+        contains:
+          oneOf:
+            - $ref: "#/definitions/RepeatedSequenceExpression"
+            - $ref: "#/definitions/DerivedSequenceExpression"
         description: >-
-          An ordered list of :ref:`SequenceExpression` components
-          comprising the expression. MUST NOT have two adjacent
-          :ref:`LiteralSequenceExpression` objects.
+          An ordered list of :ref:`SequenceExpression` components  
+          comprising the expression.
     required: [ "components" ]
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # Nested Classes
 
   GenotypeMember:
     description: >-
       A class for expressing the count of a specific :ref:`MolecularVariation` present
-      _in-trans_ at a genomic locus represented by a :ref:`Genotype`.
+      *in-trans* at a genomic locus represented by a :ref:`Genotype`.
     type: object
     properties:
       type:
         type: string
         const: "GenotypeMember"
         default: "GenotypeMember"
         description: MUST be "GenotypeMember".
@@ -549,15 +575,53 @@
           The number of copies of the `variation` at a :ref:`Genotype` locus.
       variation:
         oneOf:
           - $ref: "#/definitions/Allele"
           - $ref: "#/definitions/Haplotype"
         description: >-
           A :ref:`MolecularVariation` at a :ref:`Genotype` locus.
-    required: [ "count", "variation" ]
+    required: [ "type", "count", "variation" ]
+
+  # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+  # Feature
+
+  Feature:
+    description: >-
+      A named entity that can be mapped to a Location. Genes, protein domains,
+      exons, and chromosomes are some examples of common biological entities
+      that may be Features.
+    oneOf:
+      - $ref: "#/definitions/Gene"
+    discriminator:
+      propertyName: type
+    heritable_properties:
+      type:
+        type: string
+        description: >-
+          The Feature class type. MUST match child class type.
+    heritable_required: [ "type" ]
+
+  Gene:
+    inherits: Feature
+    description: >-
+      A reference to a Gene as defined by an authority. For human genes,
+      the use of `hgnc <https://registry.identifiers.org/registry/hgnc>`_
+      as the gene authority is RECOMMENDED.
+    type: object
+    properties:
+      type:
+        type: string
+        const: "Gene"
+        default: "Gene"
+        description: MUST be "Gene"
+      gene_id:
+        $ref: "#/definitions/CURIE"
+        description: >-
+          A CURIE reference to a Gene concept
+    required: [ "gene_id" ]
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # Numerics, Comparators, and Ranges
 
   Number:
     description: >-
       A simple integer value as a VRS class.
@@ -617,14 +681,23 @@
 
   # =============================================================================
   # BASIC TYPES (STRUCTURES)
   # These types do NOT have a VRS `type` attribute
   # These types are used solely within other definitions.
   # =============================================================================
 
+  CURIE:
+    description: >-
+      A `W3C Compact URI <https://www.w3.org/TR/curie/>`_ formatted string.
+      A CURIE string has the structure ``prefix``:``reference``, as defined by
+      the W3C syntax.
+    type: string
+    pattern: '^\w[^:]*:.+$'
+    example: "ensembl:ENSG00000139618"
+
   HumanCytoband:
     description: >-
       A character string representing cytobands derived from the
       *International System for Human Cytogenomic Nomenclature* (ISCN)
       `guidelines <http://doi.org/10.1159/isbn.978-3-318-06861-0>`_.
     type: string
     pattern: '^cen|[pq](ter|([1-9][0-9]*(\.[1-9][0-9]*)?))$'
@@ -643,7 +716,60 @@
     description: >-
       A character string of :ref:`Residues <Residue>` that represents a biological
       sequence using the conventional sequence order (5’-to-3’ for
       nucleic acid sequences, and amino-to-carboxyl for amino acid
       sequences). IUPAC ambiguity codes are permitted in Sequences.
     type: string
     pattern: '^[A-Z*\-]*$'
+
+
+  # =============================================================================
+  # DEPRECATED
+  # =============================================================================
+
+  SequenceState:
+    deprecated: true
+    description: >-
+      DEPRECATED. A :ref:`Sequence` as a :ref:`State`. This is the State class
+      to use for representing "ref-alt" style variation, including SNVs, MNVs,
+      del, ins, and delins.
+      This class is deprecated. Use :ref:`LiteralSequenceExpression` instead.
+    type: object
+    properties:
+      type:
+        type: string
+        const: "SequenceState"
+        default: "SequenceState"
+        description: MUST be "SequenceState"
+      sequence:
+        $ref: "#/definitions/Sequence"
+        description: A string of :ref:`Residues <Residue>`
+    example:
+      type: SequenceState
+      sequence: C
+    required: [ "type", "sequence" ]
+
+  SimpleInterval:
+    deprecated: true
+    description: >-
+      DEPRECATED: A SimpleInterval represents a span of sequence. Positions are
+      always represented by contiguous spans using interbase coordinates.
+
+      This class is deprecated. Use SequenceInterval instead.
+    type: object
+    properties:
+      type:
+        type: string
+        const: "SimpleInterval"
+        default: "SimpleInterval"
+        description: MUST be "SimpleInterval"
+      start:
+        type: integer
+        description: The start coordinate
+      end:
+        type: integer
+        description: The end coordinate
+    example:
+      type: SimpleInterval
+      start: 11
+      end: 22
+    required: [ "type", "start", "end" ]
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/tests/data/vrs.yaml` & `ga4gh.gks.metaschema-0.2.0rc5/tests/data/vrs1.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 $schema: http://json-schema.org/draft-07/schema
 title: GA4GH-VRS-Definitions
 type: object
 definitions:
   Variation:
     description: A representation of the state of one or more biomolecules.
     oneOf:
-    - $ref: '#/definitions/MolecularVariation'
-    - $ref: '#/definitions/SystemicVariation'
-    - $ref: '#/definitions/UtilityVariation'
+    - $ref: '#/definitions/AbsoluteCopyNumber'
+    - $ref: '#/definitions/Allele'
+    - $ref: '#/definitions/Genotype'
+    - $ref: '#/definitions/Haplotype'
+    - $ref: '#/definitions/RelativeCopyNumber'
+    - $ref: '#/definitions/Text'
+    - $ref: '#/definitions/VariationSet'
     discriminator:
       propertyName: type
   MolecularVariation:
     description: A variation on a contiguous molecule.
     oneOf:
     - $ref: '#/definitions/Allele'
     - $ref: '#/definitions/Haplotype'
@@ -26,354 +30,364 @@
     - $ref: '#/definitions/VariationSet'
     discriminator:
       propertyName: type
   SystemicVariation:
     description: A Variation of multiple molecules in the context of a system, e.g.
       a genome, sample, or homologous chromosomes.
     oneOf:
-    - $ref: '#/definitions/Genotype'
     - $ref: '#/definitions/AbsoluteCopyNumber'
+    - $ref: '#/definitions/Genotype'
     - $ref: '#/definitions/RelativeCopyNumber'
     discriminator:
       propertyName: type
   Allele:
-    ga4gh_prefix: VA
     description: The state of a molecule at a Location.
     type: object
     properties:
-      id:
-        $ref: core.json#/$defs/CURIE
-        description: The 'logical' identifier of the entity in the system of record,
-          and MUST be represented as a CURIE. This 'id' is unique within a given system,
-          but may also refer to an 'id' for the shared concept in  another system
-          (represented by namespace, accordingly).
+      _id:
+        $ref: '#/definitions/CURIE'
+        description: Variation Id. MUST be unique within document.
       type:
         type: string
         const: Allele
         default: Allele
         description: MUST be "Allele"
       location:
         oneOf:
+        - $ref: '#/definitions/CURIE'
         - $ref: '#/definitions/ChromosomeLocation'
         - $ref: '#/definitions/SequenceLocation'
-        - $ref: core.json#/$defs/CURIE
         description: Where Allele is located
       state:
-        description: An expression of the sequence state
         oneOf:
         - $ref: '#/definitions/ComposedSequenceExpression'
         - $ref: '#/definitions/DerivedSequenceExpression'
         - $ref: '#/definitions/LiteralSequenceExpression'
         - $ref: '#/definitions/RepeatedSequenceExpression'
+        - $ref: '#/definitions/SequenceState'
+        description: An expression of the sequence state
+        deprecated:
+        - $ref: '#/definitions/SequenceState'
     required:
     - location
     - state
     - type
     additionalProperties: false
   Haplotype:
-    ga4gh_prefix: HT
     description: A set of non-overlapping Allele members that co-occur on the same
       molecule.
     type: object
     properties:
-      id:
-        $ref: core.json#/$defs/CURIE
-        description: The 'logical' identifier of the entity in the system of record,
-          and MUST be represented as a CURIE. This 'id' is unique within a given system,
-          but may also refer to an 'id' for the shared concept in  another system
-          (represented by namespace, accordingly).
+      _id:
+        $ref: '#/definitions/CURIE'
+        description: Variation Id. MUST be unique within document.
       type:
         type: string
         const: Haplotype
         default: Haplotype
         description: MUST be "Haplotype"
       members:
         type: array
-        ordered: false
         minItems: 2
         uniqueItems: true
+        ordered: false
         items:
           oneOf:
           - $ref: '#/definitions/Allele'
-          - $ref: core.json#/$defs/CURIE
+          - $ref: '#/definitions/CURIE'
         description: List of Alleles, or references to Alleles, that comprise this
           Haplotype.
     required:
     - members
     - type
     additionalProperties: false
   Text:
-    ga4gh_prefix: VT
     description: A free-text definition of variation.
     type: object
     properties:
-      id:
-        $ref: core.json#/$defs/CURIE
-        description: The 'logical' identifier of the entity in the system of record,
-          and MUST be represented as a CURIE. This 'id' is unique within a given system,
-          but may also refer to an 'id' for the shared concept in  another system
-          (represented by namespace, accordingly).
+      _id:
+        $ref: '#/definitions/CURIE'
+        description: Variation Id. MUST be unique within document.
       type:
         type: string
         const: Text
         default: Text
         description: MUST be "Text"
       definition:
         type: string
         description: A textual representation of variation not representable by other
           subclasses of Variation.
     required:
     - definition
     - type
     additionalProperties: false
   VariationSet:
-    ga4gh_prefix: VS
     description: An unconstrained set of Variation members.
     type: object
     properties:
-      id:
-        $ref: core.json#/$defs/CURIE
-        description: The 'logical' identifier of the entity in the system of record,
-          and MUST be represented as a CURIE. This 'id' is unique within a given system,
-          but may also refer to an 'id' for the shared concept in  another system
-          (represented by namespace, accordingly).
+      _id:
+        $ref: '#/definitions/CURIE'
+        description: Variation Id. MUST be unique within document.
       type:
         type: string
         const: VariationSet
         default: VariationSet
         description: MUST be "VariationSet"
       members:
         type: array
-        ordered: false
         uniqueItems: true
+        ordered: false
         items:
           oneOf:
           - $ref: '#/definitions/AbsoluteCopyNumber'
           - $ref: '#/definitions/Allele'
+          - $ref: '#/definitions/CURIE'
           - $ref: '#/definitions/Genotype'
           - $ref: '#/definitions/Haplotype'
           - $ref: '#/definitions/RelativeCopyNumber'
           - $ref: '#/definitions/Text'
           - $ref: '#/definitions/VariationSet'
-          - $ref: core.json#/$defs/CURIE
         description: List of Variation objects or identifiers. Attribute is required,
           but MAY be empty.
     required:
     - members
     - type
     additionalProperties: false
   AbsoluteCopyNumber:
-    ga4gh_prefix: ACN
     type: object
-    description: The absolute count of discrete copies of a MolecularVariation, Feature,
-      SequenceExpression, or a CURIE reference within a system (e.g. genome, cell,
-      etc.).
-    properties:
-      id:
-        $ref: core.json#/$defs/CURIE
-        description: The 'logical' identifier of the entity in the system of record,
-          and MUST be represented as a CURIE. This 'id' is unique within a given system,
-          but may also refer to an 'id' for the shared concept in  another system
-          (represented by namespace, accordingly).
+    maturity: draft
+    description: The absolute count of discrete copies of a Location, within a system
+      (e.g. genome, cell, etc.).
+    properties:
+      _id:
+        $ref: '#/definitions/CURIE'
+        description: Variation Id. MUST be unique within document.
       type:
         type: string
         const: AbsoluteCopyNumber
         default: AbsoluteCopyNumber
-        description: MUST be "AbsoluteCopyNumber".
-      location:
+        description: MUST be "AbsoluteCopyNumber"
+      subject:
         oneOf:
+        - $ref: '#/definitions/CURIE'
         - $ref: '#/definitions/ChromosomeLocation'
         - $ref: '#/definitions/SequenceLocation'
-        - $ref: core.json#/$defs/CURIE
-        description: The location within the system.
+        description: A location for which the number of systemic copies is described.
       copies:
         oneOf:
         - $ref: '#/definitions/DefiniteRange'
         - $ref: '#/definitions/IndefiniteRange'
         - $ref: '#/definitions/Number'
-        description: The integral number of copies of the subject in a system.
+        description: The integral number of copies of the subject in a system
     required:
     - copies
-    - location
+    - subject
     - type
     additionalProperties: false
   RelativeCopyNumber:
-    ga4gh_prefix: RCN
     type: object
     maturity: draft
-    description: The relative copies of a MolecularVariation, Feature, SequenceExpression,
-      or a CURIE reference against an unspecified baseline in a system (e.g. genome,
-      cell, etc.).
-    properties:
-      id:
-        $ref: core.json#/$defs/CURIE
-        description: The 'logical' identifier of the entity in the system of record,
-          and MUST be represented as a CURIE. This 'id' is unique within a given system,
-          but may also refer to an 'id' for the shared concept in  another system
-          (represented by namespace, accordingly).
+    description: The copies of a Location within a system (e.g. genome, cell, etc.)
+      relative to a baseline state.
+    properties:
+      _id:
+        $ref: '#/definitions/CURIE'
+        description: Variation Id. MUST be unique within document.
       type:
         type: string
         const: RelativeCopyNumber
         default: RelativeCopyNumber
         description: MUST be "RelativeCopyNumber"
-      location:
+      subject:
         oneOf:
+        - $ref: '#/definitions/CURIE'
         - $ref: '#/definitions/ChromosomeLocation'
         - $ref: '#/definitions/SequenceLocation'
-        - $ref: core.json#/$defs/CURIE
-        description: The location within the system.
+        description: A location for which the number of systemic copies is described.
       relative_copy_class:
         type: string
         enum:
         - complete loss
         - partial loss
         - copy neutral
         - low-level gain
         - high-level gain
         description: MUST be one of "complete loss", "partial loss", "copy neutral",
           "low-level gain" or "high-level gain".
     required:
-    - location
     - relative_copy_class
+    - subject
     - type
     additionalProperties: false
   Genotype:
-    ga4gh_prefix: GT
-    description: A quantified set of _in-trans_ MolecularVariation at a genomic locus.
+    description: A quantified set of MolecularVariation associated with a genomic
+      locus.
     type: object
     properties:
-      id:
-        $ref: core.json#/$defs/CURIE
-        description: The 'logical' identifier of the entity in the system of record,
-          and MUST be represented as a CURIE. This 'id' is unique within a given system,
-          but may also refer to an 'id' for the shared concept in  another system
-          (represented by namespace, accordingly).
+      _id:
+        $ref: '#/definitions/CURIE'
+        description: Variation Id. MUST be unique within document.
       type:
         type: string
         const: Genotype
         default: Genotype
         description: MUST be "Genotype"
       members:
         type: array
-        ordered: false
         uniqueItems: true
         minItems: 1
+        ordered: false
         items:
           $ref: '#/definitions/GenotypeMember'
         description: Each GenotypeMember in `members` describes a MolecularVariation
           and the count of that variation at the locus.
       count:
         oneOf:
         - $ref: '#/definitions/DefiniteRange'
         - $ref: '#/definitions/IndefiniteRange'
         - $ref: '#/definitions/Number'
         description: The total number of copies of all MolecularVariation at this
-          locus, MUST be greater than or equal to the sum of GenotypeMember copy counts.
-          If greater than the total counts, this implies additional  MolecularVariation
-          that are expected to exist but are not explicitly indicated.
+          locus, MUST be greater than or equal to the sum of GenotypeMember copy counts
+          and MUST be greater than or equal to 1. If greater than the total of GenotypeMember
+          counts, this field describes  additional MolecularVariation that exist but
+          are not  explicitly described.
     required:
     - count
     - members
     - type
     additionalProperties: false
   Location:
     description: A contiguous segment of a biological sequence.
     oneOf:
     - $ref: '#/definitions/ChromosomeLocation'
     - $ref: '#/definitions/SequenceLocation'
     discriminator:
       propertyName: type
   ChromosomeLocation:
-    ga4gh_prefix: CL
     description: A Location on a chromosome defined by a species and chromosome name.
     type: object
     properties:
-      id:
-        $ref: core.json#/$defs/CURIE
-        description: The 'logical' identifier of the entity in the system of record,
-          and MUST be represented as a CURIE. This 'id' is unique within a given system,
-          but may also refer to an 'id' for the shared concept in  another system
-          (represented by namespace, accordingly).
+      _id:
+        $ref: '#/definitions/CURIE'
+        description: Location Id. MUST be unique within document.
       type:
         type: string
         const: ChromosomeLocation
         default: ChromosomeLocation
         description: MUST be "ChromosomeLocation"
       species_id:
+        $ref: '#/definitions/CURIE'
         default: taxonomy:9606
         description: 'CURIE representing a species from the [NCBI species taxonomy](https://registry.identifiers.org/registry/taxonomy).
           Default: "taxonomy:9606" (human)'
-        $ref: core.json#/$defs/CURIE
       chr:
         type: string
         description: The symbolic chromosome name. For humans, For humans, chromosome
           names MUST be one of 1..22, X, Y (case-sensitive)
-      start:
-        $ref: '#/definitions/HumanCytoband'
-        description: The start cytoband region. MUST specify a region nearer the terminal
-          end (telomere) of the chromosome p-arm than `end`.
-      end:
-        $ref: '#/definitions/HumanCytoband'
-        description: The start cytoband region. MUST specify a region nearer the terminal
-          end (telomere) of the chromosome q-arm than `start`.
+      interval:
+        $ref: '#/definitions/CytobandInterval'
+        description: The chromosome region defined by a CytobandInterval
     required:
     - chr
-    - end
+    - interval
     - species_id
-    - start
     - type
     additionalProperties: false
   SequenceLocation:
-    ga4gh_prefix: SL
     description: A Location defined by an interval on a referenced Sequence.
     type: object
     properties:
-      id:
-        $ref: core.json#/$defs/CURIE
-        description: The 'logical' identifier of the entity in the system of record,
-          and MUST be represented as a CURIE. This 'id' is unique within a given system,
-          but may also refer to an 'id' for the shared concept in  another system
-          (represented by namespace, accordingly).
+      _id:
+        $ref: '#/definitions/CURIE'
+        description: Location Id. MUST be unique within document.
       type:
         type: string
         const: SequenceLocation
         default: SequenceLocation
         description: MUST be "SequenceLocation"
       sequence_id:
+        $ref: '#/definitions/CURIE'
         description: A VRS Computed Identifier for the reference Sequence.
-        $ref: core.json#/$defs/CURIE
+      interval:
+        oneOf:
+        - $ref: '#/definitions/SequenceInterval'
+        - $ref: '#/definitions/SimpleInterval'
+        description: Reference sequence region defined by a SequenceInterval.
+    required:
+    - interval
+    - sequence_id
+    - type
+    additionalProperties: false
+  SequenceInterval:
+    description: A SequenceInterval represents a span on a Sequence. Positions are
+      always represented by contiguous spans using interbase coordinates or coordinate
+      ranges.
+    type: object
+    properties:
+      type:
+        type: string
+        const: SequenceInterval
+        default: SequenceInterval
+        description: MUST be "SequenceInterval"
       start:
         oneOf:
         - $ref: '#/definitions/DefiniteRange'
         - $ref: '#/definitions/IndefiniteRange'
         - $ref: '#/definitions/Number'
-        description: The start coordinate or range of the SequenceLocation. The minimum
-          value of this coordinate or range is 0. MUST represent a coordinate or range
-          less than the value of `end`.
+        description: The start coordinate or range of the interval. The minimum value
+          of this coordinate or range is 0. MUST represent a coordinate or range less
+          than the value of `end`.
       end:
         oneOf:
         - $ref: '#/definitions/DefiniteRange'
         - $ref: '#/definitions/IndefiniteRange'
         - $ref: '#/definitions/Number'
-        description: The end coordinate or range of the SequenceLocation. The minimum
-          value of this coordinate or range is 0. MUST represent a coordinate or range
-          greater than the value of `start`.
+        description: The end coordinate or range of the interval. The minimum value
+          of this coordinate or range is 0. MUST represent a coordinate or range greater
+          than the value of `start`.
+    required:
+    - end
+    - start
+    - type
+    additionalProperties: false
+  CytobandInterval:
+    description: A contiguous span on a chromosome defined by cytoband features. The
+      span includes the constituent regions described by the start and end cytobands,
+      as well as any intervening regions.
+    type: object
+    properties:
+      type:
+        type: string
+        const: CytobandInterval
+        default: CytobandInterval
+        description: MUST be "CytobandInterval"
+      start:
+        $ref: '#/definitions/HumanCytoband'
+        description: The start cytoband region. MUST specify a region nearer the terminal
+          end (telomere) of the chromosome p-arm than `end`.
+      end:
+        $ref: '#/definitions/HumanCytoband'
+        description: The start cytoband region. MUST specify a region nearer the terminal
+          end (telomere) of the chromosome q-arm than `start`.
+    example:
+      type: CytobandInterval
+      start: q22.2
+      end: q22.3
     required:
     - end
-    - sequence_id
     - start
     - type
     additionalProperties: false
   SequenceExpression:
     description: An expression describing a Sequence.
     oneOf:
-    - $ref: '#/definitions/LiteralSequenceExpression'
+    - $ref: '#/definitions/ComposedSequenceExpression'
     - $ref: '#/definitions/DerivedSequenceExpression'
+    - $ref: '#/definitions/LiteralSequenceExpression'
     - $ref: '#/definitions/RepeatedSequenceExpression'
-    - $ref: '#/definitions/ComposedSequenceExpression'
     discriminator:
       propertyName: type
   LiteralSequenceExpression:
     description: An explicit expression of a Sequence.
     type: object
     properties:
       type:
@@ -429,47 +443,14 @@
         description: An expression of the repeating subsequence
       count:
         oneOf:
         - $ref: '#/definitions/DefiniteRange'
         - $ref: '#/definitions/IndefiniteRange'
         - $ref: '#/definitions/Number'
         description: The count of repeated units, as an integer or inclusive range
-    allOf:
-    - if:
-        properties:
-          count:
-            $ref: '#/definitions/Number'
-      then:
-        properties:
-          count:
-            properties:
-              value:
-                minimum: 0
-    - if:
-        properties:
-          count:
-            $ref: '#/definitions/IndefiniteRange'
-      then:
-        properties:
-          count:
-            properties:
-              value:
-                minimum: 0
-    - if:
-        properties:
-          count:
-            $ref: '#/definitions/DefiniteRange'
-      then:
-        properties:
-          count:
-            properties:
-              min:
-                minimum: 0
-              max:
-                minimum: 0
     required:
     - count
     - seq_expr
     - type
     additionalProperties: false
   ComposedSequenceExpression:
     description: An expression of a sequence composed from multiple other Sequence
@@ -481,29 +462,33 @@
       type:
         type: string
         const: ComposedSequenceExpression
         default: ComposedSequenceExpression
         description: MUST be "ComposedSequenceExpression"
       components:
         type: array
-        ordered: true
         uniqueItems: true
         minItems: 2
+        ordered: true
         items:
-          anyOf:
+          oneOf:
+          - $ref: '#/definitions/DerivedSequenceExpression'
           - $ref: '#/definitions/LiteralSequenceExpression'
           - $ref: '#/definitions/RepeatedSequenceExpression'
+        contains:
+          oneOf:
+          - $ref: '#/definitions/RepeatedSequenceExpression'
           - $ref: '#/definitions/DerivedSequenceExpression'
-        description: An ordered list of SequenceExpression components comprising the
-          expression. MUST NOT have two adjacent LiteralSequenceExpression objects.
+        description: An ordered list of SequenceExpression components   comprising
+          the expression.
     required:
     - components
   GenotypeMember:
     description: A class for expressing the count of a specific MolecularVariation
-      present _in-trans_ at a genomic locus represented by a Genotype.
+      present *in-trans* at a genomic locus represented by a Genotype.
     type: object
     properties:
       type:
         type: string
         const: GenotypeMember
         default: GenotypeMember
         description: MUST be "GenotypeMember".
@@ -516,16 +501,43 @@
       variation:
         oneOf:
         - $ref: '#/definitions/Allele'
         - $ref: '#/definitions/Haplotype'
         description: A MolecularVariation at a Genotype locus.
     required:
     - count
+    - type
     - variation
     additionalProperties: false
+  Feature:
+    description: A named entity that can be mapped to a Location. Genes, protein domains,
+      exons, and chromosomes are some examples of common biological entities that
+      may be Features.
+    oneOf:
+    - $ref: '#/definitions/Gene'
+    discriminator:
+      propertyName: type
+  Gene:
+    description: A reference to a Gene as defined by an authority. For human genes,
+      the use of [hgnc](https://registry.identifiers.org/registry/hgnc) as the gene
+      authority is RECOMMENDED.
+    type: object
+    properties:
+      type:
+        type: string
+        const: Gene
+        default: Gene
+        description: MUST be "Gene"
+      gene_id:
+        $ref: '#/definitions/CURIE'
+        description: A CURIE reference to a Gene concept
+    required:
+    - gene_id
+    - type
+    additionalProperties: false
   Number:
     description: A simple integer value as a VRS class.
     type: object
     properties:
       type:
         type: string
         const: Number
@@ -581,14 +593,21 @@
         description: MUST be one of "<=" or ">=", indicating which direction the range
           is indefinite
     required:
     - comparator
     - type
     - value
     additionalProperties: false
+  CURIE:
+    description: A [W3C Compact URI](https://www.w3.org/TR/curie/) formatted string.
+      A CURIE string has the structure ``prefix``:``reference``, as defined by the
+      W3C syntax.
+    type: string
+    pattern: ^\w[^:]*:.+$
+    example: ensembl:ENSG00000139618
   HumanCytoband:
     description: A character string representing cytobands derived from the *International
       System for Human Cytogenomic Nomenclature* (ISCN) [guidelines](http://doi.org/10.1159/isbn.978-3-318-06861-0).
     type: string
     pattern: ^cen|[pq](ter|([1-9][0-9]*(\.[1-9][0-9]*)?))$
     example: q22.3
   Residue:
@@ -600,7 +619,56 @@
   Sequence:
     description: "A character string of Residues that represents a biological sequence\
       \ using the conventional sequence order (5\u2019-to-3\u2019 for nucleic acid\
       \ sequences, and amino-to-carboxyl for amino acid sequences). IUPAC ambiguity\
       \ codes are permitted in Sequences."
     type: string
     pattern: ^[A-Z*\-]*$
+  SequenceState:
+    deprecated: true
+    description: DEPRECATED. A Sequence as a State. This is the State class to use
+      for representing "ref-alt" style variation, including SNVs, MNVs, del, ins,
+      and delins. This class is deprecated. Use LiteralSequenceExpression instead.
+    type: object
+    properties:
+      type:
+        type: string
+        const: SequenceState
+        default: SequenceState
+        description: MUST be "SequenceState"
+      sequence:
+        $ref: '#/definitions/Sequence'
+        description: A string of Residues
+    example:
+      type: SequenceState
+      sequence: C
+    required:
+    - sequence
+    - type
+    additionalProperties: false
+  SimpleInterval:
+    deprecated: true
+    description: 'DEPRECATED: A SimpleInterval represents a span of sequence. Positions
+      are always represented by contiguous spans using interbase coordinates. This
+      class is deprecated. Use SequenceInterval instead.'
+    type: object
+    properties:
+      type:
+        type: string
+        const: SimpleInterval
+        default: SimpleInterval
+        description: MUST be "SimpleInterval"
+      start:
+        type: integer
+        description: The start coordinate
+      end:
+        type: integer
+        description: The end coordinate
+    example:
+      type: SimpleInterval
+      start: 11
+      end: 22
+    required:
+    - end
+    - start
+    - type
+    additionalProperties: false
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/tests/data/vrs1-source.yaml` & `ga4gh.gks.metaschema-0.2.0rc5/tests/data/vrs-source.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -4,772 +4,774 @@
 #   make vrs.json
 # You'll probably have to `pip install pyyaml` first.
 #
 # To watch for changes and update automatically:
 #   make watch &
 
 # https://json-schema.org/understanding-json-schema/reference/schema.html
-$schema: "http://json-schema.org/draft-07/schema"
+$schema: "http://json-schema.org/draft/2020-12/schema"
 title: "GA4GH-VRS-Definitions"
 type: object
 strict: true
 
-definitions:
+imports:
+  gks.core: core-source.yaml
+
+namespaces:
+  gks.core: core.json#/$defs/
+
+$defs:
   # VRS definitions are presented top-down.  Everything rolls up to
   # Variation, which is a polymorphic abstraction of many kinds of
   # variation.
 
   # =============================================================================
   # Kinds of Variation
   # =============================================================================
 
+  ValueObject:
+    inherits: gks.core:Entity
+    ga4ghDigest:
+      keys:
+        - type
+    description: >-
+      An object whose equality is based on value, not identity. All VRS Value Objects
+      may have computed digests from the VRS Computed Identifier algorithm.
+      See https://en.wikipedia.org/wiki/Value_object for more on Value Objects.
+    heritable_properties:
+      type:
+        type: string
+      digest:
+        description: A sha512t24u digest created using the VRS Computed Identifier algorithm.
+        type: string
+        pattern: '[0-9A-Za-z_\-]{32}'
+    heritable_required:
+      - type
+
+  # TODO: Draft recomposition of Allele as "AlleleMember" plus seq requirement
+  # TODO: Explore "typed entity"
+
   Variation:
+    inherits: ValueObject
     description: >-
       A representation of the state of one or more biomolecules.
     oneOf:
-      - $ref: "#/definitions/MolecularVariation"
-      - $ref: "#/definitions/SystemicVariation"
-      - $ref: "#/definitions/UtilityVariation"
-    heritable_properties:
-      _id:
-        $ref: "#/definitions/CURIE"
-        description: >-
-          Variation Id. MUST be unique within document.
-      type:
-        type: string
-        description: >-
-          The Variation class type. MUST match child class type.
-    heritable_required: ["type"]
+      - $ref: "#/$defs/MolecularVariation"
+      - $ref: "#/$defs/SystemicVariation"
+#      - $ref: "#/$defs/UtilityVariation"
 
     discriminator:
       propertyName: type
 
   MolecularVariation:
     inherits: Variation
     description: >-
       A :ref:`variation` on a contiguous molecule.
     oneOf:
-      - $ref: "#/definitions/Allele"
-      - $ref: "#/definitions/Haplotype"
+      - $ref: "#/$defs/Allele"
+      - $ref: "#/$defs/Haplotype"
     discriminator:
       propertyName: type
 
-  UtilityVariation:
-    inherits: Variation
-    description: >-
-      A collection of :ref:`Variation` subclasses that cannot be
-      constrained to a specific class of biological variation, but
-      are necessary for some applications of VRS.
-    oneOf:
-      - $ref: "#/definitions/Text"
-      - $ref: "#/definitions/VariationSet"
-    discriminator:
-      propertyName: type
+#  UtilityVariation:
+#    inherits: Variation
+#    description: >-
+#      A collection of :ref:`Variation` subclasses that cannot be
+#      constrained to a specific class of biological variation, but
+#      are necessary for some applications of VRS.
+#    oneOf:
+#      - $ref: "#/$defs/Text"
+#      - $ref: "#/$defs/VariationSet"
+#    discriminator:
+#      propertyName: type
 
   SystemicVariation:
     inherits: Variation
     description: >-
       A Variation of multiple molecules in the context of a system, e.g.
       a genome, sample, or homologous chromosomes.
     oneOf:
-      - $ref: "#/definitions/CopyNumber"
-      - $ref: "#/definitions/Genotype"
+      - $ref: "#/$defs/Genotype"
+      - $ref: "#/$defs/CopyNumberCount"
+      - $ref: "#/$defs/CopyNumberChange"
     discriminator:
       propertyName: type
 
   # =============================================================================
   # IDENTIFIABLE TYPES
   # Have a `type` and `_id` attribute
   # =============================================================================
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # Molecular Variation
 
   Allele:
+    maturity: Alpha
+    ga4ghDigest:
+      prefix: VA
+      keys:
+        - location
+        - state
     inherits: MolecularVariation
     description: >-
       The state of a molecule at a :ref:`Location`.
     type: object
     properties:
       type:
         type: string
         const: "Allele"
         default: "Allele"
         description: >-
           MUST be "Allele"
       location:
         oneOf:
-          - $ref: "#/definitions/CURIE"
-          - $ref: "#/definitions/Location"
+          - $ref_curie: gks.core:IRI
+          - $ref: "#/$defs/Location"
         description: >-
-          Where Allele is located
+          The location of the Allele
       state:
-        oneOf:
-          - $ref: "#/definitions/SequenceExpression"
-          - $ref: "#/definitions/SequenceState" # DEPRECATED; remove in 2.0
+        $ref: "#/$defs/SequenceExpression"
         description: >-
           An expression of the sequence state
-        deprecated:
-          - $ref: "#/definitions/SequenceState"
     required: [ "location", "state" ]
 
   Haplotype:
+    maturity: Alpha
+    ga4ghDigest:
+      prefix: HT
+      keys:
+        - members
     inherits: MolecularVariation
     description: >-
       A set of non-overlapping :ref:`Allele` members that co-occur on the same molecule.
     type: "object"
     properties:
       type:
         type: string
         const: "Haplotype"
         default: "Haplotype"
         description: >-
           MUST be "Haplotype"
       members:
         type: array
+        ordered: false
         minItems: 2
         uniqueItems: true
-        ordered: false
         items:
           oneOf:
-            - $ref: "#/definitions/Allele"
-            - $ref: "#/definitions/CURIE"
+            - $ref: "#/$defs/Allele"
+            - $ref_curie: gks.core:IRI
         description: >-
           List of Alleles, or references to Alleles, that comprise this Haplotype.
     required: [ "members" ]
 
-
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # UtilityVariation
 
-  Text:
-    inherits: UtilityVariation
-    description: >-
-      A free-text definition of variation.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "Text"
-        default: "Text"
-        description: MUST be "Text"
-      definition:
-        type: string
-        description: >-
-          A textual representation of variation not representable by
-          other subclasses of Variation.
-    required: [ "definition" ]
-
-  VariationSet:
-    inherits: UtilityVariation
-    description: >-
-      An unconstrained set of Variation members.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "VariationSet"
-        default: "VariationSet"
-        description: MUST be "VariationSet"
-      members:
-        type: array
-        uniqueItems: true
-        ordered: false
-        items:
-          oneOf:
-            - $ref: "#/definitions/CURIE"
-            - $ref: "#/definitions/Variation"
-        description: >-
-          List of Variation objects or identifiers. Attribute is
-          required, but MAY be empty.
-    required: [ "members" ]
+#  Text:
+#    ga4ghPrefix: VT
+#    inherits: UtilityVariation
+#    description: >-
+#      A free-text definition of variation.
+#    type: object
+#    properties:
+#      type:
+#        type: string
+#        const: "Text"
+#        default: "Text"
+#        description: MUST be "Text"
+#      definition:
+#        type: string
+#        description: >-
+#          A textual representation of variation not representable by
+#          other subclasses of Variation.
+#    required: [ "definition" ]
+#
+#  VariationSet:
+#    ga4ghPrefix: VS
+#    inherits: UtilityVariation
+#    description: >-
+#      An unconstrained set of Variation members.
+#    type: object
+#    properties:
+#      type:
+#        type: string
+#        const: "VariationSet"
+#        default: "VariationSet"
+#        description: MUST be "VariationSet"
+#      members:
+#        type: array
+#        ordered: false
+#        uniqueItems: true
+#        items:
+#          oneOf:
+#            - $ref_curie: gks.core:IRI
+#            - $ref: "#/$defs/Variation"
+#        description: >-
+#          List of Variation objects or identifiers. Attribute is
+#          required, but MAY be empty.
+#    required: [ "members" ]
 
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # SystemicVariation
 
   CopyNumber:
+    ga4ghDigest:
+      keys:
+        - subject
     inherits: SystemicVariation
     description: >-
-      The copies of :ref:`Location` in a system, expressed as an absolute integer
-      quantity (:ref:`AbsoluteCopyNumber`) or a qualitative description of copies 
-      relative to a baseline state (:ref:`RelativeCopyNumber`).
+      A measure of the copies of a :ref:`Location` within a system (e.g. genome, cell, etc.)
     heritable_properties:
       subject:
         oneOf:
-          - $ref: "#/definitions/Location"
-          - $ref: "#/definitions/CURIE"
+          - $ref_curie: gks.core:IRI
+          - $ref: "#/$defs/Location"
         description: >-
           A location for which the number of systemic copies is described.
     heritable_required: [ "subject" ]
 
-  AbsoluteCopyNumber:
+  CopyNumberCount:
+    maturity: Alpha
+    ga4ghDigest:
+      keys:
+        - copies
+      prefix: CN
     inherits: CopyNumber
     type: object
-    maturity: draft
     description: >-
-      The absolute count of discrete copies of a :ref:`Location`,
+      The absolute count of discrete copies of a :ref:`Location` or :ref:`Gene`,
       within a system (e.g. genome, cell, etc.).
     properties:
       type:
         type: string
-        const: "AbsoluteCopyNumber"
-        default: "AbsoluteCopyNumber"
+        const: "CopyNumberCount"
+        default: "CopyNumberCount"
         description: >-
-          MUST be "AbsoluteCopyNumber"
+          MUST be "CopyNumberCount"
       copies:
         oneOf:
-          - $ref: "#/definitions/Number"
-          - $ref: "#/definitions/IndefiniteRange"
-          - $ref: "#/definitions/DefiniteRange"
+          - type: integer
+          - $ref: "#/$defs/Range"
         description: >-
           The integral number of copies of the subject in a system
     required: [ "copies" ]
 
-  RelativeCopyNumber:
+  CopyNumberChange:
+    maturity: Alpha
+    ga4ghDigest:
+      keys:
+        - copy_change
+      prefix: CX
     inherits: CopyNumber
     type: object
-    maturity: draft
     description: >-
-      The copies of a :ref:`Location` within a system (e.g. genome, cell, etc.)
-      relative to a baseline state.
+      An assessment of the copy number of a :ref:`Location` or a :ref:`Gene` within a system (e.g. genome, cell,
+      etc.) relative to a baseline ploidy.
     properties:
       type:
         type: string
-        const: "RelativeCopyNumber"
-        default: "RelativeCopyNumber"
+        const: "CopyNumberChange"
+        default: "CopyNumberChange"
         description: >-
-          MUST be "RelativeCopyNumber"
-      relative_copy_class:
+          MUST be "CopyNumberChange"
+      copy_change:
         type: string
-        enum: [ "complete loss", "partial loss", "copy neutral", "low-level gain", "high-level gain" ]
+        enum: [ "efo:0030069", "efo:0020073", "efo:0030068", "efo:0030067", "efo:0030064", "efo:0030070", "efo:0030071", "efo:0030072" ]
         description: >-
-          MUST be one of "complete loss", "partial loss", "copy neutral", "low-level gain" or "high-level gain".
-    required: [  "relative_copy_class" ]
+          MUST be one of "efo:0030069" (complete genomic loss), "efo:0020073" (high-level loss),
+          "efo:0030068" (low-level loss), "efo:0030067" (loss), "efo:0030064" (regional base ploidy),
+          "efo:0030070" (gain), "efo:0030071" (low-level gain), "efo:0030072" (high-level gain).
+    required: [ "copy_change" ]
 
   Genotype:
+    maturity: Alpha
+    ga4ghDigest:
+      keys:
+        - members
+        - count
+      prefix: GT
     inherits: SystemicVariation
     description: >-
-      A quantified set of :ref:`MolecularVariation` associated with a genomic locus.
+      A quantified set of _in-trans_ :ref:`MolecularVariation` at a genomic locus.
     type: object
     properties:
       type:
         type: string
         const: "Genotype"
         default: "Genotype"
         description: >-
           MUST be "Genotype"
       members:
         type: array
+        ordered: false
         uniqueItems: true
         minItems: 1
-        ordered: false
         items:
-          $ref: "#/definitions/GenotypeMember"
+          $ref: "#/$defs/GenotypeMember"
         description: >-
           Each GenotypeMember in `members` describes a :ref:`MolecularVariation`
           and the count of that variation at the locus.
       count:
         oneOf:
-          - $ref: "#/definitions/Number"
-          - $ref: "#/definitions/IndefiniteRange"
-          - $ref: "#/definitions/DefiniteRange"
+          - type: integer
+          - $ref: "#/$defs/Range"
         description: >-
           The total number of copies of all :ref:`MolecularVariation` at this locus,
-          MUST be greater than or equal to the sum of :ref:`GenotypeMember` copy counts
-          and MUST be greater than or equal to 1.
-          If greater than the total of GenotypeMember counts, this field describes 
-          additional :ref:`MolecularVariation` that exist but are not 
-          explicitly described.
+          MUST be greater than or equal to the sum of :ref:`GenotypeMember` copy counts.
+          If greater than the total counts, this implies additional
+          :ref:`MolecularVariation` that are expected to exist but are not explicitly
+          indicated.
     required: [ "members", "count" ]
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # Locations
 
   Location:
+    inherits: ValueObject
     description: >-
       A contiguous segment of a biological sequence.
     oneOf:
-      - $ref: "#/definitions/ChromosomeLocation"
-      - $ref: "#/definitions/SequenceLocation"
-    heritable_properties:
-      _id:
-        $ref: "#/definitions/CURIE"
-        description: >-
-          Location Id. MUST be unique within document.
-      type:
-        type: string
-        description: >-
-          The Location class type. MUST match child class type.
-    heritable_required: ["type"]
+#      - $ref: "#/$defs/ChromosomeLocation"
+      - $ref: "#/$defs/SequenceLocation"
     discriminator:
       propertyName: type
 
-  ChromosomeLocation:
-    inherits: Location
-    description: >-
-      A Location on a chromosome defined by a species and chromosome name.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "ChromosomeLocation"
-        default: "ChromosomeLocation"
-        description: MUST be "ChromosomeLocation"
-      species_id:
-        $ref: "#/definitions/CURIE"
-        default: "taxonomy:9606"
-        description: >-
-          :ref:`CURIE` representing a species from the
-          `NCBI species taxonomy <https://registry.identifiers.org/registry/taxonomy>`_.
-          Default: "taxonomy:9606" (human)
-      chr:
-        type: string
-        description: >-
-          The symbolic chromosome name. For humans, For humans,
-          chromosome names MUST be one of 1..22, X, Y (case-sensitive)
-      interval:
-        $ref: "#/definitions/CytobandInterval"
-        description: >-
-          The chromosome region defined by a :ref:`CytobandInterval`
-    required: [ "species_id", "chr", "interval" ]
+#  ChromosomeLocation:
+#    ga4ghPrefix: CL
+#    inherits: Location
+#    description: >-
+#      A Location on a chromosome defined by a species and chromosome name.
+#    type: object
+#    properties:
+#      type:
+#        type: string
+#        const: "ChromosomeLocation"
+#        default: "ChromosomeLocation"
+#        description: MUST be "ChromosomeLocation"
+#      species_id:
+#        $ref_curie: gks.core:IRI
+#        default: "taxonomy:9606"
+#        description: >-
+#          :ref:`CURIE` representing a species from the
+#          `NCBI species taxonomy <https://registry.identifiers.org/registry/taxonomy>`_.
+#          Default: "taxonomy:9606" (human)
+#      chr:
+#        type: string
+#        description: >-
+#          The symbolic chromosome name. For humans, For humans,
+#          chromosome names MUST be one of 1..22, X, Y (case-sensitive)
+#      start:
+#        $ref: "#/$defs/HumanCytoband"
+#        description: >-
+#          The start cytoband region. MUST specify a region nearer the
+#          terminal end (telomere) of the chromosome p-arm than `end`.
+#      end:
+#        $ref: "#/$defs/HumanCytoband"
+#        description: >-
+#          The start cytoband region. MUST specify a region nearer the
+#          terminal end (telomere) of the chromosome q-arm than `start`.
+#    required: [ "species_id", "chr", "start", "end" ]
 
   SequenceLocation:
+    maturity: Alpha
+    ga4ghDigest:
+      keys:
+        - members
+        - count
+      prefix: SL
     inherits: Location
     description: >-
       A :ref:`Location` defined by an interval on a referenced :ref:`Sequence`.
     type: object
     properties:
       type:
         type: string
         const: "SequenceLocation"
         default: "SequenceLocation"
         description: MUST be "SequenceLocation"
-      sequence_id:
-        $ref: "#/definitions/CURIE"
-        description: >-
-          A VRS :ref:`Computed Identifier <computed-identifiers>`
-          for the reference :ref:`Sequence`.
-      interval:
+      sequence:
         oneOf:
-          - $ref: "#/definitions/SequenceInterval"
-          - $ref: "#/definitions/SimpleInterval"
+          - $ref_curie: gks.core:IRI
+          - $ref: "#/$defs/SequenceReference"
         description: >-
-          Reference sequence region defined by a :ref:`SequenceInterval`.
-    required: [ "sequence_id", "interval" ]
-
-
-  # =============================================================================
-  # NON-IDENTIFIABLE TYPES
-  # These types have a `type` attribute
-  # =============================================================================
-
-  # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
-  # Intervals
-
-  SequenceInterval:
-    description: >-
-      A SequenceInterval represents a span on a :ref:`Sequence`. Positions are
-      always represented by contiguous spans using interbase coordinates or
-      coordinate ranges.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "SequenceInterval"
-        default: "SequenceInterval"
-        description: MUST be "SequenceInterval"
+          A :ref:`SequenceReference`.
       start:
         oneOf:
-          - $ref: "#/definitions/Number"
-          - $ref: "#/definitions/IndefiniteRange"
-          - $ref: "#/definitions/DefiniteRange"
+          - type: integer
+          - $ref: "#/$defs/Range"
         description: >-
-          The start coordinate or range of the interval.
+          The start coordinate or range of the SequenceLocation.
           The minimum value of this coordinate or range is 0.
           MUST represent a coordinate or range less than the value of `end`.
       end:
         oneOf:
-          - $ref: "#/definitions/Number"
-          - $ref: "#/definitions/IndefiniteRange"
-          - $ref: "#/definitions/DefiniteRange"
+          - type: integer
+          - $ref: "#/$defs/Range"
         description: >-
-          The end coordinate or range of the interval.
+          The end coordinate or range of the SequenceLocation.
           The minimum value of this coordinate or range is 0.
           MUST represent a coordinate or range greater than the value of `start`.
-    required: [ "type", "start", "end" ]
-
-  # SimpleInterval has been moved to DEPRECATED section at bottom.
+    required: [ "start", "end" ]
 
-  CytobandInterval:
-    description: >-
-      A contiguous span on a chromosome defined by cytoband features.
-      The span includes the constituent regions described by the start and
-      end cytobands, as well as any intervening regions.
+  SequenceReference:
+    maturity: Alpha
+    inherits: ValueObject
+    ga4ghDigest:
+      prefix: SQR
+      keys:
+        - refgetAccession
     type: object
+    description: A sequence of nucleic or amino acid character codes.
     properties:
       type:
         type: string
-        const: "CytobandInterval"
-        default: "CytobandInterval"
-        description: MUST be "CytobandInterval"
-      start:
-        $ref: "#/definitions/HumanCytoband"
-        description: >-
-          The start cytoband region. MUST specify a region nearer the
-          terminal end (telomere) of the chromosome p-arm than `end`.
-      end:
-        $ref: "#/definitions/HumanCytoband"
-        description: >-
-          The start cytoband region. MUST specify a region nearer the
-          terminal end (telomere) of the chromosome q-arm than `start`.
-    example:
-      type: CytobandInterval
-      start: q22.2
-      end: q22.3
-    required: [ "type", "start", "end" ]
+        const: "Sequence"
+        default: "Sequence"
+        description: MUST be "Sequence"
+      refgetAccession:
+        description: A `GA4GH RefGet <http://samtools.github.io/hts-specs/refget.html>` identifier for the referenced sequence, using the sha512t24u digest.
+        type: string
+        pattern: 'SQ.[0-9A-Za-z_\-]{32}'
+      residueAlphabet:
+        type: string
+        enum:
+          - amino acid
+          - nucleic acid
+
+      #TODO: add VRSATILE
+      #TODO: implementation guidance: digest property is RefGet TRUNC512
 
+  # =============================================================================
+  # NON-IDENTIFIABLE TYPES
+  # These types have a `type` attribute
+  # =============================================================================
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # SequenceExpression
 
   SequenceExpression:
+    inherits: gks.core:Entity
     description: >-
       An expression describing a :ref:`Sequence`.
     oneOf:
-      - $ref: "#/definitions/LiteralSequenceExpression"
-      - $ref: "#/definitions/DerivedSequenceExpression"
-      - $ref: "#/definitions/RepeatedSequenceExpression"
-      - $ref: "#/definitions/ComposedSequenceExpression"
+      - $ref: "#/$defs/LiteralSequenceExpression"
+      - $ref: "#/$defs/ReferenceLengthExpression"
+#      - $ref: "#/$defs/DerivedSequenceExpression"
+#      - $ref: "#/$defs/RepeatedSequenceExpression"
+#      - $ref: "#/$defs/ComposedSequenceExpression"
     discriminator:
       propertyName: type
     heritable_properties:
       type:
         type: string
         description: >-
           The SequenceExpression class type. MUST match child class type.
-    heritable_required: ["type"]
+    heritable_required:
+      - type
 
-  LiteralSequenceExpression:
+  ReferenceLengthExpression:
+    maturity: Alpha
     inherits: SequenceExpression
     description: >-
-      An explicit expression of a Sequence.
+      An expression of a length of a sequence from a repeating reference.
     type: object
     properties:
       type:
         type: string
-        const: "LiteralSequenceExpression"
-        default: "LiteralSequenceExpression"
-        description: MUST be "LiteralSequenceExpression"
-      sequence:
-        $ref: "#/definitions/Sequence"
-        description: the literal :ref:`Sequence` expressed
-    required: [ "sequence" ]
-
-  DerivedSequenceExpression:
-    inherits: SequenceExpression
-    description: >-
-      An approximate expression of a sequence that is derived from
-      a referenced sequence location. Use of this class
-      indicates that the derived sequence is *approximately equivalent*
-      to the reference indicated, and is typically used for describing
-      large regions in contexts where the use of an approximate sequence
-      is inconsequential.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "DerivedSequenceExpression"
-        default: "DerivedSequenceExpression"
-        description: MUST be "DerivedSequenceExpression"
-      location:
-        $ref: "#/definitions/SequenceLocation"
+        const: "ReferenceLengthExpression"
+        default: "ReferenceLengthExpression"
+        description: MUST be "ReferenceLengthExpression"
+      length:
+        oneOf:
+          - type: integer
+          - $ref: "#/$defs/Range"
         description: >-
-          The location from which the approximate sequence is derived
-      reverse_complement:
-        type: boolean
+          The number of residues in the expressed sequence.
+      sequence:
+        $ref: "#/$defs/SequenceString"
+        description: the :ref:`Sequence` encoded by the Reference Length Expression.
+      repeatSubunitLength:
+        type: integer
         description: >-
-          A flag indicating if the expressed sequence is the reverse
-          complement of the sequence referred to by `location`
-    required: [ "location", "reverse_complement" ]
+          The number of residues in the repeat subunit.
+    required:
+      - length
 
-  RepeatedSequenceExpression:
+  LiteralSequenceExpression:
+    maturity: Alpha
     inherits: SequenceExpression
     description: >-
-      An expression of a sequence comprised of a tandem repeating subsequence.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "RepeatedSequenceExpression"
-        default: "RepeatedSequenceExpression"
-        description: MUST be "RepeatedSequenceExpression"
-      seq_expr:
-        oneOf:
-          - $ref: "#/definitions/LiteralSequenceExpression"
-          - $ref: "#/definitions/DerivedSequenceExpression"
-        description: >-
-          An expression of the repeating subsequence
-      count:
-        oneOf:
-          - $ref: "#/definitions/Number"
-          - $ref: "#/definitions/IndefiniteRange"
-          - $ref: "#/definitions/DefiniteRange"
-        description: >-
-          The count of repeated units, as an integer or inclusive range
-    required: [ "seq_expr", "count" ]
-
-  ComposedSequenceExpression:
-    description: >-
-      An expression of a sequence composed from multiple other
-      :ref:`Sequence Expressions<SequenceExpression>`
-      objects. MUST have at least one component that is not a
-      ref:`LiteralSequenceExpression`. CANNOT be composed from
-      nested composed sequence expressions.
-    additionalProperties: false
+      An explicit expression of a Sequence.
     type: object
     properties:
       type:
         type: string
-        const: "ComposedSequenceExpression"
-        default: "ComposedSequenceExpression"
-        description: MUST be "ComposedSequenceExpression"
-      components:
-        type: array
-        uniqueItems: true
-        minItems: 2
-        ordered: true
-        items:
-          oneOf:
-            - $ref: "#/definitions/LiteralSequenceExpression"
-            - $ref: "#/definitions/RepeatedSequenceExpression"
-            - $ref: "#/definitions/DerivedSequenceExpression"
-        contains:
-          oneOf:
-            - $ref: "#/definitions/RepeatedSequenceExpression"
-            - $ref: "#/definitions/DerivedSequenceExpression"
-        description: >-
-          An ordered list of :ref:`SequenceExpression` components  
-          comprising the expression.
-    required: [ "components" ]
+        const: "LiteralSequenceExpression"
+        default: "LiteralSequenceExpression"
+        description: MUST be "LiteralSequenceExpression"
+      sequence:
+        $ref: "#/$defs/SequenceString"
+        description: the literal sequence
+    required:
+      - sequence
+
+#  DerivedSequenceExpression:
+#    inherits: SequenceExpression
+#    description: >-
+#      An approximate expression of a sequence that is derived from
+#      a referenced sequence location. Use of this class
+#      indicates that the derived sequence is *approximately equivalent*
+#      to the reference indicated, and is typically used for describing
+#      large regions in contexts where the use of an approximate sequence
+#      is inconsequential.
+#    type: object
+#    properties:
+#      type:
+#        type: string
+#        const: "DerivedSequenceExpression"
+#        default: "DerivedSequenceExpression"
+#        description: MUST be "DerivedSequenceExpression"
+#      location:
+#        $ref: "#/$defs/SequenceLocation"
+#        description: >-
+#          The location from which the approximate sequence is derived
+#      reverse_complement:
+#        type: boolean
+#        description: >-
+#          A flag indicating if the expressed sequence is the reverse
+#          complement of the sequence referred to by `location`
+#    required: [ "location", "reverse_complement" ]
+#
+#  RepeatedSequenceExpression:
+#    inherits: SequenceExpression
+#    description: >-
+#      An expression of a sequence comprised of a tandem repeating subsequence.
+#    type: object
+#    properties:
+#      type:
+#        type: string
+#        const: "RepeatedSequenceExpression"
+#        default: "RepeatedSequenceExpression"
+#        description: MUST be "RepeatedSequenceExpression"
+#      seq_expr:
+#        oneOf:
+#          - $ref: "#/$defs/LiteralSequenceExpression"
+#          - $ref: "#/$defs/DerivedSequenceExpression"
+#        description: >-
+#          An expression of the repeating subsequence
+#      count:
+#        oneOf:
+#          - $ref: "#/$defs/Number"
+#          - $ref: "#/$defs/IndefiniteRange"
+#          - $ref: "#/$defs/DefiniteRange"
+#        description: >-
+#          The count of repeated units, as an integer or inclusive range
+#    allOf:
+#      - if:
+#          properties:
+#            count:
+#              $ref: "#/$defs/Number"
+#        then:
+#          properties:
+#            count:
+#              properties:
+#                value:
+#                  minimum: 0
+#      - if:
+#          properties:
+#            count:
+#              $ref: "#/$defs/IndefiniteRange"
+#        then:
+#          properties:
+#            count:
+#              properties:
+#                value:
+#                  minimum: 0
+#      - if:
+#          properties:
+#            count:
+#              $ref: "#/$defs/DefiniteRange"
+#        then:
+#          properties:
+#            count:
+#              properties:
+#                min:
+#                  minimum: 0
+#                max:
+#                  minimum: 0
+#    required: [ "seq_expr", "count" ]
+#
+#  ComposedSequenceExpression:
+#    description: >-
+#      An expression of a sequence composed from multiple other
+#      :ref:`Sequence Expressions<SequenceExpression>`
+#      objects. MUST have at least one component that is not a
+#      ref:`LiteralSequenceExpression`. CANNOT be composed from
+#      nested composed sequence expressions.
+#    additionalProperties: false
+#    type: object
+#    properties:
+#      type:
+#        type: string
+#        const: "ComposedSequenceExpression"
+#        default: "ComposedSequenceExpression"
+#        description: MUST be "ComposedSequenceExpression"
+#      components:
+#        type: array
+#        ordered: true
+#        uniqueItems: true
+#        minItems: 2
+#        items:
+#          anyOf:
+#            - $ref: "#/$defs/LiteralSequenceExpression"
+#            - $ref: "#/$defs/RepeatedSequenceExpression"
+#            - $ref: "#/$defs/DerivedSequenceExpression"
+#        description: >-
+#          An ordered list of :ref:`SequenceExpression` components
+#          comprising the expression. MUST NOT have two adjacent
+#          :ref:`LiteralSequenceExpression` objects.
+#    required: [ "components" ]
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # Nested Classes
 
+#  HaplotypeMember:
+#    inherits: gks.core:Entity
+#    description: >-
+#      A class for compact representation of :ref:`Allele` members in the context of a :ref:`Haplotype`.
+#    type: object
+
   GenotypeMember:
+    privateTo: Genotype
+    inherits: gks.core:Entity
     description: >-
       A class for expressing the count of a specific :ref:`MolecularVariation` present
-      *in-trans* at a genomic locus represented by a :ref:`Genotype`.
+      _in-trans_ at a genomic locus represented by a :ref:`Genotype`.
     type: object
     properties:
       type:
         type: string
         const: "GenotypeMember"
         default: "GenotypeMember"
         description: MUST be "GenotypeMember".
       count:
         oneOf:
-          - $ref: "#/definitions/Number"
-          - $ref: "#/definitions/IndefiniteRange"
-          - $ref: "#/definitions/DefiniteRange"
+          - $ref: '#/$defs/Range'
+          - type: integer
         description: >-
           The number of copies of the `variation` at a :ref:`Genotype` locus.
       variation:
         oneOf:
-          - $ref: "#/definitions/Allele"
-          - $ref: "#/definitions/Haplotype"
+          - $ref: "#/$defs/Allele"
+          - $ref: "#/$defs/Haplotype"
         description: >-
           A :ref:`MolecularVariation` at a :ref:`Genotype` locus.
-    required: [ "type", "count", "variation" ]
-
-  # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
-  # Feature
-
-  Feature:
-    description: >-
-      A named entity that can be mapped to a Location. Genes, protein domains,
-      exons, and chromosomes are some examples of common biological entities
-      that may be Features.
-    oneOf:
-      - $ref: "#/definitions/Gene"
-    discriminator:
-      propertyName: type
-    heritable_properties:
-      type:
-        type: string
-        description: >-
-          The Feature class type. MUST match child class type.
-    heritable_required: [ "type" ]
-
-  Gene:
-    inherits: Feature
-    description: >-
-      A reference to a Gene as defined by an authority. For human genes,
-      the use of `hgnc <https://registry.identifiers.org/registry/hgnc>`_
-      as the gene authority is RECOMMENDED.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "Gene"
-        default: "Gene"
-        description: MUST be "Gene"
-      gene_id:
-        $ref: "#/definitions/CURIE"
-        description: >-
-          A CURIE reference to a Gene concept
-    required: [ "gene_id" ]
+    required: [ "count", "variation" ]
 
   # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
   # Numerics, Comparators, and Ranges
 
-  Number:
-    description: >-
-      A simple integer value as a VRS class.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "Number"
-        default: "Number"
-        description: MUST be "Number"
-      value:
-        type: integer
-        description: The value represented by Number
-    required: [ "type", "value" ]
-
-  DefiniteRange:
-    description: >-
-      A bounded, inclusive range of numbers.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "DefiniteRange"
-        default: "DefiniteRange"
-        description: MUST be "DefiniteRange"
-      min:
-        type: number
-        description: The minimum value; inclusive
-      max:
-        type: number
-        description: The maximum value; inclusive
-    required: ["type", "min", "max"]
-
-  IndefiniteRange:
-    description: >-
-      A half-bounded range of numbers represented as a number bound and
-      associated comparator. The bound operator is interpreted as follows:
-      '>=' are all numbers greater than and including `value`, '<=' are all
-      numbers less than and including `value`.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "IndefiniteRange"
-        default: "IndefiniteRange"
-        description: MUST be "IndefiniteRange"
-      value:
-        type: number
-        description: The bounded value; inclusive
-      comparator:
-        type: string
-        enum: [ "<=", ">=" ]
-        description: >-
-          MUST be one of "<=" or ">=", indicating which direction the range
-          is indefinite
-    required: [ "type", "value", "comparator" ]
+  Range:
+    maturity: Alpha
+    description: An inclusive range of values bounded by one or more integers.
+    type: array
+    ordered: true
+    items:
+      oneOf:
+        - type: integer
+        - type: 'null'
+    maxItems: 2
+    minItems: 2
+
+#  Number:
+#    description: >-
+#      A simple integer value as a VRS class.
+#    type: object
+#    properties:
+#      type:
+#        type: string
+#        const: "Number"
+#        default: "Number"
+#        description: MUST be "Number"
+#      value:
+#        type: integer
+#        description: The value represented by Number
+#    required: [ "type", "value" ]
+#
+#  DefiniteRange:
+#    description: >-
+#      A bounded, inclusive range of numbers.
+#    type: object
+#    properties:
+#      type:
+#        type: string
+#        const: "DefiniteRange"
+#        default: "DefiniteRange"
+#        description: MUST be "DefiniteRange"
+#      min:
+#        type: number
+#        description: The minimum value; inclusive
+#      max:
+#        type: number
+#        description: The maximum value; inclusive
+#    required: ["type", "min", "max"]
+#
+#  IndefiniteRange:
+#    description: >-
+#      A half-bounded range of numbers represented as a number bound and
+#      associated comparator. The bound operator is interpreted as follows:
+#      '>=' are all numbers greater than and including `value`, '<=' are all
+#      numbers less than and including `value`.
+#    type: object
+#    properties:
+#      type:
+#        type: string
+#        const: "IndefiniteRange"
+#        default: "IndefiniteRange"
+#        description: MUST be "IndefiniteRange"
+#      value:
+#        type: number
+#        description: The bounded value; inclusive
+#      comparator:
+#        type: string
+#        enum: [ "<=", ">=" ]
+#        description: >-
+#          MUST be one of "<=" or ">=", indicating which direction the range
+#          is indefinite
+#    required: [ "type", "value", "comparator" ]
 
   # =============================================================================
   # BASIC TYPES (STRUCTURES)
   # These types do NOT have a VRS `type` attribute
   # These types are used solely within other definitions.
   # =============================================================================
 
-  CURIE:
-    description: >-
-      A `W3C Compact URI <https://www.w3.org/TR/curie/>`_ formatted string.
-      A CURIE string has the structure ``prefix``:``reference``, as defined by
-      the W3C syntax.
-    type: string
-    pattern: '^\w[^:]*:.+$'
-    example: "ensembl:ENSG00000139618"
-
-  HumanCytoband:
-    description: >-
-      A character string representing cytobands derived from the
-      *International System for Human Cytogenomic Nomenclature* (ISCN)
-      `guidelines <http://doi.org/10.1159/isbn.978-3-318-06861-0>`_.
-    type: string
-    pattern: '^cen|[pq](ter|([1-9][0-9]*(\.[1-9][0-9]*)?))$'
-    example: "q22.3"
+#  HumanCytoband:
+#    description: >-
+#      A character string representing cytobands derived from the
+#      *International System for Human Cytogenomic Nomenclature* (ISCN)
+#      `guidelines <http://doi.org/10.1159/isbn.978-3-318-06861-0>`_.
+#    type: string
+#    pattern: '^cen|[pq](ter|([1-9][0-9]*(\.[1-9][0-9]*)?))$'
+#    example: "q22.3"
 
   Residue:
+    maturity: Alpha
     description: >-
       A character representing a specific residue (i.e., molecular species)
       or groupings of these ("ambiguity codes"), using `one-letter IUPAC
       abbreviations <https://en.wikipedia.org/wiki/International_Union_of_Pure_and_Applied_Chemistry#Amino_acid_and_nucleotide_base_codes>`_
       for nucleic acids and amino acids.
     type: string
     pattern: '[A-Z*\-]'
 
-  Sequence:
+  SequenceString:
+    maturity: Alpha
     description: >-
       A character string of :ref:`Residues <Residue>` that represents a biological
       sequence using the conventional sequence order (5’-to-3’ for
       nucleic acid sequences, and amino-to-carboxyl for amino acid
-      sequences). IUPAC ambiguity codes are permitted in Sequences.
+      sequences). IUPAC ambiguity codes are permitted in Sequence Strings.
     type: string
     pattern: '^[A-Z*\-]*$'
-
-
-  # =============================================================================
-  # DEPRECATED
-  # =============================================================================
-
-  SequenceState:
-    deprecated: true
-    description: >-
-      DEPRECATED. A :ref:`Sequence` as a :ref:`State`. This is the State class
-      to use for representing "ref-alt" style variation, including SNVs, MNVs,
-      del, ins, and delins.
-      This class is deprecated. Use :ref:`LiteralSequenceExpression` instead.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "SequenceState"
-        default: "SequenceState"
-        description: MUST be "SequenceState"
-      sequence:
-        $ref: "#/definitions/Sequence"
-        description: A string of :ref:`Residues <Residue>`
-    example:
-      type: SequenceState
-      sequence: C
-    required: [ "type", "sequence" ]
-
-  SimpleInterval:
-    deprecated: true
-    description: >-
-      DEPRECATED: A SimpleInterval represents a span of sequence. Positions are
-      always represented by contiguous spans using interbase coordinates.
-
-      This class is deprecated. Use SequenceInterval instead.
-    type: object
-    properties:
-      type:
-        type: string
-        const: "SimpleInterval"
-        default: "SimpleInterval"
-        description: MUST be "SimpleInterval"
-      start:
-        type: integer
-        description: The start coordinate
-      end:
-        type: integer
-        description: The end coordinate
-    example:
-      type: SimpleInterval
-      start: 11
-      end: 22
-    required: [ "type", "start", "end" ]
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/tests/data/vrs1.yaml` & `ga4gh.gks.metaschema-0.2.0rc5/tests/data/vrs.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,674 +1,543 @@
-$schema: http://json-schema.org/draft-07/schema
+$schema: http://json-schema.org/draft/2020-12/schema
 title: GA4GH-VRS-Definitions
 type: object
-definitions:
+$defs:
   Variation:
     description: A representation of the state of one or more biomolecules.
     oneOf:
-    - $ref: '#/definitions/AbsoluteCopyNumber'
-    - $ref: '#/definitions/Allele'
-    - $ref: '#/definitions/Genotype'
-    - $ref: '#/definitions/Haplotype'
-    - $ref: '#/definitions/RelativeCopyNumber'
-    - $ref: '#/definitions/Text'
-    - $ref: '#/definitions/VariationSet'
+    - $ref: '#/$defs/Allele'
+    - $ref: '#/$defs/CopyNumberChange'
+    - $ref: '#/$defs/CopyNumberCount'
+    - $ref: '#/$defs/Genotype'
+    - $ref: '#/$defs/Haplotype'
     discriminator:
       propertyName: type
   MolecularVariation:
     description: A variation on a contiguous molecule.
     oneOf:
-    - $ref: '#/definitions/Allele'
-    - $ref: '#/definitions/Haplotype'
-    discriminator:
-      propertyName: type
-  UtilityVariation:
-    description: A collection of Variation subclasses that cannot be constrained to
-      a specific class of biological variation, but are necessary for some applications
-      of VRS.
-    oneOf:
-    - $ref: '#/definitions/Text'
-    - $ref: '#/definitions/VariationSet'
+    - $ref: '#/$defs/Allele'
+    - $ref: '#/$defs/Haplotype'
     discriminator:
       propertyName: type
   SystemicVariation:
     description: A Variation of multiple molecules in the context of a system, e.g.
       a genome, sample, or homologous chromosomes.
     oneOf:
-    - $ref: '#/definitions/AbsoluteCopyNumber'
-    - $ref: '#/definitions/Genotype'
-    - $ref: '#/definitions/RelativeCopyNumber'
+    - $ref: '#/$defs/CopyNumberChange'
+    - $ref: '#/$defs/CopyNumberCount'
+    - $ref: '#/$defs/Genotype'
     discriminator:
       propertyName: type
   Allele:
+    maturity: Alpha
+    ga4ghDigest:
+      prefix: VA
+      keys:
+      - location
+      - state
+      - type
     description: The state of a molecule at a Location.
     type: object
     properties:
-      _id:
-        $ref: '#/definitions/CURIE'
-        description: Variation Id. MUST be unique within document.
+      id:
+        type: string
+        description: The 'logical' identifier of the entity in the system of record,
+          e.g. a UUID. This 'id' is  unique within a given system. The identified
+          entity may have a different 'id' in a different  system, or may refer to
+          an 'id' for the shared concept in another system (e.g. a CURIE).
+      label:
+        type: string
+      extensions:
+        type: array
+        ordered: true
+        items:
+          $ref: core.json#/$defs/Extension
       type:
         type: string
         const: Allele
         default: Allele
         description: MUST be "Allele"
+      digest:
+        description: A sha512t24u digest created using the VRS Computed Identifier
+          algorithm.
+        type: string
+        pattern: '[0-9A-Za-z_\-]{32}'
       location:
         oneOf:
-        - $ref: '#/definitions/CURIE'
-        - $ref: '#/definitions/ChromosomeLocation'
-        - $ref: '#/definitions/SequenceLocation'
-        description: Where Allele is located
+        - $ref: '#/$defs/SequenceLocation'
+        - $ref: core.json#/$defs/IRI
+        description: The location of the Allele
       state:
-        oneOf:
-        - $ref: '#/definitions/ComposedSequenceExpression'
-        - $ref: '#/definitions/DerivedSequenceExpression'
-        - $ref: '#/definitions/LiteralSequenceExpression'
-        - $ref: '#/definitions/RepeatedSequenceExpression'
-        - $ref: '#/definitions/SequenceState'
         description: An expression of the sequence state
-        deprecated:
-        - $ref: '#/definitions/SequenceState'
+        oneOf:
+        - $ref: '#/$defs/LiteralSequenceExpression'
+        - $ref: '#/$defs/ReferenceLengthExpression'
     required:
     - location
     - state
     - type
     additionalProperties: false
   Haplotype:
+    maturity: Alpha
+    ga4ghDigest:
+      prefix: HT
+      keys:
+      - members
+      - type
     description: A set of non-overlapping Allele members that co-occur on the same
       molecule.
     type: object
     properties:
-      _id:
-        $ref: '#/definitions/CURIE'
-        description: Variation Id. MUST be unique within document.
+      id:
+        type: string
+        description: The 'logical' identifier of the entity in the system of record,
+          e.g. a UUID. This 'id' is  unique within a given system. The identified
+          entity may have a different 'id' in a different  system, or may refer to
+          an 'id' for the shared concept in another system (e.g. a CURIE).
+      label:
+        type: string
+      extensions:
+        type: array
+        ordered: true
+        items:
+          $ref: core.json#/$defs/Extension
       type:
         type: string
         const: Haplotype
         default: Haplotype
         description: MUST be "Haplotype"
+      digest:
+        description: A sha512t24u digest created using the VRS Computed Identifier
+          algorithm.
+        type: string
+        pattern: '[0-9A-Za-z_\-]{32}'
       members:
         type: array
+        ordered: false
         minItems: 2
         uniqueItems: true
-        ordered: false
         items:
           oneOf:
-          - $ref: '#/definitions/Allele'
-          - $ref: '#/definitions/CURIE'
+          - $ref: '#/$defs/Allele'
+          - $ref: core.json#/$defs/IRI
         description: List of Alleles, or references to Alleles, that comprise this
           Haplotype.
     required:
     - members
     - type
     additionalProperties: false
-  Text:
-    description: A free-text definition of variation.
-    type: object
-    properties:
-      _id:
-        $ref: '#/definitions/CURIE'
-        description: Variation Id. MUST be unique within document.
-      type:
-        type: string
-        const: Text
-        default: Text
-        description: MUST be "Text"
-      definition:
-        type: string
-        description: A textual representation of variation not representable by other
-          subclasses of Variation.
-    required:
-    - definition
-    - type
-    additionalProperties: false
-  VariationSet:
-    description: An unconstrained set of Variation members.
-    type: object
-    properties:
-      _id:
-        $ref: '#/definitions/CURIE'
-        description: Variation Id. MUST be unique within document.
-      type:
+  CopyNumberCount:
+    maturity: Alpha
+    ga4ghDigest:
+      keys:
+      - copies
+      - subject
+      - type
+      prefix: CN
+    type: object
+    description: The absolute count of discrete copies of a Location or Gene, within
+      a system (e.g. genome, cell, etc.).
+    properties:
+      id:
+        type: string
+        description: The 'logical' identifier of the entity in the system of record,
+          e.g. a UUID. This 'id' is  unique within a given system. The identified
+          entity may have a different 'id' in a different  system, or may refer to
+          an 'id' for the shared concept in another system (e.g. a CURIE).
+      label:
         type: string
-        const: VariationSet
-        default: VariationSet
-        description: MUST be "VariationSet"
-      members:
+      extensions:
         type: array
-        uniqueItems: true
-        ordered: false
+        ordered: true
         items:
-          oneOf:
-          - $ref: '#/definitions/AbsoluteCopyNumber'
-          - $ref: '#/definitions/Allele'
-          - $ref: '#/definitions/CURIE'
-          - $ref: '#/definitions/Genotype'
-          - $ref: '#/definitions/Haplotype'
-          - $ref: '#/definitions/RelativeCopyNumber'
-          - $ref: '#/definitions/Text'
-          - $ref: '#/definitions/VariationSet'
-        description: List of Variation objects or identifiers. Attribute is required,
-          but MAY be empty.
-    required:
-    - members
-    - type
-    additionalProperties: false
-  AbsoluteCopyNumber:
-    type: object
-    maturity: draft
-    description: The absolute count of discrete copies of a Location, within a system
-      (e.g. genome, cell, etc.).
-    properties:
-      _id:
-        $ref: '#/definitions/CURIE'
-        description: Variation Id. MUST be unique within document.
+          $ref: core.json#/$defs/Extension
       type:
         type: string
-        const: AbsoluteCopyNumber
-        default: AbsoluteCopyNumber
-        description: MUST be "AbsoluteCopyNumber"
+        const: CopyNumberCount
+        default: CopyNumberCount
+        description: MUST be "CopyNumberCount"
+      digest:
+        description: A sha512t24u digest created using the VRS Computed Identifier
+          algorithm.
+        type: string
+        pattern: '[0-9A-Za-z_\-]{32}'
       subject:
         oneOf:
-        - $ref: '#/definitions/CURIE'
-        - $ref: '#/definitions/ChromosomeLocation'
-        - $ref: '#/definitions/SequenceLocation'
+        - $ref: '#/$defs/SequenceLocation'
+        - $ref: core.json#/$defs/IRI
         description: A location for which the number of systemic copies is described.
       copies:
         oneOf:
-        - $ref: '#/definitions/DefiniteRange'
-        - $ref: '#/definitions/IndefiniteRange'
-        - $ref: '#/definitions/Number'
+        - $ref: '#/$defs/Range'
+        - type: integer
         description: The integral number of copies of the subject in a system
     required:
     - copies
     - subject
     - type
     additionalProperties: false
-  RelativeCopyNumber:
-    type: object
-    maturity: draft
-    description: The copies of a Location within a system (e.g. genome, cell, etc.)
-      relative to a baseline state.
-    properties:
-      _id:
-        $ref: '#/definitions/CURIE'
-        description: Variation Id. MUST be unique within document.
+  CopyNumberChange:
+    maturity: Alpha
+    ga4ghDigest:
+      keys:
+      - copy_change
+      - subject
+      - type
+      prefix: CX
+    type: object
+    description: An assessment of the copy number of a Location or a Gene within a
+      system (e.g. genome, cell, etc.) relative to a baseline ploidy.
+    properties:
+      id:
+        type: string
+        description: The 'logical' identifier of the entity in the system of record,
+          e.g. a UUID. This 'id' is  unique within a given system. The identified
+          entity may have a different 'id' in a different  system, or may refer to
+          an 'id' for the shared concept in another system (e.g. a CURIE).
+      label:
+        type: string
+      extensions:
+        type: array
+        ordered: true
+        items:
+          $ref: core.json#/$defs/Extension
       type:
         type: string
-        const: RelativeCopyNumber
-        default: RelativeCopyNumber
-        description: MUST be "RelativeCopyNumber"
+        const: CopyNumberChange
+        default: CopyNumberChange
+        description: MUST be "CopyNumberChange"
+      digest:
+        description: A sha512t24u digest created using the VRS Computed Identifier
+          algorithm.
+        type: string
+        pattern: '[0-9A-Za-z_\-]{32}'
       subject:
         oneOf:
-        - $ref: '#/definitions/CURIE'
-        - $ref: '#/definitions/ChromosomeLocation'
-        - $ref: '#/definitions/SequenceLocation'
+        - $ref: '#/$defs/SequenceLocation'
+        - $ref: core.json#/$defs/IRI
         description: A location for which the number of systemic copies is described.
-      relative_copy_class:
+      copy_change:
         type: string
         enum:
-        - complete loss
-        - partial loss
-        - copy neutral
-        - low-level gain
-        - high-level gain
-        description: MUST be one of "complete loss", "partial loss", "copy neutral",
-          "low-level gain" or "high-level gain".
+        - efo:0030069
+        - efo:0020073
+        - efo:0030068
+        - efo:0030067
+        - efo:0030064
+        - efo:0030070
+        - efo:0030071
+        - efo:0030072
+        description: MUST be one of "efo:0030069" (complete genomic loss), "efo:0020073"
+          (high-level loss), "efo:0030068" (low-level loss), "efo:0030067" (loss),
+          "efo:0030064" (regional base ploidy), "efo:0030070" (gain), "efo:0030071"
+          (low-level gain), "efo:0030072" (high-level gain).
     required:
-    - relative_copy_class
+    - copy_change
     - subject
     - type
     additionalProperties: false
   Genotype:
-    description: A quantified set of MolecularVariation associated with a genomic
-      locus.
-    type: object
-    properties:
-      _id:
-        $ref: '#/definitions/CURIE'
-        description: Variation Id. MUST be unique within document.
+    maturity: Alpha
+    ga4ghDigest:
+      keys:
+      - count
+      - members
+      - type
+      prefix: GT
+    description: A quantified set of _in-trans_ MolecularVariation at a genomic locus.
+    type: object
+    properties:
+      id:
+        type: string
+        description: The 'logical' identifier of the entity in the system of record,
+          e.g. a UUID. This 'id' is  unique within a given system. The identified
+          entity may have a different 'id' in a different  system, or may refer to
+          an 'id' for the shared concept in another system (e.g. a CURIE).
+      label:
+        type: string
+      extensions:
+        type: array
+        ordered: true
+        items:
+          $ref: core.json#/$defs/Extension
       type:
         type: string
         const: Genotype
         default: Genotype
         description: MUST be "Genotype"
+      digest:
+        description: A sha512t24u digest created using the VRS Computed Identifier
+          algorithm.
+        type: string
+        pattern: '[0-9A-Za-z_\-]{32}'
       members:
         type: array
+        ordered: false
         uniqueItems: true
         minItems: 1
-        ordered: false
         items:
-          $ref: '#/definitions/GenotypeMember'
+          $ref: '#/$defs/GenotypeMember'
         description: Each GenotypeMember in `members` describes a MolecularVariation
           and the count of that variation at the locus.
       count:
         oneOf:
-        - $ref: '#/definitions/DefiniteRange'
-        - $ref: '#/definitions/IndefiniteRange'
-        - $ref: '#/definitions/Number'
+        - $ref: '#/$defs/Range'
+        - type: integer
         description: The total number of copies of all MolecularVariation at this
-          locus, MUST be greater than or equal to the sum of GenotypeMember copy counts
-          and MUST be greater than or equal to 1. If greater than the total of GenotypeMember
-          counts, this field describes  additional MolecularVariation that exist but
-          are not  explicitly described.
+          locus, MUST be greater than or equal to the sum of GenotypeMember copy counts.
+          If greater than the total counts, this implies additional MolecularVariation
+          that are expected to exist but are not explicitly indicated.
     required:
     - count
     - members
     - type
     additionalProperties: false
   Location:
     description: A contiguous segment of a biological sequence.
     oneOf:
-    - $ref: '#/definitions/ChromosomeLocation'
-    - $ref: '#/definitions/SequenceLocation'
+    - $ref: '#/$defs/SequenceLocation'
     discriminator:
       propertyName: type
-  ChromosomeLocation:
-    description: A Location on a chromosome defined by a species and chromosome name.
-    type: object
-    properties:
-      _id:
-        $ref: '#/definitions/CURIE'
-        description: Location Id. MUST be unique within document.
-      type:
-        type: string
-        const: ChromosomeLocation
-        default: ChromosomeLocation
-        description: MUST be "ChromosomeLocation"
-      species_id:
-        $ref: '#/definitions/CURIE'
-        default: taxonomy:9606
-        description: 'CURIE representing a species from the [NCBI species taxonomy](https://registry.identifiers.org/registry/taxonomy).
-          Default: "taxonomy:9606" (human)'
-      chr:
-        type: string
-        description: The symbolic chromosome name. For humans, For humans, chromosome
-          names MUST be one of 1..22, X, Y (case-sensitive)
-      interval:
-        $ref: '#/definitions/CytobandInterval'
-        description: The chromosome region defined by a CytobandInterval
-    required:
-    - chr
-    - interval
-    - species_id
-    - type
-    additionalProperties: false
   SequenceLocation:
+    maturity: Alpha
+    ga4ghDigest:
+      keys:
+      - count
+      - members
+      - type
+      prefix: SL
     description: A Location defined by an interval on a referenced Sequence.
     type: object
     properties:
-      _id:
-        $ref: '#/definitions/CURIE'
-        description: Location Id. MUST be unique within document.
+      id:
+        type: string
+        description: The 'logical' identifier of the entity in the system of record,
+          e.g. a UUID. This 'id' is  unique within a given system. The identified
+          entity may have a different 'id' in a different  system, or may refer to
+          an 'id' for the shared concept in another system (e.g. a CURIE).
+      label:
+        type: string
+      extensions:
+        type: array
+        ordered: true
+        items:
+          $ref: core.json#/$defs/Extension
       type:
         type: string
         const: SequenceLocation
         default: SequenceLocation
         description: MUST be "SequenceLocation"
-      sequence_id:
-        $ref: '#/definitions/CURIE'
-        description: A VRS Computed Identifier for the reference Sequence.
-      interval:
-        oneOf:
-        - $ref: '#/definitions/SequenceInterval'
-        - $ref: '#/definitions/SimpleInterval'
-        description: Reference sequence region defined by a SequenceInterval.
-    required:
-    - interval
-    - sequence_id
-    - type
-    additionalProperties: false
-  SequenceInterval:
-    description: A SequenceInterval represents a span on a Sequence. Positions are
-      always represented by contiguous spans using interbase coordinates or coordinate
-      ranges.
-    type: object
-    properties:
-      type:
+      digest:
+        description: A sha512t24u digest created using the VRS Computed Identifier
+          algorithm.
         type: string
-        const: SequenceInterval
-        default: SequenceInterval
-        description: MUST be "SequenceInterval"
+        pattern: '[0-9A-Za-z_\-]{32}'
+      sequence:
+        oneOf:
+        - $ref: '#/$defs/SequenceReference'
+        - $ref: core.json#/$defs/IRI
+        description: A SequenceReference.
       start:
         oneOf:
-        - $ref: '#/definitions/DefiniteRange'
-        - $ref: '#/definitions/IndefiniteRange'
-        - $ref: '#/definitions/Number'
-        description: The start coordinate or range of the interval. The minimum value
-          of this coordinate or range is 0. MUST represent a coordinate or range less
-          than the value of `end`.
+        - $ref: '#/$defs/Range'
+        - type: integer
+        description: The start coordinate or range of the SequenceLocation. The minimum
+          value of this coordinate or range is 0. MUST represent a coordinate or range
+          less than the value of `end`.
       end:
         oneOf:
-        - $ref: '#/definitions/DefiniteRange'
-        - $ref: '#/definitions/IndefiniteRange'
-        - $ref: '#/definitions/Number'
-        description: The end coordinate or range of the interval. The minimum value
-          of this coordinate or range is 0. MUST represent a coordinate or range greater
-          than the value of `start`.
+        - $ref: '#/$defs/Range'
+        - type: integer
+        description: The end coordinate or range of the SequenceLocation. The minimum
+          value of this coordinate or range is 0. MUST represent a coordinate or range
+          greater than the value of `start`.
     required:
     - end
     - start
     - type
     additionalProperties: false
-  CytobandInterval:
-    description: A contiguous span on a chromosome defined by cytoband features. The
-      span includes the constituent regions described by the start and end cytobands,
-      as well as any intervening regions.
-    type: object
-    properties:
+  SequenceReference:
+    maturity: Alpha
+    ga4ghDigest:
+      prefix: SQR
+      keys:
+      - refgetAccession
+      - type
+    type: object
+    description: A sequence of nucleic or amino acid character codes.
+    properties:
+      id:
+        type: string
+        description: The 'logical' identifier of the entity in the system of record,
+          e.g. a UUID. This 'id' is  unique within a given system. The identified
+          entity may have a different 'id' in a different  system, or may refer to
+          an 'id' for the shared concept in another system (e.g. a CURIE).
+      label:
+        type: string
+      extensions:
+        type: array
+        ordered: true
+        items:
+          $ref: core.json#/$defs/Extension
       type:
         type: string
-        const: CytobandInterval
-        default: CytobandInterval
-        description: MUST be "CytobandInterval"
-      start:
-        $ref: '#/definitions/HumanCytoband'
-        description: The start cytoband region. MUST specify a region nearer the terminal
-          end (telomere) of the chromosome p-arm than `end`.
-      end:
-        $ref: '#/definitions/HumanCytoband'
-        description: The start cytoband region. MUST specify a region nearer the terminal
-          end (telomere) of the chromosome q-arm than `start`.
-    example:
-      type: CytobandInterval
-      start: q22.2
-      end: q22.3
+        const: Sequence
+        default: Sequence
+        description: MUST be "Sequence"
+      digest:
+        description: A sha512t24u digest created using the VRS Computed Identifier
+          algorithm.
+        type: string
+        pattern: '[0-9A-Za-z_\-]{32}'
+      refgetAccession:
+        description: A `GA4GH RefGet <http://samtools.github.io/hts-specs/refget.html>`
+          identifier for the referenced sequence, using the sha512t24u digest.
+        type: string
+        pattern: SQ.[0-9A-Za-z_\-]{32}
+      residueAlphabet:
+        type: string
+        enum:
+        - amino acid
+        - nucleic acid
     required:
-    - end
-    - start
     - type
     additionalProperties: false
   SequenceExpression:
     description: An expression describing a Sequence.
     oneOf:
-    - $ref: '#/definitions/ComposedSequenceExpression'
-    - $ref: '#/definitions/DerivedSequenceExpression'
-    - $ref: '#/definitions/LiteralSequenceExpression'
-    - $ref: '#/definitions/RepeatedSequenceExpression'
+    - $ref: '#/$defs/LiteralSequenceExpression'
+    - $ref: '#/$defs/ReferenceLengthExpression'
     discriminator:
       propertyName: type
-  LiteralSequenceExpression:
-    description: An explicit expression of a Sequence.
+  ReferenceLengthExpression:
+    maturity: Alpha
+    description: An expression of a length of a sequence from a repeating reference.
     type: object
     properties:
+      id:
+        type: string
+        description: The 'logical' identifier of the entity in the system of record,
+          e.g. a UUID. This 'id' is  unique within a given system. The identified
+          entity may have a different 'id' in a different  system, or may refer to
+          an 'id' for the shared concept in another system (e.g. a CURIE).
+      label:
+        type: string
+      extensions:
+        type: array
+        ordered: true
+        items:
+          $ref: core.json#/$defs/Extension
       type:
         type: string
-        const: LiteralSequenceExpression
-        default: LiteralSequenceExpression
-        description: MUST be "LiteralSequenceExpression"
+        const: ReferenceLengthExpression
+        default: ReferenceLengthExpression
+        description: MUST be "ReferenceLengthExpression"
+      length:
+        oneOf:
+        - $ref: '#/$defs/Range'
+        - type: integer
+        description: The number of residues in the expressed sequence.
       sequence:
-        $ref: '#/definitions/Sequence'
-        description: the literal Sequence expressed
+        $ref: '#/$defs/SequenceString'
+        description: the Sequence encoded by the Reference Length Expression.
+      repeatSubunitLength:
+        type: integer
+        description: The number of residues in the repeat subunit.
     required:
-    - sequence
+    - length
     - type
     additionalProperties: false
-  DerivedSequenceExpression:
-    description: An approximate expression of a sequence that is derived from a referenced
-      sequence location. Use of this class indicates that the derived sequence is
-      *approximately equivalent* to the reference indicated, and is typically used
-      for describing large regions in contexts where the use of an approximate sequence
-      is inconsequential.
+  LiteralSequenceExpression:
+    maturity: Alpha
+    description: An explicit expression of a Sequence.
     type: object
     properties:
-      type:
+      id:
         type: string
-        const: DerivedSequenceExpression
-        default: DerivedSequenceExpression
-        description: MUST be "DerivedSequenceExpression"
-      location:
-        $ref: '#/definitions/SequenceLocation'
-        description: The location from which the approximate sequence is derived
-      reverse_complement:
-        type: boolean
-        description: A flag indicating if the expressed sequence is the reverse complement
-          of the sequence referred to by `location`
-    required:
-    - location
-    - reverse_complement
-    - type
-    additionalProperties: false
-  RepeatedSequenceExpression:
-    description: An expression of a sequence comprised of a tandem repeating subsequence.
-    type: object
-    properties:
+        description: The 'logical' identifier of the entity in the system of record,
+          e.g. a UUID. This 'id' is  unique within a given system. The identified
+          entity may have a different 'id' in a different  system, or may refer to
+          an 'id' for the shared concept in another system (e.g. a CURIE).
+      label:
+        type: string
+      extensions:
+        type: array
+        ordered: true
+        items:
+          $ref: core.json#/$defs/Extension
       type:
         type: string
-        const: RepeatedSequenceExpression
-        default: RepeatedSequenceExpression
-        description: MUST be "RepeatedSequenceExpression"
-      seq_expr:
-        oneOf:
-        - $ref: '#/definitions/DerivedSequenceExpression'
-        - $ref: '#/definitions/LiteralSequenceExpression'
-        description: An expression of the repeating subsequence
-      count:
-        oneOf:
-        - $ref: '#/definitions/DefiniteRange'
-        - $ref: '#/definitions/IndefiniteRange'
-        - $ref: '#/definitions/Number'
-        description: The count of repeated units, as an integer or inclusive range
+        const: LiteralSequenceExpression
+        default: LiteralSequenceExpression
+        description: MUST be "LiteralSequenceExpression"
+      sequence:
+        $ref: '#/$defs/SequenceString'
+        description: the literal sequence
     required:
-    - count
-    - seq_expr
+    - sequence
     - type
     additionalProperties: false
-  ComposedSequenceExpression:
-    description: An expression of a sequence composed from multiple other Sequence
-      Expressions objects. MUST have at least one component that is not a ref:`LiteralSequenceExpression`.
-      CANNOT be composed from nested composed sequence expressions.
-    additionalProperties: false
+  GenotypeMember:
+    privateTo: Genotype
+    description: A class for expressing the count of a specific MolecularVariation
+      present _in-trans_ at a genomic locus represented by a Genotype.
     type: object
     properties:
-      type:
+      id:
+        type: string
+        description: The 'logical' identifier of the entity in the system of record,
+          e.g. a UUID. This 'id' is  unique within a given system. The identified
+          entity may have a different 'id' in a different  system, or may refer to
+          an 'id' for the shared concept in another system (e.g. a CURIE).
+      label:
         type: string
-        const: ComposedSequenceExpression
-        default: ComposedSequenceExpression
-        description: MUST be "ComposedSequenceExpression"
-      components:
+      extensions:
         type: array
-        uniqueItems: true
-        minItems: 2
         ordered: true
         items:
-          oneOf:
-          - $ref: '#/definitions/DerivedSequenceExpression'
-          - $ref: '#/definitions/LiteralSequenceExpression'
-          - $ref: '#/definitions/RepeatedSequenceExpression'
-        contains:
-          oneOf:
-          - $ref: '#/definitions/RepeatedSequenceExpression'
-          - $ref: '#/definitions/DerivedSequenceExpression'
-        description: An ordered list of SequenceExpression components   comprising
-          the expression.
-    required:
-    - components
-  GenotypeMember:
-    description: A class for expressing the count of a specific MolecularVariation
-      present *in-trans* at a genomic locus represented by a Genotype.
-    type: object
-    properties:
+          $ref: core.json#/$defs/Extension
       type:
         type: string
         const: GenotypeMember
         default: GenotypeMember
         description: MUST be "GenotypeMember".
       count:
         oneOf:
-        - $ref: '#/definitions/DefiniteRange'
-        - $ref: '#/definitions/IndefiniteRange'
-        - $ref: '#/definitions/Number'
+        - $ref: '#/$defs/Range'
+        - type: integer
         description: The number of copies of the `variation` at a Genotype locus.
       variation:
         oneOf:
-        - $ref: '#/definitions/Allele'
-        - $ref: '#/definitions/Haplotype'
+        - $ref: '#/$defs/Allele'
+        - $ref: '#/$defs/Haplotype'
         description: A MolecularVariation at a Genotype locus.
     required:
     - count
-    - type
     - variation
     additionalProperties: false
-  Feature:
-    description: A named entity that can be mapped to a Location. Genes, protein domains,
-      exons, and chromosomes are some examples of common biological entities that
-      may be Features.
-    oneOf:
-    - $ref: '#/definitions/Gene'
-    discriminator:
-      propertyName: type
-  Gene:
-    description: A reference to a Gene as defined by an authority. For human genes,
-      the use of [hgnc](https://registry.identifiers.org/registry/hgnc) as the gene
-      authority is RECOMMENDED.
-    type: object
-    properties:
-      type:
-        type: string
-        const: Gene
-        default: Gene
-        description: MUST be "Gene"
-      gene_id:
-        $ref: '#/definitions/CURIE'
-        description: A CURIE reference to a Gene concept
-    required:
-    - gene_id
-    - type
-    additionalProperties: false
-  Number:
-    description: A simple integer value as a VRS class.
-    type: object
-    properties:
-      type:
-        type: string
-        const: Number
-        default: Number
-        description: MUST be "Number"
-      value:
-        type: integer
-        description: The value represented by Number
-    required:
-    - type
-    - value
-    additionalProperties: false
-  DefiniteRange:
-    description: A bounded, inclusive range of numbers.
-    type: object
-    properties:
-      type:
-        type: string
-        const: DefiniteRange
-        default: DefiniteRange
-        description: MUST be "DefiniteRange"
-      min:
-        type: number
-        description: The minimum value; inclusive
-      max:
-        type: number
-        description: The maximum value; inclusive
-    required:
-    - max
-    - min
-    - type
-    additionalProperties: false
-  IndefiniteRange:
-    description: 'A half-bounded range of numbers represented as a number bound and
-      associated comparator. The bound operator is interpreted as follows: ''>=''
-      are all numbers greater than and including `value`, ''<='' are all numbers less
-      than and including `value`.'
-    type: object
-    properties:
-      type:
-        type: string
-        const: IndefiniteRange
-        default: IndefiniteRange
-        description: MUST be "IndefiniteRange"
-      value:
-        type: number
-        description: The bounded value; inclusive
-      comparator:
-        type: string
-        enum:
-        - <=
-        - '>='
-        description: MUST be one of "<=" or ">=", indicating which direction the range
-          is indefinite
-    required:
-    - comparator
-    - type
-    - value
-    additionalProperties: false
-  CURIE:
-    description: A [W3C Compact URI](https://www.w3.org/TR/curie/) formatted string.
-      A CURIE string has the structure ``prefix``:``reference``, as defined by the
-      W3C syntax.
-    type: string
-    pattern: ^\w[^:]*:.+$
-    example: ensembl:ENSG00000139618
-  HumanCytoband:
-    description: A character string representing cytobands derived from the *International
-      System for Human Cytogenomic Nomenclature* (ISCN) [guidelines](http://doi.org/10.1159/isbn.978-3-318-06861-0).
-    type: string
-    pattern: ^cen|[pq](ter|([1-9][0-9]*(\.[1-9][0-9]*)?))$
-    example: q22.3
+  Range:
+    maturity: Alpha
+    description: An inclusive range of values bounded by one or more integers.
+    type: array
+    ordered: true
+    items:
+      oneOf:
+      - type: integer
+      - type: 'null'
+    maxItems: 2
+    minItems: 2
   Residue:
+    maturity: Alpha
     description: A character representing a specific residue (i.e., molecular species)
       or groupings of these ("ambiguity codes"), using [one-letter IUPAC abbreviations](https://en.wikipedia.org/wiki/International_Union_of_Pure_and_Applied_Chemistry#Amino_acid_and_nucleotide_base_codes)
       for nucleic acids and amino acids.
     type: string
     pattern: '[A-Z*\-]'
-  Sequence:
+  SequenceString:
+    maturity: Alpha
     description: "A character string of Residues that represents a biological sequence\
       \ using the conventional sequence order (5\u2019-to-3\u2019 for nucleic acid\
       \ sequences, and amino-to-carboxyl for amino acid sequences). IUPAC ambiguity\
-      \ codes are permitted in Sequences."
+      \ codes are permitted in Sequence Strings."
     type: string
     pattern: ^[A-Z*\-]*$
-  SequenceState:
-    deprecated: true
-    description: DEPRECATED. A Sequence as a State. This is the State class to use
-      for representing "ref-alt" style variation, including SNVs, MNVs, del, ins,
-      and delins. This class is deprecated. Use LiteralSequenceExpression instead.
-    type: object
-    properties:
-      type:
-        type: string
-        const: SequenceState
-        default: SequenceState
-        description: MUST be "SequenceState"
-      sequence:
-        $ref: '#/definitions/Sequence'
-        description: A string of Residues
-    example:
-      type: SequenceState
-      sequence: C
-    required:
-    - sequence
-    - type
-    additionalProperties: false
-  SimpleInterval:
-    deprecated: true
-    description: 'DEPRECATED: A SimpleInterval represents a span of sequence. Positions
-      are always represented by contiguous spans using interbase coordinates. This
-      class is deprecated. Use SequenceInterval instead.'
-    type: object
-    properties:
-      type:
-        type: string
-        const: SimpleInterval
-        default: SimpleInterval
-        description: MUST be "SimpleInterval"
-      start:
-        type: integer
-        description: The start coordinate
-      end:
-        type: integer
-        description: The end coordinate
-    example:
-      type: SimpleInterval
-      start: 11
-      end: 22
-    required:
-    - end
-    - start
-    - type
-    additionalProperties: false
```

### Comparing `ga4gh.gks.metaschema-0.2.0rc4/tests/test_basic.py` & `ga4gh.gks.metaschema-0.2.0rc5/tests/test_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,10 +25,16 @@
 def test_yaml_create():
     p = YamlSchemaProcessor('data/core-source.yaml')
     p.js_yaml_dump(open('data/core.yaml', 'w'))
     assert True
 
 
 def test_merged_create():
-    p = YamlSchemaProcessor('data/vod-source.yaml')
+    p = YamlSchemaProcessor('data/vrs-source.yaml')
     p.merge_imported()
+    assert True
+
+
+def test_split_create():
+    p = YamlSchemaProcessor('data/vrs-source.yaml')
+    p.split_defs_to_js()
     assert True
```

