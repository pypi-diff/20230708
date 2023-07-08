# Comparing `tmp/LolzteamApi-1.0.13.tar.gz` & `tmp/LolzteamApi-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LolzteamApi-1.0.13.tar", last modified: Sat Jul  8 01:34:04 2023, max compression
+gzip compressed data, was "LolzteamApi-1.0.14.tar", last modified: Sat Jul  8 01:48:20 2023, max compression
```

## Comparing `LolzteamApi-1.0.13.tar` & `LolzteamApi-1.0.14.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 01:34:04.287033 LolzteamApi-1.0.13/
--rw-rw-rw-   0        0        0     1089 2023-07-07 23:34:42.000000 LolzteamApi-1.0.13/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-08 01:34:04.270642 LolzteamApi-1.0.13/LolzteamApi/
--rw-rw-rw-   0        0        0   163270 2023-07-07 21:04:12.000000 LolzteamApi-1.0.13/LolzteamApi/LolzteamApi.py
--rw-rw-rw-   0        0        0      111 2023-07-08 00:37:47.000000 LolzteamApi-1.0.13/LolzteamApi/__init__.py
--rw-rw-rw-   0        0        0      893 2023-07-08 00:37:17.000000 LolzteamApi-1.0.13/LolzteamApi/check_updates.py
-drwxrwxrwx   0        0        0        0 2023-07-08 01:34:04.279199 LolzteamApi-1.0.13/LolzteamApi.egg-info/
--rw-rw-rw-   0        0        0     2260 2023-07-08 01:34:04.000000 LolzteamApi-1.0.13/LolzteamApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-08 01:34:04.000000 LolzteamApi-1.0.13/LolzteamApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 01:34:04.000000 LolzteamApi-1.0.13/LolzteamApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-08 01:34:04.000000 LolzteamApi-1.0.13/LolzteamApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-08 01:34:04.000000 LolzteamApi-1.0.13/LolzteamApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2260 2023-07-08 01:34:04.282834 LolzteamApi-1.0.13/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-07-07 23:34:42.000000 LolzteamApi-1.0.13/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 01:34:04.287033 LolzteamApi-1.0.13/setup.cfg
--rw-rw-rw-   0        0        0      689 2023-07-08 01:33:44.000000 LolzteamApi-1.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 01:48:20.551369 LolzteamApi-1.0.14/
+-rw-rw-rw-   0        0        0     1089 2023-07-07 23:34:42.000000 LolzteamApi-1.0.14/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-08 01:48:20.530579 LolzteamApi-1.0.14/LolzteamApi/
+-rw-rw-rw-   0        0        0   163270 2023-07-07 21:04:12.000000 LolzteamApi-1.0.14/LolzteamApi/LolzteamApi.py
+-rw-rw-rw-   0        0        0      111 2023-07-08 01:36:03.000000 LolzteamApi-1.0.14/LolzteamApi/__init__.py
+-rw-rw-rw-   0        0        0     1121 2023-07-08 01:42:28.000000 LolzteamApi-1.0.14/LolzteamApi/check_updates.py
+drwxrwxrwx   0        0        0        0 2023-07-08 01:48:20.551369 LolzteamApi-1.0.14/LolzteamApi.egg-info/
+-rw-rw-rw-   0        0        0     2260 2023-07-08 01:48:20.000000 LolzteamApi-1.0.14/LolzteamApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-08 01:48:20.000000 LolzteamApi-1.0.14/LolzteamApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 01:48:20.000000 LolzteamApi-1.0.14/LolzteamApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-08 01:48:20.000000 LolzteamApi-1.0.14/LolzteamApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-08 01:48:20.000000 LolzteamApi-1.0.14/LolzteamApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2260 2023-07-08 01:48:20.551369 LolzteamApi-1.0.14/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-07-07 23:34:42.000000 LolzteamApi-1.0.14/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 01:48:20.551369 LolzteamApi-1.0.14/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-07-08 01:42:28.000000 LolzteamApi-1.0.14/setup.py
```

### Comparing `LolzteamApi-1.0.13/LICENSE` & `LolzteamApi-1.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.13/LolzteamApi/LolzteamApi.py` & `LolzteamApi-1.0.14/LolzteamApi/LolzteamApi.py`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.13/LolzteamApi/check_updates.py` & `LolzteamApi-1.0.14/LolzteamApi/check_updates.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 from bs4 import BeautifulSoup
 import requests
 
 
 def check_for_new_version():
     current_version = version('LolzteamApi')
     response = requests.get("https://pypi.org/project/LolzteamApi/")
-    newest_version = BeautifulSoup(response.text, 'html.parser').select(selector="#content > div.banner > div > div.package-header__left > h1")[0].text.replace("LolzteamApi","").replace(" ", "").replace("\n","")
-    if current_version == newest_version:
+    newest_version = BeautifulSoup(response.text, 'html.parser').select(
+        selector="#content > div.banner > div > div.package-header__left > h1")[0].text.replace("LolzteamApi",
+                                                                                                "").replace(" ",
+                                                                                                            "").replace(
+        "\n", "")
+    if current_version != newest_version:
         print(f"Your version of LolzteamApi is outdated.")
         print(f"It has problems that have been solved in the new version")
         print(f"Your version:   {current_version}")
         print(f"Newest version: {newest_version}")
         print()
         print(f"You can update your package using the command below")
         print(f"pip install LolzteamApi --upgrade")
```

### Comparing `LolzteamApi-1.0.13/LolzteamApi.egg-info/PKG-INFO` & `LolzteamApi-1.0.14/LolzteamApi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.13
+Version: 1.0.14
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.13 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.14 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.13/PKG-INFO` & `LolzteamApi-1.0.14/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.13
+Version: 1.0.14
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.13 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.14 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.13/README.md` & `LolzteamApi-1.0.14/README.md`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.13/setup.py` & `LolzteamApi-1.0.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import setuptools
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-requirements = ["requests","beautifulsoup4"]
+requirements = ["requests", "beautifulsoup4"]
 
 setuptools.setup(
     name="LolzteamApi",
-    version="1.0.13",
+    version="1.0.14",
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

