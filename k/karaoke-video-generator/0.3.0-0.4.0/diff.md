# Comparing `tmp/karaoke_video_generator-0.3.0.tar.gz` & `tmp/karaoke_video_generator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karaoke_video_generator-0.3.0.tar", max compression
+gzip compressed data, was "karaoke_video_generator-0.4.0.tar", max compression
```

## Comparing `karaoke_video_generator-0.3.0.tar` & `karaoke_video_generator-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2249 2023-06-30 19:16:34.212627 karaoke_video_generator-0.3.0/README.md
--rw-r--r--   0        0        0       40 2023-06-30 19:30:35.364926 karaoke_video_generator-0.3.0/karaoke_generator/__init__.py
--rw-r--r--   0        0        0    14003 2023-07-06 08:29:39.771816 karaoke_video_generator-0.3.0/karaoke_generator/generator.py
--rw-r--r--   0        0        0        0 2023-06-30 19:27:00.420507 karaoke_video_generator-0.3.0/karaoke_generator/utils/__init__.py
--rwxr-xr-x   0        0        0     3105 2023-07-06 08:30:54.011714 karaoke_video_generator-0.3.0/karaoke_generator/utils/cli.py
--rw-r--r--   0        0        0      806 2023-07-06 08:31:58.509271 karaoke_video_generator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3083 1970-01-01 00:00:00.000000 karaoke_video_generator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2249 2023-07-08 03:39:31.294419 karaoke_video_generator-0.4.0/README.md
+-rw-r--r--   0        0        0       40 2023-07-08 03:39:31.294419 karaoke_video_generator-0.4.0/karaoke_generator/__init__.py
+-rw-r--r--   0        0        0    14395 2023-07-08 03:39:31.294419 karaoke_video_generator-0.4.0/karaoke_generator/generator.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:39:31.294419 karaoke_video_generator-0.4.0/karaoke_generator/utils/__init__.py
+-rwxr-xr-x   0        0        0     3477 2023-07-08 03:39:31.294419 karaoke_video_generator-0.4.0/karaoke_generator/utils/cli.py
+-rw-r--r--   0        0        0     1296 2023-07-08 03:39:31.294419 karaoke_video_generator-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3083 1970-01-01 00:00:00.000000 karaoke_video_generator-0.4.0/PKG-INFO
```

### Comparing `karaoke_video_generator-0.3.0/README.md` & `karaoke_video_generator-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `karaoke_video_generator-0.3.0/karaoke_generator/generator.py` & `karaoke_video_generator-0.4.0/karaoke_generator/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,68 +12,75 @@
 from audio_separator import Separator
 from lyrics_transcriber import LyricsTranscriber
 
 
 class KaraokeGenerator:
     def __init__(
         self,
-        youtube_url=None,
-        audio_file=None,
-        song_artist=None,
-        song_title=None,
+        log_level=logging.DEBUG,
+        log_formatter=None,
+        input_path=None,
+        artist=None,
+        title=None,
         genius_api_token=None,
         spotify_cookie=None,
         model_name="UVR_MDXNET_KARA_2",
         model_file_dir="/tmp/audio-separator-models",
         cache_dir="/tmp/karaoke-generator-cache",
         output_dir=None,
-        log_level=logging.DEBUG,
-        log_format="%(asctime)s - %(levelname)s - %(module)s - %(message)s",
     ):
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)
+        self.log_level = log_level
+        self.log_formatter = log_formatter
+
+        self.log_handler = logging.StreamHandler()
 
-        log_handler = logging.StreamHandler()
-        log_formatter = logging.Formatter(log_format)
-        log_handler.setFormatter(log_formatter)
-        self.logger.addHandler(log_handler)
+        if self.log_formatter is None:
+            self.log_formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(module)s - %(message)s")
+
+        self.log_handler.setFormatter(self.log_formatter)
+        self.logger.addHandler(self.log_handler)
 
         self.logger.debug("KaraokeGenerator initializing")
 
+        self.input_path = input_path
+        self.artist = artist
+        self.title = title
+
+        self.genius_api_token = os.getenv("GENIUS_API_TOKEN", default=genius_api_token)
+        self.spotify_cookie = os.getenv("SPOTIFY_COOKIE_SP_DC", default=spotify_cookie)
+
         self.model_name = model_name
         self.model_file_dir = model_file_dir
         self.cache_dir = cache_dir
         self.output_dir = output_dir
 
-        self.genius_api_token = os.getenv("GENIUS_API_TOKEN", default=genius_api_token)
-        self.spotify_cookie = os.getenv("SPOTIFY_COOKIE_SP_DC", default=spotify_cookie)
-
-        self.song_artist = song_artist
-        self.song_title = song_title
+        self.audio_file = None
+        self.youtube_url = None
 
-        if audio_file is None and youtube_url is None:
-            raise Exception("Either audio_file or youtube_url must be specified as the input source")
-        if audio_file is not None and youtube_url is not None:
-            raise Exception("Only one of audio_file or youtube_url may be specified as the input source")
-
-        if audio_file is not None:
-            self.input_source_slug = slugify.slugify(os.path.basename(audio_file), lowercase=False)
-        if youtube_url is not None:
-            parsed_url = urllib.parse.urlparse(youtube_url)
+        parsed_url = urllib.parse.urlparse(self.input_path)
+        if parsed_url.scheme and parsed_url.netloc:
+            self.youtube_url = self.input_path
             self.input_source_slug = slugify.slugify(parsed_url.hostname + "-" + parsed_url.query, lowercase=False)
+            self.logger.debug(f"Input path was valid URL, set youtube_url and input_source_slug: {self.input_source_slug}")
+        elif os.path.exists(self.input_path):
+            self.audio_file = self.input_path
+            self.input_source_slug = slugify.slugify(os.path.basename(self.audio_file), lowercase=False)
+            self.logger.debug(f"Input path was valid file path, set audio_file and input_source_slug: {self.input_source_slug}")
+        else:
+            raise Exception("Input path must be either a valid file path or URL")
 
         if self.output_dir is None:
             self.output_dir = os.path.join(os.getcwd(), "karaoke-generator-output-" + self.input_source_slug)
 
         self.output_filename_slug = None
-        self.youtube_url = youtube_url
         self.youtube_video_file = None
         self.youtube_video_image_file = None
 
-        self.audio_file = audio_file
         self.primary_stem_path = None
         self.secondary_stem_path = None
 
         self.output_values = {}
         self.create_folders()
 
     def generate(self):
@@ -91,18 +98,20 @@
         return self.output_values
 
     def transcribe_lyrics(self):
         transcriber = LyricsTranscriber(
             self.audio_file,
             genius_api_token=self.genius_api_token,
             spotify_cookie=self.spotify_cookie,
-            song_artist=self.song_artist,
-            song_title=self.song_title,
+            artist=self.artist,
+            title=self.title,
             output_dir=self.output_dir,
             cache_dir=self.cache_dir,
+            log_formatter=self.log_formatter,
+            log_level=self.log_level,
         )
 
         transcription_metadata = transcriber.generate()
 
         self.logger.debug(f"Transcription Success!")
 
         formatted_duration = (
@@ -137,14 +146,16 @@
         else:
             self.logger.debug(f"instantiating Separator with model_name: {self.model_name} and output_dir: {self.output_dir}")
             separator = Separator(
                 self.audio_file,
                 model_name=self.model_name,
                 model_file_dir=self.model_file_dir,
                 output_dir=self.output_dir,
+                log_formatter=self.log_formatter,
+                log_level=self.log_level,
             )
             self.primary_stem_path, self.secondary_stem_path = separator.separate()
 
             self.logger.debug(f"Separation complete! Output files: {self.primary_stem_path} {self.secondary_stem_path}")
 
         self.output_values["primary_stem_path"] = self.primary_stem_path
         self.output_values["secondary_stem_path"] = self.secondary_stem_path
@@ -200,25 +211,25 @@
                     json.dump(ydl.sanitize_info(youtube_info), cache_file, indent=4)
 
                 ydl.download([self.youtube_url])
                 shutil.move(temp_download_filepath, youtube_info["download_filepath"])
                 self.youtube_video_file = youtube_info["download_filepath"]
                 self.logger.debug(f"successfully downloaded youtube video to path: {self.youtube_video_file}")
 
-        if self.song_title is None:
+        if self.title is None:
             self.logger.debug(f"Song title not specified, attempting to split from YouTube title: {youtube_info['title']}")
             # Define the hyphen variations pattern
             hyphen_pattern = regex.compile(r" [^[:ascii:]-_\p{Dash}] ")
             # Split the string using the hyphen variations pattern
             title_parts = hyphen_pattern.split(youtube_info["title"])
 
-            self.song_artist = title_parts[0]
-            self.song_title = title_parts[1]
+            self.artist = title_parts[0]
+            self.title = title_parts[1]
 
-            print(f"Guessed metadata from title: Artist: {self.song_artist}, Title: {self.song_title}")
+            print(f"Guessed metadata from title: Artist: {self.artist}, Title: {self.title}")
 
         # Extract audio to WAV file using ffmpeg
         self.audio_file = os.path.join(self.cache_dir, self.output_filename_slug + ".wav")
         if os.path.isfile(self.audio_file):
             self.logger.debug(f"Existing file found at self.audio_file, skipping extraction: {self.audio_file}")
         else:
             self.logger.debug(f"Extracting audio from {self.youtube_video_file} to {self.audio_file}")
```

### Comparing `karaoke_video_generator-0.3.0/karaoke_generator/utils/cli.py` & `karaoke_video_generator-0.4.0/karaoke_generator/utils/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,54 @@
 #!/usr/bin/env python
 import argparse
 import logging
+import pkg_resources
 from karaoke_generator import KaraokeGenerator
 
 
 def main():
     logger = logging.getLogger(__name__)
-    logger.setLevel(logging.DEBUG)
-
     log_handler = logging.StreamHandler()
-    log_formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(module)s - %(message)s")
+    log_formatter = logging.Formatter(fmt="%(asctime)s.%(msecs)03d - %(levelname)s - %(module)s - %(message)s", datefmt="%Y-%m-%d %H:%M:%S")
     log_handler.setFormatter(log_formatter)
     logger.addHandler(log_handler)
 
-    logger.debug("Parsing CLI args")
-
-    parser = argparse.ArgumentParser(description="Generate karaoke music video for either a local audio file or YouTube URL")
-
-    input_group = parser.add_mutually_exclusive_group(required=True)
-    input_group.add_argument(
-        "--youtube_url",
-        default=None,
-        help="Optional: YouTube URL to make karaoke version of.",
+    parser = argparse.ArgumentParser(
+        description="Generate karaoke music video for either a local audio file or YouTube URL",
+        formatter_class=lambda prog: argparse.HelpFormatter(prog, max_help_position=40),
     )
-    input_group.add_argument(
-        "--audio_file",
-        default=None,
-        help="Optional: audio file path to make karaoke version of.",
+
+    parser.add_argument(
+        "input_path", nargs="?", help="The audio file path or YouTube URL to make karaoke version of.", default=argparse.SUPPRESS
     )
 
+    package_version = pkg_resources.get_distribution("karaoke-video-generator").version
+    parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {package_version}")
+    parser.add_argument("--log_level", default="INFO", help="Optional: Logging level, e.g. info, debug, warning. Default: INFO")
+
     parser.add_argument(
-        "--song_artist",
+        "--artist",
         default=None,
-        help="Optional: specify song artist for lyrics lookup and auto-correction",
+        help="Optional: song artist for lyrics lookup and auto-correction",
     )
     parser.add_argument(
-        "--song_title",
+        "--title",
         default=None,
-        help="Optional: specify song title for lyrics lookup and auto-correction",
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
-        help="Optional: specify Spotify SP_DC cookie value for lyrics lookup and auto-correction",
+        help="Optional: Spotify sp_dc cookie value for lyrics fetching. Can also be set with SPOTIFY_COOKIE_SP_DC env var.",
     )
 
     parser.add_argument(
         "--model_name",
         default="UVR_MDXNET_KARA_2",
         help="Optional: model name to be used for audio separation.",
     )
@@ -70,29 +66,38 @@
         "--output_dir",
         default=None,
         help="Optional: directory to write output files to. Defaults to a folder in the current directory.",
     )
 
     args = parser.parse_args()
 
-    logger.info(f"Karaoke generator beginning with audio_file: {args.audio_file} / youtube_url: {args.youtube_url}")
+    log_level = getattr(logging, args.log_level.upper())
+    logger.setLevel(log_level)
+
+    if not hasattr(args, "input_path"):
+        parser.print_help()
+        exit(1)
+
+    logger.info(f"Karaoke generator beginning with input_path: {args.input_path}")
 
     generator = KaraokeGenerator(
-        audio_file=args.audio_file,
-        youtube_url=args.youtube_url,
-        song_artist=args.song_artist,
-        song_title=args.song_title,
+        log_formatter=log_formatter,
+        log_level=log_level,
+        input_path=args.input_path,
+        artist=args.artist,
+        title=args.title,
         genius_api_token=args.genius_api_token,
         spotify_cookie=args.spotify_cookie,
         model_name=args.model_name,
         model_file_dir=args.model_file_dir,
         cache_dir=args.cache_dir,
         output_dir=args.output_dir,
     )
     outputs = generator.generate()
 
     logger.info(f"Karaoke generation complete!")
 
     logger.debug(f"Output folder: {outputs['output_dir']}")
-    
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `karaoke_video_generator-0.3.0/PKG-INFO` & `karaoke_video_generator-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: karaoke-video-generator
-Version: 0.3.0
+Version: 0.4.0
 Summary: Fully automated creation of _acceptable_ karaoke music videos from any music on YouTube, using open source tools and AI (e.g. Whisper and MDX-Net)
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: audio-separator (>=0,<1)
-Requires-Dist: lyrics-transcriber (>=0.5.1,<0.6.0)
+Requires-Dist: audio-separator (>=0.3,<0.4)
+Requires-Dist: lyrics-transcriber (>=0.6,<0.7)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: yt-dlp (>=2023.6.22,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # KaraokeHunt: Karaoke video generator
```

