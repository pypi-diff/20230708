# Comparing `tmp/nonebot_plugin_gscode-0.2.0.tar.gz` & `tmp/nonebot_plugin_gscode-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gscode-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_gscode-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_gscode-0.2.0.tar` & `nonebot_plugin_gscode-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-07-08 00:49:49.987579 nonebot_plugin_gscode-0.2.0/LICENSE
--rw-r--r--   0        0        0     1950 2023-07-08 00:49:49.987579 nonebot_plugin_gscode-0.2.0/README.md
--rw-r--r--   0        0        0     1358 2023-07-08 00:49:49.987579 nonebot_plugin_gscode-0.2.0/nonebot_plugin_gscode/__init__.py
--rw-r--r--   0        0        0     6954 2023-07-08 00:49:49.987579 nonebot_plugin_gscode-0.2.0/nonebot_plugin_gscode/data_source.py
--rw-r--r--   0        0        0     1739 2023-07-08 00:49:49.987579 nonebot_plugin_gscode-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 nonebot_plugin_gscode-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-08 12:19:08.786960 nonebot_plugin_gscode-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1950 2023-07-08 12:19:08.786960 nonebot_plugin_gscode-0.2.1/README.md
+-rw-r--r--   0        0        0     1358 2023-07-08 12:19:08.786960 nonebot_plugin_gscode-0.2.1/nonebot_plugin_gscode/__init__.py
+-rw-r--r--   0        0        0     7081 2023-07-08 12:19:08.786960 nonebot_plugin_gscode-0.2.1/nonebot_plugin_gscode/data_source.py
+-rw-r--r--   0        0        0     1739 2023-07-08 12:19:08.786960 nonebot_plugin_gscode-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 nonebot_plugin_gscode-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_gscode-0.2.0/LICENSE` & `nonebot_plugin_gscode-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gscode-0.2.0/README.md` & `nonebot_plugin_gscode-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gscode-0.2.0/nonebot_plugin_gscode/__init__.py` & `nonebot_plugin_gscode-0.2.1/nonebot_plugin_gscode/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gscode-0.2.0/nonebot_plugin_gscode/data_source.py` & `nonebot_plugin_gscode-0.2.1/nonebot_plugin_gscode/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,20 @@
     live_data = {
         "code_ver": live_data_raw["code_ver"],
         "title": live_data_raw["title"].replace("特别节目", ""),
         "header": live_template["kvDesktop"],
         "room": live_template["liveConfig"][0]["desktop"],
     }
     if live_data_raw["is_end"]:
-        live_data["review"] = live_template["reviewUrl"]["args"].get("post_id")
+        review_url = live_template["reviewUrl"]
+        live_data["review"] = (
+            review_url
+            if isinstance(review_url, str)
+            else review_url["args"].get("post_id")
+        )
     else:
         now = datetime.fromtimestamp(time(), TZ)
         start = datetime.strptime(live_data_raw["start"], "%Y-%m-%d %H:%M:%S").replace(
             tzinfo=TZ
         )
         if now < start:
             live_data["start"] = live_data_raw["start"]
```

### Comparing `nonebot_plugin_gscode-0.2.0/pyproject.toml` & `nonebot_plugin_gscode-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gscode"
-version = "0.2.0"
+version = "0.2.1"
 description = "Genshin live codes plugin for NoneBot2"
 authors = ["monsterxcn <monsterxcn@gmail.com>"]
 documentation = "https://github.com/monsterxcn/nonebot-plugin-gscode#readme"
 license = "MIT"
 homepage = "https://github.com/monsterxcn/nonebot-plugin-gscode"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "genshin", "live", "code", "redeem"]
```

### Comparing `nonebot_plugin_gscode-0.2.0/PKG-INFO` & `nonebot_plugin_gscode-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gscode
-Version: 0.2.0
+Version: 0.2.1
 Summary: Genshin live codes plugin for NoneBot2
 Home-page: https://github.com/monsterxcn/nonebot-plugin-gscode
 License: MIT
 Keywords: nonebot,nonebot2,genshin,live,code,redeem
 Author: monsterxcn
 Author-email: monsterxcn@gmail.com
 Requires-Python: >=3.8.1,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gscode Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gscode Version: 0.2.1 Summary:
 Genshin live codes plugin for NoneBot2 Home-page: https://github.com/
 monsterxcn/nonebot-plugin-gscode License: MIT Keywords:
 nonebot,nonebot2,genshin,live,code,redeem Author: monsterxcn Author-email:
 monsterxcn@gmail.com Requires-Python: >=3.8.1,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

