# Comparing `tmp/threads-net-0.0.5.tar.gz` & `tmp/threads-net-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-net-0.0.5.tar", last modified: Fri Jul  7 19:46:31 2023, max compression
+gzip compressed data, was "threads-net-0.0.6.tar", last modified: Sat Jul  8 07:18:58 2023, max compression
```

## Comparing `threads-net-0.0.5.tar` & `threads-net-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:46:31.809211 threads-net-0.0.5/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-07 10:34:41.000000 threads-net-0.0.5/LICENSE
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.5/MANIFEST.in
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    44189 2023-07-07 19:46:31.809080 threads-net-0.0.5/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43338 2023-07-07 19:35:16.000000 threads-net-0.0.5/README.md
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:46:31.807798 threads-net-0.0.5/examples/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.5/examples/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      389 2023-07-07 18:52:22.000000 threads-net-0.0.5/examples/get_post.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      478 2023-07-07 18:47:05.000000 threads-net-0.0.5/examples/get_user.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      408 2023-07-07 18:40:46.000000 threads-net-0.0.5/examples/get_user_replies.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      410 2023-07-07 18:40:52.000000 threads-net-0.0.5/examples/get_user_threads.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      472 2023-07-07 19:07:00.000000 threads-net-0.0.5/examples/login.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:46:31.807905 threads-net-0.0.5/requirements/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       52 2023-07-07 19:45:44.000000 threads-net-0.0.5/requirements/project.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-07 19:46:31.809247 threads-net-0.0.5/setup.cfg
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1245 2023-07-07 19:46:30.000000 threads-net-0.0.5/setup.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:46:31.808118 threads-net-0.0.5/threads/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.5/threads/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     5379 2023-07-07 19:22:38.000000 threads-net-0.0.5/threads/main.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:46:31.808852 threads-net-0.0.5/threads_net.egg-info/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    44189 2023-07-07 19:46:31.000000 threads-net-0.0.5/threads_net.egg-info/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      412 2023-07-07 19:46:31.000000 threads-net-0.0.5/threads_net.egg-info/SOURCES.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-07 19:46:31.000000 threads-net-0.0.5/threads_net.egg-info/dependency_links.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       52 2023-07-07 19:46:31.000000 threads-net-0.0.5/threads_net.egg-info/requires.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 19:46:31.000000 threads-net-0.0.5/threads_net.egg-info/top_level.txt
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-08 07:18:58.696183 threads-net-0.0.6/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-07 10:34:41.000000 threads-net-0.0.6/LICENSE
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.6/MANIFEST.in
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    44616 2023-07-08 07:18:58.696060 threads-net-0.0.6/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43765 2023-07-08 07:17:53.000000 threads-net-0.0.6/README.md
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-08 07:18:58.694814 threads-net-0.0.6/examples/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.6/examples/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      242 2023-07-08 07:12:45.000000 threads-net-0.0.6/examples/get_post.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      478 2023-07-07 18:47:05.000000 threads-net-0.0.6/examples/get_user.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      261 2023-07-08 07:09:17.000000 threads-net-0.0.6/examples/get_user_replies.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      263 2023-07-08 07:09:25.000000 threads-net-0.0.6/examples/get_user_threads.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      472 2023-07-07 19:07:00.000000 threads-net-0.0.6/examples/login.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-08 07:18:58.694931 threads-net-0.0.6/requirements/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       52 2023-07-07 19:45:44.000000 threads-net-0.0.6/requirements/project.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-08 07:18:58.696220 threads-net-0.0.6/setup.cfg
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1245 2023-07-08 07:09:33.000000 threads-net-0.0.6/setup.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-08 07:18:58.695150 threads-net-0.0.6/threads/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.6/threads/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     5600 2023-07-08 07:11:18.000000 threads-net-0.0.6/threads/main.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-08 07:18:58.695856 threads-net-0.0.6/threads_net.egg-info/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    44616 2023-07-08 07:18:58.000000 threads-net-0.0.6/threads_net.egg-info/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      412 2023-07-08 07:18:58.000000 threads-net-0.0.6/threads_net.egg-info/SOURCES.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-08 07:18:58.000000 threads-net-0.0.6/threads_net.egg-info/dependency_links.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       52 2023-07-08 07:18:58.000000 threads-net-0.0.6/threads_net.egg-info/requires.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-08 07:18:58.000000 threads-net-0.0.6/threads_net.egg-info/top_level.txt
```

### Comparing `threads-net-0.0.5/LICENSE` & `threads-net-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-net-0.0.5/PKG-INFO` & `threads-net-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-net
-Version: 0.0.5
+Version: 0.0.6
 Summary: Threads (threads.net) Python API wrapper
 Home-page: https://github.com/dmytrostriletskyi/threads
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg)](https://stand-with-ukraine.pp.ua)
+
 Threads (threads.net) Python API wrapper
 
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
 
@@ -41,23 +43,26 @@
   * [Get Post](#get-post)
 
 ## Disclaimer
 
 * This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
   Utilizing private endpoints means simulating/pretending being a client (a mobile phone) «manually» creating all 
   needed credentials and a session. So, you might face `rate limits` or even be suspended if mess up with logining.
-  So use the project at your own risk until the normal `Threads` public `API` is available.
+  So use the project at your own risk until the normal `Threads` public `API` is available or this product become more
+  stable for such things.
 * For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
   is used because `Threads` are backed by `Instagram` and you do a login via it as well.
+* As the library use `Threads API ` private endpoints, they have no defined model for support and backward compatibility. 
+* So, some methods might end up not working until the library maintainers find out hot to fix it.
 
 ## Getting started
 
 ### How to install
 
-Install the project with the following command using `pip3`:
+Install the library with the following command using `pip3`:
 
 ```bash
 $ pip3 install threads-net
 ```
 
 ### Initialization
```

### Comparing `threads-net-0.0.5/README.md` & `threads-net-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg)](https://stand-with-ukraine.pp.ua)
+
 Threads (threads.net) Python API wrapper
 
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
 
@@ -19,23 +21,26 @@
   * [Get Post](#get-post)
 
 ## Disclaimer
 
 * This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
   Utilizing private endpoints means simulating/pretending being a client (a mobile phone) «manually» creating all 
   needed credentials and a session. So, you might face `rate limits` or even be suspended if mess up with logining.
-  So use the project at your own risk until the normal `Threads` public `API` is available.
+  So use the project at your own risk until the normal `Threads` public `API` is available or this product become more
+  stable for such things.
 * For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
   is used because `Threads` are backed by `Instagram` and you do a login via it as well.
+* As the library use `Threads API ` private endpoints, they have no defined model for support and backward compatibility. 
+* So, some methods might end up not working until the library maintainers find out hot to fix it.
 
 ## Getting started
 
 ### How to install
 
-Install the project with the following command using `pip3`:
+Install the library with the following command using `pip3`:
 
 ```bash
 $ pip3 install threads-net
 ```
 
 ### Initialization
```

### Comparing `threads-net-0.0.5/setup.py` & `threads-net-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('README.md', 'r', encoding='utf-8') as read_me:
     long_description = read_me.read()
 
 with open('requirements/project.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
-    version='0.0.5',
+    version='0.0.6',
     name='threads-net',
     description='Threads (threads.net) Python API wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dmytrostriletskyi/threads',
     license='MIT',
     author='Dmytro Striletskyi',
```

### Comparing `threads-net-0.0.5/threads/main.py` & `threads-net-0.0.6/threads/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,21 +154,26 @@
         Get a post.
 
         Arguments:
             id (int): a post's identifier.
         """
         response = requests.post(
             url=self.THREADS_API_URL,
-            headers=self.headers,
+            headers={
+                'Content-Type': 'application/x-www-form-urlencoded',
+                'X-IG-App-ID': '238260118697367',
+                'X-FB-LSD': self.temporary_token,
+                'Sec-Fetch-Site': 'same-origin',
+            },
             data={
                 'lsd': self.token,
                 'variables': json.dumps({
                     'postID': id,
                 }),
-                'doc_id': '5587632691339264',
+                'doc_id': '6529829603744567',
             },
         )
 
         return response.json()
 
     def set_proxy(self, dsn: str):
         """
```

### Comparing `threads-net-0.0.5/threads_net.egg-info/PKG-INFO` & `threads-net-0.0.6/threads_net.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-net
-Version: 0.0.5
+Version: 0.0.6
 Summary: Threads (threads.net) Python API wrapper
 Home-page: https://github.com/dmytrostriletskyi/threads
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg)](https://stand-with-ukraine.pp.ua)
+
 Threads (threads.net) Python API wrapper
 
 [![PyPI license](https://img.shields.io/pypi/l/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/threads-net.svg)](https://pypi.python.org/pypi/threads-net/)
 
 Table of content:
 
@@ -41,23 +43,26 @@
   * [Get Post](#get-post)
 
 ## Disclaimer
 
 * This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
   Utilizing private endpoints means simulating/pretending being a client (a mobile phone) «manually» creating all 
   needed credentials and a session. So, you might face `rate limits` or even be suspended if mess up with logining.
-  So use the project at your own risk until the normal `Threads` public `API` is available.
+  So use the project at your own risk until the normal `Threads` public `API` is available or this product become more
+  stable for such things.
 * For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
   is used because `Threads` are backed by `Instagram` and you do a login via it as well.
+* As the library use `Threads API ` private endpoints, they have no defined model for support and backward compatibility. 
+* So, some methods might end up not working until the library maintainers find out hot to fix it.
 
 ## Getting started
 
 ### How to install
 
-Install the project with the following command using `pip3`:
+Install the library with the following command using `pip3`:
 
 ```bash
 $ pip3 install threads-net
 ```
 
 ### Initialization
```

