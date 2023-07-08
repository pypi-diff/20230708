# Comparing `tmp/password_lib-0.0.2.tar.gz` & `tmp/password_lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "password_lib-0.0.2.tar", last modified: Wed Jul  5 21:11:34 2023, max compression
+gzip compressed data, was "password_lib-0.0.3.tar", last modified: Sat Jul  8 11:04:35 2023, max compression
```

## Comparing `password_lib-0.0.2.tar` & `password_lib-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 21:11:34.125383 password_lib-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-05 18:49:19.000000 password_lib-0.0.2/License
--rw-rw-rw-   0        0        0     2212 2023-07-05 21:11:34.124383 password_lib-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1490 2023-07-05 21:11:27.000000 password_lib-0.0.2/README.md
--rw-rw-rw-   0        0        0      802 2023-07-05 21:10:45.000000 password_lib-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 21:11:34.126384 password_lib-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-05 21:11:34.091991 password_lib-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 21:11:34.105541 password_lib-0.0.2/src/password_lib/
--rw-rw-rw-   0        0        0        0 2023-07-05 19:01:39.000000 password_lib-0.0.2/src/password_lib/__init__.py
--rw-rw-rw-   0        0        0     3002 2023-07-05 19:39:39.000000 password_lib-0.0.2/src/password_lib/checker.py
-drwxrwxrwx   0        0        0        0 2023-07-05 21:11:34.122372 password_lib-0.0.2/src/password_lib.egg-info/
--rw-rw-rw-   0        0        0     2212 2023-07-05 21:11:34.000000 password_lib-0.0.2/src/password_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-05 21:11:34.000000 password_lib-0.0.2/src/password_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 21:11:34.000000 password_lib-0.0.2/src/password_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-05 21:11:34.000000 password_lib-0.0.2/src/password_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 11:04:35.611166 password_lib-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-05 18:49:19.000000 password_lib-0.0.3/License
+-rw-rw-rw-   0        0        0     2434 2023-07-08 11:04:35.610165 password_lib-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1644 2023-07-08 11:03:48.000000 password_lib-0.0.3/README.md
+-rw-rw-rw-   0        0        0      870 2023-07-08 11:01:00.000000 password_lib-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 11:04:35.612218 password_lib-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 11:04:35.580966 password_lib-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 11:04:35.597166 password_lib-0.0.3/src/password_lib/
+-rw-rw-rw-   0        0        0        0 2023-07-05 19:01:39.000000 password_lib-0.0.3/src/password_lib/__init__.py
+-rw-rw-rw-   0        0        0     7008 2023-07-08 10:29:07.000000 password_lib-0.0.3/src/password_lib/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:04:35.607166 password_lib-0.0.3/src/password_lib.egg-info/
+-rw-rw-rw-   0        0        0     2434 2023-07-08 11:04:35.000000 password_lib-0.0.3/src/password_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-08 11:04:35.000000 password_lib-0.0.3/src/password_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 11:04:35.000000 password_lib-0.0.3/src/password_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-08 11:04:35.000000 password_lib-0.0.3/src/password_lib.egg-info/top_level.txt
```

### Comparing `password_lib-0.0.2/License` & `password_lib-0.0.3/License`

 * *Files identical despite different names*

### Comparing `password_lib-0.0.2/pyproject.toml` & `password_lib-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'password_lib'
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ahamed Ruyefa", email="ruyefadf@gmail.com" },
 ]
-description = "The 'password_lib' is a Python package for strong password checking. It validates password strength based on length, lowercase/uppercase characters, special characters, and digits. Enhance your application's security with ease."
+description = " `password-lib` is a Python library for generating secure passwords, configuring strength requirements, and checking password strength. With customizable length and requirements, it enhances application security. Use password-lib to easily generate strong passwords and ensure password security."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

