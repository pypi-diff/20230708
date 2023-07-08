# Comparing `tmp/pysomneo-3.0.0a2.tar.gz` & `tmp/pysomneo-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysomneo-3.0.0a2.tar", last modified: Sat Jul  8 13:12:15 2023, max compression
+gzip compressed data, was "pysomneo-3.0.0a3.tar", last modified: Sat Jul  8 13:15:25 2023, max compression
```

## Comparing `pysomneo-3.0.0a2.tar` & `pysomneo-3.0.0a3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:12:15.356825 pysomneo-3.0.0a2/
--rw-rw-rw-   0        0        0    35802 2023-07-05 09:34:08.000000 pysomneo-3.0.0a2/LICENSE
--rw-rw-rw-   0        0        0    41813 2023-07-08 13:12:15.356825 pysomneo-3.0.0a2/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-07-05 09:34:08.000000 pysomneo-3.0.0a2/README.md
--rw-rw-rw-   0        0        0      775 2023-07-08 13:11:43.000000 pysomneo-3.0.0a2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-08 13:12:15.338908 pysomneo-3.0.0a2/pysomneo/
--rw-rw-rw-   0        0        0    22929 2023-07-08 13:11:37.000000 pysomneo-3.0.0a2/pysomneo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:12:15.355554 pysomneo-3.0.0a2/pysomneo.egg-info/
--rw-rw-rw-   0        0        0    41813 2023-07-08 13:12:15.000000 pysomneo-3.0.0a2/pysomneo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-07-08 13:12:15.000000 pysomneo-3.0.0a2/pysomneo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:12:15.000000 pysomneo-3.0.0a2/pysomneo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 13:12:15.000000 pysomneo-3.0.0a2/pysomneo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 13:12:15.357830 pysomneo-3.0.0a2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 13:15:25.616343 pysomneo-3.0.0a3/
+-rw-rw-rw-   0        0        0    35802 2023-07-05 09:34:08.000000 pysomneo-3.0.0a3/LICENSE
+-rw-rw-rw-   0        0        0    41813 2023-07-08 13:15:25.605312 pysomneo-3.0.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-07-05 09:34:08.000000 pysomneo-3.0.0a3/README.md
+-rw-rw-rw-   0        0        0      775 2023-07-08 13:14:56.000000 pysomneo-3.0.0a3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-08 13:15:25.587524 pysomneo-3.0.0a3/pysomneo/
+-rw-rw-rw-   0        0        0    22928 2023-07-08 13:14:43.000000 pysomneo-3.0.0a3/pysomneo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:15:25.604310 pysomneo-3.0.0a3/pysomneo.egg-info/
+-rw-rw-rw-   0        0        0    41813 2023-07-08 13:15:25.000000 pysomneo-3.0.0a3/pysomneo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-07-08 13:15:25.000000 pysomneo-3.0.0a3/pysomneo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:15:25.000000 pysomneo-3.0.0a3/pysomneo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 13:15:25.000000 pysomneo-3.0.0a3/pysomneo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:15:25.617314 pysomneo-3.0.0a3/setup.cfg
```

### Comparing `pysomneo-3.0.0a2/LICENSE` & `pysomneo-3.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysomneo-3.0.0a2/PKG-INFO` & `pysomneo-3.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysomneo
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: A library to communicate with the API of Philips Somneo.
 Author-email: Ruud van der Horst <pypi@mail.ruudvdhorst.nl>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pysomneo-3.0.0a2/pyproject.toml` & `pysomneo-3.0.0a3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "requests>=2.24.0",
     "urllib3>=1.26.5"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysomneo"
-version = "3.0.0alpha2"
+version = "3.0.0alpha3"
 authors = [
   { name="Ruud van der Horst", email="pypi@mail.ruudvdhorst.nl" },
 ]
 description = "A library to communicate with the API of Philips Somneo."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `pysomneo-3.0.0a2/pysomneo/__init__.py` & `pysomneo-3.0.0a3/pysomneo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -559,15 +559,15 @@
     def set_volume_player(self, volume: float):
         """Set the volume of the player (0..1)"""
         if volume < 0:
             volume = 0
         if volume > 1:
             volume = 1
 
-        self._put('wuplay', payload={'sdvol': volume * 24 + 1})
+        self._put('wuply', payload={'sdvol': volume * 24 + 1})
 
     def set_source_player(self, source: str | int):
         """Set the source of the player, either 'aux' or preset 1..5"""
         if source == 'aux' or 'AUX':
             self._put('wuply', payload={'sndv': 'aux'})
 
         elif source in range(1,6):
```

### Comparing `pysomneo-3.0.0a2/pysomneo.egg-info/PKG-INFO` & `pysomneo-3.0.0a3/pysomneo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysomneo
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: A library to communicate with the API of Philips Somneo.
 Author-email: Ruud van der Horst <pypi@mail.ruudvdhorst.nl>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

