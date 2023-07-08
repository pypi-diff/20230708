# Comparing `tmp/nginx-static-analysis-0.2.6.tar.gz` & `tmp/nginx-static-analysis-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-static-analysis-0.2.6.tar", last modified: Thu Jan 12 20:38:00 2023, max compression
+gzip compressed data, was "nginx-static-analysis-0.2.8.tar", last modified: Sat Jul  8 08:29:55 2023, max compression
```

## Comparing `nginx-static-analysis-0.2.6.tar` & `nginx-static-analysis-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:38:00.024218 nginx-static-analysis-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-01-12 20:38:00.024218 nginx-static-analysis-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:38:00.020218 nginx-static-analysis-0.2.6/nginx_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/nginx_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/nginx_analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/nginx_analysis/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/nginx_analysis/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/nginx_analysis/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/nginx_analysis/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/nginx_analysis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/nginx_analysis/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:38:00.024218 nginx-static-analysis-0.2.6/nginx_static_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-01-12 20:37:59.000000 nginx-static-analysis-0.2.6/nginx_static_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-12 20:38:00.000000 nginx-static-analysis-0.2.6/nginx_static_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 20:37:59.000000 nginx-static-analysis-0.2.6/nginx_static_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-12 20:37:59.000000 nginx-static-analysis-0.2.6/nginx_static_analysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-12 20:37:59.000000 nginx-static-analysis-0.2.6/nginx_static_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-12 20:37:59.000000 nginx-static-analysis-0.2.6/nginx_static_analysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-12 20:38:00.024218 nginx-static-analysis-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-12 20:37:56.000000 nginx-static-analysis-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:29:55.073852 nginx-static-analysis-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-08 08:29:55.073852 nginx-static-analysis-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:29:55.073852 nginx-static-analysis-0.2.8/nginx_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:29:55.073852 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-08 08:29:55.073852 nginx-static-analysis-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/setup.py
```

### Comparing `nginx-static-analysis-0.2.6/LICENSE` & `nginx-static-analysis-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.6/PKG-INFO` & `nginx-static-analysis-0.2.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: nginx-static-analysis
-Version: 0.2.6
-Summary: Parse Nginx configurations in a clear manner for debugging purposes
-Home-page: https://github.com/AlexanderGrooff/nginx-static-analysis
-Author: Alexander Grooff
-Author-email: alexandergrooff@gmail.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Nginx Static Analysis
 
 [![nginx-static-analysis](https://img.shields.io/pypi/v/nginx-static-analysis)](https://pypi.org/project/nginx-static-analysis/)
 
 Parse Nginx configurations on your host and filter for directives/values.
 
 Largely powered by [Crossplane](https://github.com/nginxinc/crossplane).
@@ -85,7 +74,26 @@
 | /etc/nginx/sites/http.testalex.hypernode.io.conf:8 |   /    |            server -> location            |
 |            /etc/nginx/magento2.conf:17             |   /    | server -> include -> include -> location |
 +----------------------------------------------------+--------+------------------------------------------+
 ```
 
 The analysis creates filters based on the incoming loglines. Those filters are combined with the arguments given
 to the `nginx-static-analysis` command.
+
+## Development
+
+This package is using Python >=3.7. Simply `pip install -r requirements/base.txt` into your local venv to install the dependencies.
+
+### Testing
+
+This package uses `pytest` for testing. You can run the tests with `pytest`, which will invoke an Nginx container with some sample configs.
+If not present, it'll be built automatically.
+
+### Build
+
+This package can be build locally:
+
+```bash
+# Arch
+pip install -r requirements/development.txt
+makepkg -sCf  # Include -i to install the package locally
+```
```

### Comparing `nginx-static-analysis-0.2.6/nginx_analysis/analysis.py` & `nginx-static-analysis-0.2.8/nginx_analysis/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterator, List, Optional, Set, Tuple
+from typing import Iterator, List, Optional, Set, Tuple, Union
 
 import crossplane
 from loguru import logger
 
 from nginx_analysis.dataclasses import (
     DirectiveFilter,
     NginxLineConfig,
@@ -202,20 +202,23 @@
         matching_lines.extend(get_children_recursive(neighbour))
     parents = get_parents_recursive(match)
     matching_lines.extend(parents)
     return matching_lines
 
 
 def filter_config(
-    lines: Iterator[NginxLineConfig],
+    lines: Union[List[NginxLineConfig], Iterator[NginxLineConfig]],
     filters: List[DirectiveFilter],
 ) -> List[NginxLineConfig]:
     """
     Find all values for the given directive name in the root config
     """
+    if not filters:
+        return sort_by_depth(filter_unique(lines))
+
     matching_lines = []
     for line in lines:
         child_matches, _ = get_matching_lines_in_children(line, filters)
         matching_lines.extend(child_matches)
         for match in child_matches:
             matching_lines.extend(expand_upon_direct_match(match, filters))
```

### Comparing `nginx-static-analysis-0.2.6/nginx_analysis/dataclasses.py` & `nginx-static-analysis-0.2.8/nginx_analysis/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import re
 from pathlib import Path
-from typing import Any, Generator, List, Optional, Tuple, TypeVar
+from typing import Any, Generator, Iterator, List, Optional, Tuple, TypeVar, Union
 
 from pydantic import BaseModel
 
 T = TypeVar("T")
 
 
 def compare_objects(this: T, that: T, fields: List[str]) -> bool:
     for field in fields:
         if not getattr(this, field) == getattr(that, field):
             return False
     return True
 
 
-def filter_unique(line_configs: List["NginxLineConfig"]) -> List["NginxLineConfig"]:
+def filter_unique(
+    line_configs: Union[List["NginxLineConfig"], Iterator["NginxLineConfig"]]
+) -> List["NginxLineConfig"]:
     """
     Filter out lines that are already covered by a parent.
     """
     return list(set(line_configs))
 
 
 def get_children_recursive(line_config: "NginxLineConfig") -> List["NginxLineConfig"]:
```

### Comparing `nginx-static-analysis-0.2.6/nginx_analysis/filter.py` & `nginx-static-analysis-0.2.8/nginx_analysis/filter.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.6/nginx_analysis/input.py` & `nginx-static-analysis-0.2.8/nginx_analysis/input.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.6/nginx_analysis/log.py` & `nginx-static-analysis-0.2.8/nginx_analysis/log.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.6/nginx_analysis/main.py` & `nginx-static-analysis-0.2.8/nginx_analysis/main.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.6/nginx_analysis/output.py` & `nginx-static-analysis-0.2.8/nginx_analysis/output.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.6/nginx_static_analysis.egg-info/SOURCES.txt` & `nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.6/setup.py` & `nginx-static-analysis-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 loguru==0.5.3
 prettytable==2.5.0
 """
 
 
 setup(
     name="nginx-static-analysis",
-    version="0.2.6",
+    version="0.2.8",
     description="Parse Nginx configurations in a clear manner for debugging purposes",
     url="https://github.com/AlexanderGrooff/nginx-static-analysis",
     packages=find_packages(
         include=["nginx_analysis", "requirements/base.txt"], exclude=["tests"]
     ),
     author="Alexander Grooff",
     author_email="alexandergrooff@gmail.com",
```

