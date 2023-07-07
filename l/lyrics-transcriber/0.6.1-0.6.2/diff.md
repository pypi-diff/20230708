# Comparing `tmp/lyrics_transcriber-0.6.1.tar.gz` & `tmp/lyrics_transcriber-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.6.1.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.6.2.tar", max compression
```

## Comparing `lyrics_transcriber-0.6.1.tar` & `lyrics_transcriber-0.6.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/LICENSE
--rw-r--r--   0        0        0     3513 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/README.md
--rw-r--r--   0        0        0       94 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0    13091 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     4176 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0     1244 2023-07-07 23:30:04.949550 lyrics_transcriber-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 lyrics_transcriber-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-07 23:36:37.237837 lyrics_transcriber-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3513 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/README.md
+-rw-r--r--   0        0        0       94 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0    13091 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     4176 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0     1427 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 lyrics_transcriber-0.6.2/PKG-INFO
```

### Comparing `lyrics_transcriber-0.6.1/LICENSE` & `lyrics_transcriber-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.6.1/README.md` & `lyrics_transcriber-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.6.1/lyrics_transcriber/transcriber.py` & `lyrics_transcriber-0.6.2/lyrics_transcriber/transcriber.py`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.6.1/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.6.2/lyrics_transcriber/utils/cli.py`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.6.1/pyproject.toml` & `lyrics_transcriber-0.6.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-transcriber"
-version = "0.6.1"
+version = "0.6.2"
 description = "Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "lyrics_transcriber" }]
 
 [tool.poetry.dependencies]
@@ -22,14 +22,16 @@
 python-slugify = "^8"
 syrics = "^0"
 openai-whisper = "20230314"
 whisper-timestamped = "^1"
 # Note: after adding openai-whisper and whisper-timestamped with poetry lock, I then removed all traces of triton
 # from poetry.lock before running poetry install, as triton doesn't support macOS but isn't actually needed for whisper.
 # This was the only way I was able to get a working cross-platform build published to PyPI.
+# To update the lockfile and install/upgrade dependencies, modify the dependency list above then run:
+# poetry lock; patch -p0 poetry.lock <.github/removetriton.patch; poetry install
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
 [tool.black]
 line-length = 140
```

### Comparing `lyrics_transcriber-0.6.1/PKG-INFO` & `lyrics_transcriber-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-transcriber
-Version: 0.6.1
+Version: 0.6.2
 Summary: Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

