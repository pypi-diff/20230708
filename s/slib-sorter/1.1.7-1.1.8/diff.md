# Comparing `tmp/slib-sorter-1.1.7.tar.gz` & `tmp/slib-sorter-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.1.7.tar", last modified: Sat Jul  8 03:06:46 2023, max compression
+gzip compressed data, was "slib-sorter-1.1.8.tar", last modified: Sat Jul  8 03:19:23 2023, max compression
```

## Comparing `slib-sorter-1.1.7.tar` & `slib-sorter-1.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 03:06:46.027312 slib-sorter-1.1.7/
--rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     2291 2023-07-08 03:06:46.027312 slib-sorter-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 03:06:46.027312 slib-sorter-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     4378 2023-07-08 03:06:33.000000 slib-sorter-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:06:46.018277 slib-sorter-1.1.7/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2291 2023-07-08 03:06:45.000000 slib-sorter-1.1.7/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 03:06:45.000000 slib-sorter-1.1.7/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 03:06:45.000000 slib-sorter-1.1.7/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 03:06:45.000000 slib-sorter-1.1.7/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 03:06:45.000000 slib-sorter-1.1.7/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 03:06:45.000000 slib-sorter-1.1.7/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 03:06:46.026274 slib-sorter-1.1.7/src/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.7/src/__init__.py
--rw-rw-rw-   0        0        0    72616 2023-07-08 03:05:43.000000 slib-sorter-1.1.7/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:19:23.344411 slib-sorter-1.1.8/
+-rw-rw-rw-   0        0        0    11558 2023-07-07 20:03:54.000000 slib-sorter-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2291 2023-07-08 03:19:23.344411 slib-sorter-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-07-07 20:03:54.000000 slib-sorter-1.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-08 03:19:23.344411 slib-sorter-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     4378 2023-07-08 03:17:29.000000 slib-sorter-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:19:23.334402 slib-sorter-1.1.8/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     2291 2023-07-08 03:19:23.000000 slib-sorter-1.1.8/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-08 03:19:23.000000 slib-sorter-1.1.8/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 03:19:23.000000 slib-sorter-1.1.8/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 03:19:23.000000 slib-sorter-1.1.8/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 03:19:23.000000 slib-sorter-1.1.8/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-08 03:19:23.000000 slib-sorter-1.1.8/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 03:19:23.343401 slib-sorter-1.1.8/src/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:10:46.000000 slib-sorter-1.1.8/src/__init__.py
+-rw-rw-rw-   0        0        0    72626 2023-07-08 03:18:42.000000 slib-sorter-1.1.8/src/slib_sorter.py
```

### Comparing `slib-sorter-1.1.7/LICENSE` & `slib-sorter-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.7/PKG-INFO` & `slib-sorter-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.7
+Version: 1.1.8
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.1.7/README.md` & `slib-sorter-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.1.7/setup.py` & `slib-sorter-1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         importlib.reload(settings_file)
 def install():
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="slib-sorter",
-        version="1.1.7",
+        version="1.1.8",
         author="Lukas Hübinger",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.1.7/slib_sorter.egg-info/PKG-INFO` & `slib-sorter-1.1.8/slib_sorter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slib-sorter
-Version: 1.1.7
+Version: 1.1.8
 Summary: A Python package for sorting Sample Libraries
 Home-page: https://github.com/nrdrch/slib-sorter
 Author: Lukas Hübinger
 Author-email: fettkindasindauchoke@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `slib-sorter-1.1.7/src/slib_sorter.py` & `slib-sorter-1.1.8/src/slib_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         [string]$CustomInput
     )
     $argsString = $CustomInput -join "' '"
     $pythonScript = '{source_file}'
     python3 $pythonScript $argsString
 }}
     '''
-    with open(powershell_script_file, 'a') as f:
-        f.write(script_content)
+    #with open(powershell_script_file, 'a') as f:
+    #    f.write(script_content)
     
     if not os.path.exists(settings_folder):
         os.makedirs(settings_folder)
     default_config = f'''
 {{
     "Foregroud Color 1": "white",
     "Top Bar Color": "dark_grey",
@@ -87,22 +87,22 @@
     "Command On Startup": "cls" 
 }}
     '''
     with open(settings_file, 'w') as f:
         f.write(default_config)
     with open(settings_file, 'r') as file:
         settings_file = json.load(file)
-    profile_path = os.path.expanduser("~/Documents/WindowsPowerShell/Microsoft.PowerShell_profile.ps1")
-    with open(profile_path, 'r') as f:
-        profile_content = f.read()
-        if f"Import-Module -DisableNameChecking \"{powershell_script_file}\"" in profile_content:
-            pass
-        else:
-            with open(profile_path, 'a') as f:
-                f.write(f"\nImport-Module -DisableNameChecking \"{powershell_script_file}\"")
+    #profile_path = os.path.expanduser("~/Documents/WindowsPowerShell/Microsoft.PowerShell_profile.ps1")
+    #with open(profile_path, 'r') as f:
+    #    profile_content = f.read()
+    #    if f"Import-Module -DisableNameChecking \"{powershell_script_file}\"" in profile_content:
+    #        pass
+    #    else:
+    #        with open(profile_path, 'a') as f:
+    #            f.write(f"\nImport-Module -DisableNameChecking \"{powershell_script_file}\"")
     try:
         if settings.get("Run Shell Command On Startup", True):
             CmdOnStartup = settings.get("Command On Startup")
             os.system(CmdOnStartup)
         else:
             pass
     except:
```

