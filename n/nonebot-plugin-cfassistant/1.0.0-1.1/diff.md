# Comparing `tmp/nonebot-plugin-cfassistant-1.0.0.tar.gz` & `tmp/nonebot-plugin-cfassistant-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-cfassistant-1.0.0.tar", last modified: Sat Jul  8 00:54:18 2023, max compression
+gzip compressed data, was "nonebot-plugin-cfassistant-1.1.tar", last modified: Sat Jul  8 16:36:12 2023, max compression
```

## Comparing `nonebot-plugin-cfassistant-1.0.0.tar` & `nonebot-plugin-cfassistant-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 00:54:18.670419 nonebot-plugin-cfassistant-1.0.0/
--rw-rw-rw-   0        0        0      266 2023-07-08 00:54:18.662332 nonebot-plugin-cfassistant-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2996 2023-07-07 15:38:18.000000 nonebot-plugin-cfassistant-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 00:54:18.654260 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/
--rw-rw-rw-   0        0        0     6503 2023-07-07 15:44:48.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/__init__.py
--rw-rw-rw-   0        0        0     2408 2023-07-07 12:22:00.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/changeRemind.py
--rw-rw-rw-   0        0        0     8738 2023-07-07 12:22:00.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/updateContest.py
--rw-rw-rw-   0        0        0     5200 2023-07-08 00:47:14.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/updateUser.py
-drwxrwxrwx   0        0        0        0 2023-07-08 00:54:18.662332 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/
--rw-rw-rw-   0        0        0      266 2023-07-08 00:54:18.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-07-08 00:54:18.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 00:54:18.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-08 00:54:03.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       97 2023-07-08 00:54:18.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-08 00:54:18.000000 nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 00:54:18.670419 nonebot-plugin-cfassistant-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      605 2023-07-08 00:46:39.000000 nonebot-plugin-cfassistant-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:36:12.468580 nonebot-plugin-cfassistant-1.1/
+-rw-rw-rw-   0        0        0      264 2023-07-08 16:36:12.468580 nonebot-plugin-cfassistant-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3184 2023-07-08 01:30:14.000000 nonebot-plugin-cfassistant-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 16:36:12.455833 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/
+-rw-rw-rw-   0        0        0     6503 2023-07-07 15:44:48.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/__init__.py
+-rw-rw-rw-   0        0        0     3784 2023-07-08 12:01:28.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/changeRemind.py
+-rw-rw-rw-   0        0        0    10468 2023-07-08 12:12:18.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/updateContest.py
+-rw-rw-rw-   0        0        0     6085 2023-07-08 12:34:24.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/updateUser.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:36:12.467074 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-07-08 16:36:12.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-07-08 16:36:12.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 16:36:12.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-08 16:36:00.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      115 2023-07-08 16:36:12.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-08 16:36:12.000000 nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 16:36:12.469589 nonebot-plugin-cfassistant-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      633 2023-07-08 16:35:38.000000 nonebot-plugin-cfassistant-1.1/setup.py
```

### Comparing `nonebot-plugin-cfassistant-1.0.0/README.md` & `nonebot-plugin-cfassistant-1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 <a href="https://pypi.python.org/pypi/nonebot-plugin-example">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-example.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
-
-一个支持CF(codeforces)平台查询比赛/比赛提醒/监测分数变化的nonebot机器人插件
+  
+一个支持CF(codeforces)平台查询比赛/比赛提醒/监测分数变化的nonebot机器人插件  
+插件启动后，将会在nonebot机器人项目创建 `data/CFHelper/`，并存放`data.db`(储存比赛和绑定用户)和`reminder.db`(储存订阅比赛提醒的用户和群聊)
 
 ## 📖 介绍
 
 本插件支持以下功能：
 - 查询当前CF平台上还未开始的比赛
 - 比赛前48小时，11小时，3小时定时提醒。可以群提醒或好友私聊提醒
 - 绑定用户ID 当检测到绑定用户分数发生变化时通过好友私聊发送分数变化消息
@@ -64,15 +65,15 @@
 <summary>conda</summary>
 
     conda install nonebot-plugin-cfassistant
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-    plugins = ["nonebot-plugin-cfassistant"]
+    plugins = ["nonebot_plugin_cfassistant"]
 
 </details>
 
 
 ## 🎉 使用
 ### 指令表
 - **输入:/CFHELP获取插件帮助 如**
```

#### html2text {}

```diff
@@ -1,26 +1,29 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-cfassistant _â¨ NoneBot æä»¶ç®åæè¿° â¨_ [license]
                                 [pypi] [python]
 ä¸ä¸ªæ¯æCF(codeforces)å¹³å°æ¥è¯¢æ¯èµ/æ¯èµæé/
-çæµåæ°ååçnonebotæºå¨äººæä»¶ ## ð ä»ç»
+çæµåæ°ååçnonebotæºå¨äººæä»¶
+æä»¶å¯å¨åï¼å°ä¼å¨nonebotæºå¨äººé¡¹ç®åå»º `data/CFHelper/
+`ï¼å¹¶å­æ¾`data.db`(å¨å­æ¯èµåç»å®ç¨æ·)å`reminder.db`
+(å¨å­è®¢éæ¯èµæéçç¨æ·åç¾¤è) ## ð ä»ç»
 æ¬æä»¶æ¯æä»¥ä¸åè½ï¼ - æ¥è¯¢å½åCFå¹³å°ä¸è¿æªå¼å§çæ¯èµ -
 æ¯èµå48å°æ¶ï¼11å°æ¶ï¼3å°æ¶å®æ¶æéãå¯ä»¥ç¾¤æéæå¥½åç§èæé
 - ç»å®ç¨æ·ID
 å½æ£æµå°ç»å®ç¨æ·åæ°åçååæ¶éè¿å¥½åç§èåéåæ°ååæ¶æ¯
 ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-cfassistant   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot-plugin-cfassistant   pdm
 pdm add nonebot-plugin-cfassistant   poetry poetry add nonebot-plugin-
 cfassistant   conda conda install nonebot-plugin-cfassistant  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
-é¨åè¿½å åå¥ plugins = ["nonebot-plugin-cfassistant"]  ## ð ä½¿ç¨ ###
+é¨åè¿½å åå¥ plugins = ["nonebot_plugin_cfassistant"]  ## ð ä½¿ç¨ ###
 æä»¤è¡¨ - **è¾å¥:/CFHELPè·åæä»¶å¸®å© å¦** `/CFHELP` - è¾å¥:/CF æ
 /cf æ /æ¥CF æ /æ¥cf å³å¯è¿è¡æ¥è¯¢è¿ææ¯èµ å¦ `/CF` -
 å¨å¥½åç§èä¸è¾å¥:/ç»å® ä½ çCFä¸ªäººID
 å³å¯å¯¹è¯¥è´¦æ·åæ°è¿è¡çæµ(ä¸ä¸ªIDåªè½ç»å®ä¸ä¸ªQQå·) å¦ `/
 ç»å® jiangly` - å¨ç¾¤èä¸è¾å¥:/ç¾¤æé
 å³å¯å¯¹æ¬ç¾¤å¼å¯æ¯èµæéåè½
 (åå«å¨48å°æ¶ï¼11å°æ¶ï¼3å°æ¶æéä¸æ¬¡) å¦ `/ç¾¤æé` -
```

### Comparing `nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/__init__.py` & `nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/updateContest.py` & `nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/updateContest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,58 @@
 import requests
 import json
 import datetime
-import sqlite3
-contest_url = "https://codeforces.com/api/contest.list?gym=false"
+import aiosqlite
+import asyncio 
 import os
+
+contest_url = "https://codeforces.com/api/contest.list?gym=false"
 data_path = './data/CFHelper/'
 if not os.path.exists(data_path):
     os.makedirs(data_path)
-conn = sqlite3.connect('./data/CFHelper/data.db')
-cursor = conn.cursor()
-cursor.execute('''
-    CREATE TABLE IF NOT EXISTS Contest (
-        id INTEGER PRIMARY KEY,
-        name TEXT,
-        type TEXT,
-        phase TEXT,
-        duration INTEGER,
-        startTime INTEGER,
-        relativeTime INTEGER,
-        durationShow TEXT,
-        startTimeShow TEXT,
-        relativeTimeShow TEXT,
-        remindStatus INTEGER
-    )
-''')
+db_path = os.path.join(data_path, 'data.db')
+# conn = sqlite3.connect('./data/CFHelper/data.db')
+# cursor = conn.cursor()
+# cursor.execute('''
+#     CREATE TABLE IF NOT EXISTS Contest (
+#         id INTEGER PRIMARY KEY,
+#         name TEXT,
+#         type TEXT,
+#         phase TEXT,
+#         duration INTEGER,
+#         startTime INTEGER,
+#         relativeTime INTEGER,
+#         durationShow TEXT,
+#         startTimeShow TEXT,
+#         relativeTimeShow TEXT,
+#         remindStatus INTEGER
+#     )
+# ''')
+
+async def create_data():
+    async with aiosqlite.connect(db_path) as conn:
+            cursor = await conn.cursor()
+            await cursor.execute('''
+                CREATE TABLE IF NOT EXISTS Contest (
+                    id INTEGER PRIMARY KEY,
+                    name TEXT,
+                    type TEXT,
+                    phase TEXT,
+                    duration INTEGER,
+                    startTime INTEGER,
+                    relativeTime INTEGER,
+                    durationShow TEXT,
+                    startTimeShow TEXT,
+                    relativeTimeShow TEXT,
+                    remindStatus INTEGER
+                )
+            ''')
+            await conn.commit()
+
+asyncio.run(create_data())
 
 class ContestType:
     def __init__(self, id, name, type, phase, duration, startTime, relativeTime,durationShow,startTimeShow,relativeTimeShow):
         self.id = id
         self.name = name
         self.type = type
         self.phase = phase
@@ -38,15 +63,14 @@
         self.startTimeShow=startTimeShow
         self.relativeTimeShow=relativeTimeShow
         self.remindStatus=0
 
 
 async def updateContest():
     Contests=[]
-    global contest_url,cursor,conn
     try:
         response = requests.get(contest_url)
         response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
         data = json.loads(response.text)
     except requests.RequestException as e:
         print("请求错误:", e)
         return Contests
@@ -87,138 +111,148 @@
                 contest_relative_time=f"{re_hours}小时{re_minutes}分钟"
             else:
                 contest_relative_time=f"{re_days}天{re_hours}小时{re_minutes}分钟"
             
             contest=ContestType(result["id"],result["name"],result["type"],result["phase"],result["durationSeconds"],result["startTimeSeconds"],abs(result["relativeTimeSeconds"]),contest_duration,contest_start_time,contest_relative_time)
             Contests.append(contest)
 
-            cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
-            remind_status=0
-
-            status = cursor.fetchone()
-            if status is not None:
-                remind_status = status[0]
-
-            cursor.execute('''
-            INSERT OR REPLACE INTO Contest (id, name, type, phase, duration, startTime, relativeTime, durationShow, startTimeShow, relativeTimeShow, remindStatus)
-            VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)
-        ''', (
-            contest.id,
-            contest.name,
-            contest.type,
-            contest.phase,
-            contest.duration,
-            contest.startTime,
-            contest.relativeTime,
-            contest.durationShow,
-            contest.startTimeShow,
-            contest.relativeTimeShow,
-            remind_status
-        ))
-            conn.commit()
+            async with aiosqlite.connect(db_path) as conn:
+                cursor = await conn.cursor()
+                await cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
+                remind_status=0
+
+                status = await cursor.fetchone()
+                if status is not None:
+                    remind_status = status[0]
+
+                await cursor.execute('''
+                INSERT OR REPLACE INTO Contest (id, name, type, phase, duration, startTime, relativeTime, durationShow, startTimeShow, relativeTimeShow, remindStatus)
+                VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)
+            ''', (
+                contest.id,
+                contest.name,
+                contest.type,
+                contest.phase,
+                contest.duration,
+                contest.startTime,
+                contest.relativeTime,
+                contest.durationShow,
+                contest.startTimeShow,
+                contest.relativeTimeShow,
+                remind_status
+            ))
+                await conn.commit()
     else:
         print("数据请求失败")
 
     return Contests
 
 async def returnreminderInfo():
     Contests=await updateContest()
-    global cursor,conn
     output=""
-    for contest in Contests:
-        cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
-        ids = cursor.fetchone()
-        remind_status = ids[0]
-        
-        current_time_raw = datetime.datetime.now()
-        current_time = int(current_time_raw.timestamp())
-        if contest.startTime+contest.duration<=current_time:
-            cursor.execute('''
-                UPDATE Contest
-                SET phase = ?
-                WHERE id = ?
-            ''', ("FINISHED", contest.id))
-            conn.commit() 
-            cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
-            ids = cursor.fetchone()
-            remind_status = ids[0]
-        
-        if contest.relativeTime<=3*3600 and remind_status<3:
-            output+=f"3小时内将有以下比赛：\n" \
-            f"比赛ID：{contest.id}\n" \
-            f"比赛名称：{contest.name}\n" \
-            f"比赛开始时间：{contest.startTimeShow}\n" \
-            f"比赛时长：{contest.durationShow}\n" \
-            f"距离比赛开始时间：{contest.relativeTimeShow}\n\n"
-            cursor.execute('''
-                UPDATE Contest
-                SET remindStatus = ?
-                WHERE id = ?
-            ''', (3, contest.id))
-            conn.commit()     
-            cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
-            ids = cursor.fetchone()
-            remind_status = ids[0]
-
-        if contest.relativeTime<=11*3600 and remind_status<2:
-            output+=f"11小时内将有以下比赛：\n" \
-            f"比赛ID：{contest.id}\n" \
-            f"比赛名称：{contest.name}\n" \
-            f"比赛开始时间：{contest.startTimeShow}\n" \
-            f"比赛时长：{contest.durationShow}\n" \
-            f"距离比赛开始时间：{contest.relativeTimeShow}\n\n"
-            cursor.execute('''
-                UPDATE Contest
-                SET remindStatus = ?
-                WHERE id = ?
-            ''', (2, contest.id))
-            conn.commit()       
-            cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
-            ids = cursor.fetchone()
-            remind_status = ids[0]
-
-        if contest.relativeTime<=48*3600 and remind_status<1:
-            output+=f"48小时内将有以下比赛：\n" \
-            f"比赛ID：{contest.id}\n" \
-            f"比赛名称：{contest.name}\n" \
-            f"比赛开始时间：{contest.startTimeShow}\n" \
-            f"比赛时长：{contest.durationShow}\n" \
-            f"距离比赛开始时间：{contest.relativeTimeShow}\n\n"
-            cursor.execute('''
-                UPDATE Contest
-                SET remindStatus = ?
-                WHERE id = ?
-            ''', (1, contest.id))
-            conn.commit()
-            cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
-            ids = cursor.fetchone()
-            remind_status = ids[0]
-    if(output!=""):
-        print(output)
+    async with aiosqlite.connect(db_path) as conn:
+        remind_status=3
+        cursor = await conn.cursor()
+        for contest in Contests:
+            await cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
+            ids = await cursor.fetchone()
+            if ids is not None:
+                remind_status = ids[0]
+            
+            current_time_raw = datetime.datetime.now()
+            current_time = int(current_time_raw.timestamp())
+            if contest.startTime+contest.duration<=current_time:
+                await cursor.execute('''
+                    UPDATE Contest
+                    SET phase = ?
+                    WHERE id = ?
+                ''', ("FINISHED", contest.id))
+                await conn.commit() 
+                await cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
+                ids = await cursor.fetchone()
+                if ids is not None:
+                    remind_status = ids[0]
+            
+            if contest.relativeTime<=3*3600 and remind_status<3:
+                output+=f"3小时内将有以下比赛：\n" \
+                f"比赛ID：{contest.id}\n" \
+                f"比赛名称：{contest.name}\n" \
+                f"比赛开始时间：{contest.startTimeShow}\n" \
+                f"比赛时长：{contest.durationShow}\n" \
+                f"距离比赛开始时间：{contest.relativeTimeShow}\n\n"
+                await cursor.execute('''
+                    UPDATE Contest
+                    SET remindStatus = ?
+                    WHERE id = ?
+                ''', (3, contest.id))
+                await conn.commit()     
+                await cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
+                ids = await cursor.fetchone()
+                if ids is not None:
+                    remind_status = ids[0]
+
+            if contest.relativeTime<=11*3600 and remind_status<2:
+                output+=f"11小时内将有以下比赛：\n" \
+                f"比赛ID：{contest.id}\n" \
+                f"比赛名称：{contest.name}\n" \
+                f"比赛开始时间：{contest.startTimeShow}\n" \
+                f"比赛时长：{contest.durationShow}\n" \
+                f"距离比赛开始时间：{contest.relativeTimeShow}\n\n"
+                await cursor.execute('''
+                    UPDATE Contest
+                    SET remindStatus = ?
+                    WHERE id = ?
+                ''', (2, contest.id))
+                await conn.commit()       
+                await cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
+                ids = await cursor.fetchone()
+                if ids is not None:
+                    remind_status = ids[0]
+
+            if contest.relativeTime<=48*3600 and remind_status<1:
+                output+=f"48小时内将有以下比赛：\n" \
+                f"比赛ID：{contest.id}\n" \
+                f"比赛名称：{contest.name}\n" \
+                f"比赛开始时间：{contest.startTimeShow}\n" \
+                f"比赛时长：{contest.durationShow}\n" \
+                f"距离比赛开始时间：{contest.relativeTimeShow}\n\n"
+                await cursor.execute('''
+                    UPDATE Contest
+                    SET remindStatus = ?
+                    WHERE id = ?
+                ''', (1, contest.id))
+                await conn.commit()
+                await cursor.execute('SELECT remindStatus FROM Contest WHERE id = ?', (contest.id,))
+                ids = await cursor.fetchone()
+                if ids is not None:
+                    remind_status = ids[0]
+
+        if(output!=""):
+            print(output)
 
     return output
 
 async def returnContestInfo():
     Contests=await updateContest()
     output=f"当前时间：{datetime.datetime.now()}\n\n"
     for contest in Contests:
         output+=f"比赛ID：{contest.id}\n" \
                 f"比赛名称：{contest.name}\n" \
                 f"比赛开始时间：{contest.startTimeShow}\n" \
                 f"比赛时长：{contest.durationShow}\n" \
                 f"距离比赛开始时间：{contest.relativeTimeShow}\n\n"
     return output
 
-def markdata():
-    current_time_raw = datetime.datetime.now()
-    current_time = int(current_time_raw.timestamp())
-    cursor.execute('SELECT * FROM Contest')
-    RS= cursor.fetchall()
-    for row in RS:
-        id, name, type, phase, duration, startTime, relativeTime, durationShow, startTimeShow, relativeTimeShow, remindStatus = row
-        if startTime+duration<=current_time:
-            cursor.execute('''
-                UPDATE Contest
-                SET phase = ?
-                WHERE id = ?
-            ''', ("FINISHED", id))
-            conn.commit() 
+# def markdata():
+#     current_time_raw = datetime.datetime.now()
+#     current_time = int(current_time_raw.timestamp())
+#     cursor.execute('SELECT * FROM Contest')
+#     RS= cursor.fetchall()
+#     for row in RS:
+#         id, name, type, phase, duration, startTime, relativeTime, durationShow, startTimeShow, relativeTimeShow, remindStatus = row
+#         if startTime+duration<=current_time:
+#             cursor.execute('''
+#                 UPDATE Contest
+#                 SET phase = ?
+#                 WHERE id = ?
+#             ''', ("FINISHED", id))
+#             conn.commit()
```

### Comparing `nonebot-plugin-cfassistant-1.0.0/nonebot_plugin_cfassistant/updateUser.py` & `nonebot-plugin-cfassistant-1.1/nonebot_plugin_cfassistant/updateUser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 import requests
 import json
 import datetime
-import sqlite3
+import aiosqlite
+import asyncio 
 import time
 user_info_baseurl="https://codeforces.com/api/user.info?handles="
 import os
 data_path = './data/CFHelper/'
 if not os.path.exists(data_path):
     os.makedirs(data_path)
-conn = sqlite3.connect('./data/CFHelper/data.db')
-cursor = conn.cursor()
-cursor.execute('''
-    CREATE TABLE IF NOT EXISTS User (
-        id TEXT PRIMARY KEY,
-        now_rating INTEGER,
-        update_time INTEGER,
-        QQ INTEGER,
-        status INTEGER,
-        last_rating INTEGER
-    )
-''')
+
+db_path = os.path.join(data_path, 'data.db')
+
+async def create_dataS():
+    async with aiosqlite.connect(db_path) as conn:
+            cursor = await conn.cursor()
+            await cursor.execute('''
+                CREATE TABLE IF NOT EXISTS User (
+                    id TEXT PRIMARY KEY,
+                    now_rating INTEGER,
+                    update_time INTEGER,
+                    QQ INTEGER,
+                    status INTEGER,
+                    last_rating INTEGER
+                )
+            ''')
+            await conn.commit()
+
+asyncio.run(create_dataS())
 
 class UserType:
     def __init__(self, id, now_rating, update_time,QQ,status,last_rating):
         self.id = id
         self.now_rating= now_rating if now_rating is not None else 0
         self.update_time=update_time if update_time is not None else 0
         self.QQ=QQ if QQ is not None else 0
         self.status=status if status is not None else 1
         self.last_rating=last_rating if last_rating is not None else 0
 
 
 async def addUser(id,QQ):
-    global user_info_baseurl,cursor,conn
     user_info_url=user_info_baseurl+id
-
     try:
         response = requests.get(user_info_url)
         response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
         data = json.loads(response.text)
     except requests.RequestException as e:
         print("请求错误:", e)
         return False 
@@ -56,100 +62,105 @@
         # 获取result列表
         results = data["result"]
         
         # 遍历每个结果并储存键值
         for result in results:
             update_time=int(datetime.datetime.now().timestamp())
             user=UserType(id,result["rating"],update_time,QQ,1,result["rating"])
-            cursor.execute('''
-            INSERT OR REPLACE INTO User (id, now_rating, update_time,QQ,status,last_rating)
-            VALUES (?, ?, ?, ?, ?, ?)
-        ''', (
-            user.id,
-            user.now_rating,
-            user.update_time,
-            user.QQ,
-            user.status,
-            user.last_rating
-        ))
-            conn.commit()
-            return True
-    else:
-        print("添加用户请求失败")
-        return False
-
-
-async def updateUser():
-    Users=[]
-    global user_info_baseurl,cursor,conn
-
-    cursor.execute('SELECT * FROM User')
-    RS= cursor.fetchall()
-    if len(RS) == 0:
-        return Users
-    for row in RS:
-        Oid, Onow_rating, Oupdate_time, OQQ, Ostatus ,Olast_rating = row
-        user_info_url=user_info_baseurl+Oid
-        time.sleep(0.3)
-        try:
-            response = requests.get(user_info_url)
-            response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
-            data = json.loads(response.text)
-        except requests.RequestException as e:
-            print("请求错误:", e)
-            continue
-        except json.JSONDecodeError as e:
-            print("JSON解析错误:", e)
-            continue
-            # 处理JSON解析异常的情况
-        except Exception as e:
-            print("发生了其他错误:", e)
-            continue
-            # 处理其他未预料到的异常情况
-
-        # 检查API响应状态
-        if data["status"] == "OK":
-            # 获取result列表
-            results = data["result"]
-            
-            # 遍历每个结果并储存键值
-            for result in results:
-                update_time=int(datetime.datetime.now().timestamp())
-                user=UserType(Oid,result["rating"],update_time,OQQ,Ostatus,Onow_rating)
-                Users.append(user)
-
-                cursor.execute('''
+            async with aiosqlite.connect(db_path) as conn:
+                cursor = await conn.cursor()
+                await cursor.execute('''
                 INSERT OR REPLACE INTO User (id, now_rating, update_time,QQ,status,last_rating)
                 VALUES (?, ?, ?, ?, ?, ?)
             ''', (
                 user.id,
                 user.now_rating,
                 user.update_time,
                 user.QQ,
                 user.status,
                 user.last_rating
             ))
-                conn.commit()
-        else:
-            print("数据请求失败")
+                await conn.commit()
+        return True
+    else:
+        print("添加用户请求失败")
+        return False
+
+
+async def updateUser():
+    Users=[]
+    async with aiosqlite.connect(db_path) as conn:
+        cursor = await conn.cursor()
+        await cursor.execute('SELECT * FROM User')
+        RS= await cursor.fetchall()
+        if not RS:
+            return Users
+        for row in RS:
+            Oid, Onow_rating, Oupdate_time, OQQ, Ostatus ,Olast_rating = row
+            user_info_url=user_info_baseurl+Oid
+            time.sleep(0.3)
+            try:
+                response = requests.get(user_info_url)
+                response.raise_for_status()  # 检查响应是否成功，如果不成功会抛出异常
+                data = json.loads(response.text)
+            except requests.RequestException as e:
+                print("请求错误:", e)
+                continue
+            except json.JSONDecodeError as e:
+                print("JSON解析错误:", e)
+                continue
+                # 处理JSON解析异常的情况
+            except Exception as e:
+                print("发生了其他错误:", e)
+                continue
+                # 处理其他未预料到的异常情况
+
+            # 检查API响应状态
+            if data["status"] == "OK":
+                # 获取result列表
+                results = data["result"]
+                
+                # 遍历每个结果并储存键值
+                for result in results:
+                    update_time=int(datetime.datetime.now().timestamp())
+                    user=UserType(Oid,result["rating"],update_time,OQQ,Ostatus,Onow_rating)
+                    Users.append(user)
+
+                    await cursor.execute('''
+                    INSERT OR REPLACE INTO User (id, now_rating, update_time,QQ,status,last_rating)
+                    VALUES (?, ?, ?, ?, ?, ?)
+                ''', (
+                    user.id,
+                    user.now_rating,
+                    user.update_time,
+                    user.QQ,
+                    user.status,
+                    user.last_rating
+                ))
+                    await conn.commit()
+            else:
+                print("数据请求失败")
 
     return Users
 
 async def returRatingChangeInfo():
     outputlist=[]
     Users=await updateUser()
     if not Users:
         return outputlist
 
-    global cursor,conn
-    for user in Users:
-        output=f"当前时间：{datetime.datetime.now()}\n"
-        cursor.execute('SELECT now_rating,last_rating,QQ FROM User WHERE id = ?', (user.id,))
-        row = cursor.fetchone()
-        now_rating,last_rating,QQ = row
-        if last_rating!=now_rating:
-            change=now_rating-last_rating
-            output+=f"检测到您的CF账号 {user.id} 分数发生变化，从{last_rating} → {now_rating}  变动了{change}分！\n"
-            outputlist.append({'QQ':QQ,'output':output})
-
+    async with aiosqlite.connect(db_path) as conn:
+        cursor = await conn.cursor()
+        for user in Users:
+            output=f"当前时间：{datetime.datetime.now()}\n"
+            await cursor.execute('SELECT now_rating,last_rating,QQ FROM User WHERE id = ?', (user.id,))
+            row = await cursor.fetchone()
+            if row is not None:
+                now_rating,last_rating,QQ = row
+                if last_rating!=now_rating:
+                    change=now_rating-last_rating
+                    output+=f"检测到您的CF账号 {user.id} 分数发生变化，从{last_rating} → {now_rating}  变动了{change}分！\n"
+                    outputlist.append({'QQ':QQ,'output':output})
+            else:
+                continue
     return outputlist
```

### Comparing `nonebot-plugin-cfassistant-1.0.0/setup.py` & `nonebot-plugin-cfassistant-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = '1.0.0'
+VERSION = '1.1'
 
 setup(
     name='nonebot-plugin-cfassistant', 
     version=VERSION,  
     description='一个支持CF(codeforces)平台查询比赛/比赛提醒/监测分数变化的nonebot机器人插件', 
     packages=find_packages(),
     zip_safe=False,
     url='https://github.com/coyude/nonebot-plugin-cfassistant',
     author="coyude",
     install_requires=[
         "requests>=2.23.0",
         "nonebot_plugin_apscheduler>=0.3.0",
         "nonebot2>=2.0.0",
-        "nonebot-adapter-onebot>=2.2.3"
+        "nonebot-adapter-onebot>=2.2.3",
+        "aiosqlite>=0.17.0"
     ],
 )
```

