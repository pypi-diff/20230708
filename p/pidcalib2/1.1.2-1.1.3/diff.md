# Comparing `tmp/pidcalib2-1.1.2.tar.gz` & `tmp/pidcalib2-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/lhcb-rta/pidcalib2/dist/.tmp-g8myio6a/pidcalib2-1.1.2.tar", last modified: Mon Jun 12 12:13:21 2023, max compression
+gzip compressed data, was "/builds/lhcb-rta/pidcalib2/dist/.tmp-2psbh3rg/pidcalib2-1.1.3.tar", last modified: Sat Jul  8 12:02:44 2023, max compression
```

## Comparing `pidcalib2-1.1.2.tar` & `pidcalib2-1.1.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.coveragerc
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.flake8
--rw-r--r--   0 root         (0) root         (0)     2267 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.mypy.ini
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    18151 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      138 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/.sourcery.yaml
--rw-r--r--   0 root         (0) root         (0)    35065 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15428 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14817 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/notebooks/
--rw-r--r--   0 root         (0) root         (0)    15142 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/notebooks/plots.ipynb
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      371 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)      796 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)     1304 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      894 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2/
--rw-r--r--   0 root         (0) root         (0)      577 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5212 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/aliases.py
--rw-r--r--   0 root         (0) root         (0)     2709 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/argparse_tools.py
--rw-r--r--   0 root         (0) root         (0)     9884 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/binning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2/data/
--rw-r--r--   0 root         (0) root         (0)   819948 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/data/samples.json
--rw-r--r--   0 root         (0) root         (0)     8179 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/make_eff_hists.py
--rw-r--r--   0 root         (0) root         (0)     3996 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/markdown_table.py
--rw-r--r--   0 root         (0) root         (0)     3496 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/merge_trees.py
--rw-r--r--   0 root         (0) root         (0)    16282 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/pid_data.py
--rw-r--r--   0 root         (0) root         (0)     6754 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/pklhisto2root.py
--rw-r--r--   0 root         (0) root         (0)    13557 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/plot_calib_distributions.py
--rw-r--r--   0 root         (0) root         (0)     9937 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/ref_calib.py
--rw-r--r--   0 root         (0) root         (0)     2593 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/samples.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2/tests/
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_binning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/
--rw-r--r--   0 root         (0) root         (0)     9898 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/cal_test_data.csv
--rw-r--r--   0 root         (0) root         (0)     5653 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/cal_test_data.pkl
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/custom_binning.json
--rw-r--r--   0 root         (0) root         (0)     2556 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl
--rw-r--r--   0 root         (0) root         (0)     2507 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl
--rw-r--r--   0 root         (0) root         (0)    36807 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl
--rw-r--r--   0 root         (0) root         (0)     2556 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl
--rw-r--r--   0 root         (0) root         (0)      865 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl
--rw-r--r--   0 root         (0) root         (0)    20907 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_PID_eff.root
--rw-r--r--   0 root         (0) root         (0)     8045 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data.csv
--rw-r--r--   0 root         (0) root         (0)     9244 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data.root
--rw-r--r--   0 root         (0) root         (0)     9817 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data_subdir.root
--rw-r--r--   0 root         (0) root         (0)      127 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/test_file_list
--rw-r--r--   0 root         (0) root         (0)      206 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_data/test_samples.json
--rw-r--r--   0 root         (0) root         (0)     9950 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_make_eff_hist.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_merge_trees.py
--rw-r--r--   0 root         (0) root         (0)     8095 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_pid_data.py
--rw-r--r--   0 root         (0) root         (0)     2549 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_pklhisto2root.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_plot_calib_distributions.py
--rw-r--r--   0 root         (0) root         (0)     4097 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_ref_calib.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    26220 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/src/pidcalib2/utils.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15428 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2059 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      305 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/src/pidcalib2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:13:21.000000 pidcalib2-1.1.2/typings/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-12 12:13:11.000000 pidcalib2-1.1.2/typings/ROOT.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/.flake8
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/.mypy.ini
+-rw-r--r--   0 root         (0) root         (0)      691 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    18151 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/.sourcery.yaml
+-rw-r--r--   0 root         (0) root         (0)    35065 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15428 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14817 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/notebooks/
+-rw-r--r--   0 root         (0) root         (0)    15142 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/notebooks/plots.ipynb
+-rw-r--r--   0 root         (0) root         (0)      654 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)      942 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      894 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2/
+-rw-r--r--   0 root         (0) root         (0)      577 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5212 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/aliases.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/argparse_tools.py
+-rw-r--r--   0 root         (0) root         (0)     9884 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/binning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2/data/
+-rw-r--r--   0 root         (0) root         (0)   819948 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/data/samples.json
+-rw-r--r--   0 root         (0) root         (0)     9324 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/make_eff_hists.py
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/markdown_table.py
+-rw-r--r--   0 root         (0) root         (0)     3496 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/merge_trees.py
+-rw-r--r--   0 root         (0) root         (0)    16282 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/pid_data.py
+-rw-r--r--   0 root         (0) root         (0)     6754 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/pklhisto2root.py
+-rw-r--r--   0 root         (0) root         (0)    13557 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/plot_calib_distributions.py
+-rw-r--r--   0 root         (0) root         (0)     9937 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/ref_calib.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/samples.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2/tests/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_binning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/
+-rw-r--r--   0 root         (0) root         (0)     9898 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/cal_test_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5653 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/cal_test_data.pkl
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/custom_binning.json
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl
+-rw-r--r--   0 root         (0) root         (0)    36807 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl
+-rw-r--r--   0 root         (0) root         (0)      865 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl
+-rw-r--r--   0 root         (0) root         (0)    20907 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/ref_PID_eff.root
+-rw-r--r--   0 root         (0) root         (0)     8045 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/ref_test_data.csv
+-rw-r--r--   0 root         (0) root         (0)     9244 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/ref_test_data.root
+-rw-r--r--   0 root         (0) root         (0)     9817 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/ref_test_data_subdir.root
+-rw-r--r--   0 root         (0) root         (0)      127 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/test_file_list
+-rw-r--r--   0 root         (0) root         (0)      206 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_data/test_samples.json
+-rw-r--r--   0 root         (0) root         (0)     9950 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_make_eff_hist.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_merge_trees.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_pid_data.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_pklhisto2root.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_plot_calib_distributions.py
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_ref_calib.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    26220 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/src/pidcalib2/utils.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15428 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      305 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/src/pidcalib2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 12:02:44.000000 pidcalib2-1.1.3/typings/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-08 12:02:33.000000 pidcalib2-1.1.3/typings/ROOT.pyi
```

### Comparing `pidcalib2-1.1.2/.gitignore` & `pidcalib2-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/.gitlab-ci.yml` & `pidcalib2-1.1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/.pre-commit-config.yaml` & `pidcalib2-1.1.3/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.4.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
       - id: no-commit-to-branch
         args: [--branch, main]
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.7.0
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 20.8b1
+    rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.8.4
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies: [flake8-bugbear]
```

### Comparing `pidcalib2-1.1.2/.pylintrc` & `pidcalib2-1.1.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/LICENSE` & `pidcalib2-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/PKG-INFO` & `pidcalib2-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidcalib2
-Version: 1.1.2
+Version: 1.1.3
 Summary: A set of tools for estimating LHCb PID efficiencies
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidcalib2
 Author: Daniel Cervenkov
 Author-email: daniel.cervenkov@cern.ch
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidcalib2/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pidcalib2-1.1.2/README.md` & `pidcalib2-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/notebooks/plots.ipynb` & `pidcalib2-1.1.3/notebooks/plots.ipynb`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/pyproject.toml` & `pidcalib2-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/setup.cfg` & `pidcalib2-1.1.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	boost_histogram
+	lb_telemetry
 	logzero
 	matplotlib
 	mplhep
 	numpy
 	pandas
 	tqdm
 	uproot>=4.2.1
```

### Comparing `pidcalib2-1.1.2/setup.py` & `pidcalib2-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/__init__.py` & `pidcalib2-1.1.3/src/pidcalib2/__init__.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/__main__.py` & `pidcalib2-1.1.3/src/pidcalib2/__main__.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/aliases.py` & `pidcalib2-1.1.3/src/pidcalib2/aliases.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/argparse_tools.py` & `pidcalib2-1.1.3/src/pidcalib2/argparse_tools.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/binning.py` & `pidcalib2-1.1.3/src/pidcalib2/binning.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/data/samples.json` & `pidcalib2-1.1.3/src/pidcalib2/data/samples.json`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/make_eff_hists.py` & `pidcalib2-1.1.3/src/pidcalib2/make_eff_hists.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,19 +29,22 @@
         $ python -m src.pidcalib2.make_eff_hists --sample=Turbo16 --magnet=up \
             --particle=Pi --pid-cut="DLLK > 0" --pid-cut="DLLK > 4" \
             --pid-cut="DLLK > 6" --bin-var=P --bin-var=ETA \
             --bin-var=nSPDHits --output-dir=pidcalib_output
 """
 
 import argparse
+import json
+from lb_telemetry.logger import Logger
 import logging
 import pathlib
 import pickle
 import re
 import sys
+import time
 from typing import List
 
 import logzero
 from logzero import logger as log
 
 from pidcalib2 import argparse_tools, binning, utils
 
@@ -232,14 +235,44 @@
                 pickle.dump(eff_hists[f"eff_{cut}"], f)
                 pickle.dump(eff_hists[f"passing_{cut}"], f)
                 pickle.dump(eff_hists["total"], f)
 
             log.info(f"Efficiency histograms saved to '{eff_hist_path}'")
 
 
+def build_telemetry_payload(exec_time: float, config: dict) -> dict:
+    args = ["binning_file", "local_dataframe", "file_list", "samples_file"]
+
+    return {
+        "sample": config["sample"],
+        "magnet": config["magnet"],
+        "particle": config["particle"],
+        "pid_cuts": "[]" if config["pid_cuts"] is None
+        else json.dumps(config["pid_cuts"]),
+        "cuts": "[]" if config["cuts"] is None else json.dumps(config["cuts"]),
+        "max_files": 0 if config["max_files"] is None else config["max_files"],
+        "bin_vars": "[]" if config["bin_vars"] is None
+        else json.dumps(config["bin_vars"]),
+        "args": json.dumps({key: config[key] for key in args if key in config}),
+        "exec_time": exec_time,
+        "version": VERSION,
+    }
+
+
 def main():  # sourcery skip: docstrings-for-functions
     config = vars(decode_arguments(sys.argv[1:]))
+
+    start_time = time.perf_counter()
     make_eff_hists(config)
+    exec_time = time.perf_counter() - start_time
+
+    telemetry = build_telemetry_payload(exec_time, config)
+    logger = Logger()
+    _ = logger.log_to_monit(
+        "PIDCalib2",
+        telemetry,
+        tags=["sample", "magnet", "particle", "version"],
+    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pidcalib2-1.1.2/src/pidcalib2/markdown_table.py` & `pidcalib2-1.1.3/src/pidcalib2/markdown_table.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/merge_trees.py` & `pidcalib2-1.1.3/src/pidcalib2/merge_trees.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/pid_data.py` & `pidcalib2-1.1.3/src/pidcalib2/pid_data.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/pklhisto2root.py` & `pidcalib2-1.1.3/src/pidcalib2/pklhisto2root.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/plot_calib_distributions.py` & `pidcalib2-1.1.3/src/pidcalib2/plot_calib_distributions.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/ref_calib.py` & `pidcalib2-1.1.3/src/pidcalib2/ref_calib.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/samples.py` & `pidcalib2-1.1.3/src/pidcalib2/samples.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_binning.py` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/cal_test_data.csv` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/cal_test_data.csv`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/cal_test_data.pkl` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/cal_test_data.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_PID_eff.root` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/ref_PID_eff.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data.csv` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/ref_test_data.csv`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data.root` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/ref_test_data.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_data/ref_test_data_subdir.root` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_data/ref_test_data_subdir.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_make_eff_hist.py` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_make_eff_hist.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_merge_trees.py` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_merge_trees.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_pid_data.py` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_pid_data.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_pklhisto2root.py` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_pklhisto2root.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_plot_calib_distributions.py` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_plot_calib_distributions.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_ref_calib.py` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_ref_calib.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/tests/test_utils.py` & `pidcalib2-1.1.3/src/pidcalib2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2/utils.py` & `pidcalib2-1.1.3/src/pidcalib2/utils.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.1.2/src/pidcalib2.egg-info/PKG-INFO` & `pidcalib2-1.1.3/src/pidcalib2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidcalib2
-Version: 1.1.2
+Version: 1.1.3
 Summary: A set of tools for estimating LHCb PID efficiencies
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidcalib2
 Author: Daniel Cervenkov
 Author-email: daniel.cervenkov@cern.ch
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidcalib2/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pidcalib2-1.1.2/src/pidcalib2.egg-info/SOURCES.txt` & `pidcalib2-1.1.3/src/pidcalib2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

