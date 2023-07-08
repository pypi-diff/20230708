# Comparing `tmp/hat_duktape-0.5.5-cp38.cp39.cp310.cp311-cp38.cp39.cp310.cp311-win_amd64.whl.zip` & `tmp/hat_duktape-0.5.6-cp310.cp311-cp310.cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 392566 bytes, number of entries: 8
--rw-r--r--  2.0 unx    13868 b- defN 23-Mar-02 16:56 hat_duktape-0.5.5.data/purelib/hat/duktape/__init__.py
--rwxr-xr-x  2.0 unx   988122 b- defN 23-Mar-02 17:01 hat_duktape-0.5.5.data/purelib/hat/duktape/duktape.dll
--rw-r--r--  2.0 unx    11358 b- defN 23-Mar-02 17:01 hat_duktape-0.5.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1856 b- defN 23-Mar-02 17:01 hat_duktape-0.5.5.dist-info/METADATA
--rw-r--r--  2.0 unx      491 b- defN 23-Mar-02 17:01 hat_duktape-0.5.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Mar-02 17:01 hat_duktape-0.5.5.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-02 17:01 hat_duktape-0.5.5.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      722 b- defN 23-Mar-02 17:01 hat_duktape-0.5.5.dist-info/RECORD
-8 files, 1016422 bytes uncompressed, 391290 bytes compressed:  61.5%
+Zip file size: 393701 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      245 b- defN 23-Jul-08 17:02 hat_duktape-0.5.6.data/purelib/hat/duktape/__init__.py
+-rwxr-xr-x  2.0 unx   988122 b- defN 23-Jul-08 17:07 hat_duktape-0.5.6.data/purelib/hat/duktape/duktape.dll
+-rw-r--r--  2.0 unx     7990 b- defN 23-Jul-08 16:59 hat_duktape-0.5.6.data/purelib/hat/duktape/interpreter.py
+-rw-r--r--  2.0 unx     7149 b- defN 23-Jul-08 17:01 hat_duktape-0.5.6.data/purelib/hat/duktape/lib.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jul-08 17:07 hat_duktape-0.5.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2250 b- defN 23-Jul-08 17:07 hat_duktape-0.5.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      183 b- defN 23-Jul-08 17:07 hat_duktape-0.5.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-08 17:07 hat_duktape-0.5.6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-08 17:07 hat_duktape-0.5.6.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      940 b- defN 23-Jul-08 17:07 hat_duktape-0.5.6.dist-info/RECORD
+10 files, 1018242 bytes uncompressed, 392061 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
-Filename: hat_duktape-0.5.5.data/purelib/hat/duktape/__init__.py
+Filename: hat_duktape-0.5.6.data/purelib/hat/duktape/__init__.py
 Comment: 
 
-Filename: hat_duktape-0.5.5.data/purelib/hat/duktape/duktape.dll
+Filename: hat_duktape-0.5.6.data/purelib/hat/duktape/duktape.dll
 Comment: 
 
-Filename: hat_duktape-0.5.5.dist-info/LICENSE
+Filename: hat_duktape-0.5.6.data/purelib/hat/duktape/interpreter.py
 Comment: 
 
-Filename: hat_duktape-0.5.5.dist-info/METADATA
+Filename: hat_duktape-0.5.6.data/purelib/hat/duktape/lib.py
 Comment: 
 
-Filename: hat_duktape-0.5.5.dist-info/WHEEL
+Filename: hat_duktape-0.5.6.dist-info/LICENSE
 Comment: 
 
-Filename: hat_duktape-0.5.5.dist-info/top_level.txt
+Filename: hat_duktape-0.5.6.dist-info/METADATA
 Comment: 
 
-Filename: hat_duktape-0.5.5.dist-info/zip-safe
+Filename: hat_duktape-0.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: hat_duktape-0.5.5.dist-info/RECORD
+Filename: hat_duktape-0.5.6.dist-info/top_level.txt
+Comment: 
+
+Filename: hat_duktape-0.5.6.dist-info/zip-safe
+Comment: 
+
+Filename: hat_duktape-0.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `hat_duktape-0.5.5.data/purelib/hat/duktape/duktape.dll` & `hat_duktape-0.5.6.data/purelib/hat/duktape/duktape.dll`

 * *Files 0% similar despite different names*

### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Thu Mar  2 17:01:06 2023
+Time/Date		Sat Jul  8 17:07:36 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	38
 SizeOfCode		000000000005e000
 SizeOfInitializedData	0000000000070000
 SizeOfUninitializedData	0000000000000e00
 AddressOfEntryPoint	0000000000001350
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		000e3000
 SizeOfHeaders		00000600
-CheckSum		000ff779
+CheckSum		000fb9a8
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
```

## Comparing `hat_duktape-0.5.5.dist-info/LICENSE` & `hat_duktape-0.5.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_duktape-0.5.5.dist-info/METADATA` & `hat_duktape-0.5.6.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,85 @@
 Metadata-Version: 2.1
 Name: hat-duktape
-Version: 0.5.5
+Version: 0.5.6
 Summary: Hat Python Duktape JS wrapper
 Home-page: https://github.com/hat-open/hat-duktape
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: hat-util (~=0.6.8)
 
-hat-duktape - Python Duktape wrapper
-====================================
+.. _online documentation: https://hat-duktape.hat-open.com
+.. _git repository: https://github.com/hat-open/hat-duktape.git
+.. _PyPI project: https://pypi.org/project/hat-duktape
+.. _pydoit: https://pydoit.org
+.. _Hat Open: https://hat-open.com
+.. _Končar Digital: https://www.koncar.hr/en
 
-This library is part of Hat Open project - open-source framework of tools and
-libraries for developing applications used for remote monitoring, control and
-management of intelligent electronic devices such as IoT devices, PLCs,
-industrial automation or home automation systems.
 
-Development of Hat Open and associated repositories is sponsored by
-`Končar Digital <https://www.koncar.hr>`_.
+hat-duktape - Python Duktape wrapper
+====================================
 
 For more information see:
 
-    * hat-duktape documentation - `<https://hat-duktape.hat-open.com>`_
-    * hat-duktape git repository - `<https://github.com/hat-open/hat-duktape.git>`_
-    * Hat Open homepage - `<https://hat-open.com>`_
+* `online documentation`_
+* `git repository`_
 
-.. warning::
 
-    This project is currently in state of active development. Features,
-    functionality and API are unstable.
+Runtime requirements
+--------------------
+
+* python >=3.10
 
 
 Install
 -------
 
-::
+`hat-duktape` is available as `PyPI project`_::
 
     $ pip install hat-duktape
 
 
+Build
+-----
+
+Build tool used for `hat-duktape` is `pydoit`_. It can be installed together
+with other python dependencies by running::
+
+    $ pip install -r requirements.pip.dev.txt
+
+For listing available doit tasks, use::
+
+    $ doit list
+
+Default task::
+
+    $ doit
+
+creates wheel package inside `build` directory.
+
+
+Hat Open
+--------
+
+`hat-duktape` is part of `Hat Open`_ project - open-source framework of tools
+and libraries for developing applications used for remote monitoring, control
+and management of intelligent electronic devices such as IoT devices, PLCs,
+industrial automation or home automation systems.
+
+Development of Hat Open and associated repositories is sponsored by
+`Končar Digital`_.
+
+
 License
 -------
 
-Copyright 2020-2022 Hat Open AUTHORS
+Copyright 2020-2023 Hat Open AUTHORS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

## Comparing `hat_duktape-0.5.5.dist-info/RECORD` & `hat_duktape-0.5.6.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-hat_duktape-0.5.5.data/purelib/hat/duktape/__init__.py,sha256=3YigVFSEfJll3eix3nUHlVX5cAOboz-t_K9zfiWd0jo,13868
-hat_duktape-0.5.5.data/purelib/hat/duktape/duktape.dll,sha256=2eYKz8C6IY6L-i25is98Qas6k2W64H-qR4wD18LbSQE,988122
-hat_duktape-0.5.5.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-hat_duktape-0.5.5.dist-info/METADATA,sha256=X5SpMQDFL-4NyM8wgnGXUUiA1fhlPIBzsnNJRTw7kt4,1856
-hat_duktape-0.5.5.dist-info/WHEEL,sha256=tXwr1OxLG8e_RzW8jEmH-f47406vyC7kTbY0uthPazo,491
-hat_duktape-0.5.5.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
-hat_duktape-0.5.5.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-hat_duktape-0.5.5.dist-info/RECORD,,
+hat_duktape-0.5.6.data/purelib/hat/duktape/__init__.py,sha256=zpclIvmjXn3ULcQfATvj1sQmLfBMCY7KsG_tFbx4Hw0,245
+hat_duktape-0.5.6.data/purelib/hat/duktape/duktape.dll,sha256=j9IRSMs3mPg-NNK4EdhezfqgBEpeqP1BH9ojbRYiWFQ,988122
+hat_duktape-0.5.6.data/purelib/hat/duktape/interpreter.py,sha256=M0SgbuZfAd3hM1t3DSlZr6IvAoKBgjaWRVCUsKoZ2t8,7990
+hat_duktape-0.5.6.data/purelib/hat/duktape/lib.py,sha256=I3QVoSEFSGBIiM3GpAdUtq7TZjEG2iJZxVHbbMAHXoE,7149
+hat_duktape-0.5.6.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+hat_duktape-0.5.6.dist-info/METADATA,sha256=4dK09V4qOKBB6ZKlmNhsR5_ERez4Fv1AnR6LRQDpVAU,2250
+hat_duktape-0.5.6.dist-info/WHEEL,sha256=KRr3Tk41OiJVTi6ZHdJQInSJjc0D-MmV-3xGzC3Zc3Q,183
+hat_duktape-0.5.6.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
+hat_duktape-0.5.6.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+hat_duktape-0.5.6.dist-info/RECORD,,
```

