# Comparing `tmp/threads-net-0.0.4.tar.gz` & `tmp/threads-net-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-net-0.0.4.tar", last modified: Fri Jul  7 19:24:14 2023, max compression
+gzip compressed data, was "threads-net-0.0.5.tar", last modified: Fri Jul  7 19:46:31 2023, max compression
```

## Comparing `threads-net-0.0.4.tar` & `threads-net-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:24:14.914698 threads-net-0.0.4/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-07 10:34:41.000000 threads-net-0.0.4/LICENSE
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.4/MANIFEST.in
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43935 2023-07-07 19:24:14.914590 threads-net-0.0.4/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43084 2023-07-07 19:21:59.000000 threads-net-0.0.4/README.md
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:24:14.913622 threads-net-0.0.4/examples/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.4/examples/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      389 2023-07-07 18:52:22.000000 threads-net-0.0.4/examples/get_post.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      478 2023-07-07 18:47:05.000000 threads-net-0.0.4/examples/get_user.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      408 2023-07-07 18:40:46.000000 threads-net-0.0.4/examples/get_user_replies.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      410 2023-07-07 18:40:52.000000 threads-net-0.0.4/examples/get_user_threads.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      472 2023-07-07 19:07:00.000000 threads-net-0.0.4/examples/login.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:24:14.913722 threads-net-0.0.4/requirements/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 09:44:21.000000 threads-net-0.0.4/requirements/project.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-07 19:24:14.914728 threads-net-0.0.4/setup.cfg
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1245 2023-07-07 19:23:52.000000 threads-net-0.0.4/setup.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:24:14.913909 threads-net-0.0.4/threads/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.4/threads/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     5379 2023-07-07 19:22:38.000000 threads-net-0.0.4/threads/main.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:24:14.914416 threads-net-0.0.4/threads_net.egg-info/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43935 2023-07-07 19:24:14.000000 threads-net-0.0.4/threads_net.egg-info/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      412 2023-07-07 19:24:14.000000 threads-net-0.0.4/threads_net.egg-info/SOURCES.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-07 19:24:14.000000 threads-net-0.0.4/threads_net.egg-info/dependency_links.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 19:24:14.000000 threads-net-0.0.4/threads_net.egg-info/requires.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 19:24:14.000000 threads-net-0.0.4/threads_net.egg-info/top_level.txt
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:46:31.809211 threads-net-0.0.5/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-07 10:34:41.000000 threads-net-0.0.5/LICENSE
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       62 2023-07-07 09:49:10.000000 threads-net-0.0.5/MANIFEST.in
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    44189 2023-07-07 19:46:31.809080 threads-net-0.0.5/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    43338 2023-07-07 19:35:16.000000 threads-net-0.0.5/README.md
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:46:31.807798 threads-net-0.0.5/examples/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 09:42:00.000000 threads-net-0.0.5/examples/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      389 2023-07-07 18:52:22.000000 threads-net-0.0.5/examples/get_post.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      478 2023-07-07 18:47:05.000000 threads-net-0.0.5/examples/get_user.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      408 2023-07-07 18:40:46.000000 threads-net-0.0.5/examples/get_user_replies.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      410 2023-07-07 18:40:52.000000 threads-net-0.0.5/examples/get_user_threads.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      472 2023-07-07 19:07:00.000000 threads-net-0.0.5/examples/login.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:46:31.807905 threads-net-0.0.5/requirements/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       52 2023-07-07 19:45:44.000000 threads-net-0.0.5/requirements/project.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       38 2023-07-07 19:46:31.809247 threads-net-0.0.5/setup.cfg
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1245 2023-07-07 19:46:30.000000 threads-net-0.0.5/setup.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:46:31.808118 threads-net-0.0.5/threads/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       33 2023-07-07 09:42:42.000000 threads-net-0.0.5/threads/__init__.py
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     5379 2023-07-07 19:22:38.000000 threads-net-0.0.5/threads/main.py
+drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-07 19:46:31.808852 threads-net-0.0.5/threads_net.egg-info/
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)    44189 2023-07-07 19:46:31.000000 threads-net-0.0.5/threads_net.egg-info/PKG-INFO
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      412 2023-07-07 19:46:31.000000 threads-net-0.0.5/threads_net.egg-info/SOURCES.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-07 19:46:31.000000 threads-net-0.0.5/threads_net.egg-info/dependency_links.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       52 2023-07-07 19:46:31.000000 threads-net-0.0.5/threads_net.egg-info/requires.txt
+-rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       17 2023-07-07 19:46:31.000000 threads-net-0.0.5/threads_net.egg-info/top_level.txt
```

### Comparing `threads-net-0.0.4/LICENSE` & `threads-net-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-net-0.0.4/PKG-INFO` & `threads-net-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-net
-Version: 0.0.4
+Version: 0.0.5
 Summary: Threads (threads.net) Python API wrapper
 Home-page: https://github.com/dmytrostriletskyi/threads
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -39,18 +39,19 @@
   * [Get User Threads](#get-user-threads)
   * [Get User Replies](#get-user-replies)
   * [Get Post](#get-post)
 
 ## Disclaimer
 
 * This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
-  Utilizing private endpoints means simulating/pretending a client (a mobile phone) «manually» creating all needed 
-  credentials and a session. So, you might face `rate limits` or even be suspended if messed up with logining.
+  Utilizing private endpoints means simulating/pretending being a client (a mobile phone) «manually» creating all 
+  needed credentials and a session. So, you might face `rate limits` or even be suspended if mess up with logining.
+  So use the project at your own risk until the normal `Threads` public `API` is available.
 * For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
-  is used because Threads are backed by Instagram and you login via it as well.
+  is used because `Threads` are backed by `Instagram` and you do a login via it as well.
 
 ## Getting started
 
 ### How to install
 
 Install the project with the following command using `pip3`:
 
@@ -82,16 +83,16 @@
 ...
 ```
 
 ## API
 
 ### Login
 
-In order for Instagram to trust you more, you must always login from one device and one IP (or from a subnet), for this
-there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
+In order for `Instagram` to trust you more, you must always login from one device and one IP (or from a subnet), for 
+this there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
 
 ```python3
 >>> threads = Threads()
 >>> threads.login('INSTAGRAM_USERNAME', 'INSTAGRAM_PASSWORD')
 >>> threads.dump_settings('session.json')
 ```
 
@@ -103,14 +104,17 @@
 >>> threads.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
 ```
 
 The login method might ask for additional username/password entering, confirmation code and other challenges. But if
 you reuse the session, those should be minimum times. For more information, check this out — 
 https://adw0rd.github.io/instagrapi/usage-guide/interactions.html
 
+Also, the login is only needed for getting a user by identifier and username, for other endpoints it is not required, so
+you can easily skip it.
+
 ### Get User by Username
 
 To get a user by a username, use the following commands:
 
 ```python3
 >>> user = threads.get_user_by_username(username='zuck')
 >>> user
```

### Comparing `threads-net-0.0.4/README.md` & `threads-net-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,19 @@
   * [Get User Threads](#get-user-threads)
   * [Get User Replies](#get-user-replies)
   * [Get Post](#get-post)
 
 ## Disclaimer
 
 * This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
-  Utilizing private endpoints means simulating/pretending a client (a mobile phone) «manually» creating all needed 
-  credentials and a session. So, you might face `rate limits` or even be suspended if messed up with logining.
+  Utilizing private endpoints means simulating/pretending being a client (a mobile phone) «manually» creating all 
+  needed credentials and a session. So, you might face `rate limits` or even be suspended if mess up with logining.
+  So use the project at your own risk until the normal `Threads` public `API` is available.
 * For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
-  is used because Threads are backed by Instagram and you login via it as well.
+  is used because `Threads` are backed by `Instagram` and you do a login via it as well.
 
 ## Getting started
 
 ### How to install
 
 Install the project with the following command using `pip3`:
 
@@ -60,16 +61,16 @@
 ...
 ```
 
 ## API
 
 ### Login
 
-In order for Instagram to trust you more, you must always login from one device and one IP (or from a subnet), for this
-there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
+In order for `Instagram` to trust you more, you must always login from one device and one IP (or from a subnet), for 
+this there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
 
 ```python3
 >>> threads = Threads()
 >>> threads.login('INSTAGRAM_USERNAME', 'INSTAGRAM_PASSWORD')
 >>> threads.dump_settings('session.json')
 ```
 
@@ -81,14 +82,17 @@
 >>> threads.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
 ```
 
 The login method might ask for additional username/password entering, confirmation code and other challenges. But if
 you reuse the session, those should be minimum times. For more information, check this out — 
 https://adw0rd.github.io/instagrapi/usage-guide/interactions.html
 
+Also, the login is only needed for getting a user by identifier and username, for other endpoints it is not required, so
+you can easily skip it.
+
 ### Get User by Username
 
 To get a user by a username, use the following commands:
 
 ```python3
 >>> user = threads.get_user_by_username(username='zuck')
 >>> user
```

### Comparing `threads-net-0.0.4/setup.py` & `threads-net-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('README.md', 'r', encoding='utf-8') as read_me:
     long_description = read_me.read()
 
 with open('requirements/project.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
-    version='0.0.4',
+    version='0.0.5',
     name='threads-net',
     description='Threads (threads.net) Python API wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dmytrostriletskyi/threads',
     license='MIT',
     author='Dmytro Striletskyi',
```

### Comparing `threads-net-0.0.4/threads/main.py` & `threads-net-0.0.5/threads/main.py`

 * *Files identical despite different names*

### Comparing `threads-net-0.0.4/threads_net.egg-info/PKG-INFO` & `threads-net-0.0.5/threads_net.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-net
-Version: 0.0.4
+Version: 0.0.5
 Summary: Threads (threads.net) Python API wrapper
 Home-page: https://github.com/dmytrostriletskyi/threads
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -39,18 +39,19 @@
   * [Get User Threads](#get-user-threads)
   * [Get User Replies](#get-user-replies)
   * [Get Post](#get-post)
 
 ## Disclaimer
 
 * This project is unofficial (is not supported by Threads company) and utilize both public and private endpoints. 
-  Utilizing private endpoints means simulating/pretending a client (a mobile phone) «manually» creating all needed 
-  credentials and a session. So, you might face `rate limits` or even be suspended if messed up with logining.
+  Utilizing private endpoints means simulating/pretending being a client (a mobile phone) «manually» creating all 
+  needed credentials and a session. So, you might face `rate limits` or even be suspended if mess up with logining.
+  So use the project at your own risk until the normal `Threads` public `API` is available.
 * For all the authentication and a few more capabilities, [instagrapi](https://github.com/adw0rd/instagrapi) library
-  is used because Threads are backed by Instagram and you login via it as well.
+  is used because `Threads` are backed by `Instagram` and you do a login via it as well.
 
 ## Getting started
 
 ### How to install
 
 Install the project with the following command using `pip3`:
 
@@ -82,16 +83,16 @@
 ...
 ```
 
 ## API
 
 ### Login
 
-In order for Instagram to trust you more, you must always login from one device and one IP (or from a subnet), for this
-there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
+In order for `Instagram` to trust you more, you must always login from one device and one IP (or from a subnet), for 
+this there is a dump session functionality. So, once you logged in once, store them into a file and do not touch it again:
 
 ```python3
 >>> threads = Threads()
 >>> threads.login('INSTAGRAM_USERNAME', 'INSTAGRAM_PASSWORD')
 >>> threads.dump_settings('session.json')
 ```
 
@@ -103,14 +104,17 @@
 >>> threads.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
 ```
 
 The login method might ask for additional username/password entering, confirmation code and other challenges. But if
 you reuse the session, those should be minimum times. For more information, check this out — 
 https://adw0rd.github.io/instagrapi/usage-guide/interactions.html
 
+Also, the login is only needed for getting a user by identifier and username, for other endpoints it is not required, so
+you can easily skip it.
+
 ### Get User by Username
 
 To get a user by a username, use the following commands:
 
 ```python3
 >>> user = threads.get_user_by_username(username='zuck')
 >>> user
```

