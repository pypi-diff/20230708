# Comparing `tmp/LolzteamApi-1.0.12.tar.gz` & `tmp/LolzteamApi-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LolzteamApi-1.0.12.tar", last modified: Fri Jul  7 21:05:15 2023, max compression
+gzip compressed data, was "LolzteamApi-1.0.13.tar", last modified: Sat Jul  8 01:34:04 2023, max compression
```

## Comparing `LolzteamApi-1.0.12.tar` & `LolzteamApi-1.0.13.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 21:05:15.321929 LolzteamApi-1.0.12/
--rw-rw-rw-   0        0        0     1082 2023-07-07 14:49:03.000000 LolzteamApi-1.0.12/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-07 21:05:15.314929 LolzteamApi-1.0.12/LolzteamApi/
--rw-rw-rw-   0        0        0   163270 2023-07-07 21:04:12.000000 LolzteamApi-1.0.12/LolzteamApi/LolzteamApi.py
--rw-rw-rw-   0        0        0       38 2023-07-07 21:04:12.000000 LolzteamApi-1.0.12/LolzteamApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 21:05:15.319927 LolzteamApi-1.0.12/LolzteamApi.egg-info/
--rw-rw-rw-   0        0        0     2282 2023-07-07 21:05:14.000000 LolzteamApi-1.0.12/LolzteamApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-07 21:05:15.000000 LolzteamApi-1.0.12/LolzteamApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 21:05:15.000000 LolzteamApi-1.0.12/LolzteamApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 21:05:15.000000 LolzteamApi-1.0.12/LolzteamApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 21:05:15.000000 LolzteamApi-1.0.12/LolzteamApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2282 2023-07-07 21:05:15.320926 LolzteamApi-1.0.12/PKG-INFO
--rw-rw-rw-   0        0        0     1881 2023-07-07 21:02:06.000000 LolzteamApi-1.0.12/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 21:05:15.321929 LolzteamApi-1.0.12/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-07-07 21:03:24.000000 LolzteamApi-1.0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 01:34:04.287033 LolzteamApi-1.0.13/
+-rw-rw-rw-   0        0        0     1089 2023-07-07 23:34:42.000000 LolzteamApi-1.0.13/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-08 01:34:04.270642 LolzteamApi-1.0.13/LolzteamApi/
+-rw-rw-rw-   0        0        0   163270 2023-07-07 21:04:12.000000 LolzteamApi-1.0.13/LolzteamApi/LolzteamApi.py
+-rw-rw-rw-   0        0        0      111 2023-07-08 00:37:47.000000 LolzteamApi-1.0.13/LolzteamApi/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-07-08 00:37:17.000000 LolzteamApi-1.0.13/LolzteamApi/check_updates.py
+drwxrwxrwx   0        0        0        0 2023-07-08 01:34:04.279199 LolzteamApi-1.0.13/LolzteamApi.egg-info/
+-rw-rw-rw-   0        0        0     2260 2023-07-08 01:34:04.000000 LolzteamApi-1.0.13/LolzteamApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-08 01:34:04.000000 LolzteamApi-1.0.13/LolzteamApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 01:34:04.000000 LolzteamApi-1.0.13/LolzteamApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-08 01:34:04.000000 LolzteamApi-1.0.13/LolzteamApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-08 01:34:04.000000 LolzteamApi-1.0.13/LolzteamApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2260 2023-07-08 01:34:04.282834 LolzteamApi-1.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-07-07 23:34:42.000000 LolzteamApi-1.0.13/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 01:34:04.287033 LolzteamApi-1.0.13/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-07-08 01:33:44.000000 LolzteamApi-1.0.13/setup.py
```

### Comparing `LolzteamApi-1.0.12/LICENSE` & `LolzteamApi-1.0.13/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 AS7RID
+Copyright (c) 2023 AS7RIDENiED
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `LolzteamApi-1.0.12/LolzteamApi/LolzteamApi.py` & `LolzteamApi-1.0.13/LolzteamApi/LolzteamApi.py`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.12/LolzteamApi.egg-info/PKG-INFO` & `LolzteamApi-1.0.13/LolzteamApi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.12
+Version: 1.0.13
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Lolzteam Python API
+
 <p align="center">
     <a href="https://zelenka.guru/members/2410024"><img width="800" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
 
-![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-darkgreen?style=flat-square&logo=qiwi&link=https%3A%2F%2Flzt.market%2Fbalance%2Ftransfer%3Fuser_id%3D2410024%26comment%3DThanks%2520for%2520creating%2520LolzteamApi%26amount%3D500)
+[![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE)
 
 
 ## Installation
 
 You can install the library using pip:
 
@@ -38,20 +39,23 @@
 ```
 
 ## Examples
 
 <p align="left">
     <a href="https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/Examples/example.py"><img width="150" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
+
 <p align="left">
     <a href="https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/Examples/example_market.py"><img width="150" src="https://lzt.market/styles/market/logo_by_DaWeed_X_KASTE.svg" alt="Material Bread logo"></a>
 </p>
 
 
 ## Official Lolzteam documentation
+
 <p align="left">
     <a href="https://docs.api.zelenka.guru/?forum"><img width="150" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
+
 <p align="left">
     <a href="https://docs.api.zelenka.guru/?market"><img width="150" src="https://lzt.market/styles/market/logo_by_DaWeed_X_KASTE.svg" alt="Material Bread logo"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.12 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.13 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
-![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
-darkgreen?style=flat-
-square&logo=qiwi&link=https%3A%2F%2Flzt.market%2Fbalance%2Ftransfer%3Fuser_id%3D2410024%26comment%3DThanks%2520for%2520creating%2520LolzteamApi%26amount%3D500)
+[![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
+darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/
+transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE) ## Installation
 You can install the library using pip: ```cmd pip install LolzteamApi ``` ##
 Usage Import the `LolzteamApi` module and create an instance of the
 `LolzteamApi` class to start using the API: ```python from LolzteamApi import
 LolzteamApi api = LolzteamApi(token='your_token') ``` ## Examples
 [Material_Bread_logo]
```

### Comparing `LolzteamApi-1.0.12/PKG-INFO` & `LolzteamApi-1.0.13/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.12
+Version: 1.0.13
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Lolzteam Python API
+
 <p align="center">
     <a href="https://zelenka.guru/members/2410024"><img width="800" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
 
-![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-darkgreen?style=flat-square&logo=qiwi&link=https%3A%2F%2Flzt.market%2Fbalance%2Ftransfer%3Fuser_id%3D2410024%26comment%3DThanks%2520for%2520creating%2520LolzteamApi%26amount%3D500)
+[![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE)
 
 
 ## Installation
 
 You can install the library using pip:
 
@@ -38,20 +39,23 @@
 ```
 
 ## Examples
 
 <p align="left">
     <a href="https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/Examples/example.py"><img width="150" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
+
 <p align="left">
     <a href="https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/Examples/example_market.py"><img width="150" src="https://lzt.market/styles/market/logo_by_DaWeed_X_KASTE.svg" alt="Material Bread logo"></a>
 </p>
 
 
 ## Official Lolzteam documentation
+
 <p align="left">
     <a href="https://docs.api.zelenka.guru/?forum"><img width="150" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
+
 <p align="left">
     <a href="https://docs.api.zelenka.guru/?market"><img width="150" src="https://lzt.market/styles/market/logo_by_DaWeed_X_KASTE.svg" alt="Material Bread logo"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.12 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.13 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
-![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
-darkgreen?style=flat-
-square&logo=qiwi&link=https%3A%2F%2Flzt.market%2Fbalance%2Ftransfer%3Fuser_id%3D2410024%26comment%3DThanks%2520for%2520creating%2520LolzteamApi%26amount%3D500)
+[![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
+darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/
+transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE) ## Installation
 You can install the library using pip: ```cmd pip install LolzteamApi ``` ##
 Usage Import the `LolzteamApi` module and create an instance of the
 `LolzteamApi` class to start using the API: ```python from LolzteamApi import
 LolzteamApi api = LolzteamApi(token='your_token') ``` ## Examples
 [Material_Bread_logo]
```

### Comparing `LolzteamApi-1.0.12/README.md` & `LolzteamApi-1.0.13/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 # Lolzteam Python API
+
 <p align="center">
     <a href="https://zelenka.guru/members/2410024"><img width="800" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
 
-![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-darkgreen?style=flat-square&logo=qiwi&link=https%3A%2F%2Flzt.market%2Fbalance%2Ftransfer%3Fuser_id%3D2410024%26comment%3DThanks%2520for%2520creating%2520LolzteamApi%26amount%3D500)
+[![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE)
 
 
 ## Installation
 
 You can install the library using pip:
 
@@ -26,20 +27,23 @@
 ```
 
 ## Examples
 
 <p align="left">
     <a href="https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/Examples/example.py"><img width="150" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
+
 <p align="left">
     <a href="https://github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/Examples/example_market.py"><img width="150" src="https://lzt.market/styles/market/logo_by_DaWeed_X_KASTE.svg" alt="Material Bread logo"></a>
 </p>
 
 
 ## Official Lolzteam documentation
+
 <p align="left">
     <a href="https://docs.api.zelenka.guru/?forum"><img width="150" src="https://zelenka.guru/styles/brand/download/logos/LolzTeam-Wordmark-Green.svg" alt="Material Bread logo"></a>
 </p>
+
 <p align="left">
     <a href="https://docs.api.zelenka.guru/?market"><img width="150" src="https://lzt.market/styles/market/logo_by_DaWeed_X_KASTE.svg" alt="Material Bread logo"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
  # Lolzteam Python API
                              [Material_Bread_logo]
-![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
-darkgreen?style=flat-
-square&logo=qiwi&link=https%3A%2F%2Flzt.market%2Fbalance%2Ftransfer%3Fuser_id%3D2410024%26comment%3DThanks%2520for%2520creating%2520LolzteamApi%26amount%3D500)
+[![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
+darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/
+transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE) ## Installation
 You can install the library using pip: ```cmd pip install LolzteamApi ``` ##
 Usage Import the `LolzteamApi` module and create an instance of the
 `LolzteamApi` class to start using the API: ```python from LolzteamApi import
 LolzteamApi api = LolzteamApi(token='your_token') ``` ## Examples
 [Material_Bread_logo]
```

### Comparing `LolzteamApi-1.0.12/setup.py` & `LolzteamApi-1.0.13/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-requirements = ["requests"]
+requirements = ["requests","beautifulsoup4"]
 
 setuptools.setup(
     name="LolzteamApi",
-    version="1.0.12",
+    version="1.0.13",
     author="AS7RID",
     author_email="as7ridwork@gmail.com",
     description="A library that contains all the methods of the Lolzteam API (Market/Forum)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AS7RIDENIED/Lolzteam_Python_Api",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=["Programming Language :: Python :: 3.11"],
     python_requires='>=3.6'
-)
+)
```

