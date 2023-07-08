# Comparing `tmp/pysomneo-3.0.0a1.tar.gz` & `tmp/pysomneo-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysomneo-3.0.0a1.tar", last modified: Sat Jul  8 13:08:59 2023, max compression
+gzip compressed data, was "pysomneo-3.0.0a2.tar", last modified: Sat Jul  8 13:12:15 2023, max compression
```

## Comparing `pysomneo-3.0.0a1.tar` & `pysomneo-3.0.0a2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:08:59.185231 pysomneo-3.0.0a1/
--rw-rw-rw-   0        0        0    35802 2023-07-05 09:34:08.000000 pysomneo-3.0.0a1/LICENSE
--rw-rw-rw-   0        0        0    41813 2023-07-08 13:08:59.183856 pysomneo-3.0.0a1/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-07-05 09:34:08.000000 pysomneo-3.0.0a1/README.md
--rw-rw-rw-   0        0        0      775 2023-07-08 13:07:57.000000 pysomneo-3.0.0a1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-08 13:08:59.168653 pysomneo-3.0.0a1/pysomneo/
--rw-rw-rw-   0        0        0    22933 2023-07-08 13:07:59.000000 pysomneo-3.0.0a1/pysomneo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:08:59.182852 pysomneo-3.0.0a1/pysomneo.egg-info/
--rw-rw-rw-   0        0        0    41813 2023-07-08 13:08:59.000000 pysomneo-3.0.0a1/pysomneo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-07-08 13:08:59.000000 pysomneo-3.0.0a1/pysomneo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:08:59.000000 pysomneo-3.0.0a1/pysomneo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 13:08:59.000000 pysomneo-3.0.0a1/pysomneo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 13:08:59.185773 pysomneo-3.0.0a1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 13:12:15.356825 pysomneo-3.0.0a2/
+-rw-rw-rw-   0        0        0    35802 2023-07-05 09:34:08.000000 pysomneo-3.0.0a2/LICENSE
+-rw-rw-rw-   0        0        0    41813 2023-07-08 13:12:15.356825 pysomneo-3.0.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-07-05 09:34:08.000000 pysomneo-3.0.0a2/README.md
+-rw-rw-rw-   0        0        0      775 2023-07-08 13:11:43.000000 pysomneo-3.0.0a2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-08 13:12:15.338908 pysomneo-3.0.0a2/pysomneo/
+-rw-rw-rw-   0        0        0    22929 2023-07-08 13:11:37.000000 pysomneo-3.0.0a2/pysomneo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:12:15.355554 pysomneo-3.0.0a2/pysomneo.egg-info/
+-rw-rw-rw-   0        0        0    41813 2023-07-08 13:12:15.000000 pysomneo-3.0.0a2/pysomneo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-07-08 13:12:15.000000 pysomneo-3.0.0a2/pysomneo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:12:15.000000 pysomneo-3.0.0a2/pysomneo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 13:12:15.000000 pysomneo-3.0.0a2/pysomneo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:12:15.357830 pysomneo-3.0.0a2/setup.cfg
```

### Comparing `pysomneo-3.0.0a1/LICENSE` & `pysomneo-3.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysomneo-3.0.0a1/PKG-INFO` & `pysomneo-3.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysomneo
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: A library to communicate with the API of Philips Somneo.
 Author-email: Ruud van der Horst <pypi@mail.ruudvdhorst.nl>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pysomneo-3.0.0a1/pysomneo/__init__.py` & `pysomneo-3.0.0a2/pysomneo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         data['temperature'] = self.temperature()
         data['humidity'] = self.humidity()
         data['luminance'] = self.luminance()
         data['noise'] = self.noise()
 
         data['player'] = dict()
         data['player']['state'] = bool(self.player['onoff'])
-        data['player']['volume'] = (float(self.light_data['sdvol']) - 1) / 24
+        data['player']['volume'] = (float(self.player['sdvol']) - 1) / 24
         if self.player['snddv'] == 'aux':
             data['player']['source'] = 'AUX'
         elif self.player['snddv'] == 'fmr':
             data['player']['source'] = 'FM ' + self.player['sndch']
 
 
         return data
```

### Comparing `pysomneo-3.0.0a1/pysomneo.egg-info/PKG-INFO` & `pysomneo-3.0.0a2/pysomneo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysomneo
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: A library to communicate with the API of Philips Somneo.
 Author-email: Ruud van der Horst <pypi@mail.ruudvdhorst.nl>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

