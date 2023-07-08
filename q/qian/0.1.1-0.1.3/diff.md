# Comparing `tmp/qian-0.1.1.tar.gz` & `tmp/qian-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qian-0.1.1.tar", last modified: Fri Aug 27 17:15:16 2021, max compression
+gzip compressed data, was "qian-0.1.3.tar", last modified: Sat Jul  8 02:18:29 2023, max compression
```

## Comparing `qian-0.1.1.tar` & `qian-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2021-08-27 17:15:16.000000 qian-0.1.1/
--rw-r--r--   0 samsonqian   (501) staff       (20)      415 2021-08-27 17:15:16.000000 qian-0.1.1/PKG-INFO
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2021-08-27 17:15:16.000000 qian-0.1.1/qian.egg-info/
--rw-r--r--   0 samsonqian   (501) staff       (20)      415 2021-08-27 17:15:16.000000 qian-0.1.1/qian.egg-info/PKG-INFO
--rw-r--r--   0 samsonqian   (501) staff       (20)      165 2021-08-27 17:15:16.000000 qian-0.1.1/qian.egg-info/SOURCES.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)        5 2021-08-27 17:15:16.000000 qian-0.1.1/qian.egg-info/top_level.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)        1 2021-08-27 17:15:16.000000 qian-0.1.1/qian.egg-info/dependency_links.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)     1069 2021-08-27 16:12:11.000000 qian-0.1.1/LICENSE
--rw-r--r--   0 samsonqian   (501) staff       (20)        6 2021-08-27 16:12:11.000000 qian-0.1.1/README.md
--rw-r--r--   0 samsonqian   (501) staff       (20)     1383 2021-08-27 16:44:18.000000 qian-0.1.1/setup.py
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2021-08-27 17:15:16.000000 qian-0.1.1/qian/
--rw-r--r--   0 samsonqian   (501) staff       (20)        0 2021-08-27 16:14:59.000000 qian-0.1.1/qian/__init__.py
--rw-r--r--   0 samsonqian   (501) staff       (20)      141 2021-08-27 17:15:16.000000 qian-0.1.1/setup.cfg
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-08 02:18:29.246902 qian-0.1.3/
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1069 2021-08-27 16:12:11.000000 qian-0.1.3/LICENSE
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1402 2023-07-08 02:18:29.246981 qian-0.1.3/PKG-INFO
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1006 2023-07-08 02:06:30.000000 qian-0.1.3/README.md
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-08 02:18:29.246218 qian-0.1.3/qian/
+-rw-r--r--   0 samsonqian   (501) staff       (20)        0 2021-08-27 16:14:59.000000 qian-0.1.3/qian/__init__.py
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-08 02:18:29.246779 qian-0.1.3/qian.egg-info/
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1402 2023-07-08 02:18:29.000000 qian-0.1.3/qian.egg-info/PKG-INFO
+-rw-r--r--   0 samsonqian   (501) staff       (20)      165 2023-07-08 02:18:29.000000 qian-0.1.3/qian.egg-info/SOURCES.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)        1 2023-07-08 02:18:29.000000 qian-0.1.3/qian.egg-info/dependency_links.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)        5 2023-07-08 02:18:29.000000 qian-0.1.3/qian.egg-info/top_level.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)      141 2023-07-08 02:18:29.247263 qian-0.1.3/setup.cfg
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1390 2023-07-08 02:18:22.000000 qian-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qian-0.1.1/LICENSE` & `qian-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qian-0.1.1/setup.py` & `qian-0.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     install_reqs = _parse_requirements("requirements.txt")
 except Exception as e:
     logging.warning('Fail load requirements file, so using default ones.')
     install_reqs = []
 
 setup(
     name="qian",
-    version="0.1.1",
+    version="0.1.3",
     author="Samson Qian",
     author_email="samsonqian@gmail.com",
     packages=["qian"],
     url="https://github.com/qiancapital/qian",
     license="MIT",
-    description="Quantitative Value Investing methods package",
+    description="Quantitative Investment Algorithm Nexus",
     long_description=README,
     long_description_content_type="text/markdown",
     install_requires=install_reqs,
     python_requires=">=3.6",
-    keywords="quantitative-research value-investing business-analysis valuation cash-flow"
+    keywords="quantitative-research time-series value-investing business-analysis valuation cash-flow"
 )
```

