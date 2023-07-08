# Comparing `tmp/frankAllSkyCam-8.4.tar.gz` & `tmp/frankAllSkyCam-8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-8.4.tar", last modified: Sat Jun 10 18:10:05 2023, max compression
+gzip compressed data, was "frankAllSkyCam-8.5.tar", last modified: Sat Jul  8 16:56:34 2023, max compression
```

## Comparing `frankAllSkyCam-8.4.tar` & `frankAllSkyCam-8.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 18:10:05.422981 frankAllSkyCam-8.4/
--rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-06-10 18:10:05.422981 frankAllSkyCam-8.4/PKG-INFO
--rwxr--r--   0 pi        (1000) pi        (1000)     3200 2023-06-07 19:09:34.000000 frankAllSkyCam-8.4/README.txt
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 18:10:05.418981 frankAllSkyCam-8.4/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-06-10 18:09:48.000000 frankAllSkyCam-8.4/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     6068 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/allskycamdelete.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3999 2023-06-10 16:58:25.000000 frankAllSkyCam-8.4/frankAllSkyCam/config.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3505 2023-06-10 18:08:11.000000 frankAllSkyCam-8.4/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2431 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/drawtext.py
--rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/exposurecalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/fileManager.py
--rw-r--r--   0 pi        (1000) pi        (1000)      927 2023-06-10 16:58:11.000000 frankAllSkyCam-8.4/frankAllSkyCam/getextdata.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/imageHeader.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/index.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1295 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/logos.py
--rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/sqmexp.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)    16497 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/sqmreader.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-06-05 20:12:48.000000 frankAllSkyCam-8.4/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-06-07 21:13:55.000000 frankAllSkyCam-8.4/frankAllSkyCam/watchDog.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-10 18:10:05.422981 frankAllSkyCam-8.4/frankAllSkyCam.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-06-10 18:10:05.000000 frankAllSkyCam-8.4/frankAllSkyCam.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      746 2023-06-10 18:10:05.000000 frankAllSkyCam-8.4/frankAllSkyCam.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-10 18:10:05.000000 frankAllSkyCam-8.4/frankAllSkyCam.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       18 2023-06-10 18:10:05.000000 frankAllSkyCam-8.4/frankAllSkyCam.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2023-06-10 18:10:05.000000 frankAllSkyCam-8.4/frankAllSkyCam.egg-info/top_level.txt
--rwxrw-rw-   0 pi        (1000) pi        (1000)       79 2023-06-10 18:10:05.422981 frankAllSkyCam-8.4/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-06-10 18:09:36.000000 frankAllSkyCam-8.4/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-08 16:56:34.198360 frankAllSkyCam-8.5/
+-rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-07-08 16:56:34.198360 frankAllSkyCam-8.5/PKG-INFO
+-rwxr--r--   0 pi        (1000) pi        (1000)     3200 2023-06-07 19:09:34.000000 frankAllSkyCam-8.5/README.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-08 16:56:34.194360 frankAllSkyCam-8.5/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-07-08 16:56:09.000000 frankAllSkyCam-8.5/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     6139 2023-07-08 16:52:38.000000 frankAllSkyCam-8.5/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/allskycamdelete.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3999 2023-06-10 16:58:25.000000 frankAllSkyCam-8.5/frankAllSkyCam/config.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3505 2023-06-10 18:08:11.000000 frankAllSkyCam-8.5/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2431 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/drawtext.py
+-rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/exposurecalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/fileManager.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      927 2023-06-10 16:58:11.000000 frankAllSkyCam-8.5/frankAllSkyCam/getextdata.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/imageHeader.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/index.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1295 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/logos.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/sqmexp.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)    16497 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/sqmreader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-06-05 20:12:48.000000 frankAllSkyCam-8.5/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-06-07 21:13:55.000000 frankAllSkyCam-8.5/frankAllSkyCam/watchDog.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-08 16:56:34.198360 frankAllSkyCam-8.5/frankAllSkyCam.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-07-08 16:56:34.000000 frankAllSkyCam-8.5/frankAllSkyCam.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      746 2023-07-08 16:56:34.000000 frankAllSkyCam-8.5/frankAllSkyCam.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-07-08 16:56:34.000000 frankAllSkyCam-8.5/frankAllSkyCam.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       18 2023-07-08 16:56:34.000000 frankAllSkyCam-8.5/frankAllSkyCam.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       15 2023-07-08 16:56:34.000000 frankAllSkyCam-8.5/frankAllSkyCam.egg-info/top_level.txt
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       79 2023-07-08 16:56:34.198360 frankAllSkyCam-8.5/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-07-08 16:53:59.000000 frankAllSkyCam-8.5/setup.py
```

### Comparing `frankAllSkyCam-8.4/PKG-INFO` & `frankAllSkyCam-8.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: frankAllSkyCam
-Version: 8.4
+Version: 8.5
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.4.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.5.tar.gz
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
 Keywords: AllSkyCamera,Astronomy,AllSky
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `frankAllSkyCam-8.4/README.txt` & `frankAllSkyCam-8.5/README.txt`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/__main__.py` & `frankAllSkyCam-8.5/frankAllSkyCam/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 bottom_right_y = int(config['text_coords']['bottom_right_y'])
 top_center_x   = int(config['text_coords']['top_center_x'])
 top_center_y   = int(config['text_coords']['top_center_y'])
 
 text_positions = [[top_left_x,top_left_y],[top_right_x,top_right_y],[bottom_left_x,bottom_left_y],[bottom_right_x,bottom_right_y],[top_center_x,top_center_y]]
 
 et_use         = str(config['extra_text']['et_use'])
+et_data_file   = str(config['extra_text']['et_data_file'])
 et_x_pos       = int(config['extra_text']['et_x_pos'])
 et_y_pos       = int(config['extra_text']['et_y_pos'])
 et_font_size   = int(config['extra_text']['et_font_size'])
 et_font_colorR = int(config['extra_text']['et_font_colorR'])
 et_font_colorG = int(config['extra_text']['et_font_colorG'])
 et_font_colorB = int(config['extra_text']['et_font_colorB'])
 et_font_color = [et_font_colorR,et_font_colorG,et_font_colorB]
@@ -128,15 +129,15 @@
        os.system(command)
 
        print("Image captured")
 
        extra_text = [""]
        if et_use =="y":
           #extra_text needed
-          extra_string = getextdata.getData()
+          extra_string = getextdata.getData(et_data_file)
           extra_text = [extra_string, et_font_size, et_font_color, et_x_pos, et_y_pos]
 
        # print watermark
        drawtext.printWatermark(s, jpg_file_name, font_size, font_color, sqm_le, rotation, text_positions, extra_text)
 
        if logo_filename != "" or compass_filename != "":
           print(logo_filename)
```

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-8.5/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/config.py` & `frankAllSkyCam-8.5/frankAllSkyCam/config.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/crontab.py` & `frankAllSkyCam-8.5/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-8.5/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/exposurecalc.py` & `frankAllSkyCam-8.5/frankAllSkyCam/exposurecalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-8.5/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/getextdata.py` & `frankAllSkyCam-8.5/frankAllSkyCam/getextdata.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-8.5/frankAllSkyCam/imageHeader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/logos.py` & `frankAllSkyCam-8.5/frankAllSkyCam/logos.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/sqmreader.py` & `frankAllSkyCam-8.5/frankAllSkyCam/sqmreader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/startrail.py` & `frankAllSkyCam-8.5/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-8.5/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-8.5/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-8.5/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-8.5/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam.egg-info/PKG-INFO` & `frankAllSkyCam-8.5/frankAllSkyCam.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: frankAllSkyCam
-Version: 8.4
+Version: 8.5
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.4.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.5.tar.gz
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
 Keywords: AllSkyCamera,Astronomy,AllSky
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `frankAllSkyCam-8.4/frankAllSkyCam.egg-info/SOURCES.txt` & `frankAllSkyCam-8.5/frankAllSkyCam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.4/setup.py` & `frankAllSkyCam-8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'frankAllSkyCam',
   packages = ['frankAllSkyCam'],
-  version = '8.4',
+  version = '8.5',
   license='MIT',
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',
   author = 'Francesco Sferlazza',
   author_email = 'sferlazza@gmail.com',
   url = 'https://github.com/sferlix/frankAllSkyCam',
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.4.tar.gz',
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.5.tar.gz',
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],
   install_requires=[
           'pytz',
           'numpy',
           'pandas',
       ],
   classifiers=[
```

