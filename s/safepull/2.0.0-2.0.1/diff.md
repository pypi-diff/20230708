# Comparing `tmp/safepull-2.0.0.tar.gz` & `tmp/safepull-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safepull-2.0.0.tar", last modified: Thu Jul  6 14:10:21 2023, max compression
+gzip compressed data, was "safepull-2.0.1.tar", last modified: Sat Jul  8 16:50:37 2023, max compression
```

## Comparing `safepull-2.0.0.tar` & `safepull-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:21.637467 safepull-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-06 14:10:07.000000 safepull-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-06 14:10:21.637467 safepull-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-06 14:10:07.000000 safepull-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-06 14:10:07.000000 safepull-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 14:10:21.637467 safepull-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:21.633467 safepull-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:21.637467 safepull-2.0.0/src/safepull/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:07.000000 safepull-2.0.0/src/safepull/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 14:10:07.000000 safepull-2.0.0/src/safepull/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-06 14:10:07.000000 safepull-2.0.0/src/safepull/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-06 14:10:07.000000 safepull-2.0.0/src/safepull/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-06 14:10:07.000000 safepull-2.0.0/src/safepull/safepull.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:21.637467 safepull-2.0.0/src/safepull.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 16:50:37.262974 safepull-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-08 16:50:28.000000 safepull-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-08 16:50:37.262974 safepull-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-08 16:50:28.000000 safepull-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-08 16:50:28.000000 safepull-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 16:50:37.262974 safepull-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 16:50:37.262974 safepull-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 16:50:37.262974 safepull-2.0.1/src/safepull/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 16:50:28.000000 safepull-2.0.1/src/safepull/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-08 16:50:28.000000 safepull-2.0.1/src/safepull/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-08 16:50:28.000000 safepull-2.0.1/src/safepull/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-08 16:50:28.000000 safepull-2.0.1/src/safepull/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-08 16:50:28.000000 safepull-2.0.1/src/safepull/safepull.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 16:50:37.262974 safepull-2.0.1/src/safepull.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-08 16:50:37.000000 safepull-2.0.1/src/safepull.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-08 16:50:37.000000 safepull-2.0.1/src/safepull.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 16:50:37.000000 safepull-2.0.1/src/safepull.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-08 16:50:37.000000 safepull-2.0.1/src/safepull.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 16:50:37.000000 safepull-2.0.1/src/safepull.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 16:50:37.000000 safepull-2.0.1/src/safepull.egg-info/top_level.txt
```

### Comparing `safepull-2.0.0/LICENSE` & `safepull-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safepull-2.0.0/PKG-INFO` & `safepull-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safepull
-Version: 2.0.0
+Version: 2.0.1
 Summary: A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py
 License: MIT
 Project-URL: repository, https://github.com/import-pandas-as-numpy/safepull/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `safepull-2.0.0/README.md` & `safepull-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `safepull-2.0.0/pyproject.toml` & `safepull-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [project]
 name = "safepull"
-version = "2.0.0"
+version = "2.0.1"
 description = "A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.10"
 dependencies = [
-    "requests~=2.28.2",
+    "requests>=2.28.2,<2.32.0",
     "rich~=13.4.2",
 ]
 
 [project.urls]
 repository = "https://github.com/import-pandas-as-numpy/safepull/"
 
 [project.scripts]
 safepull = "safepull.safepull:run"
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.ruff]
+target-version = "py311"
 select = ["ALL"]
+ignore = ["ANN101"]
```

### Comparing `safepull-2.0.0/src/safepull/exceptions.py` & `safepull-2.0.1/src/safepull/exceptions.py`

 * *Files identical despite different names*

### Comparing `safepull-2.0.0/src/safepull/models.py` & `safepull-2.0.1/src/safepull/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,20 +23,20 @@
         return cls(
             filename=releases["filename"],
             packagetype=releases["packagetype"],
             url=releases["url"],
             size=releases["size"],
         )
 
-    def download_package(self: Self) -> tuple[BytesIO, str]:
+    def download_package(self) -> tuple[BytesIO, str]:
         """Download a compressed package."""
         r = BytesIO(requests.get(self.url, stream=True, timeout=60).content)
         return r, self.filename
 
-    def get_metadata(self: Self) -> tuple[str, str, str, str]:
+    def get_metadata(self) -> tuple[str, str, str, str]:
         """Return the metadata for a specific distribution of a package."""
         return (
             f"Filename: {self.filename}",
             f"Package Type: {self.packagetype}",
             f"URL: {self.url}",
             f"Size: {self.size / (1 << 20):,.0f}MB",
         )
@@ -61,30 +61,30 @@
             author=package_dict["info"]["author"],
             version=package_dict["info"]["version"],
             distributions=[
                 Distribution.from_dict(releases) for releases in package_dict["urls"]
             ],
         )
 
-    def get_metadata(self: Self) -> tuple[str, str, str]:
+    def get_metadata(self) -> tuple[str, str, str]:
         """Return pertinent metadata for the package."""
         return f"{self.name} {self.version}", self.summary, f"Author: {self.author}"
 
-    def get_distributions(self: Self) -> list[Distribution]:
+    def get_distributions(self) -> list[Distribution]:
         """Return a list of distributions."""
         return self.distributions
 
-    def get_sdist(self: Self) -> Distribution | None:
+    def get_sdist(self) -> Distribution | None:
         """Extract the source distribution if it exists."""
         for distro in self.distributions:
             if distro.packagetype == "sdist":
                 return distro
         return None
 
-    def table_print(self: Self) -> Table:
+    def table_print(self) -> Table:
         """Rich table printing for distribution information."""
         table = Table(
             title=f"{self.name} v.{self.version}\nAuthor: {self.author}\n{self.summary}",
         )  # ruff: noqa: E501
         table.add_column("Index")
         table.add_column("Filename")
         table.add_column("Package Type")
```

### Comparing `safepull-2.0.0/src/safepull/safepull.py` & `safepull-2.0.1/src/safepull/safepull.py`

 * *Files identical despite different names*

### Comparing `safepull-2.0.0/src/safepull.egg-info/PKG-INFO` & `safepull-2.0.1/src/safepull.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safepull
-Version: 2.0.0
+Version: 2.0.1
 Summary: A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py
 License: MIT
 Project-URL: repository, https://github.com/import-pandas-as-numpy/safepull/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

