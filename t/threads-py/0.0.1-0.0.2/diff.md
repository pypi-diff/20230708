# Comparing `tmp/threads-py-0.0.1.tar.gz` & `tmp/threads-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-py-0.0.1.tar", last modified: Fri Jul  7 18:36:43 2023, max compression
+gzip compressed data, was "threads-py-0.0.2.tar", last modified: Sat Jul  8 19:25:53 2023, max compression
```

## Comparing `threads-py-0.0.1.tar` & `threads-py-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-07 18:36:43.605444 threads-py-0.0.1/
--rw-r--r--   0 mineru     (501) staff       (20)     1066 2023-07-07 02:31:26.000000 threads-py-0.0.1/LICENSE
--rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-07 18:36:43.605287 threads-py-0.0.1/PKG-INFO
--rw-r--r--   0 mineru     (501) staff       (20)     1257 2023-07-07 18:34:10.000000 threads-py-0.0.1/README.md
--rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-07 18:36:43.605486 threads-py-0.0.1/setup.cfg
--rw-r--r--   0 mineru     (501) staff       (20)      941 2023-07-07 18:36:33.000000 threads-py-0.0.1/setup.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-07 18:36:43.600538 threads-py-0.0.1/threads_py.egg-info/
--rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-07 18:36:43.000000 threads-py-0.0.1/threads_py.egg-info/PKG-INFO
--rw-r--r--   0 mineru     (501) staff       (20)     1257 2023-07-07 18:36:43.000000 threads-py-0.0.1/threads_py.egg-info/SOURCES.txt
--rw-r--r--   0 mineru     (501) staff       (20)        1 2023-07-07 18:36:43.000000 threads-py-0.0.1/threads_py.egg-info/dependency_links.txt
--rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-07 18:36:43.000000 threads-py-0.0.1/threads_py.egg-info/requires.txt
--rw-r--r--   0 mineru     (501) staff       (20)       10 2023-07-07 18:36:43.000000 threads-py-0.0.1/threads_py.egg-info/top_level.txt
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-07 18:36:43.600845 threads-py-0.0.1/threadspy/
--rw-r--r--   0 mineru     (501) staff       (20)      111 2023-07-07 16:55:06.000000 threads-py-0.0.1/threadspy/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)     6964 2023-07-07 18:30:09.000000 threads-py-0.0.1/threadspy/_thread.py
-drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-07 18:36:43.605077 threads-py-0.0.1/threadspy/types/
--rw-r--r--   0 mineru     (501) staff       (20)     1183 2023-07-07 18:26:15.000000 threads-py-0.0.1/threadspy/types/__init__.py
--rw-r--r--   0 mineru     (501) staff       (20)      188 2023-07-07 08:49:18.000000 threads-py-0.0.1/threadspy/types/candidate.py
--rw-r--r--   0 mineru     (501) staff       (20)      134 2023-07-07 08:34:39.000000 threads-py-0.0.1/threadspy/types/caption.py
--rw-r--r--   0 mineru     (501) staff       (20)      622 2023-07-07 18:28:28.000000 threads-py-0.0.1/threadspy/types/common.py
--rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 08:49:13.000000 threads-py-0.0.1/threadspy/types/extensions.py
--rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:26:10.000000 threads-py-0.0.1/threadspy/types/get_thread_likers_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:56:07.000000 threads-py-0.0.1/threadspy/types/get_user_profile_replies_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:03:46.000000 threads-py-0.0.1/threadspy/types/get_user_profile_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      315 2023-07-07 17:57:17.000000 threads-py-0.0.1/threadspy/types/get_user_profile_thread_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:57:25.000000 threads-py-0.0.1/threadspy/types/get_user_profile_threads_response.py
--rw-r--r--   0 mineru     (501) staff       (20)      233 2023-07-07 16:58:01.000000 threads-py-0.0.1/threadspy/types/image_versions2.py
--rw-r--r--   0 mineru     (501) staff       (20)      216 2023-07-07 16:58:01.000000 threads-py-0.0.1/threadspy/types/media_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      772 2023-07-07 17:21:37.000000 threads-py-0.0.1/threadspy/types/post.py
--rw-r--r--   0 mineru     (501) staff       (20)      766 2023-07-07 17:21:46.000000 threads-py-0.0.1/threadspy/types/quoted_post.py
--rw-r--r--   0 mineru     (501) staff       (20)      189 2023-07-07 08:46:47.000000 threads-py-0.0.1/threadspy/types/reply_facepile_user.py
--rw-r--r--   0 mineru     (501) staff       (20)      812 2023-07-07 17:22:01.000000 threads-py-0.0.1/threadspy/types/reposted_post.py
--rw-r--r--   0 mineru     (501) staff       (20)      304 2023-07-07 16:58:01.000000 threads-py-0.0.1/threadspy/types/share_info.py
--rw-r--r--   0 mineru     (501) staff       (20)      313 2023-07-07 18:29:52.000000 threads-py-0.0.1/threadspy/types/text_post_app_info.py
--rw-r--r--   0 mineru     (501) staff       (20)      299 2023-07-07 16:58:01.000000 threads-py-0.0.1/threadspy/types/thread.py
--rw-r--r--   0 mineru     (501) staff       (20)      253 2023-07-07 16:58:01.000000 threads-py-0.0.1/threadspy/types/thread_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      433 2023-07-07 16:58:01.000000 threads-py-0.0.1/threadspy/types/thread_item.py
--rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 17:23:07.000000 threads-py-0.0.1/threadspy/types/threads_bio_link.py
--rw-r--r--   0 mineru     (501) staff       (20)      185 2023-07-07 17:20:54.000000 threads-py-0.0.1/threadspy/types/threads_hd_profile_pic_version.py
--rw-r--r--   0 mineru     (501) staff       (20)      729 2023-07-07 18:25:26.000000 threads-py-0.0.1/threadspy/types/threads_user.py
--rw-r--r--   0 mineru     (501) staff       (20)      222 2023-07-07 17:20:21.000000 threads-py-0.0.1/threadspy/types/threads_user_summary.py
--rw-r--r--   0 mineru     (501) staff       (20)      198 2023-07-07 16:58:01.000000 threads-py-0.0.1/threadspy/types/user_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      200 2023-07-07 16:58:00.000000 threads-py-0.0.1/threadspy/types/user_profile_data.py
--rw-r--r--   0 mineru     (501) staff       (20)      230 2023-07-07 18:11:06.000000 threads-py-0.0.1/threadspy/types/users.py
--rw-r--r--   0 mineru     (501) staff       (20)      174 2023-07-07 08:44:28.000000 threads-py-0.0.1/threadspy/types/video_version.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:25:53.302879 threads-py-0.0.2/
+-rw-r--r--   0 mineru     (501) staff       (20)     1066 2023-07-07 02:31:26.000000 threads-py-0.0.2/LICENSE
+-rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-08 19:25:53.302703 threads-py-0.0.2/PKG-INFO
+-rw-r--r--   0 mineru     (501) staff       (20)     2436 2023-07-08 19:21:10.000000 threads-py-0.0.2/README.md
+-rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-08 19:25:53.302930 threads-py-0.0.2/setup.cfg
+-rw-r--r--   0 mineru     (501) staff       (20)      941 2023-07-08 17:19:16.000000 threads-py-0.0.2/setup.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:25:53.297563 threads-py-0.0.2/threads_py.egg-info/
+-rw-r--r--   0 mineru     (501) staff       (20)      340 2023-07-08 19:25:53.000000 threads-py-0.0.2/threads_py.egg-info/PKG-INFO
+-rw-r--r--   0 mineru     (501) staff       (20)     1257 2023-07-08 19:25:53.000000 threads-py-0.0.2/threads_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mineru     (501) staff       (20)        1 2023-07-08 19:25:53.000000 threads-py-0.0.2/threads_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mineru     (501) staff       (20)       38 2023-07-08 19:25:53.000000 threads-py-0.0.2/threads_py.egg-info/requires.txt
+-rw-r--r--   0 mineru     (501) staff       (20)       10 2023-07-08 19:25:53.000000 threads-py-0.0.2/threads_py.egg-info/top_level.txt
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:25:53.297816 threads-py-0.0.2/threadspy/
+-rw-r--r--   0 mineru     (501) staff       (20)      111 2023-07-08 18:27:24.000000 threads-py-0.0.2/threadspy/__init__.py
+-rw-r--r--   0 mineru     (501) staff       (20)    10788 2023-07-08 19:25:33.000000 threads-py-0.0.2/threadspy/_thread.py
+drwxr-xr-x   0 mineru     (501) staff       (20)        0 2023-07-08 19:25:53.302341 threads-py-0.0.2/threadspy/types/
+-rw-r--r--   0 mineru     (501) staff       (20)     1250 2023-07-08 18:18:23.000000 threads-py-0.0.2/threadspy/types/__init__.py
+-rw-r--r--   0 mineru     (501) staff       (20)      188 2023-07-07 08:49:18.000000 threads-py-0.0.2/threadspy/types/candidate.py
+-rw-r--r--   0 mineru     (501) staff       (20)      134 2023-07-07 08:34:39.000000 threads-py-0.0.2/threadspy/types/caption.py
+-rw-r--r--   0 mineru     (501) staff       (20)      622 2023-07-07 18:28:28.000000 threads-py-0.0.2/threadspy/types/common.py
+-rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 08:49:13.000000 threads-py-0.0.2/threadspy/types/extensions.py
+-rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:26:10.000000 threads-py-0.0.2/threadspy/types/get_thread_likers_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:56:07.000000 threads-py-0.0.2/threadspy/types/get_user_profile_replies_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      302 2023-07-07 18:03:46.000000 threads-py-0.0.2/threadspy/types/get_user_profile_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      315 2023-07-07 17:57:17.000000 threads-py-0.0.2/threadspy/types/get_user_profile_thread_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      314 2023-07-07 17:57:25.000000 threads-py-0.0.2/threadspy/types/get_user_profile_threads_response.py
+-rw-r--r--   0 mineru     (501) staff       (20)      233 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/image_versions2.py
+-rw-r--r--   0 mineru     (501) staff       (20)      216 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/media_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      772 2023-07-07 17:21:37.000000 threads-py-0.0.2/threadspy/types/post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      766 2023-07-07 17:21:46.000000 threads-py-0.0.2/threadspy/types/quoted_post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      189 2023-07-07 08:46:47.000000 threads-py-0.0.2/threadspy/types/reply_facepile_user.py
+-rw-r--r--   0 mineru     (501) staff       (20)      812 2023-07-07 17:22:01.000000 threads-py-0.0.2/threadspy/types/reposted_post.py
+-rw-r--r--   0 mineru     (501) staff       (20)      304 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/share_info.py
+-rw-r--r--   0 mineru     (501) staff       (20)      313 2023-07-07 18:29:52.000000 threads-py-0.0.2/threadspy/types/text_post_app_info.py
+-rw-r--r--   0 mineru     (501) staff       (20)      299 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/thread.py
+-rw-r--r--   0 mineru     (501) staff       (20)      280 2023-07-08 18:20:59.000000 threads-py-0.0.2/threadspy/types/thread_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      433 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/thread_item.py
+-rw-r--r--   0 mineru     (501) staff       (20)      142 2023-07-07 17:23:07.000000 threads-py-0.0.2/threadspy/types/threads_bio_link.py
+-rw-r--r--   0 mineru     (501) staff       (20)      185 2023-07-07 17:20:54.000000 threads-py-0.0.2/threadspy/types/threads_hd_profile_pic_version.py
+-rw-r--r--   0 mineru     (501) staff       (20)      729 2023-07-08 18:23:31.000000 threads-py-0.0.2/threadspy/types/threads_user.py
+-rw-r--r--   0 mineru     (501) staff       (20)      222 2023-07-07 17:20:21.000000 threads-py-0.0.2/threadspy/types/threads_user_summary.py
+-rw-r--r--   0 mineru     (501) staff       (20)      198 2023-07-07 16:58:01.000000 threads-py-0.0.2/threadspy/types/user_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      200 2023-07-07 16:58:00.000000 threads-py-0.0.2/threadspy/types/user_profile_data.py
+-rw-r--r--   0 mineru     (501) staff       (20)      230 2023-07-07 18:11:06.000000 threads-py-0.0.2/threadspy/types/users.py
+-rw-r--r--   0 mineru     (501) staff       (20)      174 2023-07-07 08:44:28.000000 threads-py-0.0.2/threadspy/types/video_version.py
```

### Comparing `threads-py-0.0.1/LICENSE` & `threads-py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.1/setup.py` & `threads-py-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.1/threads_py.egg-info/SOURCES.txt` & `threads-py-0.0.2/threads_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.1/threadspy/_thread.py` & `threads-py-0.0.2/threadspy/_thread.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,195 +1,322 @@
 import re
-import json
 import requests
+from typing import List
 
-from threadspy.types.threads_user import ThreadsUser
 from threadspy.types import (
+    Thread,
+    UsersData,
+    ThreadsUser,
+    ThreadData,
     GetUserProfileResponse,
     GetThreadLikersResponse,
     GetUserProfileThreadResponse,
     GetUserProfileRepliesResponse,
     GetUserProfileThreadsResponse,
 )
 
+DEFAULT_LSD_TOKEN = "NjppQDEgONsU_1LCzrmp6q"
+
 
 class ThreadsAPI:
-    fbLSDToken = "NjppQDEgONsU_1LCzrmp6q"  # FIXME: Remove default value
+    fbLSDToken = DEFAULT_LSD_TOKEN
     verbose = False
+    noUpdateLSD = False
     http_client = requests.Session()
 
-    def __init__(self, options=None):
-        if options and "fbLSDToken" in options:
-            self.fbLSDToken = options["fbLSDToken"]
-        if options and "verbose" in options:
-            self.verbose = options.verbose
-
-    def _get_default_headers(self, username):
-        return {
-            "authority": "www.threads.net",
-            "accept": "*/*",
-            "accept-language": "ko,en;q=0.9,ko-KR;q=0.8,ja;q=0.7",
-            "cache-control": "no-cache",
-            "origin": "https://www.threads.net",
-            "pragma": "no-cache",
-            "referer": f"https://www.threads.net/@{username}",
-            "x-asbd-id": "129477",
-            "x-fb-lsd": self.fbLSDToken,
-            "x-ig-app-id": "238260118697367",
-        }
+    def __init__(self, verbose=None, noUpdateLSD=None, fbLSDToken=None):
+        if fbLSDToken is not None and "str" == str(type(fbLSDToken)):
+            self.fbLSDToken = fbLSDToken
+        if noUpdateLSD is not None and "bool" == str(type(noUpdateLSD)):
+            self.noUpdateLSD = noUpdateLSD
+        if verbose is not None and "bool" == str(type(verbose)):
+            self.verbose = verbose
+
+    def __get_default_headers(self, username: str = None):
+        if username is None:
+            return {
+                "authority": "www.threads.net",
+                "accept": "*/*",
+                "accept-language": "ko,en;q=0.9,ko-KR;q=0.8,ja;q=0.7",
+                "cache-control": "no-cache",
+                "origin": "https://www.threads.net",
+                "pragma": "no-cache",
+                "referer": None,
+                "x-asbd-id": "129477",
+                "x-fb-lsd": self.fbLSDToken,
+                "x-ig-app-id": "238260118697367",
+            }
+        else:
+            return {
+                "authority": "www.threads.net",
+                "accept": "*/*",
+                "accept-language": "ko,en;q=0.9,ko-KR;q=0.8,ja;q=0.7",
+                "cache-control": "no-cache",
+                "origin": "https://www.threads.net",
+                "pragma": "no-cache",
+                "referer": f"https://www.threads.net/@{username}",
+                "x-asbd-id": "129477",
+                "x-fb-lsd": self.fbLSDToken,
+                "x-ig-app-id": "238260118697367",
+            }
+
+    def get_user_id_from_username(self, username) -> str:
+        """
+        Returns user id by username.
+
+        Args:
+            username (str): username on threads.net
 
-    def get_user_id_from_username(self, username, options=None) -> str:
-        headers = self._get_default_headers(username)
-        response = self.http_client.get(f"https://www.threads.net/@{username}", headers=headers)
+        Returns:
+            str: a user id.
+        """
+        headers = self.__get_default_headers(username)
         headers["accept"] = (
             "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
         )
         headers["accept-language"] = "ko,en;q=0.9,ko-KR;q=0.8,ja;q=0.7"
         headers["pragma"] = "no-cache"
         headers["referer"] = "https://www.instagram.com/"
         headers["sec-fetch-dest"] = "document"
         headers["sec-fetch-mode"] = "navigate"
         headers["sec-fetch-site"] = "cross-site"
         headers["sec-fetch-user"] = "?1"
         headers["upgrade-insecure-requests"] = "1"
         headers["x-asbd-id"] = None
         headers["x-fb-lsd"] = None
         headers["x-ig-app-id"] = None
+        response = self.http_client.get(f"https://www.instagram.com/{username}", headers=headers)
+
         text = response.text.replace("\n", "")
 
         user_id_match = re.search(r'"props":{"user_id":"(\d+)"},', text)
         user_id = user_id_match.group(1) if user_id_match else None
 
         lsd_token_match = re.search(r'"LSD",\[\],{"token":"(\w+)"},\d+\]', text)
         lsd_token = lsd_token_match.group(1) if lsd_token_match else None
-        if options is not None and options.fbLSDToken is not None:
+
+        if not self.noUpdateLSD and self.fbLSDToken is not None:
             self.fbLSDToken = lsd_token
             if self.verbose:
                 print("[fbLSDToken] UPDATED", self.fbLSDToken)
 
         return user_id
 
-    def get_user_profile(self, username, user_id=None):
+    def get_user_profile(self, username, user_id=None) -> ThreadsUser:
         """
-        Requires username and as an optional parameter user_id.
-        If no user_id is passed then the function will automatically get user_id by
-        resolving username.
+        Returns profile info by username.
+
+        Args:
+            username (str): username on threads.net
+            user_id (str, optional):: user_id which is unique to each user.
+
+        Returns:
+            ThreadsUser: a profile info.
         """
+        if self.verbose:
+            print("[fbLSDToken] USING", self.fbLSDToken)
+
         if not user_id:
             user_id = self.get_user_id_from_username(username)
-        headers = self._get_default_headers(username)
+        headers = self.__get_default_headers(username)
         headers["x-fb-friendly-name"] = "BarcelonaProfileRootQuery"
 
         params = {
             "lsd": self.fbLSDToken,
             "variables": f'{{"userID":"{user_id}"}}',
             "doc_id": "23996318473300828",
         }
 
         response = self.http_client.post(
             "https://www.threads.net/api/graphql", params=params, headers=headers
         )
-        user = GetUserProfileResponse.from_dict(response.json())
-        return user.data.userData.user
 
-    def get_user_profile_threads(self, username: str, user_id: str):
+        try:
+            user = GetUserProfileResponse.from_dict(response.json())
+            return user.data.userData.user
+        except Exception as e:
+            if self.verbose:
+                print("[ERROR] ", e)
+            return ThreadsUser(
+                pk="",
+                full_name="",
+                profile_pic_url="",
+                follower_count=0,
+                is_verified=False,
+                username="",
+                profile_context_facepile_users=None,
+                id=None,
+            )
+
+    def get_user_profile_threads(self, username: str, user_id: str) -> List[Thread]:
         """
-        Returns user profile threads as a dict
+        Returns a list of threads posted in the profile.
 
         Args:
-            username (string): username on threads.net
-            user_id (string): user_id which is unique to each user.
+            username (str): username on threads.net
+            user_id (str): user_id which is unique to each user.
 
         Returns:
-            dict: list of user profile threads.
+            List[Thread]: list of threads posted in the profile.
         """
-        headers = self._get_default_headers(username)
+        if self.verbose:
+            print("[fbLSDToken] USING", self.fbLSDToken)
+        headers = self.__get_default_headers(username)
         headers["x-fb-friendly-name"] = "BarcelonaProfileThreadsTabQuery"
 
         params = {
             "lsd": f"{self.fbLSDToken}",
             "variables": f'{{"userID":"{user_id}"}}',
             "doc_id": "6232751443445612",
         }
 
         response = self.http_client.post(
             "https://www.threads.net/api/graphql", params=params, headers=headers
         )
-        threads = GetUserProfileThreadsResponse.from_dict(response.json())
-        return threads.data.mediaData.threads
 
-    def get_user_profile_replies(self, username: str, user_id: str):
+        try:
+            threads = GetUserProfileThreadsResponse.from_dict(response.json())
+            return threads.data.mediaData.threads
+        except Exception as e:
+            if self.verbose:
+                print("[ERROR] ", e)
+            return []
+
+    def get_user_profile_replies(self, username: str, user_id: str) -> List[Thread]:
         """
-        Returns user profile replies as a list
+        Returns a list of replies in the thread.
 
         Args:
-            username (string): username on threads.net
-            user_id (string): user_id which is unique to each user.
+            username (str): username on threads.net
+            user_id (str): user_id which is unique to each user.
 
         Returns:
-            dict: list of user profile threads.
+            List[Thread]: list of replies in the thread.
         """
-        headers = self._get_default_headers(username)
+        if self.verbose:
+            print("[fbLSDToken] USING", self.fbLSDToken)
+        headers = self.__get_default_headers(username)
         headers["x-fb-friendly-name"] = "BarcelonaProfileRepliesTabQuery"
 
         params = {
             "lsd": f"{self.fbLSDToken}",
             "variables": f'{{"userID":"{user_id}"}}',
             "doc_id": "6307072669391286",
         }
 
         response = self.http_client.post(
             "https://www.threads.net/api/graphql", params=params, headers=headers
         )
-        replies = GetUserProfileRepliesResponse.from_dict(response.json())
-        return replies.data.mediaData.threads
 
-    def get_user_profile_thread(self, username: str, post_id: str):
+        try:
+            replies = GetUserProfileRepliesResponse.from_dict(response.json())
+            return replies.data.mediaData.threads
+        except Exception as e:
+            if self.verbose:
+                print("[ERROR] ", e)
+            return []
+
+    def get_post_id_from_thread_id(self, thread_id: str) -> str:
+        """
+        Returns a thread info from thread id.
+
+        Args:
+            thread_id (str): thread_id which is unique to each thread.
+
+        Returns:
+            str: a post id
         """
-        Returns a thread info
+        thread_id = thread_id.split("?")[0]
+        thread_id = thread_id.replace("/", "")
+        post_url = f"https://www.threads.net/t/{thread_id}"
+        result = self.get_post_id_from_url(post_url=post_url)
+        return result
+
+    def get_post_id_from_url(self, post_url) -> str:
+        """
+        Returns the post_id of a specific one thread.
 
         Args:
-            username (string): username on threads.net
-            post_id (string): post_id which is unique to each post.
+            post_url (str): a threads app direct link
 
         Returns:
-            dict: a thread info.
+            str: a post id
         """
-        headers = self._get_default_headers(username)
+        response = requests.get(post_url)
+        text = response.text
+        text = text.replace("\n", "")
+        post_id_match = re.search(r'{"post_id":"(.*?)"', text)
+        post_id = post_id_match.group(1) if post_id_match else None
+
+        lsd_token_match = re.search(r'"LSD",\[\],{"token":"(\w+)"},\d+\]', text)
+        lsd_token = lsd_token_match.group(1) if lsd_token_match else None
+
+        if not self.noUpdateLSD and self.fbLSDToken is not None:
+            self.fbLSDToken = lsd_token
+            if self.verbose:
+                print("[fbLSDToken] UPDATED", self.fbLSDToken)
+        return post_id
+
+    def get_threads(self, post_id: str) -> ThreadData:
+        """
+        Returns a thread info from post id.
+
+        Args:
+            post_id (str): post_id which is unique to each post.
+
+        Returns:
+            ThreadData: a thread info
+        """
+        if self.verbose:
+            print("[fbLSDToken] USING", self.fbLSDToken)
+        headers = self.__get_default_headers()
         headers["x-fb-friendly-name"] = "BarcelonaPostPageQuery"
 
         params = {
             "lsd": f"{self.fbLSDToken}",
             "variables": f'{{"postID":"{post_id}"}}',
             "doc_id": "5587632691339264",
         }
 
         response = self.http_client.post(
             "https://www.threads.net/api/graphql", params=params, headers=headers
         )
-        thread = GetUserProfileThreadResponse.from_dict(response.json())
-        return thread.data.data.containing_thread
 
-    def get_thread_likers(self, username: str, post_id: str):
+        try:
+            thread = GetUserProfileThreadResponse.from_dict(response.json())
+            return thread.data.data
+        except Exception as e:
+            if self.verbose:
+                print("[ERROR] ", e)
+            return ThreadData(containing_thread=None, reply_threads=[])
+
+    def get_thread_likers(self, post_id: str) -> UsersData:
         """
         Returns a thread likers
 
         Args:
-            username (string): username on threads.net
-            post_id (string): post_id which is unique to each post.
+            post_id (str): post_id which is unique to each post.
 
         Returns:
-            dict: a thread info.
+            UsersData: a thread likers
         """
-        headers = self._get_default_headers(username)
+        if self.verbose:
+            print("[fbLSDToken] USING", self.fbLSDToken)
+        headers = self.__get_default_headers()
 
         params = {
             "lsd": f"{self.fbLSDToken}",
             "variables": f'{{"mediaID":"{post_id}"}}',
             "doc_id": "9360915773983802",
         }
 
         response = self.http_client.post(
             "https://www.threads.net/api/graphql", params=params, headers=headers
         )
-        thread = GetThreadLikersResponse.from_dict(response.json())
-        return thread.data.likers
+
+        try:
+            thread = GetThreadLikersResponse.from_dict(response.json())
+            return thread.data.likers
+        except Exception as e:
+            if self.verbose:
+                print("[ERROR] ", e)
+            return UsersData(users=[])
```

### Comparing `threads-py-0.0.1/threadspy/types/__init__.py` & `threads-py-0.0.2/threadspy/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from .media_data import MediaData
 from .share_info import ShareInfo
 from .extensions import Extensions
 from .quoted_post import QuotedPost
 from .thread_item import ThreadItem
 from .thread_data import ThreadData
 from .reposted_post import RepostedPost
+from .users import UsersData
+from .threads_user import ThreadsUser
 from .video_version import VideoVersion
 from .image_versions2 import ImageVersions2
 from .user_profile_data import UserProfileData
 from .text_post_app_info import TextPostAppInfo
 from .reply_facepile_user import ReplyFacepileUser
 from .threads_user_summary import ThreadsUserSummary
 from .threads_hd_profile_pic_version import ThreadsHdProfilePicVersion
```

### Comparing `threads-py-0.0.1/threadspy/types/common.py` & `threads-py-0.0.2/threadspy/types/common.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.1/threadspy/types/post.py` & `threads-py-0.0.2/threadspy/types/post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.1/threadspy/types/quoted_post.py` & `threads-py-0.0.2/threadspy/types/quoted_post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.1/threadspy/types/reposted_post.py` & `threads-py-0.0.2/threadspy/types/reposted_post.py`

 * *Files identical despite different names*

### Comparing `threads-py-0.0.1/threadspy/types/threads_user.py` & `threads-py-0.0.2/threadspy/types/threads_user.py`

 * *Files identical despite different names*

