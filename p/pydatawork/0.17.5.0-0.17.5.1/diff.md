# Comparing `tmp/pydatawork-0.17.5.0.tar.gz` & `tmp/pydatawork-0.17.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.5.0.tar", last modified: Sat Jul  8 14:12:05 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.5.1.tar", last modified: Sat Jul  8 14:16:56 2023, max compression
```

## Comparing `pydatawork-0.17.5.0.tar` & `pydatawork-0.17.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 14:12:05.000000 pydatawork-0.17.5.0/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    20895 2023-07-08 14:12:05.000000 pydatawork-0.17.5.0/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15912 2023-07-08 14:09:59.000000 pydatawork-0.17.5.0/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 14:12:05.000000 pydatawork-0.17.5.0/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    20895 2023-07-08 14:12:05.000000 pydatawork-0.17.5.0/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-08 14:12:05.000000 pydatawork-0.17.5.0/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-08 14:12:05.000000 pydatawork-0.17.5.0/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-08 14:12:05.000000 pydatawork-0.17.5.0/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    52080 2023-07-08 14:09:47.000000 pydatawork-0.17.5.0/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-08 14:12:05.000000 pydatawork-0.17.5.0/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-08 13:31:38.000000 pydatawork-0.17.5.0/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    20895 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15912 2023-07-08 14:16:32.000000 pydatawork-0.17.5.1/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    20895 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    52071 2023-07-08 14:16:21.000000 pydatawork-0.17.5.1/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-08 14:16:37.000000 pydatawork-0.17.5.1/setup.py
```

### Comparing `pydatawork-0.17.5.0/PKG-INFO` & `pydatawork-0.17.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.0
+Version: 0.17.5.1
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -44,22 +44,22 @@
         pip3 install requests
         ```
         
         
         
         # Basic Functions
         
-        ## rename_by_re() 通过正则表达式匹配实现文件名替换——先匹配指定部分，将其替换为指定关键词 （v 0.17.5.0）
+        ## rename_by_re() 通过正则表达式匹配实现文件重命名或批量重命名——先匹配，再用关键词替换匹配部分 （v 0.17.5.1）
         
         ###### Sat Jul 8 21:29:29 CST 2023
         
         ```python
         def rename_by_re(path: str, pattern: str, keyword: str):
             """
-            功能：按正则表达式匹配进行文件重命名或批量重命名。（先通关正则表达式匹配要替换的部分，再进行文件名关键词替换。）
+            功能：按正则表达式匹配进行文件重命名或批量重命名。（先通过正则表达式匹配要替换的部分，再进行关键词替换。）
         
             参数：
         
             path：一个路径，可以是文件路径或文件夹路径(文件夹中的子文件夹不处理)。
         
             pattern：正则表达式匹配模式。如pattern = "[\u4e00-\u9fa5]+"为匹配文件名中的全部中文。
```

### Comparing `pydatawork-0.17.5.0/README.md` & `pydatawork-0.17.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 pip3 install requests
 ```
 
 
 
 # Basic Functions
 
-## rename_by_re() 通过正则表达式匹配实现文件名替换——先匹配指定部分，将其替换为指定关键词 （v 0.17.5.0）
+## rename_by_re() 通过正则表达式匹配实现文件重命名或批量重命名——先匹配，再用关键词替换匹配部分 （v 0.17.5.1）
 
 ###### Sat Jul 8 21:29:29 CST 2023
 
 ```python
 def rename_by_re(path: str, pattern: str, keyword: str):
     """
-    功能：按正则表达式匹配进行文件重命名或批量重命名。（先通关正则表达式匹配要替换的部分，再进行文件名关键词替换。）
+    功能：按正则表达式匹配进行文件重命名或批量重命名。（先通过正则表达式匹配要替换的部分，再进行关键词替换。）
 
     参数：
 
     path：一个路径，可以是文件路径或文件夹路径(文件夹中的子文件夹不处理)。
 
     pattern：正则表达式匹配模式。如pattern = "[\u4e00-\u9fa5]+"为匹配文件名中的全部中文。
```

### Comparing `pydatawork-0.17.5.0/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.5.1/pydatawork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.0
+Version: 0.17.5.1
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -44,22 +44,22 @@
         pip3 install requests
         ```
         
         
         
         # Basic Functions
         
-        ## rename_by_re() 通过正则表达式匹配实现文件名替换——先匹配指定部分，将其替换为指定关键词 （v 0.17.5.0）
+        ## rename_by_re() 通过正则表达式匹配实现文件重命名或批量重命名——先匹配，再用关键词替换匹配部分 （v 0.17.5.1）
         
         ###### Sat Jul 8 21:29:29 CST 2023
         
         ```python
         def rename_by_re(path: str, pattern: str, keyword: str):
             """
-            功能：按正则表达式匹配进行文件重命名或批量重命名。（先通关正则表达式匹配要替换的部分，再进行文件名关键词替换。）
+            功能：按正则表达式匹配进行文件重命名或批量重命名。（先通过正则表达式匹配要替换的部分，再进行关键词替换。）
         
             参数：
         
             path：一个路径，可以是文件路径或文件夹路径(文件夹中的子文件夹不处理)。
         
             pattern：正则表达式匹配模式。如pattern = "[\u4e00-\u9fa5]+"为匹配文件名中的全部中文。
```

### Comparing `pydatawork-0.17.5.0/pydatawork.py` & `pydatawork-0.17.5.1/pydatawork.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
 # Basic Functions
 
 # 替换
 
 def rename_by_re(path: str, pattern: str, keyword: str):
     """
-    功能：按正则表达式匹配进行文件重命名或批量重命名。（先通关正则表达式匹配要替换的部分，再进行文件名关键词替换。）
+    功能：按正则表达式匹配进行文件重命名或批量重命名。（先通过正则表达式匹配要替换的部分，再进行关键词替换。）
 
     参数：
 
     path：一个路径，可以是文件路径或文件夹路径。
 
     pattern：正则表达式匹配模式。如pattern = "[\u4e00-\u9fa5]+"为匹配文件名中的全部中文。
```

### Comparing `pydatawork-0.17.5.0/setup.py` & `pydatawork-0.17.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.5.0',
+    version='0.17.5.1',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

