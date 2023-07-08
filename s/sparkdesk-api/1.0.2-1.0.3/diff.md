# Comparing `tmp/sparkdesk-api-1.0.2.tar.gz` & `tmp/sparkdesk-api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkdesk-api-1.0.2.tar", last modified: Sat Jul  8 08:37:19 2023, max compression
+gzip compressed data, was "sparkdesk-api-1.0.3.tar", last modified: Sat Jul  8 08:39:53 2023, max compression
```

## Comparing `sparkdesk-api-1.0.2.tar` & `sparkdesk-api-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 08:37:19.969827 sparkdesk-api-1.0.2/
--rw-rw-rw-   0        0        0    35823 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1646 2023-07-08 08:37:19.969827 sparkdesk-api-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1178 2023-07-08 08:34:53.000000 sparkdesk-api-1.0.2/README.md
--rw-rw-rw-   0        0        0      111 2023-07-08 08:37:19.971827 sparkdesk-api-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      734 2023-07-08 08:37:17.000000 sparkdesk-api-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:37:19.950823 sparkdesk-api-1.0.2/sparkdesk_api/
--rw-rw-rw-   0        0        0      198 2023-07-08 08:19:56.000000 sparkdesk-api-1.0.2/sparkdesk_api/__init__.py
--rw-rw-rw-   0        0        0     6736 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.2/sparkdesk_api/core.py
--rw-rw-rw-   0        0        0     1786 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.2/sparkdesk_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:37:19.959826 sparkdesk-api-1.0.2/sparkdesk_api.egg-info/
--rw-rw-rw-   0        0        0     1646 2023-07-08 08:37:19.000000 sparkdesk-api-1.0.2/sparkdesk_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-07-08 08:37:19.000000 sparkdesk-api-1.0.2/sparkdesk_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 08:37:19.000000 sparkdesk-api-1.0.2/sparkdesk_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-08 08:37:19.000000 sparkdesk-api-1.0.2/sparkdesk_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 08:37:19.967826 sparkdesk-api-1.0.2/sparkdesk_web/
--rw-rw-rw-   0        0        0      198 2023-07-08 08:19:56.000000 sparkdesk-api-1.0.2/sparkdesk_web/__init__.py
--rw-rw-rw-   0        0        0     4580 2023-07-08 08:15:21.000000 sparkdesk-api-1.0.2/sparkdesk_web/core.py
--rw-rw-rw-   0        0        0      880 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.2/sparkdesk_web/utils.py
--rw-rw-rw-   0        0        0     1910 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.2/sparkdesk_web/web.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:39:53.146206 sparkdesk-api-1.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1646 2023-07-08 08:39:53.146206 sparkdesk-api-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1178 2023-07-08 08:38:52.000000 sparkdesk-api-1.0.3/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-08 08:39:53.147212 sparkdesk-api-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-07-08 08:39:34.000000 sparkdesk-api-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:39:53.126196 sparkdesk-api-1.0.3/sparkdesk_api/
+-rw-rw-rw-   0        0        0      198 2023-07-08 08:19:56.000000 sparkdesk-api-1.0.3/sparkdesk_api/__init__.py
+-rw-rw-rw-   0        0        0     6736 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.3/sparkdesk_api/core.py
+-rw-rw-rw-   0        0        0     1786 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.3/sparkdesk_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:39:53.135190 sparkdesk-api-1.0.3/sparkdesk_api.egg-info/
+-rw-rw-rw-   0        0        0     1646 2023-07-08 08:39:52.000000 sparkdesk-api-1.0.3/sparkdesk_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-07-08 08:39:53.000000 sparkdesk-api-1.0.3/sparkdesk_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 08:39:52.000000 sparkdesk-api-1.0.3/sparkdesk_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-08 08:39:52.000000 sparkdesk-api-1.0.3/sparkdesk_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 08:39:53.144206 sparkdesk-api-1.0.3/sparkdesk_web/
+-rw-rw-rw-   0        0        0      198 2023-07-08 08:19:56.000000 sparkdesk-api-1.0.3/sparkdesk_web/__init__.py
+-rw-rw-rw-   0        0        0     4580 2023-07-08 08:15:21.000000 sparkdesk-api-1.0.3/sparkdesk_web/core.py
+-rw-rw-rw-   0        0        0      880 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.3/sparkdesk_web/utils.py
+-rw-rw-rw-   0        0        0     1910 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.3/sparkdesk_web/web.py
```

### Comparing `sparkdesk-api-1.0.2/LICENSE` & `sparkdesk-api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkdesk-api-1.0.2/PKG-INFO` & `sparkdesk-api-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkdesk-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: sparkdesk-api 讯飞星火大模型api
 Home-page: https://github.com/HildaM/sparkdesk-api
 Author: HildaM
 Author-email: Hilda_quan@163.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sparkdesk-api 讯飞星火大模型api
 > 如果该项目对你有帮助，不要忘记给我点个 star 哦！
 ## 使用方法
 ```shell
-pip install sparkdesk-api==1.0.1
+pip install sparkdesk-api==1.0.3
 ```
 
 ### 1. Web模式
 Web模式下，需要前往讯飞星火大模型web端通过 F12 抓取 3 个参数：cookie、fd、GtToken
 - [获取参数的方法](https://github.com/HildaM/sparkdesk-api/tree/main/docs)
 
 #### 命令行操作
```

### Comparing `sparkdesk-api-1.0.2/README.md` & `sparkdesk-api-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # sparkdesk-api 讯飞星火大模型api
 > 如果该项目对你有帮助，不要忘记给我点个 star 哦！
 ## 使用方法
 ```shell
-pip install sparkdesk-api==1.0.1
+pip install sparkdesk-api==1.0.3
 ```
 
 ### 1. Web模式
 Web模式下，需要前往讯飞星火大模型web端通过 F12 抓取 3 个参数：cookie、fd、GtToken
 - [获取参数的方法](https://github.com/HildaM/sparkdesk-api/tree/main/docs)
 
 #### 命令行操作
```

### Comparing `sparkdesk-api-1.0.2/setup.py` & `sparkdesk-api-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
       long_description = fh.read()
 
 setuptools.setup(
       name="sparkdesk-api",
-      version="1.0.2",
+      version="1.0.3",
       author="HildaM",
       author_email="Hilda_quan@163.com",
       description="sparkdesk-api 讯飞星火大模型api",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/HildaM/sparkdesk-api",
       license='GNU General Public License v3.0',
```

### Comparing `sparkdesk-api-1.0.2/sparkdesk_api/core.py` & `sparkdesk-api-1.0.3/sparkdesk_api/core.py`

 * *Files identical despite different names*

### Comparing `sparkdesk-api-1.0.2/sparkdesk_api/utils.py` & `sparkdesk-api-1.0.3/sparkdesk_api/utils.py`

 * *Files identical despite different names*

### Comparing `sparkdesk-api-1.0.2/sparkdesk_api.egg-info/PKG-INFO` & `sparkdesk-api-1.0.3/sparkdesk_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkdesk-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: sparkdesk-api 讯飞星火大模型api
 Home-page: https://github.com/HildaM/sparkdesk-api
 Author: HildaM
 Author-email: Hilda_quan@163.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sparkdesk-api 讯飞星火大模型api
 > 如果该项目对你有帮助，不要忘记给我点个 star 哦！
 ## 使用方法
 ```shell
-pip install sparkdesk-api==1.0.1
+pip install sparkdesk-api==1.0.3
 ```
 
 ### 1. Web模式
 Web模式下，需要前往讯飞星火大模型web端通过 F12 抓取 3 个参数：cookie、fd、GtToken
 - [获取参数的方法](https://github.com/HildaM/sparkdesk-api/tree/main/docs)
 
 #### 命令行操作
```

### Comparing `sparkdesk-api-1.0.2/sparkdesk_web/core.py` & `sparkdesk-api-1.0.3/sparkdesk_web/core.py`

 * *Files identical despite different names*

### Comparing `sparkdesk-api-1.0.2/sparkdesk_web/utils.py` & `sparkdesk-api-1.0.3/sparkdesk_web/utils.py`

 * *Files identical despite different names*

### Comparing `sparkdesk-api-1.0.2/sparkdesk_web/web.py` & `sparkdesk-api-1.0.3/sparkdesk_web/web.py`

 * *Files identical despite different names*

