# Comparing `tmp/telegramweb-5.3.tar.gz` & `tmp/telegramweb-5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-5.3.tar", last modified: Sat Jul  1 07:27:30 2023, max compression
+gzip compressed data, was "telegramweb-5.4.tar", last modified: Sat Jul  8 09:24:32 2023, max compression
```

## Comparing `telegramweb-5.3.tar` & `telegramweb-5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:27:30.672705 telegramweb-5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-01 07:27:14.000000 telegramweb-5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 07:27:14.000000 telegramweb-5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-01 07:27:30.672705 telegramweb-5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-01 07:27:14.000000 telegramweb-5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 07:27:30.672705 telegramweb-5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-01 07:27:14.000000 telegramweb-5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:27:30.672705 telegramweb-5.3/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-01 07:27:14.000000 telegramweb-5.3/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-01 07:27:14.000000 telegramweb-5.3/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-01 07:27:14.000000 telegramweb-5.3/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-01 07:27:14.000000 telegramweb-5.3/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-01 07:27:14.000000 telegramweb-5.3/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:27:30.672705 telegramweb-5.3/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-01 07:27:14.000000 telegramweb-5.3/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44190 2023-07-01 07:27:14.000000 telegramweb-5.3/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-01 07:27:14.000000 telegramweb-5.3/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:27:30.672705 telegramweb-5.3/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-01 07:27:30.000000 telegramweb-5.3/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-01 07:27:30.000000 telegramweb-5.3/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:27:30.000000 telegramweb-5.3/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-01 07:27:30.000000 telegramweb-5.3/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 07:27:30.000000 telegramweb-5.3/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:24:32.815288 telegramweb-5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-08 09:24:16.000000 telegramweb-5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-08 09:24:16.000000 telegramweb-5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-08 09:24:32.811288 telegramweb-5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-08 09:24:16.000000 telegramweb-5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 09:24:32.815288 telegramweb-5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-08 09:24:16.000000 telegramweb-5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:24:32.811288 telegramweb-5.4/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-08 09:24:16.000000 telegramweb-5.4/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-08 09:24:16.000000 telegramweb-5.4/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-08 09:24:16.000000 telegramweb-5.4/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-08 09:24:16.000000 telegramweb-5.4/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-08 09:24:16.000000 telegramweb-5.4/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:24:32.811288 telegramweb-5.4/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-08 09:24:16.000000 telegramweb-5.4/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44306 2023-07-08 09:24:16.000000 telegramweb-5.4/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-08 09:24:16.000000 telegramweb-5.4/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:24:32.811288 telegramweb-5.4/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-08 09:24:32.000000 telegramweb-5.4/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-08 09:24:32.000000 telegramweb-5.4/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:24:32.000000 telegramweb-5.4/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-08 09:24:32.000000 telegramweb-5.4/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-08 09:24:32.000000 telegramweb-5.4/telegramweb.egg-info/top_level.txt
```

### Comparing `telegramweb-5.3/LICENSE` & `telegramweb-5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-5.3/PKG-INFO` & `telegramweb-5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 5.3
+Version: 5.4
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Description: <h1 align="center">
           <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telegramweb Version: 5.3 Summary: Python package
+Metadata-Version: 2.1 Name: telegramweb Version: 5.4 Summary: Python package
 for automatically fetching and pushing news by Telegram. Home-page: https://
 github.com/craziks-creator/telegram-web Author: craziks Author-email:
 chandrashekharpanday07@gmail.com License: MIT Description:
                             ****** [Telegram-news]
                                  Telegram-news
                                      ******
   Python package for automatically fetching and pushing news by Telegram. [!
```

### Comparing `telegramweb-5.3/README.md` & `telegramweb-5.4/README.md`

 * *Files identical despite different names*

### Comparing `telegramweb-5.3/setup.py` & `telegramweb-5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='5.3',
+    version='5.4',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `telegramweb-5.3/telegram_news/__init__.py` & `telegramweb-5.4/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.3/telegram_news/constant.py` & `telegramweb-5.4/telegram_news/constant.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.3/telegram_news/displaypolicy.py` & `telegramweb-5.4/telegram_news/displaypolicy.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.3/telegram_news/ratelimit.py` & `telegramweb-5.4/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.3/telegram_news/template/common.py` & `telegramweb-5.4/telegram_news/template/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -775,32 +775,36 @@
     def _get_request_url(self, pure_url):
         if self._parameter_policy:
             return self._parameter_policy(url=pure_url)
         else:
             return pure_url
 
     def _get_list(self, list_request_url):  # -> (list, int)
+        session = requests.Session()
+        session.verify = False
         timeout = self._list_request_timeout
-        res = requests.get(list_request_url, headers=self._headers, timeout=timeout, verify=False)
+        res = requests.get(list_request_url, headers=self._headers, timeout=timeout)
         # print(res.text)
         if res.status_code == 200:
             res.encoding = self._list_request_response_encode
             text = self._extractor.list_pre_process(res.text, list_request_url)
             return self._extractor.get_items_policy(text, list_request_url)
         else:
             print('\033[31mList URL error exception in ' + self._tag + '! ' + str(res.status_code) + '\033[0m')
             if res.status_code == 403:
                 print('Maybe something not work.')
             return [], 0
 
     def _get_full(self, url, item):
         text = ""
         if url:
+            session = requests.Session()
+            session.verify = False
             timeout = self._full_request_timeout
-            res = requests.get(url, headers=self._headers, timeout=timeout, verify=False)
+            res = requests.get(url, headers=self._headers, timeout=timeout)
             res.encoding = self._full_request_response_encode
             text = res.text
         text = self._extractor.full_pre_process(text, item['link'])
         # print(text)
 
         title = self._extractor.get_title_policy(text, item)
         paragraphs = self._extractor.get_paragraphs_policy(text, item)
```

### Comparing `telegramweb-5.3/telegram_news/utils.py` & `telegramweb-5.4/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-5.3/telegramweb.egg-info/PKG-INFO` & `telegramweb-5.4/telegramweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 5.3
+Version: 5.4
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Description: <h1 align="center">
           <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telegramweb Version: 5.3 Summary: Python package
+Metadata-Version: 2.1 Name: telegramweb Version: 5.4 Summary: Python package
 for automatically fetching and pushing news by Telegram. Home-page: https://
 github.com/craziks-creator/telegram-web Author: craziks Author-email:
 chandrashekharpanday07@gmail.com License: MIT Description:
                             ****** [Telegram-news]
                                  Telegram-news
                                      ******
   Python package for automatically fetching and pushing news by Telegram. [!
```

