# Comparing `tmp/discoger-2.0.0.tar.gz` & `tmp/discoger-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-2.0.0.tar", last modified: Fri Jul  7 13:42:52 2023, max compression
+gzip compressed data, was "discoger-2.0.1.tar", last modified: Sat Jul  8 09:12:02 2023, max compression
```

## Comparing `discoger-2.0.0.tar` & `discoger-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:52.258410 discoger-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 13:42:29.000000 discoger-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-07 13:42:52.258410 discoger-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-07 13:42:29.000000 discoger-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:52.254410 discoger-2.0.0/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:29.000000 discoger-2.0.0/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-07 13:42:29.000000 discoger-2.0.0/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-07-07 13:42:29.000000 discoger-2.0.0/discoger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-07 13:42:29.000000 discoger-2.0.0/discoger/scrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-07 13:42:29.000000 discoger-2.0.0/discoger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:52.254410 discoger-2.0.0/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-07 13:42:52.000000 discoger-2.0.0/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 13:42:52.000000 discoger-2.0.0/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:42:52.000000 discoger-2.0.0/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 13:42:52.000000 discoger-2.0.0/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 13:42:52.000000 discoger-2.0.0/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 13:42:52.258410 discoger-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-07 13:42:29.000000 discoger-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:12:02.443870 discoger-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-08 09:11:39.000000 discoger-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-08 09:12:02.443870 discoger-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-08 09:11:39.000000 discoger-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:12:02.443870 discoger-2.0.1/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 09:11:39.000000 discoger-2.0.1/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-08 09:11:39.000000 discoger-2.0.1/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-07-08 09:11:39.000000 discoger-2.0.1/discoger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-08 09:11:39.000000 discoger-2.0.1/discoger/scrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-08 09:11:39.000000 discoger-2.0.1/discoger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:12:02.443870 discoger-2.0.1/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-08 09:12:02.000000 discoger-2.0.1/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-08 09:12:02.000000 discoger-2.0.1/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:12:02.000000 discoger-2.0.1/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-08 09:12:02.000000 discoger-2.0.1/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 09:12:02.000000 discoger-2.0.1/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-08 09:12:02.443870 discoger-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-08 09:11:39.000000 discoger-2.0.1/setup.py
```

### Comparing `discoger-2.0.0/LICENSE` & `discoger-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-2.0.0/PKG-INFO` & `discoger-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 2.0.0
+Version: 2.0.1
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/2.0.0.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/2.0.1.tar.gz
 Description: # Discoger
         
         Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
         
         ## Usage
         
         1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
```

### Comparing `discoger-2.0.0/README.md` & `discoger-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `discoger-2.0.0/discoger/client.py` & `discoger-2.0.1/discoger/client.py`

 * *Files identical despite different names*

### Comparing `discoger-2.0.0/discoger/scrap.py` & `discoger-2.0.1/discoger/scrap.py`

 * *Files identical despite different names*

### Comparing `discoger-2.0.0/discoger/utils.py` & `discoger-2.0.1/discoger/utils.py`

 * *Files identical despite different names*

### Comparing `discoger-2.0.0/discoger.egg-info/PKG-INFO` & `discoger-2.0.1/discoger.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 2.0.0
+Version: 2.0.1
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/2.0.0.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/2.0.1.tar.gz
 Description: # Discoger
         
         Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
         
         ## Usage
         
         1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
```

### Comparing `discoger-2.0.0/setup.py` & `discoger-2.0.1/setup.py`

 * *Files identical despite different names*

