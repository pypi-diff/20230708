# Comparing `tmp/changelog2version-0.8.0.tar.gz` & `tmp/changelog2version-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelog2version-0.8.0.tar", last modified: Fri Nov 11 14:36:06 2022, max compression
+gzip compressed data, was "changelog2version-0.9.0.tar", last modified: Sat Nov 12 09:04:44 2022, max compression
```

## Comparing `changelog2version-0.8.0.tar` & `changelog2version-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:36:06.391912 changelog2version-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-11-11 14:35:47.000000 changelog2version-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9775 2022-11-11 14:36:06.391912 changelog2version-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-11-11 14:35:47.000000 changelog2version-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-11 14:35:47.000000 changelog2version-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-11 14:36:06.391912 changelog2version-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     9011 2022-11-11 14:35:47.000000 changelog2version-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:36:06.391912 changelog2version-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:36:06.391912 changelog2version-0.8.0/src/changelog2version/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-11 14:35:47.000000 changelog2version-0.8.0/src/changelog2version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12015 2022-11-11 14:35:47.000000 changelog2version-0.8.0/src/changelog2version/extract_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5288 2022-11-11 14:35:47.000000 changelog2version-0.8.0/src/changelog2version/render_version_file.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:36:06.391912 changelog2version-0.8.0/src/changelog2version/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-11-11 14:35:47.000000 changelog2version-0.8.0/src/changelog2version/templates/version.h.template
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-11 14:35:47.000000 changelog2version-0.8.0/src/changelog2version/templates/version.py.template
--rw-r--r--   0 runner    (1001) docker     (121)    10308 2022-11-11 14:35:47.000000 changelog2version-0.8.0/src/changelog2version/update_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-11 14:35:59.000000 changelog2version-0.8.0/src/changelog2version/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:36:06.391912 changelog2version-0.8.0/src/changelog2version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9775 2022-11-11 14:36:06.000000 changelog2version-0.8.0/src/changelog2version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-11 14:36:06.000000 changelog2version-0.8.0/src/changelog2version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 14:36:06.000000 changelog2version-0.8.0/src/changelog2version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-11 14:36:06.000000 changelog2version-0.8.0/src/changelog2version.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-11 14:36:06.000000 changelog2version-0.8.0/src/changelog2version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-11 14:36:06.000000 changelog2version-0.8.0/src/changelog2version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:04:44.613020 changelog2version-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-11-12 09:04:25.000000 changelog2version-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11701 2022-11-12 09:04:44.613020 changelog2version-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10566 2022-11-12 09:04:25.000000 changelog2version-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-12 09:04:25.000000 changelog2version-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-12 09:04:44.617020 changelog2version-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     9011 2022-11-12 09:04:25.000000 changelog2version-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:04:44.613020 changelog2version-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:04:44.613020 changelog2version-0.9.0/src/changelog2version/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-12 09:04:25.000000 changelog2version-0.9.0/src/changelog2version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12015 2022-11-12 09:04:25.000000 changelog2version-0.9.0/src/changelog2version/extract_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5288 2022-11-12 09:04:25.000000 changelog2version-0.9.0/src/changelog2version/render_version_file.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:04:44.613020 changelog2version-0.9.0/src/changelog2version/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-11-12 09:04:25.000000 changelog2version-0.9.0/src/changelog2version/templates/version.h.template
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-12 09:04:25.000000 changelog2version-0.9.0/src/changelog2version/templates/version.py.template
+-rw-r--r--   0 runner    (1001) docker     (121)    11082 2022-11-12 09:04:25.000000 changelog2version-0.9.0/src/changelog2version/update_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-12 09:04:38.000000 changelog2version-0.9.0/src/changelog2version/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 09:04:44.613020 changelog2version-0.9.0/src/changelog2version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11701 2022-11-12 09:04:44.000000 changelog2version-0.9.0/src/changelog2version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-12 09:04:44.000000 changelog2version-0.9.0/src/changelog2version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 09:04:44.000000 changelog2version-0.9.0/src/changelog2version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-12 09:04:44.000000 changelog2version-0.9.0/src/changelog2version.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-12 09:04:44.000000 changelog2version-0.9.0/src/changelog2version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-12 09:04:44.000000 changelog2version-0.9.0/src/changelog2version.egg-info/top_level.txt
```

### Comparing `changelog2version-0.8.0/LICENSE.txt` & `changelog2version-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `changelog2version-0.8.0/PKG-INFO` & `changelog2version-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog2version
-Version: 0.8.0
+Version: 0.9.0
 Summary: Update version info file with latest changelog version entry
 Home-page: https://github.com/brainelectronics/changelog2version
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Project-URL: Bug Reports, https://github.com/brainelectronics/changelog2version/issues
 Project-URL: Source, https://github.com/brainelectronics/changelog2version/
 Keywords: changelog,version,changelog-parser,versioning,extract
@@ -147,15 +147,39 @@
 changelog2version \
     --changelog_file changelog.md \
     --print \
     --debug
 ```
 
 ```json
-{"info": {"version": "0.6.0"}, "releases": {"0.6.0": [{"upload_time": "2022-10-26"}], "0.5.0": [{"upload_time": "2022-10-20"}], "0.4.0": [{"upload_time": "2022-08-07"}], "0.3.0": [{"upload_time": "2022-08-05"}], "0.2.0": [{"upload_time": "2022-08-03"}], "0.1.1": [{"upload_time": "2022-07-31"}], "0.1.0": [{"upload_time": "2022-07-31"}]}}
+{"info": {"version": "0.7.0", "description": "### Added\n- Changelog parsed as JSON contains a new key `description` like the PyPi package JSON info, compare to `https://pypi.org/pypi/changelog2version/json`, with the description/content of the latest change, see #19, relates to #18\n- Increase unittest coverage above 95%\n\n### Changed\n- Line breaks are no longer used in this changelog for enumerations\n- Issues are referenced as `#123` instead of `[#123][ref-issue-123]` to avoid explicit references at the bottom or some other location in the file\n- Output of `changelog2version` call with `--print` but without `--debug` option is JSON compatible\n"}, "releases": {"0.7.0": [{"upload_time": "2022-11-11"}], "0.6.0": [{"upload_time": "2022-10-26"}], "0.5.0": [{"upload_time": "2022-10-20"}], "0.4.0": [{"upload_time": "2022-08-07"}], "0.3.0": [{"upload_time": "2022-08-05"}], "0.2.0": [{"upload_time": "2022-08-03"}], "0.1.1": [{"upload_time": "2022-07-31"}], "0.1.0": [{"upload_time": "2022-07-31"}]}}
+```
+
+To get the latest version and description in the console as environment
+variables use the following call
+
+```bash
+LATEST_VERSION=$(changelog2version --changelog_file changelog.md --print | python -c "import sys, json; print(json.load(sys.stdin)['info']['version'])")
+LATEST_CHANGE=$(changelog2version --changelog_file changelog.md --print | python -c "import sys, json; print(json.load(sys.stdin)['info']['description'])")
+
+echo "The latest version extracted from the changelog is ${LATEST_VERSION}"
+# The latest version extracted from the changelog is 0.7.0
+
+echo "Description of the latest change"
+echo "${LATEST_CHANGE}"
+# ### Added
+# - Changelog parsed as JSON contains a new key `description` like the PyPi package JSON info, compare to `https://pyp
+# i.org/pypi/changelog2version/json`, with the description/content of the latest change, see #19, relates to #18
+# - Increase unittest coverage above 95%
+
+# ### Changed
+# - Line breaks are no longer used in this changelog for enumerations
+# - Issues are referenced as `#123` instead of `[#123][ref-issue-123]` to avoid explicit references at the bottom or s
+# ome other location in the file
+# - Output of `changelog2version` call with `--print` but without `--debug` option is JSON compatible
 ```
 
 ##### File
 
 ```bash
 changelog2version \
     --changelog_file changelog.md \
```

### Comparing `changelog2version-0.8.0/README.md` & `changelog2version-0.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -121,15 +121,39 @@
 changelog2version \
     --changelog_file changelog.md \
     --print \
     --debug
 ```
 
 ```json
-{"info": {"version": "0.6.0"}, "releases": {"0.6.0": [{"upload_time": "2022-10-26"}], "0.5.0": [{"upload_time": "2022-10-20"}], "0.4.0": [{"upload_time": "2022-08-07"}], "0.3.0": [{"upload_time": "2022-08-05"}], "0.2.0": [{"upload_time": "2022-08-03"}], "0.1.1": [{"upload_time": "2022-07-31"}], "0.1.0": [{"upload_time": "2022-07-31"}]}}
+{"info": {"version": "0.7.0", "description": "### Added\n- Changelog parsed as JSON contains a new key `description` like the PyPi package JSON info, compare to `https://pypi.org/pypi/changelog2version/json`, with the description/content of the latest change, see #19, relates to #18\n- Increase unittest coverage above 95%\n\n### Changed\n- Line breaks are no longer used in this changelog for enumerations\n- Issues are referenced as `#123` instead of `[#123][ref-issue-123]` to avoid explicit references at the bottom or some other location in the file\n- Output of `changelog2version` call with `--print` but without `--debug` option is JSON compatible\n"}, "releases": {"0.7.0": [{"upload_time": "2022-11-11"}], "0.6.0": [{"upload_time": "2022-10-26"}], "0.5.0": [{"upload_time": "2022-10-20"}], "0.4.0": [{"upload_time": "2022-08-07"}], "0.3.0": [{"upload_time": "2022-08-05"}], "0.2.0": [{"upload_time": "2022-08-03"}], "0.1.1": [{"upload_time": "2022-07-31"}], "0.1.0": [{"upload_time": "2022-07-31"}]}}
+```
+
+To get the latest version and description in the console as environment
+variables use the following call
+
+```bash
+LATEST_VERSION=$(changelog2version --changelog_file changelog.md --print | python -c "import sys, json; print(json.load(sys.stdin)['info']['version'])")
+LATEST_CHANGE=$(changelog2version --changelog_file changelog.md --print | python -c "import sys, json; print(json.load(sys.stdin)['info']['description'])")
+
+echo "The latest version extracted from the changelog is ${LATEST_VERSION}"
+# The latest version extracted from the changelog is 0.7.0
+
+echo "Description of the latest change"
+echo "${LATEST_CHANGE}"
+# ### Added
+# - Changelog parsed as JSON contains a new key `description` like the PyPi package JSON info, compare to `https://pyp
+# i.org/pypi/changelog2version/json`, with the description/content of the latest change, see #19, relates to #18
+# - Increase unittest coverage above 95%
+
+# ### Changed
+# - Line breaks are no longer used in this changelog for enumerations
+# - Issues are referenced as `#123` instead of `[#123][ref-issue-123]` to avoid explicit references at the bottom or s
+# ome other location in the file
+# - Output of `changelog2version` call with `--print` but without `--debug` option is JSON compatible
 ```
 
 ##### File
 
 ```bash
 changelog2version \
     --changelog_file changelog.md \
```

### Comparing `changelog2version-0.8.0/setup.py` & `changelog2version-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `changelog2version-0.8.0/src/changelog2version/extract_version.py` & `changelog2version-0.9.0/src/changelog2version/extract_version.py`

 * *Files identical despite different names*

### Comparing `changelog2version-0.8.0/src/changelog2version/render_version_file.py` & `changelog2version-0.9.0/src/changelog2version/render_version_file.py`

 * *Files identical despite different names*

### Comparing `changelog2version-0.8.0/src/changelog2version/update_version.py` & `changelog2version-0.9.0/src/changelog2version/update_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from pathlib import Path
 import re
 import semver
 from sys import stdout
 
 from .extract_version import ExtractVersion
 from .render_version_file import RenderVersionFile
+from .version import __version__
 
 
 def parser_valid_file(parser: argparse.ArgumentParser, arg: str) -> Path:
     """
     Determine whether file exists.
     :param      parser:                 The parser
     :type       parser:                 parser object
@@ -77,14 +78,24 @@
     Update version info file based on changelog entry
     """, formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     # default arguments
     parser.add_argument('-d', '--debug',
                         action='store_true',
                         help='Output logger messages to stderr')
+    parser.add_argument('-v',
+                        default=0,
+                        action='count',
+                        dest='verbosity',
+                        help='Set level of verbosity, default is CRITICAL')
+    parser.add_argument('--version',
+                        action='version',
+                        version='%(prog)s {version}'.
+                                format(version=__version__),
+                        help="Print version of package and exit")
 
     # specific arguments
     parser.add_argument('--changelog_file',
                         dest='changelog_file',
                         required=True,
                         type=lambda x: parser_valid_file(parser, x),
                         help='Path to changelog file')
@@ -155,22 +166,30 @@
     return parsed_args
 
 
 def main():
     # parse CLI arguments
     args = parse_arguments()
 
+    log_levels = {
+        0: logging.CRITICAL,
+        1: logging.ERROR,
+        2: logging.WARNING,
+        3: logging.INFO,
+        4: logging.DEBUG,
+    }
     custom_format = '[%(asctime)s] [%(levelname)-8s] [%(filename)-15s @'\
                     ' %(funcName)-15s:%(lineno)4s] %(message)s'
     logging.basicConfig(level=logging.INFO,
                         format=custom_format,
                         stream=stdout)
     logger = logging.getLogger(__name__)
-    if args.debug:
-        logger.setLevel(logging.DEBUG)
+    logger.setLevel(level=log_levels[min(args.verbosity,
+                                     max(log_levels.keys()))])
+    logger.disabled = not args.debug
 
     # changelog_file = Path(args.changelog_file).resolve()
     changelog_file = args.changelog_file
     version_file = None
     template_file = args.template_file
     version_file_type = args.version_file_type
     additional_template_data = args.additional_template_data
```

### Comparing `changelog2version-0.8.0/src/changelog2version.egg-info/PKG-INFO` & `changelog2version-0.9.0/src/changelog2version.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog2version
-Version: 0.8.0
+Version: 0.9.0
 Summary: Update version info file with latest changelog version entry
 Home-page: https://github.com/brainelectronics/changelog2version
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Project-URL: Bug Reports, https://github.com/brainelectronics/changelog2version/issues
 Project-URL: Source, https://github.com/brainelectronics/changelog2version/
 Keywords: changelog,version,changelog-parser,versioning,extract
@@ -147,15 +147,39 @@
 changelog2version \
     --changelog_file changelog.md \
     --print \
     --debug
 ```
 
 ```json
-{"info": {"version": "0.6.0"}, "releases": {"0.6.0": [{"upload_time": "2022-10-26"}], "0.5.0": [{"upload_time": "2022-10-20"}], "0.4.0": [{"upload_time": "2022-08-07"}], "0.3.0": [{"upload_time": "2022-08-05"}], "0.2.0": [{"upload_time": "2022-08-03"}], "0.1.1": [{"upload_time": "2022-07-31"}], "0.1.0": [{"upload_time": "2022-07-31"}]}}
+{"info": {"version": "0.7.0", "description": "### Added\n- Changelog parsed as JSON contains a new key `description` like the PyPi package JSON info, compare to `https://pypi.org/pypi/changelog2version/json`, with the description/content of the latest change, see #19, relates to #18\n- Increase unittest coverage above 95%\n\n### Changed\n- Line breaks are no longer used in this changelog for enumerations\n- Issues are referenced as `#123` instead of `[#123][ref-issue-123]` to avoid explicit references at the bottom or some other location in the file\n- Output of `changelog2version` call with `--print` but without `--debug` option is JSON compatible\n"}, "releases": {"0.7.0": [{"upload_time": "2022-11-11"}], "0.6.0": [{"upload_time": "2022-10-26"}], "0.5.0": [{"upload_time": "2022-10-20"}], "0.4.0": [{"upload_time": "2022-08-07"}], "0.3.0": [{"upload_time": "2022-08-05"}], "0.2.0": [{"upload_time": "2022-08-03"}], "0.1.1": [{"upload_time": "2022-07-31"}], "0.1.0": [{"upload_time": "2022-07-31"}]}}
+```
+
+To get the latest version and description in the console as environment
+variables use the following call
+
+```bash
+LATEST_VERSION=$(changelog2version --changelog_file changelog.md --print | python -c "import sys, json; print(json.load(sys.stdin)['info']['version'])")
+LATEST_CHANGE=$(changelog2version --changelog_file changelog.md --print | python -c "import sys, json; print(json.load(sys.stdin)['info']['description'])")
+
+echo "The latest version extracted from the changelog is ${LATEST_VERSION}"
+# The latest version extracted from the changelog is 0.7.0
+
+echo "Description of the latest change"
+echo "${LATEST_CHANGE}"
+# ### Added
+# - Changelog parsed as JSON contains a new key `description` like the PyPi package JSON info, compare to `https://pyp
+# i.org/pypi/changelog2version/json`, with the description/content of the latest change, see #19, relates to #18
+# - Increase unittest coverage above 95%
+
+# ### Changed
+# - Line breaks are no longer used in this changelog for enumerations
+# - Issues are referenced as `#123` instead of `[#123][ref-issue-123]` to avoid explicit references at the bottom or s
+# ome other location in the file
+# - Output of `changelog2version` call with `--print` but without `--debug` option is JSON compatible
 ```
 
 ##### File
 
 ```bash
 changelog2version \
     --changelog_file changelog.md \
```

### Comparing `changelog2version-0.8.0/src/changelog2version.egg-info/SOURCES.txt` & `changelog2version-0.9.0/src/changelog2version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

