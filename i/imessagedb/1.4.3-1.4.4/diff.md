# Comparing `tmp/imessagedb-1.4.3.tar.gz` & `tmp/imessagedb-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.4.3.tar", max compression
+gzip compressed data, was "imessagedb-1.4.4.tar", max compression
```

## Comparing `imessagedb-1.4.3.tar` & `imessagedb-1.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1070 2023-06-05 13:37:46.357285 imessagedb-1.4.3/LICENSE
--rw-r--r--   0        0        0     9445 2023-06-05 13:37:46.357285 imessagedb-1.4.3/README.md
--rw-r--r--   0        0        0     1336 2023-06-05 13:38:16.286171 imessagedb-1.4.3/pyproject.toml
--rw-r--r--   0        0        0    13235 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8476 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3186 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2365 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/chat.py
--rw-r--r--   0        0        0     4100 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3300 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/default.ini
--rw-r--r--   0        0        0     1092 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/handle.py
--rw-r--r--   0        0        0     3760 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/handles.py
--rw-r--r--   0        0        0    30347 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/html.py
--rw-r--r--   0        0        0     5037 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/message.py
--rw-r--r--   0        0        0     6222 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/messages.py
--rw-r--r--   0        0        0     6757 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/text.py
--rw-r--r--   0        0        0      677 2023-06-05 13:37:46.369285 imessagedb-1.4.3/src/imessagedb/utils.py
--rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 imessagedb-1.4.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-07-08 02:41:16.178353 imessagedb-1.4.4/LICENSE
+-rw-r--r--   0        0        0     9445 2023-07-08 02:41:16.178353 imessagedb-1.4.4/README.md
+-rw-r--r--   0        0        0     1336 2023-07-08 02:41:48.714663 imessagedb-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0    13235 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8476 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3186 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2365 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     4100 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3318 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/default.ini
+-rw-r--r--   0        0        0    30359 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/generate_html.py
+-rw-r--r--   0        0        0     6757 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/generate_text.py
+-rw-r--r--   0        0        0     1092 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     3760 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/handles.py
+-rw-r--r--   0        0        0     5037 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/message.py
+-rw-r--r--   0        0        0     6222 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/messages.py
+-rw-r--r--   0        0        0      677 2023-07-08 02:41:16.190353 imessagedb-1.4.4/src/imessagedb/utils.py
+-rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 imessagedb-1.4.4/PKG-INFO
```

### Comparing `imessagedb-1.4.3/LICENSE` & `imessagedb-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/README.md` & `imessagedb-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/pyproject.toml` & `imessagedb-1.4.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.4.3"
+version = "1.4.4"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imessagedb-1.4.3/src/imessagedb/__init__.py` & `imessagedb-1.4.4/src/imessagedb/__init__.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/attachment.py` & `imessagedb-1.4.4/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/attachments.py` & `imessagedb-1.4.4/src/imessagedb/attachments.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/chat.py` & `imessagedb-1.4.4/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/chats.py` & `imessagedb-1.4.4/src/imessagedb/chats.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/db.py` & `imessagedb-1.4.4/src/imessagedb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import os
 import sqlite3
 
 import imessagedb
 from imessagedb.attachments import Attachments
 from imessagedb.chats import Chats
 from imessagedb.handles import Handles
-from imessagedb.html import HTMLOutput
+from imessagedb.generate_html import HTMLOutput
 from imessagedb.messages import Messages
-from imessagedb.text import TextOutput
+from imessagedb.generate_text import TextOutput
 
 
 class DB:
     """
     A class to connect to an iMessage database
 
     """
```

### Comparing `imessagedb-1.4.3/src/imessagedb/default.ini` & `imessagedb-1.4.4/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/handle.py` & `imessagedb-1.4.4/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/handles.py` & `imessagedb-1.4.4/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/html.py` & `imessagedb-1.4.4/src/imessagedb/generate_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
     def _generate_table(self, message_list: Messages) -> str:
         table_array = []
         self._print_and_save(f'{" ":2s}<table class="main_table">\n', table_array)
 
         previous_day = ''
 
         message_count = 0
-        with alive_bar(len(message_list), title="Generating HTML", stats="({rate}, eta: {eta})") as bar:
+        with alive_bar(len(message_list), title="Generating HTML", stats="({rate}, eta: {eta})", comma=True) as bar:
             for message in message_list:
                 message_count = message_count + 1
 
                 today = message.date[:10]
                 if today != previous_day:
                     previous_day = today
```

### Comparing `imessagedb-1.4.3/src/imessagedb/message.py` & `imessagedb-1.4.4/src/imessagedb/message.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/messages.py` & `imessagedb-1.4.4/src/imessagedb/messages.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/text.py` & `imessagedb-1.4.4/src/imessagedb/generate_text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/src/imessagedb/utils.py` & `imessagedb-1.4.4/src/imessagedb/utils.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.4.3/PKG-INFO` & `imessagedb-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.4.3
+Version: 1.4.4
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

