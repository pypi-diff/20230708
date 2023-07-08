# Comparing `tmp/fbn-0.0.8-py3-none-any.whl.zip` & `tmp/fbn-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8373 bytes, number of entries: 12
--rw-r--r--  2.0 unx       81 b- defN 23-Jul-04 21:25 fbn/__init__.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jul-04 21:25 fbn/__main__.py
--rw-r--r--  2.0 unx     2535 b- defN 23-Jul-04 21:25 fbn/cli.py
--rw-r--r--  2.0 unx       78 b- defN 23-Jul-04 21:25 fbn/constants.py
--rw-r--r--  2.0 unx      406 b- defN 23-Jul-04 21:25 fbn/exceptions.py
--rw-r--r--  2.0 unx     6825 b- defN 23-Jul-04 21:25 fbn/fb.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-04 21:25 fbn-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     4964 b- defN 23-Jul-04 21:25 fbn-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 21:25 fbn-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-04 21:25 fbn-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Jul-04 21:25 fbn-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      873 b- defN 23-Jul-04 21:25 fbn-0.0.8.dist-info/RECORD
-12 files, 17026 bytes uncompressed, 6925 bytes compressed:  59.3%
+Zip file size: 8498 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       81 b- defN 23-Jul-08 20:25 fbn/__init__.py
+-rw-r--r--  2.0 unx       61 b- defN 23-Jul-08 20:25 fbn/__main__.py
+-rw-r--r--  2.0 unx     2686 b- defN 23-Jul-08 20:25 fbn/cli.py
+-rw-r--r--  2.0 unx       78 b- defN 23-Jul-08 20:25 fbn/constants.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jul-08 20:25 fbn/exceptions.py
+-rw-r--r--  2.0 unx     7242 b- defN 23-Jul-08 20:25 fbn/fb.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-08 20:25 fbn-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5020 b- defN 23-Jul-08 20:25 fbn-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 20:25 fbn-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-08 20:25 fbn-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-08 20:25 fbn-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      873 b- defN 23-Jul-08 20:25 fbn-0.0.9.dist-info/RECORD
+12 files, 17650 bytes uncompressed, 7050 bytes compressed:  60.1%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: fbn/exceptions.py
 Comment: 
 
 Filename: fbn/fb.py
 Comment: 
 
-Filename: fbn-0.0.8.dist-info/LICENSE
+Filename: fbn-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: fbn-0.0.8.dist-info/METADATA
+Filename: fbn-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: fbn-0.0.8.dist-info/WHEEL
+Filename: fbn-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: fbn-0.0.8.dist-info/entry_points.txt
+Filename: fbn-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: fbn-0.0.8.dist-info/top_level.txt
+Filename: fbn-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fbn-0.0.8.dist-info/RECORD
+Filename: fbn-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbn/__init__.py

```diff
@@ -1,3 +1,3 @@
 __author__ = "Visesh Prasad"
 __email__ = "visesh@live.com"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

## fbn/cli.py

```diff
@@ -80,25 +80,29 @@
     type=str,
     required=True,
     envvar="FBN_APPRISE_URL",
     show_envvar=True,
     help="The apprise URL to notify",
 )
 @click.option(
+    "--include-errors", "on_error", is_flag=True, default=False, help="Notify of errors as well."
+)
+@click.option(
     "-v", "--verbose", is_flag=True, default=False, help="Enable debug logging."
 )
 def main(
     target_id,
     username,
     password,
     cookies_file,
     user_agent,
     sample_count,
     frequency,
     apprise_url,
+    on_error,
     verbose,
 ):
     """
     Simple CLI tool to look for new posts in a Facebook group and
     then send you a notification. Public groups do not require authentication information.
 
     Example usage:
@@ -113,14 +117,15 @@
             username,
             password,
             cookies_file,
             user_agent,
             sample_count,
             frequency,
             apprise_url,
+            on_error,
             verbose,
         )
     except Exception as e:
         # all other exceptions
         click.echo(e)
```

## fbn/fb.py

```diff
@@ -2,19 +2,19 @@
 import re
 import time
 from datetime import datetime
 
 import apprise
 import schedule
 from facebook_scraper import get_posts, enable_logging, set_user_agent
-from facebook_scraper.exceptions import TemporarilyBanned, AccountDisabled
+from facebook_scraper.exceptions import AccountDisabled
 from tenacity import (
     retry,
     stop_after_attempt,
-    retry_if_exception_type,
+    retry_if_not_exception_type,
     before_log,
     after_log,
     wait_chain,
     wait_fixed,
 )
 
 from .constants import SCHEDULE_UNIT_MAP
@@ -37,17 +37,17 @@
         raise InvalidFrequencyException(
             f"The provided monitor frequency '{frequency}' is invalid."
         )
     return count, unit
 
 
 @retry(
-    retry=retry_if_exception_type(TemporarilyBanned),
+    retry=retry_if_not_exception_type(AccountDisabled),
     stop=stop_after_attempt(3),
-    wait=wait_chain(wait_fixed(600), wait_fixed(700), wait_fixed(800)),
+    wait=wait_chain(wait_fixed(600), wait_fixed(1200), wait_fixed(1800)),
     reraise=True,
     before=before_log(logger, logging.DEBUG),
     after=after_log(logger, logging.DEBUG),
 )
 def get_latest_posts(**kwargs):
     sample_count = kwargs.pop("sample_count")
     posts = {}
@@ -62,98 +62,105 @@
                 "comments": post["comments"],
                 "username": post["username"],
             }
             logger.debug(f"Obtained post {post_id}")
             if len(posts) == sample_count:
                 logger.debug(f"Stopping with {sample_count} posts...")
                 break
-    except (TemporarilyBanned, AccountDisabled) as e:
+    except Exception as e:
+        logger.debug(f"Error fetching posts : {e}")
+        if kwargs["on_error"]:
+            notify(kwargs["apprise_url"], "Error fetching posts", str(e))
         raise e
+
     return posts
 
 
 def notify(apprise_url, title, body):
     app_obj = apprise.Apprise()
     app_obj.add(apprise_url)
     app_obj.notify(
         title=title,
         body=body,
     )
 
 
-def monitor_fb(**kwargs):
+def check_fb(**kwargs):
     global current_post_set
-    apprise_url = kwargs.pop("apprise_url")
     logger.debug(f"Fetching latest posts...")
     latest_posts_info = get_latest_posts(**kwargs)
     if latest_posts_info:
         logger.debug(f"Finished fetching latest posts")
         latest_post_set = set(latest_posts_info.keys())
         if current_post_set is None:
             logger.debug(f"Updating current_post_set for the first time and exiting...")
             current_post_set = latest_post_set
         else:
             logger.debug(f"Getting new posts...")
             new_post_set = latest_post_set - current_post_set
-            if not new_post_set:
-                logger.debug(f"No new posts found. Ending...")
-                return
-            current_post_set = latest_post_set
-            logger.debug(f"Obtained {len(new_post_set)} new posts.")
-            group_name = kwargs['group']
-            # email digests
-            is_email = (
-                apprise_url.startswith("mailto://")
-                or apprise_url.startswith("mailgun://")
-                or apprise_url.startswith("sendgrid://")
-            )
-            body = f"Found at {datetime.now()}"
-            if is_email:
-                body = """
-                <!DOCTYPE html>
-                <html>
-                    <body>
-                        <div>
+            if new_post_set:
+                current_post_set = latest_post_set
+                logger.debug(f"Obtained {len(new_post_set)} new posts.")
+                group_name = kwargs["group"]
+                # email digest
+                apprise_url = kwargs["apprise_url"]
+                is_email = (
+                    apprise_url.startswith("mailto://")
+                    or apprise_url.startswith("mailgun://")
+                    or apprise_url.startswith("sendgrid://")
+                )
+                if is_email:
+                    body = """
+                    <!DOCTYPE html>
+                    <html>
+                        <body>
                             <div>
-                """
-                for new_post_id in new_post_set:
-                    post = latest_posts_info[new_post_id]
-                    logger.debug(f"Getting post '{new_post_id}' from {group_name}")
-                    body += f"""
-                                    <div style="text-align:center;">
-                                        <h3>{post["username"]}</h3>
-                                        <p style="font-size: 1.2rem;">
-                                        {post.get("text") or post.get("post_text")}
-                                        </p>
-                                        <p>{post["comments"]} comments</p>
-                                        <p>{post["likes"]} likes</p>
-                                        <a href="{post["post_url"]}">Read more</a>
-                                    </div><br><br>
+                                <div>
                     """
-                body += """
+                    for new_post_id in new_post_set:
+                        post = latest_posts_info[new_post_id]
+                        logger.debug(f"Getting post '{new_post_id}' from {group_name}")
+                        body += f"""
+                                        <div style="text-align:center;">
+                                            <h3>{post["username"]}</h3>
+                                            <p style="font-size: 1.2rem;">
+                                            {post.get("text") or post.get("post_text")}
+                                            </p>
+                                            <p>{post["comments"]} comments</p>
+                                            <p>{post["likes"]} likes</p>
+                                            <a href="{post["post_url"]}">Read more</a>
+                                        </div><br><br>
+                        """
+                    body += """
+                                </div>
                             </div>
-                        </div>
-                    </body>
-                </html>    
-                """
-            # notify
-            title = f"{len(new_post_set)} new post(s) from {group_name}"
-            logger.debug(f"Notifying user of new posts : {title}")
-            notify(apprise_url, title, body)
+                        </body>
+                    </html>    
+                    """
+                else:
+                    body = f"Found at {datetime.now()}"
+                # notify
+                title = f"{len(new_post_set)} new post(s) from {group_name}"
+                logger.debug(f"Notifying user of new posts : {title}")
+                notify(apprise_url, title, body)
+            else:
+                logger.debug(f"No new posts found. Ending...")
+            logger.debug(f"Next check at {schedule.next_run()}...")
 
 
 def check_and_notify(
     target_id,
     username,
     password,
     cookies_file,
     user_agent,
     sample_count,
     frequency,
     apprise_url,
+    on_error,
     verbose,
 ):
     if verbose:
         # fbn logging
         level = logging.DEBUG
         formatter = logging.Formatter(
             "<%(asctime)s><%(name)s><%(levelname)s> %(message)s"
@@ -176,14 +183,15 @@
     kwargs = {
         "group": target_id,
         "page_limit": None,
         "extra_info": False,
         "options": {"allow_extra_requests": False, "posts_per_page": sample_count},
         "apprise_url": apprise_url,
         "sample_count": sample_count,
+        "on_error": on_error
     }
 
     if cookies_file:
         kwargs["cookies"] = cookies_file
     else:
         if username is not None and password is not None:
             kwargs["credentials"] = (username, password)
@@ -192,16 +200,16 @@
                 "Please provide your Facebook username/password or a cookies file."
             )
 
     logger.debug("Creating schedule...")
     if frequency:
         interval, unit = parse_frequency(frequency)
         schedule_unit = SCHEDULE_UNIT_MAP[unit]
-        job = getattr(schedule.every(int(interval)), schedule_unit).do(monitor_fb, **kwargs)
+        getattr(schedule.every(int(interval)), schedule_unit).do(check_fb, **kwargs)
     else:  # randomize as the default
-        job = schedule.every(2).to(4).hours.do(monitor_fb, **kwargs)
+        schedule.every(2).to(4).hours.do(check_fb, **kwargs)
     logger.debug(f"Running once...")
     schedule.run_all()
-    logger.debug(f"Starting schedule {job}...")
+    logger.debug(f"Next check at {schedule.next_run()}...")
     while True:
         time.sleep(600)
         schedule.run_pending()
```

## Comparing `fbn-0.0.8.dist-info/LICENSE` & `fbn-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fbn-0.0.8.dist-info/METADATA` & `fbn-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool to monitor fb groups and notify
 Home-page: https://github.com/viseshrp/fbn
 Author: Visesh Prasad
 Author-email: visesh@live.com
 Maintainer: Visesh Prasad
 Maintainer-email: visesh@live.com
 License: MIT license
@@ -66,14 +66,15 @@
                               FBN_FB_PASSWORD]
   -c, --cookies-file FILE     Path to the Facebook cookies file
   -g, --user-agent TEXT       User agent to use for scraping
   -s, --sample-count INTEGER  Number of posts to sample  [default: 10]
   -e, --every TEXT            Monitor frequency
   -a, --apprise-url TEXT      The apprise URL to notify  [env var:
                               FBN_APPRISE_URL; required]
+  --include-errors            Notify of errors as well.
   -v, --verbose               Enable debug logging.
   -h, --help                  Show this message and exit.
 ```
 
 This uses [facebook-scraper](https://github.com/kevinzg/facebook-scraper) that scrapes the target group for posts.
 If the group is private, authentication is required as you must be a member,
 obviously. Auth can be passed using the CLI options or the env vars `FBN_FB_USERNAME` or `FBN_FB_PASSWORD`.
```

## Comparing `fbn-0.0.8.dist-info/RECORD` & `fbn-0.0.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-fbn/__init__.py,sha256=JnITNGDtZrAx6X75CO0Nicn_ARx8z7nKoY-MMgxnxjI,81
+fbn/__init__.py,sha256=benal5n95G40a38nSrK7oic1W0MJeYGfTpo1UnrLBiI,81
 fbn/__main__.py,sha256=MSmt_5Xg84uHqzTN38JwgseJK8rsJn_11A8WD99VtEo,61
-fbn/cli.py,sha256=qn7-ORJ76LnpSW0hubpqVcjvxyfQ94f63hn6L9f0P80,2535
+fbn/cli.py,sha256=Hg0l2gxOrO_TT_RjdjU4iQnjLcIuaXLKXM3qPYDZp3Y,2686
 fbn/constants.py,sha256=cMQzDOJVV3vm3P1UqY1DKpB5OfhLdT5fbLEM6tAu6l8,78
 fbn/exceptions.py,sha256=8yan1cmPUJEbiTW12adRoyWF48zb3L2SCKEW1trobyA,406
-fbn/fb.py,sha256=ODBE60F8wq-sGw6zqPpsdXCpCKpzQk0Y-drJtFaivRk,6825
-fbn-0.0.8.dist-info/LICENSE,sha256=25qEHPeTSJTu_3MheLT2jl_taHxPcxlaORhLfxGDbTU,1065
-fbn-0.0.8.dist-info/METADATA,sha256=1fh9Fdn43_hfvmPYg-4DU9lIS4LMUk5xsa1xQSfdIf4,4964
-fbn-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fbn-0.0.8.dist-info/entry_points.txt,sha256=PjZFFzJbekNwM2i-9gSHHb6eQsIP6NRMgcoF98ysoZM,42
-fbn-0.0.8.dist-info/top_level.txt,sha256=Cekq2PfsBF7azxMgcSBWbU_elQ_WUTGuY37h4zY5Cu8,4
-fbn-0.0.8.dist-info/RECORD,,
+fbn/fb.py,sha256=-Cwu_12Sz8ix0dsST1Ot-raNx2u5ngt13b1bJ0CjDwk,7242
+fbn-0.0.9.dist-info/LICENSE,sha256=25qEHPeTSJTu_3MheLT2jl_taHxPcxlaORhLfxGDbTU,1065
+fbn-0.0.9.dist-info/METADATA,sha256=N44MrOd5SdfNXTE7aUdPO1yWoaoN1w1fPaJv5OmyAG4,5020
+fbn-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fbn-0.0.9.dist-info/entry_points.txt,sha256=PjZFFzJbekNwM2i-9gSHHb6eQsIP6NRMgcoF98ysoZM,42
+fbn-0.0.9.dist-info/top_level.txt,sha256=Cekq2PfsBF7azxMgcSBWbU_elQ_WUTGuY37h4zY5Cu8,4
+fbn-0.0.9.dist-info/RECORD,,
```

