# Comparing `tmp/jplaw-0.1.5.tar.gz` & `tmp/jplaw-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jplaw-0.1.5.tar", last modified: Sun Jul  2 05:30:02 2023, max compression
+gzip compressed data, was "jplaw-0.1.6.tar", last modified: Sat Jul  8 19:09:46 2023, max compression
```

## Comparing `jplaw-0.1.5.tar` & `jplaw-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:30:02.050643 jplaw-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-02 05:29:48.000000 jplaw-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-02 05:30:02.050643 jplaw-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-02 05:29:48.000000 jplaw-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:30:02.046643 jplaw-0.1.5/jplaw/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/api_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/community.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:30:02.050643 jplaw-0.1.5/jplaw/types/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/comment_sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/http_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/listing_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/modlog_action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/post_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/registration_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/search_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/types/subscribed_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-07-02 05:29:48.000000 jplaw-0.1.5/jplaw/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:30:02.046643 jplaw-0.1.5/jplaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-02 05:30:02.000000 jplaw-0.1.5/jplaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-02 05:30:02.000000 jplaw-0.1.5/jplaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:30:02.000000 jplaw-0.1.5/jplaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 05:30:02.000000 jplaw-0.1.5/jplaw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-02 05:29:48.000000 jplaw-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 05:30:02.050643 jplaw-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:09:46.552229 jplaw-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-08 19:09:33.000000 jplaw-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-08 19:09:46.552229 jplaw-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-08 19:09:33.000000 jplaw-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:09:46.552229 jplaw-0.1.6/jplaw/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/api_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27141 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:09:46.552229 jplaw-0.1.6/jplaw/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/comment_sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/http_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/listing_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/modlog_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/post_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/registration_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/search_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/types/subscribed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-07-08 19:09:33.000000 jplaw-0.1.6/jplaw/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:09:46.552229 jplaw-0.1.6/jplaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-08 19:09:46.000000 jplaw-0.1.6/jplaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-08 19:09:46.000000 jplaw-0.1.6/jplaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 19:09:46.000000 jplaw-0.1.6/jplaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 19:09:46.000000 jplaw-0.1.6/jplaw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 19:09:33.000000 jplaw-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 19:09:46.552229 jplaw-0.1.6/setup.cfg
```

### Comparing `jplaw-0.1.5/LICENSE` & `jplaw-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.5/PKG-INFO` & `jplaw-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jplaw-0.1.5/README.md` & `jplaw-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.5/jplaw/api_paths.py` & `jplaw-0.1.6/jplaw/api_paths.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.5/jplaw/comment.py` & `jplaw-0.1.6/jplaw/comment.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,209 +1,201 @@
+"""
+Comment class. Designed to allow Lemmy.Comment functions.
+"""
 from jplaw.requestor import Requestor
 from jplaw.api_paths import *
 from jplaw.types.listing_type import ListingType
 from jplaw.types.comment_sort_type import CommentSortType
 
 class Comment():
-    """
-    Comment class. Designed to allow Lemmy.Comment functions.
-    """
     def __init__(self, _req: Requestor):
         self._req = _req
         
-    def create(self, post_id:int, content:str, parent_id:int=None, language_id:int=None, instance:str=None, auth_token:str=None):
+    def create(self, post_id:int, content:str, parent_id:int=None, language_id:int=None, instance:str=None):
         """
         Create a comment
         
         Args:
             post_id (int): ID of the post to create a comment on
             content (str): Contents of the comment
             parent_id (int): Parent comment ID. Optional. Default/If None, posts comment directly to post.
             language_id (int): Language ID
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Comment response
         """
         form = {
             "content": content,
             "post_id": post_id,
         }
         optional={
             "language_id": language_id,
             "parent_id": parent_id
         }
-        res = self._req.lemmyRequest("createComment", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("createComment", instance=instance, form=form, optional=optional, auth=True)
         
         return res["comment_view"]
         
-    def like(self, comment_id:int, score:int=1, instance:str=None, auth_token:str=None):
+    def like(self, comment_id:int, score:int=1, instance:str=None):
         """
         Like a comment
         
         Args:
             comment_id (int): ID of the comment
             score (int): Score of the comment. -1/0/1 dislikes, removes like, and likes a comment.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Comment response
         """
         if(score > 1):
             score = 1
         if(score < -1):
             score = -1
         form = {
             "comment_id": comment_id,
             "score": score
         }
-        res = self._req.lemmyRequest("likeComment", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("likeComment", instance=instance, form=form, auth=True)
         return res["comment_view"]
         
-    def report(self, comment_id:int, reason:str, instance:str=None, auth_token:str=None):
+    def report(self, comment_id:int, reason:str, instance:str=None):
         """
         Report a comment
         
         Args:
             comment_id (int): ID of the comment
             reason (str): Reason for reporting the comment
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Comment report response
         """
         form = {
             "comment_id": comment_id,
             "reason": reason
             }
-        res = self._req.lemmyRequest("createCommentReport", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("createCommentReport", instance=instance, form=form, auth=True)
         return res
         
-    def delete(self, comment_id:int, deleted:bool=True, instance:str=None, auth_token:str=None):
+    def delete(self, comment_id:int, deleted:bool=True, instance:str=None):
         """
         Delete a comment
         
         Args:
             comment_id (int): ID of the comment
             deleted (bool): If comment is deleted. Optional. Defaults to true
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Comment response
         """
         form = {
             "comment_id": comment_id,
             "deleted": deleted
             }
-        res = self._req.lemmyRequest("deleteComment", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("deleteComment", instance=instance, form=form, auth=True)
         return res["comment_view"]
         
-    def remove(self, comment_id:int, mod_person_id:int, when_:str, removed:bool=True, reason:str=None, instance:str=None, auth_token:str=None):
+    def remove(self, comment_id:int, mod_person_id:int, when_:str, removed:bool=True, reason:str=None, instance:str=None):
         """
         Moderator remove a comment
         
         Args:
             comment_id (int): ID of the comment
             mod_person_id (int): ID of the moderator removing the comment
             when_ (str): Timestamp for when the comment was removed
             removed (bool): If the comment is removed. Optional. Defaults to true.
             deleted (bool): If comment is deleted. Optional. Defaults to true
             reason (str): Reason for removing the comment. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Comment response
         """
         form = {
             "comment_id": comment_id,
             "mod_person_id": mod_person_id,
             "when_": when_,
             "removed": removed,
             }
         optional={
             "reason":reason,
             }
-        res = self._req.lemmyRequest("removeComment", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("removeComment", instance=instance, form=form, optional=optional, auth=True)
         return res["comment_view"]
         
-    def distinguish(self, comment_id:int, distinguished:bool=True, instance:str=None, auth_token:str=None):
+    def distinguish(self, comment_id:int, distinguished:bool=True, instance:str=None):
         """
         Distinguish a comment
         
         Args:
             comment_id (int): ID of the comment
             distinguished (bool): If comment is distinguished. Optional. Defaults to true
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Comment response
         """
         form = {
             "comment_id": comment_id,
             "distinguished": distinguished,
             }
-        res = self._req.lemmyRequest("distinguishComment", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("distinguishComment", instance=instance, form=form, auth=True)
         return res["comment_view"]
         
-    def edit(self, comment_id:int, content:str=None, language_id:int=None, form_id:str=None, instance:str=None, auth_token:str=None):
+    def edit(self, comment_id:int, content:str=None, language_id:int=None, form_id:str=None, instance:str=None):
         """
         Edit a comment
         
         Args:
             comment_id (int): ID of the comment
             content (str): content of the comment
             language_id (int): Language of the comment
             form_id (str): ???
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Comment response
         """
         form = {
             "comment_id": comment_id
             }
         optional={
             "content":content,
             "language_id":language_id,
             "form_id":form_id,
             }
-        res = self._req.lemmyRequest("editComment", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("editComment", instance=instance, form=form, optional=optional, auth=True)
         return res["comment_view"]
         
-    def get(self, comment_id:int, instance:str=None, auth:bool=True, auth_token:str=None):    
+    def get(self, comment_id:int, instance:str=None, auth:bool=True):    
         """
         Get a comment by id
         
         Args:
             comment_id (int): ID of the comment
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            auth (bool): Whether to authenticate using login or not. Optional. Defaults to True
         Returns:
             Comment response
         """
         form = {
             "comment_id": comment_id
             }
-        res = self._req.lemmyRequest("getComment", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("getComment", instance=instance, form=form, optional=optional, auth=auth)
         return res["comment_view"]
         
     def list(self, 
         comment_type:ListingType=None, 
         sort:CommentSortType=None, 
         max_depth:int=None, 
         page:int=None, 
         limit:int=None, 
         community_id:int=None, 
         post_id:int=None, 
         community_name:str=None, 
         parent_id:int=None,
         saved_only:bool=None,
         instance:str=None, 
-        auth:bool=True, 
-        auth_token:str=None):
+        auth:bool=True):
         """
         Get comments in a post
         
         Args:
             comment_id (int): ID of the comment
             comment_type (ListingType): Comment type. Optional.
             sort (CommentSortType): Sort type. Optional.
@@ -213,113 +205,105 @@
             community_id (int): ID of community to get comment from. Optional.
             post_id (int): ID of post to get comments from. Optional.
             community_name (str): Name of community to get comments from. Optional.
             parent_id (int): ID of parent comment to get replies to. Optional.
             saved_only (bool): Filter by only saved comments. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
             auth (bool): Whether or not to authenticate. Optional. True by default.
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Comment list
         """
         form = {
             "comment_id": comment_id
             }
-        if(comment_type):
-            form["type_"] = comment_type,
-        if(sort):
-            form["sort"] = sort
-
         optional={
-            "max_depth"      : max_depth       ,
-            "page"           : page            ,
-            "limit"          : limit           ,
-            "post_id"        : post_id         ,
-            "community_id"   : community_id    ,
-            "community_name" : community_name  ,
-            "parent_id"      : parent_id       ,
-            "saved_only"     : saved_only      ,
+            "type_"             : type_             ,
+            "sort"              : sort              ,
+            "max_depth"         : max_depth         ,
+            "page"              : page              ,
+            "limit"             : limit             ,
+            "post_id"           : post_id           ,
+            "community_id"      : community_id      ,
+            "community_name"    : community_name    ,
+            "parent_id"         : parent_id         ,
+            "saved_only"        : saved_only        ,
             }
        
-        res = self._req.lemmyRequest("getComments", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("getComments", instance=instance, form=form, optional=optional, auth=auth)
         return res["comment_view"]
     
-    def listReports(self, page:int=None, limit:int=None, unresolved_only:bool=None, community_id:int=None, instance:str=None, auth_token:str=None):
+    def listReports(self, page:int=None, limit:int=None, unresolved_only:bool=None, community_id:int=None, instance:str=None):
         """
         Get list of comment reports
         
         Args:
             page (int): Page number. Optional.
             limit (int): Comment count limit. Optional.
             unresolved_only (bool): If only unresolved reports should be listed. Optional.
             community_id (int): ID of community to get comment from. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Comment report list response
         """
         form = {}
         optional={
             "page"           : page            ,
             "limit"          : limit           ,
             "community_id"   : community_id    ,
             "unresolved_only": unresolved_only ,
             }
-        res = self._req.lemmyRequest("listCommentReports", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("listCommentReports", instance=instance, form=form, optional=optional, auth=auth)
         return
         
-    def markReplyAsRead(self, comment_reply_id:int, read:bool=True, instance:str=None, auth_token:str=None):
+    def markReplyAsRead(self, comment_reply_id:int, read:bool=True, instance:str=None):
         """
         Mark a reply as read
         
         Args:
             comment_reply_id (int): ID of comment reply.
             read (bool): If reply is marked as read. Optional. Defaults to True
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Comment reply marked as read response
         """
         form = {
             "comment_reply_id"  : comment_reply_id  ,
             "read"              : read              ,
             }
-        res = self._req.lemmyRequest("markCommentReplyAsRead", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("markCommentReplyAsRead", instance=instance, form=form, auth=auth)
         return
     
-    def resolveReport(self, report_id:int, resolved:bool=True, instance:str=None, auth_token:str=None):
+    def resolveReport(self, report_id:int, resolved:bool=True, instance:str=None):
         """
         Resolve a comment report
         
         Args:
             report_id (int): ID of report.
             resolved (bool): If reply is marked as read. Optional. Defaults to True
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Report resolved response
         """
         form = {
             "report_id"  : report_id ,
             "resolved"   : resolved  ,
             }
-        res = self._req.lemmyRequest("resolveCommentReport", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("resolveCommentReport", instance=instance, form=form, auth=auth)
         return
     
-    def save(self, comment_id:int, save:bool=True, instance:str=None, auth_token:str=None):
+    def save(self, comment_id:int, save:bool=True, instance:str=None):
         """
         Save a comment
         
         Args:
             comment_id (int): ID of comment.
             save (bool): If comment is saved or not. Optional. Defaults to True
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Report resolved response
         """
         form = {
             "comment_id"  : comment_id ,
             "save"   : save,
             }
-        res = self._req.lemmyRequest("saveComment", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("saveComment", instance=instance, form=form, auth=auth)
         return
```

### Comparing `jplaw-0.1.5/jplaw/community.py` & `jplaw-0.1.6/jplaw/community.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,170 +7,169 @@
 from .types.listing_type import ListingType
 from .types.sort_type import SortType
 
 class Community():
     def __init__(self, _req: Requestor):
         self._req = _req
         
-    def get(self, name:str, instance:str=None, auth:bool=True, auth_token:str=None):
+    def get(self, name:str, instance:str=None, auth:bool=True):
         """
         Get community information
         
         Args:
             name (str): Name of the community. Federated communities can be accessed by [community]@[instance] 
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth (str): If true, authenticates using auth_token if given or internal token from login. Optional. Default True
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            auth (str): If true, authenticates using internal token from login. Optional. Default True
         Returns:
             Community Information. Throws an error if community_not_found (happens if community has not been federated or does not exist)
         """
         form = {
             "name": name
         }
-        res = self._req.lemmyRequest("getCommunity", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("getCommunity", instance=instance, form=form, auth=auth)
         return res["community_view"]
         
-    def list(self, type: ListingType=None, sort:SortType=None, page:int=None, limit:int=None, instance:str=None, auth:bool=True, auth_token:str=None): 
+    def list(self, 
+        type: ListingType=None, 
+        sort:SortType=None,
+        show_nsfw: bool=None,
+        page:int=None, 
+        limit:int=None, 
+        instance:str=None, 
+        auth:bool=True): 
         """
         Get a list of communities (federated or local)
         
         Args:
             type (ListingType): Type of community (all or local). Optional
             sort (SortType): Sorting Mode. Optional
+            show_nsfw (bool): Whether or not to show nsfw communities. Optional. 
             page (int): Page number. Optional
             limit (int): Limit for number of posts. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth (str): If true, authenticates using auth_token if given or internal token from login. Optional. Default True
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            auth (str): If true, authenticates using internal token from login. Optional. Default True
         Returns:
             List of communities
         """
         form={}
-        if(type):
-            form["type"]=type.value
-        if(sort):
-            form["sort"]=sort.value
         optional={
-            "page": page,
-            "limit": limit
+            "sort"      : sort,
+            "type"      : type,
+            "show_nsfw" : show_nsfw,
+            "page"      : page,
+            "limit"     : limit
             }
-        res = self._req.lemmyRequest("listCommunities", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("listCommunities", instance=instance, form=form, optional=optional, auth=auth)
         return res["communities"]
         
-    def follow(self, community_id:int, follow:bool=True, instance:str=None, auth_token:str=None):
+    def follow(self, community_id:int, follow:bool=True, instance:str=None):
         """
         Follow or subscribe to a community
         
         Args:
             community_id (int): ID of the community
             follow (bool): If true, subscribed to or following the community. Optional. Defaults to True
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             List of communities
         """
         form={
             "community_id": community_id,
             "follow": follow
         }
-        res = self._req.lemmyRequest("followCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("followCommunity", instance=instance, form=form, auth=True)
         return res["community_view"]
-    def addMod(self, community_id:int, person_id:int, added:bool=True, instance:str=None, auth_token:str=None): 
+    def addMod(self, community_id:int, person_id:int, added:bool=True, instance:str=None): 
         """
         Add or remove a moderator from a community
         
         Args:
             community_id (int): ID of the community
             person_id (int): User ID of the person to add as a moderator
             added (bool): If true, person is added as a moderator. If false, person is removed as a moderator. Optonal. Default True
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Added moderator response
         """
         form={
             "community_id": community_id,
             "person_id": person_id,
             "added": added,
         }
-        res = self._req.lemmyRequest("addModToCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("addModToCommunity", instance=instance, form=form, auth=True)
         return res
     
-    def banPerson(self, community_id:int, person_id:int, ban:bool, remove_data:bool=None, reason:str=None, expires:int=None, instance:str=None, auth_token:str=None):
+    def banPerson(self, community_id:int, person_id:int, ban:bool, remove_data:bool=None, reason:str=None, expires:int=None, instance:str=None):
         """
         Ban a person from a community
         
         Args:
             community_id (int): ID of the community
             person_id (int): User ID of the person to ban
             ban (bool): If true, person is banned. If false, person is unbanned Optonal. Default True
             remove_data (bool): ??? Presumably removes the user's posts and comments or removes their data from the instance. Optional.
             reason (str): Reason for banning user. Optional
             expires (int): Unix timestamp of ban expiry (seconds)
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Banned community response
         """
         form={
             "community_id": community_id,
             "person_id": person_id,
             "ban": ban,
         }
         optional={
             "remove_data": remove_data,
             "reason": reason,
             "expires": expires,
         }
-        res = self._req.lemmyRequest("banFromCommunity", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("banFromCommunity", instance=instance, form=form, optional=optional, auth=True)
         return res
         
-    def block(self, community_id:int, block:bool=True, instance:str=None, auth_token:str=None):
+    def block(self, community_id:int, block:bool=True, instance:str=None):
         """
         Block a community
         
         Args:
             community_id (int): ID of the community
             ban (bool): If true, community blocked. If false, community is unblocked. Optonal. Default True
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Blocked community response
         """
         form={
             "community_id": community_id,
             "block": block,
             }
-        res = self._req.lemmyRequest("blockCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("blockCommunity", instance=instance, form=form, auth=True)
         return res["community_view"]
         
     def create(self, name:str, 
         title:str, 
         description:str=None, 
         icon:str=None, 
         banner:str=None, 
         nsfw:bool=None, 
         posting_restricted_to_mods:bool=None, 
         discussion_languages:List[int]=None, 
-        instance:str=None, 
-        auth_token:str=None):
+        instance:str=None):
         """
         Create a community
         
         Args:
             name (str): Name of the community
             title (str): Title of the community. Can have spaces.
             description (str): Description of the community. Optional.
             icon (str): URL of the community icon. Optional.
             banner (str): URL of the community banner image. Optional.
             nsfw (bool): If true, community is NSFW. Optional.
             posting_restricted_to_mods (bool): If true, only moderators can post. Optional.
             discussion_languages (List[int]): List of langages in community. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Created community response
         """
         form={
             "name": name,
             "title": title,
             }
@@ -178,61 +177,58 @@
             "description": description,
             "icon": icon,
             "banner": banner,
             "nsfw": nsfw,
             "posting_restricted_to_mods": posting_restricted_to_mods,
             "discussion_languages": discussion_languages,
             }
-        res = self._req.lemmyRequest("createCommunity", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("createCommunity", instance=instance, form=form, optional=optional, auth=True)
         return res["community_view"]
         
-    def delete(self, community_id:int, deleted:bool=True, instance:str=None, auth_token:str=None):
+    def delete(self, community_id:int, deleted:bool=True, instance:str=None):
         """
         Delete a community
         
         Args:
             community_id (int): ID of the community
             deleted (bool): If true, community is deleted. If false, community is not deleted. Optonal. Default True
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Deleted community response
         """
         form={
             "community_id": community_id,
             "deleted": deleted,
             }
-        res = self._req.lemmyRequest("deleteCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("deleteCommunity", instance=instance, form=form, auth=True)
         return res["community_view"]
     
     def edit(self, 
         community_id:int, 
         title:str=None, 
         description:str=None, 
         icon:str=None, 
         banner:str=None, 
         nsfw:bool=None, 
         posting_restricted_to_mods:bool=None, 
         discussion_languages:List[int]=None, 
-        instance:str=None, 
-        auth_token:str=None):
+        instance:str=None):
         """
         Edit a community. Excluding optional items does not edit those items.
         
         Args:
             community_id (int): ID of the community to edit
             title (str): Title of the community. Can have spaces. Optional
             description (str): Description of the community. Optional.
             icon (str): URL of the community icon. Optional.
             banner (str): URL of the community banner image. Optional.
             nsfw (bool): If true, community is NSFW. Optional.
             posting_restricted_to_mods (bool): If true, only moderators can post. Optional.
             discussion_languages (List[int]): List of langages in community. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Edited community response
         """
         form={
             "community_id": community_id,
             }
         optional={
@@ -240,53 +236,51 @@
             "description": description,
             "icon": icon,
             "banner": banner,
             "nsfw": nsfw,
             "posting_restricted_to_mods": posting_restricted_to_mods,
             "discussion_languages": discussion_languages,
             }
-        res = self._req.lemmyRequest("createCommunity", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("createCommunity", instance=instance, form=form, optional=optional, auth=True)
         return res["community_view"]
         
-    def remove(self, community_id:int, removed:bool=True, reason:str=None, expires:int=None, instance:str=None, auth_token:str=None):
+    def remove(self, community_id:int, removed:bool=True, reason:str=None, expires:int=None, instance:str=None):
         """
         Remove a community
         
         Args:
             community_id (int): ID of the community
             removed (bool): If true, community is removed. If false, community is restored. Optonal. Default True
             reason (str): Reason for community removal. Optional.
             expires (int): Unix timestamp (seconds) of expiry.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Removed community response
         """
         form={
             "community_id": community_id,
             "removed":removed,
             }
         optional={
             "reason": reason,
             "expires": expires,
             }
-        res = self._req.lemmyRequest("removeCommunity", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("removeCommunity", instance=instance, form=form, optional=optional, auth=True)
         return res["community_view"]
     
-    def transfer(self, community_id:int, person_id:int, instance:str=None, auth_token:str=None):
+    def transfer(self, community_id:int, person_id:int, instance:str=None):
         """
         Transfer ownership of a community
         
         Args:
             community_id (int): ID of the community
             person_id (int): User ID of the person to transfer ownership to
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Removed community response
         """
         form={
             "community_id": community_id,
             "person_id":person_id,
             }
-        res = self._req.lemmyRequest("transferCommunity", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("transferCommunity", instance=instance, form=form, auth=True)
         return res["community_view"]
```

### Comparing `jplaw-0.1.5/jplaw/emoji.py` & `jplaw-0.1.6/jplaw/emoji.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,73 +8,70 @@
 from jplaw.types.listing_type import ListingType
 from jplaw.types.registration_mode import RegistrationMode
 
 class Emoji():
     def __init__(self, _req: Requestor):
         self._req = _req
     
-    def create(self, category:str, shortcode:str, image_url:str, alt_text:str, keywords:List[str], instance:str=None, auth_token:str=None):
+    def create(self, category:str, shortcode:str, image_url:str, alt_text:str, keywords:List[str], instance:str=None):
         """
         Create a custom emoji
         
         Args:
             category (str): Category of the emoji
             shortcode (str): Short code used to type the emoji
             image_url (str): URL of the image to use
             alt_text (str): Alt text (hover or screenreader) of the emoji
             keywords (List[str]): Keywords of the emoji.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Emoji created response
         """
         form={
             "category": category,
             "shortcode": shortcode,
             "image_url": image_url,
             "alt_text": alt_text,
             "keywords": keywords
             }
-        res = self._req.lemmyRequest("createCustomEmoji", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("createCustomEmoji", instance=instance, form=form, auth=auth)
         return res
         
-    def edit(self, emoji_id:int, category:str=None, image_url:str=None, alt_text:str=None, keywords:List[str]=None, instance:str=None, auth_token:str=None):
+    def edit(self, emoji_id:int, category:str=None, image_url:str=None, alt_text:str=None, keywords:List[str]=None, instance:str=None):
         """
         Edit a custom emoji. Excluded optional arguments are not modified.
         
         Args:
             emoji_id (int): ID of the emoji
             category (str): Category of the emoji. Optional
             image_url (str): URL of the image to use. Optional
             alt_text (str): Alt text (hover or screenreader) of the emoji. Optional
             keywords (List[str]): Keywords of the emoji. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Emoji edited response
         """
         form={
             "id": emoji_id,
             "category": category,
             "image_url": image_url,
             "alt_text": alt_text,
             "keywords": keywords
             }
-        res = self._req.lemmyRequest("editCustomEmoji", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("editCustomEmoji", instance=instance, form=form, auth=auth)
         return res
         
-    def delete(self, emoji_id:int, instance:str=None, auth_token:str=None):
+    def delete(self, emoji_id:int, instance:str=None):
         """
         Delete a custom emoji from the website
         
         Args:
             emoji_id (int): ID of emoji to delete
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
         Returns:
             Emoji deleted response
         """
         form={
             "id": emoji_id
             }
-        res = self._req.lemmyRequest("deleteCustomEmoji", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("deleteCustomEmoji", instance=instance, form=form, auth=auth)
         return res
```

### Comparing `jplaw-0.1.5/jplaw/lemmy.py` & `jplaw-0.1.6/jplaw/lemmy.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.5/jplaw/post.py` & `jplaw-0.1.6/jplaw/post.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,346 +7,341 @@
 from jplaw.types.listing_type import ListingType
 from jplaw.types.sort_type import SortType
 
 class Post():
     def __init__(self, _req: Requestor):
         self._req = _req
         
-    def list(self, type:ListingType=None, sort:SortType=None, page:int=None, limit:int=None, community_id:int=None, community_name:str=None, saved_only:bool=None, instance:str=None, auth:bool=True, auth_token:str=None):
+    def list(self, type:ListingType=None, sort:SortType=None, page:int=None, limit:int=None, community_id:int=None, community_name:str=None, saved_only:bool=None, instance:str=None, auth:bool=True):
         """
         Get a list of posts in a community
         
         Args:
             type (ListingType): Type of post. Optional
             sort (SortType): Sorting Mode. Optional
             page (int): Page number. Optional
             limit (int): Limit for number of posts. Optional
             community_id (int): ID of the community the post is in. Optional
             community_name (str): Name of the community the post is in. Optional
             saved_only (bool): Find posts only from saved posts. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth (str): If true, authenticates using auth_token if given or internal token from login. Optional. Default True
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            auth (str): If true, authenticates using internal token from login. Optional. Default True
         Returns:
             List of posts
         """
         form = {}
-        if(sort):
-            form["sort"] = sort.value
-        if(type):
-            form["type"] = type.value
         optional = {
+            "sort": sort,
+            "type": type,
             "community_id": community_id,
             "page": page,
             "limit": limit,
-            "community_id": community_id,
             "community_name": community_name,
             "saved_only": saved_only
             }
-        res = self._req.lemmyRequest("getPosts", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("getPosts", instance=instance, form=form, optional=optional, auth=auth)
         return res["posts"]
         
-    def get(self, post_id:int=None, comment_id:int=None, instance:str=None, auth:bool=True, auth_token:str=None):
+    def get(self, post_id:int=None, comment_id:int=None, instance:str=None, auth:bool=True):
         """
         Get a post by ID
         
         Args:
             post_id (int): ID of the post. Optional
             comment_id (int): Comment ID for comment view. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth (str): If true, authenticates using auth_token if given or internal token from login. Optional. Default True
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            auth (str): If true, authenticates using internal token from login. Optional. Default True
         Returns:
             Post response
         """
         form = {}
         optional = {
             "id": post_id,
             "comment_id": comment_id,
             }
-        res = self._req.lemmyRequest("getPost", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("getPost", instance=instance, form=form, optional=optional, auth=auth)
         return res["post_view"]
         
-    def create(self, community_id:int, title:str=None, body:str=None, remote_url:str=None, honeypot:str=None, nsfw=False, language_id:int=None, instance:str=None, auth_token:str=None):
+    def create(self, community_id:int, title:str=None, body:str=None, remote_url:str=None, honeypot:str=None, nsfw=False, language_id:int=None, instance:str=None):
         """
         Create a post
         
         Args:
             community_id (int): ID of the community the post is in. Optional
             title (str): Title of the post. Optional.
             body (str): Text contents of the post. Optional
             remote_url (str): URL if link post. Optional.
             nsfw (bool): NSFW post. Optional. Defaults to false.
             language_id (int): Language ID
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Created post response
         """
         form = {}
         optional={
             "url": remote_url,
             "community_id": community_id,
             "name": title,
             "body": body,
             "language_id": language_id,
             "nsfw": nsfw,
             "honeypot": honeypot
             }
-        res = self._req.lemmyRequest("createPost", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("createPost", instance=instance, form=form, optional=optional, auth=True)
         return res["post_view"]
         
-    def edit(self, post_id:int, title:str=None, body:str=None, remote_url:str=None, nsfw:bool=None, language_id:int=None, instance:str=None, auth_token:str=None):
+    def edit(self, post_id:int, title:str=None, body:str=None, remote_url:str=None, nsfw:bool=None, language_id:int=None, instance:str=None):
         """
         Edit a post
         
         Args:
             post_id (int): ID of the post to edit
             title (str): Title of the post. Optional.
             body (str): Text contents of the post. Optional
             remote_url (str): URL if link post. Optional.
             nsfw (bool): NSFW post. Optional. Defaults to None.
             language_id (int): Language ID
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Edited post response
         """
         form = {
             "post_id": post_id,
         }
         optional={
             "url": remote_url,
             "nsfw": nsfw,
             "language_id": language_id,
             "name": title,
             "body": body
         }
-        res = self._req.lemmyRequest("editPost", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("editPost", instance=instance, form=form, optional=optional, auth=True)
         return res["post_view"]
         
-    def like(self, post_id:int, score:int=1, instance:str=None, auth_token:str=None):
+    def like(self, post_id:int, score:int=1, instance:str=None):
         """
         Like a post
         
         Args:
             post_id (int): ID of the post
             score (int)::1 for like, -1 for dislike, 0 to remove like. Clamped to 1/0/-1.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Liked post response
         """
         if(score > 1):
             score = 1
         if(score < -1):
             score = -1
         form = {
             "post_id": post_id,
             "score": score
             }
-        res = self._req.lemmyRequest("likePost", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("likePost", instance=instance, form=form, auth=True)
         return res
     
-    def report(self, post_id:int, reason:str, instance:str=None, auth_token:str=None):
+    def report(self, post_id:int, reason:str, instance:str=None):
         """
         Report a post
         
         Args:
             post_id (int): ID of the post
             reason (str): Reason for reporting the post
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Reported post response
         """
         form = {
             "post_id": post_id,
             "reason": reason
             }
-        res = self._req.lemmyRequest("createPostReport", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("createPostReport", instance=instance, form=form, auth=True)
         return res
         
-    def delete(self, post_id:int, deleted:bool=True, instance:str=None, auth_token:str=None):
+    def delete(self, post_id:int, deleted:bool=True, instance:str=None):
         """
         Delete a post
         
         Args:
             post_id (int): ID of the post
             deleted (bool): If post is deleted. Optional. Defaults to true.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Deleted post response
         """
         form = {
             "post_id": post_id,
             "deleted": deleted
             }
-        res = self._req.lemmyRequest("deletePost", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("deletePost", instance=instance, form=form, auth=True)
         return res
         
-    def feature(self, post_id:int, feature_type: PostFeatureType, featured:bool=True, instance:str=None, auth_token:str=None):
+    def feature(self, post_id:int, feature_type: PostFeatureType, featured:bool=True, instance:str=None):
         """
         Feature a post
         
         Args:
             post_id (int): ID of the post
             feature_type (PostFeatureType): Type of featured post. Currently Community and Local.
             featured (bool): If post is featured or not. Optional. Defaults to True.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Featured post response
         """
         form = {
             "post_id": post_id,
             "featured": featured,
             }
         if(feature_type):
             form["feature_type"] = feature_type.value
-        res = self._req.lemmyRequest("featurePost", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("featurePost", instance=instance, form=form, auth=True)
         return res
         
-    def listReports(self, page:int=None, limit:int=None, unresolved_only:bool=True, community_id:int=None, instance:str=None, auth_token:str=None):
+    def listReports(self, page:int=None, limit:int=None, unresolved_only:bool=True, community_id:int=None, instance:str=None):
         """
         Get list of post reports
         
         Args:
             page (int): Page number. Optional
             limit (int): Limit for number of posts. Optional
             unresolved_only (bool): If only unresolved posts should be shown. Optional
             community_id (int): ID of the community to filter reports from. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             List of reported posts
         """
         form = {}
         optional = {
             "page": page,
             "limit": limit,
             "unresolved_only": unresolved_only,
             "community_id": community_id,
             }
-        res = self._req.lemmyRequest("listPostReports", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("listPostReports", instance=instance, form=form, optional=optional, auth=True)
         return res
     
-    def lock(self, post_id:int, locked:bool=True, instance:str=None, auth_token:str=None):
+    def lock(self, post_id:int, locked:bool=True, instance:str=None):
         """
         Lock a post
         
         Args:
             post_id (int): ID of the post
             locked (bool): If post is locked. Optional. Defaults to true.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Locked post response
         """
         form = {
             "post_id": post_id,
             "locked": locked,
         }
-        res = self._req.lemmyRequest("lockPost", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("lockPost", instance=instance, form=form, auth=True)
         return res
         
-    def markAsRead(self, post_id:int, read:bool=True, instance:str=None, auth_token:str=None):
+    def markAsRead(self, post_id:int, read:bool=True, instance:str=None):
         """
         Mark a post as read
         
         Args:
             post_id (int): ID of the post
             read (bool): If post is read. Optional. Defaults to true.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Read post response
         """
         form = {
             "post_id": post_id,
             "read": read,
         }
-        res = self._req.lemmyRequest("markPostAsRead", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("markPostAsRead", instance=instance, form=form, auth=True)
         return res
     
-    def resolveReport(self, report_id:int, resolved:bool=True, instance:str=None, auth_token:str=None):
+    def resolveReport(self, report_id:int, resolved:bool=True, instance:str=None):
         """
         Resolve a post report
         
         Args:
             report_id (int): ID of the post report
             resolved (bool): If post report is resolved. Optional. Defaults to true.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Post report resolved response
         """
         form = {
             "report_id"  : report_id ,
             "resolved"   : resolved  ,
             }
-        res = self._req.lemmyRequest("resolvePostReport", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("resolvePostReport", instance=instance, form=form, auth=auth)
         return
         
-    def save(self, post_id:int, save:bool=True, instance:str=None, auth_token:str=None):
+    def save(self, post_id:int, save:bool=True, instance:str=None):
         """
         Save a post
         
         Args:
             post_id (int): ID of the post
             save (bool): If post is saved. Optional. Defaults to true.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Post report resolved response
         """
         form = {
             "post_id"  : post_id ,
             "save"   : save,
             }
-        res = self._req.lemmyRequest("savePost", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("savePost", instance=instance, form=form, auth=auth)
         return
         
-    def getSiteMetadata(self, remote_url:str, instance:str=None, auth:bool=True, auth_token:str=None):
+    def getSiteMetadata(self, remote_url:str, instance:str=None, auth:bool=True):
         """
         Gets metadata for a site when linked by a post
         
         Args:
             remote_url (str): URL of the site to get the metadata for
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Post report resolved response
         """
         form={
             "url": remote_url,
         }
-        res = self._req.lemmyRequest("getSiteMetadata", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("getSiteMetadata", instance=instance, form=form, auth=auth)
         return res
         
-    def remove(self, post_id:int, mod_person_id:int, when_:str, removed:bool=True, reason:str=None, instance:str=None, auth_token:str=None):
+    def remove(self, post_id:int, mod_person_id:int, when_:str, removed:bool=True, reason:str=None, instance:str=None):
         """
         Remove a post as a moderator
         
         Args:
             post_id (int): ID of the post to remove
             mod_person_id (int): ID of the moderator removing the post
             when_ (str): Timestamp of when post was removed
             removed (bool): If post is removed. Optional. Defaults to True.
             reason (str): Reason for post removal. Optional. 
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Post report resolved response
         """
         form = {
             "post_id": post_id,
             "mod_person_id": mod_person_id,
             "when_": when_,
             "removed": removed,
             }
         optional={
             "reason":reason,
             }
-        res = self._req.lemmyRequest("removePost", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("removePost", instance=instance, form=form, optional=optional, auth=True)
         return res["post_view"]
```

### Comparing `jplaw-0.1.5/jplaw/private_message.py` & `jplaw-0.1.6/jplaw/private_message.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,158 +5,158 @@
 from jplaw.api_paths import *
 
 
 class PrivateMessage():
     def __init__(self, _req: Requestor):
         self._req = _req
     
-    def list(self, unread_only:bool=None, page:int=None, limit:int=None, instance:str=None, auth_token:str=None):
+    def list(self, unread_only:bool=None, page:int=None, limit:int=None, instance:str=None):
         """
         Get list of private messages 
         
         Args:
             unread_only (bool): Filters private by unread. Optional.
             page (int): Page number of private messages. Optional.
             limit (int): Limit for number of private messages. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token.
+            
         Returns:
             List of private messages
         """
         form = {}
         optional={
             "unread_only": unread_only,
             "page": page,
             "limit": limit,
             }
-        res = self._req.lemmyRequest("getPrivateMessages", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("getPrivateMessages", instance=instance, form=form, optional=optional, auth=True)
         return res
-    def create(self, content:str, recipient_id:int, instance:str=None, auth_token:str=None):
+    def create(self, content:str, recipient_id:int, instance:str=None):
         """
         Create and send a private message
         
         Args:
             content (str): Contents of private message
             recipient_id (int): User ID of recipient
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token.
+            
         Returns:
             Sent private message response
         """
         form = {
             "content": content,
             "recipient_id": recipient_id,
             }
-        res = self._req.lemmyRequest("createPrivateMessage", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("createPrivateMessage", instance=instance, form=form, auth=True)
         return res
         
-    def report(self, private_message_id:int, reason:str, instance:str=None, auth_token:str=None):
+    def report(self, private_message_id:int, reason:str, instance:str=None):
         """
         Report a private message
         
         Args:
             private_message_id (int): ID of private message
             reason (str): Reason for reporting the private message
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token.
+            
         Returns:
             Sent private message response
         """
         form = {
             "private_message_id": private_message_id,
             "reason": reason,
             }
-        res = self._req.lemmyRequest("createPrivateMessageReport", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("createPrivateMessageReport", instance=instance, form=form, auth=True)
         return res
         
-    def edit(self, private_message_id:int, content:str, instance:str=None, auth_token:str=None):
+    def edit(self, private_message_id:int, content:str, instance:str=None):
         """
         Edit a private message
         
         Args:
             private_message_id (int): ID of private message
             content (str): Contents of private message
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token.
+            
         Returns:
             Private message response
         """
         form = {
             "private_message_id": private_message_id,
             "content": content,
             }
-        res = self._req.lemmyRequest("editPrivateMessage", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("editPrivateMessage", instance=instance, form=form, auth=True)
         return res
         
-    def delete(self, private_message_id:int, instance:str=None, auth_token:str=None):
+    def delete(self, private_message_id:int, instance:str=None):
         """
         Delete a private message
         
         Args:
             private_message_id (int): ID of private message
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token.
+            
         Returns:
             Private message response
         """
         form = {
             "private_message_id": private_message_id,
             }
-        res = self._req.lemmyRequest("deletePrivateMessage", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("deletePrivateMessage", instance=instance, form=form, auth=True)
         return res
         
-    def markAsRead(self, private_message_id:int, instance:str=None, auth_token:str=None):
+    def markAsRead(self, private_message_id:int, instance:str=None):
         """
         Marks a private message as read
         
         Args:
             private_message_id (int): ID of private message
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token.
+            
         Returns:
             Private message response
         """
         form={
             "private_message_id": private_message_id,
             }
-        res = self._req.lemmyRequest("markPrivateMessageAsRead", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("markPrivateMessageAsRead", instance=instance, form=form, auth=True)
         return res
         
-    def listReports(self, page:int=None, limit:int=None, unresolved_only:bool=True, instance:str=None, auth_token:str=None):
+    def listReports(self, page:int=None, limit:int=None, unresolved_only:bool=True, instance:str=None):
         """
         Gets list of private message reports
         
         Args:
             page (int): Page number
             limit (int): Limit for number of reports to get
             unresolved_only (bool): Get only unresolved posts. Default true gets only unresolved reports. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token.
+            
         Returns:
             List of private message reports
         """
         form = {}
         optional = {
             "page": page,
             "limit": limit,
             "unresolved_only": unresolved_only,
             }
-        res = self._req.lemmyRequest("listPrivateMessageReports", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("listPrivateMessageReports", instance=instance, form=form, optional=optional, auth=True)
         return res
-    def resolveReport(self, report_id:int, resolved:bool=True, instance:str=None, auth_token:str=None):
+    def resolveReport(self, report_id:int, resolved:bool=True, instance:str=None):
         """
         Resolve a private message report
         
         Args:
             report_id (int): Private message report ID
             resolved (bool): If private message report is reolved. Default true resolves report. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token.
+            
         Returns:
             Private message report resolved response
         """
         form = {
             "report_id"  : report_id ,
             "resolved"   : resolved  ,
             }
-        res = self._req.lemmyRequest("resolvePrivateMessageReport", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("resolvePrivateMessageReport", instance=instance, form=form, auth=True)
         return res
```

### Comparing `jplaw-0.1.5/jplaw/requestor.py` & `jplaw-0.1.6/jplaw/requestor.py`

 * *Files 24% similar despite different names*

```diff
@@ -62,33 +62,34 @@
             instance (str): instance to access. Default None uses logged in instance
         Returns:
             URL of api endpoint
         """
         url = instance or self.instance
         return url.rstrip("/") + API_VERSION.rstrip("/") + path
     
-    def lemmyRequest(self, function: str, instance: str = None, form: Dict[str, Any]={}, optional: Dict[str, Any]={}, auth:bool=True, auth_token:str=None) -> T:
+    def lemmyRequest(self, function: str, instance: str = None, form: Dict[str, Any]={}, optional: Dict[str, Any]={}, auth:bool=True) -> T:
         """
         Make an api request specifically to a lemmy instance for a given api function
         
         Args:
             type_ (HttpType): Type of request
             function (str): API function
             instance (str): instance to access. Default None uses logged in/default instance
             form (Dict[str,Any]): dictionary with data to send
-            auth (bool): Whether or not to authenticate. Will use auth_token if available first, then internal auth_token from login.
-            auth_token (str): authentication token
+            auth (bool): Whether or not to authenticate. Will use internal auth_token from login if available, otherwise doesn't authenticate
+            
         Returns:
             request response
         """
         form = self.AddListIfValue(optional=optional, form=form)
+        form = self.fixFormValues(form)
         
-        #if auth and token available 
-        if(auth and (auth_token or self.auth_token)):
-            form["auth"] = auth_token or self.auth_token
+        #Only authorize if authorization enabled, token is available, and instance is not changed. If instance changed or logged out, disable auth. 
+        if(auth and (self.auth_token is not None) and ((instance is None) or (instance == self.instance))):
+            form["auth"] = self.auth_token
         return self.request((API_PATH[function]["method"]), self.apiURL(instance=instance, path=(API_PATH[function]["path"])), form)
     
     def logout(self):
         """
         Logs out of instance
         """
         #TODO: send log out 
@@ -102,28 +103,69 @@
             password: password for login
             instance (str): instance to access. Default None uses logged in/default/constructor instance
         Returns:
             Access token
         """
         self.instance = instance or self.instance
         form = { "username_or_email": username, "password": password }
-        res_data = self.lemmyRequest("login", form=form, instance=instance)
+        res_data = self.lemmyRequest("login", form=form, instance=instance, auth=False)
         return res_data["jwt"]
     
-    def AddIfValue(self, name:str, value, form: Dict[str, Any]):
+    def boolToStr(self, bool_val:bool):
         """
-        Adds items to form if not None
+        Convert a boolean value to a lowercase string for request
+        
         Args:
+            bool_val (bool): boolean value to convert to string
         
         Returns:
-            Access token
+            "true" if True, "false" if false, "none" if None.
+        """
+        if(bool_val is None):
+            return "none"
+        return str(bool_val).lower() if isinstance(bool_val, bool) else bool_val
+        
+    def fixFormValues(self, form: Dict[str, Any]):
+        """
+        Fix value types for requests (e.g. bool and Enum types)
+        
+        Args:
+            form (Dict[str, Any]): Dictionary of keys and items in form
+        
+        Returns:
+            Form with fixed values
+        """
+        for key, value in form.items():
+            if(isinstance(value, bool)):
+                form[key] = self.boolToStr(value)
+            if(isinstance(value, Enum)):
+                form[key] = value.value
+        return form
+    
+    def AddIfValue(self, name:str, value: Any, form: Dict[str, Any]):
+        """
+        Adds items to form if not None
+        Args:
+            name (str): Key of item to add
+            value (Any): Value of item to add to form
+            form (Dict[str, Any]): Dictionary to add optional arguments to if not none.
+        Returns:
+            Form with optional item.
         """
         if(value is not None):
             form[name]=value
         return form
     
     def AddListIfValue(self, optional: Dict[str, Any], form: Dict[str, Any]):
+        """
+        Adds items from optional list to form if not None
+        Args:
+            optional (Dict[str, Any]): Dictionary of options with string keys and value.
+            form (Dict[str, Any]): Dictionary to add optional arguments to if not none.
+        Returns:
+            Form with optional items.
+        """
         if(optional is not None):
             for key in optional:
                 if(optional[key] is not None):
                     form[key]=optional[key]
         return form
```

### Comparing `jplaw-0.1.5/jplaw/site.py` & `jplaw-0.1.6/jplaw/site.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from .types.listing_type import ListingType
 from .types.registration_mode import RegistrationMode
 
 class Site():
     def __init__(self, _req: Requestor):
         self._req = _req
     
-    def getSite(self, instance:str=None, auth:bool=True, auth_token:str=None):
+    def getSite(self, instance:str=None, auth:bool=True):
         """
         Get the site details
         
         Args:
             instance (str): URL of local instance. Optional. Default None uses logged in instance
             auth (bool): Whether or not to authenticate. Optional. Defaults to True.
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Instance details response
         """
         form = {}
-        res = self._req.lemmyRequest("getSite", instance=instance, form=form, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("getSite", instance=instance, form=form, auth=auth)
         return res
     
     def create(self,    
         name: str,
         sidebar: str=None,
         description: str=None,
         icon: str=None,
@@ -57,23 +57,21 @@
         rate_limit_image_per_second: int=None,
         rate_limit_comment: int=None,
         rate_limit_comment_per_second: int=None,
         rate_limit_search: int=None,
         rate_limit_search_per_second: int=None,
         federation_enabled: bool=None,
         federation_debug: bool=None,
-        federation_worker_count: int=None,
         captcha_enabled: bool=None,
         captcha_difficulty: str=None,
         allowed_instances: List[str]=None,
         blocked_instances: List[str]=None,
         taglines: List[str]=None,
         registration_mode: RegistrationMode=None,
-        instance:str=None, 
-        auth_token:str=None):
+        instance:str=None):
         """
         Create the lemmy instance
         
         Args:
             name (str): Name of the website                 
             sidebar (str): Text of the sidebar of the website. Optional.
             description (str): Description of the website. Optional.
@@ -103,24 +101,23 @@
             rate_limit_image_per_second (int): Image rate limit per second. Optional.
             rate_limit_comment (int): Comment rate limit. Optional.
             rate_limit_comment_per_second (int): Comment per second rate limit. Optional.
             rate_limit_search (int): Search rate limit. Optional.
             rate_limit_search_per_second (int): Search per second rate limit. Optional.
             federation_enabled (bool): If federation is enabled. Optional.
             federation_debug (bool): If federation debugging is enabled. Optional.
-            federation_worker_count (int): Number of federation workers. This is the number of threads dedicated to federating content. Optional.
             captcha_enabled (bool): If captcha is enabled. Optional.
             captcha_difficulty (str): Difficulty of the captcha. Text: easy, medium or hard.
             allowed_instances (List[str]): List of allowed instances. Optional.
             blocked_instances (List[str]: List of blocked or defederated instances. Optional.
             taglines (List[str]: List of taglines shown at top of front page). Optional.
             registration_mode (RegistrationMode): Mode of registration (Closed/Application/Open). Optional.
             reports_email_admins (bool): if reporting emails the admins. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Create site response
         """
         form = {
             "name"                              : name                              ,
             }
         optional = {
@@ -152,23 +149,22 @@
             "rate_limit_image_per_second"       : rate_limit_image_per_second       ,
             "rate_limit_comment"                : rate_limit_comment                ,
             "rate_limit_comment_per_second"     : rate_limit_comment_per_second     ,
             "rate_limit_search"                 : rate_limit_search                 ,
             "rate_limit_search_per_second"      : rate_limit_search_per_second      ,
             "federation_enabled"                : federation_enabled                ,
             "federation_debug"                  : federation_debug                  ,
-            "federation_worker_count"           : federation_worker_count           ,
             "captcha_enabled"                   : captcha_enabled                   ,
             "captcha_difficulty"                : captcha_difficulty                ,
             "allowed_instances"                 : allowed_instances                 ,
             "blocked_instances"                 : blocked_instances                 ,
             "taglines"                          : taglines                          ,
             "registration_mode"                 : registration_mode                 ,
             }
-        res = self._req.lemmyRequest("createSite", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("createSite", instance=instance, form=form, optional=optional, auth=True)
         return res
     
     def edit(self,         
         name: str=None,
         sidebar: str=None,
         description: str=None,
         icon: str=None,
@@ -197,24 +193,22 @@
         rate_limit_image_per_second: int=None,
         rate_limit_comment: int=None,
         rate_limit_comment_per_second: int=None,
         rate_limit_search: int=None,
         rate_limit_search_per_second: int=None,
         federation_enabled: bool=None,
         federation_debug: bool=None,
-        federation_worker_count: int=None,
         captcha_enabled: bool=None,
         captcha_difficulty: str=None,
         allowed_instances: List[str]=None,
         blocked_instances: List[str]=None,
         taglines: List[str]=None,
         registration_mode: RegistrationMode=None,
         reports_email_admins:bool=None,
-        instance:str=None, 
-        auth_token:str=None):
+        instance:str=None):
         """
         Edit the site details. Optional arguments can be excluded to leave them as is.
         
         Args:
             name (str): Name of the website. Optional            
             sidebar (str): Text of the sidebar of the website. Optional.
             description (str): Description of the website. Optional.
@@ -244,24 +238,23 @@
             rate_limit_image_per_second (int): Image rate limit per second. Optional.
             rate_limit_comment (int): Comment rate limit. Optional.
             rate_limit_comment_per_second (int): Comment per second rate limit. Optional.
             rate_limit_search (int): Search rate limit. Optional.
             rate_limit_search_per_second (int): Search per second rate limit. Optional.
             federation_enabled (bool): If federation is enabled. Optional.
             federation_debug (bool): If federation debugging is enabled. Optional.
-            federation_worker_count (int): Number of federation workers. This is the number of threads dedicated to federating content. Optional.
             captcha_enabled (bool): If captcha is enabled. Optional.
             captcha_difficulty (str): Difficulty of the captcha. Text: easy, medium or hard.
             allowed_instances (List[str]): List of allowed instances. Optional.
             blocked_instances (List[str]: List of blocked or defederated instances. Optional.
             taglines (List[str]: List of taglines shown at top of front page). Optional.
             registration_mode (RegistrationMode): Mode of registration (Closed/Application/Open). Optional.
             reports_email_admins (bool): if reporting emails the admins. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Edit site response
         """
         form = {}
         optional = {
             "name"                              : name                              ,
             "sidebar"                           : sidebar                           ,
@@ -292,253 +285,252 @@
             "rate_limit_image_per_second"       : rate_limit_image_per_second       ,
             "rate_limit_comment"                : rate_limit_comment                ,
             "rate_limit_comment_per_second"     : rate_limit_comment_per_second     ,
             "rate_limit_search"                 : rate_limit_search                 ,
             "rate_limit_search_per_second"      : rate_limit_search_per_second      ,
             "federation_enabled"                : federation_enabled                ,
             "federation_debug"                  : federation_debug                  ,
-            "federation_worker_count"           : federation_worker_count           ,
             "captcha_enabled"                   : captcha_enabled                   ,
             "captcha_difficulty"                : captcha_difficulty                ,
             "allowed_instances"                 : allowed_instances                 ,
             "blocked_instances"                 : blocked_instances                 ,
             "taglines"                          : taglines                          ,
             "registration_mode"                 : registration_mode                 ,
             "reports_email_admins"              : reports_email_admins              ,
             }
-        res = self._req.lemmyRequest("editSite", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("editSite", instance=instance, form=form, optional=optional, auth=True)
         return res
         
-    def getFederatedInstances(self, instance:str=None, auth:bool=True, auth_token:str=None):
+    def getFederatedInstances(self, instance:str=None, auth:bool=True):
         """
         Get the list of federated instances from the site
         
         Args:
             instance (str): URL of local instance. Optional. Default None uses logged in instance
             auth (bool): Whether or not to use authentication. Optional. Defaults to True.
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Federated instances response
         """
-        res = self._req.lemmyRequest("getFederatedInstances", instance=instance, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("getFederatedInstances", instance=instance, auth=auth)
         return res
     
-    def addAdmin(self, person_id:int, added:bool=True, instance:str=None, auth_token:str=None):
+    def addAdmin(self, person_id:int, added:bool=True, instance:str=None):
         """
         Add an administrator to the site
         
         Args:
             person_id (int): ID of user to add as administrator
             added (bool): If person is added as an administrator to the site. Optional. Defaults to True.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Administrator added response
         """
         form={
             "person_id": person_id,
             "added": added
             }
-        res = self._req.lemmyRequest("addAdmin", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("addAdmin", instance=instance, form=form, auth=True)
         return res
         
-    def getUnreadRegistrationApplicationCount(self, instance:str=None, auth_token=None):
+    def getUnreadRegistrationApplicationCount(self, instance:str=None):
         """
         Get the number of unread registration applications
         
         Args:
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Unread registration application count response
         """
         form={}
-        res = self._req.lemmyRequest("getUnreadRegistrationApplicationCount", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("getUnreadRegistrationApplicationCount", instance=instance, form=form, auth=True)
         return res
         
-    def listRegistrationApplications(self, unread_only:bool=None, page:int=None, limit:str=None, instance:str=None, auth_token=None):
+    def listRegistrationApplications(self, unread_only:bool=None, page:int=None, limit:str=None, instance:str=None):
         """
         Get a list of registration applications
         
         Args:
             unread_only (bool): Get only unread applications. Optional.
             page (int): Page of applications to get. Optional.
             limit (int): Limit for number of applications to get. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             List of registration applications 
         """
         form={}
         optional={
             "page": page,
             "limit": limit,
             "unread_only": unread_only
             }
-        res = self._req.lemmyRequest("listRegistrationApplications", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("listRegistrationApplications", instance=instance, form=form, auth=True)
         return res
         
-    def approveRegistrationApplication(self, application_id:int, approve:bool=True, deny_reason:str=None, instance:str=None, auth_token:str=None):
+    def approveRegistrationApplication(self, application_id:int, approve:bool=True, deny_reason:str=None, instance:str=None):
         """
         Approve a registration application
         
         Args:
             application_id (int): ID of the application
             approve (bool): If registration application has been approved. Optional. Defaults to True
             dent_reason (str): Reason for denying the application, if denied. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Approved registration response
         """
         form={
             "application_id": application_id,
             "approve": approve,
             }
         optional={
             "deny_reason": deny_reason
             }
-        res = self._req.lemmyRequest("approveRegistrationApplication", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("approveRegistrationApplication", instance=instance, form=form, optional=optional, auth=True)
         return res
         
-    def getModlog(self, mod_person_id:int=None, community_id:int=None, page:int=None, limit:int=None, type_:ModlogActionType=None, other_person_id:int=None, instance:str=None, auth_token:str=None):
+    def getModlog(self, mod_person_id:int=None, community_id:int=None, page:int=None, limit:int=None, type_:ModlogActionType=None, other_person_id:int=None, instance:str=None):
         """
         Get the moderation log of the site
         
         Args:
             mod_person_id (int): Filter by moderator id. Optional
             community_id (int): Filter by community id. Optional
             page (int): Page number to view. Optional
             limit (int): Limit for number of results to get. Optional
             type_ (ModlogActionType): Filter by type of moderator action. Optional
             other_person_id (int): ID of the user who made the comment, post or community. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Moderator log response
         """
         form={}
         optional={
             "mod_person_id": mod_person_id,
             "community_id": community_id,
             "page": page,
             "limit": limit,
             "type_": type_,
             "other_person_id": other_person_id,
             }
-        res = self._req.lemmyRequest("getModlog", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("getModlog", instance=instance, form=form, optional=optional, auth=True)
         return res
         
-    def purgeComment(self, comment_id:int, reason:str=None, instance:str=None, auth_token:str=None):
+    def purgeComment(self, comment_id:int, reason:str=None, instance:str=None):
         """
         Purge a comment from the site
         
         Args:
             comment_id (int): ID of the comment to purge
             reason (str): Reason for purging the comment. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Purged comment response
         """
         form={
             "comment_id": comment_id
             }
         optional={
             "reason": reason,
             }
-        res = self._req.lemmyRequest("purgeComment", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("purgeComment", instance=instance, form=form, optional=optional, auth=True)
         return res
-    def purgeCommunity(self, community_id:int, reason:str=None, instance:str=None, auth_token:str=None):
+    def purgeCommunity(self, community_id:int, reason:str=None, instance:str=None):
         """
         Purge a community from the site
         
         Args:
             community_id (int): ID of the user to purge
             reason (str): Reason for purging the community. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Purged community response
         """
         form={
             "community_id": community_id
             }
         optional={
             "reason": reason,
             }
-        res = self._req.lemmyRequest("purgeCommunity", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("purgeCommunity", instance=instance, form=form, optional=optional, auth=True)
         return res
-    def purgePost(self, post_id:int, reason:str=None, instance:str=None, auth_token:str=None):
+    def purgePost(self, post_id:int, reason:str=None, instance:str=None):
         """
         Purge a post from the site
         
         Args:
             post_id (int): ID of the post to purge
             reason (str): Reason for purging the post. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Purged post response
         """
         form={
             "post_id": post_id
             }
         optional={
             "reason": reason,
             }
-        res = self._req.lemmyRequest("purgePost", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("purgePost", instance=instance, form=form, optional=optional, auth=True)
         return res
-    def purgePerson(self, person_id:int, reason:str=None, instance:str=None, auth_token:str=None):
+    def purgePerson(self, person_id:int, reason:str=None, instance:str=None):
         """
         Purge a person from the site
         
         Args:
             person_id (int): ID of the user to purge
             reason (str): Reason for purging the person. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Purged person response
         """
         form={
             "person_id": person_id
             }
         optional={
             "reason": reason,
             }
-        res = self._req.lemmyRequest("purgePerson", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("purgePerson", instance=instance, form=form, optional=optional, auth=True)
         return res
     
-    def resolveObject(self, obj, instance:str=None, auth_token:str=None):
+    def resolveObject(self, obj, instance:str=None):
         """
         Resolves object from another instance
         
         Args:
             obj: Object to resolve from the remote instance
             instance (str): URL of local instance to request the object from
-            auth_token (str): Authentication token for local instance
+            
         Returns:
             Federated object
         """
         form={
             "q": obj
         }
-        res = self._req.lemmyRequest("resolveObject", instance=instance, form=form, auth_token=auth_token)
+        res = self._req.lemmyRequest("resolveObject", instance=instance, form=form)
         return res
         
-    def search(self, term:str, instance:str=None, auth_token:str=None):
+    def search(self, term:str, instance:str=None):
         """
         Search for term
         
         Args:
             term (str): Object to resolve from the remote instance
             instance (str): URL of local instance. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance
+            
         Returns:
             Search results
         """
         form={
             "q": term
         }
-        res = self._req.request("search", instance=instance, auth_token=auth_token, form=form)
+        res = self._req.request("search", instance=instance, form=form)
         return res
```

### Comparing `jplaw-0.1.5/jplaw/types/modlog_action_type.py` & `jplaw-0.1.6/jplaw/types/modlog_action_type.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.5/jplaw/user.py` & `jplaw-0.1.6/jplaw/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,42 +6,52 @@
 from typing import List
 from .types.listing_type import ListingType
 from .types.sort_type import SortType
 
 class User():
     def __init__(self, _req: Requestor):
         self._req = _req
-    def leaveAdmin(self, instance:str=None, auth_token:str=None):
+    def leaveAdmin(self, instance:str=None):
         """
         Leave the administrator team of a site
         
         Args:
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Removed community response
         """
         form = {}
-        res = self._req.lemmyRequest("leaveAdmin", instance=instance, form=form, auth=True, auth_token=auth_token)
-    def register(self, username:str, password:str, password_verify:str, show_nsfw:bool, email:str=None, captcha_uuid:str=None, captcha_answer:str=None, honeypot:str=None, answer:str=None, instance:str=None):
+        res = self._req.lemmyRequest("leaveAdmin", instance=instance, form=form, auth=True)
+    def register(self, 
+        username:str, 
+        password:str, 
+        password_verify:str, 
+        show_nsfw:bool, 
+        email:str=None, 
+        captcha_uuid:str=None, 
+        captcha_answer:str=None, 
+        honeypot:str=None, 
+        answer:str=None, 
+        instance:str=None):
         """
         Register at an instance
         
         Args:
             username (str): Username to use for account
             password (str): Password for account
             password_verify (str): Password repeated for verification
             show_nsfw (bool): If NSFW posts should be shown
             email (str): Email address associated with the account. Optional
             captcha_uuid (str): UUID of the captcha. Optional. Required if site requires captcha.
             captcha_answer (str): Answer to the captcha. Optional. Required if site requires captcha.
             honeypot (str): Honeypot field. Used for detecting bots which autofill all fields. Do not use unless trying to explicitly trigger honeypot
             answer (str): Answer to sign up question
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Removed community response
         """
         form={
             "username": username,
             "password": password,
             "password_verify": password_verify,
@@ -53,257 +63,252 @@
             "captcha_uuid"   :captcha_uuid   ,
             "limit"          :limit          ,
             "honeypot"       :honeypot       ,
             "answer"         :answer         ,
             }
         res = self._req.lemmyRequest("register", instance=instance, form=form, optional=optional, auth=False)
         return res
-    def getDetails(self, person_id:str=None, username:str=None, sort:SortType=None, page:int=None, limit:int=None, community_id:int=None, saved_only:bool=None, instance:str=None, auth:bool=True, auth_token:str=None):
+    def getDetails(self, person_id:str=None, username:str=None, sort:SortType=None, page:int=None, limit:int=None, community_id:int=None, saved_only:bool=None, instance:str=None, auth:bool=True):
         """
         Get details of a user
         
         Args:
             person_id (int): User ID of the person to get the details of. Optional.
             username (str): Username of the user to get the details of. Optional
             sort (SortType): Sort order of user list. Optional
             page (int): Page number to get.
             limit (int): Limit for number of users to return
             community_id (int): Community to filter by for user
             saved_only (bool): Show only saved objects
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth (bool): If true, authenticate using auth_token or login respectively. Defaults to True.
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            auth (bool): If true, authenticate using login. Defaults to True.
+            
         Returns:
             List of items which follow the filters given
         """
         form={}
-        if(sort is not None):
-            form["sort"] = sort.value
         optional={
-            "person_id"      :person_id      ,
-            "username"       :username       ,
-            "page"           :page           ,
-            "limit"          :limit          ,
-            "community_id"   :community_id   ,
-            "saved_only"     :saved_only     ,
+            "sort"          :   sort              ,
+            "person_id"     :   person_id         ,
+            "username"      :   username          ,
+            "page"          :   page              ,
+            "limit"         :   limit             ,
+            "community_id"  :   community_id      ,
+            "saved_only"    :   saved_only        ,
             }
-        res = self._req.lemmyRequest("getPersonDetails", instance=instance, form=form, optional=optional, auth=auth, auth_token=auth_token)
+        res = self._req.lemmyRequest("getPersonDetails", instance=instance, form=form, optional=optional, auth=auth)
         return res
     
-    def markMentionAsRead(self, person_mention_id:int, read:bool=True, instance:str=None, auth_token:str=None):
+    def markMentionAsRead(self, person_mention_id:int, read:bool=True, instance:str=None):
         """
         Mark a mention as read or unread
         
         Args:
             person_mention_id (int): ID of the mention
             read (bool): If true, marks mention as read. False marks unread. Defaults to True. Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             List of items which follow the filters given
         """
         form={
             "person_mention_id": person_mention_id,
             "read": read
             }
-        res = self._req.lemmyRequest("markPersonMentionAsRead", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("markPersonMentionAsRead", instance=instance, form=form, auth=True)
         return res
     
-    def getMentions(self, sort:SortType=None, page:int=None, limit:int=None, unread_only:bool=True, instance:str=None, auth_token:str=None):
+    def getMentions(self, sort:SortType=None, page:int=None, limit:int=None, unread_only:bool=True, instance:str=None):
         """
         Get the list of mentions
         
         Args:
             sort (SortType): Sort order of mention list. Optional
             page (int): Page number to get. Optional.
             limit (int): Limit for number of mentions to return. Optional.
             unread_only (bool): Show only unread mentions. Optional. Defaults to true.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             List of mentions
         """
         form={}
-        if(sort is not None):
-            form["sort"] = sort.value
         optional = {
-            "sort"           :sort           ,
-            "page"           :page           ,
-            "limit"          :limit          ,
-            "unread_only"    :unread_only    ,
+            "sort"           :  sort           ,
+            "page"           :  page           ,
+            "limit"          :  limit          ,
+            "unread_only"    :  unread_only    ,
             }
-        res = self._req.lemmyRequest("getPersonMentions", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("getPersonMentions", instance=instance, form=form, optional=optional, auth=True)
         return res
     
-    def getReplies(self, sort:SortType=None, page:int=None, limit:int=None, unread_only:bool=True, auth_token:str=None):
+    def getReplies(self, sort:SortType=None, page:int=None, limit:int=None, unread_only:bool=True):
         """
         Get the list of replies
         
         Args:
             sort (SortType): Sort order of reply list. Optional
             page (int): Page number to get. Optional.
             limit (int): Limit for number of replies to return. Optional.
             unread_only (bool): Show only unread replies. Optional. Defaults to true.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             List of replies
         """
         form={}
-        if(sort is not None):
-            form["sort"] = sort.value
         optional = {
-            "sort"           :sort           ,
-            "page"           :page           ,
-            "limit"          :limit          ,
-            "unread_only"    :unread_only    ,
+            "sort"           :  sort           ,
+            "page"           :  page           ,
+            "limit"          :  limit          ,
+            "unread_only"    :  unread_only    ,
             }
-        res = self._req.lemmyRequest("getReplies", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("getReplies", instance=instance, form=form, optional=optional, auth=True)
         return res
     
-    def ban(self, person_id:int, ban:bool, remove_data:bool=None, reason:str=None, expires:int=None, instance:str=None, auth_token:str=None):
+    def ban(self, person_id:int, ban:bool, remove_data:bool=None, reason:str=None, expires:int=None, instance:str=None):
         """
         Ban a user from the instance
         
         Args:
             person_id (int): User ID of the person to ban
             ban (bool): If the user is banned from the instance.
             remove_data (bool): Remove the data of the user. Optional.
             expires (int): Unix Timestamp of ban expiration (seconds). Optional.
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Banned user 
         """
         form={
             "person_id"     :person_id,
             "ban"           :ban
             }
         optional = {
             "remove_data"    :remove_data   ,
             "reason"         :reason        ,
             "expires"        :expires
             }
-        res = self._req.lemmyRequest("banPerson", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("banPerson", instance=instance, form=form, optional=optional, auth=True)
         return res
     
-    def getBanned(self, instance:str=None, auth_token:str=None):
+    def getBanned(self, instance:str=None):
         """
         Get the list of banned users
         
         Args:
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             List of banned users
         """
         form={}
-        res = self._req.lemmyRequest(HttpType.GET, "getBannedPersons", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest(HttpType.GET, "getBannedPersons", instance=instance, form=form, auth=True)
         return res
      
-    def block(self, person_id:int, block:bool, instance:str=None, auth_token:str=None):
+    def block(self, person_id:int, block:bool, instance:str=None):
         """"
         Block or unblock a user
         
         Args:
             person_id (int): ID of the user to block
             block (bool): True to block user. False to unblock user. 
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Blocked user response
         """
         form={
             "person_id": person_id,
             "block": block
             }
-        res = self._req.lemmyRequest("blockPerson", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("blockPerson", instance=instance, form=form, auth=True)
         return res
     
-    def getCaptcha(self, instance:str=None, auth_token:str=None): 
+    def getCaptcha(self, instance:str=None): 
         """
         Get a new captcha from an instance
         
         Args:
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Captcha
         """
         form={}
-        res = self._req.lemmyRequest("getCaptcha", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("getCaptcha", instance=instance, form=form, auth=True)
         return res
     
-    def deleteAccount(self, password:str, instance:str=None, auth_token:str=None): 
+    def deleteAccount(self, password:str, instance:str=None): 
         """
         Delete an account
         
         Args:
             password (str): password to verify account deletion
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Deleted account response
         """
         form={
             "password": password
             }
-        res = self._req.lemmyRequest("deleteAccount", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("deleteAccount", instance=instance, form=form, auth=True)
         return res
     
-    def passwordReset(self, email:str, instance:str=None, auth_token:str=None): 
+    def passwordReset(self, email:str, instance:str=None): 
         """
         Reset an account password associated with an email
         
         Args:
             email (str): Email address an account is associated with
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Pasword reset response
         """
         form={
             "email": email
             }
-        res = self._req.lemmyRequest("passwordReset", instance=instance, form=form, auth=False, auth_token=auth_token)
+        res = self._req.lemmyRequest("passwordReset", instance=instance, form=form, auth=False)
         return res
         
-    def passwordChangeAfterReset(self, token:str, password:str, password_verify:str, instance:str=None, auth_token:str=None):
+    def passwordChangeAfterReset(self, token:str, password:str, password_verify:str, instance:str=None):
         """
         Change a password after reset request
         
         Args:
             token (str): Reset token sent to email address
             password (str): New password
             password_verify (str): New password repeated for verification
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Password reset response
         """
         form={
             "token": token,
             "password": password,
             "password_verify": password_verify
             }
-        res = self._req.lemmyRequest("passwordChangeAfterReset", instance=instance, form=form, auth=False, auth_token=auth_token)
+        res = self._req.lemmyRequest("passwordChangeAfterReset", instance=instance, form=form, auth=False)
         return res
         
-    def markAllAsRead(self, instance:str=None, auth_token:str=None):
+    def markAllAsRead(self, instance:str=None):
         """
         Mark all as read
         
         Args:
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Mark read response
         """
         form={}
-        res = self._req.lemmyRequest("markAllAsRead", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("markAllAsRead", instance=instance, form=form, auth=True)
         return res
         
     def saveUserSettings(self,
         show_nsfw: bool=None,
         show_scores: bool=None,
         theme: str=None,
         default_sort_type: SortType=None,
@@ -319,16 +324,16 @@
         send_notifications_to_email: bool=None,
         bot_account: bool=None,
         show_bot_accounts: bool=None,
         show_read_posts: bool=None, 
         show_new_post_notifs: bool=None, 
         discussion_languages: List[int]=None, 
         generate_totp_2fa: bool=None, 
-        instance:str=None,
-        auth_token:str=None):
+        open_links_in_new_tab: bool=None,
+        instance:str=None):
         """
         Save user settings to account
         
         Args:
             show_nsfw (bool): If NSFW posts and communities should be shown. Optional
             show_scores (bool) If scores should be shown. Optional
             theme (str): Site theme. Optional
@@ -343,18 +348,19 @@
             matrix_user_id (str): Matrix user ID. Optional
             show_avatars (bool): If user avatars should be shown next to names. Optional 
             send_notifications_to_email (bool): If email notifications should be sent to the user. Optional
             bot_account (bool): If this is a bot account. Optional
             show_bot_accounts (bool): If bot accounts should be hidden. Optional 
             show_read_posts (bool): If read posts should be shown or hidden . Optional
             show_new_post_notifs (bool): If new posts should send a notification. Optional
-            discussion_languages (List[int]): List of langages to show. Using undefined may cause no posts to show
-            generate_totp_2fa (bool); Use TOTP 2FA
+            discussion_languages (List[int]): List of langages to show. Using undefined may cause no posts to show. Optional
+            generate_totp_2fa (bool): Use TOTP 2FA. Optional
+            open_links_in_new_tab (bool): Open links in new tab. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             User settings saved response
         """ 
         form = {}
         optional = {
             "show_nsfw"                     : show_nsfw                  ,
             "show_scores"                   : show_scores                ,
@@ -371,74 +377,74 @@
             "show_avatars"                  : show_avatars               ,
             "send_notifications_to_email"   : send_notifications_to_email,
             "bot_account"                   : bot_account                ,
             "show_bot_accounts"             : show_bot_accounts          ,
             "show_read_posts"               : show_read_posts            ,
             "show_new_post_notifs"          : show_new_post_notifs       ,
             "discussion_languages"          : discussion_languages       ,
-            "generate_totp_2fa"             : generate_totp_2fa          
+            "generate_totp_2fa"             : generate_totp_2fa          ,
+            "open_links_in_new_tab"         : open_links_in_new_tab
             }
-        res = self._req.lemmyRequest("saveUserSettings", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("saveUserSettings", instance=instance, form=form, optional=optional, auth=True)
         return res
     def changePassword(self, 
         new_password: str,
         new_password_verify: str,
         old_password: str,
-        instance:str=None,
-        auth_token:str=None):
+        instance:str=None):
         """
         Change password
         
         Args:
             new_password (str): New password
             new_password_verify (str): New password repeated for verification
             old_password (str): Old password to verify identity
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Password changed response
         """
         form = {
             "new_password": new_password,
             "new_password_verify" : new_password_verify,
             "old_password": old_password
         }
-        res = self._req.lemmyRequest("changePassword", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("changePassword", instance=instance, form=form, auth=True)
         return res
         
-    def getReportCount(self,community_id:int=None, instance:str=None, auth_token:str=None):
+    def getReportCount(self,community_id:int=None, instance:str=None):
         """
         Get the report count
         
         Args:
             community_id (int): ID of the community. Optional
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Report count response
         """
         form={}
         optional={
             "community_id": community_id
             }
-        res = self._req.lemmyRequest("getReportCount", instance=instance, form=form, optional=optional, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("getReportCount", instance=instance, form=form, optional=optional, auth=True)
         return res
         
-    def getUnreadCount(self, instance:str=None, auth_token:str=None):
+    def getUnreadCount(self, instance:str=None):
         """
         Get the unread count
         
         Args:
             instance (str): URL of local instance. Optional. Default None uses logged in instance
-            auth_token (str): Authentication token for local instance. Optional. Default None uses logged in auth_token
+            
         Returns:
             Unread count response
         """
         form={}
-        res = self._req.lemmyRequest("getUnreadCount", instance=instance, form=form, auth=True, auth_token=auth_token)
+        res = self._req.lemmyRequest("getUnreadCount", instance=instance, form=form, auth=True)
         return res
         
     def verifyEmail(self, instance:str=None, token:str=None):
         """
         Verify an email address
         
         Args:
```

### Comparing `jplaw-0.1.5/jplaw.egg-info/PKG-INFO` & `jplaw-0.1.6/jplaw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jplaw-0.1.5/jplaw.egg-info/SOURCES.txt` & `jplaw-0.1.6/jplaw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.5/pyproject.toml` & `jplaw-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61.0", "requests >=2.6.0", "tomli>=2.0.0"]
+requires = ["setuptools>=61.0", "requests >=2.6.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jplaw"
 dynamic = ["version"]
 authors = [
   { name="Amar Persaud", email="tehspartaa@gmail.com" },
```

