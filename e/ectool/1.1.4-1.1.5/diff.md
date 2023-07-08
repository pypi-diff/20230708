# Comparing `tmp/ectool-1.1.4.tar.gz` & `tmp/ectool-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ectool-1.1.4.tar", last modified: Fri Jul  7 14:48:04 2023, max compression
+gzip compressed data, was "ectool-1.1.5.tar", last modified: Sat Jul  8 03:06:36 2023, max compression
```

## Comparing `ectool-1.1.4.tar` & `ectool-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 14:48:04.573512 ectool-1.1.4/
--rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     2293 2023-07-07 14:48:04.574509 ectool-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2023-07-07 14:04:47.000000 ectool-1.1.4/README.md
--rw-rw-rw-   0        0        0      113 2023-07-07 14:48:04.574509 ectool-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     7947 2023-07-07 14:46:57.000000 ectool-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:48:04.553510 ectool-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 14:48:04.566510 ectool-1.1.4/src/ectool/
--rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.4/src/ectool/__init__.py
--rw-rw-rw-   0        0        0    15990 2023-07-07 14:41:24.000000 ectool-1.1.4/src/ectool/ecaction.py
--rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.4/src/ectool/ecag.py
--rw-rw-rw-   0        0        0     5148 2023-07-07 14:45:41.000000 ectool-1.1.4/src/ectool/eccli.py
--rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.4/src/ectool/ecconst.py
--rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.4/src/ectool/ecstruct.py
--rw-rw-rw-   0        0        0     3912 2023-07-07 14:36:13.000000 ectool-1.1.4/src/ectool/unpkg.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:48:04.572509 ectool-1.1.4/src/ectool.egg-info/
--rw-rw-rw-   0        0        0     2293 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 14:48:04.000000 ectool-1.1.4/src/ectool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 03:06:36.067153 ectool-1.1.5/
+-rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2331 2023-07-08 03:06:36.068153 ectool-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1288 2023-07-08 03:04:20.000000 ectool-1.1.5/README.md
+-rw-rw-rw-   0        0        0      113 2023-07-08 03:06:36.068153 ectool-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     7947 2023-07-08 03:04:34.000000 ectool-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:06:36.048151 ectool-1.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 03:06:36.060153 ectool-1.1.5/src/ectool/
+-rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.5/src/ectool/__init__.py
+-rw-rw-rw-   0        0        0    16103 2023-07-08 02:08:23.000000 ectool-1.1.5/src/ectool/ecaction.py
+-rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.5/src/ectool/ecag.py
+-rw-rw-rw-   0        0        0     6523 2023-07-08 03:02:18.000000 ectool-1.1.5/src/ectool/eccli.py
+-rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.5/src/ectool/ecconst.py
+-rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.5/src/ectool/ecstruct.py
+-rw-rw-rw-   0        0        0     3912 2023-07-08 02:01:12.000000 ectool-1.1.5/src/ectool/unpkg.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:06:36.066152 ectool-1.1.5/src/ectool.egg-info/
+-rw-rw-rw-   0        0        0     2331 2023-07-08 03:06:36.000000 ectool-1.1.5/src/ectool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-08 03:06:36.000000 ectool-1.1.5/src/ectool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 03:06:36.000000 ectool-1.1.5/src/ectool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-08 03:06:36.000000 ectool-1.1.5/src/ectool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-07-08 03:06:36.000000 ectool-1.1.5/src/ectool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 03:06:36.000000 ectool-1.1.5/src/ectool.egg-info/top_level.txt
```

### Comparing `ectool-1.1.4/LICENSE` & `ectool-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ectool-1.1.4/PKG-INFO` & `ectool-1.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.4
+Version: 1.1.5
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
@@ -37,34 +37,36 @@
 ```bash
 # 清华镜像
 pip3 install -U -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
 # 无镜像,或者系统默认镜像
 pip3 install -U ectool
 ```
 
-刷机(当前仅USB刷机), 支持binpkg和soc文件, 但暂不支持LuatOS的脚本刷机
+刷机(当前仅USB刷机), 支持binpkg和soc文件
 
 ```bash
 ectool burn -f example.binpkg
 # 启动后, 按住BOOT键, 复位模块, 或模块开机
 ```
 
 更多参数执行 `ectool -h` 获取说明
 
 ## TODO List
 
 * [x] EC618使用USB刷机
 * [x] binpkg解包
 * [x] 测试Linux下的兼容性
+* [x] 支持只刷AP或CP
 * [ ] EC618使用物理UART刷机
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
-* [ ] 支持只刷AP
 * [ ] 完整的注释
 * [ ] SoC日志解析
+* [ ] 支持从http加载固件文件进行下载
+* [ ] binpkg打包
 
 ## Linux刷机过程展示
 
 [![asciicast](https://asciinema.org/a/595464.svg)](https://asciinema.org/a/595464)
 
 ## 参考链接
```

### Comparing `ectool-1.1.4/README.md` & `ectool-1.1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,34 +11,36 @@
 ```bash
 # 清华镜像
 pip3 install -U -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
 # 无镜像,或者系统默认镜像
 pip3 install -U ectool
 ```
 
-刷机(当前仅USB刷机), 支持binpkg和soc文件, 但暂不支持LuatOS的脚本刷机
+刷机(当前仅USB刷机), 支持binpkg和soc文件
 
 ```bash
 ectool burn -f example.binpkg
 # 启动后, 按住BOOT键, 复位模块, 或模块开机
 ```
 
 更多参数执行 `ectool -h` 获取说明
 
 ## TODO List
 
 * [x] EC618使用USB刷机
 * [x] binpkg解包
 * [x] 测试Linux下的兼容性
+* [x] 支持只刷AP或CP
 * [ ] EC618使用物理UART刷机
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
-* [ ] 支持只刷AP
 * [ ] 完整的注释
 * [ ] SoC日志解析
+* [ ] 支持从http加载固件文件进行下载
+* [ ] binpkg打包
 
 ## Linux刷机过程展示
 
 [![asciicast](https://asciinema.org/a/595464.svg)](https://asciinema.org/a/595464)
 
 ## 参考链接
```

### Comparing `ectool-1.1.4/setup.py` & `ectool-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     name="ectool",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.1.4",  # Required
+    version="1.1.5",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A tools for EC modules, like EC618/EC616/EC718",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `ectool-1.1.4/src/ectool/ecaction.py` & `ectool-1.1.5/src/ectool/ecaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,16 @@
     ret = package_data(burncom, pCmd, fdata, pullupQspi=1)
     if ret != 0:
         return ret
 
     return 0
 
 def burn_img(burncom, path_or_data, img_type, storType, addr, tag="NAME"):
-    logging.debug("Burn image start " + str(img_type))
+    # logging.debug("Burn image start " + str(img_type))
+    logging.info("burn image " + tag + " " + str(img_type) + " " + str(storType) + " " + ("%08X" % (addr, )))
     # 1. 先执行一次 LPC Sync
     ret = burn_sync(burncom, enSynHandshakeType.SYNC_HANDSHAKE_LPC, 2)
     if ret != 0 :
         logging.error("lpc sync fail")
         return -1
     # 2. lpc burn one
     ret, _ = package_lpc_burn_one(burncom, img_type, storType)
```

### Comparing `ectool-1.1.4/src/ectool/ecag.py` & `ectool-1.1.5/src/ectool/ecag.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.4/src/ectool/eccli.py` & `ectool-1.1.5/src/ectool/eccli.py`

 * *Files 18% similar despite different names*

```diff
@@ -66,36 +66,52 @@
     if ret != 0 :
         logging.error("agentboot download fail")
         return ret
     logging.info("Done AgentBoot download")
 
     # time.sleep(1)
 
-    logging.info("Go   BL download")
-    ret = burn_img(burncom, jdata["ap_bootloader"]["data"], enBurnImageType.BTYPE_BOOTLOADER, STYPE_AP_FLASH, 0, tag="BL")
-    if ret != 0 :
-        logging.error("burn_img BootLoader fail")
-        return ret
-    logging.info("Done BL download")
-    logging.info("Go   AP download")
-    ret = burn_img(burncom, jdata["ap"]["data"], enBurnImageType.BTYPE_AP, STYPE_AP_FLASH, 0x24000, tag="AP")
-    if ret != 0 :
-        logging.error("burn_img AP fail")
-        return ret
-    logging.info("Done AP download")
-    logging.info("Go   CP download")
-    ret = burn_img(burncom, jdata["cp-demo-flash"]["data"], enBurnImageType.BTYPE_CP, STYPE_CP_FLASH, 0, tag="CP")
-    if ret != 0 :
-        logging.error("burn_img CP fail")
-        return ret
-    logging.info("Done CP download")
+    while 1 :
+        if "ap_bootloader" in jdata and ecargs.burn_bl == "y" :
+            logging.info("Go   BL download")
+            ret = burn_img(burncom, jdata["ap_bootloader"]["data"], enBurnImageType.BTYPE_BOOTLOADER, STYPE_AP_FLASH, 0, tag="BL")
+            if ret != 0 :
+                logging.error("burn_img BootLoader fail")
+                break
+            logging.info("Done BL download")
+        if "ap" in jdata and ecargs.burn_ap == "y" :
+            logging.info("Go   AP download")
+            ret = burn_img(burncom, jdata["ap"]["data"], enBurnImageType.BTYPE_AP, STYPE_AP_FLASH, 0x24000, tag="AP")
+            if ret != 0 :
+                logging.error("burn_img AP fail")
+                break
+            logging.info("Done AP download")
+        if "cp-demo-flash" in jdata and ecargs.burn_cp == "y" :
+            logging.info("Go   CP download")
+            ret = burn_img(burncom, jdata["cp-demo-flash"]["data"], enBurnImageType.BTYPE_CP, STYPE_CP_FLASH, 0, tag="CP")
+            if ret != 0 :
+                logging.error("burn_img CP fail")
+                break
+            logging.info("Done CP download")
+
+        if False and "script" in jdata and ecargs.burn_script == "y" :
+            logging.info("Do   Script download")
+            ret = burn_img(burncom, jdata["script"]["data"], enBurnImageType.BTYPE_FLEXFILE, STYPE_AP_FLASH, jdata["script"]["burn_addr"], tag="SCRIPT")
+            if ret != 0 :
+                logging.error("burn_img SCRIPT fail")
+                break
+            logging.info("Done Script download")
+
+        break
 
-    ret = sys_reset(burncom)
-    logging.info("sys reset " + str(ret))
-    logging.info("burn ok")
+    logging.info("sys reset " + str(sys_reset(burncom)))
+    if ret == 0:
+        logging.info("burn ok")
+    else :
+        logging.info("burn fail " + str(ret))
         
 def cli_unpack() :
     if not ecargs.file :
         logger.error("require -f/--file !!!")
         sys.exit(3)
     import ectool.unpkg as unpkg
     unpkg.binpkg_unpack(ecargs.file, ecargs.outdir)
@@ -105,18 +121,23 @@
     global ecargs
     global logger
     import argparse
     parser = argparse.ArgumentParser(description='A tool for EC modules, like EC618')
     parser.add_argument("action", choices=["burn", "unpack"], help="main action to perform")
     parser.add_argument("--file", "-f", help="file path")
     parser.add_argument("--burn_addr",  help="burn bin file to addr")
+    parser.add_argument("--burn_bl",  default="y",  choices=["y", "n"], help="burn BootLoader, default y")
+    parser.add_argument("--burn_ap",  default="y",  choices=["y", "n"], help="burn AP zone, default y")
+    parser.add_argument("--burn_cp",  default="y",  choices=["y", "n"], help="burn CP zone, default y")
+    parser.add_argument("--burn_script",  default="y",  choices=["y", "n"], help="burn Script Zone, default y")
     parser.add_argument("--img_type", "-t", choices=["BL", "CP", "AP", "FF"], help="image type for bin file")
     parser.add_argument("--sysreset", help="reset the chip after burn success", const=True, nargs="?")
     parser.add_argument("--debug", "-d", const=True, nargs="?", help="debug mode")
     parser.add_argument("--port", "-p", default="auto", help="COM port or path, like COM49, default is auto search")
+    parser.add_argument("--port_type", default="USB", choices=["USB", "UART"], help="USB or UART")
     parser.add_argument("--outdir", "-o", default="tmp", help="output dir for actoion like unpack/diff")
     parser.add_argument("--allow-upload", const=True, nargs="?", help="diff action require upload binpkg/soc to remote server, add this option means you agree it")
     ecargs = parser.parse_args()
     if len(sys.argv) == 1 or not ecargs.action :
         parser.print_help()
         return
     if ecargs.debug :
```

### Comparing `ectool-1.1.4/src/ectool/ecconst.py` & `ectool-1.1.5/src/ectool/ecconst.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.4/src/ectool/ecstruct.py` & `ectool-1.1.5/src/ectool/ecstruct.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.4/src/ectool/unpkg.py` & `ectool-1.1.5/src/ectool/unpkg.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                         tmpdata = bio.read()
                         jdata["script"] = {
                             "addr" : 0,
                             "flash_size" : 0,
                             "offset" : 0,
                             "image_size" : len(tmpdata),
                             "hash" : hashlib.sha256(tmpdata).hexdigest(),
-                            "image_type" : "CP"
+                            "image_type" : "AP"
                         }
                         if outpath_dir :
                             with open(os.path.join(outpath_dir, fname), "wb") as f :
                                 f.write(tmpdata)
                         if ram :
                             jdata["script"]["data"] = tmpdata
                     elif str(fname) == "info.json" :
```

### Comparing `ectool-1.1.4/src/ectool.egg-info/PKG-INFO` & `ectool-1.1.5/src/ectool.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.4
+Version: 1.1.5
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
@@ -37,34 +37,36 @@
 ```bash
 # 清华镜像
 pip3 install -U -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
 # 无镜像,或者系统默认镜像
 pip3 install -U ectool
 ```
 
-刷机(当前仅USB刷机), 支持binpkg和soc文件, 但暂不支持LuatOS的脚本刷机
+刷机(当前仅USB刷机), 支持binpkg和soc文件
 
 ```bash
 ectool burn -f example.binpkg
 # 启动后, 按住BOOT键, 复位模块, 或模块开机
 ```
 
 更多参数执行 `ectool -h` 获取说明
 
 ## TODO List
 
 * [x] EC618使用USB刷机
 * [x] binpkg解包
 * [x] 测试Linux下的兼容性
+* [x] 支持只刷AP或CP
 * [ ] EC618使用物理UART刷机
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
-* [ ] 支持只刷AP
 * [ ] 完整的注释
 * [ ] SoC日志解析
+* [ ] 支持从http加载固件文件进行下载
+* [ ] binpkg打包
 
 ## Linux刷机过程展示
 
 [![asciicast](https://asciinema.org/a/595464.svg)](https://asciinema.org/a/595464)
 
 ## 参考链接
```

