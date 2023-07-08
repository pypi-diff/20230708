# Comparing `tmp/KwoksTool-0.0.7.tar.gz` & `tmp/KwoksTool-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KwoksTool-0.0.7.tar", last modified: Thu Jul  6 02:54:32 2023, max compression
+gzip compressed data, was "KwoksTool-0.0.8.tar", last modified: Sat Jul  8 04:35:12 2023, max compression
```

## Comparing `KwoksTool-0.0.7.tar` & `KwoksTool-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 02:54:32.382503 KwoksTool-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-07-06 02:54:32.382503 KwoksTool-0.0.7/KwoksTool/
--rw-rw-rw-   0        0        0      877 2023-07-06 02:53:56.000000 KwoksTool-0.0.7/KwoksTool/__init__.py
--rw-rw-rw-   0        0        0       22 2023-07-06 02:52:45.000000 KwoksTool-0.0.7/KwoksTool/_version.py
--rw-rw-rw-   0        0        0    14458 2023-07-05 23:46:50.000000 KwoksTool-0.0.7/KwoksTool/function.py
--rw-rw-rw-   0        0        0      122 2023-07-05 23:46:50.000000 KwoksTool-0.0.7/KwoksTool/info.py
--rw-rw-rw-   0        0        0     1095 2023-07-05 23:46:50.000000 KwoksTool-0.0.7/KwoksTool/model.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:54:32.382503 KwoksTool-0.0.7/KwoksTool/source/
--rw-rw-rw-   0        0        0   199365 2023-07-05 23:46:50.000000 KwoksTool-0.0.7/KwoksTool/source/IpPool.py
--rw-rw-rw-   0        0        0     3737 2023-07-05 23:46:50.000000 KwoksTool-0.0.7/KwoksTool/spider.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:54:32.382503 KwoksTool-0.0.7/KwoksTool.egg-info/
--rw-rw-rw-   0        0        0       56 2023-07-06 02:54:32.000000 KwoksTool-0.0.7/KwoksTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-07-06 02:54:32.000000 KwoksTool-0.0.7/KwoksTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 02:54:32.000000 KwoksTool-0.0.7/KwoksTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-06 02:54:32.000000 KwoksTool-0.0.7/KwoksTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 02:54:32.000000 KwoksTool-0.0.7/KwoksTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-06 02:54:32.382503 KwoksTool-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-07-06 02:54:08.000000 KwoksTool-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 02:54:32.382503 KwoksTool-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-07-08 04:35:12.504403 KwoksTool-0.0.8/KwoksTool/
+drwxrwxrwx   0        0        0        0 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/KwoksTool/Spider/
+-rw-rw-rw-   0        0        0    12009 2023-07-08 04:30:16.000000 KwoksTool-0.0.8/KwoksTool/Spider/stock.py
+-rw-rw-rw-   0        0        0      927 2023-07-08 03:12:19.000000 KwoksTool-0.0.8/KwoksTool/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-07-08 04:34:53.000000 KwoksTool-0.0.8/KwoksTool/_version.py
+-rw-rw-rw-   0        0        0    14458 2023-07-08 01:44:22.000000 KwoksTool-0.0.8/KwoksTool/function.py
+-rw-rw-rw-   0        0        0      122 2023-07-08 01:44:22.000000 KwoksTool-0.0.8/KwoksTool/info.py
+-rw-rw-rw-   0        0        0     1095 2023-07-08 01:44:22.000000 KwoksTool-0.0.8/KwoksTool/model.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/KwoksTool/source/
+-rw-rw-rw-   0        0        0   199365 2023-07-08 01:44:22.000000 KwoksTool-0.0.8/KwoksTool/source/IpPool.py
+-rw-rw-rw-   0        0        0     3737 2023-07-08 01:44:22.000000 KwoksTool-0.0.8/KwoksTool/spider.py
+drwxrwxrwx   0        0        0        0 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/KwoksTool.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-07-08 04:35:12.000000 KwoksTool-0.0.8/KwoksTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-07-08 04:35:12.000000 KwoksTool-0.0.8/KwoksTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 04:35:12.000000 KwoksTool-0.0.8/KwoksTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-08 04:35:12.000000 KwoksTool-0.0.8/KwoksTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 04:35:12.000000 KwoksTool-0.0.8/KwoksTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-07-08 04:34:48.000000 KwoksTool-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/setup.cfg
```

### Comparing `KwoksTool-0.0.7/KwoksTool/__init__.py` & `KwoksTool-0.0.8/KwoksTool/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from KwoksTool.info import (welcome,how)
 from KwoksTool.spider import (Browser,PlateComponentStocks)
+from KwoksTool.Spider.stock import GetStocksData
 from KwoksTool.function import (GetCityNumFromLiepin,
                                 GetCityNumFromBossZhiPing,
                                 GetCityNameFromLiepin,
                                 YesOrNot,
                                 CheckIp,
                                 IntoZip,
                                 ZipOut,
```

### Comparing `KwoksTool-0.0.7/KwoksTool/function.py` & `KwoksTool-0.0.8/KwoksTool/function.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.7/KwoksTool/model.py` & `KwoksTool-0.0.8/KwoksTool/model.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.7/KwoksTool/source/IpPool.py` & `KwoksTool-0.0.8/KwoksTool/source/IpPool.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.7/KwoksTool/spider.py` & `KwoksTool-0.0.8/KwoksTool/spider.py`

 * *Files identical despite different names*

