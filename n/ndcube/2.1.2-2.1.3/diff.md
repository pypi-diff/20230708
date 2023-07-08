# Comparing `tmp/ndcube-2.1.2.tar.gz` & `tmp/ndcube-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndcube-2.1.2.tar", last modified: Wed May 31 18:16:38 2023, max compression
+gzip compressed data, was "ndcube-2.1.3.tar", last modified: Sat Jul  8 17:25:07 2023, max compression
```

## Comparing `ndcube-2.1.2.tar` & `ndcube-2.1.3.tar`

### file list

```diff
@@ -1,138 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.297014 ndcube-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 18:16:20.000000 ndcube-2.1.2/.rtd-environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-31 18:16:20.000000 ndcube-2.1.2/.sunpy-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25656 2023-05-31 18:16:20.000000 ndcube-2.1.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-31 18:16:20.000000 ndcube-2.1.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 18:16:20.000000 ndcube-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-31 18:16:38.297014 ndcube-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-31 18:16:20.000000 ndcube-2.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-31 18:16:20.000000 ndcube-2.1.2/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.265014 ndcube-2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/1_to_2_transition_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.269014 ndcube-2.1.2/docs/explaining_ndcube/
--rw-r--r--   0 runner    (1001) docker     (123)    24847 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25861 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/data_classes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.269014 ndcube-2.1.2/docs/explaining_ndcube/images/
--rw-r--r--   0 runner    (1001) docker     (123)    83880 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/images/ndcollection_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   112680 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/images/ndcube_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   129621 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/images/ndcube_sliced_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   110370 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/images/ndcubesequence_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   132979 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/images/ndcubesequence_sliced_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/reproject.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/slicing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/tabular_coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/visualization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/extending_ndcube.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.273014 ndcube-2.1.2/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/logo/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)    41016 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/logo/ndcube.png
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/logo/ndcube.svg
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.273014 ndcube-2.1.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/extra_coords.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/mixins.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/ndcube.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/visualization.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/wcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/rtd_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.273014 ndcube-2.1.2/docs/whatsnew/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/whatsnew/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/whatsnew/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.277014 ndcube-2.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-31 18:16:20.000000 ndcube-2.1.2/examples/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-31 18:16:20.000000 ndcube-2.1.2/examples/creating_ndcube_from_fitsfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.277014 ndcube-2.1.2/examples/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-31 18:16:20.000000 ndcube-2.1.2/examples/dev/example_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-31 18:16:20.000000 ndcube-2.1.2/examples/slicing_ndcube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.277014 ndcube-2.1.2/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-31 18:16:20.000000 ndcube-2.1.2/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-31 18:16:20.000000 ndcube-2.1.2/licenses/TEMPLATE_LICENSE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.277014 ndcube-2.1.2/ndcube/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.281014 ndcube-2.1.2/ndcube/extra_coords/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/extra_coords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/extra_coords/extra_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    38068 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/extra_coords/table_coord.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.281014 ndcube-2.1.2/ndcube/extra_coords/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18848 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/extra_coords/tests/test_extra_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/extra_coords/tests/test_lookup_table_coord.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/global_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.285014 ndcube-2.1.2/ndcube/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/mixins/ndslicing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/ndcollection.py
--rw-r--r--   0 runner    (1001) docker     (123)    54273 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/ndcube.py
--rw-r--r--   0 runner    (1001) docker     (123)    23261 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/ndcube_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.285014 ndcube-2.1.2/ndcube/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/test_global_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/test_ndcollection.py
--rw-r--r--   0 runner    (1001) docker     (123)    48060 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/test_ndcube.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/test_ndcubesequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    39107 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/test_sequence_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.289014 ndcube-2.1.2/ndcube/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.289014 ndcube-2.1.2/ndcube/utils/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/sphinx/code_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.289014 ndcube-2.1.2/ndcube/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/tests/test_utils_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/tests/test_utils_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/tests/test_utils_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/tests/test_utils_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20562 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/wcs_high_level_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.293014 ndcube-2.1.2/ndcube/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/mpl_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/mpl_sequence_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/plotting_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.293014 ndcube-2.1.2/ndcube/visualization/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/tests/figure_hashes_mpl_353_ft_261_astropy_51_animators_100.json
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/tests/test_plotting_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.293014 ndcube-2.1.2/ndcube/wcs/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.293014 ndcube-2.1.2/ndcube/wcs/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/compound_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/reordered_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/resampled_wcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.297014 ndcube-2.1.2/ndcube/wcs/wrappers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_compound_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_reordered_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_resampled_wcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.281014 ndcube-2.1.2/ndcube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:16:37.000000 ndcube-2.1.2/ndcube.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-31 18:16:20.000000 ndcube-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-31 18:16:38.297014 ndcube-2.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-05-31 18:16:20.000000 ndcube-2.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-05-31 18:16:20.000000 ndcube-2.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.622366 ndcube-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-08 17:24:45.000000 ndcube-2.1.3/.rtd-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-08 17:24:45.000000 ndcube-2.1.3/.sunpy-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    26302 2023-07-08 17:24:45.000000 ndcube-2.1.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-08 17:24:45.000000 ndcube-2.1.3/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-08 17:24:45.000000 ndcube-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-08 17:25:07.622366 ndcube-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-08 17:24:45.000000 ndcube-2.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-08 17:24:45.000000 ndcube-2.1.3/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.606365 ndcube-2.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/1_to_2_transition_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.606365 ndcube-2.1.3/docs/explaining_ndcube/
+-rw-r--r--   0 runner    (1001) docker     (123)    24847 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25861 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/data_classes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.606365 ndcube-2.1.3/docs/explaining_ndcube/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    83880 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/images/ndcollection_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112680 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/images/ndcube_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   129621 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/images/ndcube_sliced_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   110370 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/images/ndcubesequence_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   132979 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/images/ndcubesequence_sliced_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/reproject.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/slicing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/tabular_coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/explaining_ndcube/visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/extending_ndcube.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.610365 ndcube-2.1.3/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/logo/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41016 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/logo/ndcube.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/logo/ndcube.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.610365 ndcube-2.1.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/reference/extra_coords.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/reference/mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/reference/ndcube.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/reference/tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/reference/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/reference/visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/reference/wcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/rtd_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.610365 ndcube-2.1.3/docs/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/whatsnew/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-08 17:24:45.000000 ndcube-2.1.3/docs/whatsnew/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.610365 ndcube-2.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-08 17:24:45.000000 ndcube-2.1.3/examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-08 17:24:45.000000 ndcube-2.1.3/examples/creating_ndcube_from_fitsfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.610365 ndcube-2.1.3/examples/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-08 17:24:45.000000 ndcube-2.1.3/examples/dev/example_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-08 17:24:45.000000 ndcube-2.1.3/examples/slicing_ndcube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.610365 ndcube-2.1.3/joss_paper/
+-rw-r--r--   0 runner    (1001) docker     (123)    21320 2023-07-08 17:24:45.000000 ndcube-2.1.3/joss_paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-08 17:24:45.000000 ndcube-2.1.3/joss_paper/paper.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.610365 ndcube-2.1.3/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-08 17:24:45.000000 ndcube-2.1.3/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-08 17:24:45.000000 ndcube-2.1.3/licenses/TEMPLATE_LICENSE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.614365 ndcube-2.1.3/ndcube/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-08 17:25:07.000000 ndcube-2.1.3/ndcube/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17125 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.614365 ndcube-2.1.3/ndcube/extra_coords/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/extra_coords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/extra_coords/extra_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38068 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/extra_coords/table_coord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.614365 ndcube-2.1.3/ndcube/extra_coords/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/extra_coords/tests/test_extra_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27772 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/extra_coords/tests/test_lookup_table_coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/global_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.614365 ndcube-2.1.3/ndcube/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/mixins/ndslicing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/ndcollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54309 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/ndcube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23261 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/ndcube_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.618366 ndcube-2.1.3/ndcube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/tests/test_global_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/tests/test_ndcollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48103 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/tests/test_ndcube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/tests/test_ndcubesequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39107 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/tests/test_sequence_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.618366 ndcube-2.1.3/ndcube/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.618366 ndcube-2.1.3/ndcube/utils/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/sphinx/code_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.618366 ndcube-2.1.3/ndcube/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/tests/test_utils_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/tests/test_utils_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/tests/test_utils_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/tests/test_utils_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20562 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/utils/wcs_high_level_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.622366 ndcube-2.1.3/ndcube/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/visualization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/visualization/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/visualization/mpl_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/visualization/mpl_sequence_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/visualization/plotting_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.622366 ndcube-2.1.3/ndcube/visualization/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/visualization/tests/figure_hashes_mpl_353_ft_261_astropy_51_animators_100.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/visualization/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/visualization/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/visualization/tests/test_plotting_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.622366 ndcube-2.1.3/ndcube/wcs/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/wcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.622366 ndcube-2.1.3/ndcube/wcs/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/wcs/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/wcs/wrappers/compound_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/wcs/wrappers/reordered_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/wcs/wrappers/resampled_wcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.622366 ndcube-2.1.3/ndcube/wcs/wrappers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/wcs/wrappers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/wcs/wrappers/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/wcs/wrappers/tests/test_compound_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/wcs/wrappers/tests/test_reordered_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-08 17:24:45.000000 ndcube-2.1.3/ndcube/wcs/wrappers/tests/test_resampled_wcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:25:07.614365 ndcube-2.1.3/ndcube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-08 17:25:07.000000 ndcube-2.1.3/ndcube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-08 17:25:07.000000 ndcube-2.1.3/ndcube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:25:07.000000 ndcube-2.1.3/ndcube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:25:07.000000 ndcube-2.1.3/ndcube.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-08 17:25:07.000000 ndcube-2.1.3/ndcube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 17:25:07.000000 ndcube-2.1.3/ndcube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-08 17:24:45.000000 ndcube-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-08 17:25:07.626366 ndcube-2.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-07-08 17:24:45.000000 ndcube-2.1.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-08 17:24:45.000000 ndcube-2.1.3/tox.ini
```

### Comparing `ndcube-2.1.2/CHANGELOG.rst` & `ndcube-2.1.3/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.1.3 (2023-07-08)
+===================
+
+Trivial/Internal Changes
+------------------------
+
+- Remove internal use of numpy.product as its now deprecated and replace with numpy.prod as recommended. (`#625 <https://github.com/sunpy/ndcube/pull/625>`__)
+- Write paper to Journal of Open Source Software describing ndcube package (`#599 <https://github.com/sunpy/ndcube/pull/599>`__, `#609 <https://github.com/sunpy/ndcube/pull/609>`__, `#611 <https://github.com/sunpy/ndcube/pull/611>`__, `#621 <https://github.com/sunpy/ndcube/pull/621>`__, `#622 <https://github.com/sunpy/ndcube/pull/622>`__, `#623 <https://github.com/sunpy/ndcube/pull/623>`__)
+
 2.1.2 (2023-05-31)
 ==================
 
 Backwards Incompatible Changes
 ------------------------------
 
 - `ndcube.NDCollection.aligned_axes` attribute is now property. (`#607 <https://github.com/sunpy/ndcube/pull/607>`__)
```

### Comparing `ndcube-2.1.2/LICENSE.rst` & `ndcube-2.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/PKG-INFO` & `ndcube-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndcube
-Version: 2.1.2
+Version: 2.1.3
 Summary: A package for multi-dimensional contiguous and non-contiguous coordinate aware arrays.
 Home-page: https://docs.sunpy.org/projects/ndcube/
 Download-URL: https://pypi.org/project/ndcube/
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Project-URL: Source Code, https://github.com/sunpy/ndcube/
@@ -33,15 +33,15 @@
 Provides-Extra: plotting
 Provides-Extra: reproject
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE.rst
 
 ******
-ncdube
+ndcube
 ******
 
 |Latest Version| |codecov| |matrix| |Powered by NumFOCUS| |Powered by SunPy|
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/ndcube.svg
    :target: https://pypi.python.org/pypi/ndcube/
    :alt: It is up to date, we promise
```

### Comparing `ndcube-2.1.2/README.rst` & `ndcube-2.1.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ******
-ncdube
+ndcube
 ******
 
 |Latest Version| |codecov| |matrix| |Powered by NumFOCUS| |Powered by SunPy|
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/ndcube.svg
    :target: https://pypi.python.org/pypi/ndcube/
    :alt: It is up to date, we promise
```

### Comparing `ndcube-2.1.2/RELEASE.rst` & `ndcube-2.1.3/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/1_to_2_transition_guide.rst` & `ndcube-2.1.3/docs/1_to_2_transition_guide.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/Makefile` & `ndcube-2.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/conf.py` & `ndcube-2.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/coordinates.rst` & `ndcube-2.1.3/docs/explaining_ndcube/coordinates.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/data_classes.rst` & `ndcube-2.1.3/docs/explaining_ndcube/data_classes.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/images/ndcollection_diagram.png` & `ndcube-2.1.3/docs/explaining_ndcube/images/ndcollection_diagram.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/images/ndcube_diagram.png` & `ndcube-2.1.3/docs/explaining_ndcube/images/ndcube_diagram.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/images/ndcube_sliced_diagram.png` & `ndcube-2.1.3/docs/explaining_ndcube/images/ndcube_sliced_diagram.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/images/ndcubesequence_diagram.png` & `ndcube-2.1.3/docs/explaining_ndcube/images/ndcubesequence_diagram.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/images/ndcubesequence_sliced_diagram.png` & `ndcube-2.1.3/docs/explaining_ndcube/images/ndcubesequence_sliced_diagram.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/reproject.rst` & `ndcube-2.1.3/docs/explaining_ndcube/reproject.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/slicing.rst` & `ndcube-2.1.3/docs/explaining_ndcube/slicing.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/tabular_coordinates.rst` & `ndcube-2.1.3/docs/explaining_ndcube/tabular_coordinates.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/explaining_ndcube/visualization.rst` & `ndcube-2.1.3/docs/explaining_ndcube/visualization.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/extending_ndcube.rst` & `ndcube-2.1.3/docs/extending_ndcube.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/index.rst` & `ndcube-2.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/installation.rst` & `ndcube-2.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/introduction.rst` & `ndcube-2.1.3/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/logo/favicon.png` & `ndcube-2.1.3/docs/logo/favicon.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/logo/ndcube.png` & `ndcube-2.1.3/docs/logo/ndcube.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/logo/ndcube.svg` & `ndcube-2.1.3/docs/logo/ndcube.svg`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/make.bat` & `ndcube-2.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/docs/nitpick-exceptions` & `ndcube-2.1.3/docs/nitpick-exceptions`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/examples/creating_ndcube_from_fitsfile.py` & `ndcube-2.1.3/examples/creating_ndcube_from_fitsfile.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/examples/dev/example_template.py` & `ndcube-2.1.3/examples/dev/example_template.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/examples/slicing_ndcube.py` & `ndcube-2.1.3/examples/slicing_ndcube.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/licenses/TEMPLATE_LICENSE.rst` & `ndcube-2.1.3/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/__init__.py` & `ndcube-2.1.3/ndcube/__init__.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/conftest.py` & `ndcube-2.1.3/ndcube/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,22 @@
 
 ################################################################################
 # Helper Functions
 ################################################################################
 
 
 def skycoord_2d_lut(shape):
-    total_len = np.product(shape)
+    total_len = np.prod(shape)
     data = (np.arange(total_len).reshape(shape),
             np.arange(total_len, total_len * 2).reshape(shape))
     return SkyCoord(*data, unit=u.deg)
 
 
 def data_nd(shape):
-    nelem = np.product(shape)
+    nelem = np.prod(shape)
     return np.arange(nelem).reshape(shape)
 
 
 def time_extra_coords(shape, axis, base):
     return ExtraCoords.from_lookup_tables(
         ('time',),
         (axis,),
```

### Comparing `ndcube-2.1.2/ndcube/extra_coords/extra_coords.py` & `ndcube-2.1.3/ndcube/extra_coords/extra_coords.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/extra_coords/table_coord.py` & `ndcube-2.1.3/ndcube/extra_coords/table_coord.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/extra_coords/tests/test_extra_coords.py` & `ndcube-2.1.3/ndcube/extra_coords/tests/test_extra_coords.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     data = np.arange(9).reshape(3, 3), np.arange(9, 18).reshape(3, 3)
     return SkyCoord(*data, unit=u.deg)
 
 
 @pytest.fixture
 def quantity_2d_lut():
     ec_shape = (3, 3)
-    return np.arange(np.product(ec_shape)).reshape(ec_shape) * u.m / u.s
+    return np.arange(np.prod(ec_shape)).reshape(ec_shape) * u.m / u.s
 
 
 # ExtraCoords from WCS
 
 
 def test_empty_ec(wcs_1d_l):
     ec = ExtraCoords()
```

### Comparing `ndcube-2.1.2/ndcube/extra_coords/tests/test_lookup_table_coord.py` & `ndcube-2.1.3/ndcube/extra_coords/tests/test_lookup_table_coord.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 
     assert u.allclose(ltc.wcs.world_to_pixel(*world), (0, 0, 0))
 
 
 @pytest.mark.xfail(reason=">1D Tables not supported")
 def test_2d_quantity():
     shape = (3, 3)
-    data = np.arange(np.product(shape)).reshape(shape) * u.m / u.s
+    data = np.arange(np.prod(shape)).reshape(shape) * u.m / u.s
 
     ltc = QuantityTableCoordinate(data)
     assert u.allclose(ltc.wcs.pixel_to_world(0, 0), 0 * u.m / u.s)
 
 
 def test_repr_str(lut_1d_time, lut_1d_wave):
     assert str(lut_1d_time.table) in str(lut_1d_time)
```

### Comparing `ndcube-2.1.2/ndcube/global_coords.py` & `ndcube-2.1.3/ndcube/global_coords.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/mixins/ndslicing.py` & `ndcube-2.1.3/ndcube/mixins/ndslicing.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/ndcollection.py` & `ndcube-2.1.3/ndcube/ndcollection.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/ndcube.py` & `ndcube-2.1.3/ndcube/ndcube.py`

 * *Files 0% similar despite different names*

```diff
@@ -955,14 +955,15 @@
             Passed to the unit conversion method, self.unit.to.
 
         Returns
         -------
         : `~ndcube.NDCube`
             A new instance with the new unit and data and uncertainties scales accordingly.
         """
+        new_unit = u.Unit(new_unit)
         return self * (self.unit.to(new_unit, **kwargs) * new_unit / self.unit)
 
     def rebin(self, bin_shape, operation=np.mean, operation_ignores_mask=False, handle_mask=np.all,
               propagate_uncertainties=False, new_unit=None, **kwargs):
         """
         Downsample array by combining contiguous pixels into bins.
```

### Comparing `ndcube-2.1.2/ndcube/ndcube_sequence.py` & `ndcube-2.1.3/ndcube/ndcube_sequence.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/tests/helpers.py` & `ndcube-2.1.3/ndcube/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/tests/test_global_coords.py` & `ndcube-2.1.3/ndcube/tests/test_global_coords.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/tests/test_ndcollection.py` & `ndcube-2.1.3/ndcube/tests/test_ndcollection.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/tests/test_ndcube.py` & `ndcube-2.1.3/ndcube/tests/test_ndcube.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from astropy.wcs.wcsapi.wrappers import SlicedLowLevelWCS
 
 from ndcube import ExtraCoords, NDCube
 from ndcube.tests import helpers
 
 
 def generate_data(shape):
-    data = np.arange(np.product(shape))
+    data = np.arange(np.prod(shape))
     return data.reshape(shape)
 
 
 def test_wcs_object(all_ndcubes):
     assert isinstance(all_ndcubes.wcs.low_level_wcs, BaseLowLevelWCS)
     assert isinstance(all_ndcubes.wcs, BaseHighLevelWCS)
 
@@ -207,15 +207,15 @@
     assert awc == tuple()
 
 
 @pytest.mark.xfail(reason=">1D Tables not supported")
 def test_axis_world_coords_complex_ec(ndcube_4d_ln_lt_l_t):
     cube = ndcube_4d_ln_lt_l_t
     ec_shape = cube.data.shape[1:3]
-    data = np.arange(np.product(ec_shape)).reshape(ec_shape) * u.m / u.s
+    data = np.arange(np.prod(ec_shape)).reshape(ec_shape) * u.m / u.s
 
     # The lookup table has to be in world order so transpose it.
     cube.extra_coords.add('velocity', (2, 1), data.T)
 
     coords = cube.axis_world_coords(wcs=cube.extra_coords)
     assert len(coords) == 1
     assert isinstance(coords[0], u.Quantity)
@@ -1115,22 +1115,22 @@
 
 
 def test_cube_arithmetic_multiply_notimplementederror(ndcube_2d_ln_lt_units):
     with pytest.raises(TypeError):
         _ = ndcube_2d_ln_lt_units * ndcube_2d_ln_lt_units
 
 
-def test_to(ndcube_1d_l):
+@pytest.mark.parametrize('new_unit', [u.mJ, 'mJ'])
+def test_to(ndcube_1d_l, new_unit):
     cube = ndcube_1d_l
-    new_unit = u.mJ
     expected_factor = 1000
     output = cube.to(new_unit)
     assert np.allclose(output.data, cube.data * expected_factor)
     assert np.allclose(output.uncertainty.array, cube.uncertainty.array * expected_factor)
-    assert output.unit == new_unit
+    assert output.unit == u.Unit(new_unit)
 
 
 def test_to_dask(ndcube_2d_dask):
     output = ndcube_2d_dask.to(u.mJ)
     dask_type = dask.array.core.Array
     assert isinstance(output.data, dask_type)
     assert isinstance(output.uncertainty.array, dask_type)
```

### Comparing `ndcube-2.1.2/ndcube/tests/test_ndcubesequence.py` & `ndcube-2.1.3/ndcube/tests/test_ndcubesequence.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/tests/test_sequence_plotting.py` & `ndcube-2.1.3/ndcube/tests/test_sequence_plotting.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/utils/collection.py` & `ndcube-2.1.3/ndcube/utils/collection.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/utils/cube.py` & `ndcube-2.1.3/ndcube/utils/cube.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/utils/misc.py` & `ndcube-2.1.3/ndcube/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/utils/sequence.py` & `ndcube-2.1.3/ndcube/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/utils/sphinx/code_context.py` & `ndcube-2.1.3/ndcube/utils/sphinx/code_context.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/utils/tests/test_utils_collection.py` & `ndcube-2.1.3/ndcube/utils/tests/test_utils_collection.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/utils/tests/test_utils_cube.py` & `ndcube-2.1.3/ndcube/utils/tests/test_utils_cube.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     # Build expected output
     binned_data = data.prod(axis=0)
     expected = np.sqrt(((uncertainty.array / data)**2).sum(axis=0)) * binned_data / 2  # Why do I have to divide by a factor 2 here?
     expected = StdDevUncertainty(expected)
 
     # Run function
     output = propagate_rebin_uncertainties(uncertainty, data, mask,
-                                           np.product, operation_ignores_mask=False)
+                                           np.prod, operation_ignores_mask=False)
 
     assert type(output) is type(expected)
     assert np.allclose(output.array, expected.array)
 
 
 def test_propagate_rebin_uncertainties_nan(stacked_pixel_data):
     # Build inputs
```

### Comparing `ndcube-2.1.2/ndcube/utils/tests/test_utils_sequence.py` & `ndcube-2.1.3/ndcube/utils/tests/test_utils_sequence.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/utils/tests/test_utils_wcs.py` & `ndcube-2.1.3/ndcube/utils/tests/test_utils_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/utils/wcs.py` & `ndcube-2.1.3/ndcube/utils/wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/utils/wcs_high_level_conversion.py` & `ndcube-2.1.3/ndcube/utils/wcs_high_level_conversion.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/version.py` & `ndcube-2.1.3/ndcube/version.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/visualization/base.py` & `ndcube-2.1.3/ndcube/visualization/base.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/visualization/descriptor.py` & `ndcube-2.1.3/ndcube/visualization/descriptor.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/visualization/mpl_plotter.py` & `ndcube-2.1.3/ndcube/visualization/mpl_plotter.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/visualization/mpl_sequence_plotter.py` & `ndcube-2.1.3/ndcube/visualization/mpl_sequence_plotter.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/visualization/plotting_utils.py` & `ndcube-2.1.3/ndcube/visualization/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/visualization/tests/figure_hashes_mpl_353_ft_261_astropy_51_animators_100.json` & `ndcube-2.1.3/ndcube/visualization/tests/figure_hashes_mpl_353_ft_261_astropy_51_animators_100.json`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/visualization/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json` & `ndcube-2.1.3/ndcube/visualization/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/visualization/tests/test_plotting.py` & `ndcube-2.1.3/ndcube/visualization/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/visualization/tests/test_plotting_utils.py` & `ndcube-2.1.3/ndcube/visualization/tests/test_plotting_utils.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/wcs/wrappers/compound_wcs.py` & `ndcube-2.1.3/ndcube/wcs/wrappers/compound_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/wcs/wrappers/reordered_wcs.py` & `ndcube-2.1.3/ndcube/wcs/wrappers/reordered_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/wcs/wrappers/resampled_wcs.py` & `ndcube-2.1.3/ndcube/wcs/wrappers/resampled_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_compound_wcs.py` & `ndcube-2.1.3/ndcube/wcs/wrappers/tests/test_compound_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_reordered_wcs.py` & `ndcube-2.1.3/ndcube/wcs/wrappers/tests/test_reordered_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_resampled_wcs.py` & `ndcube-2.1.3/ndcube/wcs/wrappers/tests/test_resampled_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/ndcube.egg-info/PKG-INFO` & `ndcube-2.1.3/ndcube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndcube
-Version: 2.1.2
+Version: 2.1.3
 Summary: A package for multi-dimensional contiguous and non-contiguous coordinate aware arrays.
 Home-page: https://docs.sunpy.org/projects/ndcube/
 Download-URL: https://pypi.org/project/ndcube/
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Project-URL: Source Code, https://github.com/sunpy/ndcube/
@@ -33,15 +33,15 @@
 Provides-Extra: plotting
 Provides-Extra: reproject
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE.rst
 
 ******
-ncdube
+ndcube
 ******
 
 |Latest Version| |codecov| |matrix| |Powered by NumFOCUS| |Powered by SunPy|
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/ndcube.svg
    :target: https://pypi.python.org/pypi/ndcube/
    :alt: It is up to date, we promise
```

### Comparing `ndcube-2.1.2/ndcube.egg-info/SOURCES.txt` & `ndcube-2.1.3/ndcube.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 docs/reference/wcs.rst
 docs/whatsnew/changelog.rst
 docs/whatsnew/index.rst
 examples/README.txt
 examples/creating_ndcube_from_fitsfile.py
 examples/slicing_ndcube.py
 examples/dev/example_template.py
+joss_paper/paper.bib
+joss_paper/paper.md
 licenses/README.rst
 licenses/TEMPLATE_LICENSE.rst
 ndcube/__init__.py
 ndcube/_version.py
 ndcube/conftest.py
 ndcube/global_coords.py
 ndcube/ndcollection.py
```

### Comparing `ndcube-2.1.2/ndcube.egg-info/requires.txt` & `ndcube-2.1.3/ndcube.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/pyproject.toml` & `ndcube-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/setup.cfg` & `ndcube-2.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/setup.py` & `ndcube-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.2/tox.ini` & `ndcube-2.1.3/tox.ini`

 * *Files identical despite different names*

