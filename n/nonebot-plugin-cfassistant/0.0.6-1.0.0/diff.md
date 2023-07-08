# Comparing `tmp/nonebot-plugin-cfassistant-0.0.6.tar.gz` & `tmp/nonebot-plugin-cfassistant-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-cfassistant-0.0.6.tar", last modified: Fri Jul  7 15:47:31 2023, max compression
+gzip compressed data, was "nonebot-plugin-cfassistant-1.0.0.tar", last modified: Sat Jul  8 00:54:18 2023, max compression
```

## Comparing `nonebot-plugin-cfassistant-0.0.6.tar` & `nonebot-plugin-cfassistant-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 15:47:31.771744 nonebot-plugin-cfassistant-0.0.6/
--rw-rw-rw-   0        0        0      266 2023-07-07 15:47:31.771744 nonebot-plugin-cfassistant-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2996 2023-07-07 15:38:18.000000 nonebot-plugin-cfassistant-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 15:47:31.759212 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant/
--rw-rw-rw-   0        0        0     6503 2023-07-07 15:44:48.000000 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant/__init__.py
--rw-rw-rw-   0        0        0     2408 2023-07-07 12:22:00.000000 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant/changeRemind.py
--rw-rw-rw-   0        0        0     8738 2023-07-07 12:22:00.000000 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant/updateContest.py
--rw-rw-rw-   0        0        0     5200 2023-07-07 15:39:16.000000 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant/updateUser.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:47:31.771744 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant.egg-info/
--rw-rw-rw-   0        0        0      266 2023-07-07 15:47:31.000000 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-07-07 15:47:31.000000 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 15:47:31.000000 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-07 15:47:31.000000 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       97 2023-07-07 15:47:31.000000 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-07 15:47:31.000000 nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 15:47:31.771744 nonebot-plugin-cfassistant-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      605 2023-07-07 15:47:14.000000 nonebot-plugin-cfassistant-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 00:54:18.670419 nonebot-plugin-cfassistant-1.0.0/
+-rw-rw-rw-   0        0        0      266 2023-07-08 00:54:18.662332 nonebot-plugin-cfassistant-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2996 2023-07-07 15:38:18.000000 nonebot-plugin-cfassistant-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 00:54:18.654260 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/
+-rw-rw-rw-   0        0        0     6503 2023-07-07 15:44:48.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/__init__.py
+-rw-rw-rw-   0        0        0     2408 2023-07-07 12:22:00.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/changeRemind.py
+-rw-rw-rw-   0        0        0     8738 2023-07-07 12:22:00.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/updateContest.py
+-rw-rw-rw-   0        0        0     5200 2023-07-08 00:47:14.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/updateUser.py
+drwxrwxrwx   0        0        0        0 2023-07-08 00:54:18.662332 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-07-08 00:54:18.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-07-08 00:54:18.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 00:54:18.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-08 00:54:03.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       97 2023-07-08 00:54:18.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-08 00:54:18.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 00:54:18.670419 nonebot-plugin-cfassistant-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      605 2023-07-08 00:46:39.000000 nonebot-plugin-cfassistant-1.0.0/setup.py
```

### Comparing `nonebot-plugin-cfassistant-0.0.6/README.md` & `nonebot-plugin-cfassistant-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant/__init__.py` & `nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant/changeRemind.py` & `nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/changeRemind.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant/updateContest.py` & `nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/updateContest.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-0.0.6/nonebot_plugin_cfassistant/updateUser.py` & `nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/updateUser.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     cursor.execute('SELECT * FROM User')
     RS= cursor.fetchall()
     if len(RS) == 0:
         return Users
     for row in RS:
         Oid, Onow_rating, Oupdate_time, OQQ, Ostatus ,Olast_rating = row
         user_info_url=user_info_baseurl+Oid
-        time.sleep(0.2)
+        time.sleep(0.3)
         try:
             response = requests.get(user_info_url)
             response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
             data = json.loads(response.text)
         except requests.RequestException as e:
             print("请求错误:", e)
             continue
```

### Comparing `nonebot-plugin-cfassistant-0.0.6/setup.py` & `nonebot-plugin-cfassistant-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = '0.0.6'
+VERSION = '1.0.0'
 
 setup(
     name='nonebot-plugin-cfassistant', 
     version=VERSION,  
     description='一个支持CF(codeforces)平台查询比赛/比赛提醒/监测分数变化的nonebot机器人插件', 
     packages=find_packages(),
     zip_safe=False,
```

