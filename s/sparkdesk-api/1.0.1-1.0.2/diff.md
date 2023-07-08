# Comparing `tmp/sparkdesk-api-1.0.1.tar.gz` & `tmp/sparkdesk-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkdesk-api-1.0.1.tar", last modified: Sat Jul  8 08:26:39 2023, max compression
+gzip compressed data, was "sparkdesk-api-1.0.2.tar", last modified: Sat Jul  8 08:37:19 2023, max compression
```

## Comparing `sparkdesk-api-1.0.1.tar` & `sparkdesk-api-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 08:26:39.975810 sparkdesk-api-1.0.1/
--rw-rw-rw-   0        0        0    35823 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2604 2023-07-08 08:26:39.975810 sparkdesk-api-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2136 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.1/README.md
--rw-rw-rw-   0        0        0      111 2023-07-08 08:26:39.976810 sparkdesk-api-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      734 2023-07-08 08:26:30.000000 sparkdesk-api-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:26:39.954096 sparkdesk-api-1.0.1/sparkdesk_api/
--rw-rw-rw-   0        0        0      198 2023-07-08 08:19:56.000000 sparkdesk-api-1.0.1/sparkdesk_api/__init__.py
--rw-rw-rw-   0        0        0     6736 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.1/sparkdesk_api/core.py
--rw-rw-rw-   0        0        0     1786 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.1/sparkdesk_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:26:39.964099 sparkdesk-api-1.0.1/sparkdesk_api.egg-info/
--rw-rw-rw-   0        0        0     2604 2023-07-08 08:26:39.000000 sparkdesk-api-1.0.1/sparkdesk_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-07-08 08:26:39.000000 sparkdesk-api-1.0.1/sparkdesk_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 08:26:39.000000 sparkdesk-api-1.0.1/sparkdesk_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-08 08:26:39.000000 sparkdesk-api-1.0.1/sparkdesk_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 08:26:39.973807 sparkdesk-api-1.0.1/sparkdesk_web/
--rw-rw-rw-   0        0        0      198 2023-07-08 08:19:56.000000 sparkdesk-api-1.0.1/sparkdesk_web/__init__.py
--rw-rw-rw-   0        0        0     4580 2023-07-08 08:15:21.000000 sparkdesk-api-1.0.1/sparkdesk_web/core.py
--rw-rw-rw-   0        0        0      880 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.1/sparkdesk_web/utils.py
--rw-rw-rw-   0        0        0     1910 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.1/sparkdesk_web/web.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:37:19.969827 sparkdesk-api-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1646 2023-07-08 08:37:19.969827 sparkdesk-api-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1178 2023-07-08 08:34:53.000000 sparkdesk-api-1.0.2/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-08 08:37:19.971827 sparkdesk-api-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-07-08 08:37:17.000000 sparkdesk-api-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:37:19.950823 sparkdesk-api-1.0.2/sparkdesk_api/
+-rw-rw-rw-   0        0        0      198 2023-07-08 08:19:56.000000 sparkdesk-api-1.0.2/sparkdesk_api/__init__.py
+-rw-rw-rw-   0        0        0     6736 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.2/sparkdesk_api/core.py
+-rw-rw-rw-   0        0        0     1786 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.2/sparkdesk_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 08:37:19.959826 sparkdesk-api-1.0.2/sparkdesk_api.egg-info/
+-rw-rw-rw-   0        0        0     1646 2023-07-08 08:37:19.000000 sparkdesk-api-1.0.2/sparkdesk_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-07-08 08:37:19.000000 sparkdesk-api-1.0.2/sparkdesk_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 08:37:19.000000 sparkdesk-api-1.0.2/sparkdesk_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-08 08:37:19.000000 sparkdesk-api-1.0.2/sparkdesk_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 08:37:19.967826 sparkdesk-api-1.0.2/sparkdesk_web/
+-rw-rw-rw-   0        0        0      198 2023-07-08 08:19:56.000000 sparkdesk-api-1.0.2/sparkdesk_web/__init__.py
+-rw-rw-rw-   0        0        0     4580 2023-07-08 08:15:21.000000 sparkdesk-api-1.0.2/sparkdesk_web/core.py
+-rw-rw-rw-   0        0        0      880 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.2/sparkdesk_web/utils.py
+-rw-rw-rw-   0        0        0     1910 2023-07-08 07:11:06.000000 sparkdesk-api-1.0.2/sparkdesk_web/web.py
```

### Comparing `sparkdesk-api-1.0.1/LICENSE` & `sparkdesk-api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkdesk-api-1.0.1/PKG-INFO` & `sparkdesk-api-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,33 @@
 Metadata-Version: 2.1
 Name: sparkdesk-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: sparkdesk-api 讯飞星火大模型api
 Home-page: https://github.com/HildaM/sparkdesk-api
 Author: HildaM
 Author-email: Hilda_quan@163.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sparkdesk-api 讯飞星火大模型api
 > 如果该项目对你有帮助，不要忘记给我点个 star 哦！
 ## 使用方法
-TODO: 目前仅支持下载下来使用，暂不支持直接使用pip安装，后续将其上传到pypi后才可以 pip install。（预计这周末可以发布到python仓库中）
 ```shell
-cd sparkdesk-api
-pip install -r requirements.txt
+pip install sparkdesk-api==1.0.1
 ```
 
 ### 1. Web模式
 Web模式下，需要前往讯飞星火大模型web端通过 F12 抓取 3 个参数：cookie、fd、GtToken
-讯飞星火的web端有防护，在web端直接按 F12 不能打开开发者窗口。但是可以通过特殊方法打开：
-1. 进入 [https://xinghuo.xfyun.cn/](https://xinghuo.xfyun.cn/) 后登录账号，不要立即点“进入体验”，而是在这个页面点击 F12
-2. 进入 F12 开发者窗口后，将网页修改为“手机端”窗口
-    1. ![](docs/1688642799640-image.png)
-3. 在第二步完成后，才点击“进入体验”，进入讯飞星火的web端，可以发现成功变成手机端
-    1. ![](docs/1688642948745-image.png)
-4. 先发一条简单的语句，让讯飞回复一段话，然后在“Network”栏目找到 “chat” 请求，在该请求下抓取 3 个参数
-    1. ![](docs/1688643113313-image.png)
-    2. ![](docs/1688643185781-image.png)
-5. 获取后，即可开始使用 Web 模式
+- [获取参数的方法](https://github.com/HildaM/sparkdesk-api/tree/main/docs)
 
-#### 命令后模式
+#### 命令行操作
 ```shell
 python sparkdesk_web_cli.py
 ```
 
 #### api调用
 - chat()：一次询问
 - chat_stream()：连续询问，相当于命令行模式
```

### Comparing `sparkdesk-api-1.0.1/README.md` & `sparkdesk-api-1.0.2/sparkdesk_api.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+Metadata-Version: 2.1
+Name: sparkdesk-api
+Version: 1.0.2
+Summary: sparkdesk-api 讯飞星火大模型api
+Home-page: https://github.com/HildaM/sparkdesk-api
+Author: HildaM
+Author-email: Hilda_quan@163.com
+License: GNU General Public License v3.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # sparkdesk-api 讯飞星火大模型api
 > 如果该项目对你有帮助，不要忘记给我点个 star 哦！
 ## 使用方法
-TODO: 目前仅支持下载下来使用，暂不支持直接使用pip安装，后续将其上传到pypi后才可以 pip install。（预计这周末可以发布到python仓库中）
 ```shell
-cd sparkdesk-api
-pip install -r requirements.txt
+pip install sparkdesk-api==1.0.1
 ```
 
 ### 1. Web模式
 Web模式下，需要前往讯飞星火大模型web端通过 F12 抓取 3 个参数：cookie、fd、GtToken
-讯飞星火的web端有防护，在web端直接按 F12 不能打开开发者窗口。但是可以通过特殊方法打开：
-1. 进入 [https://xinghuo.xfyun.cn/](https://xinghuo.xfyun.cn/) 后登录账号，不要立即点“进入体验”，而是在这个页面点击 F12
-2. 进入 F12 开发者窗口后，将网页修改为“手机端”窗口
-    1. ![](docs/1688642799640-image.png)
-3. 在第二步完成后，才点击“进入体验”，进入讯飞星火的web端，可以发现成功变成手机端
-    1. ![](docs/1688642948745-image.png)
-4. 先发一条简单的语句，让讯飞回复一段话，然后在“Network”栏目找到 “chat” 请求，在该请求下抓取 3 个参数
-    1. ![](docs/1688643113313-image.png)
-    2. ![](docs/1688643185781-image.png)
-5. 获取后，即可开始使用 Web 模式
+- [获取参数的方法](https://github.com/HildaM/sparkdesk-api/tree/main/docs)
 
-#### 命令后模式
+#### 命令行操作
 ```shell
 python sparkdesk_web_cli.py
 ```
 
 #### api调用
 - chat()：一次询问
 - chat_stream()：连续询问，相当于命令行模式
```

### Comparing `sparkdesk-api-1.0.1/setup.py` & `sparkdesk-api-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
       long_description = fh.read()
 
 setuptools.setup(
       name="sparkdesk-api",
-      version="1.0.1",
+      version="1.0.2",
       author="HildaM",
       author_email="Hilda_quan@163.com",
       description="sparkdesk-api 讯飞星火大模型api",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/HildaM/sparkdesk-api",
       license='GNU General Public License v3.0',
```

### Comparing `sparkdesk-api-1.0.1/sparkdesk_api/core.py` & `sparkdesk-api-1.0.2/sparkdesk_api/core.py`

 * *Files identical despite different names*

### Comparing `sparkdesk-api-1.0.1/sparkdesk_api/utils.py` & `sparkdesk-api-1.0.2/sparkdesk_api/utils.py`

 * *Files identical despite different names*

### Comparing `sparkdesk-api-1.0.1/sparkdesk_web/core.py` & `sparkdesk-api-1.0.2/sparkdesk_web/core.py`

 * *Files identical despite different names*

### Comparing `sparkdesk-api-1.0.1/sparkdesk_web/utils.py` & `sparkdesk-api-1.0.2/sparkdesk_web/utils.py`

 * *Files identical despite different names*

### Comparing `sparkdesk-api-1.0.1/sparkdesk_web/web.py` & `sparkdesk-api-1.0.2/sparkdesk_web/web.py`

 * *Files identical despite different names*

