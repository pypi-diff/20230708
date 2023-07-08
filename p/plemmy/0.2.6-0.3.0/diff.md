# Comparing `tmp/plemmy-0.2.6.tar.gz` & `tmp/plemmy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.2.6.tar", last modified: Tue Jul  4 01:27:26 2023, max compression
+gzip compressed data, was "plemmy-0.3.0.tar", last modified: Sat Jul  8 04:04:43 2023, max compression
```

## Comparing `plemmy-0.2.6.tar` & `plemmy-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-04 01:27:26.043209 plemmy-0.2.6/
--rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.6/LICENSE
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-07-04 01:27:26.043018 plemmy-0.2.6/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.6/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-04 01:27:26.041907 plemmy-0.2.6/plemmy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.6/plemmy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    71480 2023-07-04 01:27:01.000000 plemmy-0.2.6/plemmy/lemmyhttp.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     2866 2023-06-30 20:43:38.000000 plemmy-0.2.6/plemmy/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-07-04 01:27:01.000000 plemmy-0.2.6/plemmy/version.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-04 01:27:26.042808 plemmy-0.2.6/plemmy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-07-04 01:27:26.000000 plemmy-0.2.6/plemmy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-07-04 01:27:26.043258 plemmy-0.2.6/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.6/setup.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-08 04:04:43.174264 plemmy-0.3.0/
+-rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.3.0/LICENSE
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2706 2023-07-08 04:04:43.174104 plemmy-0.3.0/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2420 2023-07-08 04:04:32.000000 plemmy-0.3.0/README.md
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-08 04:04:43.173018 plemmy-0.3.0/plemmy/
+-rw-r--r--   0 tjkessler   (501) staff       (20)      209 2023-07-08 04:04:32.000000 plemmy-0.3.0/plemmy/__init__.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    71480 2023-07-08 03:39:07.000000 plemmy-0.3.0/plemmy/lemmyhttp.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    13963 2023-07-08 04:04:32.000000 plemmy-0.3.0/plemmy/objects.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    19156 2023-07-08 04:04:32.000000 plemmy-0.3.0/plemmy/responses.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2866 2023-06-30 20:43:38.000000 plemmy-0.3.0/plemmy/utils.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-07-08 04:04:32.000000 plemmy-0.3.0/plemmy/version.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    16980 2023-07-08 04:04:32.000000 plemmy-0.3.0/plemmy/views.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-08 04:04:43.173893 plemmy-0.3.0/plemmy.egg-info/
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2706 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)      331 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/not-zip-safe
+-rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/requires.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-07-08 04:04:43.174310 plemmy-0.3.0/setup.cfg
+-rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.3.0/setup.py
```

### Comparing `plemmy-0.2.6/LICENSE` & `plemmy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.6/README.md` & `plemmy-0.3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -29,25 +29,53 @@
 ## Basic usage ##
 
 Interact with a Lemmy instance using the _LemmyHttp_ object:
 
 ```python
 from plemmy import LemmyHttp
 
-# create object for Lemmy.ml
+# create object for Lemmy.ml, log in
 srv = LemmyHttp("https://lemmy.ml")
-
-# log in to Lemmy.ml
 srv.login("<username_or_email>", "<password>")
+```
+
+Access specific communities:
+
+```python
+from plemmy.responses import GetComunityResponse
+
+# obtain community, parse JSON
+api_response = srv.get_community(name="Lemmy")
+response = GetCommunityResponse(api_response)
+
+# community info
+community = response.community_view.community
+print(community.name)
+print(community.actor_id)
+print(community.id)
+
+# list community moderators
+for person in response.moderators:
+    print(person.moderator.name, person.community.name)
+```
 
-# make a comment
-srv.create_comment("Hello from plemmy!", post_id)
+Create a post:
+```python
+from plemmy.responses import PostResponse
 
-# create a post
-srv.create_post(community_id, "New post's title", body="Body text", url="https://a.link.to.share")
+# create post, parse JSON
+api_response = srv.create_post(community.id, "Test post please ignore", "Body text")
+response = PostResponse(api_response)
+
+# post info
+post = response.post_view.post
+print(post.creator_id)
+print(post.community_id)
+print(post.name)
+print(post.body)
 ```
 
-Full documentation is on its way, but in the meantime check out our source code.
+Full documentation is on its way, but in the meantime check out our source code and some [examples]([https://github.com/tjkessler/plemmy/examples](https://github.com/tjkessler/plemmy/tree/main/examples)).
 
 ## Reporting issues, making contributions, etc. ##
 
 Don't hesitate to report a bug or unexpected results! Want to contribute? Make a pull request. Contact [@tjkessler](https://github.com/tjkessler) with any questions.
```

### Comparing `plemmy-0.2.6/plemmy/lemmyhttp.py` & `plemmy-0.3.0/plemmy/lemmyhttp.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.6/plemmy/utils.py` & `plemmy-0.3.0/plemmy/utils.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.6/setup.py` & `plemmy-0.3.0/setup.py`

 * *Files identical despite different names*

