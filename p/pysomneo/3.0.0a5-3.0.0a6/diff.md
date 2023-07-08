# Comparing `tmp/pysomneo-3.0.0a5.tar.gz` & `tmp/pysomneo-3.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysomneo-3.0.0a5.tar", last modified: Sat Jul  8 13:29:20 2023, max compression
+gzip compressed data, was "pysomneo-3.0.0a6.tar", last modified: Sat Jul  8 13:42:11 2023, max compression
```

## Comparing `pysomneo-3.0.0a5.tar` & `pysomneo-3.0.0a6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:29:20.765813 pysomneo-3.0.0a5/
--rw-rw-rw-   0        0        0    35802 2023-07-05 09:34:08.000000 pysomneo-3.0.0a5/LICENSE
--rw-rw-rw-   0        0        0    41813 2023-07-08 13:29:20.764815 pysomneo-3.0.0a5/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-07-05 09:34:08.000000 pysomneo-3.0.0a5/README.md
--rw-rw-rw-   0        0        0      775 2023-07-08 13:28:54.000000 pysomneo-3.0.0a5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-08 13:29:20.742257 pysomneo-3.0.0a5/pysomneo/
--rw-rw-rw-   0        0        0    23404 2023-07-08 13:28:46.000000 pysomneo-3.0.0a5/pysomneo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:29:20.763936 pysomneo-3.0.0a5/pysomneo.egg-info/
--rw-rw-rw-   0        0        0    41813 2023-07-08 13:29:20.000000 pysomneo-3.0.0a5/pysomneo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-07-08 13:29:20.000000 pysomneo-3.0.0a5/pysomneo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:29:20.000000 pysomneo-3.0.0a5/pysomneo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 13:29:20.000000 pysomneo-3.0.0a5/pysomneo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 13:29:20.766817 pysomneo-3.0.0a5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 13:42:11.075781 pysomneo-3.0.0a6/
+-rw-rw-rw-   0        0        0    35802 2023-07-05 09:34:08.000000 pysomneo-3.0.0a6/LICENSE
+-rw-rw-rw-   0        0        0    41813 2023-07-08 13:42:11.075781 pysomneo-3.0.0a6/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-07-05 09:34:08.000000 pysomneo-3.0.0a6/README.md
+-rw-rw-rw-   0        0        0      775 2023-07-08 13:41:43.000000 pysomneo-3.0.0a6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-08 13:42:11.056861 pysomneo-3.0.0a6/pysomneo/
+-rw-rw-rw-   0        0        0    23411 2023-07-08 13:41:26.000000 pysomneo-3.0.0a6/pysomneo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:42:11.073854 pysomneo-3.0.0a6/pysomneo.egg-info/
+-rw-rw-rw-   0        0        0    41813 2023-07-08 13:42:11.000000 pysomneo-3.0.0a6/pysomneo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-07-08 13:42:11.000000 pysomneo-3.0.0a6/pysomneo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:42:11.000000 pysomneo-3.0.0a6/pysomneo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 13:42:11.000000 pysomneo-3.0.0a6/pysomneo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:42:11.076782 pysomneo-3.0.0a6/setup.cfg
```

### Comparing `pysomneo-3.0.0a5/LICENSE` & `pysomneo-3.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `pysomneo-3.0.0a5/PKG-INFO` & `pysomneo-3.0.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysomneo
-Version: 3.0.0a5
+Version: 3.0.0a6
 Summary: A library to communicate with the API of Philips Somneo.
 Author-email: Ruud van der Horst <pypi@mail.ruudvdhorst.nl>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pysomneo-3.0.0a5/pyproject.toml` & `pysomneo-3.0.0a6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "requests>=2.24.0",
     "urllib3>=1.26.5"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysomneo"
-version = "3.0.0alpha5"
+version = "3.0.0alpha6"
 authors = [
   { name="Ruud van der Horst", email="pypi@mail.ruudvdhorst.nl" },
 ]
 description = "A library to communicate with the API of Philips Somneo."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `pysomneo-3.0.0a5/pysomneo/__init__.py` & `pysomneo-3.0.0a6/pysomneo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,21 +569,21 @@
 
     def set_source_player(self, source: str | int):
         """Set the source of the player, either 'aux' or preset 1..5"""
         if source == 'aux' or 'AUX':
             self._put('wuply', payload=
                       {'snddv': 'aux', 
                        'sndss': 0,
-                       'onoff': self.player['onoff'],
+                       #'onoff': self.player['onoff'],
                        'tempy': False
                        }
                 )
 
         elif source in range(1,6):
             self._put('wuply', payload=
                       {'snddv': 'fmr', 
-                       'sndch': source,
+                       'sndch': str(source),
                        'sndss': 0,
-                       'onoff': self.player['onoff'],
+                       #'onoff': self.player['onoff'],
                        'tempy': False
                        }
                 )
```

### Comparing `pysomneo-3.0.0a5/pysomneo.egg-info/PKG-INFO` & `pysomneo-3.0.0a6/pysomneo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysomneo
-Version: 3.0.0a5
+Version: 3.0.0a6
 Summary: A library to communicate with the API of Philips Somneo.
 Author-email: Ruud van der Horst <pypi@mail.ruudvdhorst.nl>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

