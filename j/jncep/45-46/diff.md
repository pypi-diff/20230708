# Comparing `tmp/jncep-45.tar.gz` & `tmp/jncep-46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jncep-45.tar", last modified: Tue Jun 13 22:33:02 2023, max compression
+gzip compressed data, was "dist/jncep-46.tar", last modified: Sat Jul  8 16:08:26 2023, max compression
```

## Comparing `jncep-45.tar` & `jncep-46.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:33:02.000000 jncep-45/
--rw-r--r--   0 runner    (1001) docker     (122)    37241 2023-06-13 22:33:02.000000 jncep-45/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:33:02.000000 jncep-45/jncep/
--rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-06-13 22:32:43.000000 jncep-45/jncep/jnclabs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-06-13 22:32:43.000000 jncep-45/jncep/epub.py
--rw-r--r--   0 runner    (1001) docker     (122)     2484 2023-06-13 22:32:43.000000 jncep-45/jncep/jncweb.py
--rw-r--r--   0 runner    (1001) docker     (122)     6552 2023-06-13 22:32:43.000000 jncep-45/jncep/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    20298 2023-06-13 22:32:43.000000 jncep-45/jncep/update.py
--rw-r--r--   0 runner    (1001) docker     (122)    30051 2023-06-13 22:32:43.000000 jncep-45/jncep/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-13 22:32:43.000000 jncep-45/jncep/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3990 2023-06-13 22:32:43.000000 jncep-45/jncep/trio_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-06-13 22:32:43.000000 jncep-45/jncep/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     9519 2023-06-13 22:32:43.000000 jncep-45/jncep/spec.py
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-13 22:32:43.000000 jncep-45/jncep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:33:02.000000 jncep-45/jncep/cli/
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4078 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/epub.py
--rw-r--r--   0 runner    (1001) docker     (122)     5779 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (122)     6550 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7054 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/track.py
--rw-r--r--   0 runner    (1001) docker     (122)     7771 2023-06-13 22:32:43.000000 jncep-45/jncep/track.py
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-06-13 22:32:43.000000 jncep-45/jncep/jncep.py
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-06-13 22:33:02.000000 jncep-45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-06-13 22:32:43.000000 jncep-45/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    37241 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)    31100 2023-06-13 22:32:43.000000 jncep-45/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 16:08:26.000000 jncep-46/
+-rw-r--r--   0 runner    (1001) docker     (122)    31456 2023-07-08 16:08:01.000000 jncep-46/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-08 16:08:26.000000 jncep-46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-07-08 16:08:01.000000 jncep-46/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37709 2023-07-08 16:08:26.000000 jncep-46/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 16:08:26.000000 jncep-46/jncep/
+-rw-r--r--   0 runner    (1001) docker     (122)     5283 2023-07-08 16:08:01.000000 jncep-46/jncep/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3990 2023-07-08 16:08:01.000000 jncep-46/jncep/trio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 16:08:26.000000 jncep-46/jncep/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     6550 2023-07-08 16:08:01.000000 jncep-46/jncep/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-07-08 16:08:01.000000 jncep-46/jncep/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5821 2023-07-08 16:08:01.000000 jncep-46/jncep/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7256 2023-07-08 16:08:01.000000 jncep-46/jncep/cli/track.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4078 2023-07-08 16:08:01.000000 jncep-46/jncep/cli/epub.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-08 16:08:01.000000 jncep-46/jncep/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-07-08 16:08:01.000000 jncep-46/jncep/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9519 2023-07-08 16:08:01.000000 jncep-46/jncep/spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6551 2023-07-08 16:08:01.000000 jncep-46/jncep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2484 2023-07-08 16:08:01.000000 jncep-46/jncep/jncweb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20453 2023-07-08 16:08:01.000000 jncep-46/jncep/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8337 2023-07-08 16:08:01.000000 jncep-46/jncep/track.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31097 2023-07-08 16:08:01.000000 jncep-46/jncep/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-07-08 16:08:01.000000 jncep-46/jncep/epub.py
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-08 16:08:01.000000 jncep-46/jncep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8750 2023-07-08 16:08:01.000000 jncep-46/jncep/jnclabs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-07-08 16:08:01.000000 jncep-46/jncep/jncep.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-07-08 16:08:01.000000 jncep-46/jncep/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-08 16:08:26.000000 jncep-46/jncep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-08 16:08:26.000000 jncep-46/jncep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-08 16:08:26.000000 jncep-46/jncep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-08 16:08:26.000000 jncep-46/jncep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-08 16:08:26.000000 jncep-46/jncep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    37709 2023-07-08 16:08:26.000000 jncep-46/jncep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-07-08 16:08:26.000000 jncep-46/jncep.egg-info/SOURCES.txt
```

### Comparing `jncep-45/PKG-INFO` & `jncep-46/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jncep
-Version: 45
+Version: 46
 Summary: Command-line tool to generate EPUB files for J-Novel Club pre-pub novels
 Home-page: https://github.com/gvellut/jncep
 Author: Guilhem Vellut
 Author-email: g@vellut.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/gvellut/jncep/issues
 Project-URL: Source, https://github.com/gvellut/jncep
@@ -283,14 +283,16 @@
         
         The specifig way of setting them will depend on your shell. For example, with Bash:
         
         ```console
         export JNCEP_BYVOLUME=1
         ```
         
+        The names of the environment variables are __case-sensitive__.
+        
         ### Priority order for option values
         
         The priority order for option values is as follows:
         1. If a value is passed on the command-line, it has the highest priority
         2. If no value is passed, the value is taken from an environment variable if present
         3. After that, the value is taken from the configuration file
         4. Some options have a default value defined in the code: If no value has been explicitly passed using one of the 3 methods above, that default value will be used. Some options have no default values and are instead required: If no value is passed using one of the 3 methods just described, an error will be raised.
@@ -390,15 +392,15 @@
         
         Using the `sync`subcommand, `track` will update the list of series tracked by `jncep` based on series followed on the J-Novel Club website:
         
         ```console
         jncep track sync
         ```
         
-        The `--reverse` flag can be used for the opposite: The list of series followed on the J-Novel Club website will be updated to add series that are tracked locally by the `jncep` tool. This can be useful since the Follow functionality of the website has been added just recently and the calendar of the website can be filtered with just the followed series.
+        The `--reverse` flag can be used for the opposite: The list of series followed on the J-Novel Club website will be updated to add series that are tracked locally by the `jncep` tool.
         
         By default, the `sync` subcommand doesn't do any deletion, it just adds missing entries. To make the list of tracked series and followed series identical, the `--delete` flag can be passed.
         
         ## update
         
         This command is used to generate EPUB files for newly updated series that were previously added using the `track` command. Optionally, a URL link to a part or volume or series on the J-Novel Club website can be passed, in order to only update that series.
         
@@ -430,14 +432,18 @@
                                   unlikely to be in an EPUB reader font should NOT be
                                   replaced and instead kept as is
           -t, --css FILE          Path to custom CSS file for the EPUBs [default: The
                                   CSS provided by JNCEP]
           -s, --sync              Flag to sync tracked series based on series followed
                                   on J-Novel Club and update the new ones from the
                                   beginning of the series
+          -j, --jnc-managed       Flag to indicate whether to use the series followed
+                                  on the J-Novel Club website as the tracking
+                                  reference for updating (equivalent to running 'track
+                                  sync --delete --beginning' followed by 'update')
           -w, --whole             Flag to indicate whether the whole volume should be
                                   regenerated when a new part is detected during the
                                   update
           -f, --whole-final       Flag to indicate whether an EPUB with a complete
                                   volume should also be generated when the final part
                                   of the volume is included in the update
           -e, --use-events        Flag to use the events feed to check for updates
@@ -478,21 +484,23 @@
         
         ### Configuration & environment variables
         
         Compared to the `epub` command, the `update` command understands the additional configuration options:
         - USE_EVENTS
         - WHOLE
         - WHOLE_FINAL
+        - JNC_MANAGED
         
         Since they are flags, they should have a value like `1`, `true`, `t`, `yes`, `y` or `on` (case insensitive) if set.
         
         They are also available as environment variables:
         - JNCEP_USE_EVENTS
         - JNCEP_WHOLE
         - JNCEP_WHOLE_FINAL
+        - JNCEP_JNC_MANAGED
         
         ### Automation
         
         The `update` command can be called in the background from launchd (on macOS) or a scheduled task (on Windows) or cron (on Linux) in order to regularly download new content if available and create EPUBs (for example, once a day). 
         
         There is no notification built in the `jncep update` command but the text output can be combined with other tools to make something suitable. If there are updates, the `jncep update` command outputs something like `2 series sucessfully updated!`, which can be processed by another tool do create a notification.
         
@@ -592,14 +600,20 @@
         
         The `set` subcommand can be used to set the value for a configuration option:
         
         ```console
         jncep config set EMAIL "jnclogin@aol.com"
         ```
         
+        The option names are case-insensitive so it could also be written as:
+        
+        ```console
+        jncep config set email "jnclogin@aol.com"
+        ```
+        
         This will display something like:
         
         ```console
         Option 'EMAIL' set to 'jnclogin@aol.com'
         ```
         
         The `config.ini` file will be created if needed and will contain the following line:
```

### Comparing `jncep-45/jncep/jnclabs.py` & `jncep-46/jncep/jnclabs.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 console = utils.getConsole()
 
 CDN_IMG_URL_BASE = "https://d2dq7ifhe7bu0f.cloudfront.net"
 
 LABS_API_URL_BASE = "https://labs.j-novel.club"
 LABS_API_PATH_BASE = "/app/v1"
 LABS_API_COMMON_PARAMS = {"format": "json"}
-
-LEGACY_API_URL_BASE = "https://api.j-novel.club"
-LEGACY_API_PATH_BASE = "/api"
-LEGACY_API_COMMON_HEADERS = {
+LABS_API_COMMON_HEADERS = {
     "accept": "application/json",
     "content-type": "application/json",
 }
 
 
 class InvalidCDNRequestException(Exception):
     pass
@@ -81,39 +78,46 @@
         # alway refreeze : fine in this context
         deep_freeze(cp)
         return cp
     # an image content ; won't be modifed so can be shared
     return data
 
 
+async def paginate(func, key):
+    skip = 0
+    while True:
+        page = await func(skip=skip)
+        # flatten the pages
+        for item in page[key]:
+            yield item
+
+        pagination = page.pagination
+        if pagination.lastPage:
+            break
+        skip += pagination.limit
+
+
 class JNCLabsAPI:
     def __init__(
         self,
         labs_api_connections=10,
-        legacy_api_connections=10,
         cdn_connections=20,
         jncweb_connections=10,
         labs_api_default_timeout=20,
         legacy_api_default_timeout=20,
         cdn_default_timeout=30,
         jncweb_default_timeout=20,
         connection_timeout=None,
     ):
         # connection timeout is disabled by default => no timeout waiting for a
         # connection to be available from the rate limiter
         self.labs_api_session = asks.Session(
             LABS_API_URL_BASE,
             connections=labs_api_connections,
-            headers=LEGACY_API_COMMON_HEADERS,
-        )
-
-        self.legacy_api_session = asks.Session(
-            LEGACY_API_URL_BASE,
-            connections=legacy_api_connections,
-            headers=LEGACY_API_COMMON_HEADERS,
+            headers=LABS_API_COMMON_HEADERS,
         )
 
         # CDN_IMG_URL_BASE not really necessary
         self.cdn_session = asks.Session(CDN_IMG_URL_BASE, connections=cdn_connections)
 
         self.jncweb_session = asks.Session(
             jncweb.JNC_URL_BASE, connections=jncweb_connections
@@ -158,27 +162,14 @@
     async def fetch_data(self, resource_type, slug_id, sub_resource="", skip=None):
         if sub_resource:
             sub_resource = f"/{sub_resource}"
 
         path = f"{LABS_API_PATH_BASE}/{resource_type}/{slug_id}{sub_resource}"
         return await self._fetch_resource(path, skip=skip)
 
-    async def paginate(self, func, key):
-        skip = 0
-        while True:
-            page = await func(skip=skip)
-            # flatten the pages
-            for item in page[key]:
-                yield item
-
-            pagination = page.pagination
-            if pagination.lastPage:
-                break
-            skip += pagination.limit
-
     @with_cache
     async def fetch_content(self, slug_id, content_type):
         # not LABS_API base for embed queries
         path = f"/embed/{slug_id}/{content_type}"
 
         logger.debug(f"LABS EMBED {path}")
 
@@ -186,117 +177,85 @@
         return r.text
 
     @with_cache
     async def fetch_events(self, skip=None, **params):
         path = f"{LABS_API_PATH_BASE}/events"
         return await self._fetch_resource(path, params=params, skip=skip)
 
-    async def _fetch_resource(self, path, *, params=None, skip=None):
-        logger.debug(f"LABS {path} params={params} skip={skip}")
+    @with_cache
+    async def fetch_follows(self, skip=None):
+        path = f"{LABS_API_PATH_BASE}/series"
+        body = json.dumps({"only_follows": True})
+        return await self._fetch_resource(path, "POST", body=body, skip=skip)
+
+    async def _fetch_resource(
+        self, path, verb="GET", *, params=None, body=None, skip=None
+    ):
+        logger.debug(f"LABS {verb} {path} params={params} body={body} skip={skip}")
 
         if not params:
             params = {}
 
         params.update(LABS_API_COMMON_PARAMS)
         if skip is not None:
             params.update(skip=skip)
 
-        r = await self._call_labs_api_authenticated("GET", path, params=params)
+        r = await self._call_labs_api_authenticated(
+            verb, path, params=params, body=body
+        )
 
         d = Addict(r.json())
         deep_freeze(d)
         return d
 
     async def _call_labs_api_authenticated(
-        self, method, path, headers=None, params=None, **kwargs
+        self, verb, path, *, headers=None, params=None, body=None, **kwargs
     ):
         # ~common base path + params set in caller: some calls (embed) to the Labs API
         # do not have them
         auth = {"Authorization": f"Bearer {self.token}"}
         r = await self._call_authenticated(
             self.labs_api_session,
-            method,
+            verb,
             path,
             auth,
-            headers,
-            params,
+            headers=headers,
+            params=params,
+            body=body,
             connection_timeout=self.connection_timeout,
             timeout=self.labs_api_default_timeout,
             **kwargs,
         )
 
         return r
 
-    async def _call_legacy_api_authenticated(
-        self, method, path, headers=None, params=None, **kwargs
-    ):
-        auth = {"authorization": self.token}
-        if not headers:
-            headers = LEGACY_API_COMMON_HEADERS
-        else:
-            headers = {**LEGACY_API_COMMON_HEADERS, **headers}
-
-        path = f"{LEGACY_API_PATH_BASE}{path}"
-
-        r = await self._call_authenticated(
-            self.legacy_api_session,
-            method,
-            path,
-            auth,
-            headers,
-            params,
-            connection_timeout=self.connection_timeout,
-            timeout=self.legacy_api_default_timeout,
-            **kwargs,
-        )
-
-        return r
-
     async def _call_authenticated(
-        self, session, method, path, auth, headers=None, params=None, **kwargs
+        self,
+        session,
+        verb,
+        path,
+        auth,
+        *,
+        headers=None,
+        params=None,
+        body=None,
+        **kwargs,
     ):
         if not headers:
             headers = auth
         else:
             headers = {**auth, **headers}
 
         r = await session.request(
-            method, path=path, headers=headers, params=params, **kwargs
+            verb, path=path, headers=headers, params=params, data=body, **kwargs
         )
         r.raise_for_status()
 
         return r
 
-    async def fetch_follows(self):
-        path = "/users/me"
-        # filter for only novels, exclude manga
-        qfilter = {"include": [{"serieFollows": "serie"}]}
-        payload = {"filter": json.dumps(qfilter)}
-
-        r = await self._call_legacy_api_authenticated("GET", path, params=payload)
-        r.raise_for_status()
-
-        me_data = Addict(r.json())
-        followed_series = []
-        for s in me_data.serieFollows:
-            series = s.serie
-            slug = series.titleslug
-            # the metadata is not as complete as the usual (with fetch_metadata)
-            # but it can still be useful to avoid a call later to the API
-            jnc_resource = jncweb.JNCResource(
-                jncweb.url_from_series_slug(slug),
-                slug,
-                True,
-                jncweb.RESOURCE_TYPE_SERIES,
-                series,
-            )
-            followed_series.append(jnc_resource)
-
-        return followed_series
-
     async def follow_series(self, series_id):
         await self._set_follow(series_id, True)
 
     async def unfollow_series(self, series_id):
         await self._set_follow(series_id, False)
 
     async def _set_follow(self, series_id, is_follow):
```

### Comparing `jncep-45/jncep/epub.py` & `jncep-46/jncep/epub.py`

 * *Files identical despite different names*

### Comparing `jncep-45/jncep/jncweb.py` & `jncep-46/jncep/jncweb.py`

 * *Files identical despite different names*

### Comparing `jncep-45/jncep/utils.py` & `jncep-46/jncep/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     return mod.__spec__.name
 
 
 def isoformat_with_z(d):
     # like the date format used by the JNC API
     if d.tzinfo != timezone.utc:
         # just in case but shouldn't happen : only date in UTC is used in the code
-        raise ValueError("Date not in UTC !")
+        raise ValueError("Date not in UTC!")
     return d.replace(microsecond=0).isoformat().replace("+00:00", "Z")
 
 
 def compare_date_isoformat(d1, d2):
     # convert in case ms are used
     date1 = dateutil.parser.parse(d1)
     date2 = dateutil.parser.parse(d2)
```

### Comparing `jncep-45/jncep/update.py` & `jncep-46/jncep/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,24 +316,27 @@
         # series_meta may be None if error during retrieval
         return UpdateResult(is_error=True)
 
 
 def _verify_series_needs_update_check(event_feed, series_details):
     last_check_date = dateutil.parser.parse(series_details.last_check_date)
 
-    events, has_reached_limit = event_feed
+    events, has_reached_limit, first_event_date = event_feed
 
     # shortcuts for some special cases
 
     if len(events) == 0:
         # events only contain the necessary events for dates between last_check and now:
         # no events => no update
         return False
 
-    if has_reached_limit:
+    # last_check_date is specific to the series; but event feed is checked taking into
+    # account all series so event if has_reached_limit is True, series may not need to
+    # be checked
+    if has_reached_limit and last_check_date <= first_event_date:
         # events doesn't go far enough in the past: Not possible to know for sure
         # if there are no updates
         # assumes need check
         return True
 
     series_id = series_details.series_id
 
@@ -343,17 +346,15 @@
             series = event.serie
             if series.legacyId != series_id:
                 continue
 
             launch_date = dateutil.parser.parse(event.launch)
             # <= : last_check_date is the session.now of the previous check so if
             # equal to last_check_date, already included in previous check
-            # see core.fetch_events prune
-            # TODO or do the check for dates in the future here instead of
-            # core.fetch_events
+            # see core.fetch_events request parameters
             if launch_date <= last_check_date:
                 # the events are ordered by launch desc so can never be false after
                 break
 
             # return only that there has been updates
             # the standard check for the series will be done after
             # TODO return specific parts ?
```

### Comparing `jncep-45/jncep/core.py` & `jncep-46/jncep/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 )
 
 EventFeed = namedtuple(
     "EventFeed",
     [
         "event_feed",
         "has_reached_limit",
+        "first_event_date",
     ],
 )
 
 
 class FilePathTooLongError(Exception):
     pass
 
@@ -516,15 +517,15 @@
             break
         else:
             raise jncweb.BadWebURLError(f"Incorrect URL for part: {jnc_resource.url}")
 
         return spec.IdentifierSpec(spec.PART, volume.volume_id, part.part_id)
 
 
-async def resolve_series(session, jnc_resource):
+async def resolve_series(session: JNCEPSession, jnc_resource):
     # id or slug to identify the series
     if jnc_resource.resource_type == jncweb.RESOURCE_TYPE_SERIES:
         series_slug = jnc_resource.slug
         return series_slug
     elif jnc_resource.resource_type == jncweb.RESOURCE_TYPE_VOLUME:
         if jnc_resource.is_new_website:
             series_slug, _ = jnc_resource.slug
@@ -900,16 +901,48 @@
     params = {"limit": limit, "end_date": session_now, "start_date": start_date_s}
 
     events_with_pagination = await session.api.fetch_events(**params)
 
     events = events_with_pagination.events
     pagination = events_with_pagination.pagination
     has_reached_limit = not pagination.lastPage
-    return EventFeed(events, has_reached_limit)
+    if events:
+        first_event_date = dateutil.parser.parse(events[-1].launch)
+    else:
+        # too short delay between checks => no events
+        # actual value should not matter
+        first_event_date = session.now
+    return EventFeed(events, has_reached_limit, first_event_date)
 
 
 def check_series_is_novel(series: Series):
-    if series.raw_data.type.upper() != "NOVEL":
+    if not is_novel(series.raw_data):
         raise SeriesNotANovelError(
             f"Series '[highlight]{series.raw_data.title}[/]' is not a novel "
             f"(type is '{series.raw_data.type}')"
         )
+
+
+def is_novel(raw_series):
+    return raw_series.type.upper() == "NOVEL"
+
+
+async def fetch_follows(session: JNCEPSession):
+    followed_series = []
+    async for raw_series in jnclabs.paginate(session.api.fetch_follows, "series"):
+        # ignore manga series
+        if not is_novel(raw_series):
+            continue
+
+        slug = raw_series.slug
+        # the metadata is not as complete as the usual (with fetch_meta)
+        # but it can still be useful to avoid a call later to the API
+        jnc_resource = jncweb.JNCResource(
+            jncweb.url_from_series_slug(slug),
+            slug,
+            True,
+            jncweb.RESOURCE_TYPE_SERIES,
+            raw_series,
+        )
+        followed_series.append(jnc_resource)
+
+    return followed_series
```

### Comparing `jncep-45/jncep/model.py` & `jncep-46/jncep/model.py`

 * *Files identical despite different names*

### Comparing `jncep-45/jncep/trio_utils.py` & `jncep-46/jncep/trio_utils.py`

 * *Files identical despite different names*

### Comparing `jncep-45/jncep/config.py` & `jncep-46/jncep/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,18 @@
 def unset_config_option(config, option):
     option = _validate_option(option)
     is_deleted = config.remove_option(None, option)
     return option, is_deleted
 
 
 def _validate_option(option):
+    # keys in upper case when writing
     option = option.upper()
     allowed_options = list_available_config_options().keys()
-    if option.upper() not in allowed_options:
+    if option not in allowed_options:
         raise InvalidOptionError(
             f"Option '{option}' is not valid. Valid options are: "
             f"{', '.join(allowed_options)}"
         )
     return option
 
 
@@ -153,9 +154,9 @@
         self.config_file_path.parent.mkdir(parents=True, exist_ok=True)
 
 
 class JNCEPConfigParser(ConfigParser):
     def __init__(self):
         # TOP_SECTION will be automatically created if new file
         super().__init__(default_section=TOP_SECTION, interpolation=None)
-        # will return the keys in upper case (instead of default lower)
+        # keys in upper case when reading (instead of default lower)
         self.optionxform = lambda x: x.upper()
```

### Comparing `jncep-45/jncep/spec.py` & `jncep-46/jncep/spec.py`

 * *Files identical despite different names*

### Comparing `jncep-45/jncep/cli/base.py` & `jncep-46/jncep/cli/base.py`

 * *Files identical despite different names*

### Comparing `jncep-45/jncep/cli/epub.py` & `jncep-46/jncep/cli/epub.py`

 * *Files identical despite different names*

### Comparing `jncep-45/jncep/cli/update.py` & `jncep-46/jncep/cli/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     ),
 )
 @click.option(
     "-j",
     "--jnc-managed",
     "is_jnc_managed",
     is_flag=True,
+    envvar=f"{ENVVAR_PREFIX}JNC_MANAGED",
     help=(
         "Flag to indicate whether to use the series followed on the J-Novel Club "
         "website as the tracking reference for updating (equivalent to "
         "running 'track sync --delete --beginning' followed by 'update')"
     ),
 )
 @click.option(
@@ -149,15 +150,15 @@
         track_manager = track.TrackConfigManager()
         tracked_series = track_manager.read_tracked_series()
 
         # process sync first => possibly will add new series to track
         new_synced = None
         if is_sync:
             console.status("Fetch followed series from J-Novel Club...")
-            follows = await session.api.fetch_follows()
+            follows = await core.fetch_follows(session)
             # new series will also be added to tracked_series
             new_synced, _ = await track.sync_series_forward(
                 session, follows, tracked_series, False
             )
 
             if len(new_synced) == 0:
                 console.warning(
```

### Comparing `jncep-45/jncep/cli/options.py` & `jncep-46/jncep/cli/options.py`

 * *Files identical despite different names*

### Comparing `jncep-45/jncep/cli/config.py` & `jncep-46/jncep/cli/config.py`

 * *Files identical despite different names*

### Comparing `jncep-45/jncep/cli/track.py` & `jncep-46/jncep/cli/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 @coro
 async def sync_series(email, password, is_reverse, is_delete, is_beginning):
     track_manager = track.TrackConfigManager()
     tracked_series = track_manager.read_tracked_series()
 
     async with core.JNCEPSession(email, password) as session:
         console.status("Fetch followed series from J-Novel Club...")
-        follows: List[jncweb.JNCResource] = await session.api.fetch_follows()
+        follows: List[jncweb.JNCResource] = await core.fetch_follows(session)
 
         if is_reverse:
             console.status("Sync to J-Novel Club...")
 
             new_synced, del_synced = await track.sync_series_backward(
                 session, follows, tracked_series, is_delete
             )
@@ -195,20 +195,24 @@
     track_manager = track.TrackConfigManager()
     tracked_series = track_manager.read_tracked_series()
 
     if len(tracked_series) > 0:
         console.info(f"{len(tracked_series)} series are tracked:")
         for index, (ser_url, ser_details) in enumerate(tracked_series.items()):
             details = None
-            if ser_details.part_date:
+            if ser_details.part == 0:
+                if ser_details.last_check_date == track.FROM_BEGINNING_CHECK_DATE:
+                    # added with --beginning
+                    details = "Not yet updated"
+                else:
+                    details = "No part released"
+            elif ser_details.part_date:
                 part_date = dateutil.parser.parse(ser_details.part_date)
                 part_date_formatted = part_date.strftime("%b %d, %Y")
                 details = f"{ser_details.part} [{part_date_formatted}]"
-            elif ser_details.part == 0:
-                details = "No part released"
             else:
                 details = f"{ser_details.part}"
 
             msg = f"[[yellow]{index + 1}[/]] [green]{ser_details.name}[/]"
             if is_detail:
                 msg += f" {ser_url} [red]{details}[/]"
```

### Comparing `jncep-45/jncep/track.py` & `jncep-46/jncep/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 logger = logging.getLogger(__package__)
 console = utils.getConsole()
 
 TRACK_FILE_NAME = "tracked.json"
 
 DEFAULT_CONFIG_FILEPATH = config.config_dir() / TRACK_FILE_NAME
 
+FROM_BEGINNING_CHECK_DATE = "1000-10-10T10:10:10Z"
+
 
 class TrackConfigManager:
     def __init__(self, config_file_path=None):
         if not config_file_path:
             self.config_file_path = DEFAULT_CONFIG_FILEPATH
         else:
             if config_file_path is Path:
@@ -109,23 +111,33 @@
         console.info(
             f"The series '[highlight]{series.raw_data.title}[/]' is now tracked, "
             f"starting after part [highlight]{pn} [{part_date_formatted}]"
             f"[/]",
             style="success",
         )
 
+    if is_beginning:
+        # TODO add a flag to indicate --beginning ; keep track of the last part
+        # anyway instead of the special part=0 and last_check_date in that case
+        # see also cli.track list_track_series
+        # date far in the past: used in case of --use-events => will always end up
+        # checking the full metadata of the series (as if --use-events was not used)
+        last_check_date = FROM_BEGINNING_CHECK_DATE
+    else:
+        last_check_date = utils.isoformat_with_z(session.now)
+
     series_url = jncweb.url_from_series_slug(series.raw_data.slug)
     # TODO class for trackData
     tracked_series[series_url] = Addict(
         {
             "part_date": pdate,
             "part": pn,  # now just for showing to the user in track list
             "name": series.raw_data.title,
             "series_id": series.series_id,
-            "last_check_date": utils.isoformat_with_z(session.now),
+            "last_check_date": last_check_date,
         }
     )
 
 
 async def sync_series_forward(
     session, follows, tracked_series, is_delete, is_beginning=False
 ):
@@ -176,15 +188,15 @@
     async def do_follow(jnc_resource):
         console.info(f"Fetch metadata for '{jnc_resource}'...")
         series_id = await core.resolve_series(session, jnc_resource)
         series = await core.fetch_meta(session, series_id)
         title = series.raw_data.title
 
         console.info(f"Follow '{title}'...")
-        await session.api.follow_series(series_id)
+        await session.api.follow_series(series.series_id)
 
         new_synced.append(series_url)
 
     followed_index = {f.url: f for f in follows}
     tasks = []
     for series_url in tracked_series:
         # series_url is the latest URL format (same as the follows)
@@ -193,15 +205,15 @@
         jnc_resource = jncweb.resource_from_url(series_url)
         tasks.append(partial(do_follow, jnc_resource))
 
     if is_delete:
 
         async def do_undollow(jnc_resource):
             # use the follow_raw_data: to avoid another call to the API
-            series_id = jnc_resource.follow_raw_data.id
+            series_id = jnc_resource.follow_raw_data.legacyId
             title = jnc_resource.follow_raw_data.title
             console.warning(f"Unfollow '{title}'...")
             await session.api.unfollow_series(series_id)
 
             del_synced.append(jnc_resource.url)
 
         for jnc_resource in follows:
```

### Comparing `jncep-45/jncep/jncep.py` & `jncep-46/jncep/jncep.py`

 * *Files identical despite different names*

### Comparing `jncep-45/setup.py` & `jncep-46/setup.py`

 * *Files identical despite different names*

### Comparing `jncep-45/jncep.egg-info/PKG-INFO` & `jncep-46/jncep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jncep
-Version: 45
+Version: 46
 Summary: Command-line tool to generate EPUB files for J-Novel Club pre-pub novels
 Home-page: https://github.com/gvellut/jncep
 Author: Guilhem Vellut
 Author-email: g@vellut.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/gvellut/jncep/issues
 Project-URL: Source, https://github.com/gvellut/jncep
@@ -283,14 +283,16 @@
         
         The specifig way of setting them will depend on your shell. For example, with Bash:
         
         ```console
         export JNCEP_BYVOLUME=1
         ```
         
+        The names of the environment variables are __case-sensitive__.
+        
         ### Priority order for option values
         
         The priority order for option values is as follows:
         1. If a value is passed on the command-line, it has the highest priority
         2. If no value is passed, the value is taken from an environment variable if present
         3. After that, the value is taken from the configuration file
         4. Some options have a default value defined in the code: If no value has been explicitly passed using one of the 3 methods above, that default value will be used. Some options have no default values and are instead required: If no value is passed using one of the 3 methods just described, an error will be raised.
@@ -390,15 +392,15 @@
         
         Using the `sync`subcommand, `track` will update the list of series tracked by `jncep` based on series followed on the J-Novel Club website:
         
         ```console
         jncep track sync
         ```
         
-        The `--reverse` flag can be used for the opposite: The list of series followed on the J-Novel Club website will be updated to add series that are tracked locally by the `jncep` tool. This can be useful since the Follow functionality of the website has been added just recently and the calendar of the website can be filtered with just the followed series.
+        The `--reverse` flag can be used for the opposite: The list of series followed on the J-Novel Club website will be updated to add series that are tracked locally by the `jncep` tool.
         
         By default, the `sync` subcommand doesn't do any deletion, it just adds missing entries. To make the list of tracked series and followed series identical, the `--delete` flag can be passed.
         
         ## update
         
         This command is used to generate EPUB files for newly updated series that were previously added using the `track` command. Optionally, a URL link to a part or volume or series on the J-Novel Club website can be passed, in order to only update that series.
         
@@ -430,14 +432,18 @@
                                   unlikely to be in an EPUB reader font should NOT be
                                   replaced and instead kept as is
           -t, --css FILE          Path to custom CSS file for the EPUBs [default: The
                                   CSS provided by JNCEP]
           -s, --sync              Flag to sync tracked series based on series followed
                                   on J-Novel Club and update the new ones from the
                                   beginning of the series
+          -j, --jnc-managed       Flag to indicate whether to use the series followed
+                                  on the J-Novel Club website as the tracking
+                                  reference for updating (equivalent to running 'track
+                                  sync --delete --beginning' followed by 'update')
           -w, --whole             Flag to indicate whether the whole volume should be
                                   regenerated when a new part is detected during the
                                   update
           -f, --whole-final       Flag to indicate whether an EPUB with a complete
                                   volume should also be generated when the final part
                                   of the volume is included in the update
           -e, --use-events        Flag to use the events feed to check for updates
@@ -478,21 +484,23 @@
         
         ### Configuration & environment variables
         
         Compared to the `epub` command, the `update` command understands the additional configuration options:
         - USE_EVENTS
         - WHOLE
         - WHOLE_FINAL
+        - JNC_MANAGED
         
         Since they are flags, they should have a value like `1`, `true`, `t`, `yes`, `y` or `on` (case insensitive) if set.
         
         They are also available as environment variables:
         - JNCEP_USE_EVENTS
         - JNCEP_WHOLE
         - JNCEP_WHOLE_FINAL
+        - JNCEP_JNC_MANAGED
         
         ### Automation
         
         The `update` command can be called in the background from launchd (on macOS) or a scheduled task (on Windows) or cron (on Linux) in order to regularly download new content if available and create EPUBs (for example, once a day). 
         
         There is no notification built in the `jncep update` command but the text output can be combined with other tools to make something suitable. If there are updates, the `jncep update` command outputs something like `2 series sucessfully updated!`, which can be processed by another tool do create a notification.
         
@@ -592,14 +600,20 @@
         
         The `set` subcommand can be used to set the value for a configuration option:
         
         ```console
         jncep config set EMAIL "jnclogin@aol.com"
         ```
         
+        The option names are case-insensitive so it could also be written as:
+        
+        ```console
+        jncep config set email "jnclogin@aol.com"
+        ```
+        
         This will display something like:
         
         ```console
         Option 'EMAIL' set to 'jnclogin@aol.com'
         ```
         
         The `config.ini` file will be created if needed and will contain the following line:
```

### Comparing `jncep-45/jncep.egg-info/SOURCES.txt` & `jncep-46/jncep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jncep-45/README.md` & `jncep-46/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,16 @@
 
 The specifig way of setting them will depend on your shell. For example, with Bash:
 
 ```console
 export JNCEP_BYVOLUME=1
 ```
 
+The names of the environment variables are __case-sensitive__.
+
 ### Priority order for option values
 
 The priority order for option values is as follows:
 1. If a value is passed on the command-line, it has the highest priority
 2. If no value is passed, the value is taken from an environment variable if present
 3. After that, the value is taken from the configuration file
 4. Some options have a default value defined in the code: If no value has been explicitly passed using one of the 3 methods above, that default value will be used. Some options have no default values and are instead required: If no value is passed using one of the 3 methods just described, an error will be raised.
@@ -380,15 +382,15 @@
 
 Using the `sync`subcommand, `track` will update the list of series tracked by `jncep` based on series followed on the J-Novel Club website:
 
 ```console
 jncep track sync
 ```
 
-The `--reverse` flag can be used for the opposite: The list of series followed on the J-Novel Club website will be updated to add series that are tracked locally by the `jncep` tool. This can be useful since the Follow functionality of the website has been added just recently and the calendar of the website can be filtered with just the followed series.
+The `--reverse` flag can be used for the opposite: The list of series followed on the J-Novel Club website will be updated to add series that are tracked locally by the `jncep` tool.
 
 By default, the `sync` subcommand doesn't do any deletion, it just adds missing entries. To make the list of tracked series and followed series identical, the `--delete` flag can be passed.
 
 ## update
 
 This command is used to generate EPUB files for newly updated series that were previously added using the `track` command. Optionally, a URL link to a part or volume or series on the J-Novel Club website can be passed, in order to only update that series.
 
@@ -420,14 +422,18 @@
                           unlikely to be in an EPUB reader font should NOT be
                           replaced and instead kept as is
   -t, --css FILE          Path to custom CSS file for the EPUBs [default: The
                           CSS provided by JNCEP]
   -s, --sync              Flag to sync tracked series based on series followed
                           on J-Novel Club and update the new ones from the
                           beginning of the series
+  -j, --jnc-managed       Flag to indicate whether to use the series followed
+                          on the J-Novel Club website as the tracking
+                          reference for updating (equivalent to running 'track
+                          sync --delete --beginning' followed by 'update')
   -w, --whole             Flag to indicate whether the whole volume should be
                           regenerated when a new part is detected during the
                           update
   -f, --whole-final       Flag to indicate whether an EPUB with a complete
                           volume should also be generated when the final part
                           of the volume is included in the update
   -e, --use-events        Flag to use the events feed to check for updates
@@ -468,21 +474,23 @@
 
 ### Configuration & environment variables
 
 Compared to the `epub` command, the `update` command understands the additional configuration options:
 - USE_EVENTS
 - WHOLE
 - WHOLE_FINAL
+- JNC_MANAGED
 
 Since they are flags, they should have a value like `1`, `true`, `t`, `yes`, `y` or `on` (case insensitive) if set.
 
 They are also available as environment variables:
 - JNCEP_USE_EVENTS
 - JNCEP_WHOLE
 - JNCEP_WHOLE_FINAL
+- JNCEP_JNC_MANAGED
 
 ### Automation
 
 The `update` command can be called in the background from launchd (on macOS) or a scheduled task (on Windows) or cron (on Linux) in order to regularly download new content if available and create EPUBs (for example, once a day). 
 
 There is no notification built in the `jncep update` command but the text output can be combined with other tools to make something suitable. If there are updates, the `jncep update` command outputs something like `2 series sucessfully updated!`, which can be processed by another tool do create a notification.
 
@@ -582,14 +590,20 @@
 
 The `set` subcommand can be used to set the value for a configuration option:
 
 ```console
 jncep config set EMAIL "jnclogin@aol.com"
 ```
 
+The option names are case-insensitive so it could also be written as:
+
+```console
+jncep config set email "jnclogin@aol.com"
+```
+
 This will display something like:
 
 ```console
 Option 'EMAIL' set to 'jnclogin@aol.com'
 ```
 
 The `config.ini` file will be created if needed and will contain the following line:
```

