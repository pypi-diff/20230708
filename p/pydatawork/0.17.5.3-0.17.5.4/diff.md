# Comparing `tmp/pydatawork-0.17.5.3.tar.gz` & `tmp/pydatawork-0.17.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.5.3.tar", last modified: Sat Jul  8 15:00:23 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.5.4.tar", last modified: Sat Jul  8 15:04:29 2023, max compression
```

## Comparing `pydatawork-0.17.5.3.tar` & `pydatawork-0.17.5.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 15:00:23.000000 pydatawork-0.17.5.3/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22260 2023-07-08 15:00:23.000000 pydatawork-0.17.5.3/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16981 2023-07-08 14:59:30.000000 pydatawork-0.17.5.3/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 15:00:23.000000 pydatawork-0.17.5.3/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22260 2023-07-08 15:00:23.000000 pydatawork-0.17.5.3/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-08 15:00:23.000000 pydatawork-0.17.5.3/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-08 15:00:23.000000 pydatawork-0.17.5.3/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-08 15:00:23.000000 pydatawork-0.17.5.3/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    52263 2023-07-08 14:59:48.000000 pydatawork-0.17.5.3/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-08 15:00:23.000000 pydatawork-0.17.5.3/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-08 14:56:34.000000 pydatawork-0.17.5.3/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16977 2023-07-08 15:03:51.000000 pydatawork-0.17.5.4/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    52293 2023-07-08 15:02:17.000000 pydatawork-0.17.5.4/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-08 15:04:22.000000 pydatawork-0.17.5.4/setup.py
```

### Comparing `pydatawork-0.17.5.3/PKG-INFO` & `pydatawork-0.17.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.3
+Version: 0.17.5.4
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -68,16 +68,14 @@
         ```
         
         使用示例1：匹配某一类全部字符串。（将 呼呼hhh-积极一回81871.jpg 中的中文替换成zzz。）
         
         ```python
         import pydatawork as dw
         
-        # 
-        
         path = r"/home/jkzhou/Desktop/pydatawork/test_data/rename_by_re"
         pattern = "[\u4e00-\u9fa5]+" # 匹配文件名中的全部中文字符
         keyword = "zzz"
         
         dw.rename_by_re(path,pattern,keyword)
         ```
```

### Comparing `pydatawork-0.17.5.3/README.md` & `pydatawork-0.17.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,14 @@
 ```
 
 使用示例1：匹配某一类全部字符串。（将 呼呼hhh-积极一回81871.jpg 中的中文替换成zzz。）
 
 ```python
 import pydatawork as dw
 
-# 
-
 path = r"/home/jkzhou/Desktop/pydatawork/test_data/rename_by_re"
 pattern = "[\u4e00-\u9fa5]+" # 匹配文件名中的全部中文字符
 keyword = "zzz"
 
 dw.rename_by_re(path,pattern,keyword)
 ```
```

### Comparing `pydatawork-0.17.5.3/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.5.4/pydatawork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.3
+Version: 0.17.5.4
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -68,16 +68,14 @@
         ```
         
         使用示例1：匹配某一类全部字符串。（将 呼呼hhh-积极一回81871.jpg 中的中文替换成zzz。）
         
         ```python
         import pydatawork as dw
         
-        # 
-        
         path = r"/home/jkzhou/Desktop/pydatawork/test_data/rename_by_re"
         pattern = "[\u4e00-\u9fa5]+" # 匹配文件名中的全部中文字符
         keyword = "zzz"
         
         dw.rename_by_re(path,pattern,keyword)
         ```
```

### Comparing `pydatawork-0.17.5.3/pydatawork.py` & `pydatawork-0.17.5.4/pydatawork.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
 
 
 
 
 # Basic Functions
 
-# 替换重命名，正则
+# 重命名，正则，关键词替换，批量重命名
 def rename_by_re(path: str, pattern: str, keyword: str):
     """
     功能：按正则表达式匹配进行文件重命名或批量重命名。（先通过正则表达式匹配要替换的部分，再进行关键词替换。注意：pattern参数也可当普通参数使用，用于匹配一个具体的词。））
 
     参数：
 
     path：一个路径，可以是文件路径或文件夹路径。
```

### Comparing `pydatawork-0.17.5.3/setup.py` & `pydatawork-0.17.5.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.5.3',
+    version='0.17.5.4',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

