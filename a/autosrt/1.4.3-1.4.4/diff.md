# Comparing `tmp/autosrt-1.4.3.tar.gz` & `tmp/autosrt-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.4.3.tar", last modified: Tue Jun 20 10:29:50 2023, max compression
+gzip compressed data, was "autosrt-1.4.4.tar", last modified: Sat Jul  8 03:55:41 2023, max compression
```

## Comparing `autosrt-1.4.3.tar` & `autosrt-1.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:29:50.945791 autosrt-1.4.3/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.3/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-06-20 10:29:50.946539 autosrt-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 10:29:50.740152 autosrt-1.4.3/autosrt/
--rw-rw-rw-   0        0        0   161800 2023-06-20 08:16:41.000000 autosrt-1.4.3/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:29:50.825841 autosrt-1.4.3/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-20 10:29:50.951036 autosrt-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:29:50.941295 autosrt-1.4.3/test/
--rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.3/test/test1.py
--rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.3/test/test2.py
--rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.3/test/test3.py
--rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.3/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:55:41.184198 autosrt-1.4.4/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-07-08 03:55:41.184947 autosrt-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 03:55:40.895872 autosrt-1.4.4/autosrt/
+-rw-rw-rw-   0        0        0   162921 2023-07-08 03:55:07.000000 autosrt-1.4.4/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:55:40.964839 autosrt-1.4.4/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-08 03:55:40.000000 autosrt-1.4.4/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-07-08 03:55:41.203678 autosrt-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:55:41.180452 autosrt-1.4.4/test/
+-rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.4/test/test1.py
+-rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.4/test/test2.py
+-rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.4/test/test3.py
+-rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.4/test/test4.py
```

### Comparing `autosrt-1.4.3/LICENSE` & `autosrt-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.3/PKG-INFO` & `autosrt-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.4.3
+Version: 1.4.4
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.4.3/README.md` & `autosrt-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.3/autosrt/__init__.py` & `autosrt-1.4.4/autosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import time
 from datetime import datetime, timedelta
 from pathlib import Path
 import shlex
 import shutil
 
 
-VERSION = "1.4.3"
+VERSION = "1.4.4"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -299,14 +299,17 @@
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
@@ -435,19 +438,21 @@
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
@@ -713,54 +718,60 @@
                                 'cy': 'wel', # Welsh
                                 'xh': 'xho', # Xhosa
                                 'yi': 'yid', # Yiddish
                                 'yo': 'yor', # Yoruba
                                 'zu': 'zul', # Zulu
                            }
 
-    def get_name(self, code):
+    def get_code_of_name(self, name):
+        return self.code_of_name[name]
+
+    def get_code_of_ffmpeg_code(self, ffmpeg_code):
+        return self.code_of_ffmpeg_code[ffmpeg_code]
+
+    def get_name_of_code(self, code):
         return self.name_of_code[code]
 
-    def get_code(self, language):
-        return self.code_of_name[language]
+    def get_name_of_ffmpeg_code(self, ffmpeg_code):
+        return self.name_of_ffmpeg_code[ffmpeg_code]
+
+    def get_ffmpeg_code_of_name(self, name):
+        return self.ffmpeg_code_of_name[name]
 
-    def get_ffmpeg_code(self, code):
+    def get_ffmpeg_code_of_code(self, code):
         return self.ffmpeg_code_of_code[code]
 
 
 class WavConverter:
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
-        if WavConverter.which("ffprobe"):
+    def ffprobe_check(self):
+        if self.which("ffprobe"):
             return "ffprobe"
-        if WavConverter.which("ffprobe.exe"):
+        if self.which("ffprobe.exe"):
             return "ffprobe.exe"
         return None
 
-    @staticmethod
-    def ffmpeg_check():
-        if WavConverter.which("ffmpeg"):
+    def ffmpeg_check(self):
+        if self.which("ffmpeg"):
             return "ffmpeg"
-        if WavConverter.which("ffmpeg.exe"):
+        if self.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
     def __init__(self, channels=1, rate=48000, progress_callback=None, error_messages_callback=None):
         self.channels = channels
         self.rate = rate
         self.progress_callback = progress_callback
@@ -845,17 +856,17 @@
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
 
             temp.close()
 
             return temp.name, self.rate
 
         except KeyboardInterrupt:
@@ -890,16 +901,15 @@
     #main_window.write_event_value('-EXCEPTION-', messages) AND HANDLE THAT EVENT IN pysimplegui MAIN LOOP
 # IF WE'RE IN console ENVIRONMENT WE CAN DO :
 #def show_error_messages(messages):
     #print(messages)
 
 
 class SpeechRegionFinder:
-    @staticmethod
-    def percentile(arr, percent):
+    def percentile(self, arr, percent):
         arr = sorted(arr)
         k = (len(arr) - 1) * percent
         f = math.floor(k)
         c = math.ceil(k)
         if f == c: return arr[int(k)]
         d0 = arr[int(f)] * (c - k)
         d1 = arr[int(c)] * (k - f)
@@ -921,15 +931,15 @@
             total_duration = reader.getnframes() / rate
             chunk_duration = float(self.frame_width) / rate
             n_chunks = int(total_duration / chunk_duration)
             energies = []
             for i in range(n_chunks):
                 chunk = reader.readframes(self.frame_width)
                 energies.append(audioop.rms(chunk, sample_width * n_channels))
-            threshold = SpeechRegionFinder.percentile(energies, 0.2)
+            threshold = self.percentile(energies, 0.2)
             elapsed_time = 0
             regions = []
             region_start = None
             for energy in energies:
                 is_silence = energy <= threshold
                 max_exceeded = region_start and elapsed_time - region_start >= self.max_region_size
                 if (max_exceeded or is_silence) and region_start:
@@ -953,35 +963,33 @@
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
 class FLACConverter(object):
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
-        if FLACConverter.which("ffmpeg"):
+    def ffmpeg_check(self):
+        if self.which("ffmpeg"):
             return "ffmpeg"
-        if FLACConverter.which("ffmpeg.exe"):
+        if self.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
     #def __init__(self, wav_filepath, include_before=0.25, include_after=0.25):
     def __init__(self, wav_filepath, include_before=0.25, include_after=0.25, error_messages_callback=None):
         self.wav_filepath = wav_filepath
         self.include_before = include_before
@@ -991,15 +999,15 @@
     #def __call__(self, region, error_messages_callback=None):
     def __call__(self, region):
         if not self.ffmpeg_check():
             if self.error_messages_callback:
                 self.error_messages_callback("Cannot find ffmpeg executable")
             else:
                 print("Cannot find ffmpeg executable")
-                raise Exception("Dependency not found: ffmpeg")
+            raise Exception("Dependency not found: ffmpeg")
 
         try:
             if "\\" in self.wav_filepath:
                 self.wav_filepath = self.wav_filepath.replace("\\", "/")
 
             start, end = region
             start = max(0, start - self.include_before)
@@ -1291,48 +1299,52 @@
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
 class SubtitleStreamParser:
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
-        if SubtitleStreamParser.which("ffprobe"):
+    def ffprobe_check(self):
+        if self.which("ffprobe"):
             return "ffprobe"
-        if SubtitleStreamParser.which("ffprobe.exe"):
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
     def __init__(self, error_messages_callback=None):
         self.error_messages_callback = error_messages_callback
         self._indexes = []
         self._languages = []
         self._timed_subtitles = []
         self._number_of_streams = 0
 
 
     def get_subtitle_streams(self, media_filepath):
-
         ffprobe_cmd = [
                         'ffprobe',
                         '-hide_banner',
                         '-v', 'error',
                         '-loglevel', 'error',
                         '-print_format', 'json',
                         '-show_entries', 'stream=index:stream_tags=language',
@@ -1380,15 +1392,14 @@
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
@@ -1402,17 +1413,16 @@
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
@@ -1487,71 +1497,74 @@
         if not self.ffprobe_check():
             if self.error_messages_callback:
                 self.error_messages_callback("Cannot find ffprobe executable")
             else:
                 print("Cannot find ffprobe executable")
                 raise Exception("Dependency not found: ffprobe")
 
+        if not self.ffmpeg_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffmpeg executable")
+            else:
+                print("Cannot find ffmpeg executable")
+                raise Exception("Dependency not found: ffmpeg")
+
         subtitle_streams = self.get_subtitle_streams(media_filepath)
         subtitle_streams_data = []
         if subtitle_streams:
             for subtitle_stream in subtitle_streams:
                 subtitle_stream_index = subtitle_stream['index']
                 subtitle_stream_language = subtitle_stream['language']
                 #print(f"Stream Index: {subtitle_stream_index}, Language: {subtitle_stream_language}")
                 subtitle_streams_data.append((subtitle_stream_index, subtitle_stream_language))
 
-        subtitle_data = []
-        subtitle_contents = []
+        subtitle_streams_data_with_timed_subtitles = []
 
         for subtitle_stream_index in range(len(subtitle_streams)):
             index, language = subtitle_streams_data[subtitle_stream_index]
             self._indexes.append(index)
             self._languages.append(language)
             self._timed_subtitles.append(self.get_timed_subtitles(media_filepath, subtitle_stream_index+1))
-            subtitle_data.append((index, language, self.get_timed_subtitles(media_filepath, subtitle_stream_index+1)))
+            subtitle_streams_data_with_timed_subtitles.append((index, language, self.get_timed_subtitles(media_filepath, subtitle_stream_index+1)))
 
-        self._number_of_streams = len(subtitle_data)
+        self._number_of_streams = len(subtitle_streams_data_with_timed_subtitles)
 
-        return subtitle_data
+        return subtitle_streams_data_with_timed_subtitles
 
 
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
 
@@ -1642,17 +1655,17 @@
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
 
@@ -1668,43 +1681,40 @@
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
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
@@ -1849,17 +1859,17 @@
                     if stderr_line == '' and process.poll() is not None:
                         break
 
                     if "out_time=" in stderr_line:
                         time_str = stderr_line.split('time=')[1].split()[0]
                         current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
-                        if current_duration>0:
+                        if current_duration>0 and current_duration<=total_duration*1000:
                             percentage = int(current_duration*100/(int(float(total_duration))*1000))
-                            if self.progress_callback:
+                            if self.progress_callback and percentage <= 100:
                                 self.progress_callback(info, media_file_display_name, percentage, start_time)
 
                 if os.path.isfile(self.output_path):
                     return self.output_path
                 else:
                     return None
 
@@ -1880,43 +1890,40 @@
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
 class MediaSubtitleRemover:
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
-        if MediaSubtitleRemover.which("ffprobe"):
+    def ffprobe_check(self):
+        if self.which("ffprobe"):
             return "ffprobe"
-        if MediaSubtitleRemover.which("ffprobe.exe"):
+        if self.which("ffprobe.exe"):
             return "ffprobe.exe"
         return None
 
-    @staticmethod
-    def ffmpeg_check():
-        if MediaSubtitleRemover.which("ffmpeg"):
+    def ffmpeg_check(self):
+        if self.which("ffmpeg"):
             return "ffmpeg"
-        if MediaSubtitleRemover.which("ffmpeg.exe"):
+        if self.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
     def __init__(self, output_path=None, progress_callback=None, error_messages_callback=None):
         self.output_path = output_path
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
@@ -2001,17 +2008,17 @@
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
 
@@ -2032,25 +2039,23 @@
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
 class SRTFileReader:
-    def __init__(self, srt_file_path, error_messages_callback=None):
-        self.timed_subtitles = self(srt_file_path)
+    def __init__(self, error_messages_callback=None):
         self.error_messages_callback = error_messages_callback
+        self.timed_subtitles = []
 
-    @staticmethod
-    def __call__(srt_file_path):
+    def __call__(self, srt_file_path):
         try:
             """
             Read SRT formatted subtitles file and return subtitles as list of tuples
             """
-            timed_subtitles = []
             with open(srt_file_path, 'r') as srt_file:
                 lines = srt_file.readlines()
                 # Split the subtitles file into subtitles blocks
                 subtitle_blocks = []
                 block = []
                 for line in lines:
                     if line.strip() == '':
@@ -2068,16 +2073,16 @@
                         time_format = '%H:%M:%S,%f'
                         start_time_time_delta = datetime.strptime(start_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
                         start_time_total_seconds = start_time_time_delta.total_seconds()
                         end_time_time_delta = datetime.strptime(end_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
                         end_time_total_seconds = end_time_time_delta.total_seconds()
                         # Extract subtitles text from subtitles block
                         subtitles = ' '.join(block[2:])
-                        timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitles))
-                return timed_subtitles
+                        self.timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitles))
+                return self.timed_subtitles
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
                 self.error_messages_callback("Cancelling all tasks")
             else:
                 print("Cancelling all tasks")
             return
@@ -2362,17 +2367,18 @@
  
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
@@ -2508,17 +2514,18 @@
  
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
@@ -2640,17 +2647,18 @@
  
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
 
     except KeyboardInterrupt:
         if error_messages_callback:
             error_messages_callback("Cancelling all tasks")
```

### Comparing `autosrt-1.4.3/autosrt.egg-info/PKG-INFO` & `autosrt-1.4.4/autosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.4.3
+Version: 1.4.4
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.4.3/setup.py` & `autosrt-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.3/test/test1.py` & `autosrt-1.4.4/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.3/test/test2.py` & `autosrt-1.4.4/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.3/test/test3.py` & `autosrt-1.4.4/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.3/test/test4.py` & `autosrt-1.4.4/test/test4.py`

 * *Files identical despite different names*

