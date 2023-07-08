# Comparing `tmp/whisper_autosrt-0.1.6.tar.gz` & `tmp/whisper_autosrt-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.1.6.tar", last modified: Tue Jun 20 09:59:16 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.1.7.tar", last modified: Sat Jul  8 03:50:34 2023, max compression
```

## Comparing `whisper_autosrt-0.1.6.tar` & `whisper_autosrt-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 09:59:16.226019 whisper_autosrt-0.1.6/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2056 2023-06-20 09:59:16.226768 whisper_autosrt-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.6/README.md
--rw-rw-rw-   0        0        0      147 2023-06-20 09:59:16.229232 whisper_autosrt-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1749 2023-06-19 22:39:09.000000 whisper_autosrt-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:59:16.188559 whisper_autosrt-0.1.6/whisper_autosrt/
--rw-rw-rw-   0        0        0   167742 2023-06-20 09:58:48.000000 whisper_autosrt-0.1.6/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:59:16.224519 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     2056 2023-06-20 09:59:15.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-20 09:59:16.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 09:59:15.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-20 09:59:15.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2023-06-20 09:59:15.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-20 09:59:15.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 03:50:34.653506 whisper_autosrt-0.1.7/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2056 2023-07-08 03:50:34.653506 whisper_autosrt-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.7/README.md
+-rw-rw-rw-   0        0        0      147 2023-07-08 03:50:34.657253 whisper_autosrt-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1749 2023-06-21 11:17:31.000000 whisper_autosrt-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:50:34.614548 whisper_autosrt-0.1.7/whisper_autosrt/
+-rw-rw-rw-   0        0        0   168522 2023-07-08 03:50:15.000000 whisper_autosrt-0.1.7/whisper_autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:50:34.650509 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2056 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-08 03:50:34.000000 whisper_autosrt-0.1.7/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.1.6/LICENSE` & `whisper_autosrt-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.6/PKG-INFO` & `whisper_autosrt-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_autosrt
-Version: 0.1.6
+Version: 0.1.7
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `whisper_autosrt-0.1.6/README.md` & `whisper_autosrt-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.6/setup.py` & `whisper_autosrt-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 install_requires=[
     "requests>=2.3.0",
     "httpx>=0.24.0",
     "urllib3 >=1.26.0,<3.0",
     "pysrt>=1.0.1",
     "six>=1.11.0",
     "progressbar2>=3.34.3",
-    "faster_whisper>=0.6.0",
+    "faster_whisper>=0.4.1",
 ]
 
 setup(
     name="whisper_autosrt",
     version=VERSION,
     description="a command line utility for automatic speech recognition and subtitle generation",
     long_description = long_description,
```

### Comparing `whisper_autosrt-0.1.6/whisper_autosrt/__init__.py` & `whisper_autosrt-0.1.7/whisper_autosrt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import warnings
 warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
 from faster_whisper import WhisperModel
 import ctypes
 import shutil
 
 
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 #marker='█'
 
 
 class WhisperLanguage:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("auto")
@@ -624,15 +624,15 @@
         self.list_names.append("Vietnamese")
         self.list_names.append("Welsh")
         self.list_names.append("Xhosa")
         self.list_names.append("Yiddish")
         self.list_names.append("Yoruba")
         self.list_names.append("Zulu")
 
-        # NOTE THAT Google Translate AND Whisper Speech Recognition API USE ISO-639-1 STANDARD CODE ('al', 'af', 'as', ETC)
+        # NOTE THAT Google Translate AND Vosk Speech Recognition API USE ISO-639-1 STANDARD CODE ('al', 'af', 'as', ETC)
         # WHEN ffmpeg SUBTITLES STREAMS USE ISO 639-2 STANDARD CODE ('afr', 'alb', 'amh', ETC)
 
         self.list_ffmpeg_codes = []
         self.list_ffmpeg_codes.append("afr")  # Afrikaans
         self.list_ffmpeg_codes.append("alb")  # Albanian
         self.list_ffmpeg_codes.append("amh")  # Amharic
         self.list_ffmpeg_codes.append("ara")  # Arabic
@@ -763,19 +763,21 @@
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
@@ -1041,21 +1043,30 @@
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
 
 
 google_unsupported_languages = ["auto", "ba", "br", "fo", "nn", "oc", "tl", "bo"]
 
 
 class WavConverter:
@@ -1087,15 +1098,15 @@
     def ffmpeg_check():
         if WavConverter.which("ffmpeg"):
             return "ffmpeg"
         if WavConverter.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
-    def __init__(self, channels=1, rate=48000, progress_callback=None, error_messages_callback=None):
+    def __init__(self, channels=1, rate=16000, progress_callback=None, error_messages_callback=None):
         self.channels = channels
         self.rate = rate
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
     def __call__(self, media_filepath):
         temp = tempfile.NamedTemporaryFile(suffix='.wav', delete=False)
@@ -1176,17 +1187,17 @@
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
@@ -1759,17 +1770,17 @@
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
 
@@ -1966,17 +1977,17 @@
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
 
@@ -2118,17 +2129,17 @@
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
 
@@ -2567,17 +2578,21 @@
  
             if stderr_line == '' and process.poll() is not None:
                 break
 
             if "out_time=" in stderr_line:
                 time_str = stderr_line.split('time=')[1].split()[0]
                 current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                if current_duration>0:
+
+                if current_duration>0 and current_duration<=total_duration*1000:
                     percentage = int(current_duration*100/(int(float(total_duration))*1000))
-                    pbar.update(percentage)
+                    if percentage <= 100:
+                        pbar.update(percentage)
+
+
         pbar.finish()
         return output_path
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
@@ -2698,17 +2713,19 @@
  
                 if stderr_line == '' and process.poll() is not None:
                     break
 
                 if "out_time=" in stderr_line:
                     time_str = stderr_line.split('time=')[1].split()[0]
                     current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                    if current_duration>0:
+
+                    if current_duration>0 and current_duration<=total_duration*1000:
                         percentage = int(current_duration*100/(int(float(total_duration))*1000))
-                        pbar.update(percentage)
+                        if percentage <= 100:
+                            pbar.update(percentage)
             pbar.finish()
 
             return output_path
 
         return
 
     except Exception as e:
@@ -2815,17 +2832,18 @@
  
             if stderr_line == '' and process.poll() is not None:
                 break
 
             if "out_time=" in stderr_line:
                 time_str = stderr_line.split('time=')[1].split()[0]
                 current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                if current_duration>0:
+                if current_duration>0 and current_duration<=total_duration*1000:
                     percentage = int(current_duration*100/(int(float(total_duration))*1000))
-                    pbar.update(percentage)
+                    if percentage <= 100:
+                        pbar.update(percentage)
         pbar.finish()
 
         return output_path
 
     except KeyboardInterrupt:
         if error_messages_callback:
             error_messages_callback("Cancelling all tasks")
@@ -3561,16 +3579,14 @@
 
             elif do_translate == True:
 
                 if args.embed_src == True and args.embed_dst == True:
 
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
-                    print(f"ffmpeg_src_language_code = {ffmpeg_src_language_code}")
-                    print(f"ffmpeg_dst_language_code = {ffmpeg_dst_language_code}")
 
                     base, ext = os.path.splitext(media_filepath)
                     src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
                     src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
                     embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
 
                     widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
```

### Comparing `whisper_autosrt-0.1.6/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.1.7/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-autosrt
-Version: 0.1.6
+Version: 0.1.7
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

