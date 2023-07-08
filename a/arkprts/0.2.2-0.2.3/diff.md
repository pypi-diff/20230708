# Comparing `tmp/arkprts-0.2.2.tar.gz` & `tmp/arkprts-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.2.2.tar", last modified: Wed Jul  5 22:05:54 2023, max compression
+gzip compressed data, was "arkprts-0.2.3.tar", last modified: Sat Jul  8 21:35:56 2023, max compression
```

## Comparing `arkprts-0.2.2.tar` & `arkprts-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:05:54.174566 arkprts-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 22:05:43.000000 arkprts-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-05 22:05:54.174566 arkprts-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-05 22:05:43.000000 arkprts-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:05:54.166566 arkprts-0.2.2/arkprts/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39793 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16885 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/gamedata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:05:54.170566 arkprts-0.2.2/arkprts/models/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/models/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/models/social.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:05:43.000000 arkprts-0.2.2/arkprts/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:05:54.170566 arkprts-0.2.2/arkprts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-05 22:05:54.000000 arkprts-0.2.2/arkprts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-05 22:05:54.000000 arkprts-0.2.2/arkprts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:05:54.000000 arkprts-0.2.2/arkprts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-05 22:05:54.000000 arkprts-0.2.2/arkprts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 22:05:54.000000 arkprts-0.2.2/arkprts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-05 22:05:43.000000 arkprts-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 22:05:54.174566 arkprts-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 22:05:43.000000 arkprts-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:05:54.174566 arkprts-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-05 22:05:43.000000 arkprts-0.2.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-05 22:05:43.000000 arkprts-0.2.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-05 22:05:43.000000 arkprts-0.2.2/tests/test_gamedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:35:56.260969 arkprts-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-08 21:35:47.000000 arkprts-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-08 21:35:56.260969 arkprts-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-08 21:35:47.000000 arkprts-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:35:56.260969 arkprts-0.2.3/arkprts/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39806 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/gamedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:35:56.260969 arkprts-0.2.3/arkprts/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/models/social.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:35:47.000000 arkprts-0.2.3/arkprts/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:35:56.260969 arkprts-0.2.3/arkprts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-08 21:35:56.000000 arkprts-0.2.3/arkprts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-08 21:35:56.000000 arkprts-0.2.3/arkprts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:35:56.000000 arkprts-0.2.3/arkprts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-08 21:35:56.000000 arkprts-0.2.3/arkprts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 21:35:56.000000 arkprts-0.2.3/arkprts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-08 21:35:47.000000 arkprts-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:35:56.260969 arkprts-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-08 21:35:47.000000 arkprts-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:35:56.260969 arkprts-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-08 21:35:47.000000 arkprts-0.2.3/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-08 21:35:47.000000 arkprts-0.2.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-08 21:35:47.000000 arkprts-0.2.3/tests/test_gamedata.py
```

### Comparing `arkprts-0.2.2/LICENSE` & `arkprts-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.2/PKG-INFO` & `arkprts-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.2.2
+Version: 0.2.3
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: rsa
@@ -41,28 +41,28 @@
 
 ## Usage
 
 ```py
 import arkprts
 
 async def main() -> None:
-    client = arkprts.Client()
+    client = arkprts.Client(gamedata=False)
 
     # search users by nickname
     users = await client.search_players("Doctor", server="en")
     print("User level: ", users[0].level)
 
 
     # =======
 
     # login with email or token
     auth = arkprts.YostarAuth("en")
     await auth.login_with_email_code("doctor@gmail.com")
     # or auth.login_with_token("123456", "abcdefg")
-    client = arkprts.Client(auth=auth)
+    client = arkprts.Client(auth=auth, gamedata=False)
 
     # get logged-in user data
     data = await client.get_data()
     print("Level: ", data.status.level)
 ```
 
 Returned data is in the form of pydantic models, however you can also request raw json with `client.get_raw_player_info()`/`client.get_raw_data()`/... to access even untyped data.
@@ -71,15 +71,15 @@
 
 ```py
 users = await client.search_user("UserName")
 operator = users[0].assist_char_list[0]  # type: arkprts.models.Character
 print(f"Assist operator {operator.static.name} is level {operator.level}")
 ```
 
-To disable downloading static data use `arkprts.Client(gamedata=False)`. To choose the data download location set `client.gamedata = akprts.GameData("/path/to/data")`.
+To disable downloading static data use `arkprts.Client(gamedata=False)`. To choose the data download location set `arkprts.Client(gamedata="/path/to/data")` (`/tmp`/`%TEMP%` is chosen by default).
 
 ArkPRTS supports en, jp, kr, cn and bili servers. However only global/yostar servers (en, jp and kr) can be used without logging in.
 
 ### Frequent usage cases
 
 Get all of my operators.
```

### Comparing `arkprts-0.2.2/README.md` & `arkprts-0.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,28 +28,28 @@
 
 ## Usage
 
 ```py
 import arkprts
 
 async def main() -> None:
-    client = arkprts.Client()
+    client = arkprts.Client(gamedata=False)
 
     # search users by nickname
     users = await client.search_players("Doctor", server="en")
     print("User level: ", users[0].level)
 
 
     # =======
 
     # login with email or token
     auth = arkprts.YostarAuth("en")
     await auth.login_with_email_code("doctor@gmail.com")
     # or auth.login_with_token("123456", "abcdefg")
-    client = arkprts.Client(auth=auth)
+    client = arkprts.Client(auth=auth, gamedata=False)
 
     # get logged-in user data
     data = await client.get_data()
     print("Level: ", data.status.level)
 ```
 
 Returned data is in the form of pydantic models, however you can also request raw json with `client.get_raw_player_info()`/`client.get_raw_data()`/... to access even untyped data.
@@ -58,15 +58,15 @@
 
 ```py
 users = await client.search_user("UserName")
 operator = users[0].assist_char_list[0]  # type: arkprts.models.Character
 print(f"Assist operator {operator.static.name} is level {operator.level}")
 ```
 
-To disable downloading static data use `arkprts.Client(gamedata=False)`. To choose the data download location set `client.gamedata = akprts.GameData("/path/to/data")`.
+To disable downloading static data use `arkprts.Client(gamedata=False)`. To choose the data download location set `arkprts.Client(gamedata="/path/to/data")` (`/tmp`/`%TEMP%` is chosen by default).
 
 ArkPRTS supports en, jp, kr, cn and bili servers. However only global/yostar servers (en, jp and kr) can be used without logging in.
 
 ### Frequent usage cases
 
 Get all of my operators.
```

### Comparing `arkprts-0.2.2/arkprts/__main__.py` & `arkprts-0.2.3/arkprts/__main__.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.2/arkprts/auth.py` & `arkprts-0.2.3/arkprts/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -997,15 +997,15 @@
         super().__init__(max_sessions=max_sessions, network=network)
 
         # load cache file or use provided auth
         self.upcoming_auth = []
         if cache is False:
             self.cache_path = None
         elif isinstance(cache, (pathlib.Path, str)):
-            self.cache_path = pathlib.Path(cache)
+            self.cache_path = pathlib.Path(cache).expanduser()
         elif cache is None:
             self.cache_path = pathlib.Path(tempfile.gettempdir()) / "arkprts_auth_cache.json"
         else:
             self.cache_path = None
             self.upcoming_auth = list(cache)
 
         if self.cache_path:
```

### Comparing `arkprts-0.2.2/arkprts/automation.py` & `arkprts-0.2.3/arkprts/automation.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     for key, value in source.items():
         if isinstance(value, dict):
             recursively_delete_dict(target[key], typing.cast("dict[object, object]", value))
         elif isinstance(value, list):
             for i, v in enumerate(typing.cast("list[object]", value)):
                 if isinstance(v, dict):
                     recursively_delete_dict(target[key][i], typing.cast("dict[object, object]", v))
+                else:
+                    target[key].remove(v)
         else:
             del target[key]
 
 
 # https://github.com/Rhine-Department-0xf/Rhine-DFramwork/blob/main/client/encryption.py
 
 
@@ -217,14 +219,21 @@
     async def building_sync(self) -> typing.Any:
         """Sync base data.
 
         APP behavior: Called when entered the base.
         """
         return await self.request("building/sync")
 
+    async def building_get_assist_report(self) -> typing.Any:
+        """Get base report.
+
+        APP behavior: Called when viewing base report in the control center.
+        """
+        return await self.request("building/getAssistReport")
+
     async def building_assign_char(self, room_slot_id: str, char_inst_id_list: typing.Sequence[int]) -> typing.Any:
         """Assign operators to a room.
 
         room_slot_id: Room slot ID to assign to.
         char_inst_id_list: List of operator instance IDs to assign. -1 for an empty slot.
 
         APP behavior: Called when assigning operators to a room.
@@ -296,14 +305,21 @@
     async def building_get_clue_box(self) -> typing.Any:
         """View clues gifted to your base by your friends.
 
         APP behavior: Called when opening the gifted clue box in the meeting room.
         """
         return await self.request("building/getClueBox")
 
+    async def building_get_daily_clue(self) -> typing.Any:
+        """Get a daily clue.
+
+        APP behavior: Called when claiming the daily clue in the meeting room.
+        """
+        return await self.request("building/getDailyClue")
+
     async def building_receive_clue_to_stock(self, clues: typing.Sequence[str]) -> typing.Any:
         """Claim clues gifted to your base by your friends.
 
         clues: List of clue IDs to claim.
 
         APP behavior: Called when claiming clues from the gifted clue box.
         """
@@ -344,20 +360,79 @@
         APP behavior: Called when visiting a friend's base.
         """
         data = {
             "friendId": friend_id,
         }
         return await self.request("building/visitBuilding", json=data)
 
-    async def building_get_assist_report(self) -> typing.Any:
-        """Get base report.
+    async def building_get_clue_friend_list(self, id_list: typing.Sequence[str]) -> typing.Any:
+        """Get a list of friends able to receive clues.
 
-        App behavior: Called when viewing base report in the control center.
+        APP behavior: Called when viewing the clue board in the meeting room.
         """
-        return await self.request("building/getAssistReport")
+        return await self.request("building/getClueFriendList")
+
+    async def building_send_clue(self, friend_id: str, clue_id: str) -> typing.Any:
+        """Send a clue to a friend.
+
+        friend_id: Friend's ID.
+        clue_id: Clue ID to send.
+
+        APP behavior: Called when sending a clue to a friend.
+        """
+        data = {
+            "friendId": friend_id,
+            "clueId": clue_id,
+        }
+        return await self.request("building/sendClue", json=data)
+
+    async def building_start_info_share(self) -> typing.Any:
+        """Start a clue exchange.
+
+        APP behavior: Called when starting a clue exchange in the meeting room after gathering all clues.
+        """
+        return await self.request("building/startInfoShare")
+
+    async def social_get_friend_list(self, id_list: typing.Sequence[str]) -> typing.Any:
+        """Get a list of friends by ID.
+
+        APP behavior: Called after any request for friend IDs.
+        """
+        data = {
+            "idList": id_list,
+        }
+        return await self.request("social/getFriendList", json=data)
+
+    async def social_receive_social_point(self) -> typing.Any:
+        """Claim daily social shop points.
+
+        APP behavior: Called when claiming the daily social shop points.
+        """
+        return await self.request("social/receiveSocialPoint")
+
+    async def shop_get_social_good_list(self) -> typing.Any:
+        """Get the social shop product list.
+
+        APP behavior: Called when entering the social shop.
+        """
+        return await self.request("shop/getSocialGoodList")
+
+    async def shop_buy_social_good(self, good_id: str, count: int = 1) -> typing.Any:
+        """Buy a social shop product.
+
+        good_id: Product ID.
+        count: Probably amount to buy. This should always be 1.
+
+        APP behavior: Called when buying a social shop product.
+        """
+        data = {
+            "goodId": good_id,
+            "count": count,
+        }
+        return await self.request("shop/buySocialGood", json=data)
 
     async def gacha_sync_normal_gacha(self) -> typing.Any:
         """Sync recruitment data.
 
         APP behavior: Called when entering the recruitment page.
         """
         return await self.request("gacha/syncNormalGacha")
@@ -406,37 +481,14 @@
         APP behavior: Called when finishing a recruitment.
         """
         data = {
             "slotId": slot_id,
         }
         return await self.request("gacha/finishNormalGacha", json=data)
 
-    # Maybe also get daily social points.
-
-    async def shop_get_social_good_list(self) -> typing.Any:
-        """Get the social shop product list.
-
-        APP behavior: Called when entering the social shop.
-        """
-        return await self.request("shop/getSocialGoodList")
-
-    async def shop_buy_social_good(self, good_id: str, count: int = 1) -> typing.Any:
-        """Buy a social shop product.
-
-        good_id: Product ID.
-        count: Probably amount to buy. This should always be 1.
-
-        APP behavior: Called when buying a social shop product.
-        """
-        data = {
-            "goodId": good_id,
-            "count": count,
-        }
-        return await self.request("shop/buySocialGood", json=data)
-
     async def get_battle_replay(self, battle_type: str, stage_id: str) -> typing.Any:
         """Get a replay of a stage.
 
         stage_id: Stage ID.
 
         APP behavior: Called when entering the squad selection screen with auto-deploy enabled.
         """
```

### Comparing `arkprts-0.2.2/arkprts/client.py` & `arkprts-0.2.3/arkprts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,53 +43,60 @@
     gamedata: gd.GameData  # may actually be None, but that's a pain to typehint
     """Game data client."""
 
     def __init__(
         self,
         auth: authn.CoreAuth | None = None,
         *,
-        gamedata: gd.GameData | typing.Literal[False] | None = None,
+        gamedata: gd.GameData | str | typing.Literal[False] | None = None,
         network: authn.NetworkSession | None = None,
         server: authn.ArknightsServer | None = None,
         language: authn.ArknightsLanguage | None = None,
     ) -> None:
         """Initialize a client.
 
         auth: Authentication client. May be both public and private. GuestAuth by default.
-        gamedata: Game data client. May be disabled with False.
+        gamedata: Game data client or path to its location. May be disabled with False.
         network: Network session.
         server: Default server. Not recommended for large-scale usage.
         language: Default language. Fallbacks on the gamedata's default language.
         """
         self.auth = auth or authn.GuestAuth(network=network)
         if gamedata is False:
             self.gamedata = None  # type: ignore
+        elif isinstance(gamedata, gd.GameData):
+            self.gamedata = gamedata
         else:
-            self.gamedata = gamedata or gd.GameData()
+            self.gamedata = gd.GameData(gamedata)
 
         if network:
             self.auth.network = network
         if server:
             self.auth.network.default_server = server
         if language:
             if self.gamedata is None:
                 raise ValueError("No need to use language, gamedata is disabled.")
 
             self.gamedata.language = language
 
     @property
     def network(self) -> authn.NetworkSession:
-        """Return the network of the client."""
+        """Return the network session of the client."""
         return self.auth.network
 
     @property
     def server(self) -> authn.ArknightsServer | None:
-        """Return the default server of the client."""
+        """Return the default server of the network session."""
         return self.network.default_server
 
+    @property
+    def language(self) -> authn.ArknightsLanguage | None:
+        """Return the default language of the gamedata client."""
+        return self.gamedata.language
+
     async def request(self, endpoint: str, **kwargs: typing.Any) -> typing.Any:
         """Send an authenticated request to the arknights game server."""
         if self.gamedata and not self.gamedata.loaded:
             await self.gamedata.update_gamedata()
 
         return await self.auth.auth_request(endpoint, **kwargs)
```

### Comparing `arkprts-0.2.2/arkprts/errors.py` & `arkprts-0.2.3/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.2/arkprts/gamedata.py` & `arkprts-0.2.3/arkprts/gamedata.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     _cache: dict[str, dict[str, models.DDict]]
     """Loaded files."""
     _lock: asyncio.Lock
     """Gamedata update lock."""
 
     def __init__(self, directory: PathLike | None = None, *, language: ArknightsLanguage = "en_US") -> None:
         if directory:
-            self.directory = pathlib.Path(directory)
+            self.directory = pathlib.Path(directory).expanduser()
         else:
             self.directory = pathlib.Path(tempfile.gettempdir()) / "ArknightsGameData"
 
         self.directory.mkdir(parents=True, exist_ok=True)
         self.language = language
         self.loaded = False
         self._cache = {}
@@ -226,8 +226,9 @@
         """Get a module."""
         data = self.get_excel("uniequip_table", language=language)
         return data["equipDict"][id]
 
     def calculate_trust_level(self, trust: int) -> int:
         """Calculate trust level from trust points."""
         frames = self.get_excel("favor_table")["favor_frames"]
-        return bisect.bisect_left(frames, trust, key=lambda x: x["data"]["favor_point"])
+        key_frames = [frame["data"]["favor_point"] for frame in frames]
+        return bisect.bisect_left(key_frames, trust)
```

### Comparing `arkprts-0.2.2/arkprts/models/base.py` & `arkprts-0.2.3/arkprts/models/base.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.2/arkprts/models/data.py` & `arkprts-0.2.3/arkprts/models/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
     """Medal board."""
 
 
 class ConsumableExpire(base.BaseModel):
     """Consumable expiration data."""
 
     ts: typing.Optional[base.ArknightsTimestamp]
-    """When the consumable expires."""
+    """When the consumable expires. Some consumables do not expire."""
     count: int
     """Amount of consumables."""
 
 
 class User(base.BaseModel, extra="ignore"):
     """User sync data. Not fully modeled."""
```

### Comparing `arkprts-0.2.2/arkprts/models/social.py` & `arkprts-0.2.3/arkprts/models/social.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,14 @@
     secretary_skin_id: str = pydantic.Field(alias="secretarySkinId")
     """ID of the secretary operator's skin."""
     resume: str
     """Player display bio."""
     team_v2: typing.Mapping[str, int] = pydantic.Field(alias="teamV2")
     """Amount of characters owned in each faction."""
     board: typing.Sequence[str]
-    """Factions with full trust. Shows up blue in-game."""
+    """Owned clues in the meeting room."""
     info_share: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(alias="infoShare")
     """IDK."""
     recent_visited: bool = pydantic.Field(alias="recentVisited")
     """IDK."""
     info_share_visited: typing.Optional[int] = pydantic.Field(None, alias="infoShareVisited")
     """IDK."""
```

### Comparing `arkprts-0.2.2/arkprts.egg-info/PKG-INFO` & `arkprts-0.2.3/arkprts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.2.2
+Version: 0.2.3
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: rsa
@@ -41,28 +41,28 @@
 
 ## Usage
 
 ```py
 import arkprts
 
 async def main() -> None:
-    client = arkprts.Client()
+    client = arkprts.Client(gamedata=False)
 
     # search users by nickname
     users = await client.search_players("Doctor", server="en")
     print("User level: ", users[0].level)
 
 
     # =======
 
     # login with email or token
     auth = arkprts.YostarAuth("en")
     await auth.login_with_email_code("doctor@gmail.com")
     # or auth.login_with_token("123456", "abcdefg")
-    client = arkprts.Client(auth=auth)
+    client = arkprts.Client(auth=auth, gamedata=False)
 
     # get logged-in user data
     data = await client.get_data()
     print("Level: ", data.status.level)
 ```
 
 Returned data is in the form of pydantic models, however you can also request raw json with `client.get_raw_player_info()`/`client.get_raw_data()`/... to access even untyped data.
@@ -71,15 +71,15 @@
 
 ```py
 users = await client.search_user("UserName")
 operator = users[0].assist_char_list[0]  # type: arkprts.models.Character
 print(f"Assist operator {operator.static.name} is level {operator.level}")
 ```
 
-To disable downloading static data use `arkprts.Client(gamedata=False)`. To choose the data download location set `client.gamedata = akprts.GameData("/path/to/data")`.
+To disable downloading static data use `arkprts.Client(gamedata=False)`. To choose the data download location set `arkprts.Client(gamedata="/path/to/data")` (`/tmp`/`%TEMP%` is chosen by default).
 
 ArkPRTS supports en, jp, kr, cn and bili servers. However only global/yostar servers (en, jp and kr) can be used without logging in.
 
 ### Frequent usage cases
 
 Get all of my operators.
```

### Comparing `arkprts-0.2.2/pyproject.toml` & `arkprts-0.2.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "arkprts"
 requires-python = ">=3.9"
-version = "0.2.2"
+version = "0.2.3"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
@@ -62,42 +62,42 @@
 # S101: Use of assert (type-checking)
 # S110: Try, Except, Pass (annoying)
 # S3xx: Use of random or md5
 # S607: Using git instead of an entire path
 # TRY003: Long exception message
 # UP013: Functional TypedDict
 ignore = [
-  "A",
-  "ARG",
-  "EM",
-  "ERA",
-  "FBT",
-  "SLF",
-  "TCH",
-  "TD",
-  "ANN10",
-  "ANN401",
-  "B008",
-  "B027",
-  "B028",
-  "B905",
-  "C408",
-  "D105",
-  "E501",
-  "N805",
-  "PGH003",
-  "PLR0913",
-  "PLR2004",
-  "PLW2901",
-  "RET504",
-  "S101",
-  "S3",
-  "S607",
-  "TRY003",
-  "UP013",
+    "A",
+    "ARG",
+    "EM",
+    "ERA",
+    "FBT",
+    "SLF",
+    "TCH",
+    "TD",
+    "ANN10",
+    "ANN401",
+    "B008",
+    "B027",
+    "B028",
+    "B905",
+    "C408",
+    "D105",
+    "E501",
+    "N805",
+    "PGH003",
+    "PLR0913",
+    "PLR2004",
+    "PLW2901",
+    "RET504",
+    "S101",
+    "S3",
+    "S607",
+    "TRY003",
+    "UP013",
 ]
 # auto-fixing too intrusive
 # F401: Unused import
 # F841: Unused variable
 # B007: Unused loop variable
 unfixable = ["F401", "F841", "B007"]
```

### Comparing `arkprts-0.2.2/setup.py` & `arkprts-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run setuptools."""
 import pathlib
 
 from setuptools import find_packages, setup
 
 setup(
     name="arkprts",
-    version="0.2.2",
+    version="0.2.3",
     description="Arknights python wrapper.",
     url="https://github.com/thesadru/arkprts",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     package_data={"arkprts": ["py.typed"]},
     install_requires=["aiohttp", "pydantic==2.*"],
     extras_require={"all": ["rsa", "pycryptodome"], "rsa": ["rsa"], "aes": ["pycryptodome"]},
```

### Comparing `arkprts-0.2.2/tests/test_auth.py` & `arkprts-0.2.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.2/tests/test_client.py` & `arkprts-0.2.3/tests/test_client.py`

 * *Files identical despite different names*

