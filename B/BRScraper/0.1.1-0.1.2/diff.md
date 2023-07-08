# Comparing `tmp/BRScraper-0.1.1.tar.gz` & `tmp/BRScraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BRScraper-0.1.1.tar", last modified: Sat Jul  8 15:41:57 2023, max compression
+gzip compressed data, was "BRScraper-0.1.2.tar", last modified: Sat Jul  8 16:15:04 2023, max compression
```

## Comparing `BRScraper-0.1.1.tar` & `BRScraper-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 15:41:57.680000 BRScraper-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-07-08 15:41:57.677566 BRScraper-0.1.1/BRScraper.egg-info/
--rw-rw-rw-   0        0        0     3075 2023-07-08 15:41:57.000000 BRScraper-0.1.1/BRScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-08 15:41:57.000000 BRScraper-0.1.1/BRScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 15:41:57.000000 BRScraper-0.1.1/BRScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-08 15:41:57.000000 BRScraper-0.1.1/BRScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 15:41:57.000000 BRScraper-0.1.1/BRScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-03-12 19:02:09.000000 BRScraper-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3075 2023-07-08 15:41:57.680000 BRScraper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2438 2023-07-08 15:41:20.000000 BRScraper-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 15:41:57.680000 BRScraper-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1278 2023-07-08 15:40:57.000000 BRScraper-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:04.100072 BRScraper-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:03.810163 BRScraper-0.1.2/BRScraper/
+-rw-rw-rw-   0        0        0        0 2023-03-10 22:31:23.000000 BRScraper-0.1.2/BRScraper/__init__.py
+-rw-rw-rw-   0        0        0     2272 2023-03-10 20:51:27.000000 BRScraper-0.1.2/BRScraper/gleague.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:04.100072 BRScraper-0.1.2/BRScraper/international/
+-rw-rw-rw-   0        0        0        0 2023-03-10 22:31:23.000000 BRScraper-0.1.2/BRScraper/international/__init__.py
+-rw-rw-rw-   0        0        0     1856 2023-03-10 18:42:19.000000 BRScraper-0.1.2/BRScraper/international/aba.py
+-rw-rw-rw-   0        0        0     1860 2023-03-10 17:51:26.000000 BRScraper-0.1.2/BRScraper/international/acb.py
+-rw-rw-rw-   0        0        0     1840 2023-03-10 18:15:57.000000 BRScraper-0.1.2/BRScraper/international/cba.py
+-rw-rw-rw-   0        0        0     1832 2023-03-10 18:26:02.000000 BRScraper-0.1.2/BRScraper/international/eurocup.py
+-rw-rw-rw-   0        0        0     1844 2023-03-10 18:24:36.000000 BRScraper-0.1.2/BRScraper/international/euroleague.py
+-rw-rw-rw-   0        0        0     1884 2023-03-10 18:31:37.000000 BRScraper-0.1.2/BRScraper/international/greece.py
+-rw-rw-rw-   0        0        0     1884 2023-03-10 18:35:54.000000 BRScraper-0.1.2/BRScraper/international/israel.py
+-rw-rw-rw-   0        0        0     1888 2023-03-10 18:37:55.000000 BRScraper-0.1.2/BRScraper/international/italy.py
+-rw-rw-rw-   0        0        0     1872 2023-03-10 18:45:06.000000 BRScraper-0.1.2/BRScraper/international/lnb.py
+-rw-rw-rw-   0        0        0     1860 2023-03-10 18:33:12.000000 BRScraper-0.1.2/BRScraper/international/nbl.py
+-rw-rw-rw-   0        0        0     2052 2023-03-10 18:53:21.000000 BRScraper-0.1.2/BRScraper/international/olympics.py
+-rw-rw-rw-   0        0        0     1455 2023-03-10 20:35:32.000000 BRScraper-0.1.2/BRScraper/international/players.py
+-rw-rw-rw-   0        0        0     1848 2023-03-10 18:39:57.000000 BRScraper-0.1.2/BRScraper/international/russia.py
+-rw-rw-rw-   0        0        0     1884 2023-03-10 18:38:47.000000 BRScraper-0.1.2/BRScraper/international/turkey.py
+-rw-rw-rw-   0        0        0    14422 2023-07-08 11:42:44.000000 BRScraper-0.1.2/BRScraper/nba.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:15:03.867630 BRScraper-0.1.2/BRScraper.egg-info/
+-rw-rw-rw-   0        0        0     3126 2023-07-08 16:15:03.000000 BRScraper-0.1.2/BRScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      754 2023-07-08 16:15:03.000000 BRScraper-0.1.2/BRScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 16:15:03.000000 BRScraper-0.1.2/BRScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-08 16:15:03.000000 BRScraper-0.1.2/BRScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 16:15:03.000000 BRScraper-0.1.2/BRScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2023-03-12 19:02:09.000000 BRScraper-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3126 2023-07-08 16:15:04.100072 BRScraper-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2438 2023-07-08 15:44:34.000000 BRScraper-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 16:15:04.100072 BRScraper-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1329 2023-07-08 16:13:10.000000 BRScraper-0.1.2/setup.py
```

### Comparing `BRScraper-0.1.1/BRScraper.egg-info/PKG-INFO` & `BRScraper-0.1.2/BRScraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: BRScraper
-Version: 0.1.1
-Summary: Python module for Basketball Reference scraping and easy access to basketball data
+Version: 0.1.2
+Summary: Python module for Basketball Reference scraping and easy access to basketball data, including NBA, G League and international leagues
 Home-page: https://github.com/GabrielPastorello/BRScraper
 Author: Gabriel Speranza Pastorello
 Author-email: gabriel.pastorello01@gmail.com
 License: MIT
 Keywords: basketball reference,scraper,nba,wnba,gleague,basketball,international basketball
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,15 +31,15 @@
 
 # BRScraper
 
 Python package for easy access to basketball data through scraping of [Basketball Reference](https://www.basketball-reference.com/) website.
 
 This allows users to obtain statistics, standings, and scores for various seasons and phases of the following tournaments:
 - **NBA**
-- **G-League**
+- **G League**
 - **International Tournaments** (Olympics, EuroLeague, EuroCup and international leagues from: Spain, Australia, China, France, Greece, Israel, Italy, Turkey, Russia and ABA)
 
 ## Installing
 ### Via `pip`
 This library was written as an exercise for creating my first PyPi package. Hopefully you will find it valuable!
 Install with the following command:
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: BRScraper Version: 0.1.1 Summary: Python module for
-Basketball Reference scraping and easy access to basketball data Home-page:
-https://github.com/GabrielPastorello/BRScraper Author: Gabriel Speranza
-Pastorello Author-email: gabriel.pastorello01@gmail.com License: MIT Keywords:
-basketball reference,scraper,nba,wnba,gleague,basketball,international
-basketball Classifier: Programming Language :: Python :: 3 Classifier: License
-:: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Metadata-Version: 2.1 Name: BRScraper Version: 0.1.2 Summary: Python module for
+Basketball Reference scraping and easy access to basketball data, including
+NBA, G League and international leagues Home-page: https://github.com/
+GabrielPastorello/BRScraper Author: Gabriel Speranza Pastorello Author-email:
+gabriel.pastorello01@gmail.com License: MIT Keywords: basketball
+reference,scraper,nba,wnba,gleague,basketball,international basketball
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
 [https://github.com/GabrielPastorello/BRScraper/assets/57769272/cb95ffa0-0806-
                             4469-89bb-28ba6bc7ff00]
                        [pypi] [python_version] [license]
 # BRScraper Python package for easy access to basketball data through scraping
 of [Basketball Reference](https://www.basketball-reference.com/) website. This
 allows users to obtain statistics, standings, and scores for various seasons
-and phases of the following tournaments: - **NBA** - **G-League** -
+and phases of the following tournaments: - **NBA** - **G League** -
 **International Tournaments** (Olympics, EuroLeague, EuroCup and international
 leagues from: Spain, Australia, China, France, Greece, Israel, Italy, Turkey,
 Russia and ABA) ## Installing ### Via `pip` This library was written as an
 exercise for creating my first PyPi package. Hopefully you will find it
 valuable! Install with the following command: ``` pip install BRScraper ``` ##
 Documentation For documentation about the API methods refer to [the
 documentation](https://github.com/GabrielPastorello/BRScraper/blob/main/
```

### Comparing `BRScraper-0.1.1/LICENSE` & `BRScraper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BRScraper-0.1.1/PKG-INFO` & `BRScraper-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: BRScraper
-Version: 0.1.1
-Summary: Python module for Basketball Reference scraping and easy access to basketball data
+Version: 0.1.2
+Summary: Python module for Basketball Reference scraping and easy access to basketball data, including NBA, G League and international leagues
 Home-page: https://github.com/GabrielPastorello/BRScraper
 Author: Gabriel Speranza Pastorello
 Author-email: gabriel.pastorello01@gmail.com
 License: MIT
 Keywords: basketball reference,scraper,nba,wnba,gleague,basketball,international basketball
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,15 +31,15 @@
 
 # BRScraper
 
 Python package for easy access to basketball data through scraping of [Basketball Reference](https://www.basketball-reference.com/) website.
 
 This allows users to obtain statistics, standings, and scores for various seasons and phases of the following tournaments:
 - **NBA**
-- **G-League**
+- **G League**
 - **International Tournaments** (Olympics, EuroLeague, EuroCup and international leagues from: Spain, Australia, China, France, Greece, Israel, Italy, Turkey, Russia and ABA)
 
 ## Installing
 ### Via `pip`
 This library was written as an exercise for creating my first PyPi package. Hopefully you will find it valuable!
 Install with the following command:
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: BRScraper Version: 0.1.1 Summary: Python module for
-Basketball Reference scraping and easy access to basketball data Home-page:
-https://github.com/GabrielPastorello/BRScraper Author: Gabriel Speranza
-Pastorello Author-email: gabriel.pastorello01@gmail.com License: MIT Keywords:
-basketball reference,scraper,nba,wnba,gleague,basketball,international
-basketball Classifier: Programming Language :: Python :: 3 Classifier: License
-:: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Metadata-Version: 2.1 Name: BRScraper Version: 0.1.2 Summary: Python module for
+Basketball Reference scraping and easy access to basketball data, including
+NBA, G League and international leagues Home-page: https://github.com/
+GabrielPastorello/BRScraper Author: Gabriel Speranza Pastorello Author-email:
+gabriel.pastorello01@gmail.com License: MIT Keywords: basketball
+reference,scraper,nba,wnba,gleague,basketball,international basketball
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
 [https://github.com/GabrielPastorello/BRScraper/assets/57769272/cb95ffa0-0806-
                             4469-89bb-28ba6bc7ff00]
                        [pypi] [python_version] [license]
 # BRScraper Python package for easy access to basketball data through scraping
 of [Basketball Reference](https://www.basketball-reference.com/) website. This
 allows users to obtain statistics, standings, and scores for various seasons
-and phases of the following tournaments: - **NBA** - **G-League** -
+and phases of the following tournaments: - **NBA** - **G League** -
 **International Tournaments** (Olympics, EuroLeague, EuroCup and international
 leagues from: Spain, Australia, China, France, Greece, Israel, Italy, Turkey,
 Russia and ABA) ## Installing ### Via `pip` This library was written as an
 exercise for creating my first PyPi package. Hopefully you will find it
 valuable! Install with the following command: ``` pip install BRScraper ``` ##
 Documentation For documentation about the API methods refer to [the
 documentation](https://github.com/GabrielPastorello/BRScraper/blob/main/
```

### Comparing `BRScraper-0.1.1/README.md` & `BRScraper-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # BRScraper
 
 Python package for easy access to basketball data through scraping of [Basketball Reference](https://www.basketball-reference.com/) website.
 
 This allows users to obtain statistics, standings, and scores for various seasons and phases of the following tournaments:
 - **NBA**
-- **G-League**
+- **G League**
 - **International Tournaments** (Olympics, EuroLeague, EuroCup and international leagues from: Spain, Australia, China, France, Greece, Israel, Italy, Turkey, Russia and ABA)
 
 ## Installing
 ### Via `pip`
 This library was written as an exercise for creating my first PyPi package. Hopefully you will find it valuable!
 Install with the following command:
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 [https://github.com/GabrielPastorello/BRScraper/assets/57769272/cb95ffa0-0806-
                             4469-89bb-28ba6bc7ff00]
                        [pypi] [python_version] [license]
 # BRScraper Python package for easy access to basketball data through scraping
 of [Basketball Reference](https://www.basketball-reference.com/) website. This
 allows users to obtain statistics, standings, and scores for various seasons
-and phases of the following tournaments: - **NBA** - **G-League** -
+and phases of the following tournaments: - **NBA** - **G League** -
 **International Tournaments** (Olympics, EuroLeague, EuroCup and international
 leagues from: Spain, Australia, China, France, Greece, Israel, Italy, Turkey,
 Russia and ABA) ## Installing ### Via `pip` This library was written as an
 exercise for creating my first PyPi package. Hopefully you will find it
 valuable! Install with the following command: ``` pip install BRScraper ``` ##
 Documentation For documentation about the API methods refer to [the
 documentation](https://github.com/GabrielPastorello/BRScraper/blob/main/
```

### Comparing `BRScraper-0.1.1/setup.py` & `BRScraper-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
             name='BRScraper',
-            version='0.1.1',
-            description='Python module for Basketball Reference scraping and easy access to basketball data',
+            version='0.1.2',
+            description='Python module for Basketball Reference scraping and easy access to basketball data, including NBA, G League and international leagues',
             long_description=long_description,
             long_description_content_type="text/markdown",
             url='https://github.com/GabrielPastorello/BRScraper',
             author='Gabriel Speranza Pastorello',
             author_email='gabriel.pastorello01@gmail.com',
             license='MIT',
             packages=setuptools.find_packages(),
```

