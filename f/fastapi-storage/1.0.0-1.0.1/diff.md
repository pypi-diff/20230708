# Comparing `tmp/fastapi-storage-1.0.0.tar.gz` & `tmp/fastapi-storage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-storage-1.0.0.tar", last modified: Fri Jul  7 12:48:58 2023, max compression
+gzip compressed data, was "fastapi-storage-1.0.1.tar", last modified: Sat Jul  8 03:02:57 2023, max compression
```

## Comparing `fastapi-storage-1.0.0.tar` & `fastapi-storage-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,36 @@
-drwxr-xr-x   0 xjaqil     (501) staff       (20)        0 2023-07-07 12:48:58.437696 fastapi-storage-1.0.0/
--rw-r--r--   0 xjaqil     (501) staff       (20)        0 2023-07-07 12:38:12.000000 fastapi-storage-1.0.0/LICENSE
--rw-r--r--   0 xjaqil     (501) staff       (20)      697 2023-07-07 12:48:58.437465 fastapi-storage-1.0.0/PKG-INFO
--rw-r--r--   0 xjaqil     (501) staff       (20)      139 2023-07-07 12:39:46.000000 fastapi-storage-1.0.0/README.rst
-drwxr-xr-x   0 xjaqil     (501) staff       (20)        0 2023-07-07 12:48:58.436502 fastapi-storage-1.0.0/fastapi_storage.egg-info/
--rw-r--r--   0 xjaqil     (501) staff       (20)      697 2023-07-07 12:48:58.000000 fastapi-storage-1.0.0/fastapi_storage.egg-info/PKG-INFO
--rw-r--r--   0 xjaqil     (501) staff       (20)      225 2023-07-07 12:48:58.000000 fastapi-storage-1.0.0/fastapi_storage.egg-info/SOURCES.txt
--rw-r--r--   0 xjaqil     (501) staff       (20)        1 2023-07-07 12:48:58.000000 fastapi-storage-1.0.0/fastapi_storage.egg-info/dependency_links.txt
--rw-r--r--   0 xjaqil     (501) staff       (20)       11 2023-07-07 12:48:58.000000 fastapi-storage-1.0.0/fastapi_storage.egg-info/top_level.txt
-drwxr-xr-x   0 xjaqil     (501) staff       (20)        0 2023-07-07 12:48:58.437091 fastapi-storage-1.0.0/filesystem/
--rw-r--r--   0 xjaqil     (501) staff       (20)        0 2023-07-07 12:44:33.000000 fastapi-storage-1.0.0/filesystem/__init__.py
--rw-r--r--   0 xjaqil     (501) staff       (20)      519 2023-07-07 12:38:04.000000 fastapi-storage-1.0.0/filesystem/main.py
--rw-r--r--   0 xjaqil     (501) staff       (20)       38 2023-07-07 12:48:58.437839 fastapi-storage-1.0.0/setup.cfg
--rw-r--r--   0 xjaqil     (501) staff       (20)      882 2023-07-07 12:42:06.000000 fastapi-storage-1.0.0/setup.py
+drwxr-xr-x   0 xjaqil     (501) staff       (20)        0 2023-07-08 03:02:57.362307 fastapi-storage-1.0.1/
+-rw-r--r--   0 xjaqil     (501) staff       (20)        0 2023-07-07 12:38:12.000000 fastapi-storage-1.0.1/LICENSE
+-rw-r--r--   0 xjaqil     (501) staff       (20)      788 2023-07-08 03:02:57.362465 fastapi-storage-1.0.1/PKG-INFO
+-rw-r--r--   0 xjaqil     (501) staff       (20)      139 2023-07-07 12:39:46.000000 fastapi-storage-1.0.1/README.rst
+drwxr-xr-x   0 xjaqil     (501) staff       (20)        0 2023-07-08 03:02:57.315532 fastapi-storage-1.0.1/config/
+-rw-r--r--   0 xjaqil     (501) staff       (20)        0 2023-07-07 13:27:02.000000 fastapi-storage-1.0.1/config/__init__.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)     1362 2023-07-07 13:32:12.000000 fastapi-storage-1.0.1/config/filesystems.py
+drwxr-xr-x   0 xjaqil     (501) staff       (20)        0 2023-07-08 03:02:57.315889 fastapi-storage-1.0.1/contracts/
+-rw-r--r--   0 xjaqil     (501) staff       (20)        0 2022-10-09 15:32:28.000000 fastapi-storage-1.0.1/contracts/__init__.py
+drwxr-xr-x   0 xjaqil     (501) staff       (20)        0 2023-07-08 03:02:57.317273 fastapi-storage-1.0.1/contracts/filesystem/
+-rw-r--r--   0 xjaqil     (501) staff       (20)       46 2022-10-09 19:00:26.000000 fastapi-storage-1.0.1/contracts/filesystem/__init__.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)      171 2023-07-07 13:24:36.000000 fastapi-storage-1.0.1/contracts/filesystem/cloud.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)      112 2022-10-09 17:51:19.000000 fastapi-storage-1.0.1/contracts/filesystem/factory.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)     1311 2022-10-10 23:03:59.000000 fastapi-storage-1.0.1/contracts/filesystem/filesystem.py
+drwxr-xr-x   0 xjaqil     (501) staff       (20)        0 2023-07-08 03:02:57.317921 fastapi-storage-1.0.1/core/
+-rw-r--r--   0 xjaqil     (501) staff       (20)        0 2023-07-07 13:28:38.000000 fastapi-storage-1.0.1/core/__init__.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)      251 2023-07-07 13:29:56.000000 fastapi-storage-1.0.1/core/settings.py
+drwxr-xr-x   0 xjaqil     (501) staff       (20)        0 2023-07-08 03:02:57.357489 fastapi-storage-1.0.1/fastapi_storage.egg-info/
+-rw-r--r--   0 xjaqil     (501) staff       (20)      788 2023-07-08 03:02:57.000000 fastapi-storage-1.0.1/fastapi_storage.egg-info/PKG-INFO
+-rw-r--r--   0 xjaqil     (501) staff       (20)      740 2023-07-08 03:02:57.000000 fastapi-storage-1.0.1/fastapi_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 xjaqil     (501) staff       (20)        1 2023-07-08 03:02:57.000000 fastapi-storage-1.0.1/fastapi_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 xjaqil     (501) staff       (20)       58 2023-07-08 03:02:57.000000 fastapi-storage-1.0.1/fastapi_storage.egg-info/entry_points.txt
+-rw-r--r--   0 xjaqil     (501) staff       (20)      102 2023-07-08 03:02:57.000000 fastapi-storage-1.0.1/fastapi_storage.egg-info/requires.txt
+-rw-r--r--   0 xjaqil     (501) staff       (20)       33 2023-07-08 03:02:57.000000 fastapi-storage-1.0.1/fastapi_storage.egg-info/top_level.txt
+-rw-r--r--   0 xjaqil     (501) staff       (20)        1 2023-07-08 03:01:30.000000 fastapi-storage-1.0.1/fastapi_storage.egg-info/zip-safe
+drwxr-xr-x   0 xjaqil     (501) staff       (20)        0 2023-07-08 03:02:57.362009 fastapi-storage-1.0.1/filesystem/
+-rw-r--r--   0 xjaqil     (501) staff       (20)      134 2023-07-07 13:05:39.000000 fastapi-storage-1.0.1/filesystem/__init__.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)      106 2022-10-09 16:47:15.000000 fastapi-storage-1.0.1/filesystem/filesystem.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)     4137 2023-07-07 13:05:39.000000 fastapi-storage-1.0.1/filesystem/filesystem_adapter.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)     2339 2023-07-07 13:27:12.000000 fastapi-storage-1.0.1/filesystem/filesystem_manager.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)      379 2023-07-08 02:57:03.000000 fastapi-storage-1.0.1/filesystem/main.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)     1063 2023-07-07 13:05:39.000000 fastapi-storage-1.0.1/filesystem/obs_adapter.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)     1919 2023-07-07 13:15:25.000000 fastapi-storage-1.0.1/filesystem/oss_adapter.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)     1743 2023-07-07 13:21:00.000000 fastapi-storage-1.0.1/filesystem/upload.py
+-rw-r--r--   0 xjaqil     (501) staff       (20)      834 2023-07-08 03:02:57.363229 fastapi-storage-1.0.1/setup.cfg
+-rw-r--r--   0 xjaqil     (501) staff       (20)      710 2023-07-08 02:58:18.000000 fastapi-storage-1.0.1/setup.py
```

