# Comparing `tmp/rendersrt-0.0.7.tar.gz` & `tmp/rendersrt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rendersrt-0.0.7.tar", last modified: Tue Jun 20 08:56:41 2023, max compression
+gzip compressed data, was "rendersrt-0.0.8.tar", last modified: Sat Jul  8 13:19:31 2023, max compression
```

## Comparing `rendersrt-0.0.7.tar` & `rendersrt-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:56:41.286883 rendersrt-0.0.7/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1563 2023-06-20 08:56:41.286883 rendersrt-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 08:56:41.250174 rendersrt-0.0.7/rendersrt/
--rw-rw-rw-   0        0        0    67807 2023-06-20 08:46:24.000000 rendersrt-0.0.7/rendersrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:56:41.284639 rendersrt-0.0.7/rendersrt.egg-info/
--rw-rw-rw-   0        0        0     1563 2023-06-20 08:56:40.000000 rendersrt-0.0.7/rendersrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-20 08:56:41.000000 rendersrt-0.0.7/rendersrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:56:40.000000 rendersrt-0.0.7/rendersrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-20 08:56:40.000000 rendersrt-0.0.7/rendersrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-20 08:56:40.000000 rendersrt-0.0.7/rendersrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-20 08:56:40.000000 rendersrt-0.0.7/rendersrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-20 08:56:41.289880 rendersrt-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1362 2023-06-07 15:11:16.000000 rendersrt-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:19:31.330448 rendersrt-0.0.8/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1563 2023-07-08 13:19:31.331197 rendersrt-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 13:19:31.268263 rendersrt-0.0.8/rendersrt/
+-rw-rw-rw-   0        0        0    69964 2023-07-08 13:17:20.000000 rendersrt-0.0.8/rendersrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:19:31.328199 rendersrt-0.0.8/rendersrt.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-07-08 13:19:30.000000 rendersrt-0.0.8/rendersrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-07-08 13:19:31.000000 rendersrt-0.0.8/rendersrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:19:30.000000 rendersrt-0.0.8/rendersrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-08 13:19:30.000000 rendersrt-0.0.8/rendersrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-07-08 13:19:30.000000 rendersrt-0.0.8/rendersrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 13:19:30.000000 rendersrt-0.0.8/rendersrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-07-08 13:19:31.334193 rendersrt-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1362 2023-06-07 15:11:16.000000 rendersrt-0.0.8/setup.py
```

### Comparing `rendersrt-0.0.7/LICENSE` & `rendersrt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.7/PKG-INFO` & `rendersrt-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.7
+Version: 0.0.8
 Summary: a utility for rendering subtitle file into video file
 Home-page: https://github.com/botbahlul/rendersrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `rendersrt-0.0.7/README.md` & `rendersrt-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.7/rendersrt/__init__.py` & `rendersrt-0.0.8/rendersrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 import pysrt
 from pathlib import Path
 from datetime import datetime, timedelta
 import time
 
 
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -284,14 +284,17 @@
         self.list_names.append("Vietnamese")
         self.list_names.append("Welsh")
         self.list_names.append("Xhosa")
         self.list_names.append("Yiddish")
         self.list_names.append("Yoruba")
         self.list_names.append("Zulu")
 
+        # NOTE THAT Google Translate AND Vosk Speech Recognition API USE ISO-639-1 STANDARD CODE ('al', 'af', 'as', ETC)
+        # WHEN ffmpeg SUBTITLES STREAMS USE ISO 639-2 STANDARD CODE ('afr', 'alb', 'amh', ETC)
+
         self.list_ffmpeg_codes = []
         self.list_ffmpeg_codes.append("afr")  # Afrikaans
         self.list_ffmpeg_codes.append("alb")  # Albanian
         self.list_ffmpeg_codes.append("amh")  # Amharic
         self.list_ffmpeg_codes.append("ara")  # Arabic
         self.list_ffmpeg_codes.append("hye")  # Armenian
         self.list_ffmpeg_codes.append("asm")  # Assamese
@@ -420,19 +423,21 @@
         self.list_ffmpeg_codes.append("wel")  # Welsh
         self.list_ffmpeg_codes.append("xho")  # Xhosa
         self.list_ffmpeg_codes.append("yid")  # Yiddish
         self.list_ffmpeg_codes.append("yor")  # Yoruba
         self.list_ffmpeg_codes.append("zul")  # Zulu
 
         self.code_of_name = dict(zip(self.list_names, self.list_codes))
+        self.code_of_ffmpeg_code = dict(zip(self.list_ffmpeg_codes, self.list_codes))
+
         self.name_of_code = dict(zip(self.list_codes, self.list_names))
+        self.name_of_ffmpeg_code = dict(zip(self.list_ffmpeg_codes, self.list_names))
 
         self.ffmpeg_code_of_name = dict(zip(self.list_names, self.list_ffmpeg_codes))
         self.ffmpeg_code_of_code = dict(zip(self.list_codes, self.list_ffmpeg_codes))
-        self.name_of_ffmpeg_code = dict(zip(self.list_ffmpeg_codes, self.list_names))
 
         self.dict = {
                         'af': 'Afrikaans',
                         'sq': 'Albanian',
                         'am': 'Amharic',
                         'ar': 'Arabic',
                         'hy': 'Armenian',
@@ -698,62 +703,72 @@
                                 'cy': 'wel', # Welsh
                                 'xh': 'xho', # Xhosa
                                 'yi': 'yid', # Yiddish
                                 'yo': 'yor', # Yoruba
                                 'zu': 'zul', # Zulu
                            }
 
-    def get_name(self, get_code):
-        return self.dict.get(get_code.lower(), "")
+    def get_code_of_name(self, name):
+        return self.code_of_name[name]
+
+    def get_code_of_ffmpeg_code(self, ffmpeg_code):
+        return self.code_of_ffmpeg_code[ffmpeg_code]
+
+    def get_name_of_code(self, code):
+        return self.name_of_code[code]
+
+    def get_name_of_ffmpeg_code(self, ffmpeg_code):
+        return self.name_of_ffmpeg_code[ffmpeg_code]
 
-    def get_code(self, language):
-        for get_code, lang in self.dict.items():
-            if lang.lower() == language.lower():
-                return get_code
-        return ""
+    def get_ffmpeg_code_of_name(self, name):
+        return self.ffmpeg_code_of_name[name]
 
-    def get_ffmpeg_code(self, get_code):
-        return self.ffmpeg_dict.get(get_code.lower(), "")
+    def get_ffmpeg_code_of_code(self, code):
+        return self.ffmpeg_code_of_code[code]
 
 
 class SubtitleStreamParser:
+    def which(self, program):
+        def is_exe(file_path):
+            return os.path.isfile(file_path) and os.access(file_path, os.X_OK)
+        fpath, _ = os.path.split(program)
+        if fpath:
+            if is_exe(program):
+                return program
+        else:
+            for path in os.environ["PATH"].split(os.pathsep):
+                path = path.strip('"')
+                exe_file = os.path.join(path, program)
+                if is_exe(exe_file):
+                    return exe_file
+        return None
+
+    def ffprobe_check(self):
+        if self.which("ffprobe"):
+            return "ffprobe"
+        if self.which("ffprobe.exe"):
+            return "ffprobe.exe"
+        return None
+
+    def ffmpeg_check(self):
+        if self.which("ffmpeg"):
+            return "ffmpeg"
+        if self.which("ffmpeg.exe"):
+            return "ffmpeg.exe"
+        return None
+
     def __init__(self, error_messages_callback=None):
         self.error_messages_callback = error_messages_callback
         self._indexes = []
         self._languages = []
         self._timed_subtitles = []
         self._number_of_streams = 0
 
-    def __call__(self, media_filepath):
-        if "\\" in media_filepath:
-            media_filepath = media_filepath.replace("\\", "/")
-        subtitle_streams = self.get_subtitle_streams(media_filepath)
-        subtitle_streams_data = []
-        if subtitle_streams:
-            for subtitle_stream in subtitle_streams:
-                subtitle_stream_index = subtitle_stream['index']
-                subtitle_stream_language = subtitle_stream['language']
-                #print(f"Stream Index: {subtitle_stream_index}, Language: {subtitle_stream_language}")
-                subtitle_streams_data.append((subtitle_stream_index, subtitle_stream_language))
-
-        subtitle_data = []
-        subtitle_contents = []
-
-        for subtitle_stream_index in range(len(subtitle_streams)):
-            index, language = subtitle_streams_data[subtitle_stream_index]
-            self._indexes.append(index)
-            self._languages.append(language)
-            self._timed_subtitles.append(self.get_timed_subtitles(media_filepath, subtitle_stream_index+1))
-            subtitle_data.append((index, language, self.get_timed_subtitles(media_filepath, subtitle_stream_index+1)))
-
-        self._number_of_streams = len(subtitle_data)
-        return subtitle_data
 
     def get_subtitle_streams(self, media_filepath):
-
         ffprobe_cmd = [
                         'ffprobe',
                         '-hide_banner',
                         '-v', 'error',
                         '-loglevel', 'error',
                         '-print_format', 'json',
                         '-show_entries', 'stream=index:stream_tags=language',
@@ -801,15 +816,14 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return None
 
     def get_timed_subtitles(self, media_filepath, subtitle_stream_index):
-
         ffmpeg_cmd = [
                         'ffmpeg',
                         '-hide_banner',
                         '-loglevel', 'error',
                         '-v', 'error',
                         '-i', media_filepath,
                         '-map', f'0:s:{subtitle_stream_index-1}',
@@ -823,17 +837,16 @@
                 result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True)
 
             output = result.stdout
 
             timed_subtitles = []
-            subtitle_data = []
+            subtitle_streams_data_with_timed_subtitles = []
             lines = output.strip().split('\n')
-            #print(lines)
             subtitles = []
             subtitles = None
             subtitle_blocks = []
             block = []
             for line in lines:
                 if line.strip() == '':
                     subtitle_blocks.append(block)
@@ -897,48 +910,85 @@
         return self.timed_subtitles()[index-1]
 
     def timed_subtitles_of_language(self, language):
         for i in range(self.number_of_streams()):
             if self.languages()[i] == language:
                 return self.timed_subtitles()[i]
 
+    def __call__(self, media_filepath):
+        if "\\" in media_filepath:
+            media_filepath = media_filepath.replace("\\", "/")
+
+        if not self.ffprobe_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffprobe executable")
+            else:
+                print("Cannot find ffprobe executable")
+                raise Exception("Dependency not found: ffprobe")
+
+        if not self.ffmpeg_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffmpeg executable")
+            else:
+                print("Cannot find ffmpeg executable")
+                raise Exception("Dependency not found: ffmpeg")
+
+        subtitle_streams = self.get_subtitle_streams(media_filepath)
+        subtitle_streams_data = []
+        if subtitle_streams:
+            for subtitle_stream in subtitle_streams:
+                subtitle_stream_index = subtitle_stream['index']
+                subtitle_stream_language = subtitle_stream['language']
+                #print(f"Stream Index: {subtitle_stream_index}, Language: {subtitle_stream_language}")
+                subtitle_streams_data.append((subtitle_stream_index, subtitle_stream_language))
+
+        subtitle_streams_data_with_timed_subtitles = []
+
+        for subtitle_stream_index in range(len(subtitle_streams)):
+            index, language = subtitle_streams_data[subtitle_stream_index]
+            self._indexes.append(index)
+            self._languages.append(language)
+            self._timed_subtitles.append(self.get_timed_subtitles(media_filepath, subtitle_stream_index+1))
+            subtitle_streams_data_with_timed_subtitles.append((index, language, self.get_timed_subtitles(media_filepath, subtitle_stream_index+1)))
+
+        self._number_of_streams = len(subtitle_streams_data_with_timed_subtitles)
+
+        return subtitle_streams_data_with_timed_subtitles
+
 
 class MediaSubtitleRenderer:
-    @staticmethod
-    def which(program):
+    def which(self, program):
         def is_exe(file_path):
             return os.path.isfile(file_path) and os.access(file_path, os.X_OK)
         fpath, _ = os.path.split(program)
         if fpath:
             if is_exe(program):
                 return program
         else:
             for path in os.environ["PATH"].split(os.pathsep):
                 path = path.strip('"')
                 exe_file = os.path.join(path, program)
                 if is_exe(exe_file):
                     return exe_file
         return None
 
-    @staticmethod
-    def ffmpeg_check():
-        if MediaSubtitleRenderer.which("ffmpeg"):
-            return "ffmpeg"
-        if MediaSubtitleRenderer.which("ffmpeg.exe"):
-            return "ffmpeg.exe"
-        return None
-
-    @staticmethod
-    def ffprobe_check():
-        if MediaSubtitleRenderer.which("ffprobe"):
+    def ffprobe_check(self):
+        if self.which("ffprobe"):
             return "ffprobe"
-        if MediaSubtitleRenderer.which("ffprobe.exe"):
+        if self.which("ffprobe.exe"):
             return "ffprobe.exe"
         return None
 
+    def ffmpeg_check(self):
+        if self.which("ffmpeg"):
+            return "ffmpeg"
+        if self.which("ffmpeg.exe"):
+            return "ffmpeg.exe"
+        return None
+
     def __init__(self, subtitle_path=None, language=None, output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
         self.language = language
         self.output_path = output_path
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
@@ -1029,17 +1079,17 @@
                 if stderr_line == '' and process.poll() is not None:
                     break
 
                 if "out_time=" in stderr_line:
                     time_str = stderr_line.split('time=')[1].split()[0]
                     current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
-                    if current_duration>0:
+                    if current_duration>0 and current_duration<=total_duration*1000:
                         percentage = int(current_duration*100/(int(float(total_duration))*1000))
-                        if self.progress_callback:
+                        if self.progress_callback and percentage <= 100:
                             self.progress_callback(info, media_file_display_name, percentage, start_time)
 
             if os.path.isfile(self.output_path):
                 return self.output_path
             else:
                 return None
 
@@ -1178,17 +1228,18 @@
  
             if stderr_line == '' and process.poll() is not None:
                 break
 
             if "out_time=" in stderr_line:
                 time_str = stderr_line.split('time=')[1].split()[0]
                 current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                if current_duration>0:
+                if current_duration>0 and current_duration<=total_duration*1000:
                     percentage = int(current_duration*100/(int(float(total_duration))*1000))
-                    pbar.update(percentage)
+                    if percentage<=100:
+                        pbar.update(percentage)
         pbar.finish()
         return output_path
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
```

### Comparing `rendersrt-0.0.7/rendersrt.egg-info/PKG-INFO` & `rendersrt-0.0.8/rendersrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.7
+Version: 0.0.8
 Summary: a utility for rendering subtitle file into video file
 Home-page: https://github.com/botbahlul/rendersrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `rendersrt-0.0.7/setup.py` & `rendersrt-0.0.8/setup.py`

 * *Files identical despite different names*

