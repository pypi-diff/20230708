# Comparing `tmp/lyrics_transcriber-0.5.1.tar.gz` & `tmp/lyrics_transcriber-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.5.1.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.6.1.tar", max compression
```

## Comparing `lyrics_transcriber-0.5.1.tar` & `lyrics_transcriber-0.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.5.1/LICENSE
--rw-r--r--   0        0        0     3523 2023-07-03 03:34:02.162763 lyrics_transcriber-0.5.1/README.md
--rw-r--r--   0        0        0       94 2023-07-01 16:43:51.383557 lyrics_transcriber-0.5.1/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0    13003 2023-07-06 07:05:57.554203 lyrics_transcriber-0.5.1/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.5.1/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     3849 2023-07-06 06:29:00.769390 lyrics_transcriber-0.5.1/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0     1244 2023-07-06 07:06:01.865876 lyrics_transcriber-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 lyrics_transcriber-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3513 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/README.md
+-rw-r--r--   0        0        0       94 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0    13091 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     4176 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0     1244 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 lyrics_transcriber-0.6.1/PKG-INFO
```

### Comparing `lyrics_transcriber-0.5.1/LICENSE` & `lyrics_transcriber-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.5.1/README.md` & `lyrics_transcriber-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ```
 lyrics-transcriber /path/to/your/audiofile.mp3
 ```
 
 2. To specify Genius API token, song artist, and song title for auto-correction:
 
 ```
-lyrics-transcriber /path/to/your/audiofile.mp3 --genius_api_token YOUR_API_TOKEN --song_artist "Artist Name" --song_title "Song Title"
+lyrics-transcriber /path/to/your/audiofile.mp3 --genius_api_token YOUR_API_TOKEN --artist "Artist Name" --title "Song Title"
 ```
 
 ### As a Python package in your project
 
 1. Import LyricsTranscriber in your Python script:
 
 ```
```

### Comparing `lyrics_transcriber-0.5.1/lyrics_transcriber/transcriber.py` & `lyrics_transcriber-0.6.1/lyrics_transcriber/transcriber.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,40 +11,45 @@
 import syrics.api
 
 
 class LyricsTranscriber:
     def __init__(
         self,
         audio_filepath,
-        song_artist=None,
-        song_title=None,
+        artist=None,
+        title=None,
         genius_api_token=None,
         spotify_cookie=None,
         output_dir=None,
         cache_dir="/tmp/lyrics-transcriber-cache/",
         log_level=logging.DEBUG,
-        log_format="%(asctime)s - %(levelname)s - %(module)s - %(message)s",
+        log_formatter=None,
     ):
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)
+        self.log_level = log_level
+        self.log_formatter = log_formatter
 
-        log_handler = logging.StreamHandler()
-        log_formatter = logging.Formatter(log_format)
-        log_handler.setFormatter(log_formatter)
-        self.logger.addHandler(log_handler)
+        self.log_handler = logging.StreamHandler()
+
+        if self.log_formatter is None:
+            self.log_formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(module)s - %(message)s")
+
+        self.log_handler.setFormatter(self.log_formatter)
+        self.logger.addHandler(self.log_handler)
 
         self.logger.debug(f"LyricsTranscriber instantiating with input file: {audio_filepath}")
 
         self.cache_dir = cache_dir
         self.output_dir = output_dir
         self.audio_filepath = audio_filepath
 
-        self.song_artist = song_artist
-        self.song_title = song_title
-        self.song_known = self.song_artist is not None and self.song_title is not None
+        self.artist = artist
+        self.title = title
+        self.song_known = self.artist is not None and self.title is not None
 
         self.genius_api_token = os.getenv("GENIUS_API_TOKEN", default=genius_api_token)
         self.spotify_cookie = os.getenv("SPOTIFY_COOKIE_SP_DC", default=spotify_cookie)
 
         self.whisper_result_dict = None
 
         self.result_metadata = {
@@ -120,15 +125,15 @@
             f"no cached lyrics found at spotify_lyrics_cache_filepath: {spotify_lyrics_cache_filepath}, attempting to fetch from spotify"
         )
 
         spotify_lyrics_json = None
 
         try:
             spotify_client = syrics.api.Spotify(self.spotify_cookie)
-            spotify_search_query = f"{self.song_title} - {self.song_artist}"
+            spotify_search_query = f"{self.title} - {self.artist}"
             spotify_search_results = spotify_client.search(spotify_search_query, type="track", limit=5)
 
             spotify_top_result = spotify_search_results["tracks"]["items"][0]
             self.logger.debug(
                 f"spotify_top_result: {spotify_top_result['artists'][0]['name']} - {spotify_top_result['name']} ({spotify_top_result['external_urls']['spotify']})"
             )
 
@@ -159,19 +164,19 @@
 
             with open(genius_lyrics_cache_filepath, "r") as cached_lyrics:
                 self.result_metadata["genius_lyrics_filepath"] = genius_lyrics_cache_filepath
                 self.result_metadata["genius_lyrics"] = cached_lyrics
                 return cached_lyrics
 
         self.logger.debug(f"no cached lyrics found at genius_lyrics_cache_filepath: {genius_lyrics_cache_filepath}, fetching from Genius")
-        genius = lyricsgenius.Genius(self.genius_api_token)
+        genius = lyricsgenius.Genius(self.genius_api_token, verbose=(self.log_level == logging.DEBUG))
 
-        song = genius.search_song(self.song_title, self.song_artist)
+        song = genius.search_song(self.title, self.artist)
         if song is None:
-            self.logger.warning(f'Could not find lyrics on Genius for "{self.song_title}" by {self.song_artist}')
+            self.logger.warning(f'Could not find lyrics on Genius for "{self.title}" by {self.artist}')
             return
         lyrics = self.clean_genius_lyrics(song.lyrics)
 
         self.logger.debug(f"writing clean lyrics to genius_lyrics_cache_filepath: {genius_lyrics_cache_filepath}")
         with open(genius_lyrics_cache_filepath, "w") as f:
             f.write(lyrics)
 
@@ -267,17 +272,17 @@
         filename_slug = slugify.slugify(filename)
         hash_value = self.get_file_hash(self.audio_filepath)
         cache_filepath = os.path.join(self.cache_dir, filename_slug + "_" + hash_value + extension)
         self.logger.debug(f"get_cache_filepath returning cache_filepath: {cache_filepath}")
         return cache_filepath
 
     def get_song_slug(self):
-        song_artist_slug = slugify.slugify(self.song_artist)
-        song_title_slug = slugify.slugify(self.song_title)
-        return song_artist_slug + "_" + song_title_slug
+        artist_slug = slugify.slugify(self.artist)
+        title_slug = slugify.slugify(self.title)
+        return artist_slug + "_" + title_slug
 
     def get_file_hash(self, filepath):
         return hashlib.md5(open(filepath, "rb").read()).hexdigest()
 
     def create_folders(self):
         if self.cache_dir is not None:
             os.makedirs(self.cache_dir, exist_ok=True)
```

### Comparing `lyrics_transcriber-0.5.1/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.6.1/lyrics_transcriber/utils/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,85 +3,91 @@
 import logging
 import pkg_resources
 from lyrics_transcriber import LyricsTranscriber
 
 
 def main():
     logger = logging.getLogger(__name__)
-    logger.setLevel(logging.DEBUG)
-
     log_handler = logging.StreamHandler()
-    log_formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(module)s - %(message)s")
+    log_formatter = logging.Formatter(fmt="%(asctime)s.%(msecs)03d - %(levelname)s - %(module)s - %(message)s", datefmt="%Y-%m-%d %H:%M:%S")
     log_handler.setFormatter(log_formatter)
     logger.addHandler(log_handler)
 
     logger.debug("Parsing CLI args")
 
     parser = argparse.ArgumentParser(
-        description="Create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, from any input song file"
+        description="Create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, from any input song file",
+        formatter_class=lambda prog: argparse.HelpFormatter(prog, max_help_position=40),
     )
 
     parser.add_argument("audio_filepath", nargs="?", help="The audio file path to transcribe lyrics for.", default=argparse.SUPPRESS)
 
+    package_version = pkg_resources.get_distribution("lyrics-transcriber").version
+    parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {package_version}")
+    parser.add_argument("--log_level", default="INFO", help="Optional: Logging level, e.g. info, debug, warning. Default: INFO")
+
     parser.add_argument(
-        "--song_artist",
+        "--artist",
         default=None,
-        help="Optional: specify song artist for Genius lyrics lookup and auto-correction",
+        help="Optional: song artist for lyrics lookup and auto-correction",
     )
     parser.add_argument(
-        "--song_title",
+        "--title",
         default=None,
-        help="Optional: specify song title for Genius lyrics lookup and auto-correction",
+        help="Optional: song title for lyrics lookup and auto-correction",
     )
     parser.add_argument(
         "--genius_api_token",
         default=None,
-        help="Optional: specify Genius API token for lyrics lookup and auto-correction",
+        help="Optional: Genius API token for lyrics fetching. Can also be set with GENIUS_API_TOKEN env var.",
     )
     parser.add_argument(
         "--spotify_cookie",
         default=None,
-        help="Optional: specify Spotify sp_dc cookie value for lyrics lookup and auto-correction",
+        help="Optional: Spotify sp_dc cookie value for lyrics fetching. Can also be set with SPOTIFY_COOKIE_SP_DC env var.",
     )
 
-    parser.add_argument("--cache_dir", default="/tmp/lyrics-transcriber-cache/", help="Optional cache directory.")
+    parser.add_argument(
+        "--cache_dir",
+        default="/tmp/lyrics-transcriber-cache/",
+        help="Optional: directory to cache files downloaded or generated during execution",
+    )
 
     parser.add_argument(
         "--output_dir",
         default=None,
-        help="Optional directory where the resulting lyrics files will be saved. If not specified, outputs to current dir.",
+        help="Optional: directory where the output lyrics files will be saved. Default: current directory",
     )
-    parser.add_argument("--version", action="store_true", help="Show the version number and exit")
 
     args = parser.parse_args()
 
-    if args.version:
-        version = pkg_resources.get_distribution("lyrics-transcriber").version
-        print(f"lyrics-transcriber version: {version}")
-        exit(0)
+    log_level = getattr(logging, args.log_level.upper())
+    logger.setLevel(log_level)
 
     if not hasattr(args, "audio_filepath"):
         parser.print_help()
         exit(1)
 
-    if 1 <= [args.genius_api_token, args.song_title, args.song_artist].count(True) < 3:
-        print(f"To use genius lyrics auto-correction, all 3 args genius_api_token, song_artist, song_title must be provided")
+    if 1 <= [args.genius_api_token, args.title, args.artist].count(True) < 3:
+        print(f"To use genius lyrics auto-correction, all 3 args genius_api_token, artist, title must be provided")
         print(args)
         exit(1)
 
     logger.debug("Loading LyricsTranscriber class")
 
     transcriber = LyricsTranscriber(
         args.audio_filepath,
         genius_api_token=args.genius_api_token,
         spotify_cookie=args.spotify_cookie,
-        song_artist=args.song_artist,
-        song_title=args.song_title,
+        artist=args.artist,
+        title=args.title,
         output_dir=args.output_dir,
         cache_dir=args.cache_dir,
+        log_formatter=log_formatter,
+        log_level=log_level,
     )
 
     result_metadata = transcriber.generate()
 
     logger.info(f"*** Success! ***")
 
     formatted_duration = f'{int(result_metadata["song_duration"] // 60):02d}:{int(result_metadata["song_duration"] % 60):02d}'
```

### Comparing `lyrics_transcriber-0.5.1/pyproject.toml` & `lyrics_transcriber-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-transcriber"
-version = "0.5.1"
+version = "0.6.1"
 description = "Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "lyrics_transcriber" }]
 
 [tool.poetry.dependencies]
```

### Comparing `lyrics_transcriber-0.5.1/PKG-INFO` & `lyrics_transcriber-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-transcriber
-Version: 0.5.1
+Version: 0.6.1
 Summary: Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -61,15 +61,15 @@
 ```
 lyrics-transcriber /path/to/your/audiofile.mp3
 ```
 
 2. To specify Genius API token, song artist, and song title for auto-correction:
 
 ```
-lyrics-transcriber /path/to/your/audiofile.mp3 --genius_api_token YOUR_API_TOKEN --song_artist "Artist Name" --song_title "Song Title"
+lyrics-transcriber /path/to/your/audiofile.mp3 --genius_api_token YOUR_API_TOKEN --artist "Artist Name" --title "Song Title"
 ```
 
 ### As a Python package in your project
 
 1. Import LyricsTranscriber in your Python script:
 
 ```
```

