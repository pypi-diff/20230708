# Comparing `tmp/pydeezer_asy-1.0.0.tar.gz` & `tmp/pydeezer_asy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeezer_asy-1.0.0.tar", last modified: Fri Jul  7 17:59:30 2023, max compression
+gzip compressed data, was "pydeezer_asy-1.1.0.tar", last modified: Sat Jul  8 13:36:59 2023, max compression
```

## Comparing `pydeezer_asy-1.0.0.tar` & `pydeezer_asy-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:59:30.741748 pydeezer_asy-1.0.0/
--rw-rw-rw-   0        0        0      230 2023-07-07 17:59:30.741748 pydeezer_asy-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 17:59:30.676898 pydeezer_asy-1.0.0/deezer_asy/
--rw-rw-rw-   0        0        0    22109 2023-07-07 17:14:44.000000 pydeezer_asy-1.0.0/deezer_asy/DeezerAsy.py
--rw-rw-rw-   0        0        0      134 2023-07-07 16:55:48.000000 pydeezer_asy-1.0.0/deezer_asy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:59:30.703508 pydeezer_asy-1.0.0/deezer_asy/constants/
--rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-1.0.0/deezer_asy/constants/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-1.0.0/deezer_asy/constants/api_methods.py
--rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-1.0.0/deezer_asy/constants/api_urls.py
--rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-1.0.0/deezer_asy/constants/image_hosts.py
--rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-1.0.0/deezer_asy/constants/networking_settings.py
--rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-1.0.0/deezer_asy/constants/search_types.py
--rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-1.0.0/deezer_asy/constants/track_formats.py
--rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-1.0.0/deezer_asy/exceptions.py
--rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-1.0.0/deezer_asy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:59:30.737754 pydeezer_asy-1.0.0/pydeezer_asy.egg-info/
--rw-rw-rw-   0        0        0      230 2023-07-07 17:59:30.000000 pydeezer_asy-1.0.0/pydeezer_asy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-07-07 17:59:30.000000 pydeezer_asy-1.0.0/pydeezer_asy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:59:30.000000 pydeezer_asy-1.0.0/pydeezer_asy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-07 17:59:30.000000 pydeezer_asy-1.0.0/pydeezer_asy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-07 17:59:30.000000 pydeezer_asy-1.0.0/pydeezer_asy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 17:59:30.742738 pydeezer_asy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      445 2023-07-07 17:59:28.000000 pydeezer_asy-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:36:59.646851 pydeezer_asy-1.1.0/
+-rw-rw-rw-   0        0        0      230 2023-07-08 13:36:59.645854 pydeezer_asy-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-08 13:36:59.578036 pydeezer_asy-1.1.0/deezer_asy/
+-rw-rw-rw-   0        0        0    29534 2023-07-08 13:36:35.000000 pydeezer_asy-1.1.0/deezer_asy/DeezerAsy.py
+-rw-rw-rw-   0        0        0      134 2023-07-07 16:55:48.000000 pydeezer_asy-1.1.0/deezer_asy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:36:59.601973 pydeezer_asy-1.1.0/deezer_asy/constants/
+-rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/api_methods.py
+-rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/api_urls.py
+-rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/image_hosts.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/networking_settings.py
+-rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/search_types.py
+-rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/track_formats.py
+-rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/exceptions.py
+-rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-1.1.0/deezer_asy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:36:59.644858 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/
+-rw-rw-rw-   0        0        0      230 2023-07-08 13:36:59.000000 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-07-08 13:36:59.000000 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:36:59.000000 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-08 13:36:59.000000 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-08 13:36:59.000000 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:36:59.647850 pydeezer_asy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      445 2023-07-08 13:36:49.000000 pydeezer_asy-1.1.0/setup.py
```

### Comparing `pydeezer_asy-1.0.0/deezer_asy/DeezerAsy.py` & `pydeezer_asy-1.1.0/deezer_asy/DeezerAsy.py`

 * *Files 14% similar despite different names*

```diff
@@ -147,15 +147,55 @@
         data = await self._legacy_api_call(method, {
             "q": query,
             "limit": limit,
             "index": index
         })
 
         return data["data"]
+    async def get_track_valid_quality(self, track):
+        """Gets the valid download qualities of the given track
 
+        Arguments:
+            track {dict} -- Track dictionary, similar to the {info} value that is returned {using get_track()}
+
+        Returns:
+            list -- List of keys of the valid qualities from the {track_formats.TRACK_FORMAT_MAP}
+        """
+
+        track = track["DATA"] if "DATA" in track else track
+
+        qualities = []
+
+        # Fixes issue #4
+        for key in [track_formats.MP3_128, track_formats.MP3_320, track_formats.FLAC]:
+            download_url = await self.get_track_download_url(
+                track, quality=key, fallback=False)
+
+
+            async with httpx.AsyncClient(headers=networking_settings.HTTP_HEADERS, cookies=self.cookies) as session:
+                res = await session.get(download_url)
+
+                if res.status_code == 200 and int(res.headers["Content-length"]) > 0:
+                    qualities.append(key)
+
+        return qualities
+    async def _select_valid_quality(self, track, quality):
+        valid_qualities = await self.get_track_valid_quality(track)
+
+        if not quality or not quality in valid_qualities:
+            default_size = int(track["FILESIZE"])
+
+            for key in track_formats.TRACK_FORMAT_MAP.keys():
+                if f"FILESIZE_{key}" in track and int(track[f"FILESIZE_{key}"]) == default_size:
+                    quality = track_formats.TRACK_FORMAT_MAP[key]
+                    break
+        else:
+            quality = track_formats.TRACK_FORMAT_MAP[quality]
+
+        return quality
     """
         ALBUM
     """
     async def get_album(self, album_id):
         """Gets the album data of the given {album_id}
 
         Arguments:
@@ -199,15 +239,193 @@
                 
                 return {
                     "image": image_bytes,
                     "size": (size, size),
                     "ext": ext,
                     "mime_type": "image/jpeg" if ext == "jpg" else "image/png"
                 }
-    
+    async def get_album_tracks(self, album_id):
+        """Gets the tracks of the given {album_id}
+
+        Arguments:
+            album_id {str} -- Album Id
+
+        Returns:
+            list -- List of tracks
+        """
+
+        data = await self._api_call(api_methods.ALBUM_TRACKS, params={
+            "ALB_ID": album_id,
+            "NB": -1
+        })
+
+        for i, track in enumerate(data["results"]["data"]):
+            track["_POSITION"] = i + 1
+
+        return data["results"]["data"]
+    async def search_albums(self, query, limit=30, index=0):
+        """Searches albums on a given query
+
+        Arguments:
+            query {str} -- Query keyword
+
+        Keyword Arguments:
+            limit {int} -- Number of results (default: {30})
+            index {int} -- Offset (default: {0})
+
+        Returns:
+            list -- List of albums
+        """
+
+        return await self._legacy_search(api_methods.SEARCH_ALBUM, query, limit=limit, index=index)
+
+    """
+        ARTIST
+    """
+    async def get_artist(self, artist_id):
+        """Gets the artist data from the given {artist_id}
+
+        Arguments:
+            artist_id {str} -- Artist Id
+
+        Returns:
+            dict -- Artist data
+        """
+
+        data = await self._api_call(api_methods.PAGE_ARTIST, params={
+            "ART_ID": artist_id,
+            "LANG": "en"
+        })
+
+        return data["results"]
+    async def get_artist_poster(self, artist, size=500, ext="jpg"):
+        """Gets the artist poster as a binary data
+
+        Arguments:
+            artist {dict} -- artist data
+
+        Keyword Arguments:
+            size {int} -- Size of the image, {size}x{size} (default: {500})
+            ext {str} -- Extension of the image, can be ('.jpg' or '.png') (default: {"jpg"})
+
+        Returns:
+            bytes -- Binary data of the image
+        """
+
+        if not "ART_PICTURE" in artist and "DATA" in artist:
+            artist = artist["DATA"]
+
+        return await self._get_poster(artist["ART_PICTURE"], size=size, ext=ext)
+    async def get_artist_discography(self, artist_id):
+        """Gets the artist's discography (tracks)
+
+        Arguments:
+            artist_id {str} -- Artist Id
+
+        Returns:
+            dict -- Artist discography data
+        """
+
+        data = await self._api_call(api_methods.ARTIST_DISCOGRAPHY, params={
+            "ART_ID": artist_id,
+            "NB": 500,
+            "NB_SONGS": -1,
+            "START": 0
+        })
+
+        return data["results"]["data"]
+    async def get_artist_top_tracks(self, artist_id):
+        """Gets the top tracks of the given artist
+
+        Arguments:
+            artist_id {str} -- Artist Id
+
+        Returns:
+            list -- List of track
+        """
+
+        data = await self._api_call(api_methods.ARTIST_TOP_TRACKS, params={
+            "ART_ID": artist_id,
+            "NB": 100
+        })
+
+        for i, track in enumerate(data["results"]["data"]):
+            track["_POSITION"] = i + 1
+
+        return data["results"]["data"]
+    async def search_artists(self, query, limit=30, index=0):
+        """Searches artists on a given query
+
+        Arguments:
+            query {str} -- Query keyword
+
+        Keyword Arguments:
+            limit {int} -- Number of tracks (default: {30})
+            index {int} -- Offset (default: {0})
+
+        Returns:
+            list -- List of artists
+        """
+
+        return await self._legacy_search(api_methods.SEARCH_ARTIST, query, limit=limit, index=index)
+
+    """
+        PLAYLIST
+    """
+    async def get_playlist(self, playlist_id):
+        """Gets the playlist data from the given playlist_id
+
+        Arguments:
+            playlist_id {str} -- Playlist Id
+
+        Returns:
+            dict -- Playlist data
+        """
+
+        data = await self._api_call(api_methods.PAGE_PLAYLIST, params={
+            "playlist_id": playlist_id,
+            "LANG": "en"
+        })
+
+        return data["results"]
+    async def get_playlist_tracks(self, playlist_id):
+        """Gets the tracks inside the playlist
+
+        Arguments:
+            playlist_id {str} -- Playlist Id
+
+        Returns:
+            list -- List of tracks
+        """
+
+        data = await self._api_call(api_methods.PLAYLIST_TRACKS, params={
+            "PLAYLIST_ID": playlist_id,
+            "NB": -1
+        })
+
+        for i, track in enumerate(data["results"]["data"]):
+            track["_POSITION"] = i + 1
+
+        return data["results"]["data"]
+    async def search_playlists(self, query, limit=30, index=0):
+        """Searches playlists on a given query
+
+        Arguments:
+            query {str} -- Query keyword
+
+        Keyword Arguments:
+            limit {int} -- Number of tracks (default: {30})
+            index {int} -- Offset (default: {0})
+
+        Returns:
+            list -- List of playlists
+        """
+
+        return await self._legacy_search(api_methods.SEARCH_PLAYLIST, query, limit=limit, index=index)
+
     """
         TRACKS
     """
     async def search_tracks(self, query, limit=30, index=0):
         """Searches tracks on a given query
 
         Arguments:
@@ -504,15 +722,37 @@
             if not lyric_check[0]:
                 asyncio.get_event_loop().run_in_executor(None, remove, lyric_check[1])
                 return (download_path)
 
             return (download_path, lyric_check[1])
 
         return (download_path)
+    async def get_tracks(self, track_ids):
+        """Gets the list of the tracks that corresponds with the given {track_ids}
+
+        Arguments:
+            track_ids {list} -- List of track id
+
+        Returns:
+            dict -- List of tracks
+        """
+
+        data = await self._api_call(api_methods.SONG_GET_LIST_DATA, params={
+            "SNG_IDS": track_ids
+        })
 
+        data = data["results"]
+        valid_ids = [str(song["SNG_ID"]) for song in data["data"]]
+
+        data["errors"] = []
+        for id in track_ids:
+            if not str(id) in valid_ids:
+                data["errors"].append(id)
+
+        return data
 
     """
         LYRIC
     """
     async def get_track_lyrics(self, track_id):
         """Gets the lyrics data of the given {track_id}
```

### Comparing `pydeezer_asy-1.0.0/deezer_asy/constants/api_methods.py` & `pydeezer_asy-1.1.0/deezer_asy/constants/api_methods.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.0.0/deezer_asy/constants/track_formats.py` & `pydeezer_asy-1.1.0/deezer_asy/constants/track_formats.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.0.0/deezer_asy/util.py` & `pydeezer_asy-1.1.0/deezer_asy/util.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.0.0/pydeezer_asy.egg-info/SOURCES.txt` & `pydeezer_asy-1.1.0/pydeezer_asy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

