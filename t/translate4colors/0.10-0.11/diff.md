# Comparing `tmp/translate4colors-0.10.tar.gz` & `tmp/translate4colors-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translate4colors-0.10.tar", last modified: Sat Jul  8 00:50:23 2023, max compression
+gzip compressed data, was "translate4colors-0.11.tar", last modified: Sat Jul  8 01:22:04 2023, max compression
```

## Comparing `translate4colors-0.10.tar` & `translate4colors-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 00:50:23.586587 translate4colors-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-08 00:50:05.000000 translate4colors-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      119 2023-07-08 00:50:04.000000 translate4colors-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     4968 2023-07-08 00:50:23.586587 translate4colors-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     4332 2023-07-08 00:49:27.000000 translate4colors-0.10/README.md
--rw-rw-rw-   0        0        0       85 2023-07-08 00:50:23.587584 translate4colors-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1506 2023-07-08 00:50:19.000000 translate4colors-0.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 00:50:23.583595 translate4colors-0.10/translate4colors/
--rw-rw-rw-   0        0        0     4332 2023-07-08 00:49:27.000000 translate4colors-0.10/translate4colors/README.MD
--rw-rw-rw-   0        0        0     6270 2023-07-08 00:43:04.000000 translate4colors-0.10/translate4colors/__init__.py
--rw-rw-rw-   0        0        0      103 2023-07-08 00:50:19.000000 translate4colors-0.10/translate4colors/requirements.txt
--rw-rw-rw-   0        0        0    42389 2023-07-08 00:50:19.000000 translate4colors-0.10/translate4colors/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-08 00:50:23.585591 translate4colors-0.10/translate4colors.egg-info/
--rw-rw-rw-   0        0        0     4968 2023-07-08 00:50:23.000000 translate4colors-0.10/translate4colors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-08 00:50:23.000000 translate4colors-0.10/translate4colors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 00:50:23.000000 translate4colors-0.10/translate4colors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-07-08 00:50:23.000000 translate4colors-0.10/translate4colors.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 00:50:23.000000 translate4colors-0.10/translate4colors.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 01:22:04.391298 translate4colors-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-08 01:21:55.000000 translate4colors-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      119 2023-07-08 01:21:54.000000 translate4colors-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     4968 2023-07-08 01:22:04.391298 translate4colors-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     4332 2023-07-08 00:49:27.000000 translate4colors-0.11/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-08 01:22:04.392296 translate4colors-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1506 2023-07-08 01:22:03.000000 translate4colors-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 01:22:04.388307 translate4colors-0.11/translate4colors/
+-rw-rw-rw-   0        0        0     4332 2023-07-08 00:49:27.000000 translate4colors-0.11/translate4colors/README.MD
+-rw-rw-rw-   0        0        0     6271 2023-07-08 01:19:43.000000 translate4colors-0.11/translate4colors/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-07-08 01:22:03.000000 translate4colors-0.11/translate4colors/requirements.txt
+-rw-rw-rw-   0        0        0    42389 2023-07-08 01:22:03.000000 translate4colors-0.11/translate4colors/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-08 01:22:04.390301 translate4colors-0.11/translate4colors.egg-info/
+-rw-rw-rw-   0        0        0     4968 2023-07-08 01:22:04.000000 translate4colors-0.11/translate4colors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-08 01:22:04.000000 translate4colors-0.11/translate4colors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 01:22:04.000000 translate4colors-0.11/translate4colors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-07-08 01:22:04.000000 translate4colors-0.11/translate4colors.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 01:22:04.000000 translate4colors-0.11/translate4colors.egg-info/top_level.txt
```

### Comparing `translate4colors-0.10/LICENSE.rst` & `translate4colors-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `translate4colors-0.10/PKG-INFO` & `translate4colors-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate4colors
-Version: 0.10
+Version: 0.11
 Summary: automates text translation using Google Translate
 Home-page: https://github.com/hansalemaos/translate4colors
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: google,translate
 Classifier: Development Status :: 4 - Beta
```

### Comparing `translate4colors-0.10/README.md` & `translate4colors-0.11/README.md`

 * *Files identical despite different names*

### Comparing `translate4colors-0.10/setup.py` & `translate4colors-0.11/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''automates text translation using Google Translate'''
 
 # Setting up
 setup(
     name="translate4colors",
     version=VERSION,
     license='MIT',
```

### Comparing `translate4colors-0.10/translate4colors/README.MD` & `translate4colors-0.11/translate4colors/README.MD`

 * *Files identical despite different names*

### Comparing `translate4colors-0.10/translate4colors/__init__.py` & `translate4colors-0.11/translate4colors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         self.quit_translator(soft_kill_first=True)
 
     def _chunk(self, text):
         return wrapre(
             " ".join([g for x in text.splitlines() if (g := x.strip())]),
             blocksize=self.maxchars,
             regexsep=r"\.",
-            raisewhenlonger=True,
+            raisewhenlonger=False,
             removenewlines_from_result=True,
         )
 
     def _get_google_link(self, s):
         return f"https://translate.google.com/?sl={self.src}&tl={self.dst}&text={urllib.parse.quote(s)}&op=translate"
 
     def quit_translator(self, soft_kill_first=True):
```

### Comparing `translate4colors-0.10/translate4colors/thirdparty.json` & `translate4colors-0.11/translate4colors/thirdparty.json`

 * *Files identical despite different names*

### Comparing `translate4colors-0.10/translate4colors.egg-info/PKG-INFO` & `translate4colors-0.11/translate4colors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate4colors
-Version: 0.10
+Version: 0.11
 Summary: automates text translation using Google Translate
 Home-page: https://github.com/hansalemaos/translate4colors
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: google,translate
 Classifier: Development Status :: 4 - Beta
```

