# Comparing `tmp/embedsrt-0.0.2.tar.gz` & `tmp/embedsrt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedsrt-0.0.2.tar", last modified: Tue Jun 20 09:12:44 2023, max compression
+gzip compressed data, was "embedsrt-0.0.3.tar", last modified: Sat Jul  8 13:20:32 2023, max compression
```

## Comparing `embedsrt-0.0.2.tar` & `embedsrt-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 09:12:44.908788 embedsrt-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 embedsrt-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 embedsrt-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1560 2023-06-20 09:12:44.909539 embedsrt-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3199 2023-06-07 14:26:01.000000 embedsrt-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 09:12:44.866832 embedsrt-0.0.2/embedsrt/
--rw-rw-rw-   0        0        0    71202 2023-06-20 08:55:52.000000 embedsrt-0.0.2/embedsrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:12:44.906541 embedsrt-0.0.2/embedsrt.egg-info/
--rw-rw-rw-   0        0        0     1560 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-20 09:12:44.911786 embedsrt-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1355 2023-06-07 14:21:47.000000 embedsrt-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:20:32.790245 embedsrt-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 embedsrt-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 embedsrt-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1560 2023-07-08 13:20:32.790992 embedsrt-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3199 2023-06-07 14:26:01.000000 embedsrt-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 13:20:32.755030 embedsrt-0.0.3/embedsrt/
+-rw-rw-rw-   0        0        0    73365 2023-07-08 13:17:54.000000 embedsrt-0.0.3/embedsrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:20:32.788746 embedsrt-0.0.3/embedsrt.egg-info/
+-rw-rw-rw-   0        0        0     1560 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 13:20:32.000000 embedsrt-0.0.3/embedsrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-07-08 13:20:32.793991 embedsrt-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2023-06-07 14:21:47.000000 embedsrt-0.0.3/setup.py
```

### Comparing `embedsrt-0.0.2/LICENSE` & `embedsrt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `embedsrt-0.0.2/PKG-INFO` & `embedsrt-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedsrt
-Version: 0.0.2
+Version: 0.0.3
 Summary: a utility for embedding subtitle file into video file
 Home-page: https://github.com/botbahlul/embedsrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `embedsrt-0.0.2/README.md` & `embedsrt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `embedsrt-0.0.2/embedsrt/__init__.py` & `embedsrt-0.0.3/embedsrt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 import pysrt
 from pathlib import Path
 from datetime import datetime, timedelta
 import time
 
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 
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
 
-    def get_code(self, language):
-        for get_code, lang in self.dict.items():
-            if lang.lower() == language.lower():
-                return get_code
-        return ""
+    def get_name_of_ffmpeg_code(self, ffmpeg_code):
+        return self.name_of_ffmpeg_code[ffmpeg_code]
 
-    def get_ffmpeg_code(self, get_code):
-        return self.ffmpeg_dict.get(get_code.lower(), "")
+    def get_ffmpeg_code_of_name(self, name):
+        return self.ffmpeg_code_of_name[name]
+
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
@@ -897,45 +910,82 @@
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
 
 class MediaSubtitleEmbedder:
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
-    def ffprobe_check():
-        if MediaSubtitleEmbedder.which("ffprobe"):
+    def ffprobe_check(self):
+        if self.which("ffprobe"):
             return "ffprobe"
-        if MediaSubtitleEmbedder.which("ffprobe.exe"):
+        if self.which("ffprobe.exe"):
             return "ffprobe.exe"
         return None
 
-    @staticmethod
-    def ffmpeg_check():
-        if MediaSubtitleEmbedder.which("ffmpeg"):
+    def ffmpeg_check(self):
+        if self.which("ffmpeg"):
             return "ffmpeg"
-        if MediaSubtitleEmbedder.which("ffmpeg.exe"):
+        if self.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
     def __init__(self, subtitle_path=None, language=None, output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
         self.language = language
         self.output_path = output_path
@@ -1079,17 +1129,18 @@
  
                     if stderr_line == '' and process.poll() is not None:
                         break
 
                     if "out_time=" in stderr_line:
                         time_str = stderr_line.split('time=')[1].split()[0]
                         current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                        if current_duration>0:
+
+                        if current_duration>0 and current_duration<=total_duration*1000:
                             percentage = int(current_duration*100/(int(float(total_duration))*1000))
-                            if self.progress_callback:
+                            if self.progress_callback and percentage <= 100:
                                 self.progress_callback(info, media_file_display_name, percentage, start_time)
 
                 if os.path.isfile(self.output_path):
                     return self.output_path
                 else:
                     return None
 
@@ -1241,17 +1292,18 @@
  
                 if stderr_line == '' and process.poll() is not None:
                     break
 
                 if "out_time=" in stderr_line:
                     time_str = stderr_line.split('time=')[1].split()[0]
                     current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                    if current_duration>0:
+                    if current_duration>0 and current_duration<=total_duration*1000:
                         percentage = int(current_duration*100/(int(float(total_duration))*1000))
-                        pbar.update(percentage)
+                        if percentage<=100:
+                            pbar.update(percentage)
             pbar.finish()
 
             return output_path
 
         return
 
     except Exception as e:
```

### Comparing `embedsrt-0.0.2/embedsrt.egg-info/PKG-INFO` & `embedsrt-0.0.3/embedsrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedsrt
-Version: 0.0.2
+Version: 0.0.3
 Summary: a utility for embedding subtitle file into video file
 Home-page: https://github.com/botbahlul/embedsrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `embedsrt-0.0.2/setup.py` & `embedsrt-0.0.3/setup.py`

 * *Files identical despite different names*

