# Comparing `tmp/excelrd-2.0.3.tar.gz` & `tmp/excelrd-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/excelrd-2.0.3.tar", last modified: Sun Jan 12 12:13:51 2020, max compression
+gzip compressed data, was "excelrd-3.0.0.tar", last modified: Sat Jul  8 06:58:00 2023, max compression
```

## Comparing `excelrd-2.0.3.tar` & `excelrd-3.0.0.tar`

### file list

```diff
@@ -1,90 +1,76 @@
-drwxrwxr-x   0 toor      (1000) toor      (1000)        0 2020-01-12 12:13:51.000000 excelrd-2.0.3/
-drwxrwxr-x   0 toor      (1000) toor      (1000)        0 2020-01-12 12:13:51.000000 excelrd-2.0.3/docs/
--rw-rw-r--   0 toor      (1000) toor      (1000)     4903 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/Makefile
--rw-rw-r--   0 toor      (1000) toor      (1000)      859 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/acknowledgements.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)      881 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/api.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)    18025 2020-01-05 06:23:36.000000 excelrd-2.0.3/docs/changes.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)      752 2020-01-05 06:49:23.000000 excelrd-2.0.3/docs/conf.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     3989 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/dates.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)     1673 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/development.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)     4441 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/formatting.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)      723 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/index.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)      472 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/installation.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)       50 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/licenses.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)     4691 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/make.bat
--rw-rw-r--   0 toor      (1000) toor      (1000)     2514 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/on_demand.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)     1831 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/references.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)     1452 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/unicode.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)     1634 2020-01-05 04:29:39.000000 excelrd-2.0.3/docs/vulnerabilities.rst
-drwxrwxr-x   0 toor      (1000) toor      (1000)        0 2020-01-12 12:13:51.000000 excelrd-2.0.3/examples/
--rw-rw-r--   0 toor      (1000) toor      (1000)    22528 2020-01-05 04:29:39.000000 excelrd-2.0.3/examples/namesdemo.xls
--rwxrwxr-x   0 toor      (1000) toor      (1000)      649 2020-01-05 07:14:44.000000 excelrd-2.0.3/examples/quickstart.py
--rwxrwxr-x   0 toor      (1000) toor      (1000)     7361 2020-01-05 06:52:23.000000 excelrd-2.0.3/examples/xlrdnameAPIdemo.py
-drwxrwxr-x   0 toor      (1000) toor      (1000)        0 2020-01-12 12:13:51.000000 excelrd-2.0.3/excelrd/
--rw-rw-r--   0 toor      (1000) toor      (1000)     6752 2020-01-05 07:24:49.000000 excelrd-2.0.3/excelrd/__init__.py
--rw-rw-r--   0 toor      (1000) toor      (1000)    16856 2020-01-05 07:29:53.000000 excelrd-2.0.3/excelrd/biffh.py
--rw-rw-r--   0 toor      (1000) toor      (1000)    59966 2020-01-05 07:24:49.000000 excelrd-2.0.3/excelrd/book.py
--rw-rw-r--   0 toor      (1000) toor      (1000)    23116 2020-01-11 02:26:44.000000 excelrd-2.0.3/excelrd/compdoc.py
--rw-rw-r--   0 toor      (1000) toor      (1000)    47860 2020-01-05 07:30:00.000000 excelrd-2.0.3/excelrd/formatting.py
--rw-rw-r--   0 toor      (1000) toor      (1000)    95266 2020-01-05 07:30:04.000000 excelrd-2.0.3/excelrd/formula.py
--rw-rw-r--   0 toor      (1000) toor      (1000)       36 2020-01-12 12:11:36.000000 excelrd-2.0.3/excelrd/info.py
--rw-rw-r--   0 toor      (1000) toor      (1000)   112139 2020-01-05 07:30:07.000000 excelrd-2.0.3/excelrd/sheet.py
--rw-rw-r--   0 toor      (1000) toor      (1000)      771 2020-01-05 06:51:55.000000 excelrd-2.0.3/excelrd/timemachine.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     7942 2020-01-05 07:30:12.000000 excelrd-2.0.3/excelrd/xldate.py
--rw-rw-r--   0 toor      (1000) toor      (1000)    32989 2020-01-05 07:24:49.000000 excelrd-2.0.3/excelrd/xlsx.py
-drwxrwxr-x   0 toor      (1000) toor      (1000)        0 2020-01-12 12:13:51.000000 excelrd-2.0.3/excelrd.egg-info/
--rw-rw-r--   0 toor      (1000) toor      (1000)     6035 2020-01-12 12:13:51.000000 excelrd-2.0.3/excelrd.egg-info/PKG-INFO
--rw-rw-r--   0 toor      (1000) toor      (1000)     1842 2020-01-12 12:13:51.000000 excelrd-2.0.3/excelrd.egg-info/SOURCES.txt
--rw-rw-r--   0 toor      (1000) toor      (1000)        1 2020-01-12 12:13:51.000000 excelrd-2.0.3/excelrd.egg-info/dependency_links.txt
--rw-rw-r--   0 toor      (1000) toor      (1000)       69 2020-01-12 12:13:51.000000 excelrd-2.0.3/excelrd.egg-info/requires.txt
--rw-rw-r--   0 toor      (1000) toor      (1000)        8 2020-01-12 12:13:51.000000 excelrd-2.0.3/excelrd.egg-info/top_level.txt
-drwxrwxr-x   0 toor      (1000) toor      (1000)        0 2020-01-12 12:13:51.000000 excelrd-2.0.3/scripts/
--rw-rw-r--   0 toor      (1000) toor      (1000)    16822 2020-01-05 06:52:47.000000 excelrd-2.0.3/scripts/runxlrd.py
-drwxrwxr-x   0 toor      (1000) toor      (1000)        0 2020-01-12 12:13:51.000000 excelrd-2.0.3/tests/
--rw-rw-r--   0 toor      (1000) toor      (1000)    10752 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/Formate.xls
--rw-rw-r--   0 toor      (1000) toor      (1000)        0 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/__init__.py
--rw-rw-r--   0 toor      (1000) toor      (1000)   105424 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/apachepoi_49609.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)     5292 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/apachepoi_52348.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)      119 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/base.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     2810 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/biff4_no_format_no_window2.xls
--rw-rw-r--   0 toor      (1000) toor      (1000)   972800 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/corrupted_error.xls
--rw-rw-r--   0 toor      (1000) toor      (1000)   127624 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/err_cell_empty.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)     7680 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/formula_test_names.xls
--rw-rw-r--   0 toor      (1000) toor      (1000)    16896 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/formula_test_sjmachin.xls
--rw-rw-r--   0 toor      (1000) toor      (1000)    99016 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/issue150.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)     6144 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/issue20.xls
--rw-rw-r--   0 toor      (1000) toor      (1000)     9275 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/merged_cells.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)     6656 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/picture_in_cell.xls
--rw-rw-r--   0 toor      (1000) toor      (1000)    33792 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/profiles.xls
--rw-rw-r--   0 toor      (1000) toor      (1000)     6656 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/ragged.xls
--rw-rw-r--   0 toor      (1000) toor      (1000)    16683 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/reveng1.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)     7278 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/self_evaluation_report_2014-05-19.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)     4821 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/sharedstrings_alt_location.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)      541 2020-01-05 06:52:12.000000 excelrd-2.0.3/tests/test_alt_sharedstrings_loc.py
--rw-rw-r--   0 toor      (1000) toor      (1000)      386 2020-01-05 07:24:49.000000 excelrd-2.0.3/tests/test_biffh.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     2718 2020-01-05 06:52:12.000000 excelrd-2.0.3/tests/test_cell.py
--rw-rw-r--   0 toor      (1000) toor      (1000)    15803 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/test_comments_excel.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)    32180 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/test_comments_excel_sheet2.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)     4187 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/test_comments_gdocs.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)     2837 2020-01-05 07:30:16.000000 excelrd-2.0.3/tests/test_formats.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     2162 2020-01-05 07:30:17.000000 excelrd-2.0.3/tests/test_formulas.py
--rw-rw-r--   0 toor      (1000) toor      (1000)      462 2020-01-05 06:52:12.000000 excelrd-2.0.3/tests/test_ignore_workbook_corruption_error.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     5413 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/test_lower_case_cellnames.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)      664 2020-01-05 06:52:12.000000 excelrd-2.0.3/tests/test_missing_records.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     1905 2020-01-05 06:52:12.000000 excelrd-2.0.3/tests/test_open_workbook.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     5456 2020-01-05 07:24:49.000000 excelrd-2.0.3/tests/test_sheet.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     2033 2020-01-05 07:24:49.000000 excelrd-2.0.3/tests/test_workbook.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     2322 2020-01-05 07:24:49.000000 excelrd-2.0.3/tests/test_xldate.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     6125 2020-01-05 07:24:49.000000 excelrd-2.0.3/tests/test_xldate_to_datetime.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     1903 2020-01-05 06:52:12.000000 excelrd-2.0.3/tests/test_xlsx_comments.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     2861 2020-01-05 06:52:13.000000 excelrd-2.0.3/tests/test_xlsx_parse.py
--rw-rw-r--   0 toor      (1000) toor      (1000)     8196 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/text_bar.xlsx
--rw-rw-r--   0 toor      (1000) toor      (1000)    23040 2020-01-05 04:29:39.000000 excelrd-2.0.3/tests/xf_class.xls
--rw-rw-r--   0 toor      (1000) toor      (1000)     3771 2020-01-05 04:29:39.000000 excelrd-2.0.3/LICENSE
--rw-rw-r--   0 toor      (1000) toor      (1000)      158 2020-01-05 06:14:21.000000 excelrd-2.0.3/MANIFEST.in
--rw-rw-r--   0 toor      (1000) toor      (1000)     3801 2020-01-12 11:58:46.000000 excelrd-2.0.3/README.rst
--rw-rw-r--   0 toor      (1000) toor      (1000)      765 2020-01-12 03:43:35.000000 excelrd-2.0.3/pyproject.toml
--rw-rw-r--   0 toor      (1000) toor      (1000)       98 2020-01-12 12:13:51.000000 excelrd-2.0.3/setup.cfg
--rw-rw-r--   0 toor      (1000) toor      (1000)     2314 2020-01-12 12:09:31.000000 excelrd-2.0.3/setup.py
--rw-rw-r--   0 toor      (1000) toor      (1000)      521 2020-01-12 12:04:40.000000 excelrd-2.0.3/tox.ini
--rw-rw-r--   0 toor      (1000) toor      (1000)     6035 2020-01-12 12:13:51.000000 excelrd-2.0.3/PKG-INFO
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 06:58:00.951823 excelrd-3.0.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     3771 2023-07-08 06:57:12.000000 excelrd-3.0.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      191 2023-07-08 06:57:12.000000 excelrd-3.0.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     5449 2023-07-08 06:58:00.951823 excelrd-3.0.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     4015 2023-07-08 06:57:12.000000 excelrd-3.0.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 06:58:00.921823 excelrd-3.0.0/examples/
+-rw-r--r--   0 toor      (1000) toor      (1000)    22528 2023-07-08 06:57:12.000000 excelrd-3.0.0/examples/namesdemo.xls
+-rwxr-xr-x   0 toor      (1000) toor      (1000)      617 2023-07-08 06:57:12.000000 excelrd-3.0.0/examples/quickstart.py
+-rwxr-xr-x   0 toor      (1000) toor      (1000)     7355 2023-07-08 06:57:12.000000 excelrd-3.0.0/examples/xlrdnameAPIdemo.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 06:58:00.931823 excelrd-3.0.0/excelrd/
+-rw-r--r--   0 toor      (1000) toor      (1000)     6851 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      281 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16806 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/biffh.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    59934 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/book.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    23291 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/compdoc.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    48443 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/formatting.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    95451 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/formula.py
+-rw-r--r--   0 toor      (1000) toor      (1000)   112209 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/sheet.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      665 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/timemachine.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7924 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/xldate.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    33198 2023-07-08 06:57:12.000000 excelrd-3.0.0/excelrd/xlsx.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 06:58:00.931823 excelrd-3.0.0/excelrd.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5449 2023-07-08 06:58:00.000000 excelrd-3.0.0/excelrd.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1620 2023-07-08 06:58:00.000000 excelrd-3.0.0/excelrd.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-08 06:58:00.000000 excelrd-3.0.0/excelrd.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      152 2023-07-08 06:58:00.000000 excelrd-3.0.0/excelrd.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        8 2023-07-08 06:58:00.000000 excelrd-3.0.0/excelrd.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      913 2023-07-08 06:57:12.000000 excelrd-3.0.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 06:58:00.931823 excelrd-3.0.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       36 2023-07-08 06:57:12.000000 excelrd-3.0.0/requirements/docs_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       36 2023-07-08 06:57:12.000000 excelrd-3.0.0/requirements/test_requirements.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 06:58:00.931823 excelrd-3.0.0/scripts/
+-rw-r--r--   0 toor      (1000) toor      (1000)    16818 2023-07-08 06:57:12.000000 excelrd-3.0.0/scripts/runxlrd.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-08 06:58:00.951823 excelrd-3.0.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2720 2023-07-08 06:57:12.000000 excelrd-3.0.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-08 06:58:00.951823 excelrd-3.0.0/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)    10752 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/Formate.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)   105424 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/apachepoi_49609.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)     5292 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/apachepoi_52348.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)      119 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2810 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/biff4_no_format_no_window2.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)   972800 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/corrupted_error.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)   127624 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/err_cell_empty.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)     7680 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/formula_test_names.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)    16896 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/formula_test_sjmachin.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)    99016 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/issue150.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)     6144 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/issue20.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)     9275 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/merged_cells.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)     6656 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/picture_in_cell.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)    33792 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/profiles.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)     6656 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/ragged.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)    16683 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/reveng1.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)     7278 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/self_evaluation_report_2014-05-19.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)     4821 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/sharedstrings_alt_location.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)      541 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_alt_sharedstrings_loc.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      375 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_biffh.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2636 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_cell.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    15803 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_comments_excel.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)    32180 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_comments_excel_sheet2.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)     4187 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_comments_gdocs.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)     2826 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_formats.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2162 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_formulas.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      462 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_ignore_workbook_corruption_error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5413 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_lower_case_cellnames.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)      664 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_missing_records.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1927 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_open_workbook.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5455 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_sheet.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2033 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_workbook.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2322 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_xldate.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6125 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_xldate_to_datetime.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1903 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_xlsx_comments.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2861 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/test_xlsx_parse.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8196 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/text_bar.xlsx
+-rw-r--r--   0 toor      (1000) toor      (1000)    23040 2023-07-08 06:57:12.000000 excelrd-3.0.0/tests/xf_class.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)     1058 2023-07-08 06:57:12.000000 excelrd-3.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `excelrd-2.0.3/examples/namesdemo.xls` & `excelrd-3.0.0/examples/namesdemo.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/examples/quickstart.py` & `excelrd-3.0.0/examples/quickstart.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 import excelrd
 
 
 def main():
     book = excelrd.open_workbook("namesdemo.xls")
 
-    print("The number of worksheets is {}".format(book.nsheets))
+    print(f"The number of worksheets is {book.nsheets}")
     print("Worksheet name(s): {}".format(", ".join(book.sheet_names())))
 
     sh = book.sheet_by_index(2)
-    print("{}: rows={}, cols={}".format(sh.name, sh.nrows, sh.ncols))
+    print(f"{sh.name}: rows={sh.nrows}, cols={sh.ncols}")
 
     for row_idx in range(sh.nrows):
         for col_idx in range(sh.ncols):
             cell = sh.cell(row_idx, col_idx)
 
             if not cell.value:
                 continue
 
-            print("row={}, col={}, value={}".format(row_idx, col_idx, cell.value))
+            print(f"row={row_idx}, col={col_idx}, value={cell.value}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `excelrd-2.0.3/examples/xlrdnameAPIdemo.py` & `excelrd-3.0.0/examples/xlrdnameAPIdemo.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 
 def showable_cell_value(celltype, cellvalue, datemode):
     if celltype == excelrd.XL_CELL_DATE:
         try:
             showval = excelrd.xldate_as_tuple(cellvalue, datemode)
         except excelrd.XLDateError as e:
-            showval = "%s:%s" % (type(e).__name__, e)
+            showval = f"{type(e).__name__}:{e}"
     elif celltype == excelrd.XL_CELL_ERROR:
         showval = excelrd.error_text_from_code.get(
             cellvalue, "<Unknown error code 0x%02x>" % cellvalue
         )
     else:
         showval = cellvalue
     return showval
```

### Comparing `excelrd-2.0.3/excelrd/__init__.py` & `excelrd-3.0.0/excelrd/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 # Copyright (c) 2005-2012 Stephen John Machin, Lingfo Pty Ltd
 # This module is part of the excelrd package, which is released under a
 # BSD-style licence.
+
+import io
 import os
 import pprint
 import sys
 import zipfile
 
-from . import timemachine
+from .__version__ import (
+    __author__,
+    __copyright__,
+    __email__,
+    __license__,
+    __maintainer__,
+    __maintainer_email__,
+    __version__,
+)
 from .biffh import (
     XL_CELL_BLANK,
     XL_CELL_BOOLEAN,
     XL_CELL_DATE,
     XL_CELL_EMPTY,
     XL_CELL_ERROR,
     XL_CELL_NUMBER,
     XL_CELL_TEXT,
     XLRDError,
     biff_text_from_num,
     error_text_from_code,
 )
 from .book import Book, colname
 from .formula import *  # is constrained by __all__
-from .info import __VERSION__, __version__
 from .sheet import empty_cell
 from .xldate import XLDateError, xldate_as_datetime, xldate_as_tuple
 from .xlsx import X12Book
 
 
 if sys.version.startswith("IronPython"):
     # print >> sys.stderr, "...importing encodings"
@@ -128,22 +137,22 @@
         peek = file_contents[:peeksz]
     else:
         filename = os.path.expanduser(filename)
         with open(filename, "rb") as f:
             peek = f.read(peeksz)
     if peek == b"PK\x03\x04":  # a ZIP file
         if file_contents:
-            zf = zipfile.ZipFile(timemachine.BYTES_IO(file_contents))
+            zf = zipfile.ZipFile(io.BytesIO(file_contents))
         else:
             zf = zipfile.ZipFile(filename)
 
         # Workaround for some third party files that use forward slashes and
         # lower case names. We map the expected name in lowercase to the
         # actual filename in the zip container.
-        component_names = dict([(X12Book.convert_filename(name), name) for name in zf.namelist()])
+        component_names = {X12Book.convert_filename(name): name for name in zf.namelist()}
 
         if verbosity:
             logfile.write("ZIP component_names:\n")
             pprint.pprint(component_names, logfile)
         if "xl/workbook.xml" in component_names:
             from . import xlsx
 
@@ -189,15 +198,16 @@
     :param outfile: An open file, to which the dump is written.
     :param unnumbered: If true, omit offsets (for meaningful diffs).
     """
     from .biffh import biff_dump
 
     bk = Book()
     bk.biff2_8_load(
-        filename=filename, logfile=outfile,
+        filename=filename,
+        logfile=outfile,
     )
     biff_dump(bk.mem, bk.base, bk.stream_len, 0, outfile, unnumbered)
 
 
 def count_records(filename, outfile=sys.stdout):
     """
     For debugging and analysis: summarise the file's BIFF records.
@@ -206,10 +216,11 @@
     :param filename: The path to the file to be summarised.
     :param outfile: An open file, to which the summary is written.
     """
     from .biffh import biff_count_records
 
     bk = Book()
     bk.biff2_8_load(
-        filename=filename, logfile=outfile,
+        filename=filename,
+        logfile=outfile,
     )
     biff_count_records(bk.mem, bk.base, bk.stream_len, outfile)
```

### Comparing `excelrd-2.0.3/excelrd/biffh.py` & `excelrd-3.0.0/excelrd/biffh.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class XLRDError(Exception):
     """
     An exception indicating problems reading data from an Excel file.
     """
 
 
-class BaseObject(object):
+class BaseObject:
     """
     Parent of almost all other classes in the package. Defines a common
     :meth:`dump` method for debugging.
     """
 
     _repr_these = []
 
@@ -47,15 +47,15 @@
             print(header, file=f)
         list_type = type([])
         dict_type = type({})
         for attr, value in alist:
             if getattr(value, "dump", None) and attr != "book":
                 value.dump(
                     f,
-                    header="%s%s (%s object):" % (pad, attr, value.__class__.__name__),
+                    header=f"{pad}{attr} ({value.__class__.__name__} object):",
                     indent=indent + 4,
                 )
             elif attr not in self._repr_these and (
                 isinstance(value, list_type) or isinstance(value, dict_type)
             ):
                 print("%s%s: %s, len = %d" % (pad, attr, type(value), len(value)), file=f)
             else:
@@ -271,15 +271,15 @@
 
 def unpack_unicode(data, pos, lenlen=2):
     "Return unicode_strg"
     nchars = unpack("<" + "BH"[lenlen - 1], data[pos : pos + lenlen])[0]
     if not nchars:
         # Ambiguous whether 0-length string should have an "options" byte.
         # Avoid crash if missing.
-        return UNICODE_LITERAL("")
+        return ""
     pos += lenlen
     options = BYTES_ORD(data[pos])
     pos += 1
     # phonetic = options & 0x04
     # richtext = options & 0x08
     if options & 0x08:
         # rt = unpack('<H', data[pos:pos+2])[0] # unused
@@ -315,15 +315,15 @@
         # On a NAME record, the length byte is detached from the front of the string.
         nchars = known_len
     else:
         nchars = unpack("<" + "BH"[lenlen - 1], data[pos : pos + lenlen])[0]
         pos += lenlen
     if not nchars and not data[pos:]:
         # Zero-length string with no options byte
-        return (UNICODE_LITERAL(""), pos)
+        return ("", pos)
     options = BYTES_ORD(data[pos])
     pos += 1
     phonetic = options & 0x04
     richtext = options & 0x08
     if richtext:
         rt = unpack("<H", data[pos : pos + 2])[0]
         pos += 2
```

### Comparing `excelrd-2.0.3/excelrd/book.py` & `excelrd-3.0.0/excelrd/book.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     "Auto_Deactivate": "\x0B",
     "Sheet_Title": "\x0C",
     "_FilterDatabase": "\x0D",
 }
 builtin_name_from_code = {}
 code_from_builtin_name = {}
 for _bin, _bic in _code_from_builtin_name.items():
-    _bin = UNICODE_LITERAL(_bin)
-    _bic = UNICODE_LITERAL(_bic)
+    _bin = _bin
+    _bic = _bic
     code_from_builtin_name[_bin] = _bic
     builtin_name_from_code[_bic] = _bin
 del _bin, _bic, _code_from_builtin_name
 
 
 def open_workbook_xls(
     filename=None,
@@ -195,15 +195,15 @@
     #: .. note:: No examples have been sighted.
     binary = 0
 
     #: The index of this object in book.name_obj_list
     name_index = 0
 
     # A Unicode string. If builtin, decoded as per OOo docs.
-    name = UNICODE_LITERAL("")
+    name = ""
 
     #: An 8-bit string.
     raw_formula = b""
 
     #: ``-1``:
     #:    The name is global (visible in all calculation sheets).
     #: ``-2``:
@@ -357,15 +357,15 @@
     #: This information may give a clue to the correct encoding for an
     #: unknown codepage. For a long list of observed values, refer to the
     #: OpenOffice.org documentation for the ``COUNTRY`` record.
     countries = (0, 0)
 
     #: What (if anything) is recorded as the name of the last user to
     #: save the file.
-    user_name = UNICODE_LITERAL("")
+    user_name = ""
 
     #: A list of :class:`~excelrd.formatting.Font` class instances,
     #: each corresponding to a FONT record.
     #:
     #: .. versionadded:: 0.6.1
     font_list = []
 
@@ -672,24 +672,22 @@
             cd = compdoc.CompDoc(
                 self.filestr,
                 logfile=self.logfile,
                 ignore_workbook_corruption=ignore_workbook_corruption,
             )
             if USE_FANCY_CD:
                 for qname in ["Workbook", "Book"]:
-                    self.mem, self.base, self.stream_len = cd.locate_named_stream(
-                        UNICODE_LITERAL(qname)
-                    )
+                    self.mem, self.base, self.stream_len = cd.locate_named_stream(qname)
                     if self.mem:
                         break
                 else:
                     raise XLRDError("Can't find workbook in OLE2 compound document")
             else:
                 for qname in ["Workbook", "Book"]:
-                    self.mem = cd.get_named_stream(UNICODE_LITERAL(qname))
+                    self.mem = cd.get_named_stream(qname)
                     if self.mem:
                         break
                 else:
                     raise XLRDError("Can't find workbook in OLE2 compound document")
                 self.stream_len = len(self.mem)
             del cd
             if self.mem is not self.filestr:
@@ -751,15 +749,20 @@
             self._position = self._sh_abs_posn[sh_number]
         self.getbof(XL_WORKSHEET)
         # assert biff_version == self.biff_version ### FAILS
         # Have an example where book is v7 but sheet reports v8!!!
         # It appears to work OK if the sheet version is ignored.
         # Confirmed by Daniel Rentz: happens when Excel does "save as"
         # creating an old version file; ignore version details on sheet BOF.
-        sh = sheet.Sheet(self, self._position, self._sheet_names[sh_number], sh_number,)
+        sh = sheet.Sheet(
+            self,
+            self._position,
+            self._sheet_names[sh_number],
+            sh_number,
+        )
         sh.read(self)
         self._sheet_list[sh_number] = sh
         return sh
 
     def get_sheets(self):
         # DEBUG = 0
         if DEBUG:
@@ -773,15 +776,15 @@
                     self._sh_abs_posn,
                     file=self.logfile,
                 )
             self.get_sheet(sheetno)
 
     def fake_globals_get_sheet(self):  # for BIFF 4.0 and earlier
         formatting.initialise_book(self)
-        fake_sheet_name = UNICODE_LITERAL("Sheet 1")
+        fake_sheet_name = "Sheet 1"
         self._sheet_names = [fake_sheet_name]
         self._sh_abs_posn = [0]
         self._sheet_visibility = [0]  # one sheet, visible
         self._sheet_list.append(None)  # get_sheet updates _sheet_list but needs a None beforehand
         self.get_sheets()
 
     def handle_boundsheet(self, data):
@@ -820,17 +823,19 @@
                 sheet_name,
                 abs_posn,
                 sheet_type,
             )
         self._all_sheets_count += 1
         if sheet_type != XL_BOUNDSHEET_WORKSHEET:
             self._all_sheets_map.append(-1)
-            descr = {1: "Macro sheet", 2: "Chart", 6: "Visual Basic module",}.get(
-                sheet_type, "UNKNOWN"
-            )
+            descr = {
+                1: "Macro sheet",
+                2: "Chart",
+                6: "Visual Basic module",
+            }.get(sheet_type, "UNKNOWN")
 
             if DEBUG or self.verbosity >= 1:
                 fprintf(
                     self.logfile,
                     "NOTE *** Ignoring non-worksheet data named %r (type 0x%02x = %s)\n",
                     sheet_name,
                     sheet_type,
@@ -1302,15 +1307,15 @@
                 fprintf(self.logfile, "CONTINUE: adding %d bytes to SST -> %d\n", nb, nbt)
             strlist.append(data)
         self._sharedstrings, rt_runlist = unpack_SST_table(strlist, uniquestrings)
         if self.formatting_info:
             self._rich_text_runlist_map = rt_runlist
         if DEBUG:
             t1 = perf_counter()
-            print("SST processing took %.2f seconds" % (t1 - t0,), file=self.logfile)
+            print(f"SST processing took {t1 - t0:.2f} seconds", file=self.logfile)
 
     def handle_writeaccess(self, data):
         DEBUG = 0
         if self.biff_version < 80:
             if not self.encoding:
                 self.raw_user_name = True
                 self.user_name = data
@@ -1459,17 +1464,21 @@
             elif version2 == 0x0500:
                 if year < 1994 or build in (2412, 3218, 3321):
                     version = 50
                 else:
                     version = 70
             else:
                 # dodgy one, created by a 3rd-party tool
-                version = {0x0000: 21, 0x0007: 21, 0x0200: 21, 0x0300: 30, 0x0400: 40,}.get(
-                    version2, 0
-                )
+                version = {
+                    0x0000: 21,
+                    0x0007: 21,
+                    0x0200: 21,
+                    0x0300: 30,
+                    0x0400: 40,
+                }.get(version2, 0)
         elif version1 in (0x04, 0x02, 0x00):
             version = {0x04: 40, 0x02: 30, 0x00: 21}[version1]
 
         if version == 40 and streamtype == XL_WORKBOOK_GLOBALS_4W:
             version = 45  # i.e. 4W
 
         if DEBUG or self.verbosity >= 2:
@@ -1513,15 +1522,15 @@
     else:
         relcol = 0
     return outrow, outcol, relrow, relcol
 
 
 def colname(colx, _A2Z="ABCDEFGHIJKLMNOPQRSTUVWXYZ"):
     assert colx >= 0
-    name = UNICODE_LITERAL("")
+    name = ""
     while 1:
         quot, rem = divmod(colx, 26)
         name = _A2Z[rem] + name
         if not quot:
             return name
         colx = quot - 1
 
@@ -1561,15 +1570,15 @@
         phosz = 0
         if options & 0x08:  # richtext
             rtcount = local_unpack("<H", data[pos : pos + 2])[0]
             pos += 2
         if options & 0x04:  # phonetic
             phosz = local_unpack("<i", data[pos : pos + 4])[0]
             pos += 4
-        accstrg = UNICODE_LITERAL("")
+        accstrg = ""
         charsgot = 0
         while 1:
             charsneed = nchars - charsgot
             if options & 0x01:
                 # Uncompressed UTF-16
                 charsavail = local_min((datalen - pos) >> 1, charsneed)
                 rawstrg = data[pos : pos + 2 * charsavail]
```

### Comparing `excelrd-2.0.3/excelrd/compdoc.py` & `excelrd-3.0.0/excelrd/compdoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 EVILSID = -5
 
 
 class CompDocError(Exception):
     pass
 
 
-class DirNode(object):
+class DirNode:
     def __init__(self, DID, dent, DEBUG=0, logfile=sys.stdout):
         # dent is the 128-byte directory entry
         self.DID = DID
         self.logfile = logfile
         (cbufsize, self.etype, self.colour, self.left_DID, self.right_DID, self.root_DID) = unpack(
             "<HBBiii", dent[64:80]
         )
         (self.first_SID, self.tot_size) = unpack("<ii", dent[116:124])
         if cbufsize == 0:
-            self.name = UNICODE_LITERAL("")
+            self.name = ""
         else:
             self.name = str(dent[0 : cbufsize - 2], "utf_16_le")  # omit the trailing U+0000
         self.children = []  # filled in later
         self.parent = -1  # indicates orphan; fixed up later
         self.tsinfo = unpack("<IIII", dent[100:116])
         if DEBUG:
             self.dump(DEBUG)
@@ -77,15 +77,15 @@
     dirlist[parent_DID].children.append(child_DID)
     dirlist[child_DID].parent = parent_DID
     _build_family_tree(dirlist, parent_DID, dirlist[child_DID].right_DID)
     if dirlist[child_DID].etype == 1:  # storage
         _build_family_tree(dirlist, child_DID, dirlist[child_DID].root_DID)
 
 
-class CompDoc(object):
+class CompDoc:
     """
     Compound document handler.
 
     :param mem:
       The raw contents of the file, as a string, or as an :class:`mmap.mmap`
       object. The only operation it needs to support is slicing.
     """
@@ -97,15 +97,15 @@
         if mem[0:8] != SIGNATURE:
             raise CompDocError("Not an OLE2 compound document")
         if mem[28:30] != b"\xFE\xFF":
             raise CompDocError('Expected "little-endian" marker, found %r' % mem[28:30])
         revision, version = unpack("<HH", mem[24:28])
         if DEBUG:
             print(
-                "\nCompDoc format: version=0x%04x revision=0x%04x" % (version, revision),
+                f"\nCompDoc format: version=0x{version:04x} revision=0x{revision:04x}",
                 file=logfile,
             )
         self.mem = mem
         ssz, sssz = unpack("<HH", mem[30:34])
         if ssz > 20:  # allows for 2**20 bytes i.e. 1MB
             print(
                 "WARNING: sector size (2**%d) is preposterous; assuming 512 and continuing ..."
@@ -152,24 +152,35 @@
         seen = self.seen = array.array("B", [0]) * mem_data_secs
 
         if DEBUG:
             print("sec sizes", ssz, sssz, sec_size, self.short_sec_size, file=logfile)
             print("mem data: %d bytes == %d sectors" % (mem_data_len, mem_data_secs), file=logfile)
             print(
                 "SAT_tot_secs=%d, dir_first_sec_sid=%d, min_size_std_stream=%d"
-                % (SAT_tot_secs, self.dir_first_sec_sid, self.min_size_std_stream,),
+                % (
+                    SAT_tot_secs,
+                    self.dir_first_sec_sid,
+                    self.min_size_std_stream,
+                ),
                 file=logfile,
             )
             print(
-                "SSAT_first_sec_sid=%d, SSAT_tot_secs=%d" % (SSAT_first_sec_sid, SSAT_tot_secs,),
+                "SSAT_first_sec_sid=%d, SSAT_tot_secs=%d"
+                % (
+                    SSAT_first_sec_sid,
+                    SSAT_tot_secs,
+                ),
                 file=logfile,
             )
             print(
                 "MSATX_first_sec_sid=%d, MSATX_tot_secs=%d"
-                % (MSATX_first_sec_sid, MSATX_tot_secs,),
+                % (
+                    MSATX_first_sec_sid,
+                    MSATX_tot_secs,
+                ),
                 file=logfile,
             )
         nent = sec_size // 4  # number of SID entries in a sector
         fmt = "<%di" % nent
         trunc_warned = 0
         #
         # === build the MSAT ===
```

### Comparing `excelrd-2.0.3/excelrd/formatting.py` & `excelrd-3.0.0/excelrd/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         print(
             "nearest_colour_index for %r is %r -> %r; best_metric is %d"
             % (rgb, best_colourx, colour_map[best_colourx], best_metric)
         )
     return best_colourx
 
 
-class EqNeAttrs(object):
+class EqNeAttrs:
     """
     This mixin class exists solely so that :class:`Format`, :class:`Font`, and
     :class:`XF` objects can be compared by value of their attributes.
     """
 
     def __eq__(self, other):
         return self.__dict__ == other.__dict__
@@ -323,15 +323,15 @@
     #: Height of the font (in twips). A twip = 1/20 of a point.
     height = 0
 
     #: 1 = Characters are italic.
     italic = 0
 
     #: The name of the font. Example: ``"Arial"``.
-    name = UNICODE_LITERAL("")
+    name = ""
 
     #: 1 = Characters are struck out.
     struck_out = 0
 
     #: Values::
     #:
     #:   0 = None
@@ -366,15 +366,15 @@
     if not book.encoding:
         book.derive_encoding()
     blah = DEBUG or book.verbosity >= 2
     bv = book.biff_version
     k = len(book.font_list)
     if k == 4:
         f = Font()
-        f.name = UNICODE_LITERAL("Dummy Font")
+        f.name = "Dummy Font"
         f.font_index = k
         book.font_list.append(f)
         k += 1
     f = Font()
     f.font_index = k
     book.font_list.append(f)
     if bv >= 50:
@@ -458,15 +458,15 @@
     #:   FDT = 1 # date
     #:   FNU = 2 # number
     #:   FGE = 3 # general
     #:   FTX = 4 # text
     type = FUN
 
     #: The format string
-    format_str = UNICODE_LITERAL("")
+    format_str = ""
 
     def __init__(self, format_key, ty, format_str):
         self.format_key = format_key
         self.type = ty
         self.format_str = format_str
 
 
@@ -532,37 +532,37 @@
 
 std_format_code_types = {}
 for lo, hi, ty in fmt_code_ranges:
     for x in range(lo, hi + 1):
         std_format_code_types[x] = ty
 del lo, hi, ty, x
 
-date_chars = UNICODE_LITERAL("ymdhs")  # year, month/minute, day, hour, second
+date_chars = "ymdhs"  # year, month/minute, day, hour, second
 date_char_dict = {}
 for _c in date_chars + date_chars.upper():
     date_char_dict[_c] = 5
 del _c, date_chars
 
 skip_char_dict = {}
-for _c in UNICODE_LITERAL("$-+/(): "):
+for _c in "$-+/(): ":
     skip_char_dict[_c] = 1
 
 num_char_dict = {
-    UNICODE_LITERAL("0"): 5,
-    UNICODE_LITERAL("#"): 5,
-    UNICODE_LITERAL("?"): 5,
+    "0": 5,
+    "#": 5,
+    "?": 5,
 }
 
 non_date_formats = {
-    UNICODE_LITERAL("0.00E+00"): 1,
-    UNICODE_LITERAL("##0.0E+0"): 1,
-    UNICODE_LITERAL("General"): 1,
-    UNICODE_LITERAL("GENERAL"): 1,  # OOo Calc 1.1.4 does this.
-    UNICODE_LITERAL("general"): 1,  # pyExcelerator 0.6.3 does this.
-    UNICODE_LITERAL("@"): 1,
+    "0.00E+00": 1,
+    "##0.0E+0": 1,
+    "General": 1,
+    "GENERAL": 1,  # OOo Calc 1.1.4 does this.
+    "general": 1,  # pyExcelerator 0.6.3 does this.
+    "@": 1,
 }
 
 fmt_bracketed_sub = re.compile(r"\[[^]]*\]").sub
 
 # Boolean format strings (actual cases)
 # '"Yes";"Yes";"No"'
 # '"True";"True";"False"'
@@ -580,24 +580,24 @@
     # TODO: Find where formats are interpreted in Gnumeric
     # TODO: '[h]\\ \\h\\o\\u\\r\\s' ([h] means don't care about hours > 23)
     state = 0
     s = ""
 
     for c in fmt:
         if state == 0:
-            if c == UNICODE_LITERAL('"'):
+            if c == '"':
                 state = 1
-            elif c in UNICODE_LITERAL(r"\_*"):
+            elif c in r"\_*":
                 state = 2
             elif c in skip_char_dict:
                 pass
             else:
                 s += c
         elif state == 1:
-            if c == UNICODE_LITERAL('"'):
+            if c == '"':
                 state = 0
         elif state == 2:
             # Ignore char after backslash, underscore or asterisk
             state = 0
         assert 0 <= state <= 2
     if book.verbosity >= 4:
         print("is_date_format_string: reduced format is %s" % REPR(s), file=book.logfile)
@@ -881,15 +881,20 @@
             pkd_align2,
             pkd_used,
             pkd_brdbkg1,
             pkd_brdbkg2,
             pkd_brdbkg3,
         ) = unpack(unpack_fmt, data[0:20])
         upkbits(
-            xf.protection, pkd_type_par, ((0, 0x01, "cell_locked"), (1, 0x02, "formula_hidden"),)
+            xf.protection,
+            pkd_type_par,
+            (
+                (0, 0x01, "cell_locked"),
+                (1, 0x02, "formula_hidden"),
+            ),
         )
         upkbits(
             xf,
             pkd_type_par,
             (
                 (2, 0x0004, "is_style"),
                 # Following is not in OOo docs, but is mentioned
@@ -898,20 +903,28 @@
                 (3, 0x0008, "lotus_123_prefix"),  # Meaning is not known.
                 (4, 0xFFF0, "parent_style_index"),
             ),
         )
         upkbits(
             xf.alignment,
             pkd_align1,
-            ((0, 0x07, "hor_align"), (3, 0x08, "text_wrapped"), (4, 0x70, "vert_align"),),
+            (
+                (0, 0x07, "hor_align"),
+                (3, 0x08, "text_wrapped"),
+                (4, 0x70, "vert_align"),
+            ),
         )
         upkbits(
             xf.alignment,
             pkd_align2,
-            ((0, 0x0F, "indent_level"), (4, 0x10, "shrink_to_fit"), (6, 0xC0, "text_direction"),),
+            (
+                (0, 0x0F, "indent_level"),
+                (4, 0x10, "shrink_to_fit"),
+                (6, 0xC0, "text_direction"),
+            ),
         )
         reg = pkd_used >> 2
         attr_stems = [
             "format",
             "font",
             "alignment",
             "border",
@@ -946,43 +959,55 @@
                 (21, 0x01E00000, "diag_line_style"),
             ),
         )
         upkbitsL(xf.background, pkd_brdbkg2, ((26, 0xFC000000, "fill_pattern"),))
         upkbits(
             xf.background,
             pkd_brdbkg3,
-            ((0, 0x007F, "pattern_colour_index"), (7, 0x3F80, "background_colour_index"),),
+            (
+                (0, 0x007F, "pattern_colour_index"),
+                (7, 0x3F80, "background_colour_index"),
+            ),
         )
     elif bv >= 50:
         unpack_fmt = "<HHHBBIi"
         (
             xf.font_index,
             xf.format_key,
             pkd_type_par,
             pkd_align1,
             pkd_orient_used,
             pkd_brdbkg1,
             pkd_brdbkg2,
         ) = unpack(unpack_fmt, data[0:16])
         upkbits(
-            xf.protection, pkd_type_par, ((0, 0x01, "cell_locked"), (1, 0x02, "formula_hidden"),)
+            xf.protection,
+            pkd_type_par,
+            (
+                (0, 0x01, "cell_locked"),
+                (1, 0x02, "formula_hidden"),
+            ),
         )
         upkbits(
             xf,
             pkd_type_par,
             (
                 (2, 0x0004, "is_style"),
                 (3, 0x0008, "lotus_123_prefix"),  # Meaning is not known.
                 (4, 0xFFF0, "parent_style_index"),
             ),
         )
         upkbits(
             xf.alignment,
             pkd_align1,
-            ((0, 0x07, "hor_align"), (3, 0x08, "text_wrapped"), (4, 0x70, "vert_align"),),
+            (
+                (0, 0x07, "hor_align"),
+                (3, 0x08, "text_wrapped"),
+                (4, 0x70, "vert_align"),
+            ),
         )
         orientation = pkd_orient_used & 0x03
         xf.alignment.rotation = [0, 255, 90, 180][orientation]
         reg = pkd_orient_used >> 2
         attr_stems = [
             "format",
             "font",
@@ -1003,15 +1028,18 @@
                 (7, 0x00003F80, "background_colour_index"),
                 (16, 0x003F0000, "fill_pattern"),
             ),
         )
         upkbitsL(
             xf.border,
             pkd_brdbkg1,
-            ((22, 0x01C00000, "bottom_line_style"), (25, 0xFE000000, "bottom_colour_index"),),
+            (
+                (22, 0x01C00000, "bottom_line_style"),
+                (25, 0xFE000000, "bottom_colour_index"),
+            ),
         )
         upkbits(
             xf.border,
             pkd_brdbkg2,
             (
                 (0, 0x00000007, "top_line_style"),
                 (3, 0x00000038, "left_line_style"),
@@ -1029,29 +1057,38 @@
             pkd_type_par,
             pkd_align_orient,
             pkd_used,
             pkd_bkg_34,
             pkd_brd_34,
         ) = unpack(unpack_fmt, data[0:12])
         upkbits(
-            xf.protection, pkd_type_par, ((0, 0x01, "cell_locked"), (1, 0x02, "formula_hidden"),)
+            xf.protection,
+            pkd_type_par,
+            (
+                (0, 0x01, "cell_locked"),
+                (1, 0x02, "formula_hidden"),
+            ),
         )
         upkbits(
             xf,
             pkd_type_par,
             (
                 (2, 0x0004, "is_style"),
                 (3, 0x0008, "lotus_123_prefix"),  # Meaning is not known.
                 (4, 0xFFF0, "parent_style_index"),
             ),
         )
         upkbits(
             xf.alignment,
             pkd_align_orient,
-            ((0, 0x07, "hor_align"), (3, 0x08, "text_wrapped"), (4, 0x30, "vert_align"),),
+            (
+                (0, 0x07, "hor_align"),
+                (3, 0x08, "text_wrapped"),
+                (4, 0x30, "vert_align"),
+            ),
         )
         orientation = (pkd_align_orient & 0xC0) >> 6
         xf.alignment.rotation = [0, 255, 90, 180][orientation]
         reg = pkd_used >> 2
         attr_stems = [
             "format",
             "font",
@@ -1095,22 +1132,37 @@
             pkd_type_prot,
             pkd_used,
             pkd_align_par,
             pkd_bkg_34,
             pkd_brd_34,
         ) = unpack(unpack_fmt, data[0:12])
         upkbits(
-            xf.protection, pkd_type_prot, ((0, 0x01, "cell_locked"), (1, 0x02, "formula_hidden"),)
+            xf.protection,
+            pkd_type_prot,
+            (
+                (0, 0x01, "cell_locked"),
+                (1, 0x02, "formula_hidden"),
+            ),
         )
         upkbits(
             xf,
             pkd_type_prot,
-            ((2, 0x0004, "is_style"), (3, 0x0008, "lotus_123_prefix"),),  # Meaning is not known.
+            (
+                (2, 0x0004, "is_style"),
+                (3, 0x0008, "lotus_123_prefix"),
+            ),  # Meaning is not known.
+        )
+        upkbits(
+            xf.alignment,
+            pkd_align_par,
+            (
+                (0, 0x07, "hor_align"),
+                (3, 0x08, "text_wrapped"),
+            ),
         )
-        upkbits(xf.alignment, pkd_align_par, ((0, 0x07, "hor_align"), (3, 0x08, "text_wrapped"),))
         upkbits(xf, pkd_align_par, ((4, 0xFFF0, "parent_style_index"),))
         reg = pkd_used >> 2
         attr_stems = [
             "format",
             "font",
             "alignment",
             "border",
@@ -1149,15 +1201,22 @@
     elif bv == 21:
         ## Warning: incomplete treatment; formatting_info not fully supported.
         ## Probably need to offset incoming BIFF2 XF[n] to BIFF8-like XF[n+16],
         ## and create XF[0:16] like the standard ones in BIFF8 *AND* add 16 to
         ## all XF references in cell records :-(
         (xf.font_index, format_etc, halign_etc) = unpack("<BxBB", data)
         xf.format_key = format_etc & 0x3F
-        upkbits(xf.protection, format_etc, ((6, 0x40, "cell_locked"), (7, 0x80, "formula_hidden"),))
+        upkbits(
+            xf.protection,
+            format_etc,
+            (
+                (6, 0x40, "cell_locked"),
+                (7, 0x80, "formula_hidden"),
+            ),
+        )
         upkbits(xf.alignment, halign_etc, ((0, 0x07, "hor_align"),))
         for mask, side in ((0x08, "left"), (0x10, "right"), (0x20, "top"), (0x40, "bottom")):
             if halign_etc & mask:
                 colour_index, line_style = 8, 1  # black, thin
             else:
                 colour_index, line_style = 0, 0  # none, none
             setattr(xf.border, side + "_colour_index", colour_index)
@@ -1187,15 +1246,17 @@
         raise XLRDError("programmer stuff-up: bv=%d" % bv)
 
     xf.xf_index = len(self.xf_list)
     self.xf_list.append(xf)
     self.xfcount += 1
     if blah:
         xf.dump(
-            self.logfile, header="--- handle_xf: xf[%d] ---" % xf.xf_index, footer=" ",
+            self.logfile,
+            header="--- handle_xf: xf[%d] ---" % xf.xf_index,
+            footer=" ",
         )
     try:
         fmt = self.format_map[xf.format_key]
         cellty = _cellty_from_fmtty[fmt.type]
     except KeyError:
         cellty = XL_CELL_NUMBER
     self._xf_index_to_xl_type_map[xf.xf_index] = cellty
```

### Comparing `excelrd-2.0.3/excelrd/formula.py` & `excelrd-3.0.0/excelrd/formula.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 import copy
 import operator as opr
 from struct import unpack
 
 from .biffh import (
-    BaseObject,
     XLRDError,
     error_text_from_code,
     hex_char_dump,
     unpack_string_update_pos,
     unpack_unicode_update_pos,
 )
 from .timemachine import *
@@ -794,15 +793,15 @@
     0x08: "Skip",
     0x10: "Sum",
     0x20: "Assign",
     0x40: "Space",
     0x41: "SpaceVolatile",
 }
 
-error_opcodes = set([0x07, 0x08, 0x0A, 0x0B, 0x1C, 0x1D, 0x2F])
+error_opcodes = {0x07, 0x08, 0x0A, 0x0B, 0x1C, 0x1D, 0x2F}
 
 tRangeFuncs = (min, max, min, max, min, max)
 tIsectFuncs = (max, min, max, min, max, min)
 
 
 def do_box_funcs(box_funcs, boxa, boxb):
     return tuple(func(numa, numb) for func, numa, numb in zip(box_funcs, boxa.coords, boxb.coords))
@@ -952,15 +951,15 @@
     return xlrd_sheetx1, xlrd_sheetx2
 
 
 class FormulaError(Exception):
     pass
 
 
-class Operand(object):
+class Operand:
     """
     Used in evaluating formulas.
     The following table describes the kinds and how their values
     are represented.
 
     .. raw:: html
 
@@ -1040,15 +1039,15 @@
         self.rank = arank
         # rank is an internal gizmo (operator precedence);
         # it's used in reconstructing formula text.
         self.text = atext
 
     def __repr__(self):
         kind_text = okind_dict.get(self.kind, "?Unknown kind?")
-        return "Operand(kind=%s, value=%r, text=%r)" % (kind_text, self.value, self.text)
+        return f"Operand(kind={kind_text}, value={self.value!r}, text={self.text!r})"
 
 
 class Ref3D(tuple):
     """
     Represents an absolute or relative 3-dimensional reference to a box
     of one or more cells.
 
@@ -1101,17 +1100,17 @@
         self.relflags = atuple[6:12]
         if not self.relflags:
             self.relflags = (0, 0, 0, 0, 0, 0)
         (self.shtxlo, self.shtxhi, self.rowxlo, self.rowxhi, self.colxlo, self.colxhi) = self.coords
 
     def __repr__(self):
         if not self.relflags or self.relflags == (0, 0, 0, 0, 0, 0):
-            return "Ref3D(coords=%r)" % (self.coords,)
+            return f"Ref3D(coords={self.coords!r})"
         else:
-            return "Ref3D(coords=%r, relflags=%r)" % (self.coords, self.relflags)
+            return f"Ref3D(coords={self.coords!r}, relflags={self.relflags!r})"
 
 
 tAdd = 0x03
 tSub = 0x04
 tMul = 0x05
 tDiv = 0x06
 tPower = 0x07
@@ -1120,15 +1119,15 @@
 
 
 def nop(x):
     return x
 
 
 def _opr_pow(x, y):
-    return x ** y
+    return x**y
 
 
 def _opr_lt(x, y):
     return x < y
 
 
 def _opr_le(x, y):
@@ -1166,15 +1165,15 @@
 # Seems no conversions done on relops; in Excel, "1" > 9 produces TRUE.
 _strg_argdict = {oNUM: num2strg, oSTRG: nop}
 binop_rules = {
     tAdd: (_arith_argdict, oNUM, opr.add, 30, "+"),
     tSub: (_arith_argdict, oNUM, opr.sub, 30, "-"),
     tMul: (_arith_argdict, oNUM, opr.mul, 40, "*"),
     tDiv: (_arith_argdict, oNUM, opr.truediv, 40, "/"),
-    tPower: (_arith_argdict, oNUM, _opr_pow, 50, "^",),
+    tPower: (_arith_argdict, oNUM, _opr_pow, 50, "^"),
     tConcat: (_strg_argdict, oSTRG, opr.add, 20, "&"),
     tLT: (_cmp_argdict, oBOOL, _opr_lt, 10, "<"),
     tLE: (_cmp_argdict, oBOOL, _opr_le, 10, "<="),
     tEQ: (_cmp_argdict, oBOOL, _opr_eq, 10, "="),
     tGE: (_cmp_argdict, oBOOL, _opr_ge, 10, ">="),
     tGT: (_cmp_argdict, oBOOL, _opr_gt, 10, ">"),
     tNE: (_cmp_argdict, oBOOL, _opr_ne, 10, "<>"),
@@ -1254,21 +1253,29 @@
         stk.append(resop)
 
     def do_unaryop(opcode, result_kind, stk):
         assert len(stk) >= 1
         aop = stk.pop()
         val = aop.value
         func, rank, sym1, sym2 = unop_rules[opcode]
-        otext = "".join([sym1, "("[: aop.rank < rank], aop.text, ")"[: aop.rank < rank], sym2,])
+        otext = "".join(
+            [
+                sym1,
+                "("[: aop.rank < rank],
+                aop.text,
+                ")"[: aop.rank < rank],
+                sym2,
+            ]
+        )
         if val is not None:
             val = func(val)
         stk.append(Operand(result_kind, val, rank, otext))
 
     def not_in_name_formula(op_arg, oname_arg):
-        msg = "ERROR *** Token 0x%02x (%s) found in NAME formula" % (op_arg, oname_arg)
+        msg = f"ERROR *** Token 0x{op_arg:02x} ({oname_arg}) found in NAME formula"
         raise FormulaError(msg)
 
     if fmlalen == 0:
         stack = [unk_opnd]
 
     while 0 <= pos < fmlalen:
         op = BYTES_ORD(data[pos])
@@ -1509,15 +1516,15 @@
                     print(
                         "    FuncID=%d name=%s nargs=%d" % (funcx, func_name, nargs),
                         file=bk.logfile,
                     )
                 assert len(stack) >= nargs
                 if nargs:
                     argtext = listsep.join(arg.text for arg in stack[-nargs:])
-                    otext = "%s(%s)" % (func_name, argtext)
+                    otext = f"{func_name}({argtext})"
                     del stack[-nargs:]
                 else:
                     otext = func_name + "()"
                 res = Operand(oUNK, None, FUNC_RANK, otext)
                 spush(res)
         elif opcode == 0x02:  # tFuncVar
             nb = 1 + int(bv >= 40)
@@ -1540,15 +1547,15 @@
                         "    name: %r, min~max args: %d~%d" % (func_name, minargs, maxargs),
                         file=bk.logfile,
                     )
                 assert minargs <= nargs <= maxargs
                 assert len(stack) >= nargs
                 assert len(stack) >= nargs
                 argtext = listsep.join(arg.text for arg in stack[-nargs:])
-                otext = "%s(%s)" % (func_name, argtext)
+                otext = f"{func_name}({argtext})"
                 res = Operand(oUNK, None, FUNC_RANK, otext)
                 if funcx == 1:  # IF
                     testarg = stack[-nargs]
                     if testarg.kind not in (oNUM, oBOOL):
                         if blah and testarg.kind != oUNK:
                             print("IF testarg kind?", file=bk.logfile)
                     elif testarg.value not in (0, 1):
@@ -1600,15 +1607,15 @@
             else:
                 assert len(tgtobj.stack) == 1
                 res = copy.deepcopy(tgtobj.stack[0])
             res.rank = LEAF_RANK
             if tgtobj.scope == -1:
                 res.text = tgtobj.name
             else:
-                res.text = "%s!%s" % (bk._sheet_names[tgtobj.scope], tgtobj.name)
+                res.text = f"{bk._sheet_names[tgtobj.scope]}!{tgtobj.name}"
             if blah:
                 print("    tName: setting text to", repr(res.text), file=bk.logfile)
             spush(res)
         elif opcode == 0x04:  # tRef
             # not_in_name_formula(op, oname)
             res = get_cell_addr(data, pos + 1, bv, reldelta)
             if blah:
@@ -1776,27 +1783,29 @@
                 tgtobj = bk.name_obj_list[tgtnamex]
                 if not tgtobj.evaluated:
                     ### recursive ###
                     evaluate_name_formula(bk, tgtobj, tgtnamex, blah, level + 1)
                 if tgtobj.macro or tgtobj.binary or tgtobj.any_err:
                     if blah:
                         tgtobj.dump(
-                            bk.logfile, header="!!! bad tgtobj !!!", footer="------------------",
+                            bk.logfile,
+                            header="!!! bad tgtobj !!!",
+                            footer="------------------",
                         )
                     res = Operand(oUNK, None)
                     any_err = any_err or tgtobj.macro or tgtobj.binary or tgtobj.any_err
                     any_rel = any_rel or tgtobj.any_rel
                 else:
                     assert len(tgtobj.stack) == 1
                     res = copy.deepcopy(tgtobj.stack[0])
                 res.rank = LEAF_RANK
                 if tgtobj.scope == -1:
                     res.text = tgtobj.name
                 else:
-                    res.text = "%s!%s" % (bk._sheet_names[tgtobj.scope], tgtobj.name)
+                    res.text = f"{bk._sheet_names[tgtobj.scope]}!{tgtobj.name}"
                 if blah:
                     print("    tNameX: setting text to", repr(res.text), file=bk.logfile)
             spush(res)
         elif opcode in error_opcodes:
             any_err = 1
             spush(error_opnd)
         else:
@@ -1881,19 +1890,27 @@
         resop = Operand(result_kind, None, rank, otext)
         stk.append(resop)
 
     def do_unaryop(opcode, result_kind, stk):
         assert len(stk) >= 1
         aop = stk.pop()
         func, rank, sym1, sym2 = unop_rules[opcode]
-        otext = "".join([sym1, "("[: aop.rank < rank], aop.text, ")"[: aop.rank < rank], sym2,])
+        otext = "".join(
+            [
+                sym1,
+                "("[: aop.rank < rank],
+                aop.text,
+                ")"[: aop.rank < rank],
+                sym2,
+            ]
+        )
         stk.append(Operand(result_kind, None, rank, otext))
 
     def unexpected_opcode(op_arg, oname_arg):
-        msg = "ERROR *** Unexpected token 0x%02x (%s) found in formula type %s" % (
+        msg = "ERROR *** Unexpected token 0x{:02x} ({}) found in formula type {}".format(
             op_arg,
             oname_arg,
             FMLA_TYPEDESCR_MAP[fmlatype],
         )
         print(msg, file=bk.logfile)
         # raise FormulaError(msg)
 
@@ -2120,15 +2137,15 @@
                     print(
                         "    FuncID=%d name=%s nargs=%d" % (funcx, func_name, nargs),
                         file=bk.logfile,
                     )
                 assert len(stack) >= nargs
                 if nargs:
                     argtext = listsep.join(arg.text for arg in stack[-nargs:])
-                    otext = "%s(%s)" % (func_name, argtext)
+                    otext = f"{func_name}({argtext})"
                     del stack[-nargs:]
                 else:
                     otext = func_name + "()"
                 res = Operand(oUNK, None, FUNC_RANK, otext)
                 spush(res)
         elif opcode == 0x02:  # tFuncVar
             nb = 1 + int(bv >= 40)
@@ -2155,28 +2172,28 @@
                         "    name: %r, min~max args: %d~%d" % (func_name, minargs, maxargs),
                         file=bk.logfile,
                     )
                 assert minargs <= nargs <= maxargs
                 assert len(stack) >= nargs
                 assert len(stack) >= nargs
                 argtext = listsep.join(arg.text for arg in stack[-nargs:])
-                otext = "%s(%s)" % (func_name, argtext)
+                otext = f"{func_name}({argtext})"
                 res = Operand(oUNK, None, FUNC_RANK, otext)
                 del stack[-nargs:]
                 spush(res)
         elif opcode == 0x03:  # tName
             tgtnamex = unpack("<H", data[pos + 1 : pos + 3])[0] - 1
             # Only change with BIFF version is number of trailing UNUSED bytes!
             if blah:
                 print("   tgtnamex=%d" % tgtnamex, file=bk.logfile)
             tgtobj = bk.name_obj_list[tgtnamex]
             if tgtobj.scope == -1:
                 otext = tgtobj.name
             else:
-                otext = "%s!%s" % (bk._sheet_names[tgtobj.scope], tgtobj.name)
+                otext = f"{bk._sheet_names[tgtobj.scope]}!{tgtobj.name}"
             if blah:
                 print("    tName: setting text to", repr(otext), file=bk.logfile)
             res = Operand(oUNK, None, LEAF_RANK, otext)
             spush(res)
         elif opcode == 0x04:  # tRef
             res = get_cell_addr(data, pos + 1, bv, reldelta, browx, bcolx)
             if blah:
@@ -2362,15 +2379,15 @@
             elif dodgy or shx1 < -1:
                 otext = "<<Name #%d in external(?) file #%d>>" % (tgtnamex, origrefx)
             else:
                 tgtobj = bk.name_obj_list[tgtnamex]
                 if tgtobj.scope == -1:
                     otext = tgtobj.name
                 else:
-                    otext = "%s!%s" % (bk._sheet_names[tgtobj.scope], tgtobj.name)
+                    otext = f"{bk._sheet_names[tgtobj.scope]}!{tgtobj.name}"
                 if blah:
                     print("    tNameX: setting text to", repr(res.text), file=bk.logfile)
             res = Operand(okind, ovalue, LEAF_RANK, otext)
             spush(res)
         elif opcode in error_opcodes:
             any_err = 1
             spush(error_opnd)
@@ -2664,44 +2681,44 @@
         return alphabet[colx]
     else:
         xdiv26, xmod26 = divmod(colx, 26)
         return alphabet[xdiv26 - 1] + alphabet[xmod26]
 
 
 def rangename2d(rlo, rhi, clo, chi, r1c1=0):
-    """ ``(5, 20, 7, 10)`` => ``'$H$6:$J$20'`` """
+    """``(5, 20, 7, 10)`` => ``'$H$6:$J$20'``"""
     if r1c1:
         return
     if rhi == rlo + 1 and chi == clo + 1:
         return cellnameabs(rlo, clo, r1c1)
-    return "%s:%s" % (cellnameabs(rlo, clo, r1c1), cellnameabs(rhi - 1, chi - 1, r1c1))
+    return f"{cellnameabs(rlo, clo, r1c1)}:{cellnameabs(rhi - 1, chi - 1, r1c1)}"
 
 
 def rangename2drel(rlo_rhi_clo_chi, rlorel_rhirel_clorel_chirel, browx=None, bcolx=None, r1c1=0):
     rlo, rhi, clo, chi = rlo_rhi_clo_chi
     rlorel, rhirel, clorel, chirel = rlorel_rhirel_clorel_chirel
     if (rlorel or rhirel) and browx is None:
         r1c1 = True
     if (clorel or chirel) and bcolx is None:
         r1c1 = True
-    return "%s:%s" % (
+    return "{}:{}".format(
         cellnamerel(rlo, clo, rlorel, clorel, browx, bcolx, r1c1),
         cellnamerel(rhi - 1, chi - 1, rhirel, chirel, browx, bcolx, r1c1),
     )
 
 
 def rangename3d(book, ref3d):
     """
     Utility function:
     ``Ref3D(1, 4, 5, 20, 7, 10)`` =>
     ``'Sheet2:Sheet3!$H$6:$J$20'``
     (assuming Excel's default sheetnames)
     """
     coords = ref3d.coords
-    return "%s!%s" % (sheetrange(book, *coords[:2]), rangename2d(*coords[2:6]))
+    return f"{sheetrange(book, *coords[:2])}!{rangename2d(*coords[2:6])}"
 
 
 def rangename3drel(book, ref3d, browx=None, bcolx=None, r1c1=0):
     """
     Utility function:
     ``Ref3D(coords=(0, 1, -32, -22, -13, 13), relflags=(0, 0, 1, 1, 1, 1))``
 
@@ -2711,15 +2728,15 @@
     """
     coords = ref3d.coords
     relflags = ref3d.relflags
     shdesc = sheetrangerel(book, coords[:2], relflags[:2])
     rngdesc = rangename2drel(coords[2:6], relflags[2:6], browx, bcolx, r1c1)
     if not shdesc:
         return rngdesc
-    return "%s!%s" % (shdesc, rngdesc)
+    return f"{shdesc}!{rngdesc}"
 
 
 def quotedsheetname(shnames, shx):
     if shx >= 0:
         shname = shnames[shx]
     else:
         shname = {
```

### Comparing `excelrd-2.0.3/excelrd/sheet.py` & `excelrd-3.0.0/excelrd/sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,15 +398,19 @@
         """
         :class:`Cell` object in the given row and column.
         """
         if self.formatting_info:
             xfx = self.cell_xf_index(rowx, colx)
         else:
             xfx = None
-        return Cell(self._cell_types[rowx][colx], self._cell_values[rowx][colx], xfx,)
+        return Cell(
+            self._cell_types[rowx][colx],
+            self._cell_values[rowx][colx],
+            xfx,
+        )
 
     def cell_value(self, rowx, colx):
         "Value of the cell in the given row and column."
         return self._cell_values[rowx][colx]
 
     def cell_type(self, rowx, colx):
         """
@@ -565,15 +569,18 @@
 
     # === Following methods are used in building the worksheet.
     # === They are not part of the API.
 
     def tidy_dimensions(self):
         if self.verbosity >= 3:
             fprintf(
-                self.logfile, "tidy_dimensions: nrows=%d ncols=%d \n", self.nrows, self.ncols,
+                self.logfile,
+                "tidy_dimensions: nrows=%d ncols=%d \n",
+                self.nrows,
+                self.ncols,
             )
         if 1 and self.merged_cells:
             nr = nc = 0
             umaxrows = self.utter_max_rows
             umaxcols = self.utter_max_cols
             for crange in self.merged_cells:
                 rlo, rhi, clo, chi = crange
@@ -592,15 +599,15 @@
             if nc > self.ncols:
                 self.ncols = nc
                 self._first_full_rowx = -2
             if nr > self.nrows:
                 # we put one empty cell at (nr-1,0) to make sure
                 # we have the right number of rows. The ragged rows
                 # will sort out the rest if needed.
-                self.put_cell(nr - 1, 0, XL_CELL_EMPTY, UNICODE_LITERAL(""), -1)
+                self.put_cell(nr - 1, 0, XL_CELL_EMPTY, "", -1)
         if self.verbosity >= 1 and (self.nrows != self._dimnrows or self.ncols != self._dimncols):
             fprintf(
                 self.logfile,
                 "NOTE *** sheet %d (%r): DIMENSIONS R,C = %d,%d should be %d,%d\n",
                 self.number,
                 self.name,
                 self._dimnrows,
@@ -621,15 +628,15 @@
             else:
                 ubound = self._first_full_rowx
             for rowx in range(ubound):
                 trow = s_cell_types[rowx]
                 rlen = len(trow)
                 nextra = ncols - rlen
                 if nextra > 0:
-                    s_cell_values[rowx][rlen:] = [UNICODE_LITERAL("")] * nextra
+                    s_cell_values[rowx][rlen:] = [""] * nextra
                     trow[rlen:] = self.bt * nextra
                     if s_fmt_info:
                         s_cell_xf_indexes[rowx][rlen:] = self.bf * nextra
 
     def put_cell_ragged(self, rowx, colx, ctype, value, xf_index):
         if ctype is None:
             # we have a number, so look up the cell type
@@ -637,15 +644,14 @@
         assert 0 <= colx < self.utter_max_cols
         assert 0 <= rowx < self.utter_max_rows
         fmt_info = self.formatting_info
 
         try:
             nr = rowx + 1
             if self.nrows < nr:
-
                 scta = self._cell_types.append
                 scva = self._cell_values.append
                 scxa = self._cell_xf_indexes.append
                 bt = self.bt
                 bf = self.bf
                 for _unused in range(self.nrows, nr):
                     scta(bt * 0)
@@ -670,19 +676,19 @@
                 if fmt_info:
                     fmt_row.append(xf_index)
                 return
             if num_empty > 0:
                 num_empty += 1
                 # self._put_cell_row_widenings += 1
                 # types_row.extend(self.bt * num_empty)
-                # values_row.extend([UNICODE_LITERAL('')] * num_empty)
+                # values_row.extend([''] * num_empty)
                 # if fmt_info:
                 #     fmt_row.extend(self.bf * num_empty)
                 types_row[ltr:] = self.bt * num_empty
-                values_row[ltr:] = [UNICODE_LITERAL("")] * num_empty
+                values_row[ltr:] = [""] * num_empty
                 if fmt_info:
                     fmt_row[ltr:] = self.bf * num_empty
             types_row[colx] = ctype
             values_row[colx] = value
             if fmt_info:
                 fmt_row[colx] = xf_index
         except:
@@ -728,27 +734,27 @@
                 trow = self._cell_types[rowx]
                 nextra = self.ncols - len(trow)
                 if nextra > 0:
                     # self._put_cell_row_widenings += 1
                     trow.extend(self.bt * nextra)
                     if self.formatting_info:
                         self._cell_xf_indexes[rowx].extend(self.bf * nextra)
-                    self._cell_values[rowx].extend([UNICODE_LITERAL("")] * nextra)
+                    self._cell_values[rowx].extend([""] * nextra)
             else:
                 scta = self._cell_types.append
                 scva = self._cell_values.append
                 scxa = self._cell_xf_indexes.append
                 fmt_info = self.formatting_info
                 nc = self.ncols
                 bt = self.bt
                 bf = self.bf
                 for _unused in range(self.nrows, nr):
                     # self._put_cell_rows_appended += 1
                     scta(bt * nc)
-                    scva([UNICODE_LITERAL("")] * nc)
+                    scva([""] * nc)
                     if fmt_info:
                         scxa(bf * nc)
                 self.nrows = nr
             # === end of code from extend_cells()
             try:
                 self._cell_types[rowx][colx] = ctype
                 self._cell_values[rowx][colx] = value
@@ -1184,18 +1190,26 @@
                 if DEBUG:
                     print("---> found EOF", file=self.logfile)
             elif rc == XL_COUNTRY:
                 bk.handle_country(data)
             elif rc == XL_LABELRANGES:
                 pos = 0
                 pos = unpack_cell_range_address_list_update_pos(
-                    self.row_label_ranges, data, pos, bv, addr_size=8,
+                    self.row_label_ranges,
+                    data,
+                    pos,
+                    bv,
+                    addr_size=8,
                 )
                 pos = unpack_cell_range_address_list_update_pos(
-                    self.col_label_ranges, data, pos, bv, addr_size=8,
+                    self.col_label_ranges,
+                    data,
+                    pos,
+                    bv,
+                    addr_size=8,
                 )
                 assert pos == data_len
             elif rc == XL_ARRAY:
                 row1x, rownx, col1x, colnx, array_flags, tokslen = local_unpack(
                     "<HHBBBxxxxxH", data[:14]
                 )
                 if blah_formulas:
@@ -1357,17 +1371,19 @@
                         self.first_visible_colx,
                         self.gridline_colour_index,
                         self.cached_page_break_preview_mag_factor,
                         self.cached_normal_view_mag_factor,
                     ) = unpack("<HHHHxxHH", data[:14])
                 else:
                     assert bv >= 30  # BIFF3-7
-                    (options, self.first_visible_rowx, self.first_visible_colx,) = unpack(
-                        "<HHH", data[:6]
-                    )
+                    (
+                        options,
+                        self.first_visible_rowx,
+                        self.first_visible_colx,
+                    ) = unpack("<HHH", data[:6])
                     self.gridline_colour_rgb = unpack("<BBB", data[6:9])
                     self.gridline_colour_index = nearest_colour_index(
                         self.book.colour_map, self.gridline_colour_rgb, debug=0
                     )
                 # options -- Bit, Mask, Contents:
                 # 0 0001H 0 = Show formula results 1 = Show formulas
                 # 1 0002H 0 = Do not show grid lines 1 = Show grid lines
@@ -1643,15 +1659,15 @@
         bk = self.book
         lenlen = (bv >= 30) + 1
         nchars_expected = unpack("<" + "BH"[lenlen - 1], data[:lenlen])[0]
         offset = lenlen
         if bv < 80:
             enc = bk.encoding or bk.derive_encoding()
         nchars_found = 0
-        result = UNICODE_LITERAL("")
+        result = ""
         while 1:
             if bv >= 80:
                 flag = BYTES_ORD(data[offset]) & 1
                 enc = ("latin_1", "utf_16_le")[flag]
                 offset += 1
             chunk = str(data[offset:], enc)
             result += chunk
@@ -1760,15 +1776,15 @@
         book.xf_list.append(xf)
         if blah:
             xf.dump(self.logfile, header="=== Faked XF %d ===" % xfx, footer="======")
         if xf.format_key not in book.format_map:
             if xf.format_key:
                 msg = "ERROR *** XF[%d] unknown format key (%d, 0x%04x)\n"
                 fprintf(self.logfile, msg, xf.xf_index, xf.format_key, xf.format_key)
-            fmt = Format(xf.format_key, FUN, UNICODE_LITERAL("General"))
+            fmt = Format(xf.format_key, FUN, "General")
             book.format_map[xf.format_key] = fmt
             book.format_list.append(fmt)
         cellty_from_fmtty = {
             FNU: XL_CELL_NUMBER,
             FUN: XL_CELL_NUMBER,
             FGE: XL_CELL_NUMBER,
             FDT: XL_CELL_DATE,
@@ -1777,15 +1793,15 @@
         fmt = book.format_map[xf.format_key]
         cellty = cellty_from_fmtty[fmt.type]
         self._xf_index_to_xl_type_map[xf.xf_index] = cellty
         self._cell_attr_to_xfx[cell_attr] = xfx
         return xfx
 
     def fake_XF_from_BIFF20_cell_attr(self, cell_attr, style=0):
-        from .formatting import XF, XFAlignment, XFBorder, XFBackground, XFProtection
+        from .formatting import XF, XFAlignment, XFBackground, XFBorder, XFProtection
 
         xf = XF()
         xf.alignment = XFAlignment()
         xf.alignment.indent_level = 0
         xf.alignment.shrink_to_fit = 0
         xf.alignment.text_direction = 0
         xf.border = XFBorder()
@@ -1794,15 +1810,22 @@
         xf.border.diag_colour_index = 0
         xf.border.diag_line_style = 0  # no line
         xf.background = XFBackground()
         xf.protection = XFProtection()
         (prot_bits, font_and_format, halign_etc) = unpack("<BBB", cell_attr)
         xf.format_key = font_and_format & 0x3F
         xf.font_index = (font_and_format & 0xC0) >> 6
-        upkbits(xf.protection, prot_bits, ((6, 0x40, "cell_locked"), (7, 0x80, "formula_hidden"),))
+        upkbits(
+            xf.protection,
+            prot_bits,
+            (
+                (6, 0x40, "cell_locked"),
+                (7, 0x80, "formula_hidden"),
+            ),
+        )
         xf.alignment.hor_align = halign_etc & 0x07
         for mask, side in ((0x08, "left"), (0x10, "right"), (0x20, "top"), (0x40, "bottom")):
             if halign_etc & mask:
                 colour_index, line_style = 8, 1  # black, thin
             else:
                 colour_index, line_style = 0, 0  # none, none
             setattr(xf.border, side + "_colour_index", colour_index)
@@ -1905,15 +1928,15 @@
             (clsid,) = unpack("<16s", data[offset : offset + 16])
             if DEBUG:
                 fprintf(self.logfile, "clsid=%r\n", clsid)
             offset += 16
             if clsid == b"\xE0\xC9\xEA\x79\xF9\xBA\xCE\x11\x8C\x82\x00\xAA\x00\x4B\xA9\x0B":
                 #          E0H C9H EAH 79H F9H BAH CEH 11H 8CH 82H 00H AAH 00H 4BH A9H 0BH
                 # URL Moniker
-                h.type = UNICODE_LITERAL("url")
+                h.type = "url"
                 nbytes = unpack("<L", data[offset : offset + 4])[0]
                 offset += 4
                 h.url_or_path = str(data[offset : offset + nbytes], "UTF-16le")
                 if DEBUG:
                     fprintf(
                         self.logfile, "initial url=%r len=%d\n", h.url_or_path, len(h.url_or_path)
                     )
@@ -1935,15 +1958,15 @@
                         nbytes,
                         true_nbytes,
                         extra_nbytes,
                     )
                 assert extra_nbytes in (24, 0)
             elif clsid == b"\x03\x03\x00\x00\x00\x00\x00\x00\xC0\x00\x00\x00\x00\x00\x00\x46":
                 # file moniker
-                h.type = UNICODE_LITERAL("local file")
+                h.type = "local file"
                 uplevels, nbytes = unpack("<Hi", data[offset : offset + 6])
                 offset += 6
                 shortpath = (
                     b"..\\" * uplevels + data[offset : offset + nbytes - 1]
                 )  #### BYTES, not unicode
                 if DEBUG:
                     fprintf(self.logfile, "uplevels=%d shortpath=%r\n", uplevels, shortpath)
@@ -1966,20 +1989,20 @@
                 else:
                     h.url_or_path = shortpath
                     #### MS KLUDGE WARNING ####
                     # The "shortpath" is bytes encoded in the **UNKNOWN** creator's "ANSI" encoding.
             else:
                 fprintf(self.logfile, "*** unknown clsid %r\n", clsid)
         elif options & 0x163 == 0x103:  # UNC
-            h.type = UNICODE_LITERAL("unc")
+            h.type = "unc"
             h.url_or_path, offset = get_nul_terminated_unicode(data, offset)
         elif options & 0x16B == 8:
-            h.type = UNICODE_LITERAL("workbook")
+            h.type = "workbook"
         else:
-            h.type = UNICODE_LITERAL("unknown")
+            h.type = "unknown"
 
         if options & 0x8:  # has textmark
             h.textmark, offset = get_nul_terminated_unicode(data, offset)
 
         if DEBUG:
             h.dump(header="... object dump ...")
             print("offset=%d record_size=%d" % (offset, record_size))
@@ -2145,15 +2168,15 @@
             assert expected_bytes == 0
             enc = self.book.encoding or self.book.derive_encoding()
             o.text = str(b"".join(pieces), enc)
             o.rich_text_runlist = [(0, 0)]
             o.show = 0
             o.row_hidden = 0
             o.col_hidden = 0
-            o.author = UNICODE_LITERAL("")
+            o.author = ""
             o._object_id = None
             self.cell_note_map[o.rowx, o.colx] = o
             return
         # Excel 8.0+
         o.rowx, o.colx, option_flags, o._object_id = unpack("<4H", data[:8])
         o.show = (option_flags >> 1) & 1
         o.row_hidden = (option_flags >> 7) & 1
@@ -2189,15 +2212,15 @@
                 (6, 0x0070, "vert_align"),
                 (9, 0x0200, "lock_text"),
                 (14, 0x4000, "just_last"),
                 (15, 0x8000, "secret_edit"),
             ),
         )
         totchars = 0
-        o.text = UNICODE_LITERAL("")
+        o.text = ""
         while totchars < cchText:
             rc2, data2_len, data2 = self.book.get_record_parts()
             assert rc2 == XL_CONTINUE
             if OBJ_MSO_DEBUG:
                 hex_char_dump(data2, 0, data2_len, base=0, fout=self.logfile)
             nb = BYTES_ORD(data2[0])  # 0 means latin1, 1 means utf_16_le
             nchars = data2_len - 1
@@ -2312,15 +2335,15 @@
                 rgbHashParam,
                 cchName,
             ),
             file=self.logfile,
         )
 
     def __repr__(self):
-        return "Sheet {:>2}:<{}>".format(self.number, self.name)
+        return f"Sheet {self.number:>2}:<{self.name}>"
 
 
 class MSODrawing(BaseObject):
     pass
 
 
 class MSObj(BaseObject):
@@ -2336,15 +2359,15 @@
     Represents a user "comment" or "note".
     Note objects are accessible through :attr:`Sheet.cell_note_map`.
 
     .. versionadded:: 0.7.2
     """
 
     #: Author of note
-    author = UNICODE_LITERAL("")
+    author = ""
 
     #: ``True`` if the containing column is hidden
     col_hidden = 0
 
     #: Column index
     colx = 0
 
@@ -2359,15 +2382,15 @@
     #: Row index
     rowx = 0
 
     #: True if note is always shown
     show = 0
 
     #: Text of the note
-    text = UNICODE_LITERAL("")
+    text = ""
 
 
 class Hyperlink(BaseObject):
     """
     Contains the attributes of a hyperlink.
     Hyperlink objects are accessible through :attr:`Sheet.hyperlink_list`
     and :attr:`Sheet.hyperlink_map`.
@@ -2533,20 +2556,20 @@
     def __init__(self, ctype, value, xf_index=None):
         self.ctype = ctype
         self.value = value
         self.xf_index = xf_index
 
     def __repr__(self):
         if self.xf_index is None:
-            return "%s:%r" % (ctype_text[self.ctype], self.value)
+            return f"{ctype_text[self.ctype]}:{self.value!r}"
         else:
-            return "%s:%r (XF:%r)" % (ctype_text[self.ctype], self.value, self.xf_index)
+            return f"{ctype_text[self.ctype]}:{self.value!r} (XF:{self.xf_index!r})"
 
 
-empty_cell = Cell(XL_CELL_EMPTY, UNICODE_LITERAL(""))
+empty_cell = Cell(XL_CELL_EMPTY, "")
 
 ##### =============== Colinfo and Rowinfo ============================== #####
 
 
 class Colinfo(BaseObject):
     """
     Width and default formatting information that applies to one or
```

### Comparing `excelrd-2.0.3/excelrd/timemachine.py` & `excelrd-3.0.0/excelrd/timemachine.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,27 +3,22 @@
 # <p>This module is part of the excelrd package, which is released under a BSD-style licence.</p>
 ##
 
 # timemachine.py -- adaptation for single codebase.
 # Currently supported: 2.6 to 2.7, 3.2+
 # usage: from timemachine import *
 
-import sys
-from io import BytesIO as BYTES_IO
-
 
 BYTES_LITERAL = lambda x: x.encode("latin1")
-UNICODE_LITERAL = lambda x: x
 BYTES_ORD = lambda byte: byte
 
 
 def fprintf(f, fmt, *vargs):
     fmt = fmt.replace("%r", "%a")
     if fmt.endswith("\n"):
         print(fmt[:-1] % vargs, file=f)
     else:
         print(fmt % vargs, end=" ", file=f)
 
 
 EXCEL_TEXT_TYPES = (str, bytes, bytearray)  # xlwt: isinstance(obj, EXCEL_TEXT_TYPES)
 REPR = ascii
-ensure_unicode = lambda s: s
```

### Comparing `excelrd-2.0.3/excelrd/xldate.py` & `excelrd-3.0.0/excelrd/xldate.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,33 +194,33 @@
     if datemode not in (0, 1):
         raise XLDateBadDatemode(datemode)
 
     if year == 0 and month == 0 and day == 0:
         return 0.00
 
     if not (1900 <= year <= 9999):
-        raise XLDateBadTuple("Invalid year: %r" % ((year, month, day),))
+        raise XLDateBadTuple(f"Invalid year: {(year, month, day)!r}")
     if not (1 <= month <= 12):
-        raise XLDateBadTuple("Invalid month: %r" % ((year, month, day),))
+        raise XLDateBadTuple(f"Invalid month: {(year, month, day)!r}")
     if day < 1 or (day > _days_in_month[month] and not (day == 29 and month == 2 and _leap(year))):
-        raise XLDateBadTuple("Invalid day: %r" % ((year, month, day),))
+        raise XLDateBadTuple(f"Invalid day: {(year, month, day)!r}")
 
     Yp = year + 4716
     M = month
     if M <= 2:
         Yp = Yp - 1
         Mp = M + 9
     else:
         Mp = M - 3
     jdn = (1461 * Yp // 4) + ((979 * Mp + 16) // 32) + day - 1364 - (((Yp + 184) // 100) * 3 // 4)
     xldays = jdn - _JDN_delta[datemode]
     if xldays <= 0:
-        raise XLDateBadTuple("Invalid (year, month, day): %r" % ((year, month, day),))
+        raise XLDateBadTuple(f"Invalid (year, month, day): {(year, month, day)!r}")
     if xldays < 61 and datemode == 0:
-        raise XLDateAmbiguous("Before 1900-03-01: %r" % ((year, month, day),))
+        raise XLDateAmbiguous(f"Before 1900-03-01: {(year, month, day)!r}")
     return float(xldays)
 
 
 def xldate_from_time_tuple(time_tuple):
     """
     Convert a time tuple ``(hour, minute, second)`` to an Excel "date" value
     (fraction of a day).
@@ -229,15 +229,15 @@
     :param minute: ``0 <= minute < 60``
     :param second: ``0 <= second < 60``
     :raises excelrd.xldate.XLDateBadTuple: Out-of-range hour, minute, or second
     """
     hour, minute, second = time_tuple
     if 0 <= hour < 24 and 0 <= minute < 60 and 0 <= second < 60:
         return ((second / 60.0 + minute) / 60.0 + hour) / 24.0
-    raise XLDateBadTuple("Invalid (hour, minute, second): %r" % ((hour, minute, second),))
+    raise XLDateBadTuple(f"Invalid (hour, minute, second): {(hour, minute, second)!r}")
 
 
 def xldate_from_datetime_tuple(datetime_tuple, datemode):
     """
     Convert a datetime tuple ``(year, month, day, hour, minute, second)`` to an
     Excel date value.
     For more details, refer to other xldate_from_*_tuple functions.
```

### Comparing `excelrd-2.0.3/excelrd/xlsx.py` & `excelrd-3.0.0/excelrd/xlsx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ##
 # Portions copyright (c) 2008-2012 Stephen John Machin, Lingfo Pty Ltd
 # This module is part of the excelrd package, which is released under a BSD-style licence.
 ##
 
-
+import io
 import re
 import sys
 from os.path import join, normpath
 
 from .biffh import (
     XL_CELL_BLANK,
     XL_CELL_BOOLEAN,
@@ -29,43 +29,34 @@
 
 ET = None
 ET_has_iterparse = False
 
 
 def ensure_elementtree_imported(verbosity, logfile):
     global ET, ET_has_iterparse
+
     if ET is not None:
         return
+
     if "IronPython" in sys.version:
         import xml.etree.ElementTree as ET
 
         #### 2.7.2.1: fails later with
         #### NotImplementedError: iterparse is not supported on IronPython. (CP #31923)
     else:
         try:
             import defusedxml.cElementTree as ET
         except ImportError:
             try:
-                import xml.etree.cElementTree as ET
+                import lxml.etree as ET
             except ImportError:
-                try:
-                    import cElementTree as ET
-                except ImportError:
-                    try:
-                        import lxml.etree as ET
-                    except ImportError:
-                        try:
-                            import xml.etree.ElementTree as ET
-                        except ImportError:
-                            try:
-                                import elementtree.ElementTree as ET
-                            except ImportError:
-                                raise Exception("Failed to import an ElementTree implementation")
+                import xml.etree.ElementTree as ET
+
     if hasattr(ET, "iterparse"):
-        _dummy_stream = BYTES_IO(b"")
+        _dummy_stream = io.BytesIO(b"")
         try:
             ET.iterparse(_dummy_stream)
             ET_has_iterparse = True
         except NotImplementedError:
             pass
 
     if verbosity:
@@ -122,15 +113,15 @@
                     else:
                         raise Exception("Missing col in cell name %r", cell_name)
                 else:
                     colx = colx - 1
                     assert 0 <= colx < X12_MAX_COLS
                     break
     except KeyError:
-        raise Exception("Unexpected character %r in cell name %r" % (c, cell_name))
+        raise Exception(f"Unexpected character {c!r} in cell name {cell_name!r}")
     rowx = int(cell_name[charx:]) - 1
     return rowx, colx
 
 
 error_code_from_text = {}
 for _code, _text in list(error_text_from_code.items()):
     error_code_from_text[_text] = _code
@@ -141,16 +132,16 @@
 U_ODREL = "{http://schemas.openxmlformats.org/officeDocument/2006/relationships}"
 U_PKGREL = "{http://schemas.openxmlformats.org/package/2006/relationships}"
 U_CP = "{http://schemas.openxmlformats.org/package/2006/metadata/core-properties}"
 U_DC = "{http://purl.org/dc/elements/1.1/}"
 U_DCTERMS = "{http://purl.org/dc/terms/}"
 XML_SPACE_ATTR = "{http://www.w3.org/XML/1998/namespace}space"
 XML_WHITESPACE = "\t\n \r"
-X12_MAX_ROWS = 2 ** 20
-X12_MAX_COLS = 2 ** 14
+X12_MAX_ROWS = 2**20
+X12_MAX_COLS = 2**14
 V_TAG = U_SSML12 + "v"  # cell child: value
 F_TAG = U_SSML12 + "f"  # cell child: formula
 IS_TAG = U_SSML12 + "is"  # cell child: inline string
 
 
 def unescape(
     s,
@@ -164,15 +155,15 @@
 
 def cooked_text(self, elem):
     t = elem.text
     if t is None:
         return ""
     if elem.get(XML_SPACE_ATTR) != "preserve":
         t = t.strip(XML_WHITESPACE)
-    return ensure_unicode(unescape(t))
+    return unescape(t)
 
 
 def get_text_from_si_or_is(self, elem, r_tag=U_SSML12 + "r", t_tag=U_SSML12 + "t"):
     "Returns unescaped unicode"
     accum = []
     for child in elem:
         # self.dump_elem(child)
@@ -201,15 +192,16 @@
         cooked_value = cnv_func_or_const(raw_value)
         setattr(obj, obj_attr, cooked_value)
 
 
 def cnv_ST_Xstring(s):
     if s is None:
         return ""
-    return ensure_unicode(s)
+
+    return s
 
 
 def cnv_xsd_unsignedInt(s):
     if not s:
         return None
     value = int(s)
     assert value >= 0
@@ -223,55 +215,167 @@
         return 1
     if s in ("0", "false", "off"):
         return 0
     raise ValueError("unexpected xsd:boolean value: %r" % s)
 
 
 _defined_name_attribute_map = (
-    ("name", "name", cnv_ST_Xstring,),
-    ("comment", "", cnv_ST_Xstring,),
-    ("customMenu", "", cnv_ST_Xstring,),
-    ("description", "", cnv_ST_Xstring,),
-    ("help", "", cnv_ST_Xstring,),
-    ("statusBar", "", cnv_ST_Xstring,),
-    ("localSheetId", "scope", cnv_xsd_unsignedInt,),
-    ("hidden", "hidden", cnv_xsd_boolean,),
-    ("function", "func", cnv_xsd_boolean,),
-    ("vbProcedure", "vbasic", cnv_xsd_boolean,),
-    ("xlm", "macro", cnv_xsd_boolean,),
-    ("functionGroupId", "funcgroup", cnv_xsd_unsignedInt,),
-    ("shortcutKey", "", cnv_ST_Xstring,),
-    ("publishToServer", "", cnv_xsd_boolean,),
-    ("workbookParameter", "", cnv_xsd_boolean,),
-    ("", "any_err", 0,),
-    ("", "any_external", 0,),
-    ("", "any_rel", 0,),
-    ("", "basic_formula_len", 0,),
-    ("", "binary", 0,),
-    ("", "builtin", 0,),
-    ("", "complex", 0,),
-    ("", "evaluated", 0,),
-    ("", "excel_sheet_index", 0,),
-    ("", "excel_sheet_num", 0,),
-    ("", "option_flags", 0,),
-    ("", "result", None,),
-    ("", "stack", None,),
+    (
+        "name",
+        "name",
+        cnv_ST_Xstring,
+    ),
+    (
+        "comment",
+        "",
+        cnv_ST_Xstring,
+    ),
+    (
+        "customMenu",
+        "",
+        cnv_ST_Xstring,
+    ),
+    (
+        "description",
+        "",
+        cnv_ST_Xstring,
+    ),
+    (
+        "help",
+        "",
+        cnv_ST_Xstring,
+    ),
+    (
+        "statusBar",
+        "",
+        cnv_ST_Xstring,
+    ),
+    (
+        "localSheetId",
+        "scope",
+        cnv_xsd_unsignedInt,
+    ),
+    (
+        "hidden",
+        "hidden",
+        cnv_xsd_boolean,
+    ),
+    (
+        "function",
+        "func",
+        cnv_xsd_boolean,
+    ),
+    (
+        "vbProcedure",
+        "vbasic",
+        cnv_xsd_boolean,
+    ),
+    (
+        "xlm",
+        "macro",
+        cnv_xsd_boolean,
+    ),
+    (
+        "functionGroupId",
+        "funcgroup",
+        cnv_xsd_unsignedInt,
+    ),
+    (
+        "shortcutKey",
+        "",
+        cnv_ST_Xstring,
+    ),
+    (
+        "publishToServer",
+        "",
+        cnv_xsd_boolean,
+    ),
+    (
+        "workbookParameter",
+        "",
+        cnv_xsd_boolean,
+    ),
+    (
+        "",
+        "any_err",
+        0,
+    ),
+    (
+        "",
+        "any_external",
+        0,
+    ),
+    (
+        "",
+        "any_rel",
+        0,
+    ),
+    (
+        "",
+        "basic_formula_len",
+        0,
+    ),
+    (
+        "",
+        "binary",
+        0,
+    ),
+    (
+        "",
+        "builtin",
+        0,
+    ),
+    (
+        "",
+        "complex",
+        0,
+    ),
+    (
+        "",
+        "evaluated",
+        0,
+    ),
+    (
+        "",
+        "excel_sheet_index",
+        0,
+    ),
+    (
+        "",
+        "excel_sheet_num",
+        0,
+    ),
+    (
+        "",
+        "option_flags",
+        0,
+    ),
+    (
+        "",
+        "result",
+        None,
+    ),
+    (
+        "",
+        "stack",
+        None,
+    ),
 )
 
 
 def make_name_access_maps(bk):
     name_and_scope_map = {}  # (name.lower(), scope): Name_object
     name_map = {}  # name.lower() : list of Name_objects (sorted in scope order)
     num_names = len(bk.name_obj_list)
     for namex in range(num_names):
         nobj = bk.name_obj_list[namex]
         name_lcase = nobj.name.lower()
         key = (name_lcase, nobj.scope)
         if key in name_and_scope_map:
-            msg = "Duplicate entry %r in name_and_scope_map" % (key,)
+            msg = f"Duplicate entry {key!r} in name_and_scope_map"
             if 0:
                 raise XLRDError(msg)
             else:
                 if bk.verbosity:
                     print(msg, file=bk.logfile)
         name_and_scope_map[key] = nobj
         sort_data = (nobj.scope, namex, nobj)
@@ -283,15 +387,15 @@
         alist = name_map[key]
         alist.sort()
         name_map[key] = [x[2] for x in alist]
     bk.name_and_scope_map = name_and_scope_map
     bk.name_map = name_map
 
 
-class X12General(object):
+class X12General:
     def process_stream(self, stream, heading=None):
         if self.verbosity >= 2 and heading is not None:
             fprintf(self.logfile, "\n=== %s ===\n", heading)
         self.tree = ET.parse(stream)
         getmethod = self.tag2meth.get
         for elem in self.tree.iter():
             if self.verbosity >= 3:
@@ -408,15 +512,15 @@
 
     def do_sheet(self, elem):
         bk = self.bk
         sheetx = bk.nsheets
         # print elem.attrib
         rid = elem.get(U_ODREL + "id")
         sheetId = int(elem.get("sheetId"))
-        name = unescape(ensure_unicode(elem.get("name")))
+        name = unescape(elem.get("name"))
         reltype = self.relid2reltype[rid]
         target = self.relid2path[rid]
         if self.verbosity >= 2:
             self.dumpout(
                 "sheetx=%d sheetId=%r rid=%r type=%r name=%r", sheetx, sheetId, rid, reltype, name
             )
         if reltype != "worksheet":
@@ -522,15 +626,15 @@
     def do_cellstylexfs(self, elem):
         self.xf_type = 0
 
     def do_cellxfs(self, elem):
         self.xf_type = 1
 
     def do_numfmt(self, elem):
-        formatCode = ensure_unicode(elem.get("formatCode"))
+        formatCode = elem.get("formatCode")
         numFmtId = int(elem.get("numFmtId"))
         is_date = is_date_format_string(self.bk, formatCode)
         self.fmt_is_date[numFmtId] = is_date
         fmt_obj = Format(numFmtId, is_date + 2, formatCode)
         self.bk.format_map[numFmtId] = fmt_obj
         if self.verbosity >= 3:
             self.dumpout("numFmtId=%d formatCode=%r is_date=%d", numFmtId, formatCode, is_date)
@@ -704,17 +808,17 @@
                         if lv:
                             colx = colx * 26 + lv
                         else:  # start of row number; can't be '0'
                             colx = colx - 1
                             assert 0 <= colx < X12_MAX_COLS
                             break
                 except KeyError:
-                    raise Exception("Unexpected character %r in cell name %r" % (c, cell_name))
+                    raise Exception(f"Unexpected character {c!r} in cell name {cell_name!r}")
                 if explicit_row_number and cell_name[charx:] != row_number:
-                    raise Exception("cell name %r but row number is %r" % (cell_name, row_number))
+                    raise Exception(f"cell name {cell_name!r} but row number is {row_number!r}")
             xf_index = int(cell_elem.get("s", "0"))
             cell_type = cell_elem.get("t", "n")
             tvalue = None
             if cell_type == "n":
                 # n = number. Most frequent type.
                 # <v> child contains plain text which can go straight into float()
                 # OR there's no text in which case it's a BLANK cell
```

### Comparing `excelrd-2.0.3/excelrd.egg-info/PKG-INFO` & `excelrd-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,147 +1,162 @@
 Metadata-Version: 2.1
 Name: excelrd
-Version: 2.0.3
+Version: 3.0.0
 Summary: Library for developers to extract data from Microsoft Excel (tm) spreadsheet files
 Home-page: https://github.com/thombashi/excelrd
 Author: John Machin
 Author-email: sjmachin@lexicon.net
 Maintainer: Tsuyoshi Hombashi
 Maintainer-email: tsuyoshi.hombashi@gmail.com
 License: BSD
-Description: .. contents:: **excelrd**
-           :backlinks: top
-           :depth: 2
-        
-        .. image:: https://badge.fury.io/py/excelrd.svg
-            :target: https://badge.fury.io/py/excelrd
-            :alt: PyPI package version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/excelrd.svg
-            :target: https://pypi.org/project/excelrd
-            :alt: Supported Python versions
-        
-        .. image:: https://img.shields.io/pypi/implementation/excelrd.svg
-            :target: https://pypi.org/project/excelrd
-            :alt: Supported Python implementations
-        
-        .. image:: https://img.shields.io/travis/thombashi/excelrd/master.svg?label=CI
-            :target: https://travis-ci.org/thombashi/excelrd
-            :alt: Linux/macOS CI status
-        
-        .. image:: https://coveralls.io/repos/github/thombashi/excelrd/badge.svg?branch=master
-            :target: https://coveralls.io/github/thombashi/excelrd?branch=master
-            :alt: Test coverage
-        
-        excelrd
-        ==================
-        ``excelrd`` is a modified version of `xlrd <http://www.python-excel.org/>`__ to work for the latest Python versions.
-        ``xlrd`` will not work at Python 3.9 or newer versions.
-        
-        **Purpose**: Provide a library for developers to use to extract data from Microsoft Excel (tm) spreadsheet files. It is not an end-user tool.
-        
-        **Author**: John Machin
-        
-        **Licence**: BSD-style (see licences.py)
-        
-        **Versions of Python supported**: 3.5+.
-        
-        **Outside scope**: excelrd will safely and reliably ignore any of these
-        if present in the file:
-        
-        -  Charts, Macros, Pictures, any other embedded object. WARNING:
-           currently this includes embedded worksheets.
-        -  VBA modules
-        -  Formulas (results of formula calculations are extracted, of course).
-        -  Comments
-        -  Hyperlinks
-        -  Autofilters, advanced filters, pivot tables, conditional formatting,
-           data validation
-        -  Handling password-protected (encrypted) files.
-        
-        
-        Quick start
-        ==================
-        Print all of the cell values in a specific sheet:
-        
-        :Sample Code:
-            .. code:: python
-        
-                import excelrd
-        
-        
-                def main():
-                    book = excelrd.open_workbook("namesdemo.xls")
-        
-                    print("The number of worksheets is {}".format(book.nsheets))
-                    print("Worksheet name(s): {}".format(", ".join(book.sheet_names())))
-        
-                    sh = book.sheet_by_index(2)
-                    print("{}: rows={}, cols={}".format(sh.name, sh.nrows, sh.ncols))
-        
-                    for row_idx in range(sh.nrows):
-                        for col_idx in range(sh.ncols):
-                            cell = sh.cell(row_idx, col_idx)
-        
-                            if not cell.value:
-                                continue
-        
-                            print("row={}, col={}, value={}".format(row_idx, col_idx, cell.value))
-        
-        Transition from xlrd to excelrd
-        ------------------------------------
-        Just replace the ``import xlrd``:
-        
-        .. code:: python
-        
-            import excelrd as xlrd
-        
-        
-        Another quick start
-        ------------------------------------
-        This will show the first, second and last rows
-        of each sheet in each file:
-        
-        ::
-        
-            python PYDIR/scripts/runxlrd.py 3rows *blah*.xls
-        
-        
-        Acknowledgements
-        ====================================
-        -  This package started life as a translation from C into Python of
-           parts of a utility called "xlreader" developed by David Giffin. "This
-           product includes software developed by David Giffin
-           david@giffin.org."
-        -  OpenOffice.org has truly excellent documentation of the Microsoft
-           Excel file formats and Compound Document file format, authored by
-           Daniel Rentz. See http://sc.openoffice.org
-        -  U+5F20 U+654F: over a decade of inspiration, support, and interesting
-           decoding opportunities.
-        -  Ksenia Marasanova: sample Macintosh and non-Latin1 files, alpha
-           testing
-        -  Backporting to Python 2.1 was partially funded by Journyx - provider
-           of timesheet and project accounting solutions (http://journyx.com/).
-        -  Provision of formatting information in version 0.6.1 was funded by
-           Simplistix Ltd (http://www.simplistix.co.uk/)
-        
 Keywords: xls,excel,spreadsheet,workbook
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+.. contents:: **excelrd**
+   :backlinks: top
+   :depth: 2
+
+.. image:: https://badge.fury.io/py/excelrd.svg
+    :target: https://badge.fury.io/py/excelrd
+    :alt: PyPI package version
+
+.. image:: https://img.shields.io/pypi/pyversions/excelrd.svg
+    :target: https://pypi.org/project/excelrd
+    :alt: Supported Python versions
+
+.. image:: https://img.shields.io/pypi/implementation/excelrd.svg
+    :target: https://pypi.org/project/excelrd
+    :alt: Supported Python implementations
+
+.. image:: https://github.com/thombashi/excelrd/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/excelrd/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. image:: https://coveralls.io/repos/github/thombashi/excelrd/badge.svg?branch=master
+    :target: https://coveralls.io/github/thombashi/excelrd?branch=master
+    :alt: Test coverage
+
+excelrd
+==================
+``excelrd`` is a modified version of `xlrd <http://www.python-excel.org/>`__ to work for the latest Python versions.
+``xlrd`` will not work in Python 3.9 or newer versions.
+
+**Purpose**: Provide a library for developers to use to extract data from Microsoft Excel (tm) spreadsheet files. It is not an end-user tool.
+
+**Author**: John Machin
+
+**Licence**: BSD-style (see licences.py)
+
+**Versions of Python supported**: 3.5+.
+
+**Outside scope**: excelrd will safely and reliably ignore any of these
+if present in the file:
+
+-  Charts, Macros, Pictures, any other embedded object. WARNING:
+   currently this includes embedded worksheets.
+-  VBA modules
+-  Formulas (results of formula calculations are extracted, of course).
+-  Comments
+-  Hyperlinks
+-  Autofilters, advanced filters, pivot tables, conditional formatting,
+   data validation
+-  Handling password-protected (encrypted) files.
+
+
+Installation
+============================================
+::
+
+    pip install excelrd
+
+
+Quick start
+==================
+Print all of the cell values in a specific sheet:
+
+:Sample Code:
+    .. code:: python
+
+        import excelrd
+
+
+        def main():
+            book = excelrd.open_workbook("namesdemo.xls")
+
+            print("The number of worksheets is {}".format(book.nsheets))
+            print("Worksheet name(s): {}".format(", ".join(book.sheet_names())))
+
+            sh = book.sheet_by_index(2)
+            print("{}: rows={}, cols={}".format(sh.name, sh.nrows, sh.ncols))
+
+            for row_idx in range(sh.nrows):
+                for col_idx in range(sh.ncols):
+                    cell = sh.cell(row_idx, col_idx)
+
+                    if not cell.value:
+                        continue
+
+                    print("row={}, col={}, value={}".format(row_idx, col_idx, cell.value))
+
+Transition from xlrd to excelrd
+------------------------------------
+Replace the import from ``import xlrd`` to ``import excelrd``:
+
+.. code:: python
+
+    import excelrd as xlrd
+
+
+Another quick start
+------------------------------------
+This will show the first, second and last rows
+of each sheet in each file:
+
+::
+
+    python PYDIR/scripts/runxlrd.py 3rows *blah*.xls
+
+
+Acknowledgements
+====================================
+-  This package started life as a translation from C into Python of
+   parts of a utility called "xlreader" developed by David Giffin. "This
+   product includes software developed by David Giffin
+   david@giffin.org."
+-  OpenOffice.org has truly excellent documentation of the Microsoft
+   Excel file formats and Compound Document file format, authored by
+   Daniel Rentz. See http://sc.openoffice.org
+-  U+5F20 U+654F: over a decade of inspiration, support, and interesting
+   decoding opportunities.
+-  Ksenia Marasanova: sample Macintosh and non-Latin1 files, alpha
+   testing
+-  Backporting to Python 2.1 was partially funded by Journyx - provider
+   of timesheet and project accounting solutions (http://journyx.com/).
+-  Provision of formatting information in version 0.6.1 was funded by
+   Simplistix Ltd (http://www.simplistix.co.uk/)
+
+
+Documentation
+==================
+https://excelrd.rtfd.io/
```

### Comparing `excelrd-2.0.3/excelrd.egg-info/SOURCES.txt` & `excelrd-3.0.0/excelrd.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,34 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 tox.ini
-docs/Makefile
-docs/acknowledgements.rst
-docs/api.rst
-docs/changes.rst
-docs/conf.py
-docs/dates.rst
-docs/development.rst
-docs/formatting.rst
-docs/index.rst
-docs/installation.rst
-docs/licenses.rst
-docs/make.bat
-docs/on_demand.rst
-docs/references.rst
-docs/unicode.rst
-docs/vulnerabilities.rst
 examples/namesdemo.xls
 examples/quickstart.py
 examples/xlrdnameAPIdemo.py
 excelrd/__init__.py
+excelrd/__version__.py
 excelrd/biffh.py
 excelrd/book.py
 excelrd/compdoc.py
 excelrd/formatting.py
 excelrd/formula.py
-excelrd/info.py
 excelrd/sheet.py
 excelrd/timemachine.py
 excelrd/xldate.py
 excelrd/xlsx.py
 excelrd.egg-info/PKG-INFO
 excelrd.egg-info/SOURCES.txt
 excelrd.egg-info/dependency_links.txt
 excelrd.egg-info/requires.txt
 excelrd.egg-info/top_level.txt
+requirements/docs_requirements.txt
+requirements/test_requirements.txt
 scripts/runxlrd.py
 tests/Formate.xls
 tests/__init__.py
 tests/apachepoi_49609.xlsx
 tests/apachepoi_52348.xlsx
 tests/base.py
 tests/biff4_no_format_no_window2.xls
```

### Comparing `excelrd-2.0.3/scripts/runxlrd.py` & `excelrd-3.0.0/scripts/runxlrd.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,24 +26,24 @@
 
 [0] means no file arg
 [1] means only one file arg i.e. no glob.glob pattern
 """
 
 options = None
 if __name__ == "__main__":
-    import excelrd
+    import gc
+    import glob
     import sys
     import time
-    import glob
     import traceback
-    import gc
 
+    import excelrd
     from excelrd.timemachine import REPR
 
-    class LogHandler(object):
+    class LogHandler:
         def __init__(self, logfileobj):
             self.logfileobj = logfileobj
             self.fileheading = None
             self.shown = 0
 
         def setfileheading(self, fileheading):
             self.fileheading = fileheading
@@ -90,15 +90,15 @@
                 cxfx = str(sh.cell_xf_index(rowx, colx))
             else:
                 cxfx = ""
             if cty == excelrd.XL_CELL_DATE:
                 try:
                     showval = excelrd.xldate_as_tuple(cval, dmode)
                 except excelrd.XLDateError as e:
-                    showval = "%s:%s" % (type(e).__name__, e)
+                    showval = f"{type(e).__name__}:{e}"
                     cty = excelrd.XL_CELL_ERROR
             elif cty == excelrd.XL_CELL_ERROR:
                 showval = excelrd.error_text_from_code.get(
                     cval, "<Unknown error code 0x%02x>" % cval
                 )
             else:
                 showval = cval
@@ -108,15 +108,17 @@
     def bk_header(bk):
         print()
         print(
             "BIFF version: %s; datemode: %s"
             % (excelrd.biff_text_from_num[bk.biff_version], bk.datemode)
         )
         print(
-            "codepage: %r (encoding: %s); countries: %r" % (bk.codepage, bk.encoding, bk.countries)
+            "codepage: {!r} (encoding: {}); countries: {!r}".format(
+                bk.codepage, bk.encoding, bk.countries
+            )
         )
         print("Last saved by: %r" % bk.user_name)
         print("Number of data sheets: %d" % bk.nsheets)
         print(
             "Use mmap: %d; Formatting: %d; On demand: %d"
             % (bk.use_mmap, bk.formatting_info, bk.on_demand)
         )
@@ -163,15 +165,15 @@
         for rlo, rhi, clo, chi in labs:
             print(
                 "%s label range %s:%s contains:"
                 % (title, excelrd.cellname(rlo, clo), excelrd.cellname(rhi - 1, chi - 1))
             )
             for rx in range(rlo, rhi):
                 for cx in range(clo, chi):
-                    print("    %s: %r" % (excelrd.cellname(rx, cx), sh.cell_value(rx, cx)))
+                    print(f"    {excelrd.cellname(rx, cx)}: {sh.cell_value(rx, cx)!r}")
 
     def show_labels(bk):
         # bk_header(bk)
         hdr = 0
         for shx in range(bk.nsheets):
             sh = bk.sheet_by_index(shx)
             clabs = sh.col_label_ranges
@@ -324,23 +326,23 @@
         )
         options, args = oparser.parse_args(cmd_args)
         if len(args) == 1 and args[0] in ("version",):
             pass
         elif len(args) < 2:
             oparser.error("Expected at least 2 args, found %d" % len(args))
         cmd = args[0]
-        xlrd_version = getattr(excelrd, "__VERSION__", "unknown; before 0.5")
+        xlrd_version = getattr(excelrd, "__version__", "unknown; before 0.5")
         if cmd == "biff_dump":
             excelrd.dump(args[1], unnumbered=options.unnumbered)
             sys.exit(0)
         if cmd == "biff_count":
             excelrd.count_records(args[1])
             sys.exit(0)
         if cmd == "version":
-            print("excelrd: %s, from %s" % (xlrd_version, excelrd.__file__))
+            print(f"excelrd: {xlrd_version}, from {excelrd.__file__}")
             print("Python:", sys.version)
             sys.exit(0)
         if options.logfilename:
             logfile = LogHandler(open(options.logfilename, "w"))
         else:
             logfile = sys.stdout
         mmap_opt = options.mmap
@@ -372,24 +374,24 @@
                         encoding_override=options.encoding,
                         formatting_info=fmt_opt,
                         on_demand=options.on_demand,
                         ragged_rows=options.ragged_rows,
                     )
                     t1 = time.time()
                     if not options.suppress_timing:
-                        print("Open took %.2f seconds" % (t1 - t0,))
+                        print(f"Open took {t1 - t0:.2f} seconds")
                 except excelrd.XLRDError as e:
-                    print("*** Open failed: %s: %s" % (type(e).__name__, e))
+                    print(f"*** Open failed: {type(e).__name__}: {e}")
                     continue
                 except KeyboardInterrupt:
                     print("*** KeyboardInterrupt ***")
                     traceback.print_exc(file=sys.stdout)
                     sys.exit(1)
                 except BaseException as e:
-                    print("*** Open failed: %s: %s" % (type(e).__name__, e))
+                    print(f"*** Open failed: {type(e).__name__}: {e}")
                     traceback.print_exc(file=sys.stdout)
                     continue
                 t0 = time.time()
                 if cmd == "hdr":
                     bk_header(bk)
                 elif cmd == "ov":  # OverView
                     show(bk, 0)
@@ -418,15 +420,15 @@
                 del bk
                 if gc_mode == 1:
                     n_unreachable = gc.collect()
                     if n_unreachable:
                         print("GC post cmd:", fname, "->", n_unreachable, "unreachable objects")
                 if not options.suppress_timing:
                     t1 = time.time()
-                    print("\ncommand took %.2f seconds\n" % (t1 - t0,))
+                    print(f"\ncommand took {t1 - t0:.2f} seconds\n")
 
         return None
 
     av = sys.argv[1:]
     if not av:
         main(av)
     firstarg = av[0].lower()
```

### Comparing `excelrd-2.0.3/tests/Formate.xls` & `excelrd-3.0.0/tests/Formate.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/apachepoi_49609.xlsx` & `excelrd-3.0.0/tests/apachepoi_49609.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/apachepoi_52348.xlsx` & `excelrd-3.0.0/tests/apachepoi_52348.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/biff4_no_format_no_window2.xls` & `excelrd-3.0.0/tests/biff4_no_format_no_window2.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/corrupted_error.xls` & `excelrd-3.0.0/tests/corrupted_error.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/err_cell_empty.xlsx` & `excelrd-3.0.0/tests/err_cell_empty.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/formula_test_names.xls` & `excelrd-3.0.0/tests/formula_test_names.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/formula_test_sjmachin.xls` & `excelrd-3.0.0/tests/formula_test_sjmachin.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/issue150.xlsx` & `excelrd-3.0.0/tests/issue150.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/issue20.xls` & `excelrd-3.0.0/tests/issue20.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/merged_cells.xlsx` & `excelrd-3.0.0/tests/merged_cells.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/picture_in_cell.xls` & `excelrd-3.0.0/tests/picture_in_cell.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/profiles.xls` & `excelrd-3.0.0/tests/profiles.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/ragged.xls` & `excelrd-3.0.0/tests/ragged.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/reveng1.xlsx` & `excelrd-3.0.0/tests/reveng1.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/self_evaluation_report_2014-05-19.xlsx` & `excelrd-3.0.0/tests/self_evaluation_report_2014-05-19.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/sharedstrings_alt_location.xlsx` & `excelrd-3.0.0/tests/sharedstrings_alt_location.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_alt_sharedstrings_loc.py` & `excelrd-3.0.0/tests/test_alt_sharedstrings_loc.py`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_cell.py` & `excelrd-3.0.0/tests/test_cell.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # Portions Copyright (C) 2010, Manfred Moitzi under a BSD licence
 
 import unittest
 
 import excelrd
-from excelrd.timemachine import UNICODE_LITERAL
 
 from .base import from_this_dir
 
 
 class TestCell(unittest.TestCase):
     def setUp(self):
         self.book = excelrd.open_workbook(from_this_dir("profiles.xls"), formatting_info=True)
         self.sheet = self.book.sheet_by_name("PROFILEDEF")
 
     def test_empty_cell(self):
         sheet = self.book.sheet_by_name("TRAVERSALCHAINAGE")
         cell = sheet.cell(0, 0)
         self.assertEqual(cell.ctype, excelrd.book.XL_CELL_EMPTY)
         self.assertEqual(cell.value, "")
-        self.assertEqual(type(cell.value), type(UNICODE_LITERAL("")))
+        self.assertEqual(type(cell.value), type(""))
         self.assertTrue(cell.xf_index > 0)
 
     def test_string_cell(self):
         cell = self.sheet.cell(0, 0)
         self.assertEqual(cell.ctype, excelrd.book.XL_CELL_TEXT)
         self.assertEqual(cell.value, "PROFIL")
-        self.assertEqual(type(cell.value), type(UNICODE_LITERAL("")))
+        self.assertEqual(type(cell.value), type(""))
         self.assertTrue(cell.xf_index > 0)
 
     def test_number_cell(self):
         cell = self.sheet.cell(1, 1)
         self.assertEqual(cell.ctype, excelrd.book.XL_CELL_NUMBER)
         self.assertEqual(cell.value, 100)
         self.assertTrue(cell.xf_index > 0)
```

### Comparing `excelrd-2.0.3/tests/test_comments_excel.xlsx` & `excelrd-3.0.0/tests/test_comments_excel.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_comments_excel_sheet2.xlsx` & `excelrd-3.0.0/tests/test_comments_excel_sheet2.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_comments_gdocs.xlsx` & `excelrd-3.0.0/tests/test_comments_gdocs.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_formats.py` & `excelrd-3.0.0/tests/test_formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Portions Copyright (C) 2010, Manfred Moitzi under a BSD licence
 
-import sys
 from unittest import TestCase
 
 import excelrd
 
 from .base import from_this_dir
```

### Comparing `excelrd-2.0.3/tests/test_formulas.py` & `excelrd-3.0.0/tests/test_formulas.py`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_lower_case_cellnames.xlsx` & `excelrd-3.0.0/tests/test_lower_case_cellnames.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_missing_records.py` & `excelrd-3.0.0/tests/test_missing_records.py`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_open_workbook.py` & `excelrd-3.0.0/tests/test_open_workbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 
 class TestOpen(TestCase):
     # test different uses of open_workbook
 
     def test_names_demo(self):
         # For now, we just check this doesn't raise an error.
-        open_workbook(from_this_dir(os.path.join("..", "examples", "namesdemo.xls")),)
+        open_workbook(
+            from_this_dir(os.path.join("..", "examples", "namesdemo.xls")),
+        )
 
     def test_tilde_path_expansion(self):
         with tempfile.NamedTemporaryFile(suffix=".xlsx", dir=os.path.expanduser("~")) as fp:
             shutil.copyfile(from_this_dir("text_bar.xlsx"), fp.name)
             # For now, we just check this doesn't raise an error.
             open_workbook(os.path.join("~", os.path.basename(fp.name)))
```

### Comparing `excelrd-2.0.3/tests/test_sheet.py` & `excelrd-3.0.0/tests/test_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 NCOLS = 13
 
 ROW_ERR = NROWS + 10
 COL_ERR = NCOLS + 10
 
 
 class TestSheet(TestCase):
-
     sheetnames = ["PROFILEDEF", "AXISDEF", "TRAVERSALCHAINAGE", "AXISDATUMLEVELS", "PROFILELEVELS"]
 
     def setUp(self):
         self.book = excelrd.open_workbook(from_this_dir("profiles.xls"), formatting_info=True)
 
     def check_sheet_function(self, function):
         self.assertTrue(function(0, 0))
```

### Comparing `excelrd-2.0.3/tests/test_workbook.py` & `excelrd-3.0.0/tests/test_workbook.py`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_xldate.py` & `excelrd-3.0.0/tests/test_xldate.py`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_xldate_to_datetime.py` & `excelrd-3.0.0/tests/test_xldate_to_datetime.py`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_xlsx_comments.py` & `excelrd-3.0.0/tests/test_xlsx_comments.py`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/test_xlsx_parse.py` & `excelrd-3.0.0/tests/test_xlsx_parse.py`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/text_bar.xlsx` & `excelrd-3.0.0/tests/text_bar.xlsx`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/tests/xf_class.xls` & `excelrd-3.0.0/tests/xf_class.xls`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/LICENSE` & `excelrd-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `excelrd-2.0.3/README.rst` & `excelrd-3.0.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -10,26 +10,26 @@
     :target: https://pypi.org/project/excelrd
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/implementation/excelrd.svg
     :target: https://pypi.org/project/excelrd
     :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/travis/thombashi/excelrd/master.svg?label=CI
-    :target: https://travis-ci.org/thombashi/excelrd
-    :alt: Linux/macOS CI status
+.. image:: https://github.com/thombashi/excelrd/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/excelrd/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
 .. image:: https://coveralls.io/repos/github/thombashi/excelrd/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/excelrd?branch=master
     :alt: Test coverage
 
 excelrd
 ==================
 ``excelrd`` is a modified version of `xlrd <http://www.python-excel.org/>`__ to work for the latest Python versions.
-``xlrd`` will not work at Python 3.9 or newer versions.
+``xlrd`` will not work in Python 3.9 or newer versions.
 
 **Purpose**: Provide a library for developers to use to extract data from Microsoft Excel (tm) spreadsheet files. It is not an end-user tool.
 
 **Author**: John Machin
 
 **Licence**: BSD-style (see licences.py)
 
@@ -45,14 +45,21 @@
 -  Comments
 -  Hyperlinks
 -  Autofilters, advanced filters, pivot tables, conditional formatting,
    data validation
 -  Handling password-protected (encrypted) files.
 
 
+Installation
+============================================
+::
+
+    pip install excelrd
+
+
 Quick start
 ==================
 Print all of the cell values in a specific sheet:
 
 :Sample Code:
     .. code:: python
 
@@ -75,15 +82,15 @@
                     if not cell.value:
                         continue
 
                     print("row={}, col={}, value={}".format(row_idx, col_idx, cell.value))
 
 Transition from xlrd to excelrd
 ------------------------------------
-Just replace the ``import xlrd``:
+Replace the import from ``import xlrd`` to ``import excelrd``:
 
 .. code:: python
 
     import excelrd as xlrd
 
 
 Another quick start
@@ -109,7 +116,12 @@
    decoding opportunities.
 -  Ksenia Marasanova: sample Macintosh and non-Latin1 files, alpha
    testing
 -  Backporting to Python 2.1 was partially funded by Journyx - provider
    of timesheet and project accounting solutions (http://journyx.com/).
 -  Provision of formatting information in version 0.6.1 was funded by
    Simplistix Ltd (http://www.simplistix.co.uk/)
+
+
+Documentation
+==================
+https://excelrd.rtfd.io/
```

### Comparing `excelrd-2.0.3/pyproject.toml` & `excelrd-3.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
     | \.mypy_cache
@@ -12,14 +16,15 @@
     | buck-out
     | build
     | dist
     | examples
 )/
 | docs/conf.py
 '''
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.isort]
 dont_skip = "*/**/__init__.py"
 known_third_party = [
 ]
 include_trailing_comma = true
 line_length = 100
```

### Comparing `excelrd-2.0.3/setup.py` & `excelrd-3.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,79 @@
-import sys
+import os
+from typing import Dict, Type
 
-from setuptools import setup
-
-from excelrd.info import __VERSION__
+import setuptools
 
 
 MODULE_NAME = "excelrd"
-REPOSITORY_URL = "https://github.com/thombashi/{:s}".format(MODULE_NAME)
-TESTS_REQUIRES = ["pytest"]
-
-
-def pytest_runner_requires() -> list:
-    if set(["pytest", "test", "ptr"]).intersection(sys.argv):
-        return ["pytest-runner"]
+REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
+REQUIREMENT_DIR = "requirements"
 
-    return []
+pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class():
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
 
+with open(os.path.join(MODULE_NAME, "__version__.py")) as f:
+    exec(f.read(), pkg_info)
+
 with open("README.rst") as fp:
     long_description = fp.read()
 
+with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
+    TESTS_REQUIRES = [line.strip() for line in f if line.strip()]
+
+with open(os.path.join(REQUIREMENT_DIR, "docs_requirements.txt")) as f:
+    docs_requires = [line.strip() for line in f if line.strip()]
 
-setup(
+setuptools.setup(
     name=MODULE_NAME,
-    version=__VERSION__,
-    author="John Machin",
-    author_email="sjmachin@lexicon.net",
-    maintainer="Tsuyoshi Hombashi",
-    maintainer_email="tsuyoshi.hombashi@gmail.com",
-    url="https://github.com/thombashi/excelrd",
-    packages=["excelrd"],
-    scripts=["scripts/runxlrd.py",],
+    version=pkg_info["__version__"],
+    author=pkg_info["__author__"],
+    author_email=pkg_info["__email__"],
+    maintainer=pkg_info["__maintainer__"],
+    maintainer_email=pkg_info["__maintainer_email__"],
+    url=REPOSITORY_URL,
+    packages=setuptools.find_packages(exclude=["test*"]),
+    scripts=[
+        "scripts/runxlrd.py",
+    ],
     description=(
         "Library for developers to extract data from Microsoft Excel (tm) spreadsheet files"
     ),
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    license="BSD",
+    license=pkg_info["__license__"],
     keywords=["xls", "excel", "spreadsheet", "workbook"],
-    python_requires=">=3.5",
-    setup_requires=pytest_runner_requires(),
+    python_requires=">=3.7",
     tests_require=TESTS_REQUIRES,
     extras_require={
-        "dev": ["releasecmd>=0.2.0,<1", "twine", "wheel"] + ["pylama"] + TESTS_REQUIRES,
+        "docs": docs_requires,
+        "dev": ["releasecmd>=0.2.0,<1"] + TESTS_REQUIRES,
         "test": TESTS_REQUIRES,
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Operating System :: OS Independent",
         "Topic :: Office/Business",
         "Topic :: Office/Business :: Financial :: Spreadsheet",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

### Comparing `excelrd-2.0.3/PKG-INFO` & `excelrd-3.0.0/excelrd.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,147 +1,162 @@
 Metadata-Version: 2.1
 Name: excelrd
-Version: 2.0.3
+Version: 3.0.0
 Summary: Library for developers to extract data from Microsoft Excel (tm) spreadsheet files
 Home-page: https://github.com/thombashi/excelrd
 Author: John Machin
 Author-email: sjmachin@lexicon.net
 Maintainer: Tsuyoshi Hombashi
 Maintainer-email: tsuyoshi.hombashi@gmail.com
 License: BSD
-Description: .. contents:: **excelrd**
-           :backlinks: top
-           :depth: 2
-        
-        .. image:: https://badge.fury.io/py/excelrd.svg
-            :target: https://badge.fury.io/py/excelrd
-            :alt: PyPI package version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/excelrd.svg
-            :target: https://pypi.org/project/excelrd
-            :alt: Supported Python versions
-        
-        .. image:: https://img.shields.io/pypi/implementation/excelrd.svg
-            :target: https://pypi.org/project/excelrd
-            :alt: Supported Python implementations
-        
-        .. image:: https://img.shields.io/travis/thombashi/excelrd/master.svg?label=CI
-            :target: https://travis-ci.org/thombashi/excelrd
-            :alt: Linux/macOS CI status
-        
-        .. image:: https://coveralls.io/repos/github/thombashi/excelrd/badge.svg?branch=master
-            :target: https://coveralls.io/github/thombashi/excelrd?branch=master
-            :alt: Test coverage
-        
-        excelrd
-        ==================
-        ``excelrd`` is a modified version of `xlrd <http://www.python-excel.org/>`__ to work for the latest Python versions.
-        ``xlrd`` will not work at Python 3.9 or newer versions.
-        
-        **Purpose**: Provide a library for developers to use to extract data from Microsoft Excel (tm) spreadsheet files. It is not an end-user tool.
-        
-        **Author**: John Machin
-        
-        **Licence**: BSD-style (see licences.py)
-        
-        **Versions of Python supported**: 3.5+.
-        
-        **Outside scope**: excelrd will safely and reliably ignore any of these
-        if present in the file:
-        
-        -  Charts, Macros, Pictures, any other embedded object. WARNING:
-           currently this includes embedded worksheets.
-        -  VBA modules
-        -  Formulas (results of formula calculations are extracted, of course).
-        -  Comments
-        -  Hyperlinks
-        -  Autofilters, advanced filters, pivot tables, conditional formatting,
-           data validation
-        -  Handling password-protected (encrypted) files.
-        
-        
-        Quick start
-        ==================
-        Print all of the cell values in a specific sheet:
-        
-        :Sample Code:
-            .. code:: python
-        
-                import excelrd
-        
-        
-                def main():
-                    book = excelrd.open_workbook("namesdemo.xls")
-        
-                    print("The number of worksheets is {}".format(book.nsheets))
-                    print("Worksheet name(s): {}".format(", ".join(book.sheet_names())))
-        
-                    sh = book.sheet_by_index(2)
-                    print("{}: rows={}, cols={}".format(sh.name, sh.nrows, sh.ncols))
-        
-                    for row_idx in range(sh.nrows):
-                        for col_idx in range(sh.ncols):
-                            cell = sh.cell(row_idx, col_idx)
-        
-                            if not cell.value:
-                                continue
-        
-                            print("row={}, col={}, value={}".format(row_idx, col_idx, cell.value))
-        
-        Transition from xlrd to excelrd
-        ------------------------------------
-        Just replace the ``import xlrd``:
-        
-        .. code:: python
-        
-            import excelrd as xlrd
-        
-        
-        Another quick start
-        ------------------------------------
-        This will show the first, second and last rows
-        of each sheet in each file:
-        
-        ::
-        
-            python PYDIR/scripts/runxlrd.py 3rows *blah*.xls
-        
-        
-        Acknowledgements
-        ====================================
-        -  This package started life as a translation from C into Python of
-           parts of a utility called "xlreader" developed by David Giffin. "This
-           product includes software developed by David Giffin
-           david@giffin.org."
-        -  OpenOffice.org has truly excellent documentation of the Microsoft
-           Excel file formats and Compound Document file format, authored by
-           Daniel Rentz. See http://sc.openoffice.org
-        -  U+5F20 U+654F: over a decade of inspiration, support, and interesting
-           decoding opportunities.
-        -  Ksenia Marasanova: sample Macintosh and non-Latin1 files, alpha
-           testing
-        -  Backporting to Python 2.1 was partially funded by Journyx - provider
-           of timesheet and project accounting solutions (http://journyx.com/).
-        -  Provision of formatting information in version 0.6.1 was funded by
-           Simplistix Ltd (http://www.simplistix.co.uk/)
-        
 Keywords: xls,excel,spreadsheet,workbook
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+.. contents:: **excelrd**
+   :backlinks: top
+   :depth: 2
+
+.. image:: https://badge.fury.io/py/excelrd.svg
+    :target: https://badge.fury.io/py/excelrd
+    :alt: PyPI package version
+
+.. image:: https://img.shields.io/pypi/pyversions/excelrd.svg
+    :target: https://pypi.org/project/excelrd
+    :alt: Supported Python versions
+
+.. image:: https://img.shields.io/pypi/implementation/excelrd.svg
+    :target: https://pypi.org/project/excelrd
+    :alt: Supported Python implementations
+
+.. image:: https://github.com/thombashi/excelrd/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/excelrd/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. image:: https://coveralls.io/repos/github/thombashi/excelrd/badge.svg?branch=master
+    :target: https://coveralls.io/github/thombashi/excelrd?branch=master
+    :alt: Test coverage
+
+excelrd
+==================
+``excelrd`` is a modified version of `xlrd <http://www.python-excel.org/>`__ to work for the latest Python versions.
+``xlrd`` will not work in Python 3.9 or newer versions.
+
+**Purpose**: Provide a library for developers to use to extract data from Microsoft Excel (tm) spreadsheet files. It is not an end-user tool.
+
+**Author**: John Machin
+
+**Licence**: BSD-style (see licences.py)
+
+**Versions of Python supported**: 3.5+.
+
+**Outside scope**: excelrd will safely and reliably ignore any of these
+if present in the file:
+
+-  Charts, Macros, Pictures, any other embedded object. WARNING:
+   currently this includes embedded worksheets.
+-  VBA modules
+-  Formulas (results of formula calculations are extracted, of course).
+-  Comments
+-  Hyperlinks
+-  Autofilters, advanced filters, pivot tables, conditional formatting,
+   data validation
+-  Handling password-protected (encrypted) files.
+
+
+Installation
+============================================
+::
+
+    pip install excelrd
+
+
+Quick start
+==================
+Print all of the cell values in a specific sheet:
+
+:Sample Code:
+    .. code:: python
+
+        import excelrd
+
+
+        def main():
+            book = excelrd.open_workbook("namesdemo.xls")
+
+            print("The number of worksheets is {}".format(book.nsheets))
+            print("Worksheet name(s): {}".format(", ".join(book.sheet_names())))
+
+            sh = book.sheet_by_index(2)
+            print("{}: rows={}, cols={}".format(sh.name, sh.nrows, sh.ncols))
+
+            for row_idx in range(sh.nrows):
+                for col_idx in range(sh.ncols):
+                    cell = sh.cell(row_idx, col_idx)
+
+                    if not cell.value:
+                        continue
+
+                    print("row={}, col={}, value={}".format(row_idx, col_idx, cell.value))
+
+Transition from xlrd to excelrd
+------------------------------------
+Replace the import from ``import xlrd`` to ``import excelrd``:
+
+.. code:: python
+
+    import excelrd as xlrd
+
+
+Another quick start
+------------------------------------
+This will show the first, second and last rows
+of each sheet in each file:
+
+::
+
+    python PYDIR/scripts/runxlrd.py 3rows *blah*.xls
+
+
+Acknowledgements
+====================================
+-  This package started life as a translation from C into Python of
+   parts of a utility called "xlreader" developed by David Giffin. "This
+   product includes software developed by David Giffin
+   david@giffin.org."
+-  OpenOffice.org has truly excellent documentation of the Microsoft
+   Excel file formats and Compound Document file format, authored by
+   Daniel Rentz. See http://sc.openoffice.org
+-  U+5F20 U+654F: over a decade of inspiration, support, and interesting
+   decoding opportunities.
+-  Ksenia Marasanova: sample Macintosh and non-Latin1 files, alpha
+   testing
+-  Backporting to Python 2.1 was partially funded by Journyx - provider
+   of timesheet and project accounting solutions (http://journyx.com/).
+-  Provision of formatting information in version 0.6.1 was funded by
+   Simplistix Ltd (http://www.simplistix.co.uk/)
+
+
+Documentation
+==================
+https://excelrd.rtfd.io/
```

