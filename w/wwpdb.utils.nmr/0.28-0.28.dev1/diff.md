# Comparing `tmp/wwpdb.utils.nmr-0.28.tar.gz` & `tmp/wwpdb.utils.nmr-0.28.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.nmr-0.28.tar", last modified: Sat Jul  8 12:03:00 2023, max compression
+gzip compressed data, was "wwpdb.utils.nmr-0.28.dev1.tar", last modified: Thu Jul  6 12:26:17 2023, max compression
```

## Comparing `wwpdb.utils.nmr-0.28.tar` & `wwpdb.utils.nmr-0.28.dev1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.406182 wwpdb.utils.nmr-0.28/
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      704 2023-07-08 12:03:00.410182 wwpdb.utils.nmr-0.28/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       36 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-08 12:03:00.410182 wwpdb.utils.nmr-0.28/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2814 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.374182 wwpdb.utils.nmr-0.28/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.374182 wwpdb.utils.nmr-0.28/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.382182 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/
--rw-r--r--   0 vsts      (1001) docker     (123)   103812 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/AlignUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    72301 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/BMRBChemShiftStat.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12129 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/ChemCompUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26972 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/CifToNmrStar.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.382182 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/
--rw-r--r--   0 vsts      (1001) docker     (123)   517809 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4051 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.382182 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/lib/
--rw-r--r--   0 vsts      (1001) docker     (123)    27217 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     9863 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    10176 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   103535 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NmrDpReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)  2763977 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NmrDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)    23027 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NmrStarToCif.py
--rw-r--r--   0 vsts      (1001) docker     (123)   130980 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NmrVrptUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.386182 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/
--rwxr-xr-x   0 vsts      (1001) docker     (123)    10676 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    25729 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)    10656 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    25737 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3458 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3495 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8742 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)   170036 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/others.csv
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3573 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8327 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3591 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8409 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.386182 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    13142 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/io/ChemCompIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)    66593 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/io/CifReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/io/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10198 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/io/mmCIFUtil.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.406182 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/
--rw-r--r--   0 vsts      (1001) docker     (123)    79462 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   234229 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   493179 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20363 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    42777 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberPTLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   178190 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberPTParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    79373 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberPTParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8451 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberPTReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11409 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/BiosymMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    41669 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/BiosymMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   135928 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/BiosymMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9563 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/BiosymMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    84136 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CharmmMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   212951 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CharmmMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   295091 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CharmmMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9003 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CharmmMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)   151068 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CnsMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   417159 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CnsMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   469882 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CnsMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13554 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CnsMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    32899 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CyanaMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   167192 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CyanaMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   454966 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CyanaMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18196 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CyanaMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    50972 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/DynamoMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   219341 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/DynamoMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   236108 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/DynamoMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9611 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/DynamoMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15500 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    43150 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    92902 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10402 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27535 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsPTLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   159229 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsPTParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    71357 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsPTParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8276 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsPTReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10640 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/IsdMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7446 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/IsdMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    83785 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/IsdMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8792 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/IsdMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3593 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/LexerErrorListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4792 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/ParserErrorListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)   406211 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/ParserListenerUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    33530 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/RosettaMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   119610 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/RosettaMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   215435 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/RosettaMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10471 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/RosettaMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11350 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/SybylMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10246 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/SybylMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    84828 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/SybylMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9089 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/SybylMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)   165077 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/XplorMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   679237 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/XplorMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   684343 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/XplorMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    21181 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/XplorMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.406182 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/rci/
--rw-r--r--   0 vsts      (1001) docker     (123)   361662 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/rci/RCI.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-08 11:58:33.000000 wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/rci/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-08 12:03:00.374182 wwpdb.utils.nmr-0.28/wwpdb.utils.nmr.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      704 2023-07-08 12:03:00.000000 wwpdb.utils.nmr-0.28/wwpdb.utils.nmr.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3774 2023-07-08 12:03:00.000000 wwpdb.utils.nmr-0.28/wwpdb.utils.nmr.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-08 12:03:00.000000 wwpdb.utils.nmr-0.28/wwpdb.utils.nmr.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-08 11:59:50.000000 wwpdb.utils.nmr-0.28/wwpdb.utils.nmr.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      330 2023-07-08 12:03:00.000000 wwpdb.utils.nmr-0.28/wwpdb.utils.nmr.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-08 12:03:00.000000 wwpdb.utils.nmr-0.28/wwpdb.utils.nmr.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      709 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       36 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2814 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.299945 wwpdb.utils.nmr-0.28.dev1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.299945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.303945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/
+-rw-r--r--   0 vsts      (1001) docker     (123)   103812 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/AlignUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    72301 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/BMRBChemShiftStat.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12129 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/ChemCompUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26972 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/CifToNmrStar.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/
+-rw-r--r--   0 vsts      (1001) docker     (123)   517809 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4051 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/
+-rw-r--r--   0 vsts      (1001) docker     (123)    27217 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     9863 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    10176 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   103535 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  2763977 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    23027 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrStarToCif.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   130980 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrVrptUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    10676 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    25729 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    10656 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    25737 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3458 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3495 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8742 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)   170036 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/others.csv
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3573 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8327 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3591 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8409 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)    13142 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/ChemCompIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66593 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/CifReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10198 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/mmCIFUtil.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    79462 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   234229 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   493179 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20363 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    42777 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   178190 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    79373 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8451 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11409 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    41669 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   135928 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9563 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    84136 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   212951 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   295091 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9003 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   151068 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   417159 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   469882 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13554 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    32899 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   167192 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   454966 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18196 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    50972 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   219341 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   236108 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9611 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15500 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    43150 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    92902 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10402 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27535 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   159229 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    71357 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8276 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10640 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7446 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    83785 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8792 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3593 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/LexerErrorListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4792 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserErrorListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   406211 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserListenerUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    33530 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   119610 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   215435 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10471 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11350 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10246 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    84828 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9089 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   165077 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   679237 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   684343 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21181 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/
+-rw-r--r--   0 vsts      (1001) docker     (123)   361662 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/RCI.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.299945 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      709 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3774 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-06 12:23:12.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      330 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.nmr-0.28/LICENSE` & `wwpdb.utils.nmr-0.28.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/PKG-INFO` & `wwpdb.utils.nmr-0.28.dev1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.nmr
-Version: 0.28
+Version: 0.28.dev1
 Summary: wwPDB NMR utilities
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_nmr
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.nmr-0.28/setup.py` & `wwpdb.utils.nmr-0.28.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/AlignUtil.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/AlignUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/BMRBChemShiftStat.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/BMRBChemShiftStat.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/ChemCompUtil.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/ChemCompUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/CifToNmrStar.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/CifToNmrStar.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/README.md` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/README.md`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NmrDpReport.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NmrDpUtility.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpUtility.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NmrStarToCif.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrStarToCif.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/NmrVrptUtility.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrVrptUtility.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/others.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/others.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/io/ChemCompIo.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/ChemCompIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/io/CifReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/CifReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/io/mmCIFUtil.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/mmCIFUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberPTLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberPTParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberPTParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/AmberPTReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/BiosymMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/BiosymMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/BiosymMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/BiosymMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CharmmMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CharmmMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CharmmMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CharmmMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CnsMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CnsMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CnsMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CnsMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CyanaMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CyanaMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CyanaMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/CyanaMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/DynamoMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/DynamoMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/DynamoMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/DynamoMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsPTLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsPTParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsPTParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/GromacsPTReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/IsdMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/IsdMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/IsdMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/IsdMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/LexerErrorListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/LexerErrorListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/ParserErrorListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserErrorListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/ParserListenerUtil.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserListenerUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/RosettaMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/RosettaMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/RosettaMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/RosettaMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/SybylMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/SybylMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/SybylMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/SybylMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/XplorMRLexer.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRLexer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/XplorMRParser.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/XplorMRParserListener.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/mr/XplorMRReader.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb/utils/nmr/rci/RCI.py` & `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/RCI.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28/wwpdb.utils.nmr.egg-info/PKG-INFO` & `wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.nmr
-Version: 0.28
+Version: 0.28.dev1
 Summary: wwPDB NMR utilities
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_nmr
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.nmr-0.28/wwpdb.utils.nmr.egg-info/SOURCES.txt` & `wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

