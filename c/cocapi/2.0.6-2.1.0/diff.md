# Comparing `tmp/cocapi-2.0.6.tar.gz` & `tmp/cocapi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cocapi-2.0.6.tar", last modified: Fri Jun 12 10:14:22 2020, max compression
+gzip compressed data, was "cocapi-2.1.0.tar", last modified: Sat Jul  8 12:45:51 2023, max compression
```

## Comparing `cocapi-2.0.6.tar` & `cocapi-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 tony      (1000) users      (985)        0 2020-06-12 10:14:22.206854 cocapi-2.0.6/
--rw-r--r--   0 tony      (1000) users      (985)    20425 2020-06-12 10:14:22.206854 cocapi-2.0.6/PKG-INFO
--rw-r--r--   0 tony      (1000) users      (985)    13479 2020-06-11 22:09:54.000000 cocapi-2.0.6/README.md
-drwxr-xr-x   0 tony      (1000) users      (985)        0 2020-06-12 10:14:22.206854 cocapi-2.0.6/cocapi/
--rw-r--r--   0 tony      (1000) users      (985)       49 2019-01-02 09:39:48.000000 cocapi-2.0.6/cocapi/__init__.py
--rw-r--r--   0 tony      (1000) users      (985)     9259 2020-05-12 10:57:44.000000 cocapi-2.0.6/cocapi/cocapi.py
-drwxr-xr-x   0 tony      (1000) users      (985)        0 2020-06-12 10:14:22.206854 cocapi-2.0.6/cocapi.egg-info/
--rw-r--r--   0 tony      (1000) users      (985)    20425 2020-06-12 10:14:22.000000 cocapi-2.0.6/cocapi.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) users      (985)      203 2020-06-12 10:14:22.000000 cocapi-2.0.6/cocapi.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) users      (985)        1 2020-06-12 10:14:22.000000 cocapi-2.0.6/cocapi.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) users      (985)        6 2020-06-12 10:14:22.000000 cocapi-2.0.6/cocapi.egg-info/requires.txt
--rw-r--r--   0 tony      (1000) users      (985)        7 2020-06-12 10:14:22.000000 cocapi-2.0.6/cocapi.egg-info/top_level.txt
--rw-r--r--   0 tony      (1000) users      (985)       38 2020-06-12 10:14:22.206854 cocapi-2.0.6/setup.cfg
--rw-r--r--   0 tony      (1000) users      (985)      766 2020-06-12 10:14:18.000000 cocapi-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:45:51.746301 cocapi-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-08 12:45:38.000000 cocapi-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-07-08 12:45:51.746301 cocapi-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-08 12:45:38.000000 cocapi-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:45:51.746301 cocapi-2.1.0/cocapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-08 12:45:38.000000 cocapi-2.1.0/cocapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13937 2023-07-08 12:45:38.000000 cocapi-2.1.0/cocapi/cocapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:45:51.746301 cocapi-2.1.0/cocapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-07-08 12:45:51.000000 cocapi-2.1.0/cocapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-08 12:45:51.000000 cocapi-2.1.0/cocapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:45:51.000000 cocapi-2.1.0/cocapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 12:45:51.000000 cocapi-2.1.0/cocapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 12:45:51.000000 cocapi-2.1.0/cocapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-08 12:45:38.000000 cocapi-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:45:51.746301 cocapi-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-08 12:45:38.000000 cocapi-2.1.0/setup.py
```

### Comparing `cocapi-2.0.6/README.md` & `cocapi-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,36 +8,36 @@
     <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/python-3.6+-blue.svg" alt="Python version" height="17"></a>
     <a href="https://github.com/tonybenoy/cocapi/blob/master/LICENSE"><img src="https://img.shields.io/github/license/tonybenoy/cocapi" alt="License" height="17"></a>
     <a href="https://github.com/psf/black">
         <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Codestyle Black" height="17">
     </a>
 </p>
 
-# ClashOfClansAPI 
+# ClashOfClansAPI
 
 Python Wrapper for SuperCells Clash Of Clans API
 
 Get Token from https://developer.clashofclans.com/
 
 # Install
 
 > pip install cocapi
 
 
 # Features and usage examples
 
 ### Initialize
 
-Required to set up the class
+Required to set up the class. Versions post 6.1.0 also support getting the status code of the API call. This is useful for debugging. To use it pass `status_code=True` to the `CocApi`.
 
 ```python
 from cocapi import CocApi
 
 token = 'YOUR_API_TOKEN'
-timeout=1 #requests timeout
+timeout=60 #requests timeout
 
 api=CocApi(token,timeout)
 ```
 
 
 
 
@@ -117,15 +117,15 @@
 
 ### War Log Information
 ```python
 api.clan_war_log(tag)
 ```
 <details>
  <summary>Click to view output</summary>
- 
+
 ```text
 {items:
 [
   {
     "clan": {
       "destructionPercentage": {},
       "tag": "string",
@@ -196,15 +196,15 @@
           ]
         }
       ]
     },
     "endTime": "string",
     "result": "string"
   }
-], 
+],
 "paging": {'cursors': {}}
 }
 ```
 </details>
 
 ### Current War Information
 ```python
@@ -330,15 +330,15 @@
   ]
 }
 ```
 </details>
 
 ### Warleague Information
 ```python
-api.clan_warleague(war_tag)
+api.warleague(war_tag)
 ```
 <details>
  <summary>Click to view output</summary>
 
 ```text
 {
   "tag": "string",
@@ -546,15 +546,15 @@
     "members": 0,
     "tag": "string",
     "name": "string",
     "rank": 0,
     "previousRank": 0,
     "badgeUrls": {}
   }
-], 
+],
 "paging": {'cursors': {}}
 }
 ```
 </details>
 
 ### Top Players in a Location
 ```python
@@ -583,15 +583,15 @@
     "tag": "string",
     "name": "string",
     "expLevel": 0,
     "rank": 0,
     "previousRank": 0,
     "trophies": 0
   }
-], 
+],
 "paging": {'cursors': {}}
 }
 ```
 </details>
 
 
 ### Top Versus Clans in a Location
@@ -605,15 +605,15 @@
 ```text
 {"items":
 [
   {
     "clanPoints": 0,
     "clanVersusPoints": 0
   }
-], 
+],
 "paging": {'cursors': {}}
 }
 ```
 </details>
 
 
 ### Top Versus Players in a Location
@@ -637,15 +637,15 @@
     "tag": "string",
     "name": "string",
     "expLevel": 0,
     "rank": 0,
     "previousRank": 0,
     "versusTrophies": 0
   }
-], 
+],
 "paging": {'cursors': {}}
 }
 ```
 </details>
 
 
 
@@ -663,15 +663,15 @@
 {"items":
 [
   {
     "name": {},
     "id": 0,
     "iconUrls": {}
   }
-], 
+],
 "paging": {'cursors': {}}
 }
 ```
 </details>
 
 
 ### League Information
@@ -701,15 +701,15 @@
 
 ```text
 {"items":
 [
   {
     "id": "string"
   }
-], 
+],
 "paging": {'cursors': {}}
 }
 ```
 </details>
 
 
 ### League Season Ranking
@@ -739,15 +739,15 @@
     "tag": "string",
     "name": "string",
     "expLevel": 0,
     "rank": 0,
     "previousRank": 0,
     "trophies": 0
   }
-], 
+],
 "paging": {'cursors': {}}
 }
 ```
 </details>
 
 
 
@@ -765,15 +765,15 @@
 {"items":
 [
   {
     "name": {},
     "id": 0,
     "iconUrls": {}
   }
-], 
+],
 "paging": {'cursors': {}}
 }
 ```
 </details>
 
 
 ### List Player Labels
@@ -787,15 +787,15 @@
 {"items":
 [
   {
     "name": {},
     "id": 0,
     "iconUrls": {}
   }
-], 
+],
 "paging": {'cursors': {}}
 }
 ```
 </details>
 
 
 ## Credits
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 [Test_Status] [Pypi_version]
 [Python_version] [License] [Codestyle_Black]
 # ClashOfClansAPI Python Wrapper for SuperCells Clash Of Clans API Get Token
 from https://developer.clashofclans.com/ # Install > pip install cocapi #
-Features and usage examples ### Initialize Required to set up the class
-```python from cocapi import CocApi token = 'YOUR_API_TOKEN' timeout=1
+Features and usage examples ### Initialize Required to set up the class.
+Versions post 6.1.0 also support getting the status code of the API call. This
+is useful for debugging. To use it pass `status_code=True` to the `CocApi`.
+```python from cocapi import CocApi token = 'YOUR_API_TOKEN' timeout=60
 #requests timeout api=CocApi(token,timeout) ``` ## Clans ### Information about
 a Clan ```python api.clan_tag(tag) #example tag "#9UOVJJ9J" ```  Click to view
 output ```text { "warLeague": { "name": {}, "id": 0 }, "memberList": [
 { "league": { "name": {}, "id": 0, "iconUrls": {} }, "tag": "string", "name":
 "string", "role": "string", "expLevel": 0, "clanRank": 0, "previousClanRank":
 0, "donations": 0, "donationsReceived": 0, "trophies": 0, "versusTrophies": 0 }
 ], "isWarLogPublic": true, "tag": "string", "warFrequency": "string",
@@ -53,15 +55,15 @@
 "stars": 0, "destructionPercentage": 0 } ] } ] }, "startTime": "string",
 "state": "string", "endTime": "string", "preparationStartTime": "string" } ```
 ### Clan League Group Information ```python api.clan_leaguegroup(tag) ```
 Click to view output ```text { "tag": "string", "state": "string", "season":
 "string", "clans": [ { "tag": "string", "clanLevel": 0, "name": "string",
 "members": [ { "tag": "string", "townHallLevel": 0, "name": "string" } ],
 "badgeUrls": {} } ], "rounds": [ { "warTags": [ "string" ] } ] } ```  ###
-Warleague Information ```python api.clan_warleague(war_tag) ```  Click to view
+Warleague Information ```python api.warleague(war_tag) ```  Click to view
 output ```text { "tag": "string", "state": "string", "season": "string",
 "clans": [ { "tag": "string", "clanLevel": 0, "name": "string", "members": [
 { "tag": "string", "townHallLevel": 0, "name": "string" } ], "badgeUrls": {} }
 ], "rounds": [ { "warTags": [ "string" ] } ] } ```  ## Player ### Player
 information ```python api.players(player_tag) #for example "#900PUCPV" ```
 Click to view output ```text { "clan": { "tag": "string", "clanLevel": 0,
 "name": "string", "badgeUrls": {} }, "league": { "name": {}, "id": 0,
```

### Comparing `cocapi-2.0.6/cocapi/cocapi.py` & `cocapi-2.1.0/cocapi/cocapi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,242 +1,381 @@
 import urllib
-from typing import Dict, Tuple
+from typing import Any, Dict, Tuple
+from warnings import warn
+
 import httpx
 
 
 class CocApi:
-    def __init__(self, token: str, timeout: int = 20):
+    def __init__(self, token: str, timeout: int = 20, status_code: bool = False):
         """
         Initialising requisites
         """
         self.token = token
         self.ENDPOINT = "https://api.clashofclans.com/v1"
         self.timeout = timeout
         self.headers = {
-            "authorization": "Bearer %s" % token,
+            "authorization": f"Bearer {token}",
             "Accept": "application/json",
         }
+        self.status_code = status_code
         self.DEFAULT_PARAMS = ("limit", "after", "before")
         self.ERROR_INVALID_PARAM = {
             "result": "error",
             "message": "Invalid params for method",
         }
+        test_reponse = self.test()
+        if test_reponse.get("result") == "error":
+            raise Exception(test_reponse.get("message"))
 
-    def check_if_dict_invalid(self, params: Dict, valid_items: Tuple = ()) -> bool:
-        if not valid_items:
-            valid_items = self.DEFAULT_PARAMS
+    def __check_if_dict_invalid(self, params: Dict, valid_items: Tuple = ()) -> bool:
+        valid_items = self.DEFAULT_PARAMS if not valid_items else valid_items
         return set(params.keys()).issubset(valid_items)
 
-    def api_response(self, uri: str, params: Dict = {}) -> Dict:
+    def __api_response(
+        self, uri: str, params: Dict = {}, status_code: bool = False
+    ) -> Dict:
         """
         Function to handle requests,it is possible to use this handler on it's
         own to make request to the api on in case of a new or unsupported api
         Args:
-            uri      -> The endpoint uri that needs to be called for the specific function
+            uri  -> The endpoint uri that needs to be called for the specific function
             params   -> Dictionary of supported params to be filtered
                         with Refer https://developer.clashofclans.com/#/documentation
         Return:
             The json response from the api as is or returns error if broken
         """
-
-        url = self.ENDPOINT + uri + "?" + urllib.parse.urlencode(params)  # type: ignore
+        url = f"{self.ENDPOINT}{uri}?{urllib.parse.urlencode(params)}"  # type: ignore
         try:
             response = httpx.get(url=url, headers=self.headers, timeout=self.timeout)
-            return dict(response.json())
-        except:
-            return {"result": "error", "message": "Something broke"}
+            response_json = response.json()
+            if status_code or self.status_code:
+                response_json = dict(
+                    response_json.update({"status_code": response.status_code})
+                )
+            return dict(response_json)
+        except Exception as e:
+            return {
+                "result": "error",
+                "message": "Something broke, please try again!",
+                "exception": str(e),
+            }
 
-    def test(self) -> Dict:
+    def test(self) -> Dict[str, Any]:
         """
         Function to test if the api is up and running.
             Dictionary with a success if api is up error if false
         """
         response = httpx.get(url=self.ENDPOINT, headers=self.headers)
         if response.status_code == 200:
             return {"result": "success", "message": "Api is up and running!"}
+        elif response.status_code == 403:
+            return {
+                "result": "error",
+                "message": "Invalid token",
+            }
         else:
-            return {"result": "error", "message": "Api is Down!"}
+            response_json = {
+                "result": "error",
+                "message": "Api is Down!",
+            }
+            if self.status_code:
+                response_json.update(
+                    {"status_code": response.status_code}
+                )  # type: ignore
+            return response_json
+
+    def clan_leaguegroup(self, tag: str) -> Dict:
+        """
+        Function to Retrieve information about clan's current clan war league group
+        """
+        return self.__api_response(uri=f"/clans/%23{tag[1:]}/currentwar/leaguegroup")
+
+    def warleague(self, sid: str) -> Dict:
+        """
+        Function to Retrieve information about a clan war league war.
+        """
+        return self.__api_response(uri=f"/clanwarleagues/wars/{str(sid)}")
+
+    def clan_war_log(self, tag: str, params: Dict = {}) -> Dict:
+        """
+        Function to Retrieve clan's clan war log
+        """
+        if not self.__check_if_dict_invalid(params=params):
+            return self.ERROR_INVALID_PARAM
+        return self.__api_response(uri=f"/clans/%23{tag[1:]}/warlog", params=params)
 
     def clan(self, params: Dict = {}) -> Dict:
         """
-        Function to Search all clans by name and/or filtering the results using various criteria.
-        At least one filtering criteria must be defined and if name is used as part of search, it
-        is required to be at least three characters long.It is not possible to specify ordering for
-        results so clients should not rely on any specific ordering as that may change in the
-        future releases of the API.
+        Function to Search all clans by name and/or filtering the results using
+        various criteria.At least one filtering criteria must be defined and if
+        name is used as part of search, it is required to be at least three
+        characters long.It is not possible to specify ordering for results so
+        clients should not rely on any specific ordering as that may change
+        in the future releases of the API.
         """
         valid_items = tuple(
             [
                 "name",
                 "warFrequency",
                 "locationId",
                 "minMembers",
                 "maxMembers",
                 "minClanPoints",
                 "minClanLevel",
                 "labelIds",
             ]
             + list(self.DEFAULT_PARAMS)
         )
-        if not self.check_if_dict_invalid(params=params, valid_items=valid_items):
+        if not self.__check_if_dict_invalid(params=params, valid_items=valid_items):
             return self.ERROR_INVALID_PARAM
-        uri = "/clans"
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(uri="/clans", params=params)
+
+    def clan_current_war(self, tag: str) -> Dict:
+        """
+        Function to Retrieve information about clan's current clan war
+        """
+        return self.__api_response(uri=f"/clans/%23{tag[1:]}/currentwar")
 
     def clan_tag(self, tag: str) -> Dict:
         """
         Function to Get information about a single clan by clan tag.
         Clan tags can be found using clan search operation.
         """
-        uri = "/clans/%23" + tag[1:]
-        return self.api_response(uri=uri)
+        return self.__api_response(uri=f"/clans/%23{tag[1:]}")
 
     def clan_members(self, tag: str, params: Dict = {}) -> Dict:
         """
         Function to List clan members
         """
-        if not self.check_if_dict_invalid(params=params):
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/clans/%23" + tag[1:] + "/members"
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(uri=f"/clans/%23{tag[1:]}/members", params=params)
 
-    def clan_war_log(self, tag: str, params: Dict = {}) -> Dict:
+    def clan_capitalraidseasons(self, tag: str, params: Dict = {}) -> Dict:
         """
-        Function to Retrieve clan's clan war log
+        Function to Retrieve information about clan's current clan war
         """
-        if not self.check_if_dict_invalid(params=params):
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/clans/%23" + tag[1:] + "/warlog"
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(
+            uri=f"/clans/%23{tag[1:]}/currentwar/capitalraidseasons", params=params
+        )
 
-    def clan_current_war(self, tag: str) -> Dict:
+    def players(self, tag: str) -> Dict:
         """
-        Function to Retrieve information about clan's current clan war
+        Function to Get information about a single player by player tag.
+        Player tags can be found either in game or by from clan member lists.
         """
-        uri = "/clans/%23" + tag[1:] + "/currentwar"
-        return self.api_response(uri=uri)
+        return self.__api_response(uri=f"/players/%23{tag[1:]}")
 
-    def clan_leaguegroup(self, tag: str) -> Dict:
+    def location_id_clan_rank(self, id: str, params: Dict = {}) -> Dict:
         """
-        Function to Retrieve information about clan's current clan war league group
+        Function to Get clan rankings for a specific location
         """
-        uri = "/clans/%23" + tag[1:] + "/currentwar/leaguegroup"
-        return self.api_response(uri=uri)
+        if not self.__check_if_dict_invalid(params=params):
+            return self.ERROR_INVALID_PARAM
+        return self.__api_response(
+            uri=f"/locations/{str(id)}/rankings/clans", params=params
+        )
 
-    def warleague(self, sid: str) -> Dict:
+    def location_id_player_rank(self, id: str, params: Dict = {}) -> Dict:
         """
-        Function to Retrieve information about a clan war league war.
+        Function to Get player rankings for a specific location
         """
-        uri = "/clanwarleagues/wars/" + str(sid)
-        return self.api_response(uri=uri)
+        if not self.__check_if_dict_invalid(params=params):
+            return self.ERROR_INVALID_PARAM
+        return self.__api_response(
+            uri=f"/locations/{str(id)}/rankings/players", params=params
+        )
 
-    def players(self, tag: str) -> Dict:
+    def location_clan_versus(self, id: str, params: Dict = {}) -> Dict:
         """
-        Function to Get information about a single player by player tag. Player tags can be found either in game or by from clan member lists.
+        Function to Get clan versus rankings for a specific location
         """
-        uri = "/players/%23" + tag[1:]
-        return self.api_response(uri=uri)
+        warn(
+            "This end will be deprecated in the future.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        if not self.__check_if_dict_invalid(params=params):
+            return self.ERROR_INVALID_PARAM
 
-    def location(self, params: Dict = {}) -> Dict:
+        return self.__api_response(
+            uri=f"/locations/{str(id)}/rankings/clans-versus", params=params
+        )
+
+    def location_players_builder_base(self, id: str, params: Dict = {}) -> Dict:
         """
-        Function List all available locations
+        Function to Get player builder base rankings for a specific location
         """
-        if not self.check_if_dict_invalid(params=params):
+
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/locations"
-        return self.api_response(uri=uri, params=params)
 
-    def location_id(self, id: str) -> Dict:
-        """
-        Function to Get information about specific location
-        """
-        uri = "/locations/" + str(id)
-        return self.api_response(uri=uri)
+        return self.__api_response(
+            uri=f"/locations/{str(id)}/rankings/players-builder-base", params=params
+        )
 
-    def location_id_clan_rank(self, id: str, params: Dict = {}) -> Dict:
+    def location_clans_builder_base(self, id: str, params: Dict = {}) -> Dict:
         """
-        Function to Get clan rankings for a specific location
+        Function to Get clan builder base rankings for a specific location
         """
-        if not self.check_if_dict_invalid(params=params):
+
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/locations/" + str(id) + "/rankings/clans"
-        return self.api_response(uri=uri, params=params)
 
-    def location_id_player_rank(self, id: str, params: Dict = {}) -> Dict:
+        return self.__api_response(
+            uri=f"/locations/{str(id)}/rankings/clans-builder-base", params=params
+        )
+
+    def location_player_versus(self, id: str, params: Dict = {}) -> Dict:
         """
-        Function to Get player rankings for a specific location
+        Function to Get player versus rankings for a specific location
         """
-        if not self.check_if_dict_invalid(params=params):
+        warn(
+            "This end will be deprecated in the future.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/locations/" + str(id) + "/rankings/players"
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(
+            uri=f"/locations/{str(id)}/rankings/players-versus", params=params
+        )
 
-    def location_clan_versus(self, id: str, params: Dict = {}) -> Dict:
+    def location(self, params: Dict = {}) -> Dict:
         """
-        Function to Get clan versus rankings for a specific location
+        Function List all available locations
+        Will be depricated in the future in favour of locations
+
         """
+        warn(
+            "This method will be \
+            deprecated in the future in favour\
+            of locations to maintain parity with original api",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.locations(params=params)
 
-        if not self.check_if_dict_invalid(params=params):
+    def locations(self, params: Dict = {}) -> Dict:
+        """
+        Function to List all available locations
+        """
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/locations/" + str(id) + "/rankings/clans-versus"
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(uri="/locations", params=params)
 
-    def location_player_versus(self, id: str, params: Dict = {}) -> Dict:
+    def location_rankings_capitals(self, id: str, params: Dict = {}) -> Dict:
         """
-        Function to Get player versus rankings for a specific location
+        Function to Get capital rankings for a specific location
         """
-        if not self.check_if_dict_invalid(params=params):
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/locations/" + str(id) + "/rankings/players-versus"
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(
+            uri=f"/locations/{str(id)}/rankings/capitals", params=params
+        )
+
+    def location_id(self, id: str) -> Dict:
+        """
+        Function to Get information about specific location
+        """
+        return self.__api_response(uri=f"/locations/{str(id)}")
 
     def league(self, params: Dict = {}) -> Dict:
         """
         Function to Get list of leagues
         """
-        if not self.check_if_dict_invalid(params=params):
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/leagues"
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(uri="/leagues", params=params)
 
     def league_id(self, id: str) -> Dict:
         """
         Function to Get league information
         """
-        uri = "/leagues/" + str(id)
-        return self.api_response(uri=uri)
+        return self.__api_response(uri=f"/leagues/{str(id)}")
 
     def league_season(self, id: str, params: Dict = {}) -> Dict:
         """
-        Function to Get league seasons. Note that league season information is available only for Legend League.
+        Function to Get league seasons.
+        Note that league season information is available only for Legend League.
         """
-        if not self.check_if_dict_invalid(params=params):
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/leagues/" + str(id) + "/seasons"
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(uri=f"/leagues/{str(id)}/seasons", params=params)
 
     def league_season_id(self, id: str, sid: str, params: Dict = {}) -> Dict:
         """
-        Function to Get league season rankings. Note that league season information is available only for Legend League.
+        Function to Get league season rankings.
+        Note that league season information is available only for Legend League.
         """
-        if not self.check_if_dict_invalid(params=params):
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/leagues/" + str(id) + "/seasons/" + str(sid)
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(
+            uri=f"/leagues/{str(id)}/seasons/{str(sid)}", params=params
+        )
+
+    def warleagues(self) -> Dict:
+        """
+        Function to Get list of clan war leagues
+        """
+        return self.__api_response(
+            uri="/warleagues",
+        )
+
+    def warleagues_id(self, league_id: str) -> Dict:
+        """
+        Function to Get information about a clan war league
+        """
+        return self.__api_response(
+            uri=f"/warleagues/{str(league_id)}",
+        )
 
     def labels_clans(self, params: Dict = {}) -> Dict:
         """
         Function to Get labels for a clan
         """
-        if not self.check_if_dict_invalid(params=params):
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/labels/clans"
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(uri="/labels/clans", params=params)
 
     def labels_players(self, params: Dict = {}) -> Dict:
         """
         Function to Get labels for a player
         """
-        if not self.check_if_dict_invalid(params=params):
+        if not self.__check_if_dict_invalid(params=params):
             return self.ERROR_INVALID_PARAM
-        uri = "/labels/players/"
-        return self.api_response(uri=uri, params=params)
+        return self.__api_response(uri="/labels/players/", params=params)
+
+    def goldpass_seasons_current(self) -> Dict:
+        """
+        Function to Get current gold pass season
+        """
+        return self.__api_response(uri="/goldpass/seasons/current")
+
+    def player_verifytoken(self, token: str, player_tag: str) -> Dict:
+        """
+        Function to Verify player token
+        """
+
+        try:
+            response = httpx.post(
+                url=f"{self.ENDPOINT}/players/%23{player_tag[1:]}/verifytoken",
+                headers={
+                    "Authorization": f"Bearer {token}",
+                    "Accept": "application/json",
+                },
+                data={"token": token},
+            )
+            response_json = dict(response.json())
+
+            if self.status_code:
+                response_json = dict(response_json, status_code=response.status_code)
+            return response_json
+        except Exception as e:
+            return {
+                "status": "error",
+                "message": "Something broke",
+                "exception": str(e),
+            }
```

### Comparing `cocapi-2.0.6/setup.py` & `cocapi-2.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools  # type: ignore
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cocapi",
-    version="2.0.6",
+    version="2.1.0",
     author="Tony Benoy",
-    setup_requires=['wheel'],
+    setup_requires=["wheel"],
     author_email="me@tonybenoy.com",
     description="A python wrapper around clash of clans api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tonybenoy/cocapi",
     install_requires=["httpx"],
     keywords="Clash of Clans SuperCell API COC",
     packages=setuptools.find_packages(),
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent",
     ),
+    extras_require={"dev": ["black", "pylint", "mypy", "isort"]},
 )
```

