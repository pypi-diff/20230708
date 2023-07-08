# Comparing `tmp/visionscript-0.0.1.tar.gz` & `tmp/visionscript-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionscript-0.0.1.tar", last modified: Thu Jul  6 16:13:33 2023, max compression
+gzip compressed data, was "visionscript-0.0.2.tar", last modified: Sat Jul  8 09:35:39 2023, max compression
```

## Comparing `visionscript-0.0.1.tar` & `visionscript-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,38 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-06 16:13:33.465256 visionscript-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)     1056 2023-07-06 08:06:43.000000 visionscript-0.0.1/LICENSE
--rw-r--r--   0 james      (501) staff       (20)       24 2023-07-06 14:34:07.000000 visionscript-0.0.1/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     6374 2023-07-06 16:13:33.465031 visionscript-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     5857 2023-07-06 16:12:06.000000 visionscript-0.0.1/README.md
--rw-r--r--   0 james      (501) staff       (20)      161 2023-07-06 08:06:43.000000 visionscript-0.0.1/requirements.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-07-06 16:13:33.465330 visionscript-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1193 2023-07-06 14:34:00.000000 visionscript-0.0.1/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-06 16:13:33.462964 visionscript-0.0.1/visionscript/
--rw-r--r--   0 james      (501) staff       (20)       41 2023-07-04 20:13:52.000000 visionscript-0.0.1/visionscript/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1957 2023-07-06 13:38:43.000000 visionscript-0.0.1/visionscript/grammar.py
--rw-r--r--   0 james      (501) staff       (20)    21846 2023-07-06 14:29:30.000000 visionscript-0.0.1/visionscript/lang.py
--rw-r--r--   0 james      (501) staff       (20)     1654 2023-07-06 14:30:02.000000 visionscript-0.0.1/visionscript/usage.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-06 16:13:33.464557 visionscript-0.0.1/visionscript.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     6374 2023-07-06 16:13:33.000000 visionscript-0.0.1/visionscript.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      326 2023-07-06 16:13:33.000000 visionscript-0.0.1/visionscript.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-07-06 16:13:33.000000 visionscript-0.0.1/visionscript.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      215 2023-07-06 16:13:33.000000 visionscript-0.0.1/visionscript.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       13 2023-07-06 16:13:33.000000 visionscript-0.0.1/visionscript.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 09:35:39.541249 visionscript-0.0.2/
+-rw-r--r--   0 james      (501) staff       (20)       16 2023-07-06 16:15:17.000000 visionscript-0.0.2/CNAME
+-rw-r--r--   0 james      (501) staff       (20)     1056 2023-07-06 08:06:43.000000 visionscript-0.0.2/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)       24 2023-07-06 16:15:17.000000 visionscript-0.0.2/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     6374 2023-07-08 09:35:39.541030 visionscript-0.0.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     5857 2023-07-06 16:15:17.000000 visionscript-0.0.2/README.md
+-rw-r--r--   0 james      (501) staff       (20)   725622 2023-07-06 14:40:32.000000 visionscript-0.0.2/banner.png
+-rw-r--r--   0 james      (501) staff       (20)      171 2023-07-06 23:02:32.000000 visionscript-0.0.2/requirements.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-07-08 09:35:39.541308 visionscript-0.0.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1337 2023-07-06 22:41:49.000000 visionscript-0.0.2/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 09:35:39.536507 visionscript-0.0.2/tests/
+-rw-r--r--   0 james      (501) staff       (20)       53 2023-07-08 06:32:08.000000 visionscript-0.0.2/tests/classify_image.vic
+-rw-r--r--   0 james      (501) staff       (20)       46 2023-07-06 23:35:58.000000 visionscript-0.0.2/tests/find_in_images.vic
+-rw-r--r--   0 james      (501) staff       (20)       63 2023-07-08 06:31:57.000000 visionscript-0.0.2/tests/load_detect_save.vic
+-rw-r--r--   0 james      (501) staff       (20)       97 2023-07-08 06:31:57.000000 visionscript-0.0.2/tests/replace_in_images.vic
+-rw-r--r--   0 james      (501) staff       (20)       49 2023-07-08 06:32:08.000000 visionscript-0.0.2/tests/segment_image.vic
+-rw-r--r--   0 james      (501) staff       (20)      602 2023-07-08 07:07:01.000000 visionscript-0.0.2/tests/test.py
+-rw-r--r--   0 james      (501) staff       (20)       31 2023-07-06 23:35:53.000000 visionscript-0.0.2/tests/train_od.vic
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 09:35:39.538646 visionscript-0.0.2/visionscript/
+-rw-r--r--   0 james      (501) staff       (20)       55 2023-07-08 09:35:31.000000 visionscript-0.0.2/visionscript/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     3141 2023-07-07 23:12:56.000000 visionscript-0.0.2/visionscript/grammar.py
+-rw-r--r--   0 james      (501) staff       (20)    38745 2023-07-08 09:35:22.000000 visionscript-0.0.2/visionscript/lang.py
+-rw-r--r--   0 james      (501) staff       (20)     3743 2023-07-08 09:05:17.000000 visionscript-0.0.2/visionscript/notebook.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 09:35:39.540764 visionscript-0.0.2/visionscript/std/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/caption.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/classify.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/detect.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/label.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/segment.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/train.py
+-rw-r--r--   0 james      (501) staff       (20)     1655 2023-07-06 22:30:51.000000 visionscript-0.0.2/visionscript/usage.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 09:35:39.539807 visionscript-0.0.2/visionscript.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     6374 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      733 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       56 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      225 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       13 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/top_level.txt
```

### Comparing `visionscript-0.0.1/LICENSE` & `visionscript-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.1/PKG-INFO` & `visionscript-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionscript
-Version: 0.0.1
+Version: 0.0.2
 Summary: VisionScript is an abstract programming language for doing common computer vision tasks, fast.
 Home-page: https://github.com/capjamesg/visionscript
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `visionscript-0.0.1/README.md` & `visionscript-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.1/setup.py` & `visionscript-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,23 @@
     author="capjamesg",
     author_email="jamesg@jamesg.blog",
     description="VisionScript is an abstract programming language for doing common computer vision tasks, fast.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/capjamesg/visionscript",
     install_requires=reqs,
-    packages=find_packages(exclude=("tests",)),
+    packages=find_packages(exclude=("tests",), include=("visionscript",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
+    entry_points={
+        "console_scripts": [
+            "visionscript=visionscript.lang:main",
+        ],
+    },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
```

### Comparing `visionscript-0.0.1/visionscript/grammar.py` & `visionscript-0.0.2/visionscript/grammar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,71 @@
 grammar = """
-start: (expr)*
+start: (expr | EOL | EOF | " ")*
 
-expr: (if | in | train | label | detect | countinregion | help | list | get | exit | read | compare | count | cutout | show | size | caption | say | save | load | use | replace | var | classify | segment | comment | contains | if | else | end | tutorial | make | run | isita | find | describe) (EOL | EOF | " ")
+expr: (if | in | train | label | detect | countinregion | help | list | get | exit | read | compare | count | cutout | show | size | caption | say | save | load | use | replace | var | classify | segment | comment | contains | if | else | end | make | run | isita | find | describe | import | rotate | getcolours | getcolors | get_text | greyscale | select | paste | pasterandom | resize | blur | literal | setbrightness | search | similarity | readqr | reset | negate | BOOL | INT | equality | not_equality | input) (EOL | EOF | " ")
 classify: "Classify" "[" STRING ("," STRING)* "]"
 var: variable "=" expr
 replace: "Replace" "[" STRING "]"
 use: "Use" "[" STRING "]"
-load: "Load" "[" STRING "]" | "Load" "[" "]"
+load: "Load" "[" (STRING | input) "]" | "Load" ("[" "]")?
 save: "Save" "[" STRING "]"
-say: "Say" "[" "]"
-describe: "Describe" "[" "]"
+say: "Say" "[" STRING "]" | "Say" ("[" "]")?
+get_text: "GetText" ("[" "]")?
+greyscale: "Greyscale" ("[" "]")?
+search: "Search" "[" STRING "]"
+describe: "Describe" ("[" "]")?
+readqr: "ReadQR" ("[" "]")?
+rotate: "Rotate" "[" INT "]"
+resize: "Resize" "[" INT "," INT "]"
+getcolors: "GetColors" ("[" "]")? | "GetColors" "[" INT "]"
+getcolours: "GetColours" ("[" "]")? | "GetColours" "[" INT "]"
 isita: "Is it a " (("," STRING)* | ("or" STRING)*)? EOL
 find: "Find" "[" STRING "]"
 args: ((STRING | INT | expr) ("," (STRING | INT | expr))*) | (STRING | INT | expr)?
-make: "Make" STRING "[" args "]" EOL (INDENT expr+)*
-caption: "Caption" "[" "]"
-size: "Size" "[" "]"
+make: "Make" literal ("[" args "]")? EOL (INDENT expr+)* EOL
+caption: "Caption" ("[" "]")?
+size: "Size" ("[" "]")?
+import: "Import" "[" STRING "]"
 run: "Run" "[" STRING "]"
-show: "Show" "[" "]"
-cutout: "Cutout" "[" "]"
-count: "Count" "[" "]"
+show: "Show" ("[" "]")?
+select: "Select" ("[" "]")? | "Select" "[" INT "]"
+paste: "Paste" "[" INT "," INT "]"
+pasterandom: "PasteRandom" ("[" "]")?
+cutout: "Cutout" ("[" "]")?
+count: "Count" ("[" "]")?
+input: "Input" ("[" STRING "]")?
 contains: "Contains" "[" STRING "]"
-compare: "Compare" "[" "]"
-read: "Read" "[" "]"
-exit: "Exit" "[" "]"
+compare: "Compare" ("[" "]")?
+setbrightness: "SetBrightness" "[" INT "]"
+read: "Read" ("[" "]")?
+exit: "Exit" ("[" "]")?
+blur: "Blur" ("[" "]")?
+similarity: "Similarity" ("[" INT "]")?
 get: "Get" "[" INT "]" EOL
 list: "[" ((STRING | INT | expr) "," | (STRING | INT | expr) )* "]" EOL
 help: "Help" "[" STRING "]"
-end: "End" "[" "]"
+end: "End" ("[" "]")?
 countinregion: "CountInRegion" "[" INT "," INT "," INT "," INT "]"
-detect: "Detect" "[" STRING ("," STRING)* "]" | "Detect" "[" "]"
+detect: "Detect" "[" STRING ("," STRING)* "]" | "Detect" ("[" "]")?
 segment: "Segment" "[" STRING "]"
 else: "Else"
 in: "IN" "[" STRING "]" EOL (INDENT expr+)*
 if: "IF" "[" (expr+)* "]" EOL (INDENT expr+)* (EOL | EOF | " ") (else EOL (INDENT expr+)* (EOL | EOF | " "))?
-tutorial: "Tutorial" "[" STRING "]"
+reset: "Reset" ("[" "]")?
+negate: "Not" "[" expr "]"
 OPERAND: "+" | "-" | "*" | "/"
-EQUALITY: "=="
+equality: (INT | STRING | expr) "==" (INT | STRING | expr)
+not_equality: (INT | STRING | expr) "!=" (INT | STRING | expr)
 train: "Train" "[" STRING "," STRING "]" | "Train" "[" STRING "]"
-label: "Label" "[" STRING "," STRING ("," STRING )*  "]" 
+label: "Label" "[" STRING "," STRING ("," STRING )*  "]"
+literal: /([a-z][a-zA-Z0-9_]*)/ ( "[" (STRING | INT | expr) ("," (STRING | INT | expr))* "]" )? | /([a-z][a-zA-Z0-9_]*)/ "[" "]"
 variable: /[a-zA-Z_][a-zA-Z0-9_]*/
 comment: "#"
 EOL: "\\n"
 EOF: "\\Z"
 INT: /-?\d+/
 INDENT: "    "
 BOOL: "True" | "False"
 %import common.ESCAPED_STRING -> STRING
 %import common.WS_INLINE
 %ignore WS_INLINE
-"""
+"""
```

### Comparing `visionscript-0.0.1/visionscript/usage.py` & `visionscript-0.0.2/visionscript/usage.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
 Find a church in the image and cut it out.
 
 Load["./abbey.jpg"]
 Detect["church"]
 Cutout[]
 Save["./abbey2.jpg"]
-"""
+"""
```

### Comparing `visionscript-0.0.1/visionscript.egg-info/PKG-INFO` & `visionscript-0.0.2/visionscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionscript
-Version: 0.0.1
+Version: 0.0.2
 Summary: VisionScript is an abstract programming language for doing common computer vision tasks, fast.
 Home-page: https://github.com/capjamesg/visionscript
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

