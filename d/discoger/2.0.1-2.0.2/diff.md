# Comparing `tmp/discoger-2.0.1.tar.gz` & `tmp/discoger-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-2.0.1.tar", last modified: Sat Jul  8 09:12:02 2023, max compression
+gzip compressed data, was "discoger-2.0.2.tar", last modified: Sat Jul  8 20:21:32 2023, max compression
```

## Comparing `discoger-2.0.1.tar` & `discoger-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:12:02.443870 discoger-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-08 09:11:39.000000 discoger-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-08 09:12:02.443870 discoger-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-08 09:11:39.000000 discoger-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:12:02.443870 discoger-2.0.1/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 09:11:39.000000 discoger-2.0.1/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-08 09:11:39.000000 discoger-2.0.1/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-07-08 09:11:39.000000 discoger-2.0.1/discoger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-08 09:11:39.000000 discoger-2.0.1/discoger/scrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-08 09:11:39.000000 discoger-2.0.1/discoger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 09:12:02.443870 discoger-2.0.1/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-08 09:12:02.000000 discoger-2.0.1/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-08 09:12:02.000000 discoger-2.0.1/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 09:12:02.000000 discoger-2.0.1/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-08 09:12:02.000000 discoger-2.0.1/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 09:12:02.000000 discoger-2.0.1/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-08 09:12:02.443870 discoger-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-08 09:11:39.000000 discoger-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:21:32.638914 discoger-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-08 20:21:17.000000 discoger-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-08 20:21:32.638914 discoger-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-08 20:21:17.000000 discoger-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:21:32.638914 discoger-2.0.2/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:21:17.000000 discoger-2.0.2/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-08 20:21:17.000000 discoger-2.0.2/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-08 20:21:17.000000 discoger-2.0.2/discoger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-08 20:21:17.000000 discoger-2.0.2/discoger/scrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-08 20:21:17.000000 discoger-2.0.2/discoger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:21:32.638914 discoger-2.0.2/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-08 20:21:32.000000 discoger-2.0.2/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-08 20:21:32.000000 discoger-2.0.2/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 20:21:32.000000 discoger-2.0.2/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-08 20:21:32.000000 discoger-2.0.2/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 20:21:32.000000 discoger-2.0.2/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-08 20:21:32.638914 discoger-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-08 20:21:17.000000 discoger-2.0.2/setup.py
```

### Comparing `discoger-2.0.1/LICENSE` & `discoger-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-2.0.1/PKG-INFO` & `discoger-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 2.0.1
+Version: 2.0.2
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/2.0.1.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/2.0.2.tar.gz
 Description: # Discoger
         
         Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
         
         ## Usage
         
         1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
```

### Comparing `discoger-2.0.1/README.md` & `discoger-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `discoger-2.0.1/discoger/client.py` & `discoger-2.0.2/discoger/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,9 +212,13 @@
         polling_thread.daemon = True
         polling_thread.start()
         while 1:
             schedule.run_pending()
             time.sleep(1)
 
 
-if __name__ == "__main__":
+def main():
     Discoger()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `discoger-2.0.1/discoger/scrap.py` & `discoger-2.0.2/discoger/scrap.py`

 * *Files identical despite different names*

### Comparing `discoger-2.0.1/discoger/utils.py` & `discoger-2.0.2/discoger/utils.py`

 * *Files identical despite different names*

### Comparing `discoger-2.0.1/discoger.egg-info/PKG-INFO` & `discoger-2.0.2/discoger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 2.0.1
+Version: 2.0.2
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/2.0.1.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/2.0.2.tar.gz
 Description: # Discoger
         
         Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
         
         ## Usage
         
         1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
```

### Comparing `discoger-2.0.1/setup.py` & `discoger-2.0.2/setup.py`

 * *Files identical despite different names*

