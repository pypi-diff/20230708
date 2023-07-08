# Comparing `tmp/nonebot_plugin_gscode-0.1.8.tar.gz` & `tmp/nonebot_plugin_gscode-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gscode-0.1.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_gscode-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_gscode-0.1.8.tar` & `nonebot_plugin_gscode-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-05-15 12:04:42.661528 nonebot_plugin_gscode-0.1.8/LICENSE
--rw-r--r--   0        0        0     1950 2023-05-15 12:04:42.661528 nonebot_plugin_gscode-0.1.8/README.md
--rw-r--r--   0        0        0     1028 2023-05-15 12:04:42.661528 nonebot_plugin_gscode-0.1.8/nonebot_plugin_gscode/__init__.py
--rw-r--r--   0        0        0     6805 2023-05-15 12:04:42.661528 nonebot_plugin_gscode-0.1.8/nonebot_plugin_gscode/data_source.py
--rw-r--r--   0        0        0     1739 2023-05-15 12:04:42.661528 nonebot_plugin_gscode-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 nonebot_plugin_gscode-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-08 00:49:49.987579 nonebot_plugin_gscode-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1950 2023-07-08 00:49:49.987579 nonebot_plugin_gscode-0.2.0/README.md
+-rw-r--r--   0        0        0     1358 2023-07-08 00:49:49.987579 nonebot_plugin_gscode-0.2.0/nonebot_plugin_gscode/__init__.py
+-rw-r--r--   0        0        0     6954 2023-07-08 00:49:49.987579 nonebot_plugin_gscode-0.2.0/nonebot_plugin_gscode/data_source.py
+-rw-r--r--   0        0        0     1739 2023-07-08 00:49:49.987579 nonebot_plugin_gscode-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 nonebot_plugin_gscode-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_gscode-0.1.8/LICENSE` & `nonebot_plugin_gscode-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gscode-0.1.8/README.md` & `nonebot_plugin_gscode-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gscode-0.1.8/nonebot_plugin_gscode/data_source.py` & `nonebot_plugin_gscode-0.2.0/nonebot_plugin_gscode/data_source.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import json
 from time import time
-from re import findall
+from re import sub, findall
 from typing import Dict, List, Union
 from datetime import datetime, timezone, timedelta
 
 from httpx import AsyncClient
-
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 
 TZ = timezone(timedelta(hours=8))
 
 
-async def getData(type, data: Dict = {}) -> Dict:
+async def get_data(type, mhy_type: str = "", data: Dict = {}) -> Dict:
     """米哈游接口请求"""
 
+    uid = 288909600 if mhy_type == "sr" else 75276550
     url = {
-        "actId": "https://bbs-api.mihoyo.com/painter/api/user_instant/list?offset=0&size=20&uid=75276550",
+        "act_id": f"https://bbs-api.mihoyo.com/painter/api"
+        f"/user_instant/list?offset=0&size=20&uid={uid}",
         "index": "https://api-takumi.mihoyo.com/event/miyolive/index",
         "code": "https://api-takumi-static.mihoyo.com/event/miyolive/refreshCode",
     }
     async with AsyncClient() as client:
         try:
             if type == "index":
                 res = await client.get(
@@ -39,165 +40,162 @@
                 res = await client.get(url[type])
             return res.json()
         except Exception as e:
             logger.opt(exception=e).error(f"{type} 接口请求错误")
             return {"error": f"[{e.__class__.__name__}] {type} 接口请求错误"}
 
 
-async def getActId() -> str:
+async def get_act_id(mhy_type) -> str:
     """获取 ``act_id``"""
 
-    ret = await getData("actId")
+    ret = await get_data(type="act_id", mhy_type=mhy_type)
     if ret.get("error") or ret.get("retcode") != 0:
         return ""
 
-    actId = ""
-    keywords = ["来看《原神》", "版本前瞻特别节目"]
+    act_id = ""
+    keywords = ["版本前瞻特别节目"]
     for p in ret["data"]["list"]:
         post = p.get("post", {}).get("post", {})
         if not post:
             continue
         if not all(word in post["subject"] for word in keywords):
             continue
         shit = json.loads(post["structured_content"])
         for segment in shit:
             link = segment.get("attributes", {}).get("link", "")
-            if "观看直播" in segment.get("insert", "") and link:
+            if "直播" in segment.get("insert", "") and link:
                 matched = findall(r"act_id=(.*?)\&", link)
                 if matched:
-                    actId = matched[0]
-        if actId:
+                    act_id = matched[0]
+        if act_id:
             break
 
-    return actId
+    return act_id
 
 
-async def getLiveData(actId: str) -> Dict:
+async def get_live_data(act_id: str) -> Dict:
     """获取直播数据，尤其是 ``code_ver``"""
 
-    ret = await getData("index", {"actId": actId})
+    ret = await get_data(type="index", data={"actId": act_id})
     if ret.get("error") or ret.get("retcode") != 0:
         return {"error": ret.get("error") or "前瞻直播数据异常"}
 
-    liveDataRaw = ret["data"]["live"]
-    liveTemplate = json.loads(ret["data"]["template"])
-    liveData = {
-        "code_ver": liveDataRaw["code_ver"],
-        "title": liveDataRaw["title"].replace("特别节目", ""),
-        "header": liveTemplate["kvDesktop"],
-        "room": liveTemplate["liveConfig"][0]["desktop"],
+    live_data_raw = ret["data"]["live"]
+    live_template = json.loads(ret["data"]["template"])
+    live_data = {
+        "code_ver": live_data_raw["code_ver"],
+        "title": live_data_raw["title"].replace("特别节目", ""),
+        "header": live_template["kvDesktop"],
+        "room": live_template["liveConfig"][0]["desktop"],
     }
-    if liveDataRaw["is_end"]:
-        liveData["review"] = liveTemplate["reviewUrl"]["args"]["post_id"]
+    if live_data_raw["is_end"]:
+        live_data["review"] = live_template["reviewUrl"]["args"].get("post_id")
     else:
         now = datetime.fromtimestamp(time(), TZ)
-        start = datetime.strptime(liveDataRaw["start"], "%Y-%m-%d %H:%M:%S").replace(
+        start = datetime.strptime(live_data_raw["start"], "%Y-%m-%d %H:%M:%S").replace(
             tzinfo=TZ
         )
         if now < start:
-            liveData["start"] = liveDataRaw["start"]
+            live_data["start"] = live_data_raw["start"]
 
-    return liveData
+    return live_data
 
 
-async def getCodes(version: str, actId: str) -> Union[Dict, List[Dict]]:
+async def get_codes(version: str, act_id: str) -> Union[Dict, List[Dict]]:
     """获取兑换码"""
 
-    ret = await getData("code", {"version": version, "actId": actId})
+    ret = await get_data(type="code", data={"version": version, "actId": act_id})
     if ret.get("error") or ret.get("retcode") != 0:
         return {"error": ret.get("error") or "兑换码数据异常"}
 
-    codesData = []
-    for codeInfo in ret["data"]["code_list"]:
-        gifts = findall(
-            r">\s*([\u4e00-\u9fa5]+|\*[0-9]+)\s*\*<",
-            codeInfo["title"].replace("&nbsp;", " "),
-        )
-        codesData.append(
+    codes_data = []
+    for code_info in ret["data"]["code_list"]:
+        codes_data.append(
             {
-                "items": "+".join(g for g in gifts if not g[-1].isdigit()),
-                "code": codeInfo["code"],
+                "items": sub("<.*?>", "", code_info["title"].replace("&nbsp;", " ")),
+                "code": code_info["code"],
             }
         )
 
-    return codesData
+    return codes_data
 
 
-async def getMsg() -> List[MessageSegment]:
+async def get_msg(mhy_type) -> List[MessageSegment]:
     """生成最新前瞻直播兑换码合并转发消息"""
 
-    actId = await getActId()
-    if not actId:
+    act_id = await get_act_id(mhy_type=mhy_type)
+    nickname = "原神前瞻直播" if mhy_type == "gs" else "星穹铁道前瞻直播"
+    if not act_id:
         return [
             MessageSegment.node_custom(
                 user_id=2854196320,
-                nickname="原神前瞻直播",
+                nickname=nickname,
                 content=Message(MessageSegment.text("暂无前瞻直播资讯！")),
             )
         ]
 
-    liveData = await getLiveData(actId)
-    if liveData.get("error"):
+    live_data = await get_live_data(act_id)
+    if live_data.get("error"):
         return [
             MessageSegment.node_custom(
                 user_id=2854196320,
-                nickname="原神前瞻直播",
-                content=Message(MessageSegment.text(liveData["error"])),
+                nickname=nickname,
+                content=Message(MessageSegment.text(live_data["error"])),
             )
         ]
-    elif liveData.get("start"):
+    elif live_data.get("start"):
         return [
             MessageSegment.node_custom(
                 user_id=2854196320,
-                nickname=liveData["title"],
-                content=Message(MessageSegment.image(liveData["header"])),
+                nickname=live_data["title"],
+                content=Message(MessageSegment.image(live_data["header"])),
             ),
             MessageSegment.node_custom(
                 user_id=2854196320,
-                nickname=liveData["title"],
-                content=Message(MessageSegment.text(liveData["room"])),
+                nickname=live_data["title"],
+                content=Message(MessageSegment.text(live_data["room"])),
             ),
         ]
 
-    codesData = await getCodes(liveData["code_ver"], actId)
-    if isinstance(codesData, Dict):
+    codes_data = await get_codes(live_data["code_ver"], act_id)
+    if isinstance(codes_data, Dict):
         return [
             MessageSegment.node_custom(
                 user_id=2854196320,
-                nickname=liveData["title"],
-                content=Message(MessageSegment.text(codesData["error"])),
+                nickname=live_data["title"],
+                content=Message(MessageSegment.text(codes_data["error"])),
             )
         ]
-    codesMsg = [
+    codes_msg = [
         MessageSegment.node_custom(
             user_id=2854196320,
-            nickname=liveData["title"],
+            nickname=live_data["title"],
             content=Message(
                 MessageSegment.text(
-                    f"当前发布了 {len(codesData)} 个兑换码，请在有效期内及时兑换哦~"
+                    f"当前发布了 {len(codes_data)} 个兑换码，请在有效期内及时兑换哦~"
                     + "\n\n* 官方接口数据有 2 分钟左右延迟，请耐心等待下~"
                 )
             ),
         ),
         *[
             MessageSegment.node_custom(
                 user_id=2854196320,
-                nickname=code["items"] or liveData["title"],
+                nickname=code["items"] or live_data["title"],
                 content=Message(MessageSegment.text(code["code"])),
             )
-            for code in codesData
+            for code in codes_data
         ],
     ]
-    if liveData.get("review"):
-        codesMsg.append(
+    if live_data.get("review"):
+        codes_msg.append(
             MessageSegment.node_custom(
                 user_id=2854196320,
-                nickname=liveData["title"],
+                nickname=live_data["title"],
                 content=Message(
                     MessageSegment.text(
                         "直播已经结束，查看回放：\n\n"
-                        + f"https://www.miyoushe.com/ys/article/{liveData['review']}"
+                        + f"https://www.miyoushe.com/ys/article/{live_data['review']}"
                     )
                 ),
             )
         )
-    return codesMsg
+    return codes_msg
```

### Comparing `nonebot_plugin_gscode-0.1.8/pyproject.toml` & `nonebot_plugin_gscode-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gscode"
-version = "0.1.8"
+version = "0.2.0"
 description = "Genshin live codes plugin for NoneBot2"
 authors = ["monsterxcn <monsterxcn@gmail.com>"]
 documentation = "https://github.com/monsterxcn/nonebot-plugin-gscode#readme"
 license = "MIT"
 homepage = "https://github.com/monsterxcn/nonebot-plugin-gscode"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "genshin", "live", "code", "redeem"]
```

### Comparing `nonebot_plugin_gscode-0.1.8/PKG-INFO` & `nonebot_plugin_gscode-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gscode
-Version: 0.1.8
+Version: 0.2.0
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
-Metadata-Version: 2.1 Name: nonebot-plugin-gscode Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gscode Version: 0.2.0 Summary:
 Genshin live codes plugin for NoneBot2 Home-page: https://github.com/
 monsterxcn/nonebot-plugin-gscode License: MIT Keywords:
 nonebot,nonebot2,genshin,live,code,redeem Author: monsterxcn Author-email:
 monsterxcn@gmail.com Requires-Python: >=3.8.1,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

