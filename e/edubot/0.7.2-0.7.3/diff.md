# Comparing `tmp/edubot-0.7.2.tar.gz` & `tmp/edubot-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edubot-0.7.2.tar", max compression
+gzip compressed data, was "edubot-0.7.3.tar", max compression
```

## Comparing `edubot-0.7.2.tar` & `edubot-0.7.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-11-24 18:21:26.784597 edubot-0.7.2/LICENSE
--rw-r--r--   0        0        0     1400 2023-03-29 15:28:01.248879 edubot-0.7.2/README.md
--rw-r--r--   0        0        0      894 2023-05-19 11:19:02.481354 edubot-0.7.2/edubot/__init__.py
--rw-r--r--   0        0        0    23231 2023-06-15 15:04:03.405439 edubot-0.7.2/edubot/bot.py
--rw-r--r--   0        0        0     2950 2023-02-23 10:32:46.665675 edubot-0.7.2/edubot/sql.py
--rw-r--r--   0        0        0      636 2023-06-02 16:51:19.347235 edubot-0.7.2/edubot/types.py
--rw-r--r--   0        0        0      644 2023-06-15 15:04:44.244354 edubot-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 edubot-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-13 07:21:16.493245 edubot-0.7.3/LICENSE
+-rw-r--r--   0        0        0     1400 2023-05-04 15:06:07.555469 edubot-0.7.3/README.md
+-rw-r--r--   0        0        0      894 2023-05-05 09:01:03.030249 edubot-0.7.3/edubot/__init__.py
+-rw-r--r--   0        0        0    23375 2023-07-08 21:15:50.354655 edubot-0.7.3/edubot/bot.py
+-rw-r--r--   0        0        0     2950 2023-02-13 07:21:16.496579 edubot-0.7.3/edubot/sql.py
+-rw-r--r--   0        0        0      636 2023-05-05 09:45:44.455107 edubot-0.7.3/edubot/types.py
+-rw-r--r--   0        0        0      644 2023-07-08 21:14:54.919581 edubot-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 edubot-0.7.3/PKG-INFO
```

### Comparing `edubot-0.7.2/LICENSE` & `edubot-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edubot-0.7.2/README.md` & `edubot-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `edubot-0.7.2/edubot/__init__.py` & `edubot-0.7.3/edubot/__init__.py`

 * *Files identical despite different names*

### Comparing `edubot-0.7.2/edubot/bot.py` & `edubot-0.7.3/edubot/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,14 +247,18 @@
                 "role": "system",
                 "content": f"The current year is: {datetime.datetime.now().year}",
             },
             {
                 "role": "system",
                 "content": f"You use the language model {GPT_SETTINGS['model']}",
             },
+            {
+                "role": "system",
+                "content": f"Never prefix your messages with '{self.username}:'",
+            },
         ]
 
         for i in personality:
             system_messages.append({"role": "system", "content": i})
 
         return system_messages + gpt_context
 
@@ -402,15 +406,15 @@
             if self.__get_bot(message["username"]) is not None:
                 continue
             complete_context.append(message)
 
             if completion := self.__get_completion_from_message(message):
                 complete_context.append(
                     {
-                        "username": completion.bot,
+                        "username": self.username,
                         "message": completion.message,
                         "time": message[
                             "time"
                         ],  # Estimate this, it doesn't matter for gpt_context
                     }
                 )
```

### Comparing `edubot-0.7.2/edubot/sql.py` & `edubot-0.7.3/edubot/sql.py`

 * *Files identical despite different names*

### Comparing `edubot-0.7.2/edubot/types.py` & `edubot-0.7.3/edubot/types.py`

 * *Files identical despite different names*

### Comparing `edubot-0.7.2/pyproject.toml` & `edubot-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edubot"
-version = "0.7.2"
+version = "0.7.3"
 description = ""
 authors = ["exciteabletom <tom@digitalnook.net>", "moodler <martin@moodle.com>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `edubot-0.7.2/PKG-INFO` & `edubot-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edubot
-Version: 0.7.2
+Version: 0.7.3
 Summary: 
 License: GPLv3
 Author: exciteabletom
 Author-email: tom@digitalnook.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

