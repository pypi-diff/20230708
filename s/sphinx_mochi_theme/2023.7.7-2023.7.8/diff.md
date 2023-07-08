# Comparing `tmp/sphinx_mochi_theme-2023.7.7.tar.gz` & `tmp/sphinx_mochi_theme-2023.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_mochi_theme-2023.7.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_mochi_theme-2023.7.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_mochi_theme-2023.7.7.tar` & `sphinx_mochi_theme-2023.7.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0      247 2023-03-05 13:15:30.126968 sphinx_mochi_theme-2023.7.7/.editorconfig
--rw-r--r--   0        0        0      819 2023-07-07 12:47:44.184263 sphinx_mochi_theme-2023.7.7/.github/workflows/actions.yml
--rw-r--r--   0        0        0       39 2023-07-07 11:45:58.454810 sphinx_mochi_theme-2023.7.7/.gitignore
--rw-r--r--   0        0        0      633 2023-03-04 10:57:54.069253 sphinx_mochi_theme-2023.7.7/.vscode/launch.json
--rw-r--r--   0        0        0     1465 2023-07-07 10:36:15.670801 sphinx_mochi_theme-2023.7.7/LICENSE
--rw-r--r--   0        0        0      217 2023-07-07 12:31:42.913577 sphinx_mochi_theme-2023.7.7/README.md
--rw-r--r--   0        0        0     4103 2023-03-07 13:12:24.348292 sphinx_mochi_theme-2023.7.7/assets/sass/_core.scss
--rw-r--r--   0        0        0     3532 2023-04-06 12:39:54.383091 sphinx_mochi_theme-2023.7.7/assets/sass/_main.scss
--rw-r--r--   0        0        0     1815 2023-03-04 07:28:24.809163 sphinx_mochi_theme-2023.7.7/assets/sass/_normalize.scss
--rw-r--r--   0        0        0      743 2023-03-05 10:07:18.967516 sphinx_mochi_theme-2023.7.7/assets/sass/_print.scss
--rw-r--r--   0        0        0      445 2023-03-05 03:41:38.888834 sphinx_mochi_theme-2023.7.7/assets/sass/_scroll.scss
--rw-r--r--   0        0        0     4550 2023-03-05 13:19:45.912491 sphinx_mochi_theme-2023.7.7/assets/sass/_sidebar.scss
--rw-r--r--   0        0        0       36 2023-07-07 08:58:03.948268 sphinx_mochi_theme-2023.7.7/assets/sass/_style.scss
--rw-r--r--   0        0        0      128 2023-07-07 08:58:44.327914 sphinx_mochi_theme-2023.7.7/assets/sass/theme.scss
--rw-r--r--   0        0        0       31 2023-03-05 13:15:55.204253 sphinx_mochi_theme-2023.7.7/assets/scripts/theme.ts
--rw-r--r--   0        0        0        0 2023-03-02 00:07:59.819715 sphinx_mochi_theme-2023.7.7/codecov.yml
--rw-r--r--   0        0        0        6 2023-03-02 00:42:33.285144 sphinx_mochi_theme-2023.7.7/docs/.gitignore
--rw-r--r--   0        0        0      638 2023-03-02 00:04:40.129197 sphinx_mochi_theme-2023.7.7/docs/Makefile
--rwxr-xr-x   0        0        0      804 2023-03-02 00:04:40.147191 sphinx_mochi_theme-2023.7.7/docs/make.bat
--rw-r--r--   0        0        0        0 2023-03-03 06:25:27.225038 sphinx_mochi_theme-2023.7.7/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0    15086 2023-07-07 08:45:03.000000 sphinx_mochi_theme-2023.7.7/docs/source/_static/favicon.ico
--rw-r--r--   0        0        0    10197 2023-07-07 08:43:57.175320 sphinx_mochi_theme-2023.7.7/docs/source/_static/mochi.png
--rw-r--r--   0        0        0        0 2023-03-03 06:25:23.469226 sphinx_mochi_theme-2023.7.7/docs/source/_templates/.gitkeep
--rw-r--r--   0        0        0     3141 2023-07-07 12:06:49.065494 sphinx_mochi_theme-2023.7.7/docs/source/conf.py
--rw-r--r--   0        0        0        0 2023-03-05 13:20:20.528525 sphinx_mochi_theme-2023.7.7/docs/source/doc/_images/.gitkeep
--rw-r--r--   0        0        0      257 2023-07-07 09:05:51.234446 sphinx_mochi_theme-2023.7.7/docs/source/doc/customize.md
--rw-r--r--   0        0        0     1633 2023-07-07 09:55:50.029114 sphinx_mochi_theme-2023.7.7/docs/source/doc/req.md
--rw-r--r--   0        0        0     1608 2023-03-02 00:24:19.312805 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/admonitions.rst
--rw-r--r--   0        0        0      983 2023-03-02 00:24:19.350802 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/api.rst
--rw-r--r--   0        0        0     8353 2023-07-07 06:21:09.777334 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/blocks.rst
--rw-r--r--   0        0        0     8597 2023-03-02 00:24:19.437801 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/generic.rst
--rw-r--r--   0        0        0     3070 2023-03-02 00:24:19.474802 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/images.rst
--rw-r--r--   0        0        0      521 2023-03-02 00:24:19.507802 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/index.rst
--rw-r--r--   0        0        0     6393 2023-07-07 06:21:15.875116 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/lists.rst
--rw-r--r--   0        0        0    13453 2023-03-02 00:24:19.598803 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/really-long.rst
--rw-r--r--   0        0        0     6375 2023-03-02 00:24:19.637838 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/structure.rst
--rw-r--r--   0        0        0     5068 2023-03-02 00:24:19.681082 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/tables.rst
--rw-r--r--   0        0        0     2668 2023-03-02 00:24:19.726111 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/typography.rst
--rw-r--r--   0        0        0     2993 2023-07-07 09:26:51.056445 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/page/japanese.rst
--rw-r--r--   0        0        0    15790 2023-03-07 10:48:01.778016 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/page/long-page.rst
--rw-r--r--   0        0        0      134 2023-03-02 00:24:19.135749 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/page/placeholder-four.rst
--rw-r--r--   0        0        0      131 2023-03-02 00:24:19.167750 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/page/placeholder-one.rst
--rw-r--r--   0        0        0      137 2023-03-02 00:24:19.198801 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/page/placeholder-three.rst
--rw-r--r--   0        0        0      131 2023-03-02 00:24:19.235801 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/page/placeholder-two.rst
--rw-r--r--   0        0        0      360 2023-03-02 00:24:19.264801 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/page/really-long-title.rst
--rw-r--r--   0        0        0      111 2023-03-07 10:59:45.520746 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/tree/page1-1.rst
--rw-r--r--   0        0        0       80 2023-03-02 00:52:26.180564 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/tree/page1-2-1.rst
--rw-r--r--   0        0        0       82 2023-03-02 04:46:36.673401 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/tree/page1-2-2-1.rst
--rw-r--r--   0        0        0       82 2023-03-02 04:46:34.311335 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/tree/page1-2-2-2.rst
--rw-r--r--   0        0        0      146 2023-03-02 04:47:01.073485 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/tree/page1-2-2.rst
--rw-r--r--   0        0        0      141 2023-03-02 00:52:03.090002 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/tree/page1-2.rst
--rw-r--r--   0        0        0      131 2023-03-02 00:51:25.686416 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/tree/page1.rst
--rw-r--r--   0        0        0      105 2023-03-07 10:59:56.733845 sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/tree/page2.rst
--rw-r--r--   0        0        0      169 2023-07-08 01:46:37.356748 sphinx_mochi_theme-2023.7.7/docs/source/doc/setup.md
--rw-r--r--   0        0        0     1294 2023-07-07 09:24:05.844803 sphinx_mochi_theme-2023.7.7/docs/source/index.rst
--rw-r--r--   0        0        0      961 2023-03-05 13:16:16.121184 sphinx_mochi_theme-2023.7.7/package.json
--rw-r--r--   0        0        0      869 2023-07-08 00:44:30.898385 sphinx_mochi_theme-2023.7.7/pyproject.toml
--rw-r--r--   0        0        0       11 2023-03-05 13:22:59.649239 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/.gitignore
--rw-r--r--   0        0        0     4585 2023-07-07 12:12:19.943936 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/__init__.py
--rw-r--r--   0        0        0        4 2023-03-02 07:39:32.058556 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/base.html
--rw-r--r--   0        0        0     1739 2023-03-07 10:49:14.136235 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/genindex.html
--rw-r--r--   0        0        0     4177 2023-04-06 12:22:24.586047 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/page.html
--rw-r--r--   0        0        0      450 2023-03-05 06:03:52.965337 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/partials/brand.html
--rw-r--r--   0        0        0      699 2023-03-07 12:10:47.751957 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/partials/footer.html
--rw-r--r--   0        0        0     1292 2023-03-05 08:29:25.434950 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/partials/icons.html
--rw-r--r--   0        0        0      243 2023-03-05 10:54:00.588783 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/partials/mobile-header.html
--rw-r--r--   0        0        0      896 2023-03-05 05:35:32.852477 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/partials/related-pages.html
--rw-r--r--   0        0        0      436 2023-03-05 08:30:56.520058 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/partials/search.html
--rw-r--r--   0        0        0      785 2023-03-07 10:48:06.907037 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/search.html
--rw-r--r--   0        0        0      112 2023-03-02 02:51:08.249626 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/static/.gitignore
--rw-r--r--   0        0        0    14129 2023-07-07 08:59:39.780526 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/static/styles/theme.css
--rw-r--r--   0        0        0       96 2023-03-05 13:22:16.469338 sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/theme.conf
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 sphinx_mochi_theme-2023.7.7/PKG-INFO
+-rw-r--r--   0        0        0      247 2023-03-05 13:15:30.126968 sphinx_mochi_theme-2023.7.8/.editorconfig
+-rw-r--r--   0        0        0      819 2023-07-07 12:47:44.184263 sphinx_mochi_theme-2023.7.8/.github/workflows/actions.yml
+-rw-r--r--   0        0        0       39 2023-07-07 11:45:58.454810 sphinx_mochi_theme-2023.7.8/.gitignore
+-rw-r--r--   0        0        0      633 2023-03-04 10:57:54.069253 sphinx_mochi_theme-2023.7.8/.vscode/launch.json
+-rw-r--r--   0        0        0     1465 2023-07-07 10:36:15.670801 sphinx_mochi_theme-2023.7.8/LICENSE
+-rw-r--r--   0        0        0      217 2023-07-07 12:31:42.913577 sphinx_mochi_theme-2023.7.8/README.md
+-rw-r--r--   0        0        0     4103 2023-03-07 13:12:24.348292 sphinx_mochi_theme-2023.7.8/assets/sass/_core.scss
+-rw-r--r--   0        0        0     3532 2023-04-06 12:39:54.383091 sphinx_mochi_theme-2023.7.8/assets/sass/_main.scss
+-rw-r--r--   0        0        0     1815 2023-03-04 07:28:24.809163 sphinx_mochi_theme-2023.7.8/assets/sass/_normalize.scss
+-rw-r--r--   0        0        0      743 2023-03-05 10:07:18.967516 sphinx_mochi_theme-2023.7.8/assets/sass/_print.scss
+-rw-r--r--   0        0        0      445 2023-03-05 03:41:38.888834 sphinx_mochi_theme-2023.7.8/assets/sass/_scroll.scss
+-rw-r--r--   0        0        0     4550 2023-03-05 13:19:45.912491 sphinx_mochi_theme-2023.7.8/assets/sass/_sidebar.scss
+-rw-r--r--   0        0        0       36 2023-07-07 08:58:03.948268 sphinx_mochi_theme-2023.7.8/assets/sass/_style.scss
+-rw-r--r--   0        0        0      128 2023-07-07 08:58:44.327914 sphinx_mochi_theme-2023.7.8/assets/sass/theme.scss
+-rw-r--r--   0        0        0       31 2023-03-05 13:15:55.204253 sphinx_mochi_theme-2023.7.8/assets/scripts/theme.ts
+-rw-r--r--   0        0        0        0 2023-03-02 00:07:59.819715 sphinx_mochi_theme-2023.7.8/codecov.yml
+-rw-r--r--   0        0        0        6 2023-03-02 00:42:33.285144 sphinx_mochi_theme-2023.7.8/docs/.gitignore
+-rw-r--r--   0        0        0      638 2023-03-02 00:04:40.129197 sphinx_mochi_theme-2023.7.8/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2023-03-02 00:04:40.147191 sphinx_mochi_theme-2023.7.8/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-03-03 06:25:27.225038 sphinx_mochi_theme-2023.7.8/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0    15086 2023-07-07 08:45:03.000000 sphinx_mochi_theme-2023.7.8/docs/source/_static/favicon.ico
+-rw-r--r--   0        0        0    10197 2023-07-07 08:43:57.175320 sphinx_mochi_theme-2023.7.8/docs/source/_static/mochi.png
+-rw-r--r--   0        0        0        0 2023-03-03 06:25:23.469226 sphinx_mochi_theme-2023.7.8/docs/source/_templates/.gitkeep
+-rw-r--r--   0        0        0     3141 2023-07-08 03:50:28.200651 sphinx_mochi_theme-2023.7.8/docs/source/conf.py
+-rw-r--r--   0        0        0        0 2023-03-05 13:20:20.528525 sphinx_mochi_theme-2023.7.8/docs/source/doc/_images/.gitkeep
+-rw-r--r--   0        0        0      763 2023-07-08 09:57:42.610778 sphinx_mochi_theme-2023.7.8/docs/source/doc/customize.md
+-rw-r--r--   0        0        0     1633 2023-07-07 09:55:50.029114 sphinx_mochi_theme-2023.7.8/docs/source/doc/req.md
+-rw-r--r--   0        0        0     1608 2023-03-02 00:24:19.312805 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/admonitions.rst
+-rw-r--r--   0        0        0      983 2023-03-02 00:24:19.350802 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/api.rst
+-rw-r--r--   0        0        0     8353 2023-07-07 06:21:09.777334 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/blocks.rst
+-rw-r--r--   0        0        0     8597 2023-03-02 00:24:19.437801 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/generic.rst
+-rw-r--r--   0        0        0     3070 2023-03-02 00:24:19.474802 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/images.rst
+-rw-r--r--   0        0        0      521 2023-03-02 00:24:19.507802 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/index.rst
+-rw-r--r--   0        0        0     6393 2023-07-07 06:21:15.875116 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/lists.rst
+-rw-r--r--   0        0        0    13453 2023-03-02 00:24:19.598803 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/really-long.rst
+-rw-r--r--   0        0        0     6375 2023-03-02 00:24:19.637838 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/structure.rst
+-rw-r--r--   0        0        0     5068 2023-03-02 00:24:19.681082 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/tables.rst
+-rw-r--r--   0        0        0     2668 2023-03-02 00:24:19.726111 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/typography.rst
+-rw-r--r--   0        0        0     2993 2023-07-07 09:26:51.056445 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/page/japanese.rst
+-rw-r--r--   0        0        0    15790 2023-03-07 10:48:01.778016 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/page/long-page.rst
+-rw-r--r--   0        0        0      134 2023-03-02 00:24:19.135749 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/page/placeholder-four.rst
+-rw-r--r--   0        0        0      131 2023-03-02 00:24:19.167750 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/page/placeholder-one.rst
+-rw-r--r--   0        0        0      137 2023-03-02 00:24:19.198801 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/page/placeholder-three.rst
+-rw-r--r--   0        0        0      131 2023-03-02 00:24:19.235801 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/page/placeholder-two.rst
+-rw-r--r--   0        0        0      360 2023-03-02 00:24:19.264801 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/page/really-long-title.rst
+-rw-r--r--   0        0        0      111 2023-03-07 10:59:45.520746 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/tree/page1-1.rst
+-rw-r--r--   0        0        0       80 2023-03-02 00:52:26.180564 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/tree/page1-2-1.rst
+-rw-r--r--   0        0        0       82 2023-03-02 04:46:36.673401 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/tree/page1-2-2-1.rst
+-rw-r--r--   0        0        0       82 2023-03-02 04:46:34.311335 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/tree/page1-2-2-2.rst
+-rw-r--r--   0        0        0      146 2023-03-02 04:47:01.073485 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/tree/page1-2-2.rst
+-rw-r--r--   0        0        0      141 2023-03-02 00:52:03.090002 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/tree/page1-2.rst
+-rw-r--r--   0        0        0      131 2023-03-02 00:51:25.686416 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/tree/page1.rst
+-rw-r--r--   0        0        0      105 2023-03-07 10:59:56.733845 sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/tree/page2.rst
+-rw-r--r--   0        0        0      169 2023-07-08 01:46:37.356748 sphinx_mochi_theme-2023.7.8/docs/source/doc/setup.md
+-rw-r--r--   0        0        0     1264 2023-07-08 09:54:58.043494 sphinx_mochi_theme-2023.7.8/docs/source/index.rst
+-rw-r--r--   0        0        0      961 2023-03-05 13:16:16.121184 sphinx_mochi_theme-2023.7.8/package.json
+-rw-r--r--   0        0        0      869 2023-07-08 00:44:30.898385 sphinx_mochi_theme-2023.7.8/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-03-05 13:22:59.649239 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/.gitignore
+-rw-r--r--   0        0        0     5579 2023-07-08 09:59:11.806008 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/__init__.py
+-rw-r--r--   0        0        0        4 2023-03-02 07:39:32.058556 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/base.html
+-rw-r--r--   0        0        0     1739 2023-03-07 10:49:14.136235 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/genindex.html
+-rw-r--r--   0        0        0     4177 2023-04-06 12:22:24.586047 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/page.html
+-rw-r--r--   0        0        0      450 2023-03-05 06:03:52.965337 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/partials/brand.html
+-rw-r--r--   0        0        0      699 2023-03-07 12:10:47.751957 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/partials/footer.html
+-rw-r--r--   0        0        0     1292 2023-03-05 08:29:25.434950 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/partials/icons.html
+-rw-r--r--   0        0        0      243 2023-03-05 10:54:00.588783 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/partials/mobile-header.html
+-rw-r--r--   0        0        0      896 2023-03-05 05:35:32.852477 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/partials/related-pages.html
+-rw-r--r--   0        0        0      436 2023-03-05 08:30:56.520058 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/partials/search.html
+-rw-r--r--   0        0        0      785 2023-03-07 10:48:06.907037 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/search.html
+-rw-r--r--   0        0        0      112 2023-03-02 02:51:08.249626 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/static/.gitignore
+-rw-r--r--   0        0        0    14129 2023-07-07 08:59:39.780526 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/static/styles/theme.css
+-rw-r--r--   0        0        0      157 2023-07-08 05:48:11.529966 sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/theme.conf
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 sphinx_mochi_theme-2023.7.8/PKG-INFO
```

### Comparing `sphinx_mochi_theme-2023.7.7/.github/workflows/actions.yml` & `sphinx_mochi_theme-2023.7.8/.github/workflows/actions.yml`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/.vscode/launch.json` & `sphinx_mochi_theme-2023.7.8/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/LICENSE` & `sphinx_mochi_theme-2023.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/assets/sass/_core.scss` & `sphinx_mochi_theme-2023.7.8/assets/sass/_core.scss`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/assets/sass/_main.scss` & `sphinx_mochi_theme-2023.7.8/assets/sass/_main.scss`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/assets/sass/_normalize.scss` & `sphinx_mochi_theme-2023.7.8/assets/sass/_normalize.scss`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/assets/sass/_print.scss` & `sphinx_mochi_theme-2023.7.8/assets/sass/_print.scss`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/assets/sass/_sidebar.scss` & `sphinx_mochi_theme-2023.7.8/assets/sass/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/Makefile` & `sphinx_mochi_theme-2023.7.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/make.bat` & `sphinx_mochi_theme-2023.7.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/_static/favicon.ico` & `sphinx_mochi_theme-2023.7.8/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/_static/mochi.png` & `sphinx_mochi_theme-2023.7.8/docs/source/_static/mochi.png`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/conf.py` & `sphinx_mochi_theme-2023.7.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/req.md` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/req.md`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/admonitions.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/api.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/blocks.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/generic.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/images.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/index.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/lists.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/really-long.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/really-long.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/structure.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/tables.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/kitchen-sink/typography.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/page/japanese.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/page/japanese.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/doc/sample/page/long-page.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/doc/sample/page/long-page.rst`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/docs/source/index.rst` & `sphinx_mochi_theme-2023.7.8/docs/source/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 This is a developer's documentation for simple sphinx theme named "sphinx-mochi-theme".
 
 To read how to setup, check this page: :doc:`doc/setup`
 
 For requirements when developing this theme, check this page: :doc:`doc/req`
 
 
-.. toctree::
-    :maxdepth: 1
+..  toctree::
+    :maxdepth: 2
     :caption: Index
+    :numbered:
 
     doc/setup
     doc/customize
     doc/req
 
 Sample
 ==========
 
-:doc:`doc/sample/tree/page1` constructs nested pages. The theme should render nested page nicely at the left sidebar.
+Tree pages (:doc:`doc/sample/tree/page1`) constructs nested navtree. 
 
 The :doc:`doc/sample/kitchen-sink/index` section contains pages that contains basically
 everything that you can with Sphinx "out-of-the-box".
 
-.. toctree::
+..  toctree::
     :titlesonly:
     :caption: Sample Pages
 
     doc/sample/tree/page1
     doc/sample/tree/page2
     doc/sample/kitchen-sink/index
     doc/sample/page/placeholder-one
```

### Comparing `sphinx_mochi_theme-2023.7.7/package.json` & `sphinx_mochi_theme-2023.7.8/package.json`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/pyproject.toml` & `sphinx_mochi_theme-2023.7.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/__init__.py` & `sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-""" mochi, a plain sphinx theme for reliable documentation platform """
-__version__ = "2023.7.7"
+""" mochi, a plain sphinx theme for steady documentation platform """
+__version__ = "2023.7.8"
 
 import hashlib
 import logging
 import os
 from os import path
 from bs4 import BeautifulSoup as bs, Tag
 from sphinx.application import Sphinx
@@ -16,29 +16,64 @@
 
 
 def _inspect(item):
     """ set breakpoint here and inspect any item passed from jinja"""
     _ = item
     pass
 
+def _get_theme_var_bool(context: Ctx, key: str, fallback: bool = False) -> bool:
+    try:
+        value: str = context[key]
+
+        if type(value) != str:
+            return fallback
+        
+        value = value.strip().lower()
+        if value == 'true':
+            return True
+        elif value == 'false':
+            return False
+        elif value == '1':
+            return True
+        elif value == '0':
+            return False
+        else:
+            return fallback
+    except:
+        return fallback
+
+
+def _get_theme_var_int(context: Ctx, key: str, fallback: int = 0) -> int:
+    try:
+        value: str = context[key]
+
+        if type(value) != str:
+            return fallback
+        
+        return int(value)
+    except:
+        fallback
+
+
+
 def _get_navigation_expand_image(soup: bs) -> Tag:
     retval = soup.new_tag("i", attrs={"class": "icon"})
 
     svg_element = soup.new_tag("svg")
     svg_use_element = soup.new_tag("use", href="#svg-arrow-right")
     svg_element.append(svg_use_element)
 
     retval.append(svg_element)
     return retval
 
 lru_cache(maxsize=None)
 def _create_sidebar_toc(toctree_html: str) -> str:
     """
-    add custom styles to toctree_html so it can be stylized. this function
-    also appends label tag to provide open/collapse button
+    add custom styles to toctree_html so it can be stylized. 
+    this function also appends label tag to provide open/collapse button
     """
     if not toctree_html:
         return toctree_html
 
     soup = bs(toctree_html, "html.parser")
 
     toctree_checkbox_count = 0
@@ -94,18 +129,22 @@
     return str(soup)
 
 def _get_full_toctree(context: Ctx) -> str:
     """Use sphinx-provided API to get a full-depth navtree in html string"""
 
     if "toctree" in context:
         fn_toctree = context["toctree"]
+
+        titles_only = _get_theme_var_bool(context, 'theme_mochi_navtree_titlesonly', False)
+        maxdepth = _get_theme_var_int(context, 'theme_mochi_navtree_maxdepth', -1)
+
         toctree_html = fn_toctree(
             collapse=False,
-            titles_only=True,
-            maxdepth=-1,
+            titles_only=titles_only,
+            maxdepth=maxdepth,
             includehidden=True
         )
     else:
         toctree_html = ""
 
     return toctree_html
```

### Comparing `sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/genindex.html` & `sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/page.html` & `sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/page.html`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/partials/footer.html` & `sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/partials/footer.html`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/partials/icons.html` & `sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/partials/icons.html`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/partials/related-pages.html` & `sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/partials/related-pages.html`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/search.html` & `sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/sphinx_mochi_theme/static/styles/theme.css` & `sphinx_mochi_theme-2023.7.8/sphinx_mochi_theme/static/styles/theme.css`

 * *Files identical despite different names*

### Comparing `sphinx_mochi_theme-2023.7.7/PKG-INFO` & `sphinx_mochi_theme-2023.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sphinx_mochi_theme
-Version: 2023.7.7
-Summary: mochi, a plain sphinx theme for reliable documentation platform 
+Version: 2023.7.8
+Summary: mochi, a plain sphinx theme for steady documentation platform 
 Author: yamavol
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

