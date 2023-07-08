# Comparing `tmp/telepycrypto-1.0.0.tar.gz` & `tmp/telepycrypto-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\telepycrypto-1.0.0.tar", last modified: Sat Jul  8 15:53:18 2023, max compression
+gzip compressed data, was "dist\telepycrypto-1.0.1.tar", last modified: Sat Jul  8 15:57:56 2023, max compression
```

## Comparing `telepycrypto-1.0.0.tar` & `telepycrypto-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 15:53:18.252929 telepycrypto-1.0.0/
--rw-rw-rw-   0        0        0       22 2023-07-08 15:53:17.000000 telepycrypto-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      379 2023-07-08 15:53:18.252929 telepycrypto-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-08 15:53:18.258789 telepycrypto-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      369 2023-07-08 15:53:17.000000 telepycrypto-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:53:18.232421 telepycrypto-1.0.0/telepycrypto/
--rw-rw-rw-   0        0        0       23 2023-07-08 15:43:26.000000 telepycrypto-1.0.0/telepycrypto/__init__.py
--rw-rw-rw-   0        0        0     5372 2023-07-08 15:43:44.000000 telepycrypto-1.0.0/telepycrypto/api.py
--rw-rw-rw-   0        0        0      300 2023-07-08 09:06:03.000000 telepycrypto-1.0.0/telepycrypto/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:53:18.250976 telepycrypto-1.0.0/telepycrypto.egg-info/
--rw-rw-rw-   0        0        0      379 2023-07-08 15:53:18.000000 telepycrypto-1.0.0/telepycrypto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-08 15:53:18.000000 telepycrypto-1.0.0/telepycrypto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 15:53:18.000000 telepycrypto-1.0.0/telepycrypto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-08 15:53:18.000000 telepycrypto-1.0.0/telepycrypto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 15:57:56.899414 telepycrypto-1.0.1/
+-rw-rw-rw-   0        0        0       22 2023-07-08 15:57:55.000000 telepycrypto-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      379 2023-07-08 15:57:56.899414 telepycrypto-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 15:57:56.908203 telepycrypto-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      369 2023-07-08 15:57:55.000000 telepycrypto-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:57:56.885742 telepycrypto-1.0.1/telepycrypto/
+drwxrwxrwx   0        0        0        0 2023-07-08 15:57:56.898437 telepycrypto-1.0.1/telepycrypto/Types/
+-rw-rw-rw-   0        0        0       28 2023-07-08 14:15:39.000000 telepycrypto-1.0.1/telepycrypto/Types/__init__.py
+-rw-rw-rw-   0        0        0      402 2023-07-08 15:46:06.000000 telepycrypto-1.0.1/telepycrypto/Types/invoice.py
+-rw-rw-rw-   0        0        0       23 2023-07-08 15:43:26.000000 telepycrypto-1.0.1/telepycrypto/__init__.py
+-rw-rw-rw-   0        0        0     5372 2023-07-08 15:43:44.000000 telepycrypto-1.0.1/telepycrypto/api.py
+-rw-rw-rw-   0        0        0      300 2023-07-08 09:06:03.000000 telepycrypto-1.0.1/telepycrypto/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:57:56.893554 telepycrypto-1.0.1/telepycrypto.egg-info/
+-rw-rw-rw-   0        0        0      379 2023-07-08 15:57:56.000000 telepycrypto-1.0.1/telepycrypto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-07-08 15:57:56.000000 telepycrypto-1.0.1/telepycrypto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 15:57:56.000000 telepycrypto-1.0.1/telepycrypto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-08 15:57:56.000000 telepycrypto-1.0.1/telepycrypto.egg-info/top_level.txt
```

### Comparing `telepycrypto-1.0.0/telepycrypto/api.py` & `telepycrypto-1.0.1/telepycrypto/api.py`

 * *Files identical despite different names*

