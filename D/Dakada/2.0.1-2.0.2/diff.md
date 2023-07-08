# Comparing `tmp/Dakada-2.0.1.tar.gz` & `tmp/Dakada-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Dakada-2.0.1.tar", last modified: Sat Jul  8 03:20:25 2023, max compression
+gzip compressed data, was "dist\Dakada-2.0.2.tar", last modified: Sat Jul  8 03:22:37 2023, max compression
```

## Comparing `Dakada-2.0.1.tar` & `Dakada-2.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 03:20:25.000000 Dakada-2.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-08 03:20:25.000000 Dakada-2.0.1/Dakada.egg-info/
--rw-rw-rw-   0        0        0      648 2023-07-08 03:20:25.000000 Dakada-2.0.1/Dakada.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-07-08 03:20:25.000000 Dakada-2.0.1/Dakada.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 03:20:25.000000 Dakada-2.0.1/Dakada.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-08 03:20:25.000000 Dakada-2.0.1/Dakada.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-08 03:20:25.000000 Dakada-2.0.1/Dakada.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-07-08 03:20:25.000000 Dakada-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8226 2023-07-08 03:10:59.000000 Dakada-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 03:20:25.000000 Dakada-2.0.1/dakada/
--rw-rw-rw-   0        0        0    11088 2023-07-08 03:20:04.000000 Dakada-2.0.1/dakada/Dakada.py
--rw-rw-rw-   0        0        0     1194 2023-06-21 12:25:24.000000 Dakada-2.0.1/dakada/User.py
--rw-rw-rw-   0        0        0        0 2023-06-18 08:03:16.000000 Dakada-2.0.1/dakada/__init__.py
--rw-rw-rw-   0        0        0     1823 2023-06-20 13:19:04.000000 Dakada-2.0.1/dakada/admin.py
--rw-rw-rw-   0        0        0      119 2023-07-08 02:24:49.000000 Dakada-2.0.1/dakada/blueprint.py
--rw-rw-rw-   0        0        0      547 2023-06-18 08:21:29.000000 Dakada-2.0.1/dakada/cookie.py
--rw-rw-rw-   0        0        0      497 2023-06-20 12:22:16.000000 Dakada-2.0.1/dakada/render.py
--rw-rw-rw-   0        0        0      256 2023-07-08 02:24:11.000000 Dakada-2.0.1/dakada/startproject.py
--rw-rw-rw-   0        0        0       42 2023-07-08 03:20:25.000000 Dakada-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3830 2023-07-08 03:19:38.000000 Dakada-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:22:37.000000 Dakada-2.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-08 03:22:36.000000 Dakada-2.0.2/Dakada.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-07-08 03:22:36.000000 Dakada-2.0.2/Dakada.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-07-08 03:22:36.000000 Dakada-2.0.2/Dakada.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 03:22:36.000000 Dakada-2.0.2/Dakada.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 03:22:36.000000 Dakada-2.0.2/Dakada.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 03:22:36.000000 Dakada-2.0.2/Dakada.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2023-07-08 03:22:37.000000 Dakada-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8226 2023-07-08 03:10:59.000000 Dakada-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 03:22:36.000000 Dakada-2.0.2/dakada/
+-rw-rw-rw-   0        0        0    11088 2023-07-08 03:22:04.000000 Dakada-2.0.2/dakada/Dakada.py
+-rw-rw-rw-   0        0        0     1194 2023-06-21 12:25:24.000000 Dakada-2.0.2/dakada/User.py
+-rw-rw-rw-   0        0        0        0 2023-06-18 08:03:16.000000 Dakada-2.0.2/dakada/__init__.py
+-rw-rw-rw-   0        0        0     1823 2023-06-20 13:19:04.000000 Dakada-2.0.2/dakada/admin.py
+-rw-rw-rw-   0        0        0      119 2023-07-08 02:24:49.000000 Dakada-2.0.2/dakada/blueprint.py
+-rw-rw-rw-   0        0        0      547 2023-06-18 08:21:29.000000 Dakada-2.0.2/dakada/cookie.py
+-rw-rw-rw-   0        0        0      497 2023-06-20 12:22:16.000000 Dakada-2.0.2/dakada/render.py
+-rw-rw-rw-   0        0        0      256 2023-07-08 02:24:11.000000 Dakada-2.0.2/dakada/startproject.py
+-rw-rw-rw-   0        0        0       42 2023-07-08 03:22:37.000000 Dakada-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3830 2023-07-08 03:21:43.000000 Dakada-2.0.2/setup.py
```

### Comparing `Dakada-2.0.1/Dakada.egg-info/PKG-INFO` & `Dakada-2.0.2/Dakada.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dakada
-Version: 2.0.1
+Version: 2.0.2
 Summary: A web framework by Dakada CN
 Home-page: https://github.com/dakadayyds/dakadaWeb
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `Dakada-2.0.1/PKG-INFO` & `Dakada-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dakada
-Version: 2.0.1
+Version: 2.0.2
 Summary: A web framework by Dakada CN
 Home-page: https://github.com/dakadayyds/dakadaWeb
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `Dakada-2.0.1/README.md` & `Dakada-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Dakada-2.0.1/dakada/Dakada.py` & `Dakada-2.0.2/dakada/Dakada.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
             http=make_server(str(self.host),self.port,app)
             print("OK")
             print("starting cookiehandler...")
             t=threading.Thread(target=cookie)
             t.setDaemon(True)
             t.start()
             print("OK")
-            print("Dakada(ver 2.0.1) is running!")
+            print("Dakada(ver 2.0.2) is running!")
             if self.host=='':
                 print("View at:http://localhost:"+str(self.port))
             else:
                 print("View at:http://"+self.host+":"+str(self.port))
             http.serve_forever()
         except KeyboardInterrupt:
             print("server exit")
```

### Comparing `Dakada-2.0.1/dakada/User.py` & `Dakada-2.0.2/dakada/User.py`

 * *Files identical despite different names*

### Comparing `Dakada-2.0.1/dakada/admin.py` & `Dakada-2.0.2/dakada/admin.py`

 * *Files identical despite different names*

### Comparing `Dakada-2.0.1/dakada/cookie.py` & `Dakada-2.0.2/dakada/cookie.py`

 * *Files identical despite different names*

### Comparing `Dakada-2.0.1/setup.py` & `Dakada-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'Dakada'
 DESCRIPTION = 'A web framework by Dakada CN'
 URL = 'https://github.com/dakadayyds/dakadaWeb'
 EMAIL = 's75uy1e@dingtalk.com'
 AUTHOR = 'dakada'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '2.0.1'
+VERSION = '2.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'jinja2'
 ]
 
 # What packages are optional?
```

