# Comparing `tmp/pyams_portal-1.8.1.tar.gz` & `tmp/pyams_portal-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_portal-1.8.1.tar", last modified: Tue Mar 14 08:39:52 2023, max compression
+gzip compressed data, was "dist/pyams_portal-1.9.1.tar", last modified: Fri Jul  7 22:29:48 2023, max compression
```

## Comparing `pyams_portal-1.8.1.tar` & `pyams_portal-1.9.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5254 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)     3165 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1540 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2930 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/
--rw-rw-rw-   0 root         (0) root         (0)      863 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    32950 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1735 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1929 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/generations/evolve1.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/generations/evolve2.py
--rw-rw-rw-   0 root         (0) root         (0)     1808 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/generations/evolve3.py
--rw-rw-rw-   0 root         (0) root         (0)     1877 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/generations/evolve4.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/include.py
--rw-rw-rw-   0 root         (0) root         (0)    19269 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    23902 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.mo
--rw-rw-rw-   0 root         (0) root         (0)    39074 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.po
--rw-rw-rw-   0 root         (0) root         (0)    27473 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/locales/pyams_portal.pot
--rw-rw-rw-   0 root         (0) root         (0)    11053 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/page.py
--rw-rw-rw-   0 root         (0) root         (0)    14662 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/
--rw-rw-rw-   0 root         (0) root         (0)     3863 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3516 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3002 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2377 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1946 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/skin/templates/cards-masonry.pt
--rw-rw-rw-   0 root         (0) root         (0)     2015 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/skin/templates/cards.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    10245 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/cards/zmi/templates/cards-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/
--rw-rw-rw-   0 root         (0) root         (0)     3663 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2275 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2670 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3108 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/skin/templates/carousel.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     9803 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      455 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/zmi/templates/carousel-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1678 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/skin/
--rw-rw-rw-   0 root         (0) root         (0)     5034 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/skin/templates/html.pt
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/skin/templates/raw-code.pt
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/skin/templates/raw.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2341 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/zmi/templates/html-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/html/zmi/templates/raw-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/
--rw-rw-rw-   0 root         (0) root         (0)     1819 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/skin/templates/image.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/image/zmi/templates/image-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/
--rw-rw-rw-   0 root         (0) root         (0)     1999 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2895 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1382 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/skin/templates/jumbotron.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1234 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/zmi/templates/jumbotron-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2996 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/skin/templates/spacer-double.pt
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/skin/templates/spacer-thin.pt
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/skin/templates/spacer.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/zmi/templates/spacer-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/skin/
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8753 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/skin/page.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1197 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/skin/templates/layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1151 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/skin/templates/pagelet.pt
--rw-rw-rw-   0 root         (0) root         (0)     4078 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/slot.py
--rw-rw-rw-   0 root         (0) root         (0)    15310 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/tests/
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     1443 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5113 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8461 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    16525 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/layout.py
--rw-rw-rw-   0 root         (0) root         (0)    21523 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/portlet.py
--rw-rw-rw-   0 root         (0) root         (0)    13585 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/presentation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/css/
--rw-rw-rw-   0 root         (0) root         (0)    24268 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/css/layout.css
--rw-rw-rw-   0 root         (0) root         (0)    20882 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/css/layout.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/js/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/js/i18n/layout-fr.js
--rw-rw-rw-   0 root         (0) root         (0)    32192 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/js/layout.js
--rw-rw-rw-   0 root         (0) root         (0)    14898 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/js/layout.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/sass/
--rw-rw-rw-   0 root         (0) root         (0)    14582 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/resources/sass/layout.scss
--rw-rw-rw-   0 root         (0) root         (0)    14123 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/slot.py
--rw-rw-rw-   0 root         (0) root         (0)     6956 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/templates/empty.pt
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/templates/layout.pt
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/templates/portlet-hidden.pt
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/templates/portlet-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     2649 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/templates/presentation-template.pt
--rw-rw-rw-   0 root         (0) root         (0)     2110 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/templates/renderer-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/templates/setting-bool-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/templates/setting-none-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/templates/setting-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     1696 2023-03-14 08:39:31.000000 pyams_portal-1.8.1/src/pyams_portal/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5254 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4702 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      399 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-14 08:39:52.000000 pyams_portal-1.8.1/src/pyams_portal.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5458 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     3369 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2930 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/
+-rw-rw-rw-   0 root         (0) root         (0)      863 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    32697 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1735 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1929 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/generations/evolve1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/generations/evolve2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1808 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/generations/evolve3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/generations/evolve4.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/include.py
+-rw-rw-rw-   0 root         (0) root         (0)    19487 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    24258 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.mo
+-rw-rw-rw-   0 root         (0) root         (0)    39459 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.po
+-rw-rw-rw-   0 root         (0) root         (0)    27659 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/locales/pyams_portal.pot
+-rw-rw-rw-   0 root         (0) root         (0)    11053 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/page.py
+-rw-rw-rw-   0 root         (0) root         (0)    14662 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3516 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3002 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1946 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/skin/templates/cards-masonry.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2015 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/skin/templates/cards.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    10245 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/cards/zmi/templates/cards-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/skin/templates/carousel.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     9803 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/zmi/templates/carousel-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     5034 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/skin/templates/html.pt
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/skin/templates/raw-code.pt
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/skin/templates/raw.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2341 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/zmi/templates/html-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/html/zmi/templates/raw-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1819 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/skin/templates/image.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/image/zmi/templates/image-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2895 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/skin/templates/jumbotron.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/zmi/templates/jumbotron-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2996 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/skin/templates/spacer-double.pt
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/skin/templates/spacer-thin.pt
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/skin/templates/spacer.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/zmi/templates/spacer-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8759 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/skin/page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/skin/templates/layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/skin/templates/pagelet.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4159 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/slot.py
+-rw-rw-rw-   0 root         (0) root         (0)    15310 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1443 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     6388 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8461 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    16535 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/layout.py
+-rw-rw-rw-   0 root         (0) root         (0)    21546 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/portlet.py
+-rw-rw-rw-   0 root         (0) root         (0)    13637 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/presentation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/css/
+-rw-rw-rw-   0 root         (0) root         (0)    24268 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/css/layout.css
+-rw-rw-rw-   0 root         (0) root         (0)    20882 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/css/layout.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/js/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/js/i18n/layout-fr.js
+-rw-rw-rw-   0 root         (0) root         (0)    32192 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/js/layout.js
+-rw-rw-rw-   0 root         (0) root         (0)    14898 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/js/layout.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/sass/
+-rw-rw-rw-   0 root         (0) root         (0)    14582 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/resources/sass/layout.scss
+-rw-rw-rw-   0 root         (0) root         (0)    14054 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/slot.py
+-rw-rw-rw-   0 root         (0) root         (0)     6956 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/templates/empty.pt
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/templates/layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/templates/portlet-hidden.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/templates/portlet-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2649 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/templates/presentation-template.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2110 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/templates/renderer-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/templates/setting-bool-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/templates/setting-none-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/templates/setting-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-07-07 22:29:30.000000 pyams_portal-1.9.1/src/pyams_portal/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5458 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4702 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      399 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 22:29:48.000000 pyams_portal-1.9.1/src/pyams_portal.egg-info/top_level.txt
```

### Comparing `pyams_portal-1.8.1/LICENSE` & `pyams_portal-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/PKG-INFO` & `pyams_portal-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_portal
-Version: 1.8.1
+Version: 1.9.1
 Summary: PyAMS portlets management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -53,14 +53,25 @@
 content management packages like PyAMS_content, while other extension packages can be used to
 provide custom portlets renderers.
 
 
 Changelog
 =========
 
+1.9.1
+-----
+ - updated doctests
+
+1.9.0
+-----
+ - added slot CSS class to portlets container
+ - updated portlet previewer
+ - updated portlet edit form status
+ - bypass workflow state check on page preview
+
 1.8.1
 -----
  - use new sortable table base class
 
 1.8.0
 -----
  - added marker interfaces to handle header and footer templates
```

### Comparing `pyams_portal-1.8.1/docs/HISTORY.rst` & `pyams_portal-1.9.1/docs/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+1.9.1
+-----
+ - updated doctests
+
+1.9.0
+-----
+ - added slot CSS class to portlets container
+ - updated portlet previewer
+ - updated portlet edit form status
+ - bypass workflow state check on page preview
+
 1.8.1
 -----
  - use new sortable table base class
 
 1.8.0
 -----
  - added marker interfaces to handle header and footer templates
```

### Comparing `pyams_portal-1.8.1/docs/README.rst` & `pyams_portal-1.9.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/setup.py` & `pyams_portal-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.8.1'
+version = '1.9.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_catalog',
     'pyams_form',
     'pyams_zmi',
     'pyramid_zcml',
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/doctests/README.rst` & `pyams_portal-1.9.1/src/pyams_portal/doctests/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -611,29 +611,24 @@
 
 Portlets renderers can use a shared cache to store their content for a short duration; this
 cache is never used in preview mode.
 
     >>> renderer.use_portlets_cache
     True
 
-The cache key is based on the current hostname, on the context and on the current locale:
-
-    >>> renderer.get_cache_key()
-    'portlet::http::example.com:80::...::1::en'
-    >>> renderer.render()
-    Traceback (most recent call last):
-    ...
-    KeyError: 'portlets'
-
 Rendering portlets requires a matching cache region:
 
     >>> from beaker.cache import CacheManager, cache_regions
     >>> cache = CacheManager(**{'cache.type': 'memory'})
     >>> cache_regions.update({'portlets': {'type': 'memory', 'expire': 60}})
 
+The cache key is based on the current hostname, on the context and on the current locale:
+
+    >>> renderer.get_cache_key()
+    'portlet::http::example.com:80::...::1::en'
     >>> renderer.render()
     '<p>This is a test!</p>'
 
 A second rendering should use the cache:
 
     >>> renderer.render()
     '<p>This is a test!</p>'
@@ -670,18 +665,15 @@
     >>> from pyams_template.template import override_template
     >>> from pyams_portal.portlets.html.skin import HTMLPortletDefaultRenderer
 
     >>> override_template(HTMLPortletDefaultRenderer, name='custom',
     ...                   template=custom_template, layer=IPyAMSLayer)
 
     >>> folder_portlets[6].settings.get_renderer().render(template_name='custom')
-    '<p>This is a test!</p>'
-
-Why don't we get custom template content? This is because our renderer is using the cache, which
-was set on first render, before the custom template was registered!
+    '<div>This is a custom template!</div>'
 
 We can disable the cache by defining a "preview mode" on the request:
 
     >>> get_annotations(request)['PREVIEW_MODE'] = True
     >>> folder_portlets[6].settings.get_renderer().render(template_name='custom')
     '<div>This is a custom template!</div>'
 
@@ -724,16 +716,16 @@
       <body class="m-0 p-0">
         <div class="main container">
           <div>
             <div class="rows">
               <div class="row m-0">
                 <div class="slots w-100">
                   <div class="slot float-left col  col-12 col-sm-12 col-md-12 col-lg-12 col-xl-12 px-0">
-                    <div class="portlets">
-                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block  ">
+                    <div class="portlets ">
+                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block ">
                         <p>This is a test!</p>
                       </div>
                     </div>
                   </div>
                 </div>
               </div>
             </div>
@@ -755,16 +747,16 @@
       <body class="m-0 p-0">
         <div class="main container">
           <div>
             <div class="rows">
               <div class="row m-0">
                 <div class="slots w-100">
                   <div class="slot float-left col  col-12 col-sm-12 col-md-12 col-lg-12 col-xl-12 px-0">
-                    <div class="portlets">
-                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block  ">
+                    <div class="portlets ">
+                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block ">
                         <p>This is a test!</p>
                       </div>
                     </div>
                   </div>
                 </div>
               </div>
             </div>
@@ -793,19 +785,19 @@
       <body class="m-0 p-0">
         <div class="main container">
           <div>
             <div class="rows">
               <div class="row m-0">
                 <div class="slots w-100">
                   <div class="slot float-left col  col-12 col-sm-12 col-md-12 col-lg-12 col-xl-12 px-0">
-                    <div class="portlets">
-                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block  ">
+                    <div class="portlets ">
+                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block ">
                         <p>This is a test!</p>
                       </div>
-                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block  ">
+                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block ">
                         <div class="source"><pre><span></span><span class="linenos">1</span>*This* is my code
                           </pre></div>
                       </div>
                     </div>
                   </div>
                 </div>
               </div>
@@ -827,19 +819,19 @@
       <body class="m-0 p-0">
         <div class="main container">
           <div>
             <div class="rows">
               <div class="row m-0">
                 <div class="slots w-100">
                   <div class="slot float-left col  col-12 col-sm-12 col-md-12 col-lg-12 col-xl-12 px-0">
-                    <div class="portlets">
-                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block  ">
+                    <div class="portlets ">
+                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block ">
                         <p>This is a test!</p>
                       </div>
-                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block  ">
+                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block ">
                         <p><em>This</em> is my code</p>
                       </div>
                     </div>
                   </div>
                 </div>
               </div>
             </div>
@@ -860,19 +852,19 @@
       <body class="m-0 p-0">
         <div class="main container">
           <div>
             <div class="rows">
               <div class="row m-0">
                 <div class="slots w-100">
                   <div class="slot float-left col  col-12 col-sm-12 col-md-12 col-lg-12 col-xl-12 px-0">
-                    <div class="portlets">
-                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block  ">
+                    <div class="portlets ">
+                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block ">
                         <p>This is a test!</p>
                       </div>
-                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block  ">
+                      <div class="portlet d-block d-sm-block d-md-block d-lg-block d-xl-block ">
                         <p><em>This</em> is my code</p>
                       </div>
                     </div>
                   </div>
                 </div>
               </div>
             </div>
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/generations/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/generations/evolve1.py` & `pyams_portal-1.9.1/src/pyams_portal/generations/evolve1.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/generations/evolve2.py` & `pyams_portal-1.9.1/src/pyams_portal/generations/evolve2.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/generations/evolve3.py` & `pyams_portal-1.9.1/src/pyams_portal/generations/evolve3.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/generations/evolve4.py` & `pyams_portal-1.9.1/src/pyams_portal/generations/evolve4.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/include.py` & `pyams_portal-1.9.1/src/pyams_portal/include.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/interfaces.py` & `pyams_portal-1.9.1/src/pyams_portal/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,18 @@
                    min=0,
                    max=12)
 
     css_class = TextLine(title=_("CSS class"),
                          description=_("CSS class applied to this slot"),
                          required=False)
 
+    portlets_css_class = TextLine(title=_("Portlets CSS class"),
+                                  description=_("CSS class applied to the inner portlets container"),
+                                  required=False)
+
     prefix = Text(title=_("HTML prefix"),
                   description=_("This HTML code with be included, as is, before the first "
                                 "portlet"),
                   required=False)
 
     suffix = Text(title=_("HTML suffix"),
                   description=_("This HTML code will be included, as is, after the last "
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.mo` & `pyams_portal-1.9.1/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -122,19 +122,25 @@
 
 msgid "Button status"
 msgstr "Statut du bouton"
 
 msgid "CSS class"
 msgstr "Classe CSS"
 
+msgid "CSS class applied to the inner portlets container"
+msgstr ""
+"Classe CSS spécifique appliquée au conteneur intermédiaire des composants"
+
 msgid "CSS class applied to this slot"
 msgstr "Classe CSS spécifique appliquée à ce bloc"
 
 msgid "CSS class applied to this slot container"
-msgstr "Classe CSS spécifique appliquée au conteneur de ce bloc"
+msgstr ""
+"Classe CSS spécifique appliquée au conteneur de ce bloc ; dans le cas où "
+"aucune classe CSS n'est indiquée, ce conteneur n'est pas créé"
 
 msgid "Card properties"
 msgstr "Propriétés de la carte"
 
 msgid "Card's CSS class"
 msgstr "Classe CSS"
 
@@ -543,14 +549,17 @@
 msgstr ""
 "Les propriétés du composant sont différentes de celles du modèle de "
 "présentation"
 
 msgid "Portlet: {portlet}"
 msgstr "Composant « {portlet} »"
 
+msgid "Portlets CSS class"
+msgstr "Classe CSS du conteneur des composants"
+
 msgid "Presentation"
 msgstr "Présentation"
 
 msgid "Previous"
 msgstr "Précédent"
 
 msgid "Properties"
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.po` & `pyams_portal-1.9.1/src/pyams_portal/locales/fr/LC_MESSAGES/pyams_portal.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2023-01-30 08:56+0100\n"
+"POT-Creation-Date: 2023-05-28 12:14+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.14\n"
 
-#: src/pyams_portal/include.py:42
+#: src/pyams_portal/include.py:43
 msgid "Manage presentation templates"
 msgstr "Gérer les modèles de présentation"
 
-#: src/pyams_portal/include.py:48
+#: src/pyams_portal/include.py:49
 msgid "Designer (role)"
 msgstr "Designer (rôle)"
 
 #: src/pyams_portal/interfaces.py:83
 msgid "Portlet"
 msgstr "Composant"
 
@@ -87,15 +87,17 @@
 
 #: src/pyams_portal/interfaces.py:266
 msgid "Container CSS class"
 msgstr "Classe CSS du conteneur"
 
 #: src/pyams_portal/interfaces.py:267
 msgid "CSS class applied to this slot container"
-msgstr "Classe CSS spécifique appliquée au conteneur de ce bloc"
+msgstr ""
+"Classe CSS spécifique appliquée au conteneur de ce bloc ; dans le cas où aucune "
+"classe CSS n'est indiquée, ce conteneur n'est pas créé"
 
 #: src/pyams_portal/interfaces.py:270
 msgid "Extra small device width"
 msgstr "Largeur sur très petits périphériques"
 
 #: src/pyams_portal/interfaces.py:271
 msgid ""
@@ -154,192 +156,200 @@
 "Slot width, in columns count, on extra large desktop devices (&gt;= 1200 "
 "pixels); set to 0 to hide the slot"
 msgstr ""
 "Largeur du bloc, en nombre de colonnes, sur les très grands périphériques "
 "(&gt;= 1200 pixels) ; indiquez une valeur de 0 pour ne pas afficher ce bloc "
 "sur ce type de périphérique..."
 
-#: src/pyams_portal/interfaces.py:305 src/pyams_portal/interfaces.py:438
+#: src/pyams_portal/interfaces.py:305 src/pyams_portal/interfaces.py:442
 #: src/pyams_portal/zmi/templates/presentation-template.pt:46
 #: src/pyams_portal/portlets/cards/interfaces.py:76
 #: src/pyams_portal/portlets/cards/skin/interfaces.py:34
 #: src/pyams_portal/portlets/cards/skin/interfaces.py:52
 #: src/pyams_portal/portlets/carousel/skin/interfaces.py:34
 msgid "CSS class"
 msgstr "Classe CSS"
 
 #: src/pyams_portal/interfaces.py:306
 msgid "CSS class applied to this slot"
 msgstr "Classe CSS spécifique appliquée à ce bloc"
 
 #: src/pyams_portal/interfaces.py:309
+msgid "Portlets CSS class"
+msgstr "Classe CSS du conteneur des composants"
+
+#: src/pyams_portal/interfaces.py:310
+msgid "CSS class applied to the inner portlets container"
+msgstr "Classe CSS spécifique appliquée au conteneur intermédiaire des composants"
+
+#: src/pyams_portal/interfaces.py:313
 msgid "HTML prefix"
 msgstr "Préfixe HTML"
 
-#: src/pyams_portal/interfaces.py:310
+#: src/pyams_portal/interfaces.py:314
 msgid "This HTML code with be included, as is, before the first portlet"
 msgstr ""
 "Ce code HTML sera intégré dans la page, en l'état, juste avant le premier "
 "composant"
 
-#: src/pyams_portal/interfaces.py:314
+#: src/pyams_portal/interfaces.py:318
 msgid "HTML suffix"
 msgstr "Suffixe HTML"
 
-#: src/pyams_portal/interfaces.py:315
+#: src/pyams_portal/interfaces.py:319
 msgid "This HTML code will be included, as is, after the last portlet"
 msgstr ""
 "Ce code HTML sera intégré dans la page, en l'état, juste après le dernier "
 "composant"
 
-#: src/pyams_portal/interfaces.py:434
+#: src/pyams_portal/interfaces.py:438
 msgid "Template name"
 msgstr "Nom du modèle"
 
-#: src/pyams_portal/interfaces.py:435
+#: src/pyams_portal/interfaces.py:439
 msgid "Explicit name given to portal template"
 msgstr "Nom explicite du modèle de présentation"
 
-#: src/pyams_portal/interfaces.py:439
+#: src/pyams_portal/interfaces.py:443
 #: src/pyams_portal/zmi/templates/presentation-template.pt:48
 msgid "This CSS class will be used as main template container CSS class"
 msgstr ""
 "Cette classe CSS sera appliquée comme classe principale du conteneur du "
 "modèle de présentation, lors du rendu en front-office"
 
-#: src/pyams_portal/interfaces.py:449
+#: src/pyams_portal/interfaces.py:453
 msgid "Access menu from home"
 msgstr "Ajouter un accès depuis l'accueil"
 
-#: src/pyams_portal/interfaces.py:450
+#: src/pyams_portal/interfaces.py:454
 msgid ""
 "If 'yes', a menu will be displayed to get access to portal templates "
 "container from site admin home page"
 msgstr ""
 "Si 'oui', un menu d'accès au gestionnaire de modèles de présentation sera "
 "ajouté depuis la page d'accueil de l'interface d'administration du site"
 
-#: src/pyams_portal/interfaces.py:467
+#: src/pyams_portal/interfaces.py:471
 msgid "Designers"
 msgstr "Designers"
 
-#: src/pyams_portal/interfaces.py:468
+#: src/pyams_portal/interfaces.py:472
 msgid "List of designers allowed to manage presentation templates"
 msgstr "Liste des mandataires hbailités à gérer les modèles de présentation"
 
-#: src/pyams_portal/interfaces.py:477
+#: src/pyams_portal/interfaces.py:481
 msgid "Toolbar portlets"
 msgstr "Composants de la barre d'outils"
 
-#: src/pyams_portal/interfaces.py:478
+#: src/pyams_portal/interfaces.py:482
 msgid ""
 "These portlets will be directly available in templates configuration page "
 "toolbar"
 msgstr ""
 "Les composants sélectionnés seront accessibles directement dans la barre "
 "d'outils de configuration des modèles de présentation"
 
-#: src/pyams_portal/interfaces.py:512
+#: src/pyams_portal/interfaces.py:516
 msgid "Inherit parent template?"
 msgstr "Hériter du modèle du parent ?"
 
-#: src/pyams_portal/interfaces.py:513
+#: src/pyams_portal/interfaces.py:517
 msgid "Should we reuse parent template?"
 msgstr "Si 'oui', le même modèle que le niveau parent sera utilisé"
 
-#: src/pyams_portal/interfaces.py:517
+#: src/pyams_portal/interfaces.py:521
 msgid "Override parent template?"
 msgstr "Redéfinir le modèle de présentation"
 
-#: src/pyams_portal/interfaces.py:518
+#: src/pyams_portal/interfaces.py:522
 msgid "Should we override parent template?"
 msgstr "Si 'oui', le modèle du niveau parent ne sera pas utilisé"
 
-#: src/pyams_portal/interfaces.py:522
+#: src/pyams_portal/interfaces.py:526
 msgid "Use local template?"
 msgstr "Utiliser un modèle spécifique"
 
-#: src/pyams_portal/interfaces.py:523
+#: src/pyams_portal/interfaces.py:527
 msgid ""
 "If 'yes', you can define a custom local template instead of a shared template"
 msgstr ""
 "Si 'oui', vous pouvez choisir d'utiliser un modèle de présentation propre à "
 "ce contexte plutôt qu'un modèle de présentation partagé"
 
-#: src/pyams_portal/interfaces.py:528 src/pyams_portal/zmi/portlet.py:132
+#: src/pyams_portal/interfaces.py:532 src/pyams_portal/zmi/portlet.py:132
 #: src/pyams_portal/zmi/portlet.py:257 src/pyams_portal/zmi/slot.py:65
 msgid "Local template"
 msgstr "Modèle de présentation spécifique"
 
-#: src/pyams_portal/interfaces.py:533
+#: src/pyams_portal/interfaces.py:537
 msgid "Use shared template?"
 msgstr "Utiliser un modèle partagé"
 
-#: src/pyams_portal/interfaces.py:534
+#: src/pyams_portal/interfaces.py:538
 msgid "If 'yes', you can select a shared template"
 msgstr ""
 "Si 'oui', vous pouvez sélectionner un modèle de présentation partagé pour "
 "prendre en charge la présentation de ce contexte"
 
-#: src/pyams_portal/interfaces.py:538
+#: src/pyams_portal/interfaces.py:542
 msgid "Page template"
 msgstr "Modèle de présentation"
 
-#: src/pyams_portal/interfaces.py:539
+#: src/pyams_portal/interfaces.py:543
 msgid "Template used for this page"
 msgstr "Modèle de présentation utilisé pour ce contexte"
 
-#: src/pyams_portal/zmi/presentation.py:63
+#: src/pyams_portal/zmi/presentation.py:65
 msgid "Presentation"
 msgstr "Présentation"
 
-#: src/pyams_portal/zmi/presentation.py:74
+#: src/pyams_portal/zmi/presentation.py:76
 msgid "Page template configuration"
 msgstr "Choix du modèle de présentation"
 
-#: src/pyams_portal/zmi/presentation.py:130
+#: src/pyams_portal/zmi/presentation.py:132
 msgid "Header presentation"
 msgstr "En-tête de page"
 
-#: src/pyams_portal/zmi/presentation.py:141
+#: src/pyams_portal/zmi/presentation.py:143
 msgid "Page header template configuration"
 msgstr "Modèle de présentation de l'en-tête de page"
 
-#: src/pyams_portal/zmi/presentation.py:158
+#: src/pyams_portal/zmi/presentation.py:160
 msgid "Footer presentation"
 msgstr "Pied de page"
 
-#: src/pyams_portal/zmi/presentation.py:169
+#: src/pyams_portal/zmi/presentation.py:171
 msgid "Page footer template configuration"
 msgstr "Modèle de présentation du pied de page"
 
-#: src/pyams_portal/zmi/presentation.py:191
+#: src/pyams_portal/zmi/presentation.py:193
 msgid ""
 "You must choose between using a shared template or a local template if you "
 "don't inherit from parent template!"
 msgstr ""
 "Vous devez choisir un modèle partagé ou un modèle spécifique si vous "
 "n'héritez pas du modèle de présentation du parent !"
 
-#: src/pyams_portal/zmi/presentation.py:197
+#: src/pyams_portal/zmi/presentation.py:199
 msgid "You must select a template when setting shared template mode!"
 msgstr ""
 "Vous devez choisir un modèle lorsque vous souhaitez utiliser un modèle "
 "partagé !"
 
-#: src/pyams_portal/zmi/presentation.py:250
+#: src/pyams_portal/zmi/presentation.py:252
 msgid "No selected template"
 msgstr "Pas de modèle sélectionné"
 
-#: src/pyams_portal/zmi/presentation.py:251
-#: src/pyams_portal/zmi/presentation.py:252
+#: src/pyams_portal/zmi/presentation.py:253
+#: src/pyams_portal/zmi/presentation.py:254
 msgid "Please select template..."
 msgstr "Veuillez choisir un modèle de présentation..."
 
-#: src/pyams_portal/zmi/presentation.py:266
+#: src/pyams_portal/zmi/presentation.py:268
 msgid ""
 "If you select a shared template or choose to inherit from parent "
 "configuration, you can adjust settings of each portlet but can't change page "
 "configuration.\n"
 "If you choose to use a local template, it's configuration will only be "
 "reusable in sub-levels which will choose to inherit from it."
 msgstr ""
@@ -347,23 +357,23 @@
 "de la configuration du niveau parent, vous pourrez ajuster les paramètres de "
 "chaque composant mais vous ne pourrez pas modifier la configuration de la "
 "page.\n"
 "Si vous choisissez d'utiliser un modèle de présentation spécifique, vous "
 "aurez toute liberté pour paramétrer ce modèle, mais il ne sera réutilisable "
 "que dans les sous-niveaux qui choisiront d'en hériter."
 
-#: src/pyams_portal/zmi/presentation.py:284 src/pyams_portal/zmi/layout.py:80
+#: src/pyams_portal/zmi/presentation.py:286 src/pyams_portal/zmi/layout.py:80
 msgid "Page layout"
 msgstr "Mise en page"
 
-#: src/pyams_portal/zmi/presentation.py:319
+#: src/pyams_portal/zmi/presentation.py:321
 msgid "Header layout"
 msgstr "Mise en page"
 
-#: src/pyams_portal/zmi/presentation.py:341
+#: src/pyams_portal/zmi/presentation.py:343
 msgid "Footer layout"
 msgstr "Mise en page"
 
 #: src/pyams_portal/zmi/layout.py:69
 msgid "Portal template"
 msgstr "Modèle de présentation"
 
@@ -457,18 +467,18 @@
 
 #: src/pyams_portal/zmi/portlet.py:259
 #, python-format
 msgid "{} (inherited from parent)"
 msgstr "{} (hérité du parent)"
 
 #: src/pyams_portal/zmi/portlet.py:265
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:226
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:277
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:208
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:257
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:220
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:271
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:203
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:252
 #, python-format
 msgid "Portlet configuration: « {} »"
 msgstr "Configuration du composant « {} »"
 
 #: src/pyams_portal/zmi/portlet.py:359
 msgid ""
 "WARNING: portlet configuration is saved immediately when inherit mode is "
@@ -560,15 +570,15 @@
 msgstr "Le numéro de ligne doit être compris entre 1 et {} !"
 
 #: src/pyams_portal/zmi/slot.py:192
 #, python-format
 msgid "« {} » slot properties"
 msgstr "Propriétés du bloc « {} »"
 
-#: src/pyams_portal/zmi/slot.py:228
+#: src/pyams_portal/zmi/slot.py:226
 msgid "HTML codes"
 msgstr "Codes HTML"
 
 #: src/pyams_portal/zmi/template.py:60
 msgid "Add template"
 msgstr "Ajouter un modèle de présentation"
 
@@ -710,17 +720,17 @@
 msgstr "Carte visible ?"
 
 #: src/pyams_portal/portlets/cards/interfaces.py:42
 msgid "Card's title"
 msgstr "Titre de la carte"
 
 #: src/pyams_portal/portlets/cards/interfaces.py:45
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:152
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:146
 #: src/pyams_portal/portlets/carousel/interfaces.py:51
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:143
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:138
 msgid "Illustration"
 msgstr "Illustration"
 
 #: src/pyams_portal/portlets/cards/interfaces.py:46
 msgid "Card's illustration"
 msgstr "Image d'illustration de la carte"
 
@@ -783,18 +793,18 @@
 msgstr "Statut correspondant à la couleur du bouton"
 
 #: src/pyams_portal/portlets/cards/interfaces.py:77
 msgid "Card's CSS class"
 msgstr "Classe CSS"
 
 #: src/pyams_portal/portlets/cards/interfaces.py:86
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:122
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:116
 #: src/pyams_portal/portlets/carousel/interfaces.py:43
 #: src/pyams_portal/portlets/carousel/interfaces.py:65
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:119
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:114
 #: src/pyams_portal/portlets/jumbotron/interfaces.py:35
 #: src/pyams_portal/portlets/html/interfaces.py:29
 msgid "Title"
 msgstr "Titre"
 
 #: src/pyams_portal/portlets/cards/interfaces.py:87
 #: src/pyams_portal/portlets/carousel/interfaces.py:66
@@ -813,48 +823,48 @@
 msgid "Short text to be displayed below title"
 msgstr "Texte court affiché en-dessous du titre"
 
 #: src/pyams_portal/portlets/cards/__init__.py:109
 msgid "Bootstrap: cards"
 msgstr "Bootstrap: cartes"
 
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:105
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:99
 msgid "Click icon to show or hide card"
 msgstr "Cliquer pour afficher ou masquer la carte"
 
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:131
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:125
 msgid "Target"
 msgstr "Cible"
 
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:184
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:178
 msgid "List of portlet cards"
 msgstr "Liste des cartes"
 
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:205
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:199
 msgid "Add card"
 msgstr "Ajouter une carte"
 
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:227
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:221
 msgid "Add new card"
 msgstr "Ajouter une carte"
 
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:230
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:224
 msgid "New card properties"
 msgstr "Propriétés de la nouvelle carte"
 
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:278
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:272
 #, python-format
 msgid "Card: {}"
 msgstr "Carte « {} »"
 
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:281
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:275
 msgid "Card properties"
 msgstr "Propriétés de la carte"
 
-#: src/pyams_portal/portlets/cards/zmi/__init__.py:310
+#: src/pyams_portal/portlets/cards/zmi/__init__.py:304
 msgid "Action button"
 msgstr "Bouton d'action"
 
 #: src/pyams_portal/portlets/cards/zmi/templates/cards-preview.pt:4
 msgid "Cards list:"
 msgstr "Liste des cartes :"
 
@@ -967,40 +977,40 @@
 "Durée d'affichage de l'image, en secondes, lorsque le balayage automatique "
 "est activé"
 
 #: src/pyams_portal/portlets/carousel/__init__.py:103
 msgid "Bootstrap: carousel"
 msgstr "Bootstrap: carousel"
 
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:128
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:123
 msgid "Lead"
 msgstr "En-tête"
 
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:172
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:167
 msgid "List of carousel items"
 msgstr "Liste des images du carousel"
 
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:193
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:188
 msgid "Add image"
 msgstr "Ajouter une image"
 
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:209
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:204
 msgid "Add new image"
 msgstr "Ajouter une image"
 
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:212
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:207
 msgid "New image properties"
 msgstr "Propriétés de la nouvelle image"
 
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:258
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:253
 #, python-format
 msgid "Image: {}"
 msgstr "Image « {} »"
 
-#: src/pyams_portal/portlets/carousel/zmi/__init__.py:261
+#: src/pyams_portal/portlets/carousel/zmi/__init__.py:256
 msgid "Carousel image properties"
 msgstr "Propriétés de l'image"
 
 #: src/pyams_portal/portlets/carousel/zmi/templates/carousel-preview.pt:3
 msgid "Items list:"
 msgstr "Liste des images :"
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/locales/pyams_portal.pot` & `pyams_portal-1.9.1/src/pyams_portal/locales/pyams_portal.pot`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2023-01-30 08:56+0100\n"
+"POT-Creation-Date: 2023-05-28 12:14+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.15.0\n"
 
-#: ./src/pyams_portal/include.py:42
+#: ./src/pyams_portal/include.py:43
 msgid "Manage presentation templates"
 msgstr ""
 
-#: ./src/pyams_portal/include.py:48
+#: ./src/pyams_portal/include.py:49
 msgid "Designer (role)"
 msgstr ""
 
 #: ./src/pyams_portal/interfaces.py:83
 msgid "Portlet"
 msgstr ""
 
@@ -136,189 +136,197 @@
 
 #: ./src/pyams_portal/interfaces.py:299
 msgid ""
 "Slot width, in columns count, on extra large desktop devices (&gt;= 1200 "
 "pixels); set to 0 to hide the slot"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:305 ./src/pyams_portal/interfaces.py:438
+#: ./src/pyams_portal/interfaces.py:305 ./src/pyams_portal/interfaces.py:442
 #: ./src/pyams_portal/zmi/templates/presentation-template.pt:46
 #: ./src/pyams_portal/portlets/cards/interfaces.py:76
 #: ./src/pyams_portal/portlets/cards/skin/interfaces.py:34
 #: ./src/pyams_portal/portlets/cards/skin/interfaces.py:52
 #: ./src/pyams_portal/portlets/carousel/skin/interfaces.py:34
 msgid "CSS class"
 msgstr ""
 
 #: ./src/pyams_portal/interfaces.py:306
 msgid "CSS class applied to this slot"
 msgstr ""
 
 #: ./src/pyams_portal/interfaces.py:309
-msgid "HTML prefix"
+msgid "Portlets CSS class"
 msgstr ""
 
 #: ./src/pyams_portal/interfaces.py:310
-msgid "This HTML code with be included, as is, before the first portlet"
+msgid "CSS class applied to the inner portlets container"
+msgstr ""
+
+#: ./src/pyams_portal/interfaces.py:313
+msgid "HTML prefix"
 msgstr ""
 
 #: ./src/pyams_portal/interfaces.py:314
+msgid "This HTML code with be included, as is, before the first portlet"
+msgstr ""
+
+#: ./src/pyams_portal/interfaces.py:318
 msgid "HTML suffix"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:315
+#: ./src/pyams_portal/interfaces.py:319
 msgid "This HTML code will be included, as is, after the last portlet"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:434
+#: ./src/pyams_portal/interfaces.py:438
 msgid "Template name"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:435
+#: ./src/pyams_portal/interfaces.py:439
 msgid "Explicit name given to portal template"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:439
+#: ./src/pyams_portal/interfaces.py:443
 #: ./src/pyams_portal/zmi/templates/presentation-template.pt:48
 msgid "This CSS class will be used as main template container CSS class"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:449
+#: ./src/pyams_portal/interfaces.py:453
 msgid "Access menu from home"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:450
+#: ./src/pyams_portal/interfaces.py:454
 msgid ""
 "If 'yes', a menu will be displayed to get access to portal templates "
 "container from site admin home page"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:467
+#: ./src/pyams_portal/interfaces.py:471
 msgid "Designers"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:468
+#: ./src/pyams_portal/interfaces.py:472
 msgid "List of designers allowed to manage presentation templates"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:477
+#: ./src/pyams_portal/interfaces.py:481
 msgid "Toolbar portlets"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:478
+#: ./src/pyams_portal/interfaces.py:482
 msgid ""
 "These portlets will be directly available in templates configuration page "
 "toolbar"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:512
+#: ./src/pyams_portal/interfaces.py:516
 msgid "Inherit parent template?"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:513
+#: ./src/pyams_portal/interfaces.py:517
 msgid "Should we reuse parent template?"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:517
+#: ./src/pyams_portal/interfaces.py:521
 msgid "Override parent template?"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:518
+#: ./src/pyams_portal/interfaces.py:522
 msgid "Should we override parent template?"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:522
+#: ./src/pyams_portal/interfaces.py:526
 msgid "Use local template?"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:523
+#: ./src/pyams_portal/interfaces.py:527
 msgid ""
 "If 'yes', you can define a custom local template instead of a shared template"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:528 ./src/pyams_portal/zmi/portlet.py:132
+#: ./src/pyams_portal/interfaces.py:532 ./src/pyams_portal/zmi/portlet.py:132
 #: ./src/pyams_portal/zmi/portlet.py:257 ./src/pyams_portal/zmi/slot.py:65
 msgid "Local template"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:533
+#: ./src/pyams_portal/interfaces.py:537
 msgid "Use shared template?"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:534
+#: ./src/pyams_portal/interfaces.py:538
 msgid "If 'yes', you can select a shared template"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:538
+#: ./src/pyams_portal/interfaces.py:542
 msgid "Page template"
 msgstr ""
 
-#: ./src/pyams_portal/interfaces.py:539
+#: ./src/pyams_portal/interfaces.py:543
 msgid "Template used for this page"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:63
+#: ./src/pyams_portal/zmi/presentation.py:65
 msgid "Presentation"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:74
+#: ./src/pyams_portal/zmi/presentation.py:76
 msgid "Page template configuration"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:130
+#: ./src/pyams_portal/zmi/presentation.py:132
 msgid "Header presentation"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:141
+#: ./src/pyams_portal/zmi/presentation.py:143
 msgid "Page header template configuration"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:158
+#: ./src/pyams_portal/zmi/presentation.py:160
 msgid "Footer presentation"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:169
+#: ./src/pyams_portal/zmi/presentation.py:171
 msgid "Page footer template configuration"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:191
+#: ./src/pyams_portal/zmi/presentation.py:193
 msgid ""
 "You must choose between using a shared template or a local template if you "
 "don't inherit from parent template!"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:197
+#: ./src/pyams_portal/zmi/presentation.py:199
 msgid "You must select a template when setting shared template mode!"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:250
+#: ./src/pyams_portal/zmi/presentation.py:252
 msgid "No selected template"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:251
-#: ./src/pyams_portal/zmi/presentation.py:252
+#: ./src/pyams_portal/zmi/presentation.py:253
+#: ./src/pyams_portal/zmi/presentation.py:254
 msgid "Please select template..."
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:266
+#: ./src/pyams_portal/zmi/presentation.py:268
 msgid ""
 "If you select a shared template or choose to inherit from parent configuration, you can adjust settings of each portlet but can't change page configuration.\n"
 "If you choose to use a local template, it's configuration will only be reusable in sub-levels which will choose to inherit from it."
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:284
+#: ./src/pyams_portal/zmi/presentation.py:286
 #: ./src/pyams_portal/zmi/layout.py:80
 msgid "Page layout"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:319
+#: ./src/pyams_portal/zmi/presentation.py:321
 msgid "Header layout"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/presentation.py:341
+#: ./src/pyams_portal/zmi/presentation.py:343
 msgid "Footer layout"
 msgstr ""
 
 #: ./src/pyams_portal/zmi/layout.py:69
 msgid "Portal template"
 msgstr ""
 
@@ -402,18 +410,18 @@
 
 #: ./src/pyams_portal/zmi/portlet.py:259
 #, python-format
 msgid "{} (inherited from parent)"
 msgstr ""
 
 #: ./src/pyams_portal/zmi/portlet.py:265
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:226
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:277
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:208
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:257
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:220
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:271
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:203
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:252
 #, python-format
 msgid "Portlet configuration: « {} »"
 msgstr ""
 
 #: ./src/pyams_portal/zmi/portlet.py:359
 msgid ""
 "WARNING: portlet configuration is saved immediately when inherit mode is "
@@ -502,15 +510,15 @@
 msgstr ""
 
 #: ./src/pyams_portal/zmi/slot.py:192
 #, python-format
 msgid "« {} » slot properties"
 msgstr ""
 
-#: ./src/pyams_portal/zmi/slot.py:228
+#: ./src/pyams_portal/zmi/slot.py:226
 msgid "HTML codes"
 msgstr ""
 
 #: ./src/pyams_portal/zmi/template.py:60
 msgid "Add template"
 msgstr ""
 
@@ -646,17 +654,17 @@
 msgstr ""
 
 #: ./src/pyams_portal/portlets/cards/interfaces.py:42
 msgid "Card's title"
 msgstr ""
 
 #: ./src/pyams_portal/portlets/cards/interfaces.py:45
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:152
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:146
 #: ./src/pyams_portal/portlets/carousel/interfaces.py:51
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:143
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:138
 msgid "Illustration"
 msgstr ""
 
 #: ./src/pyams_portal/portlets/cards/interfaces.py:46
 msgid "Card's illustration"
 msgstr ""
 
@@ -716,18 +724,18 @@
 msgstr ""
 
 #: ./src/pyams_portal/portlets/cards/interfaces.py:77
 msgid "Card's CSS class"
 msgstr ""
 
 #: ./src/pyams_portal/portlets/cards/interfaces.py:86
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:122
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:116
 #: ./src/pyams_portal/portlets/carousel/interfaces.py:43
 #: ./src/pyams_portal/portlets/carousel/interfaces.py:65
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:119
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:114
 #: ./src/pyams_portal/portlets/jumbotron/interfaces.py:35
 #: ./src/pyams_portal/portlets/html/interfaces.py:29
 msgid "Title"
 msgstr ""
 
 #: ./src/pyams_portal/portlets/cards/interfaces.py:87
 #: ./src/pyams_portal/portlets/carousel/interfaces.py:66
@@ -746,48 +754,48 @@
 msgid "Short text to be displayed below title"
 msgstr ""
 
 #: ./src/pyams_portal/portlets/cards/__init__.py:109
 msgid "Bootstrap: cards"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:105
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:99
 msgid "Click icon to show or hide card"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:131
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:125
 msgid "Target"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:184
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:178
 msgid "List of portlet cards"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:205
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:199
 msgid "Add card"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:227
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:221
 msgid "Add new card"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:230
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:224
 msgid "New card properties"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:278
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:272
 #, python-format
 msgid "Card: {}"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:281
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:275
 msgid "Card properties"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:310
+#: ./src/pyams_portal/portlets/cards/zmi/__init__.py:304
 msgid "Action button"
 msgstr ""
 
 #: ./src/pyams_portal/portlets/cards/zmi/templates/cards-preview.pt:4
 msgid "Cards list:"
 msgstr ""
 
@@ -894,40 +902,40 @@
 msgid "Image slide duration, in seconds"
 msgstr ""
 
 #: ./src/pyams_portal/portlets/carousel/__init__.py:103
 msgid "Bootstrap: carousel"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:128
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:123
 msgid "Lead"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:172
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:167
 msgid "List of carousel items"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:193
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:188
 msgid "Add image"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:209
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:204
 msgid "Add new image"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:212
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:207
 msgid "New image properties"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:258
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:253
 #, python-format
 msgid "Image: {}"
 msgstr ""
 
-#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:261
+#: ./src/pyams_portal/portlets/carousel/zmi/__init__.py:256
 msgid "Carousel image properties"
 msgstr ""
 
 #: ./src/pyams_portal/portlets/carousel/zmi/templates/carousel-preview.pt:3
 msgid "Items list:"
 msgstr ""
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/page.py` & `pyams_portal-1.9.1/src/pyams_portal/page.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlet.py` & `pyams_portal-1.9.1/src/pyams_portal/portlet.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/cards/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/cards/interfaces.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/cards/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/cards/skin/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/cards/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/cards/skin/interfaces.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/cards/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/cards/skin/templates/cards-masonry.pt` & `pyams_portal-1.9.1/src/pyams_portal/portlets/cards/skin/templates/cards-masonry.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/cards/skin/templates/cards.pt` & `pyams_portal-1.9.1/src/pyams_portal/portlets/cards/skin/templates/cards.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/cards/zmi/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/cards/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/interfaces.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/skin/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/skin/interfaces.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/skin/templates/carousel.pt` & `pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/skin/templates/carousel.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/carousel/zmi/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/carousel/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/html/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/html/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/html/interfaces.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/html/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/html/skin/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/html/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/html/zmi/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/html/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/html/zmi/templates/raw-preview.pt` & `pyams_portal-1.9.1/src/pyams_portal/portlets/html/zmi/templates/raw-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/image/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/image/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/image/interfaces.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/image/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/image/skin/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/image/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/image/zmi/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/image/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/image/zmi/templates/image-preview.pt` & `pyams_portal-1.9.1/src/pyams_portal/portlets/image/zmi/templates/image-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/interfaces.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/skin/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/skin/templates/jumbotron.pt` & `pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/skin/templates/jumbotron.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/jumbotron/zmi/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/jumbotron/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/interfaces.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/skin/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/portlets/spacer/zmi/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/portlets/spacer/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/skin/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/skin/page.py` & `pyams_portal-1.9.1/src/pyams_portal/skin/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 @pagelet_config(name='preview.html',
                 context=IPortalContext, layer=IPyAMSLayer,
                 permission=VIEW_SYSTEM_PERMISSION)
 class PortalContextPreviewPage(PortalContextIndexPage):
     """Portal context preview page"""
 
     def update(self):
-        # Bypass publication status in preview
+        # Bypass publication status check in preview
         get_annotations(self.request)[PREVIEW_MODE] = True  # pylint: disable=no-member
         super(PortalContextIndexPage, self).update()  # pylint: disable=bad-super-call
 
 
 #
 # Templates classes
 #
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/skin/templates/layout.pt` & `pyams_portal-1.9.1/src/pyams_portal/skin/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/skin/templates/pagelet.pt` & `pyams_portal-1.9.1/src/pyams_portal/skin/templates/pagelet.pt`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 			<div class="slots w-100">
 				<tal:loop repeat="slot_name template_config.get_slots(row)">
 					<div tal:define="slot_config template_config.get_slot_configuration(slot_name)"
 						 tal:condition="slot_config.visible"
 						 tal:omit-tag="not:slot_config.container_css_class"
 						 class="${slot_config.container_css_class}">
 						<div class="slot float-left ${slot_config.get_css_class()} px-0">
-							<div class="portlets">
+							<div class="portlets ${slot_config.portlets_css_class}">
 								${structure:slot_config.prefix or ''}
 								<tal:loop repeat="portlet_id template_config.slot_config[slot_name].portlet_ids">
 									<div tal:define="portlet view.render_portlet(portlet_id).strip()"
 										 tal:condition="portlet"
 										 class="portlet ${view.get_portlet_css_class(portlet_id)}">
 										${structure:portlet}
 									</div>
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/slot.py` & `pyams_portal-1.9.1/src/pyams_portal/slot.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     container_css_class = FieldProperty(ISlotConfiguration['container_css_class'])
     xs_width = FieldProperty(ISlotConfiguration['xs_width'])
     sm_width = FieldProperty(ISlotConfiguration['sm_width'])
     md_width = FieldProperty(ISlotConfiguration['md_width'])
     lg_width = FieldProperty(ISlotConfiguration['lg_width'])
     xl_width = FieldProperty(ISlotConfiguration['xl_width'])
     css_class = FieldProperty(ISlotConfiguration['css_class'])
+    portlets_css_class = FieldProperty(ISlotConfiguration['portlets_css_class'])
     prefix = FieldProperty(ISlotConfiguration['prefix'])
     suffix = FieldProperty(ISlotConfiguration['suffix'])
 
     def __init__(self, slot_name, **kwargs):
         self.slot_name = slot_name
         self._portlet_ids = PersistentList()
         self.xs_width = 12
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/template.py` & `pyams_portal-1.9.1/src/pyams_portal/template.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/tests/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/tests/test_utilsdocs.py` & `pyams_portal-1.9.1/src/pyams_portal/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/tests/test_utilsdocstrings.py` & `pyams_portal-1.9.1/src/pyams_portal/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/utils.py` & `pyams_portal-1.9.1/src/pyams_portal/utils.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/__init__.py` & `pyams_portal-1.9.1/src/pyams_portal/zmi/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,29 +10,33 @@
 # FOR A PARTICULAR PURPOSE.
 #
 
 """PyAMS_portal.zmi main module
 
 This module defines base ZMI components.
 """
+from _testbuffer import get_sizeof_void_p
 
 from fanstatic import Library, Resource
 from pyramid.renderers import render
 from zope.interface import Interface
 from zope.schema import getFields
-from zope.schema.interfaces import IBool
+from zope.schema.interfaces import IBool, IChoice
+from zope.schema.vocabulary import getVocabularyRegistry
 
 from pyams_i18n.schema import II18nField
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_portal.interfaces import IPortalTemplate, IPortalTemplateConfiguration, \
-    IPortletPreviewer, IPortletSettings
+    IPortletPreviewer, IPortletSettings, PREVIEW_MODE
 from pyams_portal.skin import PortletContentProvider
 from pyams_skin.interfaces import BOOTSTRAP_DEVICES_ICONS, BOOTSTRAP_SIZES
 from pyams_template.template import template_config
 from pyams_utils.adapter import adapter_config
+from pyams_utils.interfaces.text import IHTMLRenderer
+from pyams_utils.request import get_annotations
 from pyams_utils.text import text_to_html
 
 __docformat__ = 'restructuredtext'
 
 from pyams_portal import _  # pylint: disable=ungrouped-imports
 
 
@@ -86,29 +90,34 @@
             template = self.context
         else:
             template = self.settings.configuration.parent
         config = IPortalTemplateConfiguration(template)
         _slot_id, slot_name = config.get_portlet_slot(self.settings.configuration.portlet_id)
         return config.get_slot_configuration(slot_name)
 
+    def update(self):
+        """Set preview mode on previewer update"""
+        get_annotations(self.request)[PREVIEW_MODE] = True
+        super().update()
+
     def render(self, template_name=''):
         """Preview portlet content"""
         if self.settings.renderer == 'hidden':
             return render('templates/portlet-hidden.pt', {}, request=self.request)
         translate = self.request.localizer.translate
         renderer = self.settings.get_renderer()
         result = PREVIEW_PREFIX.format(
             label=translate(_("Renderer:")),
             renderer=translate(renderer.label if renderer is not None
                                else _("!! MISSING RENDERER !!")),
             visibility=' '.join(get_visibility_icons(self.settings, translate)))
         result += super().render(template_name)
         return result
 
-    def get_setting(self, source, name, renderer=None, visible=True, icon=None):  # pylint: disable=too-many-arguments
+    def get_setting(self, source, name, renderer=None, visible=True, icon=None, converter=None):  # pylint: disable=too-many-arguments
         """Setting value renderer"""
         localizer = self.request.localizer
         translate = localizer.translate
         field = getFields(self.portlet.settings_factory)[name]
         label = translate(field.title)
         value = field.bind(source).get(source)
         if value and II18nField.providedBy(field):
@@ -121,14 +130,30 @@
                 'icon': icon
             })
         if IBool.providedBy(field):
             return render('templates/setting-bool-preview.pt', {
                 'label': label,
                 'checked': bool(value)
             })
+        if IChoice.providedBy(field):
+            try:
+                source = field.source
+                if source is not None:
+                    value = translate(source.by_value.get(value).title)
+                elif field.vocabularyName is not None:
+                    source = getVocabularyRegistry().get(source, field.vocabularyName)
+                    value = translate(source.getTerm(value).token)
+            except AttributeError:
+                value = translate(_("(missing value: {})")).format(value)
+        if converter is not None:
+            converter = self.request.registry.queryMultiAdapter((source, value),
+                                                                IHTMLRenderer,
+                                                                name=converter)
+            if converter is not None:
+                value = converter.render()
         if renderer is not None:
             value = text_to_html(value, renderer, field=field, context=source)
         return render('templates/setting-preview.pt', {
             'label': label,
             'value': value,
             'visible': visible,
             'icon': icon
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/container.py` & `pyams_portal-1.9.1/src/pyams_portal/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/interfaces.py` & `pyams_portal-1.9.1/src/pyams_portal/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/layout.py` & `pyams_portal-1.9.1/src/pyams_portal/zmi/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from pyams_utils.interfaces.intids import IUniqueID
 from pyams_utils.registry import query_utility
 from pyams_utils.traversing import get_parent
 from pyams_viewlet.manager import viewletmanager_config
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminModalAddForm
 from pyams_zmi.interfaces import IAdminLayer, IInnerAdminView
-from pyams_zmi.interfaces.viewlet import IActionsViewletManager, IContentManagementMenu, \
+from pyams_zmi.interfaces.viewlet import IContextActionsDropdownMenu, IContentManagementMenu, \
     IContextAddingsViewletManager, IMenuHeader, IPropertiesMenu, ISiteManagementMenu
 from pyams_zmi.utils import get_object_label
 from pyams_zmi.zmi.viewlet.breadcrumb import AdminLayerBreadcrumbItem
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
 __docformat__ = 'restructuredtext'
 
@@ -282,15 +282,15 @@
 
 #
 # Convert local template to shared template
 #
 
 @viewlet_config(name='share-template.menu',
                 context=IPortalContext, layer=IAdminLayer, view=PortalTemplateLayoutView,
-                manager=IActionsViewletManager, weight=10,
+                manager=IContextActionsDropdownMenu, weight=10,
                 permission=MANAGE_TEMPLATE_PERMISSION)
 class LocalTemplateShareMenu(MenuItem):
     """Local template share menu"""
 
     def __new__(cls, context, request, view, manager):  # pylint: disable=unused-argument
         page = get_portal_page(context, page_name=view.page_name)
         if (page is None) or not page.use_local_template:
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/portlet.py` & `pyams_portal-1.9.1/src/pyams_portal/zmi/portlet.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
     def render(self, changes):
         """AJAX form renderer"""
         config = IPortletConfiguration(self.form.context)
         settings = config.settings
         previewer = self.request.registry.queryMultiAdapter(
             (self.context, self.request, self.form, settings), IPortletPreviewer)
         result = {
-            'status': 'success',
+            'status': 'success' if changes else 'info',
             'callbacks': [{
                 'callback': 'MyAMS.portal.template.editPortletCallback',
                 'options': {
                     'portlet_id': config.portlet_id,
                     'inherit_parent': config.inherit_parent
                 }
             }]
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/presentation.py` & `pyams_portal-1.9.1/src/pyams_portal/zmi/presentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 from pyams_form.ajax import ajax_form_config
 from pyams_form.field import Fields
 from pyams_form.interfaces.form import IDataExtractedEvent, IGroup, IInnerSubForm
 from pyams_form.subform import InnerEditForm
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_pagelet.pagelet import pagelet_config
 from pyams_portal.interfaces import IPortalContext, IPortalFooterContext, IPortalHeaderContext, \
-    IPortalPage, \
-    MANAGE_TEMPLATE_PERMISSION
+    IPortalPage, MANAGE_TEMPLATE_PERMISSION
 from pyams_portal.utils import get_portal_page
 from pyams_portal.zmi.interfaces import IPortalContextPresentationForm, \
     IPortalContextPresentationMenu, IPortalContextHeaderPresentationMenu, IPortalContextFooterPresentationMenu
 from pyams_portal.zmi.layout import PortalTemplateLayoutView
 from pyams_skin.interfaces.viewlet import IHelpViewletManager
 from pyams_skin.viewlet.help import AlertMessage
 from pyams_template.template import template_config
 from pyams_utils.adapter import adapter_config
 from pyams_utils.interfaces.data import IObjectData
+from pyams_utils.interfaces.form import NO_VALUE_STRING
 from pyams_viewlet.manager import viewletmanager_config
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_zmi.form import AdminEditForm, FormGroupChecker
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import ISiteManagementMenu
 from pyams_zmi.zmi.viewlet.menu import NavigationMenuItem
 
@@ -191,15 +191,15 @@
         template_mode = params.get('template_mode')
         if template_mode is None:
             form.widgets.errors += (Invalid(_("You must choose between using a shared template "
                                               "or a local template if you don't inherit from "
                                               "parent template!")),)
         elif template_mode == TEMPLATE_SHARED_MODE:
             template = params.get('{}{}shared_template'.format(form.prefix, form.widgets.prefix))
-            if (not template) or (template == '--NOVALUE--'):
+            if (not template) or (template == NO_VALUE_STRING):
                 form.widgets.errors += (Invalid(_("You must select a template when setting "
                                                   "shared template mode!")),)
 
 
 @adapter_config(name='presentation-override',
                 required=(IPortalContext, IAdminLayer, PortalContextPresentationEditForm),
                 provides=IGroup)
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/resources/css/layout.css` & `pyams_portal-1.9.1/src/pyams_portal/zmi/resources/css/layout.css`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/resources/css/layout.min.css` & `pyams_portal-1.9.1/src/pyams_portal/zmi/resources/css/layout.min.css`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/resources/js/layout.js` & `pyams_portal-1.9.1/src/pyams_portal/zmi/resources/js/layout.js`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/resources/js/layout.min.js` & `pyams_portal-1.9.1/src/pyams_portal/zmi/resources/js/layout.min.js`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/resources/sass/layout.scss` & `pyams_portal-1.9.1/src/pyams_portal/zmi/resources/sass/layout.scss`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/slot.py` & `pyams_portal-1.9.1/src/pyams_portal/zmi/slot.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,20 +207,18 @@
         return self.config.slot_config[slot_name]
 
     def update_widgets(self, prefix=None):
         super().update_widgets(prefix)
         slot_name = self.widgets.get('slot_name')
         if slot_name is not None:
             slot_name.mode = HIDDEN_MODE
-        css_class = self.widgets.get('container_css_class')
-        if css_class is not None:
-            css_class.input_css_class = 'col-sm-6'
-        css_class = self.widgets.get('css_class')
-        if css_class is not None:
-            css_class.input_css_class = 'col-sm-6'
+        for name in ('container_css_class', 'css_class', 'portlets_css_class'):
+            widget = self.widgets.get(name)
+            if widget is not None:
+                widget.input_css_class = 'col-sm-6'
 
 
 @adapter_config(name='html-codes',
                 required=(Interface, IAdminLayer, PortalTemplateSlotPropertiesEditForm),
                 provides=IGroup)
 class PortalTemplateSlotPropertiesHTMLCodes(FormGroupSwitcher):
     """Portal template slot properties HTML codes"""
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/template.py` & `pyams_portal-1.9.1/src/pyams_portal/zmi/template.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/templates/layout.pt` & `pyams_portal-1.9.1/src/pyams_portal/zmi/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/templates/portlet-preview.pt` & `pyams_portal-1.9.1/src/pyams_portal/zmi/templates/portlet-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/templates/presentation-template.pt` & `pyams_portal-1.9.1/src/pyams_portal/zmi/templates/presentation-template.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/templates/renderer-input.pt` & `pyams_portal-1.9.1/src/pyams_portal/zmi/templates/renderer-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal/zmi/widget.py` & `pyams_portal-1.9.1/src/pyams_portal/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_portal-1.8.1/src/pyams_portal.egg-info/PKG-INFO` & `pyams_portal-1.9.1/src/pyams_portal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-portal
-Version: 1.8.1
+Version: 1.9.1
 Summary: PyAMS portlets management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -53,14 +53,25 @@
 content management packages like PyAMS_content, while other extension packages can be used to
 provide custom portlets renderers.
 
 
 Changelog
 =========
 
+1.9.1
+-----
+ - updated doctests
+
+1.9.0
+-----
+ - added slot CSS class to portlets container
+ - updated portlet previewer
+ - updated portlet edit form status
+ - bypass workflow state check on page preview
+
 1.8.1
 -----
  - use new sortable table base class
 
 1.8.0
 -----
  - added marker interfaces to handle header and footer templates
```

### Comparing `pyams_portal-1.8.1/src/pyams_portal.egg-info/SOURCES.txt` & `pyams_portal-1.9.1/src/pyams_portal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

