# Comparing `tmp/shikithon-2.5.2.tar.gz` & `tmp/shikithon-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shikithon-2.5.2.tar", max compression
+gzip compressed data, was "shikithon-2.5.3.tar", max compression
```

## Comparing `shikithon-2.5.2.tar` & `shikithon-2.5.3.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0     1075 2023-06-18 07:20:26.724541 shikithon-2.5.2/LICENSE
--rw-r--r--   0        0        0    12346 2023-06-18 07:20:26.724541 shikithon-2.5.2/README.md
--rw-r--r--   0        0        0     1223 2023-06-18 07:20:26.728541 shikithon-2.5.2/pyproject.toml
--rw-r--r--   0        0        0      262 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/__init__.py
--rw-r--r--   0        0        0     3958 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/api.py
--rw-r--r--   0        0        0    22038 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/base_client.py
--rw-r--r--   0        0        0      189 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/decorators/__init__.py
--rw-r--r--   0        0        0     2074 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/decorators/exceptions_handler.py
--rw-r--r--   0        0        0     1617 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/decorators/method_endpoint.py
--rw-r--r--   0        0        0    35815 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/endpoints.py
--rw-r--r--   0        0        0     1699 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/__init__.py
--rw-r--r--   0        0        0     2707 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/anime.py
--rw-r--r--   0        0        0      897 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/club.py
--rw-r--r--   0        0        0      634 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/comment.py
--rw-r--r--   0        0        0      312 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/enhanced_enum.py
--rw-r--r--   0        0        0      291 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/favorite.py
--rw-r--r--   0        0        0      225 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/history.py
--rw-r--r--   0        0        0     1963 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/manga.py
--rw-r--r--   0        0        0      289 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/message.py
--rw-r--r--   0        0        0      470 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/person.py
--rw-r--r--   0        0        0     1524 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/ranobe.py
--rw-r--r--   0        0        0      240 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/request.py
--rw-r--r--   0        0        0      218 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/response.py
--rw-r--r--   0        0        0      247 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/review.py
--rw-r--r--   0        0        0      200 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/style.py
--rw-r--r--   0        0        0     2001 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/topic.py
--rw-r--r--   0        0        0      712 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/user_rate.py
--rw-r--r--   0        0        0      382 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/enums/video.py
--rw-r--r--   0        0        0      657 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/exceptions/__init__.py
--rw-r--r--   0        0        0      276 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/exceptions/already_running_client.py
--rw-r--r--   0        0        0      329 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/exceptions/invalid_content_type.py
--rw-r--r--   0        0        0      732 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/exceptions/missing_app_variable.py
--rw-r--r--   0        0        0      231 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/exceptions/retry_later.py
--rw-r--r--   0        0        0      358 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/exceptions/shikimori_api_response_error.py
--rw-r--r--   0        0        0      240 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/exceptions/shikithon_exception.py
--rw-r--r--   0        0        0      235 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/exceptions/store_exception.py
--rw-r--r--   0        0        0     2167 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/__init__.py
--rw-r--r--   0        0        0      233 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/abuse_response.py
--rw-r--r--   0        0        0      306 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/achievement.py
--rw-r--r--   0        0        0      193 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/activity.py
--rw-r--r--   0        0        0     1676 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/anime.py
--rw-r--r--   0        0        0      433 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/ban.py
--rw-r--r--   0        0        0      342 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/calendar_event.py
--rw-r--r--   0        0        0      855 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/character.py
--rw-r--r--   0        0        0      803 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/club.py
--rw-r--r--   0        0        0      293 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/club_image.py
--rw-r--r--   0        0        0      590 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/comment.py
--rw-r--r--   0        0        0     1579 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/constants.py
--rw-r--r--   0        0        0      210 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/created_user_image.py
--rw-r--r--   0        0        0      727 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/critique.py
--rw-r--r--   0        0        0      276 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/date.py
--rw-r--r--   0        0        0      238 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/dialog.py
--rw-r--r--   0        0        0      246 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/favourite.py
--rw-r--r--   0        0        0      455 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/favourites.py
--rw-r--r--   0        0        0      199 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/forum.py
--rw-r--r--   0        0        0      330 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/franchise_tree.py
--rw-r--r--   0        0        0      228 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/genre.py
--rw-r--r--   0        0        0      428 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/history.py
--rw-r--r--   0        0        0      197 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/image.py
--rw-r--r--   0        0        0      417 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/link.py
--rw-r--r--   0        0        0      613 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/linked_topic.py
--rw-r--r--   0        0        0      202 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/logo.py
--rw-r--r--   0        0        0     1751 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/manga.py
--rw-r--r--   0        0        0      647 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/message.py
--rw-r--r--   0        0        0     1008 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/person.py
--rw-r--r--   0        0        0      161 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/publisher.py
--rw-r--r--   0        0        0     1663 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/ranobe.py
--rw-r--r--   0        0        0      164 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/rating.py
--rw-r--r--   0        0        0      280 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/rating_list.py
--rw-r--r--   0        0        0      406 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/relation.py
--rw-r--r--   0        0        0      578 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/review.py
--rw-r--r--   0        0        0      376 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/role.py
--rw-r--r--   0        0        0      290 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/roles.py
--rw-r--r--   0        0        0      161 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/score.py
--rw-r--r--   0        0        0      244 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/score_list.py
--rw-r--r--   0        0        0      174 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/screenshot.py
--rw-r--r--   0        0        0      237 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/seyu.py
--rw-r--r--   0        0        0      860 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/stats.py
--rw-r--r--   0        0        0      209 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/status.py
--rw-r--r--   0        0        0      249 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/status_list.py
--rw-r--r--   0        0        0      252 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/studio.py
--rw-r--r--   0        0        0      500 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/style.py
--rw-r--r--   0        0        0     1600 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/topic.py
--rw-r--r--   0        0        0      255 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/tree_link.py
--rw-r--r--   0        0        0      304 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/tree_node.py
--rw-r--r--   0        0        0      158 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/type.py
--rw-r--r--   0        0        0      238 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/type_list.py
--rw-r--r--   0        0        0      247 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/unread_messages.py
--rw-r--r--   0        0        0      988 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/user.py
--rw-r--r--   0        0        0      232 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/user_image.py
--rw-r--r--   0        0        0      726 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/user_list.py
--rw-r--r--   0        0        0      543 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/user_rate.py
--rw-r--r--   0        0        0      170 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/user_rate_score.py
--rw-r--r--   0        0        0      172 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/user_rate_status.py
--rw-r--r--   0        0        0      290 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/video.py
--rw-r--r--   0        0        0      355 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/models/works.py
--rw-r--r--   0        0        0        0 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/py.typed
--rw-r--r--   0        0        0     1338 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/__init__.py
--rw-r--r--   0        0        0     4706 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/abuse_requests.py
--rw-r--r--   0        0        0     1176 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/achievements.py
--rw-r--r--   0        0        0    14269 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/animes.py
--rw-r--r--   0        0        0     1160 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/appears.py
--rw-r--r--   0        0        0     1319 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/bans.py
--rw-r--r--   0        0        0      162 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/base_resource.py
--rw-r--r--   0        0        0     1294 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/calendars.py
--rw-r--r--   0        0        0     1839 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/characters.py
--rw-r--r--   0        0        0    13716 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/clubs.py
--rw-r--r--   0        0        0     6302 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/comments.py
--rw-r--r--   0        0        0     3218 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/constants.py
--rw-r--r--   0        0        0     2440 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/dialogs.py
--rw-r--r--   0        0        0     3684 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/favorites.py
--rw-r--r--   0        0        0      912 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/forums.py
--rw-r--r--   0        0        0     1483 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/friends.py
--rw-r--r--   0        0        0      911 2023-06-18 07:20:26.728541 shikithon-2.5.2/shikithon/resources/genres.py
--rw-r--r--   0        0        0     9732 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/mangas.py
--rw-r--r--   0        0        0     6578 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/messages.py
--rw-r--r--   0        0        0     2028 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/people.py
--rw-r--r--   0        0        0      955 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/publishers.py
--rw-r--r--   0        0        0     9542 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/ranobes.py
--rw-r--r--   0        0        0     4380 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/reviews.py
--rw-r--r--   0        0        0      751 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/stats.py
--rw-r--r--   0        0        0      922 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/studios.py
--rw-r--r--   0        0        0     4153 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/styles.py
--rw-r--r--   0        0        0     9901 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/topics.py
--rw-r--r--   0        0        0     1536 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/user_images.py
--rw-r--r--   0        0        0    10959 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/user_rates.py
--rw-r--r--   0        0        0    15848 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/resources/users.py
--rw-r--r--   0        0        0      217 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/store/__init__.py
--rw-r--r--   0        0        0     4116 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/store/base.py
--rw-r--r--   0        0        0     3142 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/store/json.py
--rw-r--r--   0        0        0     4427 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/store/memory.py
--rw-r--r--   0        0        0     1189 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/store/null.py
--rw-r--r--   0        0        0       82 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/utils/__init__.py
--rw-r--r--   0        0        0    13856 2023-06-18 07:20:26.732541 shikithon-2.5.2/shikithon/utils/utils.py
--rw-r--r--   0        0        0    13438 1970-01-01 00:00:00.000000 shikithon-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-08 20:40:44.108568 shikithon-2.5.3/LICENSE
+-rw-r--r--   0        0        0    12346 2023-07-08 20:40:44.108568 shikithon-2.5.3/README.md
+-rw-r--r--   0        0        0     1222 2023-07-08 20:40:44.108568 shikithon-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/__init__.py
+-rw-r--r--   0        0        0     3958 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/api.py
+-rw-r--r--   0        0        0    22038 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/base_client.py
+-rw-r--r--   0        0        0      189 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/decorators/__init__.py
+-rw-r--r--   0        0        0     2074 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/decorators/exceptions_handler.py
+-rw-r--r--   0        0        0     1617 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/decorators/method_endpoint.py
+-rw-r--r--   0        0        0    35815 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/endpoints.py
+-rw-r--r--   0        0        0     1699 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/__init__.py
+-rw-r--r--   0        0        0     2707 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/anime.py
+-rw-r--r--   0        0        0      897 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/club.py
+-rw-r--r--   0        0        0      634 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/comment.py
+-rw-r--r--   0        0        0      312 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/enhanced_enum.py
+-rw-r--r--   0        0        0      291 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/favorite.py
+-rw-r--r--   0        0        0      225 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/history.py
+-rw-r--r--   0        0        0     1963 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/manga.py
+-rw-r--r--   0        0        0      289 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/message.py
+-rw-r--r--   0        0        0      470 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/person.py
+-rw-r--r--   0        0        0     1524 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/ranobe.py
+-rw-r--r--   0        0        0      240 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/request.py
+-rw-r--r--   0        0        0      218 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/response.py
+-rw-r--r--   0        0        0      247 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/review.py
+-rw-r--r--   0        0        0      200 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/style.py
+-rw-r--r--   0        0        0     2001 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/topic.py
+-rw-r--r--   0        0        0      712 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/user_rate.py
+-rw-r--r--   0        0        0      382 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/enums/video.py
+-rw-r--r--   0        0        0      657 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/exceptions/__init__.py
+-rw-r--r--   0        0        0      276 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/exceptions/already_running_client.py
+-rw-r--r--   0        0        0      329 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/exceptions/invalid_content_type.py
+-rw-r--r--   0        0        0      732 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/exceptions/missing_app_variable.py
+-rw-r--r--   0        0        0      231 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/exceptions/retry_later.py
+-rw-r--r--   0        0        0      358 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/exceptions/shikimori_api_response_error.py
+-rw-r--r--   0        0        0      240 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/exceptions/shikithon_exception.py
+-rw-r--r--   0        0        0      235 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/exceptions/store_exception.py
+-rw-r--r--   0        0        0     2167 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/abuse_response.py
+-rw-r--r--   0        0        0      306 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/achievement.py
+-rw-r--r--   0        0        0      193 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/activity.py
+-rw-r--r--   0        0        0     1753 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/anime.py
+-rw-r--r--   0        0        0      440 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/ban.py
+-rw-r--r--   0        0        0      349 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/calendar_event.py
+-rw-r--r--   0        0        0      883 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/character.py
+-rw-r--r--   0        0        0      817 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/club.py
+-rw-r--r--   0        0        0      300 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/club_image.py
+-rw-r--r--   0        0        0      590 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/comment.py
+-rw-r--r--   0        0        0     1579 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/constants.py
+-rw-r--r--   0        0        0      210 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/created_user_image.py
+-rw-r--r--   0        0        0      769 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/critique.py
+-rw-r--r--   0        0        0      297 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/date.py
+-rw-r--r--   0        0        0      238 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/dialog.py
+-rw-r--r--   0        0        0      253 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/favourite.py
+-rw-r--r--   0        0        0      455 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/favourites.py
+-rw-r--r--   0        0        0      199 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/forum.py
+-rw-r--r--   0        0        0      330 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/franchise_tree.py
+-rw-r--r--   0        0        0      296 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/genre.py
+-rw-r--r--   0        0        0      435 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/history.py
+-rw-r--r--   0        0        0      197 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/image.py
+-rw-r--r--   0        0        0      445 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/link.py
+-rw-r--r--   0        0        0      690 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/linked_topic.py
+-rw-r--r--   0        0        0      202 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/logo.py
+-rw-r--r--   0        0        0     1798 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/manga.py
+-rw-r--r--   0        0        0      668 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/message.py
+-rw-r--r--   0        0        0     1022 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/person.py
+-rw-r--r--   0        0        0      161 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/publisher.py
+-rw-r--r--   0        0        0     1710 2023-07-08 20:40:44.108568 shikithon-2.5.3/shikithon/models/ranobe.py
+-rw-r--r--   0        0        0      164 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/rating.py
+-rw-r--r--   0        0        0      294 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/rating_list.py
+-rw-r--r--   0        0        0      420 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/relation.py
+-rw-r--r--   0        0        0      599 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/review.py
+-rw-r--r--   0        0        0      390 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/role.py
+-rw-r--r--   0        0        0      290 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/roles.py
+-rw-r--r--   0        0        0      161 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/score.py
+-rw-r--r--   0        0        0      244 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/score_list.py
+-rw-r--r--   0        0        0      174 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/screenshot.py
+-rw-r--r--   0        0        0      237 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/seyu.py
+-rw-r--r--   0        0        0      930 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/stats.py
+-rw-r--r--   0        0        0      209 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/status.py
+-rw-r--r--   0        0        0      249 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/status_list.py
+-rw-r--r--   0        0        0      259 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/studio.py
+-rw-r--r--   0        0        0      542 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/style.py
+-rw-r--r--   0        0        0     1656 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/topic.py
+-rw-r--r--   0        0        0      255 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/tree_link.py
+-rw-r--r--   0        0        0      318 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/tree_node.py
+-rw-r--r--   0        0        0      158 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/type.py
+-rw-r--r--   0        0        0      238 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/type_list.py
+-rw-r--r--   0        0        0      247 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/unread_messages.py
+-rw-r--r--   0        0        0     1039 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/user.py
+-rw-r--r--   0        0        0      232 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/user_image.py
+-rw-r--r--   0        0        0      768 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/user_list.py
+-rw-r--r--   0        0        0      592 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/user_rate.py
+-rw-r--r--   0        0        0      170 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/user_rate_score.py
+-rw-r--r--   0        0        0      172 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/user_rate_status.py
+-rw-r--r--   0        0        0      297 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/video.py
+-rw-r--r--   0        0        0      369 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/models/works.py
+-rw-r--r--   0        0        0        0 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/py.typed
+-rw-r--r--   0        0        0     1338 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/__init__.py
+-rw-r--r--   0        0        0     4706 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/abuse_requests.py
+-rw-r--r--   0        0        0     1176 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/achievements.py
+-rw-r--r--   0        0        0    14269 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/animes.py
+-rw-r--r--   0        0        0     1160 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/appears.py
+-rw-r--r--   0        0        0     1319 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/bans.py
+-rw-r--r--   0        0        0      162 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/base_resource.py
+-rw-r--r--   0        0        0     1294 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/calendars.py
+-rw-r--r--   0        0        0     1839 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/characters.py
+-rw-r--r--   0        0        0    13716 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/clubs.py
+-rw-r--r--   0        0        0     6302 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/comments.py
+-rw-r--r--   0        0        0     3218 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/constants.py
+-rw-r--r--   0        0        0     2440 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/dialogs.py
+-rw-r--r--   0        0        0     3684 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/favorites.py
+-rw-r--r--   0        0        0      912 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/forums.py
+-rw-r--r--   0        0        0     1483 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/friends.py
+-rw-r--r--   0        0        0      911 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/genres.py
+-rw-r--r--   0        0        0     9732 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/mangas.py
+-rw-r--r--   0        0        0     6578 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/messages.py
+-rw-r--r--   0        0        0     2028 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/people.py
+-rw-r--r--   0        0        0      955 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/publishers.py
+-rw-r--r--   0        0        0     9542 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/ranobes.py
+-rw-r--r--   0        0        0     4380 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/reviews.py
+-rw-r--r--   0        0        0      751 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/stats.py
+-rw-r--r--   0        0        0      922 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/studios.py
+-rw-r--r--   0        0        0     4153 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/styles.py
+-rw-r--r--   0        0        0     9901 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/topics.py
+-rw-r--r--   0        0        0     1536 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/user_images.py
+-rw-r--r--   0        0        0    10959 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/user_rates.py
+-rw-r--r--   0        0        0    15848 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/resources/users.py
+-rw-r--r--   0        0        0      217 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/store/__init__.py
+-rw-r--r--   0        0        0     4116 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/store/base.py
+-rw-r--r--   0        0        0     3142 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/store/json.py
+-rw-r--r--   0        0        0     4427 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/store/memory.py
+-rw-r--r--   0        0        0     1189 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/store/null.py
+-rw-r--r--   0        0        0       82 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/utils/__init__.py
+-rw-r--r--   0        0        0    13912 2023-07-08 20:40:44.112568 shikithon-2.5.3/shikithon/utils/utils.py
+-rw-r--r--   0        0        0    13437 1970-01-01 00:00:00.000000 shikithon-2.5.3/PKG-INFO
```

### Comparing `shikithon-2.5.2/LICENSE` & `shikithon-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/README.md` & `shikithon-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/pyproject.toml` & `shikithon-2.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shikithon"
-version = "2.5.2"
+version = "2.5.3"
 description = "Yet another Python wrapper for Shikimori API"
 authors = [
     "SecondThundeR <awayfromgalaxy@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/SecondThundeR/shikithon"
@@ -32,22 +32,22 @@
 warn_redundant_casts = true
 plugins = [
     "pydantic.mypy"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.10"
-pydantic = "^1.10.9"
+pydantic = "^2.0.2"
 loguru = "^0.7.0"
 validators = "^0.20.0"
 aiohttp = "^3.8.4"
 pyrate-limiter = "^2.10.0"
 backoff = "^2.2.1"
-typing-extensions = "^4.6.3"
+typing-extensions = "^4.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
-mypy = "^1.3.0"
+mypy = "^1.4.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shikithon-2.5.2/shikithon/api.py` & `shikithon-2.5.3/shikithon/api.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/base_client.py` & `shikithon-2.5.3/shikithon/base_client.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/decorators/exceptions_handler.py` & `shikithon-2.5.3/shikithon/decorators/exceptions_handler.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/decorators/method_endpoint.py` & `shikithon-2.5.3/shikithon/decorators/method_endpoint.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/endpoints.py` & `shikithon-2.5.3/shikithon/endpoints.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/enums/__init__.py` & `shikithon-2.5.3/shikithon/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/enums/anime.py` & `shikithon-2.5.3/shikithon/enums/anime.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/enums/club.py` & `shikithon-2.5.3/shikithon/enums/club.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/enums/comment.py` & `shikithon-2.5.3/shikithon/enums/comment.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/enums/manga.py` & `shikithon-2.5.3/shikithon/enums/manga.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/enums/ranobe.py` & `shikithon-2.5.3/shikithon/enums/ranobe.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/enums/topic.py` & `shikithon-2.5.3/shikithon/enums/topic.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/enums/user_rate.py` & `shikithon-2.5.3/shikithon/enums/user_rate.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/exceptions/__init__.py` & `shikithon-2.5.3/shikithon/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/exceptions/missing_app_variable.py` & `shikithon-2.5.3/shikithon/exceptions/missing_app_variable.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/models/__init__.py` & `shikithon-2.5.3/shikithon/models/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/models/anime.py` & `shikithon-2.5.3/shikithon/models/ranobe.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,65 @@
-"""Model for `/api/animes`."""
-from datetime import date, datetime
+"""Model for `/api/ranobe`."""
+from datetime import date
 from typing import List, Optional
 
-from pydantic import BaseModel
+from pydantic import BaseModel, field_validator
 
 from .genre import Genre
 from .image import Image
-from .screenshot import Screenshot
-from .studio import Studio
+from .publisher import Publisher
 from .user_rate import UserRate
 from .user_rate_score import UserRateScore
 from .user_rate_status import UserRateStatus
-from .video import Video
 
 
-class AnimeInfo(BaseModel):
-    """Represents an anime info entity."""
+class RanobeInfo(BaseModel):
+    """Represents ranobe info entity."""
     id: int
     name: str
     russian: str
     image: Image
     url: str
-    kind: Optional[str]
+    kind: str
     score: float
     status: str
-    episodes: int
-    episodes_aired: int
-    aired_on: Optional[date]
-    released_on: Optional[date]
+    volumes: int
+    chapters: int
+    aired_on: Optional[date] = None
+    released_on: Optional[date] = None
+
+    @field_validator('kind')
+    def kind_validator(cls, v):
+        if 'novel' not in v:
+            raise ValueError(f'Invalid kind. Got "{v}"'
+                             f' but expected kind, containing "novel"')
+        return v
 
 
-class Anime(AnimeInfo):
-    """Represents an anime entity."""
-    rating: str
+class Ranobe(RanobeInfo):
+    """Represents ranobe entity."""
     english: List[Optional[str]]
     japanese: List[Optional[str]]
     synonyms: List[str]
-    license_name_ru: Optional[str]
-    duration: int
-    description: Optional[str]
+    license_name_ru: Optional[str] = None
+    description: Optional[str] = None
     description_html: str
-    description_source: Optional[str]
-    franchise: Optional[str]
+    description_source: Optional[str] = None
+    franchise: Optional[str] = None
     favoured: bool
     anons: bool
     ongoing: bool
-    thread_id: Optional[int]
-    topic_id: Optional[int]
+    thread_id: Optional[int] = None
+    topic_id: Optional[int] = None
     myanimelist_id: int
     rates_scores_stats: List[UserRateScore]
     rates_statuses_stats: List[UserRateStatus]
-    updated_at: datetime
-    next_episode_at: Optional[datetime]
-    fansubbers: List[str]
-    fandubbers: List[str]
     licensors: List[str]
     genres: List[Genre]
-    studios: List[Studio]
-    videos: List[Video]
-    screenshots: List[Screenshot]
-    user_rate: Optional[UserRate]
+    publishers: List[Publisher]
+    user_rate: Optional[UserRate] = None
 
 
-class CharacterAnime(AnimeInfo):
-    """Represents a character anime info entity."""
+class CharacterRanobe(RanobeInfo):
+    """Represents a character ranobe info entity."""
     roles: List[str]
     role: str
```

### Comparing `shikithon-2.5.2/shikithon/models/character.py` & `shikithon-2.5.3/shikithon/models/character.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     url: str
 
 
 class Character(CharacterInfo):
     """Represents character entity."""
     altname: str
     japanese: str
-    description: Optional[str]
+    description: Optional[str] = None
     description_html: str
-    description_source: Optional[str]
+    description_source: Optional[str] = None
     favoured: bool
-    thread_id: Optional[int]
-    topic_id: Optional[int]
+    thread_id: Optional[int] = None
+    topic_id: Optional[int] = None
     updated_at: datetime
     seyu: List[Seyu]
     animes: List[CharacterAnime]
     mangas: List[Union[CharacterManga, CharacterRanobe]]
```

### Comparing `shikithon-2.5.2/shikithon/models/club.py` & `shikithon-2.5.3/shikithon/models/club.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     is_censored: bool
     join_policy: str
     comment_policy: str
 
 
 class Club(ClubInfo):
     """Represents a club entity."""
-    description: Optional[str]
+    description: Optional[str] = None
     description_html: str
     mangas: List[MangaInfo]
     characters: List[CharacterInfo]
     thread_id: int
     topic_id: int
-    user_role: Optional[str]
+    user_role: Optional[str] = None
     style_id: int
     members: List[UserInfo]
     animes: List[AnimeInfo]
     images: List[ClubImage]
```

### Comparing `shikithon-2.5.2/shikithon/models/comment.py` & `shikithon-2.5.3/shikithon/models/comment.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/models/constants.py` & `shikithon-2.5.3/shikithon/models/constants.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/models/critique.py` & `shikithon-2.5.3/shikithon/models/user_list.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""Submodel for `topic.py`."""
+"""Model for `/api/users/:id/anime_rates|manga_rates`."""
 from datetime import datetime
 from typing import Optional, Union
 
 from pydantic import BaseModel
 
 from .anime import AnimeInfo
 from .manga import MangaInfo
 from .ranobe import RanobeInfo
 from .user import UserInfo
 
 
-class Critique(BaseModel):
-    """Represents critique entity.
+class UserList(BaseModel):
+    """Represents user list entity.
 
-    Can be found in topics with type
-    `Topics::EntryTopics::CritiqueTopic`
+    Contains data of watched/read titles.
     """
     id: int
-    target: Optional[Union[AnimeInfo, MangaInfo, RanobeInfo]]
-    user: UserInfo
-    votes_count: int
-    votes_for: int
-    body: str
-    html_body: str
-    overall: Optional[int]
-    storyline: Optional[int]
-    music: Optional[int]
-    characters: Optional[int]
-    animation: Optional[int]
+    score: int
+    status: str
+    text: Optional[str] = None
+    episodes: Optional[int] = None
+    chapters: Optional[int] = None
+    volumes: Optional[int] = None
+    text_html: str
+    rewatches: int
     created_at: datetime
+    updated_at: datetime
+    user: UserInfo
+    anime: Optional[AnimeInfo] = None
+    manga: Optional[Union[MangaInfo, RanobeInfo]] = None
```

### Comparing `shikithon-2.5.2/shikithon/models/manga.py` & `shikithon-2.5.3/shikithon/models/manga.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Model for `/api/mangas`."""
 from datetime import date
 from typing import List, Optional
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 
 from .genre import Genre
 from .image import Image
 from .publisher import Publisher
 from .user_rate import UserRate
 from .user_rate_score import UserRateScore
 from .user_rate_status import UserRateStatus
@@ -28,47 +28,46 @@
     image: Image
     url: str
     kind: str
     score: float
     status: str
     volumes: int
     chapters: int
-    aired_on: Optional[date]
-    released_on: Optional[date]
+    aired_on: Optional[date] = None
+    released_on: Optional[date] = None
 
-    # pylint: disable=E0213
-    @validator('kind')
+    @field_validator('kind')
     def kind_validator(cls, v):
         if v not in MANGAS_KIND:
             raise ValueError(f'Invalid manga kind. Got "{v}"'
                              f' but expected one of {MANGAS_KIND}')
         return v
 
 
 class Manga(MangaInfo):
     """Represents manga entity."""
     english: List[Optional[str]]
     japanese: List[Optional[str]]
     synonyms: List[str]
-    license_name_ru: Optional[str]
-    description: Optional[str]
+    license_name_ru: Optional[str] = None
+    description: Optional[str] = None
     description_html: str
-    description_source: Optional[str]
-    franchise: Optional[str]
+    description_source: Optional[str] = None
+    franchise: Optional[str] = None
     favoured: bool
     anons: bool
     ongoing: bool
-    thread_id: Optional[int]
-    topic_id: Optional[int]
+    thread_id: Optional[int] = None
+    topic_id: Optional[int] = None
     myanimelist_id: int
     rates_scores_stats: List[UserRateScore]
     rates_statuses_stats: List[UserRateStatus]
     licensors: List[str]
     genres: List[Genre]
     publishers: List[Publisher]
-    user_rate: Optional[UserRate]
+    user_rate: Optional[UserRate] = None
 
 
 class CharacterManga(MangaInfo):
     """Represents a character manga info entity."""
     roles: List[str]
     role: str
```

### Comparing `shikithon-2.5.2/shikithon/models/message.py` & `shikithon-2.5.3/shikithon/models/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 
 class MessageInfo(BaseModel):
     """Represents message info entity."""
     id: int
     kind: str
     read: bool
-    body: Optional[str]
+    body: Optional[str] = None
     html_body: str
     created_at: datetime
     linked_id: int
-    linked_type: Optional[str]
-    linked: Optional[LinkedTopic]
+    linked_type: Optional[str] = None
+    linked: Optional[LinkedTopic] = None
 
 
 class Message(MessageInfo):
     """Represents message entity."""
     from_user: UserInfo = Field(alias='from')
     to_user: UserInfo = Field(alias='to')
```

### Comparing `shikithon-2.5.2/shikithon/models/person.py` & `shikithon-2.5.3/shikithon/models/person.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     job_title: str
     birth_on: Date
     deceased_on: Date
     website: str
     groupped_roles: List[Tuple[str, int]]
     roles: List[Roles]
     works: List[Works]
-    topic_id: Optional[int]
+    topic_id: Optional[int] = None
     person_favoured: bool
     producer: bool
     producer_favoured: bool
     mangaka: bool
     mangaka_favoured: bool
     seyu: bool
     seyu_favoured: bool
     updated_at: datetime
-    thread_id: Optional[int]
+    thread_id: Optional[int] = None
     # ? Seems like it's gonna be removed soon
     # because of birth_on and deceased_on fields
     birthday: Date
```

### Comparing `shikithon-2.5.2/shikithon/models/review.py` & `shikithon-2.5.3/shikithon/models/review.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from pydantic import BaseModel
 
 
 class Review(BaseModel):
     """Represents review entity."""
     id: int
     user_id: int
-    anime_id: Optional[int]
-    manga_id: Optional[int]
+    anime_id: Optional[int] = None
+    manga_id: Optional[int] = None
     body: str
     opinion: Union[Literal['positive'], Literal['neutral'], Literal['negative']]
     is_written_before_release: bool
     created_at: datetime
     updated_at: datetime
     comments_count: int
     cached_votes_up: int
     cached_votes_down: int
-    changed_at: Optional[datetime]
+    changed_at: Optional[datetime] = None
```

### Comparing `shikithon-2.5.2/shikithon/models/topic.py` & `shikithon-2.5.3/shikithon/models/topic.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,25 +34,25 @@
     html_body: str
     html_footer: str
     created_at: datetime
     comments_count: int
     forum: Forum
     user: UserInfo
     type: str
-    linked_id: Optional[int]
-    linked_type: Optional[str]
+    linked_id: Optional[int] = None
+    linked_type: Optional[str] = None
     linked: Optional[Union[AnimeInfo, MangaInfo, RanobeInfo, ClubInfo,
-                           CharacterInfo, Critique]]
+                           CharacterInfo, Critique]] = None
     viewed: bool
-    last_comment_viewed: Optional[bool]
-    event: Optional[str]
-    episode: Optional[int]
+    last_comment_viewed: Optional[bool] = None
+    event: Optional[str] = None
+    episode: Optional[int] = None
 
 
 class TopicUpdate(BaseModel):
     """Represents topic update entity."""
     id: int
     linked: Union[AnimeInfo, MangaInfo, RanobeInfo]
-    event: Optional[str]
-    episode: Optional[int]
+    event: Optional[str] = None
+    episode: Optional[int] = None
     created_at: datetime
     url: str
```

### Comparing `shikithon-2.5.2/shikithon/models/user_rate.py` & `shikithon-2.5.3/shikithon/models/user_rate.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from pydantic import BaseModel
 
 
 class UserRate(BaseModel):
     """Represents user rate entity."""
     id: int
-    user_id: Optional[int]
-    target_id: Optional[int]
-    target_type: Optional[str]
+    user_id: Optional[int] = None
+    target_id: Optional[int] = None
+    target_type: Optional[str] = None
     score: int
     status: str
-    text: Optional[str]
-    episodes: Optional[int]
-    chapters: Optional[int]
-    volumes: Optional[int]
+    text: Optional[str] = None
+    episodes: Optional[int] = None
+    chapters: Optional[int] = None
+    volumes: Optional[int] = None
     text_html: str
     rewatches: int
     created_at: datetime
     updated_at: datetime
```

### Comparing `shikithon-2.5.2/shikithon/resources/__init__.py` & `shikithon-2.5.3/shikithon/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/abuse_requests.py` & `shikithon-2.5.3/shikithon/resources/abuse_requests.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/achievements.py` & `shikithon-2.5.3/shikithon/resources/achievements.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/animes.py` & `shikithon-2.5.3/shikithon/resources/animes.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/appears.py` & `shikithon-2.5.3/shikithon/resources/appears.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/bans.py` & `shikithon-2.5.3/shikithon/resources/bans.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/calendars.py` & `shikithon-2.5.3/shikithon/resources/calendars.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/characters.py` & `shikithon-2.5.3/shikithon/resources/characters.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/clubs.py` & `shikithon-2.5.3/shikithon/resources/clubs.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/comments.py` & `shikithon-2.5.3/shikithon/resources/comments.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/constants.py` & `shikithon-2.5.3/shikithon/resources/constants.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/dialogs.py` & `shikithon-2.5.3/shikithon/resources/dialogs.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/favorites.py` & `shikithon-2.5.3/shikithon/resources/favorites.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/forums.py` & `shikithon-2.5.3/shikithon/resources/forums.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/friends.py` & `shikithon-2.5.3/shikithon/resources/friends.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/genres.py` & `shikithon-2.5.3/shikithon/resources/genres.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/mangas.py` & `shikithon-2.5.3/shikithon/resources/mangas.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/messages.py` & `shikithon-2.5.3/shikithon/resources/messages.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/people.py` & `shikithon-2.5.3/shikithon/resources/people.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/publishers.py` & `shikithon-2.5.3/shikithon/resources/publishers.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/ranobes.py` & `shikithon-2.5.3/shikithon/resources/ranobes.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/reviews.py` & `shikithon-2.5.3/shikithon/resources/reviews.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/stats.py` & `shikithon-2.5.3/shikithon/resources/stats.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/studios.py` & `shikithon-2.5.3/shikithon/resources/studios.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/styles.py` & `shikithon-2.5.3/shikithon/resources/styles.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/topics.py` & `shikithon-2.5.3/shikithon/resources/topics.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/user_images.py` & `shikithon-2.5.3/shikithon/resources/user_images.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/user_rates.py` & `shikithon-2.5.3/shikithon/resources/user_rates.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/resources/users.py` & `shikithon-2.5.3/shikithon/resources/users.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/store/base.py` & `shikithon-2.5.3/shikithon/store/base.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/store/json.py` & `shikithon-2.5.3/shikithon/store/json.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/store/memory.py` & `shikithon-2.5.3/shikithon/store/memory.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/store/null.py` & `shikithon-2.5.3/shikithon/store/null.py`

 * *Files identical despite different names*

### Comparing `shikithon-2.5.2/shikithon/utils/utils.py` & `shikithon-2.5.3/shikithon/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 import imghdr
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union, overload
 
 from aiohttp import ClientResponse, ClientSession, FormData
 from loguru import logger
-from pydantic import BaseModel, parse_obj_as
+from pydantic import BaseModel, TypeAdapter
 from validators import url
 
 from ..enums import ResponseCode
 
 LOWER_LIMIT_NUMBER = 1
 CENSORED_FIELDS = (
     'access_token',
@@ -311,15 +311,16 @@
         :type parse_type: Type[T]
 
         :return: Parsed response to passed type
         :rtype: T
         """
         logger.info('Parsing response with mixed models')
         logger.info(f'Parsing using type: {parse_type}')
-        return parse_obj_as(parse_type, response)
+        adapter: TypeAdapter[T] = TypeAdapter(parse_type)
+        return adapter.validate_python(response)
 
     @staticmethod
     def create_form_data(raw_data: Dict[str, Any]):
         """Creates form data for API request.
 
         Method converts dictionary with data to
         FormData object for API request
```

### Comparing `shikithon-2.5.2/PKG-INFO` & `shikithon-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shikithon
-Version: 2.5.2
+Version: 2.5.3
 Summary: Yet another Python wrapper for Shikimori API
 Home-page: https://github.com/SecondThundeR/shikithon
 License: MIT
 Keywords: Python,Shikimori,API
 Author: SecondThundeR
 Author-email: awayfromgalaxy@gmail.com
 Requires-Python: >=3.8.10,<4.0.0
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: pyrate-limiter (>=2.10.0,<3.0.0)
-Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Project-URL: Documentation, https://github.com/SecondThundeR/shikithon/README.md
 Project-URL: Repository, https://github.com/SecondThundeR/shikithon
 Description-Content-Type: text/markdown
 
 <!-- If PyCharm or IDEA will throw a warning here, just ignore it -->
 <div align="center">
```

