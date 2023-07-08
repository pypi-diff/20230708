# Comparing `tmp/lib-not-dr-0.0.4.tar.gz` & `tmp/lib-not-dr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-not-dr-0.0.4.tar", last modified: Sat Jun 24 18:21:21 2023, max compression
+gzip compressed data, was "lib-not-dr-0.1.0.tar", last modified: Sat Jul  8 03:33:44 2023, max compression
```

## Comparing `lib-not-dr-0.0.4.tar` & `lib-not-dr-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:21:21.417413 lib-not-dr-0.0.4/
--rw-rw-rw-   0        0        0    17098 2023-06-09 16:24:01.000000 lib-not-dr-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    21441 2023-06-24 18:21:21.416403 lib-not-dr-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      749 2023-06-24 13:59:54.000000 lib-not-dr-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 18:21:21.395788 lib-not-dr-0.0.4/lib_not_dr/
--rw-rw-rw-   0        0        0      205 2023-06-24 13:59:51.000000 lib-not-dr-0.0.4/lib_not_dr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:21:21.406786 lib-not-dr-0.0.4/lib_not_dr/nuitka/
--rw-rw-rw-   0        0        0     6464 2023-06-24 12:56:32.000000 lib-not-dr-0.0.4/lib_not_dr/nuitka/compile.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:21:21.413791 lib-not-dr-0.0.4/lib_not_dr/types/
--rw-rw-rw-   0        0        0      785 2023-06-17 04:51:13.000000 lib-not-dr-0.0.4/lib_not_dr/types/__init__.py
--rw-rw-rw-   0        0        0     8943 2023-06-24 13:04:34.000000 lib-not-dr-0.0.4/lib_not_dr/types/options.py
--rw-rw-rw-   0        0        0     8114 2023-06-17 04:49:52.000000 lib-not-dr-0.0.4/lib_not_dr/types/version.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:21:21.404786 lib-not-dr-0.0.4/lib_not_dr.egg-info/
--rw-rw-rw-   0        0        0    21441 2023-06-24 18:21:21.000000 lib-not-dr-0.0.4/lib_not_dr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-06-24 18:21:21.000000 lib-not-dr-0.0.4/lib_not_dr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:21:21.000000 lib-not-dr-0.0.4/lib_not_dr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 18:21:21.000000 lib-not-dr-0.0.4/lib_not_dr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-06-24 13:58:50.000000 lib-not-dr-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 18:21:21.417413 lib-not-dr-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 03:33:44.030456 lib-not-dr-0.1.0/
+-rw-rw-rw-   0        0        0    17098 2023-06-09 16:24:01.000000 lib-not-dr-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0    22148 2023-07-08 03:33:44.029459 lib-not-dr-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-07-08 03:32:43.000000 lib-not-dr-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 03:33:44.009457 lib-not-dr-0.1.0/lib_not_dr/
+-rw-rw-rw-   0        0        0      205 2023-07-08 03:23:46.000000 lib-not-dr-0.1.0/lib_not_dr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:33:44.019458 lib-not-dr-0.1.0/lib_not_dr/nuitka/
+-rw-rw-rw-   0        0        0     7093 2023-07-08 03:20:15.000000 lib-not-dr-0.1.0/lib_not_dr/nuitka/compile.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:33:44.025458 lib-not-dr-0.1.0/lib_not_dr/types/
+-rw-rw-rw-   0        0        0      785 2023-06-17 04:51:13.000000 lib-not-dr-0.1.0/lib_not_dr/types/__init__.py
+-rw-rw-rw-   0        0        0     8943 2023-06-24 13:04:34.000000 lib-not-dr-0.1.0/lib_not_dr/types/options.py
+-rw-rw-rw-   0        0        0     8114 2023-06-17 04:49:52.000000 lib-not-dr-0.1.0/lib_not_dr/types/version.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:33:44.017457 lib-not-dr-0.1.0/lib_not_dr.egg-info/
+-rw-rw-rw-   0        0        0    22148 2023-07-08 03:33:43.000000 lib-not-dr-0.1.0/lib_not_dr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-07-08 03:33:43.000000 lib-not-dr-0.1.0/lib_not_dr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 03:33:43.000000 lib-not-dr-0.1.0/lib_not_dr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-08 03:33:43.000000 lib-not-dr-0.1.0/lib_not_dr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-07-08 03:24:06.000000 lib-not-dr-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 03:33:44.030456 lib-not-dr-0.1.0/setup.cfg
```

### Comparing `lib-not-dr-0.0.4/LICENSE` & `lib-not-dr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.4/PKG-INFO` & `lib-not-dr-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-not-dr
-Version: 0.0.4
+Version: 0.1.0
 Summary: A python lib created from Difficult Rocket development
 Author-email: shenjackyuanjie <3695888@qq.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -390,15 +390,15 @@
 
 A python lib came from [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) development
 
 一个在 [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) 开发中 分离出来的 python 库
 
 ## Information/信息
 
-- Version/版本: 0.0.4
+- Version/版本: 0.1.0
 
 ### Author/作者
 
 [shenjackyuanjie](https://github/shenjackyuanjie)
 
 ### License/许可证
 
@@ -410,16 +410,46 @@
 pip install lib-not-dr
 ```
 
 ## 使用/Usage
 
 ### Nuitka Compiler Helper
 
+> simple example
+> 简单示例
+
 ```python
 import subprocess
 from lib_not_dr.nuitka import CompilerHelper
 
 compiler = CompilerHelper("main.py")
 
 print(compiler)
 subprocess.run(compiler.gen_subprocess_cmd())
 ```
+
+> more complex example
+> 复杂示例
+
+```python
+import sys
+import subprocess
+from lib_not_dr.nuitka import CompilerHelper
+
+compiler = CompilerHelper("main.py", run_after_build=True)
+
+print(compiler)
+
+if '-y' in sys.argv or '--yes' in sys.argv:
+    do_run = True
+elif '-n' in sys.argv or '--no' in sys.argv:
+    do_run = False
+else: # do_run is None
+    while (do_run := input("compile? [y/n]").lower()) not in ["y", "n", "yes", "no"]:
+        # 获取用户输入是否编译
+        # get user confirmation to compile or not
+    do_run = True if do_run[0] == "y" else False
+
+if do_run:
+    subprocess.run(compiler.gen_subprocess_cmd())
+
+```
```

### Comparing `lib-not-dr-0.0.4/lib_not_dr/nuitka/compile.py` & `lib-not-dr-0.1.0/lib_not_dr/nuitka/compile.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 #  Difficult Rocket
 #  Copyright © 2020-2023 by shenjackyuanjie 3695888@qq.com
 #  All rights reserved
 #  -------------------------------
 
 # 用于使用 nuitka 构建 DR
 import platform
+import warnings
 import traceback
 from pathlib import Path
 from typing import List, Tuple, Optional
 
-from lib_not_dr.types import Options, Version
+from lib_not_dr.types import Options, Version, VersionRequirement
 
 
 def _add_cmd(cmd: List[str], string: Optional[str]) -> List[str]:
     if string is not None and string:
         cmd.append(string)
     return cmd
 
@@ -27,30 +28,33 @@
     """
     name = 'Nuitka Compiler Helper'
 
     output_path: Path = Path('./build')
     src_file: Path
 
     python_cmd: str = 'python'
+    compat_nuitka_version: VersionRequirement = VersionRequirement("~1.7.1")  # STATIC VERSION
 
     # 以下为 nuitka 的参数
+    # nuitka options below
     use_lto: bool = False  # --lto=yes (no is faster)
     use_clang: bool = True  # --clang
     use_msvc: bool = True  # --msvc=latest
     use_mingw: bool = False  # --mingw64
     standalone: bool = True  # --standalone
     use_ccache: bool = True  # not --disable-ccache
     enable_console: bool = True  # --enable-console / --disable-console
 
     show_progress: bool = True  # --show-progress
     show_memory: bool = False  # --show-memory
     save_xml: bool = False  # --xml
     xml_path: Path = Path('build/compile_data.xml')
 
     download_confirm: bool = True  # --assume-yes-for-download
+    run_after_build: bool = False  # --run
 
     company_name: Optional[str] = ''
     product_name: Optional[str] = ''
     file_version: Optional[Version] = None
     product_version: Optional[Version] = None
     file_description: Optional[str] = ''  # --file-description
 
@@ -64,14 +68,20 @@
     include_data_dir: List[Tuple[str, str]] = []
     include_packages: List[str] = []
 
     enable_plugin: List[str] = []  # --enable-plugin=xxx,xxx
     disable_plugin: List[str] = []  # --disable-plugin=xxx,xxx
 
     def init(self, **kwargs) -> None:
+        if (compat_version := kwargs.get('compat_nuitka_version')) is not None:
+            if not self.compat_nuitka_version.accept(compat_version):
+                warnings.warn(
+                    f"Nuitka version may not compat with {compat_version}\n"
+                    "requirement: {self.compat_nuitka_version}"
+                )
         # 非 windows 平台不使用 msvc
         if platform.system() != 'Windows':
             self.use_msvc = False
             self.use_mingw = False
         else:
             self.use_mingw = self.use_mingw and not self.use_msvc
             # Windows 平台下使用 msvc 时不使用 mingw
@@ -122,14 +132,15 @@
         _add_cmd(cmd_list, '--mingw64' if self.use_mingw else None)
         _add_cmd(cmd_list, '--standalone' if self.standalone else None)
 
         _add_cmd(cmd_list, '--disable-ccache' if not self.use_ccache else None)
         _add_cmd(cmd_list, '--show-progress' if self.show_progress else None)
         _add_cmd(cmd_list, '--show-memory' if self.show_memory else None)
         _add_cmd(cmd_list, '--assume-yes-for-download' if self.download_confirm else None)
+        _add_cmd(cmd_list, '--run' if self.run_after_build else None)
         _add_cmd(cmd_list, '--enable-console' if self.enable_console else '--disable-console')
 
         _add_cmd(cmd_list, f'--xml={self.xml_path.absolute()}' if self.save_xml else None)
         _add_cmd(cmd_list, f'--output-dir={self.output_path.absolute()}' if self.output_path else None)
         _add_cmd(cmd_list, f'--company-name={self.company_name}' if self.company_name else None)
         _add_cmd(cmd_list, f'--product-name={self.product_name}' if self.product_name else None)
         _add_cmd(cmd_list, f'--file-version={self.file_version}' if self.file_version else None)
@@ -143,9 +154,9 @@
         _add_cmd(cmd_list, f'--disable-plugin={",".join(self.disable_plugin)}' if self.disable_plugin else None)
 
         if self.include_data_dir:
             cmd_list += [f"--include-data-dir={src}={dst}" for src, dst in self.include_data_dir]
         if self.include_packages:
             cmd_list += [f"--include-package={package}" for package in self.include_packages]
 
-        cmd_list.append(f"{self.src_file}")
+        cmd_list.append(f"--main={self.src_file}")
         return cmd_list
```

### Comparing `lib-not-dr-0.0.4/lib_not_dr/types/__init__.py` & `lib-not-dr-0.1.0/lib_not_dr/types/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.4/lib_not_dr/types/options.py` & `lib-not-dr-0.1.0/lib_not_dr/types/options.py`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.4/lib_not_dr/types/version.py` & `lib-not-dr-0.1.0/lib_not_dr/types/version.py`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.4/lib_not_dr.egg-info/PKG-INFO` & `lib-not-dr-0.1.0/lib_not_dr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-not-dr
-Version: 0.0.4
+Version: 0.1.0
 Summary: A python lib created from Difficult Rocket development
 Author-email: shenjackyuanjie <3695888@qq.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -390,15 +390,15 @@
 
 A python lib came from [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) development
 
 一个在 [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) 开发中 分离出来的 python 库
 
 ## Information/信息
 
-- Version/版本: 0.0.4
+- Version/版本: 0.1.0
 
 ### Author/作者
 
 [shenjackyuanjie](https://github/shenjackyuanjie)
 
 ### License/许可证
 
@@ -410,16 +410,46 @@
 pip install lib-not-dr
 ```
 
 ## 使用/Usage
 
 ### Nuitka Compiler Helper
 
+> simple example
+> 简单示例
+
 ```python
 import subprocess
 from lib_not_dr.nuitka import CompilerHelper
 
 compiler = CompilerHelper("main.py")
 
 print(compiler)
 subprocess.run(compiler.gen_subprocess_cmd())
 ```
+
+> more complex example
+> 复杂示例
+
+```python
+import sys
+import subprocess
+from lib_not_dr.nuitka import CompilerHelper
+
+compiler = CompilerHelper("main.py", run_after_build=True)
+
+print(compiler)
+
+if '-y' in sys.argv or '--yes' in sys.argv:
+    do_run = True
+elif '-n' in sys.argv or '--no' in sys.argv:
+    do_run = False
+else: # do_run is None
+    while (do_run := input("compile? [y/n]").lower()) not in ["y", "n", "yes", "no"]:
+        # 获取用户输入是否编译
+        # get user confirmation to compile or not
+    do_run = True if do_run[0] == "y" else False
+
+if do_run:
+    subprocess.run(compiler.gen_subprocess_cmd())
+
+```
```

### Comparing `lib-not-dr-0.0.4/pyproject.toml` & `lib-not-dr-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-version = "0.0.4"
+version = "0.1.0"
 name = "lib-not-dr"
 
 description = "A python lib created from Difficult Rocket development"
 
 readme = "README.md"
 
 authors = [
```

