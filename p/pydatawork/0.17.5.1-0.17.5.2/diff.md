# Comparing `tmp/pydatawork-0.17.5.1.tar.gz` & `tmp/pydatawork-0.17.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.5.1.tar", last modified: Sat Jul  8 14:16:56 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.5.2.tar", last modified: Sat Jul  8 14:40:42 2023, max compression
```

## Comparing `pydatawork-0.17.5.1.tar` & `pydatawork-0.17.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    20895 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15912 2023-07-08 14:16:32.000000 pydatawork-0.17.5.1/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    20895 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    52071 2023-07-08 14:16:21.000000 pydatawork-0.17.5.1/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-08 14:16:56.000000 pydatawork-0.17.5.1/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-08 14:16:37.000000 pydatawork-0.17.5.1/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 14:40:42.000000 pydatawork-0.17.5.2/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    21454 2023-07-08 14:40:42.000000 pydatawork-0.17.5.2/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16327 2023-07-08 14:40:15.000000 pydatawork-0.17.5.2/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 14:40:42.000000 pydatawork-0.17.5.2/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    21454 2023-07-08 14:40:42.000000 pydatawork-0.17.5.2/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-08 14:40:42.000000 pydatawork-0.17.5.2/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-08 14:40:42.000000 pydatawork-0.17.5.2/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-08 14:40:42.000000 pydatawork-0.17.5.2/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    52070 2023-07-08 14:36:07.000000 pydatawork-0.17.5.2/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-08 14:40:42.000000 pydatawork-0.17.5.2/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-08 14:40:02.000000 pydatawork-0.17.5.2/setup.py
```

### Comparing `pydatawork-0.17.5.1/PKG-INFO` & `pydatawork-0.17.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.1
+Version: 0.17.5.2
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -44,15 +44,15 @@
         pip3 install requests
         ```
         
         
         
         # Basic Functions
         
-        ## rename_by_re() 通过正则表达式匹配实现文件重命名或批量重命名——先匹配，再用关键词替换匹配部分 （v 0.17.5.1）
+        ## rename_by_re() 通过正则表达式匹配实现文件重命名或批量重命名——先匹配，再用关键词替换匹配部分 （v 0.17.5.2）
         
         ###### Sat Jul 8 21:29:29 CST 2023
         
         ```python
         def rename_by_re(path: str, pattern: str, keyword: str):
             """
             功能：按正则表达式匹配进行文件重命名或批量重命名。（先通过正则表达式匹配要替换的部分，再进行关键词替换。）
@@ -63,14 +63,32 @@
         
             pattern：正则表达式匹配模式。如pattern = "[\u4e00-\u9fa5]+"为匹配文件名中的全部中文。
         
             keyword：用于替换的关键词。
             """
         ```
         
+        使用示例1：
+        ```python
+        import pydatawork as dw
+        
+        # 将 呼呼叫hhh-积极一回81871.jpg 中的中文替换成zzz。
+        
+        path = r"/home/jkzhou/Desktop/pydatawork/test_data/rename_by_re"
+        pattern = "[\u4e00-\u9fa5]+" # 匹配文件名中的全部中文字符
+        keyword = "zzz"
+        
+        dw.rename_by_re(path,pattern,keyword)
+        ```
+        
+        输出结果：
+        ```text
+        renaming: 呼呼叫hhh-积极一回81871.jpg to zzzhhh-zzz81871.jpg
+        ```
+        
         
         
         ## rename_by_insert_keyword() 在文件名的指定位置插入关键词（默认为当前时间戳），实现重命名或批量重命名 (v 0.17.4.4)
         
         ###### Fri Jul 7 16:06:42 CST 2023
         
         ```python
```

### Comparing `pydatawork-0.17.5.1/README.md` & `pydatawork-0.17.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 pip3 install requests
 ```
 
 
 
 # Basic Functions
 
-## rename_by_re() 通过正则表达式匹配实现文件重命名或批量重命名——先匹配，再用关键词替换匹配部分 （v 0.17.5.1）
+## rename_by_re() 通过正则表达式匹配实现文件重命名或批量重命名——先匹配，再用关键词替换匹配部分 （v 0.17.5.2）
 
 ###### Sat Jul 8 21:29:29 CST 2023
 
 ```python
 def rename_by_re(path: str, pattern: str, keyword: str):
     """
     功能：按正则表达式匹配进行文件重命名或批量重命名。（先通过正则表达式匹配要替换的部分，再进行关键词替换。）
@@ -55,14 +55,32 @@
 
     pattern：正则表达式匹配模式。如pattern = "[\u4e00-\u9fa5]+"为匹配文件名中的全部中文。
 
     keyword：用于替换的关键词。
     """
 ```
 
+使用示例1：
+```python
+import pydatawork as dw
+
+# 将 呼呼叫hhh-积极一回81871.jpg 中的中文替换成zzz。
+
+path = r"/home/jkzhou/Desktop/pydatawork/test_data/rename_by_re"
+pattern = "[\u4e00-\u9fa5]+" # 匹配文件名中的全部中文字符
+keyword = "zzz"
+
+dw.rename_by_re(path,pattern,keyword)
+```
+
+输出结果：
+```text
+renaming: 呼呼叫hhh-积极一回81871.jpg to zzzhhh-zzz81871.jpg
+```
+
 
 
 ## rename_by_insert_keyword() 在文件名的指定位置插入关键词（默认为当前时间戳），实现重命名或批量重命名 (v 0.17.4.4)
 
 ###### Fri Jul 7 16:06:42 CST 2023
 
 ```python
```

### Comparing `pydatawork-0.17.5.1/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.5.2/pydatawork.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.1
+Version: 0.17.5.2
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -44,15 +44,15 @@
         pip3 install requests
         ```
         
         
         
         # Basic Functions
         
-        ## rename_by_re() 通过正则表达式匹配实现文件重命名或批量重命名——先匹配，再用关键词替换匹配部分 （v 0.17.5.1）
+        ## rename_by_re() 通过正则表达式匹配实现文件重命名或批量重命名——先匹配，再用关键词替换匹配部分 （v 0.17.5.2）
         
         ###### Sat Jul 8 21:29:29 CST 2023
         
         ```python
         def rename_by_re(path: str, pattern: str, keyword: str):
             """
             功能：按正则表达式匹配进行文件重命名或批量重命名。（先通过正则表达式匹配要替换的部分，再进行关键词替换。）
@@ -63,14 +63,32 @@
         
             pattern：正则表达式匹配模式。如pattern = "[\u4e00-\u9fa5]+"为匹配文件名中的全部中文。
         
             keyword：用于替换的关键词。
             """
         ```
         
+        使用示例1：
+        ```python
+        import pydatawork as dw
+        
+        # 将 呼呼叫hhh-积极一回81871.jpg 中的中文替换成zzz。
+        
+        path = r"/home/jkzhou/Desktop/pydatawork/test_data/rename_by_re"
+        pattern = "[\u4e00-\u9fa5]+" # 匹配文件名中的全部中文字符
+        keyword = "zzz"
+        
+        dw.rename_by_re(path,pattern,keyword)
+        ```
+        
+        输出结果：
+        ```text
+        renaming: 呼呼叫hhh-积极一回81871.jpg to zzzhhh-zzz81871.jpg
+        ```
+        
         
         
         ## rename_by_insert_keyword() 在文件名的指定位置插入关键词（默认为当前时间戳），实现重命名或批量重命名 (v 0.17.4.4)
         
         ###### Fri Jul 7 16:06:42 CST 2023
         
         ```python
```

### Comparing `pydatawork-0.17.5.1/pydatawork.py` & `pydatawork-0.17.5.2/pydatawork.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,14 @@
 
 
 
 
 # Basic Functions
 
 # 替换
-
 def rename_by_re(path: str, pattern: str, keyword: str):
     """
     功能：按正则表达式匹配进行文件重命名或批量重命名。（先通过正则表达式匹配要替换的部分，再进行关键词替换。）
 
     参数：
 
     path：一个路径，可以是文件路径或文件夹路径。
```

### Comparing `pydatawork-0.17.5.1/setup.py` & `pydatawork-0.17.5.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.5.1',
+    version='0.17.5.2',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

