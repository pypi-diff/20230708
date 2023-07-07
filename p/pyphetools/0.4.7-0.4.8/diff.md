# Comparing `tmp/pyphetools-0.4.7.tar.gz` & `tmp/pyphetools-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphetools-0.4.7.tar", last modified: Fri Jul  7 15:05:29 2023, max compression
+gzip compressed data, was "pyphetools-0.4.8.tar", last modified: Fri Jul  7 23:43:53 2023, max compression
```

## Comparing `pyphetools-0.4.7.tar` & `pyphetools-0.4.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.456592 pyphetools-0.4.7/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.4.7/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.4.7/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-07-07 15:05:29.456592 pyphetools-0.4.7/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.4.7/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.448592 pyphetools-0.4.7/docs/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.4.7/docs/conf.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.448592 pyphetools-0.4.7/pyphetools/
--rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.4.7/pyphetools/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.448592 pyphetools-0.4.7/pyphetools/analyze/
--rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.4.7/pyphetools/analyze/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.4.7/pyphetools/analyze/downsampler.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.452592 pyphetools-0.4.7/pyphetools/creation/
--rw-rw-r--   0 peter     (1000) peter     (1000)      911 2023-07-07 14:16:51.000000 pyphetools-0.4.7/pyphetools/creation/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.4.7/pyphetools/creation/age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7929 2023-06-29 13:53:18.000000 pyphetools-0.4.7/pyphetools/creation/case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    10828 2023-06-29 12:55:59.000000 pyphetools-0.4.7/pyphetools/creation/cohort_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.4.7/pyphetools/creation/column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.4.7/pyphetools/creation/constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.4.7/pyphetools/creation/constants.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.4.7/pyphetools/creation/custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5506 2023-06-29 11:35:00.000000 pyphetools-0.4.7/pyphetools/creation/hgvs_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.4.7/pyphetools/creation/hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.4.7/pyphetools/creation/hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7408 2023-07-07 14:18:33.000000 pyphetools-0.4.7/pyphetools/creation/hpo_exact_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.4.7/pyphetools/creation/hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7515 2023-06-29 13:36:57.000000 pyphetools-0.4.7/pyphetools/creation/individual.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6402 2023-06-29 15:58:37.000000 pyphetools-0.4.7/pyphetools/creation/metadata.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6643 2023-07-07 15:03:31.000000 pyphetools-0.4.7/pyphetools/creation/option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.4.7/pyphetools/creation/sex_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6191 2023-07-07 14:27:35.000000 pyphetools-0.4.7/pyphetools/creation/simple_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6969 2023-06-29 11:43:08.000000 pyphetools-0.4.7/pyphetools/creation/structural_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.4.7/pyphetools/creation/thresholded_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      268 2023-06-29 11:43:15.000000 pyphetools-0.4.7/pyphetools/creation/variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5641 2023-06-29 13:35:41.000000 pyphetools-0.4.7/pyphetools/creation/variant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3240 2023-06-29 12:52:03.000000 pyphetools-0.4.7/pyphetools/creation/variant_validator.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.452592 pyphetools-0.4.7/pyphetools/output/
--rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.4.7/pyphetools/output/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.4.7/pyphetools/output/detailed_suppl_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.4.7/pyphetools/output/focus_count_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.4.7/pyphetools/output/hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.4.7/pyphetools/output/phenopacket_ingestor.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.4.7/pyphetools/output/phenopacket_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.4.7/pyphetools/output/simple_patient.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3306 2023-07-04 23:45:19.000000 pyphetools-0.4.7/pyphetools/output/simple_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.4.7/pyphetools/output/term_count.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.452592 pyphetools-0.4.7/pyphetools/validation/
--rw-rw-r--   0 peter     (1000) peter     (1000)      111 2023-06-29 14:50:29.000000 pyphetools-0.4.7/pyphetools/validation/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3792 2023-06-29 17:31:14.000000 pyphetools-0.4.7/pyphetools/validation/content_validator.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      187 2023-06-29 14:49:26.000000 pyphetools-0.4.7/pyphetools/validation/phenopacket_validator.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1115 2023-06-29 17:46:07.000000 pyphetools-0.4.7/pyphetools/validation/validation_result.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.448592 pyphetools-0.4.7/pyphetools.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-07-07 15:05:29.000000 pyphetools-0.4.7/pyphetools.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     2326 2023-07-07 15:05:29.000000 pyphetools-0.4.7/pyphetools.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-07 15:05:29.000000 pyphetools-0.4.7/pyphetools.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-07-07 15:05:29.000000 pyphetools-0.4.7/pyphetools.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       56 2023-07-07 15:05:29.000000 pyphetools-0.4.7/pyphetools.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-07-07 15:04:43.000000 pyphetools-0.4.7/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-07 15:05:29.456592 pyphetools-0.4.7/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.452592 pyphetools-0.4.7/test/
--rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.4.7/test/test_age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3370 2023-06-29 13:58:19.000000 pyphetools-0.4.7/test/test_case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.4.7/test/test_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.4.7/test/test_constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.4.7/test/test_custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.4.7/test/test_hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.4.7/test/test_hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.4.7/test/test_hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.4.7/test/test_hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5398 2023-07-07 15:04:27.000000 pyphetools-0.4.7/test/test_option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1648 2023-06-28 18:34:15.000000 pyphetools-0.4.7/test/test_structural_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.4.7/test/test_threshold_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1447 2023-06-29 12:31:36.000000 pyphetools-0.4.7/test/test_variant.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.448592 pyphetools-0.4.7/venv/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 15:05:29.456592 pyphetools-0.4.7/venv/bin/
--rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2html.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2html4.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2html5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2latex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2man.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2odt.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2s5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2xetex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rst2xml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.4.7/venv/bin/rstpep2html.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.537470 pyphetools-0.4.8/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.4.8/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.4.8/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-07-07 23:43:53.537470 pyphetools-0.4.8/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.4.8/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.529470 pyphetools-0.4.8/docs/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.4.8/docs/conf.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.529470 pyphetools-0.4.8/pyphetools/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.4.8/pyphetools/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.529470 pyphetools-0.4.8/pyphetools/analyze/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.4.8/pyphetools/analyze/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.4.8/pyphetools/analyze/downsampler.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.533470 pyphetools-0.4.8/pyphetools/creation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      911 2023-07-07 14:16:51.000000 pyphetools-0.4.8/pyphetools/creation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.4.8/pyphetools/creation/age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7929 2023-06-29 13:53:18.000000 pyphetools-0.4.8/pyphetools/creation/case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10828 2023-06-29 12:55:59.000000 pyphetools-0.4.8/pyphetools/creation/cohort_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.4.8/pyphetools/creation/column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.4.8/pyphetools/creation/constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.4.8/pyphetools/creation/constants.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.4.8/pyphetools/creation/custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5279 2023-07-07 23:38:12.000000 pyphetools-0.4.8/pyphetools/creation/hgvs_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.4.8/pyphetools/creation/hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.4.8/pyphetools/creation/hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7408 2023-07-07 14:18:33.000000 pyphetools-0.4.8/pyphetools/creation/hpo_exact_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.4.8/pyphetools/creation/hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7515 2023-06-29 13:36:57.000000 pyphetools-0.4.8/pyphetools/creation/individual.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6402 2023-06-29 15:58:37.000000 pyphetools-0.4.8/pyphetools/creation/metadata.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6643 2023-07-07 15:03:31.000000 pyphetools-0.4.8/pyphetools/creation/option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.4.8/pyphetools/creation/sex_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6191 2023-07-07 14:27:35.000000 pyphetools-0.4.8/pyphetools/creation/simple_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6701 2023-07-07 23:40:41.000000 pyphetools-0.4.8/pyphetools/creation/structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.4.8/pyphetools/creation/thresholded_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      750 2023-07-07 23:43:35.000000 pyphetools-0.4.8/pyphetools/creation/variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5641 2023-06-29 13:35:41.000000 pyphetools-0.4.8/pyphetools/creation/variant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3240 2023-06-29 12:52:03.000000 pyphetools-0.4.8/pyphetools/creation/variant_validator.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.533470 pyphetools-0.4.8/pyphetools/output/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.4.8/pyphetools/output/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.4.8/pyphetools/output/detailed_suppl_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.4.8/pyphetools/output/focus_count_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.4.8/pyphetools/output/hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.4.8/pyphetools/output/phenopacket_ingestor.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.4.8/pyphetools/output/phenopacket_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.4.8/pyphetools/output/simple_patient.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3306 2023-07-04 23:45:19.000000 pyphetools-0.4.8/pyphetools/output/simple_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.4.8/pyphetools/output/term_count.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.533470 pyphetools-0.4.8/pyphetools/validation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      111 2023-06-29 14:50:29.000000 pyphetools-0.4.8/pyphetools/validation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3792 2023-06-29 17:31:14.000000 pyphetools-0.4.8/pyphetools/validation/content_validator.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      187 2023-06-29 14:49:26.000000 pyphetools-0.4.8/pyphetools/validation/phenopacket_validator.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1115 2023-06-29 17:46:07.000000 pyphetools-0.4.8/pyphetools/validation/validation_result.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.529470 pyphetools-0.4.8/pyphetools.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-07-07 23:43:53.000000 pyphetools-0.4.8/pyphetools.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2326 2023-07-07 23:43:53.000000 pyphetools-0.4.8/pyphetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-07 23:43:53.000000 pyphetools-0.4.8/pyphetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-07-07 23:43:53.000000 pyphetools-0.4.8/pyphetools.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       56 2023-07-07 23:43:53.000000 pyphetools-0.4.8/pyphetools.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-07-07 23:41:02.000000 pyphetools-0.4.8/pyproject.toml
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-07 23:43:53.537470 pyphetools-0.4.8/setup.cfg
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.537470 pyphetools-0.4.8/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.4.8/test/test_age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3370 2023-06-29 13:58:19.000000 pyphetools-0.4.8/test/test_case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.4.8/test/test_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.4.8/test/test_constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.4.8/test/test_custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.4.8/test/test_hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.4.8/test/test_hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.4.8/test/test_hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.4.8/test/test_hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5398 2023-07-07 15:04:27.000000 pyphetools-0.4.8/test/test_option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1607 2023-07-07 23:39:10.000000 pyphetools-0.4.8/test/test_structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.4.8/test/test_threshold_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1447 2023-06-29 12:31:36.000000 pyphetools-0.4.8/test/test_variant.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.529470 pyphetools-0.4.8/venv/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-07 23:43:53.537470 pyphetools-0.4.8/venv/bin/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2html.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2html4.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2html5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2latex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2man.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2odt.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2s5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rst2xml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.4.8/venv/bin/rstpep2html.py
```

### Comparing `pyphetools-0.4.7/LICENSE` & `pyphetools-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/PKG-INFO` & `pyphetools-0.4.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.4.7
+Version: 0.4.8
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.4.7/README.md` & `pyphetools-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/docs/conf.py` & `pyphetools-0.4.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/analyze/downsampler.py` & `pyphetools-0.4.8/pyphetools/analyze/downsampler.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/__init__.py` & `pyphetools-0.4.8/pyphetools/creation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/age_column_mapper.py` & `pyphetools-0.4.8/pyphetools/creation/age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/case_encoder.py` & `pyphetools-0.4.8/pyphetools/creation/case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/cohort_encoder.py` & `pyphetools-0.4.8/pyphetools/creation/cohort_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/column_mapper.py` & `pyphetools-0.4.8/pyphetools/creation/column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/constant_column_mapper.py` & `pyphetools-0.4.8/pyphetools/creation/constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/custom_column_mapper.py` & `pyphetools-0.4.8/pyphetools/creation/custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/hgvs_variant.py` & `pyphetools-0.4.8/pyphetools/creation/hgvs_variant.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,23 +53,14 @@
     @property
     def alt(self):
         return self._alt
     
     @property
     def genotype(self):
         return self._genotype
-    
-    def set_heterozygous(self):
-        self._genotype = 'heterozygous'
-    
-    def set_homozygous(self):
-        self._genotype = 'homozygous'
-        
-    def set_hemizygous(self):
-        self._genotype = 'hemizygous'
           
     def __str__(self):
         return f"{self._chr}:{self._position}{self._ref}>{self._alt}"
     
     def to_string(self):
         return self.__str__()
```

### Comparing `pyphetools-0.4.7/pyphetools/creation/hp_term.py` & `pyphetools-0.4.8/pyphetools/creation/hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/hpo_cr.py` & `pyphetools-0.4.8/pyphetools/creation/hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/hpo_exact_cr.py` & `pyphetools-0.4.8/pyphetools/creation/hpo_exact_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/hpo_parser.py` & `pyphetools-0.4.8/pyphetools/creation/hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/individual.py` & `pyphetools-0.4.8/pyphetools/creation/individual.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/metadata.py` & `pyphetools-0.4.8/pyphetools/creation/metadata.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/option_column_mapper.py` & `pyphetools-0.4.8/pyphetools/creation/option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/sex_column_mapper.py` & `pyphetools-0.4.8/pyphetools/creation/sex_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/simple_column_mapper.py` & `pyphetools-0.4.8/pyphetools/creation/simple_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/structural_variant.py` & `pyphetools-0.4.8/pyphetools/creation/structural_variant.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     """
 
     def __init__(self, cell_contents,
                  gene_symbol,
                  gene_id,
                  sequence_ontology_id,
                  sequence_ontology_label,
-                 genotype,
                  variant_id: None):
         super().__init__()
         if variant_id is None:
             self._variant_id = "var_" + "".join(random.choices(string.ascii_letters, k=25))
         else:
             self._variant_id = variant_id
         self._label = cell_contents.strip()
@@ -49,15 +48,15 @@
             raise ValueError(f"Need to pass a valid gene symbol!")
         self._gene_symbol = gene_symbol
         if gene_id is None:
             raise ValueError(f"Need to pass a valid HGNC gene id!")
         self._hgnc_id = gene_id
         self._so_id = sequence_ontology_id
         self._so_label = sequence_ontology_label
-        self._genotype = genotype
+        self._genotype = None
 
     def to_ga4gh_variant_interpretation(self, acmg=None):
         """
         Transform this Variant object into a "variantInterpretation" message of the GA4GH Phenopacket schema
         """
         vdescriptor = phenopackets.VariationDescriptor()
         vdescriptor.id = self._variant_id
@@ -98,44 +97,39 @@
 
     # provide static constructors for most important structural variation types
 
     @staticmethod
     def chromosomal_deletion(cell_contents,
                              gene_symbol,
                              gene_id,
-                             genotype,
                              variant_id=None):
         return StructuralVariant(cell_contents=cell_contents,
                                  gene_symbol=gene_symbol,
                                  gene_id=gene_id,
                                  sequence_ontology_id="SO:1000029",
                                  sequence_ontology_label="chromosomal_deletion",
-                                 genotype=genotype,
                                  variant_id=variant_id)
 
     @staticmethod
     def chromosomal_duplication(cell_contents,
                                 gene_symbol,
                                 gene_id,
-                                genotype,
                                 variant_id=None):
         return StructuralVariant(cell_contents=cell_contents,
                                  gene_symbol=gene_symbol,
                                  gene_id=gene_id,
                                  sequence_ontology_id="SO:1000037",
                                  sequence_ontology_label="chromosomal_duplication",
-                                 genotype=genotype,
                                  variant_id=variant_id)
 
     @staticmethod
     def chromosomal_inversion(cell_contents,
                               gene_symbol,
                               gene_id,
                               genotype,
                               variant_id=None):
         return StructuralVariant(cell_contents=cell_contents,
                                  gene_symbol=gene_symbol,
                                  gene_id=gene_id,
                                  sequence_ontology_id="SO:1000030",
                                  sequence_ontology_label="chromosomal_inversion",
-                                 genotype=genotype,
                                  variant_id=variant_id)
```

### Comparing `pyphetools-0.4.7/pyphetools/creation/thresholded_column_mapper.py` & `pyphetools-0.4.8/pyphetools/creation/thresholded_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/variant_column_mapper.py` & `pyphetools-0.4.8/pyphetools/creation/variant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/creation/variant_validator.py` & `pyphetools-0.4.8/pyphetools/creation/variant_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/output/detailed_suppl_table.py` & `pyphetools-0.4.8/pyphetools/output/detailed_suppl_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/output/focus_count_table.py` & `pyphetools-0.4.8/pyphetools/output/focus_count_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/output/hpo_category.py` & `pyphetools-0.4.8/pyphetools/output/hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/output/phenopacket_ingestor.py` & `pyphetools-0.4.8/pyphetools/output/phenopacket_ingestor.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/output/phenopacket_table.py` & `pyphetools-0.4.8/pyphetools/output/phenopacket_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/output/simple_patient.py` & `pyphetools-0.4.8/pyphetools/output/simple_patient.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/output/simple_variant.py` & `pyphetools-0.4.8/pyphetools/output/simple_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/output/term_count.py` & `pyphetools-0.4.8/pyphetools/output/term_count.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/validation/content_validator.py` & `pyphetools-0.4.8/pyphetools/validation/content_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools/validation/validation_result.py` & `pyphetools-0.4.8/pyphetools/validation/validation_result.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyphetools.egg-info/PKG-INFO` & `pyphetools-0.4.8/pyphetools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.4.7
+Version: 0.4.8
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.4.7/pyphetools.egg-info/SOURCES.txt` & `pyphetools-0.4.8/pyphetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/pyproject.toml` & `pyphetools-0.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["notebooks", "test"]
 
 [project]
 name = "pyphetools"
-version = "0.4.7"
+version = "0.4.8"
 requires-python = ">=3.5"
 description = "Generate and work with GA4GH phenopackets"
 readme = "README.md"
 authors = [
     {name = "Peter Robinson", email="peter.robinson@jax.org"},
      ]
 license = { file = "LICENSE" }
```

### Comparing `pyphetools-0.4.7/test/test_age_column_mapper.py` & `pyphetools-0.4.8/test/test_age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_case_encoder.py` & `pyphetools-0.4.8/test/test_case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_column_mapper.py` & `pyphetools-0.4.8/test/test_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_constant_column_mapper.py` & `pyphetools-0.4.8/test/test_constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_custom_column_mapper.py` & `pyphetools-0.4.8/test/test_custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_hp_term.py` & `pyphetools-0.4.8/test/test_hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_hpo_category.py` & `pyphetools-0.4.8/test/test_hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_hpo_cr.py` & `pyphetools-0.4.8/test/test_hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_hpo_parser.py` & `pyphetools-0.4.8/test/test_hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_option_column_mapper.py` & `pyphetools-0.4.8/test/test_option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_structural_variant.py` & `pyphetools-0.4.8/test/test_structural_variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     def setUpClass(cls) -> None:
         variant = "46,XY.ish del(7)(p14.1)(RP11-816F16-)"
         genotype = "heterozygous"
         gene = "GLI3"
         gene_id = "HGNC:4319"
         sv = StructuralVariant.chromosomal_deletion(cell_contents=variant,
                                                     gene_symbol=gene,
-                                                    gene_id=gene_id,
-                                                    genotype=genotype)
+                                                    gene_id=gene_id)
+        sv.set_heterozygous()
         cls._variant_interpretation = sv.to_ga4gh_variant_interpretation()
 
     def test_label(self):
         var_inter = self._variant_interpretation
         variant_descriptor = var_inter.variation_descriptor
         print(type(variant_descriptor))
         print([field.full_name for field in self._variant_interpretation.DESCRIPTOR.fields])
```

### Comparing `pyphetools-0.4.7/test/test_threshold_column_mapper.py` & `pyphetools-0.4.8/test/test_threshold_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/test/test_variant.py` & `pyphetools-0.4.8/test/test_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2html.py` & `pyphetools-0.4.8/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2html4.py` & `pyphetools-0.4.8/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2html5.py` & `pyphetools-0.4.8/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2latex.py` & `pyphetools-0.4.8/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2man.py` & `pyphetools-0.4.8/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2odt.py` & `pyphetools-0.4.8/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2odt_prepstyles.py` & `pyphetools-0.4.8/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2pseudoxml.py` & `pyphetools-0.4.8/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2s5.py` & `pyphetools-0.4.8/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2xetex.py` & `pyphetools-0.4.8/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rst2xml.py` & `pyphetools-0.4.8/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.7/venv/bin/rstpep2html.py` & `pyphetools-0.4.8/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

