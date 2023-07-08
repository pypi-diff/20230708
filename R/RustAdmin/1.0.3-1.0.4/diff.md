# Comparing `tmp/rustadmin-1.0.3.tar.gz` & `tmp/RustAdmin-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustadmin-1.0.3.tar", last modified: Thu Jul  6 20:05:29 2023, max compression
+gzip compressed data, was "RustAdmin-1.0.4.tar", last modified: Sat Jul  8 20:07:49 2023, max compression
```

## Comparing `rustadmin-1.0.3.tar` & `RustAdmin-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 20:05:29.900745 rustadmin-1.0.3/
--rw-rw-rw-   0        0        0      168 2023-07-06 20:05:29.898743 rustadmin-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 20:05:29.857741 rustadmin-1.0.3/RustAdmin/
--rw-rw-rw-   0        0        0        0 2023-07-02 13:22:37.000000 rustadmin-1.0.3/RustAdmin/__init__.py
--rw-rw-rw-   0        0        0    17208 2023-07-06 19:50:47.000000 rustadmin-1.0.3/RustAdmin/create.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:05:29.894743 rustadmin-1.0.3/rustadmin.egg-info/
--rw-rw-rw-   0        0        0      168 2023-07-06 20:05:29.000000 rustadmin-1.0.3/rustadmin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-07-06 20:05:29.000000 rustadmin-1.0.3/rustadmin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 20:05:29.000000 rustadmin-1.0.3/rustadmin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-06 20:05:29.000000 rustadmin-1.0.3/rustadmin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 20:05:29.000000 rustadmin-1.0.3/rustadmin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-06 20:05:29.000000 rustadmin-1.0.3/rustadmin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 20:05:29.903745 rustadmin-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      473 2023-07-06 20:03:54.000000 rustadmin-1.0.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:07:49.789938 RustAdmin-1.0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-07-08 20:07:49.789938 RustAdmin-1.0.4/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 20:07:49.789938 RustAdmin-1.0.4/RustAdmin.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-07-08 20:07:49.000000 RustAdmin-1.0.4/RustAdmin.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-07-08 20:07:49.000000 RustAdmin-1.0.4/RustAdmin.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-08 20:07:49.000000 RustAdmin-1.0.4/RustAdmin.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-07-08 20:07:49.000000 RustAdmin-1.0.4/RustAdmin.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-08 20:07:49.000000 RustAdmin-1.0.4/RustAdmin.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-08 20:07:49.789938 RustAdmin-1.0.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-07-08 20:07:25.000000 RustAdmin-1.0.4/setup.py
```

