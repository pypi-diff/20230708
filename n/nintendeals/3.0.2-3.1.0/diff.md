# Comparing `tmp/nintendeals-3.0.2.tar.gz` & `tmp/nintendeals-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nintendeals-3.0.2.tar", max compression
+gzip compressed data, was "nintendeals-3.1.0.tar", max compression
```

## Comparing `nintendeals-3.0.2.tar` & `nintendeals-3.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1071 2023-02-27 13:17:12.082213 nintendeals-3.0.2/LICENSE
--rw-r--r--   0        0        0     8209 2023-02-27 13:17:12.082213 nintendeals-3.0.2/README.md
--rw-r--r--   0        0        0        0 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/api/__init__.py
--rw-r--r--   0        0        0     3461 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/api/prices.py
--rw-r--r--   0        0        0        0 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/commons/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/commons/classes/__init__.py
--rw-r--r--   0        0        0     3288 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/commons/classes/eshops.py
--rw-r--r--   0        0        0     1839 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/commons/classes/games.py
--rw-r--r--   0        0        0     1074 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/commons/classes/prices.py
--rw-r--r--   0        0        0      740 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/commons/enumerates.py
--rw-r--r--   0        0        0      107 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noa/__init__.py
--rw-r--r--   0        0        0      114 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noa/api/__init__.py
--rw-r--r--   0        0        0     1930 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noa/api/algolia.py
--rw-r--r--   0        0        0     1454 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noa/info.py
--rw-r--r--   0        0        0      836 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noa/listing.py
--rw-r--r--   0        0        0        0 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noa/scrapers/__init__.py
--rw-r--r--   0        0        0     1028 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noa/scrapers/nintendo.py
--rw-r--r--   0        0        0      942 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noa/search.py
--rw-r--r--   0        0        0     1760 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noa/util.py
--rw-r--r--   0        0        0      107 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noe/__init__.py
--rw-r--r--   0        0        0      117 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noe/api/__init__.py
--rw-r--r--   0        0        0     1965 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noe/api/nintendo.py
--rw-r--r--   0        0        0      820 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noe/info.py
--rw-r--r--   0        0        0      789 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noe/listing.py
--rw-r--r--   0        0        0      895 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noe/search.py
--rw-r--r--   0        0        0     2176 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noe/util.py
--rw-r--r--   0        0        0      107 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noj/__init__.py
--rw-r--r--   0        0        0      117 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noj/api/__init__.py
--rw-r--r--   0        0        0     1159 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noj/api/nintendo.py
--rw-r--r--   0        0        0      745 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noj/info.py
--rw-r--r--   0        0        0      726 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noj/listing.py
--rw-r--r--   0        0        0      833 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noj/search.py
--rw-r--r--   0        0        0     1833 2023-02-27 13:17:12.082213 nintendeals-3.0.2/nintendeals/noj/util.py
--rw-r--r--   0        0        0     1053 2023-02-27 13:17:12.082213 nintendeals-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     9607 1970-01-01 00:00:00.000000 nintendeals-3.0.2/setup.py
--rw-r--r--   0        0        0     9424 1970-01-01 00:00:00.000000 nintendeals-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-08 11:59:27.068711 nintendeals-3.1.0/LICENSE
+-rw-r--r--   0        0        0     8209 2023-07-08 11:59:27.068711 nintendeals-3.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/api/__init__.py
+-rw-r--r--   0        0        0     3461 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/api/prices.py
+-rw-r--r--   0        0        0        0 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/classes/__init__.py
+-rw-r--r--   0        0        0     3285 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/classes/eshops.py
+-rw-r--r--   0        0        0     1839 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/classes/games.py
+-rw-r--r--   0        0        0     1074 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/classes/prices.py
+-rw-r--r--   0        0        0      762 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/enumerates.py
+-rw-r--r--   0        0        0      107 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/api/__init__.py
+-rw-r--r--   0        0        0     2089 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/api/algolia.py
+-rw-r--r--   0        0        0     1482 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/info.py
+-rw-r--r--   0        0        0      870 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/listing.py
+-rw-r--r--   0        0        0        0 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/scrapers/__init__.py
+-rw-r--r--   0        0        0     1075 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/scrapers/nintendo.py
+-rw-r--r--   0        0        0      976 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/search.py
+-rw-r--r--   0        0        0     1900 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/util.py
+-rw-r--r--   0        0        0      107 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/__init__.py
+-rw-r--r--   0        0        0      117 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/api/__init__.py
+-rw-r--r--   0        0        0     1927 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/api/nintendo.py
+-rw-r--r--   0        0        0      846 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/info.py
+-rw-r--r--   0        0        0      811 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/listing.py
+-rw-r--r--   0        0        0      917 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/search.py
+-rw-r--r--   0        0        0     2248 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/util.py
+-rw-r--r--   0        0        0      107 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/__init__.py
+-rw-r--r--   0        0        0      117 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/api/__init__.py
+-rw-r--r--   0        0        0     1159 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/api/nintendo.py
+-rw-r--r--   0        0        0      744 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/info.py
+-rw-r--r--   0        0        0      725 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/listing.py
+-rw-r--r--   0        0        0      832 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/search.py
+-rw-r--r--   0        0        0     1832 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/util.py
+-rw-r--r--   0        0        0     1085 2023-07-08 11:59:27.068711 nintendeals-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9607 1970-01-01 00:00:00.000000 nintendeals-3.1.0/setup.py
+-rw-r--r--   0        0        0     9424 1970-01-01 00:00:00.000000 nintendeals-3.1.0/PKG-INFO
```

### Comparing `nintendeals-3.0.2/LICENSE` & `nintendeals-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nintendeals-3.0.2/README.md` & `nintendeals-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nintendeals-3.0.2/nintendeals/api/prices.py` & `nintendeals-3.1.0/nintendeals/api/prices.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.0.2/nintendeals/commons/classes/eshops.py` & `nintendeals-3.1.0/nintendeals/commons/classes/eshops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 class NAeShop:
-
     FORMAT = "https://www.nintendo.com/{lang}_{country}/games/detail/{slug}"
 
     def __init__(self, game: "Game"):
         self.game = game
 
     @property
     def ca_en(self) -> str:
@@ -15,15 +14,14 @@
 
     @property
     def us_en(self) -> str:
         return NAeShop.FORMAT.format(lang="en", country="US", slug=self.game.slug)
 
 
 class EUeShop:
-
     FORMAT_NO_LANG = "https://www.nintendo.{domain}{slug}"
     FORMAT_LANG = "https://www.nintendo.{domain}/{lang}{slug}"
 
     FORMAT_ALT = "https://ec.nintendo.com/{country}/{lang}/titles/{nsuid}"
 
     def __init__(self, game: "Game"):
         self.game = game
@@ -94,15 +92,14 @@
 
     @property
     def nz_en(self) -> str:
         return EUeShop.FORMAT_ALT.format(country="NZ", lang="en", nsuid=self.game.nsuid)
 
 
 class JPeShop:
-
     NEW_FORMAT = "https://store-jp.nintendo.com/list/software/{nsuid}.html"
     OLD_FORMAT = "https://www.nintendo.co.jp/titles/{nsuid}"
 
     def __init__(self, game: "Game"):
         self.game = game
 
     @property
```

### Comparing `nintendeals-3.0.2/nintendeals/commons/classes/games.py` & `nintendeals-3.1.0/nintendeals/commons/classes/games.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.0.2/nintendeals/commons/classes/prices.py` & `nintendeals-3.1.0/nintendeals/commons/classes/prices.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.0.2/nintendeals/commons/enumerates.py` & `nintendeals-3.1.0/nintendeals/commons/enumerates.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from enum import Enum
 
 
 class Features(str, Enum):
     AMIIBO = "Amiibo Supported"
     DEMO = "Demo Available"
     DLC = "DLC Available"
-    NSO_REQUIRED = "Nintendo Switch Online Required"
+    GAME_VOUCHER = "Game Voucher Eligible"
+    ONLINE_PLAY = "Online Play"
     SAVE_DATA_CLOUD = "Save Data Cloud Supported"
     VOICE_CHAT = "Voice Chat Supported"
 
     def __str__(self):
         return str(self.value)
```

### Comparing `nintendeals-3.0.2/nintendeals/noa/api/algolia.py` & `nintendeals-3.1.0/nintendeals/noa/api/algolia.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from algoliasearch.search_client import SearchClient
 
 from nintendeals.commons.enumerates import Platforms
 
 APP_ID = "U3B6GR4UA3"
 API_KEY = "a29c6927638bfd8cee23993e51e721c9"
 
-INDEX_NAME = "ncom_game_en_us"
+INDEX_NAME = "store_game_en_us"
 INDEX = None
 
 
 PLATFORMS = {
     Platforms.NINTENDO_SWITCH: "Nintendo Switch",
 }
 
@@ -41,49 +41,57 @@
 
     platform_code = PLATFORM_CODES[platform]
 
     options = {
         "allowTyposOnNumericTokens": False,
         "queryType": "prefixAll",
         "restrictSearchableAttributes": ["nsuid"],
-        "facetFilters": [f"platform:{PLATFORMS[platform]}"],
         "hitsPerPage": 500,
     }
 
     current = -1
 
     while True:
         current += 1
         query = f"{platform_code}{current:07}"
-        games = _search_index(query, **options)
+        items = _search_index(query, **options)
 
-        if not games:
+        if not items:
             empty_pages += 1
 
         if empty_pages == 5:
             break
 
-        yield from games
+        for item in items:
+            if item["platform"] != platform:
+                continue
+
+            yield item
 
 
 def search_by_query(query: str, platform: Platforms = None) -> Iterator[dict]:
     hits_per_page = 50
 
     options = {
         "hitsPerPage": hits_per_page,
     }
 
-    if platform:
-        options["facetFilters"] = [f"platform:{PLATFORMS[platform]}"]
-
     page = -1
 
     while True:
         page += 1
         options["page"] = page
 
-        games = _search_index(query, **options)
+        items = _search_index(query, **options)
+
+        for item in items:
+            if item["topLevelCategoryCode"] != "GAMES":
+                continue
+
+            if platform:
+                if item["platform"] != platform:
+                    continue
 
-        yield from games
+            yield item
 
-        if len(games) < hits_per_page:
+        if len(items) < hits_per_page:
             break
```

### Comparing `nintendeals-3.0.2/nintendeals/noa/info.py` & `nintendeals-3.1.0/nintendeals/noa/info.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def game_info_by_nsuid(nsuid: str) -> Optional[Game]:
     data = algolia.search_by_nsuid(nsuid)
 
     if not data:
         return None
 
-    data["extra"] = nintendo.scrap(data["slug"])
+    data["extra"] = nintendo.scrap(data["urlKey"])
 
     return build_game(data)
 
 
 def game_info_by_slug(slug: str) -> Optional[Game]:
     extra = nintendo.scrap(slug)
     nsuid = extra.get("nsuid")
@@ -40,15 +40,16 @@
     its information from Nintendo of America.
 
     Available Features
     ------------------
         * Nintendo Switch
             - DEMO
             - DLC
-            - NSO_REQUIRED
+            - GAME_VOUCHER
+            - ONLINE_PLAY
             - SAVE_DATA_CLOUD
 
     Parameters
     ----------
     nsuid: str
         Valid nsuid of a nintendo game.
     slug: str
```

### Comparing `nintendeals-3.0.2/nintendeals/noa/listing.py` & `nintendeals-3.1.0/nintendeals/noa/search.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 
 from nintendeals.commons.classes.games import Game
 from nintendeals.commons.enumerates import Platforms
 from nintendeals.noa.api import algolia
 from nintendeals.noa.util import build_game
 
 
-def list_games(platform: Platforms) -> Iterator[Game]:
-    for data in algolia.search_by_platform(platform):
+def search_games(query: str, platform: Platforms) -> Iterator[Game]:
+    for data in algolia.search_by_query(query, platform):
         yield build_game(data)
 
 
-def list_switch_games() -> Iterator[Game]:
+def search_switch_games(query: str) -> Iterator[Game]:
     """
-    Get a list of Nintendo Switch games for the NA region.
+    Search for Nintendo Switch games in the NA region.
 
     Note: game.product_code is unavailable with this method, to get it use the
     method noa.game_info(nsuid).
 
     Available Features
     ------------------
         * DEMO
-        * DLC
-        * NSO_REQUIRED
+        * GAME_VOUCHER
+        * ONLINE_PLAY
+        * SAVE_DATA_CLOUD
+
+    Parameters
+    ----------
+    query: str
+        Text to search.
 
     Yields
     -------
     nintendeals.classes.common.Game:
         Information of a game.
     """
-    yield from list_games(Platforms.NINTENDO_SWITCH)
+
+    yield from search_games(query, Platforms.NINTENDO_SWITCH)
```

### Comparing `nintendeals-3.0.2/nintendeals/noa/search.py` & `nintendeals-3.1.0/nintendeals/noe/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from typing import Iterator
 
 from nintendeals.commons.classes.games import Game
 from nintendeals.commons.enumerates import Platforms
-from nintendeals.noa.api import algolia
-from nintendeals.noa.util import build_game
+from nintendeals.noe.api import nintendo
+from nintendeals.noe.util import build_game
 
 
 def search_games(query: str, platform: Platforms) -> Iterator[Game]:
-    for data in algolia.search_by_query(query, platform):
+    for data in nintendo.search_by_query(query, platform):
         yield build_game(data)
 
 
 def search_switch_games(query: str) -> Iterator[Game]:
     """
-    Search for Nintendo Switch games in the NA region.
-
-    Note: game.product_code is unavailable with this method, to get it use the
-    method noa.game_info(nsuid).
+    Search for Nintendo Switch games in the EU region.
 
     Available Features
     ------------------
+        * AMIIBO
         * DEMO
         * DLC
-        * NSO_REQUIRED
+        * GAME_VOUCHER
+        * ONLINE_PLAY
+        * SAVE_DATA_CLOUD
+        * VOICE_CHAT
 
     Parameters
     ----------
     query: str
         Text to search.
 
     Yields
```

### Comparing `nintendeals-3.0.2/nintendeals/noa/util.py` & `nintendeals-3.1.0/nintendeals/noj/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,77 @@
-import re
 from datetime import datetime
 from typing import Dict
 
 from nintendeals.commons.classes.games import Game
 from nintendeals.commons.enumerates import Features, Platforms, Ratings, Regions
 
 PLATFORMS = {
-    "Nintendo Switch": Platforms.NINTENDO_SWITCH,
+    "1_HAC": Platforms.NINTENDO_SWITCH,
+}
+
+RATINGS = {
+    "0": None,
+    "1": "A",
+    "2": "B",
+    "3": "C",
+    "4": "D",
+    "5": "Z",
 }
 
 
 def build_game(data: Dict) -> Game:
-    extra = data.get("extra", {})
+    hard = data.get("hard")
+    icode = data.get("icode")
+
+    if hard and icode:
+        product_code = hard[2:] + icode
+    else:
+        product_code = None
 
     game = Game(
-        platform=PLATFORMS[data["platform"]],
-        region=Regions.NA,
+        platform=PLATFORMS[hard],
+        region=Regions.JP,
         title=data["title"],
         nsuid=data.get("nsuid"),
-        product_code=extra.get("product_code"),
+        product_code=product_code,
     )
 
-    game.description = data.get("description")
-    game.slug = data.get("slug")
-    game.free_to_play = data.get("free_to_start", False)
+    game.description = data.get("text")
+    game.slug = data.get("icode")
+    game.free_to_play = data.get("price") == 0.0
 
     # Players
-    try:
-        game.players = int(re.sub(r"[^\d]*", "", data["numOfPlayers"]))
-    except (KeyError, ValueError):
-        game.players = 0
+    players = data.get("player") or ["0"]
+    game.players = max(map(int, players[0].split("~")))
 
     # Release Date
     try:
-        release_date = data["releaseDateDisplay"].split("T")[0]
-        game.release_date = datetime.strptime(release_date, "%Y-%m-%d")
-    except (KeyError, ValueError):
+        game.release_date = datetime.strptime(data.get("sdate"), "%Y.%m.%d")
+    except (ValueError, TypeError):
         game.release_date = None
 
     # Categories
-    game.categories = data.get("genres", [])
+    game.categories = data.get("genre", [])
 
     # Developer
-    game.developers = data.get("developers", [])
+    developer = data.get("maker")
+    game.developers = [developer] if developer else []
 
     # Languages
-    game.languages = extra.get("languages", [])
+    game.languages = data.get("lang", [])
 
     # Publisher
-    game.publishers = data.get("publishers", [])
+    publisher = data.get("publisher")
+    game.publishers = [publisher] if publisher else []
 
-    # Rating (ESRB)
-    game.rating = (Ratings.ESRB, data.get("esrbRating"))
+    # Rating (CERO)
+    rating = data.get("cero") or ["0"]
+    game.rating = (Ratings.CERO, RATINGS.get(rating[0]))
 
     # Features
-    filters = data.get("generalFilters", [])
-
     game.features = {
-        Features.DEMO: "Demo available" in filters,
-        Features.DLC: "DLC available" in filters,
-        Features.NSO_REQUIRED: "Nintendo Switch Online compatible" in filters,
-        Features.SAVE_DATA_CLOUD: extra.get("save_data_cloud"),
+        Features.AMIIBO: data.get("amiibo", "0") == "1",
+        Features.DLC: len(data.get("cnsuid") or []) > 0,
+        Features.ONLINE_PLAY: (data.get("nso") or ["0"]) == ["1"],
     }
 
     return game
```

### Comparing `nintendeals-3.0.2/nintendeals/noe/api/nintendo.py` & `nintendeals-3.1.0/nintendeals/noe/api/nintendo.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,15 @@
     Platforms.NINTENDO_SWITCH: "Switch",
 }
 
 PRODUCT_CODE_PREFIXES = "HAC"
 NSUIDS_PREFIXES = "700"
 
 
-def _search(
-    query: str = "*", nsuid: str = None, platform: Platforms = None
-) -> Iterator[dict]:
+def _search(query: str = "*", nsuid: str = None, platform: Platforms = None) -> Iterator[dict]:
     rows = 200
 
     params = {
         "fq": "type:GAME",
         "q": query,
         "rows": rows,
         "sort": "title asc",
@@ -46,17 +44,15 @@
 
         if not len(json):
             break
 
         for data in json:
             nsuids = data.get("nsuid_txt", [])
             product_codes = data["product_code_txt"] = [
-                pc.replace("-", "")
-                for pc in data.get("product_code_txt", [])
-                if pc[:3] in PRODUCT_CODE_PREFIXES
+                pc.replace("-", "") for pc in data.get("product_code_txt", []) if pc[:3] in PRODUCT_CODE_PREFIXES
             ]
 
             if not any((nsuids, product_codes)):
                 continue
 
             data["nsuid_txt"] = nsuids[0] if nsuids else 0
             data["product_code_txt"] = product_codes[0] if product_codes else 0
```

### Comparing `nintendeals-3.0.2/nintendeals/noe/info.py` & `nintendeals-3.1.0/nintendeals/noj/info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 from typing import Optional
 
 from nintendeals.commons.classes.games import Game
-from nintendeals.noe.api import nintendo
-from nintendeals.noe.util import build_game
+from nintendeals.noj.api import nintendo
+from nintendeals.noj.util import build_game
 
 
 def game_info(nsuid: str) -> Optional[Game]:
     """
-    Given a game's `nsuid` for the EU region, it will retrieve its information
-    from Nintendo of Europe.
+    Given a game's `nsuid` for the JP region, it will retrieve its information
+    from Nintendo of Japan.
 
     Available Features
     ------------------
         * Nintendo Switch
             - AMIIBO
-            - DEMO
             - DLC
-            - NSO_REQUIRED
-            - SAVE_DATA_CLOUD
-            - VOICE_CHAT
+            - ONLINE_PLAY
 
     Parameters
     ----------
     nsuid: str
         Valid nsuid of a nintendo game.
 
     Returns
     -------
     nintendeals.classes.common.Game:
         Information of the game.
     """
-    data = nintendo.search_by_nsuid(nsuid)
 
+    data = nintendo.search_by_nsuid(nsuid)
     return build_game(data) if data else None
```

### Comparing `nintendeals-3.0.2/nintendeals/noe/listing.py` & `nintendeals-3.1.0/nintendeals/noj/listing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from typing import Iterator
 
 from nintendeals.commons.classes.games import Game
 from nintendeals.commons.enumerates import Platforms
-from nintendeals.noe.api import nintendo
-from nintendeals.noe.util import build_game
+from nintendeals.noj.api import nintendo
+from nintendeals.noj.util import build_game
 
 
 def list_games(platform: Platforms) -> Iterator[Game]:
     for data in nintendo.search_by_platform(platform):
         yield build_game(data)
 
 
 def list_switch_games() -> Iterator[Game]:
     """
-    Get a list of Nintendo Switch games for the EU region.
+    Get a list of Nintendo WiiU games for the JP region.
 
     Available Features
     ------------------
         * AMIIBO
-        * DEMO
         * DLC
-        * NSO_REQUIRED
-        * SAVE_DATA_CLOUD
-        * VOICE_CHAT
+        * ONLINE_PLAY
 
     Yields
     -------
     nintendeals.classes.common.Game:
         Information of a game.
     """
+
     yield from list_games(Platforms.NINTENDO_SWITCH)
```

### Comparing `nintendeals-3.0.2/nintendeals/noe/search.py` & `nintendeals-3.1.0/nintendeals/noj/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from typing import Iterator
 
 from nintendeals.commons.classes.games import Game
 from nintendeals.commons.enumerates import Platforms
-from nintendeals.noe.api import nintendo
-from nintendeals.noe.util import build_game
+from nintendeals.noj.api import nintendo
+from nintendeals.noj.util import build_game
 
 
 def search_games(query: str, platform: Platforms) -> Iterator[Game]:
     for data in nintendo.search_by_query(query, platform):
         yield build_game(data)
 
 
 def search_switch_games(query: str) -> Iterator[Game]:
     """
-    Search for Nintendo Switch games in the EU region.
+    Search for Nintendo Switch games in the JP region.
 
     Available Features
     ------------------
         * AMIIBO
-        * DEMO
         * DLC
-        * NSO_REQUIRED
-        * SAVE_DATA_CLOUD
-        * VOICE_CHAT
+        * ONLINE_PLAY
 
     Parameters
     ----------
     query: str
         Text to search.
 
     Yields
```

### Comparing `nintendeals-3.0.2/nintendeals/noe/util.py` & `nintendeals-3.1.0/nintendeals/noe/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,13 +65,14 @@
     game.rating = (Ratings.PEGI, data.get("age_rating_sorting_i"))
 
     # Features
     game.features = {
         Features.AMIIBO: data.get("near_field_comm_b", False),
         Features.DEMO: data.get("demo_availability", False),
         Features.DLC: data.get("add_on_content_b", False),
-        Features.NSO_REQUIRED: data.get("paid_subscription_required_b", False),
+        Features.GAME_VOUCHER: data.get("switch_game_voucher_b", False),
+        Features.ONLINE_PLAY: data.get("paid_subscription_required_b", False),
         Features.SAVE_DATA_CLOUD: data.get("cloud_saves_b", False),
         Features.VOICE_CHAT: data.get("voice_chat_b", False),
     }
 
     return game
```

### Comparing `nintendeals-3.0.2/nintendeals/noj/api/nintendo.py` & `nintendeals-3.1.0/nintendeals/noj/api/nintendo.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.0.2/nintendeals/noj/listing.py` & `nintendeals-3.1.0/nintendeals/noa/listing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from typing import Iterator
 
 from nintendeals.commons.classes.games import Game
 from nintendeals.commons.enumerates import Platforms
-from nintendeals.noj.api import nintendo
-from nintendeals.noj.util import build_game
+from nintendeals.noa.api import algolia
+from nintendeals.noa.util import build_game
 
 
 def list_games(platform: Platforms) -> Iterator[Game]:
-    for data in nintendo.search_by_platform(platform):
+    for data in algolia.search_by_platform(platform):
         yield build_game(data)
 
 
 def list_switch_games() -> Iterator[Game]:
     """
-    Get a list of Nintendo WiiU games for the JP region.
+    Get a list of Nintendo Switch games for the NA region.
+
+    Note: game.product_code is unavailable with this method, to get it use the
+    method noa.game_info(nsuid).
 
     Available Features
     ------------------
-        * AMIIBO
-        * DLC
-        * NSO_REQUIRED
+        * DEMO
+        * GAME_VOUCHER
+        * ONLINE_PLAY
+        * SAVE_DATA_CLOUD
 
     Yields
     -------
     nintendeals.classes.common.Game:
         Information of a game.
     """
-
     yield from list_games(Platforms.NINTENDO_SWITCH)
```

### Comparing `nintendeals-3.0.2/nintendeals/noj/search.py` & `nintendeals-3.1.0/nintendeals/noe/info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from typing import Iterator
+from typing import Optional
 
 from nintendeals.commons.classes.games import Game
-from nintendeals.commons.enumerates import Platforms
-from nintendeals.noj.api import nintendo
-from nintendeals.noj.util import build_game
+from nintendeals.noe.api import nintendo
+from nintendeals.noe.util import build_game
 
 
-def search_games(query: str, platform: Platforms) -> Iterator[Game]:
-    for data in nintendo.search_by_query(query, platform):
-        yield build_game(data)
-
-
-def search_switch_games(query: str) -> Iterator[Game]:
+def game_info(nsuid: str) -> Optional[Game]:
     """
-    Search for Nintendo Switch games in the JP region.
+    Given a game's `nsuid` for the EU region, it will retrieve its information
+    from Nintendo of Europe.
 
     Available Features
     ------------------
-        * AMIIBO
-        * DLC
-        * NSO_REQUIRED
+        * Nintendo Switch
+            - AMIIBO
+            - DEMO
+            - DLC
+            - GAME_VOUCHER
+            - ONLINE_PLAY
+            - SAVE_DATA_CLOUD
+            - VOICE_CHAT
 
     Parameters
     ----------
-    query: str
-        Text to search.
+    nsuid: str
+        Valid nsuid of a nintendo game.
 
-    Yields
+    Returns
     -------
     nintendeals.classes.common.Game:
-        Information of a game.
+        Information of the game.
     """
+    data = nintendo.search_by_nsuid(nsuid)
 
-    yield from search_games(query, Platforms.NINTENDO_SWITCH)
+    return build_game(data) if data else None
```

### Comparing `nintendeals-3.0.2/pyproject.toml` & `nintendeals-3.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "nintendeals"
 description = "Scraping tools for Nintendo Switch games and prices on NA, EU and JP."
 documentation = "https://github.com/fedecalendino/nintendeals/blob/main/README.md"
 homepage = "https://github.com/fedecalendino/nintendeals"
 license = "MIT"
 readme = "README.md"
-version = "3.0.2"
+version = "3.1.0"
 
 authors = [
   "Fede Calendino <fede@calendino.com>",
 ]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
@@ -23,22 +23,25 @@
 ]
 packages = [
   { include = "nintendeals" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-algoliasearch = "^2.6.2"
+algoliasearch = "^3.0.0"
 beautifulsoup4 = "^4.11.1"
 pycountry = "^22.3.5"
 python-dateutil = "^2.8.2"
 requests = "^2.28.1"
 xmltodict = "^0.13.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.6.0"
-coverage = "^6.4.1"
+black = "^23.3.0"
+coverage = "^7.2.7"
 ddt = "^1.5.0"
 
+[tool.black]
+line-length = 120
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nintendeals-3.0.2/setup.py` & `nintendeals-3.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,24 +14,24 @@
  'nintendeals.noj',
  'nintendeals.noj.api']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['algoliasearch>=2.6.2,<3.0.0',
+['algoliasearch>=3.0.0,<4.0.0',
  'beautifulsoup4>=4.11.1,<5.0.0',
  'pycountry>=22.3.5,<23.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'requests>=2.28.1,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0']
 
 setup_kwargs = {
     'name': 'nintendeals',
-    'version': '3.0.2',
+    'version': '3.1.0',
     'description': 'Scraping tools for Nintendo Switch games and prices on NA, EU and JP.',
     'long_description': ' # nintendeals\n> "nintendeals was a bot, he loved learning and deals on nintendo\'s eshop." **LetsFunHans** 💬️\n\n[![Version](https://img.shields.io/pypi/v/nintendeals?logo=pypi)](https://pypi.org/project/nintendeals)\n[![Quality Gate Status](https://img.shields.io/sonar/alert_status/fedecalendino_nintendeals?logo=sonarcloud&server=https://sonarcloud.io)](https://sonarcloud.io/dashboard?id=fedecalendino_nintendeals)\n[![CodeCoverage](https://img.shields.io/sonar/coverage/fedecalendino_nintendeals?logo=sonarcloud&server=https://sonarcloud.io)](https://sonarcloud.io/dashboard?id=fedecalendino_nintendeals)\n\n-----\n\nNamed after the my old [reddit bot](https://reddit.com/u/nintendeals), nintendeals is now a library with \nall the scrapers and integrations of nintendo services that I used.\n\n\n## Terminology\n\nBefore getting into any details first we need too get into the same page with a few terms:\n\n### Region\n\nHere we have three regions NA, EU and JP each one corresponding to Nintendo of America (NoA), Nintendo of Europe (NoE)\nand Nintendo of Japan (NoJ). Each of these regions have set of countries they are "in charge of":\n\nNoA:\n  * Canada\n  * Mexico\n  * United Stated\n  \nNoE:\n  * Every country in the European Union\n  * Australia\n  * New Zealand\n  * South Africa\n  \nNoJ:\n  * Japan\n  \n### nsuid\n\nAn nsuid is a 14 digit long string which Nintendo uses to identify games on each region. \nTaking Breath of the Wild as an example, we have these 3 nsuids for it (one per region):\n\n```    \n  * 70010000000025 (NA)\n  * 70010000000023 (EU)\n  * 70010000000026 (JP)\n```\n    \n### Product Code\n\nThe product code is another type of ID that Nintendo uses, it usually is a 8/9 character long string.\nTaking Splatoon 2 as an example, we have these 3 product codes for it (one per region):\n\n```\n  * HACPAAB6B (NA)\n  * HACPAAB6C (EU)\n  *  HACAAB6A (JP)\n```\n\nThe difference with the nsuid is that the product code has a constant between all regions (`AAB6` in this example), \nand this is what I decided to call [unique_id](https://github.com/fedecalendino/nintendeals/blob/master/nintendeals/commons/classes/games.py#L56) \nand it is what we can you to join a game across all regions.\n\nYou can also see this code in the front of your Nintendo Switch [cartridge](https://media.karousell.com/media/photos/products/2019/08/17/splatoon_2_cartridge_only_1566040350_4f38e061_progressive.jpg).\n\n## Services\n\nThis library provides three types of services: Info, Listing, Searching and Pricing. Each region has a different \nversion of Info, Listing and Searching, but Pricing is the same for all as it only requires a country and an nsuid.\n\n### Listing\n\nEven thought there are different version for each region, they all work in the same way. Given a supported \nplatform ([for this library](https://github.com/fedecalendino/nintendeals/blob/master/nintendeals/constants.py#L15))\nthey will retrieve a list games in the selected region (in the form of an iterator).\n\n```python\nfrom nintendeals import noa\n\nfor game in noa.list_switch_games():\n    print(game.title, "/", game.nsuid)\n```\n\n```text\n>> ARMS / 70010000000392\n>> Astro Duel Deluxe / 70010000000301\n>> Axiom Verge / 70010000000821\n>> Azure Striker GUNVOLT: STRIKER PACK / 70010000000645\n>> Beach Buggy Racing / 70010000000721\n```\n\n```python\nfrom nintendeals import noe\n\nfor game in noe.list_switch_games():\n    print(game.title, "/", game.nsuid)\n```\n\n```text\n>> I and Me / 70010000000314\n>> In Between / 70010000009184\n>> Ghost 1.0 / 70010000001386\n>> Resident Evil 0 / 70010000012848\n>> 64.0 / 70010000020867\n```\n\n### Searching\n\nBuilt on top of the listing services, these provide a simple way to search for games by title or release_date:\n\n```python\nfrom nintendeals import noa\n\nfor game in noa.search_switch_games(query="Zelda"):\n    print(game.title, "/", game.nsuid)\n```\n\n```text\n>> The Legend of Zelda™: Link’s Awakening / 70010000020033\n>> The Legend of Zelda™: Link\'s Awakening: Dreamer Edition / None\n>> Cadence of Hyrule: Crypt of the NecroDancer Featuring The Legend of Zelda / 70010000021364\n>> The Legend of Zelda™: Breath of the Wild / 70010000000025\n```\n\n\n### Info\n\nOnce you have the nsuid of the game that you want, you can call the `game_info` service. And again, each region has their\nown version but they all work the same, but keep in mind that you need to use the correct nsuid for each region.\nComing back to the nsuid of Breath of the Wild as an example:\n\n```python\nfrom nintendeals import noa\n\ngame = noa.game_info("70010000000025")\nprint(game.title)\nprint(game.product_code, game.unique_id)\nprint(game.release_date)\nprint(game.players)\nprint(str(game.rating[0]), game.rating[1])\nprint(game.eshop.ca_fr)\n\nfor feature, value in game.features.items():\n    print(" *", str(feature), ":", value)\n```\n\n```text\n>> The Legend of Zelda™: Breath of the Wild\n>> HACPAAAAA AAAA\n>> 2017-03-03 00:00:00\n>> 1\n>> ESRB Everyone 10+\n>> https://www.nintendo.com/fr_CA/games/detail/the-legend-of-zelda-breath-of-the-wild-switch\n>>  * Demo Available : False\n>>  * DLC Available : False\n>>  * Nintendo Switch Online Required : True\n>>  * Save Data Cloud Supported : True\n```\n\n```python\nfrom nintendeals import noe\n\ngame = noe.game_info("70010000000023")\nprint(game.title)\nprint(game.product_code, game.unique_id)\nprint(game.release_date)\nprint(game.players)\nprint(str(game.rating[0]), game.rating[1])\nprint(game.eshop.uk_en)\n\nfor feature, value in game.features.items():\n    print(" *", str(feature), ":", value)\n```\n\n```text\n>> The Legend of Zelda: Breath of the Wild\n>> HACPAAAAA AAAA\n>> 2017-03-03 00:00:00\n>> 1\n>> PEGI 12\n>> https://www.nintendo.co.uk/Games/Nintendo-Switch/The-Legend-of-Zelda-Breath-of-the-Wild-1173609.html\n>>  * Amiibo Supported : True\n>>  * Demo Available : False\n>>  * DLC Available : False\n>>  * Nintendo Switch Online Required : False\n>>  * Save Data Cloud Supported : True\n>>  * Voice Chat Supported : False\n```\n\n```python\nfrom nintendeals import noj\n\ngame = noj.game_info("70010000000026")\nprint(game.title)\nprint(game.product_code, game.unique_id)\nprint(game.release_date)\nprint(game.players)\nprint(str(game.rating[0]), game.rating[1])\nprint(game.eshop.jp_jp)\n\nfor feature, value in game.features.items():\n    print(" *", str(feature), ":", value)\n```\n\n```text\n>> ゼルダの伝説\u3000ブレス オブ ザ ワイルド\n>> HACAAAAA AAAA\n>> 2017-03-03 00:00:00\n>> 1\n>> CERO B\n>> https://store-jp.nintendo.com/list/software/70010000000026.html\n>>  * Amiibo Supported : True\n>>  * DLC Available : True\n>>  * Nintendo Switch Online Required : False\n```\n\n\n### Pricing\n\nGiven a country code (using the alpha-2 iso standard) and a game or list of games this service will fetch the current \npricing of that/those games for that country. Since this service uses nsuids to fetch the price, make sure that the\ngames that you provide have the regional nsuid that matches the country that you want. For example, only the nsuid for\nthe American region will be able to fetch you the prices of Canada, Mexico and United Stated but not for Japan or Spain.\n\n```python\nfrom nintendeals import noe\nfrom nintendeals.api import prices\n\ngame = noe.game_info("70010000007705")\nprint(game.title)\nprint()\n\nprice = prices.get_price(game, country="CZ")  # Czech Republic\nprint(price.currency)\nprint(price.value)\nprint(price.sale_discount, "%")\nprint(price.sale_value)\nprint(price.sale_start)\nprint(price.sale_end)\n\n# Alternatively you can do this for the same effect:\nprice = game.price(country="CZ") \n``` \n\n```text\nDead Cells\n\nCZK\n625.0\n80 %\n500.0\n2020-04-19 22:00:00\n2020-05-03 21:59:59\n```\n\nTo reduce the amount of call to the prices api, you can also use the `get_prices` service that works in a similar way\nbut it expects a list of games instead of only one:\n\n```python\nfrom nintendeals import noa\nfrom nintendeals.api import prices\n\nbotw = noa.game_info("70010000000025")\nprint(botw.title)\nceleste = noa.game_info("70010000006442")\nprint(celeste.title)\n\nprint()\n\nprices = prices.get_prices([botw, celeste], country="US")\nfor nsuid, price in prices:\n    print(nsuid)\n    print(price.value)\n    print(price.sale_value)\n    print()\n```\n\n```text\nThe Legend of Zelda™: Breath of the Wild\nCeleste\n\n70010000000025\n59.99\nNone\n\n70010000006442\n19.99\n4.99\n```\n',
     'author': 'Fede Calendino',
     'author_email': 'fede@calendino.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fedecalendino/nintendeals',
```

### Comparing `nintendeals-3.0.2/PKG-INFO` & `nintendeals-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nintendeals
-Version: 3.0.2
+Version: 3.1.0
 Summary: Scraping tools for Nintendo Switch games and prices on NA, EU and JP.
 Home-page: https://github.com/fedecalendino/nintendeals
 License: MIT
 Keywords: nintendo,deals
 Author: Fede Calendino
 Author-email: fede@calendino.com
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: algoliasearch (>=2.6.2,<3.0.0)
+Requires-Dist: algoliasearch (>=3.0.0,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Documentation, https://github.com/fedecalendino/nintendeals/blob/main/README.md
 Description-Content-Type: text/markdown
```

