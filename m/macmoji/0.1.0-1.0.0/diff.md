# Comparing `tmp/macmoji-0.1.0.tar.gz` & `tmp/macmoji-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macmoji-0.1.0.tar", max compression
+gzip compressed data, was "macmoji-1.0.0.tar", max compression
```

## Comparing `macmoji-0.1.0.tar` & `macmoji-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     9839 2023-07-07 23:12:45.361756 macmoji-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-02 18:50:45.584375 macmoji-0.1.0/macmoji/__init__.py
--rw-r--r--   0        0        0      501 2023-07-07 14:24:41.879778 macmoji-0.1.0/macmoji/__main__.py
--rw-r--r--   0        0        0        0 2023-07-02 18:50:45.683808 macmoji-0.1.0/macmoji/cli/__init__.py
--rw-r--r--   0        0        0     5980 2023-07-07 14:34:00.361957 macmoji-0.1.0/macmoji/cli/create.py
--rw-r--r--   0        0        0     4318 2023-07-07 14:42:39.735837 macmoji-0.1.0/macmoji/cli/main.py
--rw-r--r--   0        0        0     1785 2023-07-07 22:47:43.350325 macmoji-0.1.0/macmoji/config.py
--rw-r--r--   0        0        0     2567 2023-07-07 14:33:18.214371 macmoji-0.1.0/macmoji/converter.py
--rw-r--r--   0        0        0     4166 2023-07-07 23:11:57.695983 macmoji-0.1.0/macmoji/font.py
--rw-r--r--   0        0        0     4496 2023-07-07 14:18:54.134095 macmoji-0.1.0/macmoji/inserter.py
--rw-r--r--   0        0        0    13968 2023-07-07 20:37:49.982038 macmoji-0.1.0/macmoji/utils.py
--rw-r--r--   0        0        0      625 2023-07-03 20:59:17.458826 macmoji-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10490 1970-01-01 00:00:00.000000 macmoji-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9957 2023-07-07 23:16:14.514022 macmoji-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-02 18:50:45.584375 macmoji-1.0.0/macmoji/__init__.py
+-rw-r--r--   0        0        0      501 2023-07-07 14:24:41.879778 macmoji-1.0.0/macmoji/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:50:45.683808 macmoji-1.0.0/macmoji/cli/__init__.py
+-rw-r--r--   0        0        0     5980 2023-07-07 14:34:00.361957 macmoji-1.0.0/macmoji/cli/create.py
+-rw-r--r--   0        0        0     4318 2023-07-07 14:42:39.735837 macmoji-1.0.0/macmoji/cli/main.py
+-rw-r--r--   0        0        0     1785 2023-07-07 22:47:43.350325 macmoji-1.0.0/macmoji/config.py
+-rw-r--r--   0        0        0     2567 2023-07-07 14:33:18.214371 macmoji-1.0.0/macmoji/converter.py
+-rw-r--r--   0        0        0     4166 2023-07-07 23:11:57.695983 macmoji-1.0.0/macmoji/font.py
+-rw-r--r--   0        0        0     4496 2023-07-07 14:18:54.134095 macmoji-1.0.0/macmoji/inserter.py
+-rw-r--r--   0        0        0    13968 2023-07-07 20:37:49.982038 macmoji-1.0.0/macmoji/utils.py
+-rw-r--r--   0        0        0      625 2023-07-07 23:18:38.533509 macmoji-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10608 1970-01-01 00:00:00.000000 macmoji-1.0.0/PKG-INFO
```

### Comparing `macmoji-0.1.0/README.md` & `macmoji-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![MacMoji logo](./macmoji-logo.png)
+![MacMoji logo](https://raw.githubusercontent.com/gustavwilliam/macmoji/main/macmoji-logo.png)
 
 ### MacMoji - Create custom emoji fonts for macOS.
 ---
 
 Desite Apple's tight control over iOS and macOS, there is a way to use *any* custom emojis on Mac! :star_struck: Best part? Using a custom emoji font doesn't interfere with Apple's standard emoji font, so if you ever decide to go back to using the default emojis, you can do so with a single click.
 
 # Table of contents
@@ -148,15 +148,15 @@
 - `/System/Library/Fonts/Apple Color Emoji.ttc` - system font
 - `~/Library/Fonts/Apple Color Emoji.ttc` - our custom font :heart_eyes:
 
 ## Generating a custom font
 
 In broad terms, the custom emoji font file is generatad by taking Apple's base emojis, decompiling the font files, inserting your assets in the right sizes and formats, and recompiling. Here's a diagram to illustrate the process, before we dig deeper :nerd_face:
 
-![Conversion process](./conversion-process.png)
+![Conversion process](https://raw.githubusercontent.com/gustavwilliam/macmoji/main/conversion-process.png)
 
 
 ### Formats
 
 These are terms you might see a lot when using MacMoji. In essence, this is what the file types are for:
 
 - **`TTC`** (TrueType Collection): a collection of multiple TTF files, combined into a single file
```

### Comparing `macmoji-0.1.0/macmoji/cli/create.py` & `macmoji-1.0.0/macmoji/cli/create.py`

 * *Files identical despite different names*

### Comparing `macmoji-0.1.0/macmoji/cli/main.py` & `macmoji-1.0.0/macmoji/cli/main.py`

 * *Files identical despite different names*

### Comparing `macmoji-0.1.0/macmoji/config.py` & `macmoji-1.0.0/macmoji/config.py`

 * *Files identical despite different names*

### Comparing `macmoji-0.1.0/macmoji/converter.py` & `macmoji-1.0.0/macmoji/converter.py`

 * *Files identical despite different names*

### Comparing `macmoji-0.1.0/macmoji/font.py` & `macmoji-1.0.0/macmoji/font.py`

 * *Files identical despite different names*

### Comparing `macmoji-0.1.0/macmoji/inserter.py` & `macmoji-1.0.0/macmoji/inserter.py`

 * *Files identical despite different names*

### Comparing `macmoji-0.1.0/macmoji/utils.py` & `macmoji-1.0.0/macmoji/utils.py`

 * *Files identical despite different names*

### Comparing `macmoji-0.1.0/pyproject.toml` & `macmoji-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "macmoji"
-version = "0.1.0"
+version = "1.0.0"
 description = "Create custom emoji fonts for macOS."
 authors = ["Gustav Odinger <65498475+gustavwilliam@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `macmoji-0.1.0/PKG-INFO` & `macmoji-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macmoji
-Version: 0.1.0
+Version: 1.0.0
 Summary: Create custom emoji fonts for macOS.
 Author: Gustav Odinger
 Author-email: 65498475+gustavwilliam@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,15 @@
 Requires-Dist: cairosvg (>=2.7.0,<3.0.0)
 Requires-Dist: fonttools (>=4.40.0,<5.0.0)
 Requires-Dist: humanize (>=4.7.0,<5.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
-![MacMoji logo](./macmoji-logo.png)
+![MacMoji logo](https://raw.githubusercontent.com/gustavwilliam/macmoji/main/macmoji-logo.png)
 
 ### MacMoji - Create custom emoji fonts for macOS.
 ---
 
 Desite Apple's tight control over iOS and macOS, there is a way to use *any* custom emojis on Mac! :star_struck: Best part? Using a custom emoji font doesn't interfere with Apple's standard emoji font, so if you ever decide to go back to using the default emojis, you can do so with a single click.
 
 # Table of contents
@@ -166,15 +166,15 @@
 - `/System/Library/Fonts/Apple Color Emoji.ttc` - system font
 - `~/Library/Fonts/Apple Color Emoji.ttc` - our custom font :heart_eyes:
 
 ## Generating a custom font
 
 In broad terms, the custom emoji font file is generatad by taking Apple's base emojis, decompiling the font files, inserting your assets in the right sizes and formats, and recompiling. Here's a diagram to illustrate the process, before we dig deeper :nerd_face:
 
-![Conversion process](./conversion-process.png)
+![Conversion process](https://raw.githubusercontent.com/gustavwilliam/macmoji/main/conversion-process.png)
 
 
 ### Formats
 
 These are terms you might see a lot when using MacMoji. In essence, this is what the file types are for:
 
 - **`TTC`** (TrueType Collection): a collection of multiple TTF files, combined into a single file
```

