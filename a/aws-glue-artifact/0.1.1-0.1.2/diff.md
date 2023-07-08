# Comparing `tmp/aws_glue_artifact-0.1.1.tar.gz` & `tmp/aws_glue_artifact-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_glue_artifact-0.1.1.tar", last modified: Fri Jul  7 19:18:58 2023, max compression
+gzip compressed data, was "aws_glue_artifact-0.1.2.tar", last modified: Sat Jul  8 20:24:07 2023, max compression
```

## Comparing `aws_glue_artifact-0.1.1.tar` & `aws_glue_artifact-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 19:18:58.457310 aws_glue_artifact-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1128 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      325 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4685 2023-07-07 19:18:58.457191 aws_glue_artifact-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3479 2023-07-07 19:17:05.000000 aws_glue_artifact-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 19:18:58.454722 aws_glue_artifact-0.1.1/aws_glue_artifact/
--rw-r--r--   0 sanhehu    (501) staff       (20)      529 2023-07-07 19:15:03.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      107 2023-07-07 19:10:51.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 19:18:58.455429 aws_glue_artifact-0.1.1/aws_glue_artifact/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6899 2023-07-07 19:11:54.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/model.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 19:18:58.455828 aws_glue_artifact-0.1.1/aws_glue_artifact/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 19:18:58.456610 aws_glue_artifact-0.1.1/aws_glue_artifact/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3006 2023-07-07 15:19:11.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/vendor/build.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7590 2023-07-05 12:53:46.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/aws_glue_artifact/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 19:18:58.455310 aws_glue_artifact-0.1.1/aws_glue_artifact.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4685 2023-07-07 19:18:58.000000 aws_glue_artifact-0.1.1/aws_glue_artifact.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      858 2023-07-07 19:18:58.000000 aws_glue_artifact-0.1.1/aws_glue_artifact.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-07 19:18:58.000000 aws_glue_artifact-0.1.1/aws_glue_artifact.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      203 2023-07-07 19:18:58.000000 aws_glue_artifact-0.1.1/aws_glue_artifact.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       18 2023-07-07 19:18:58.000000 aws_glue_artifact-0.1.1/aws_glue_artifact.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      601 2023-07-07 19:16:02.000000 aws_glue_artifact-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-07 15:40:31.000000 aws_glue_artifact-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       84 2023-07-07 18:17:43.000000 aws_glue_artifact-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-07 19:18:58.457347 aws_glue_artifact-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7566 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-07 19:18:58.456934 aws_glue_artifact-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      303 2023-07-07 19:16:06.000000 aws_glue_artifact-0.1.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2166 2023-07-07 19:12:16.000000 aws_glue_artifact-0.1.1/tests/test_model.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-08 20:24:07.910154 aws_glue_artifact-0.1.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1128 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      325 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4685 2023-07-08 20:24:07.910002 aws_glue_artifact-0.1.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3479 2023-07-07 19:17:05.000000 aws_glue_artifact-0.1.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-08 20:24:07.907216 aws_glue_artifact-0.1.2/aws_glue_artifact/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      529 2023-07-07 19:15:03.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-08 20:12:31.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      107 2023-07-07 19:10:51.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-08 20:24:07.907922 aws_glue_artifact-0.1.2/aws_glue_artifact/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7434 2023-07-08 20:23:15.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/model.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-08 20:24:07.908254 aws_glue_artifact-0.1.2/aws_glue_artifact/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-08 20:24:07.909362 aws_glue_artifact-0.1.2/aws_glue_artifact/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3006 2023-07-07 15:19:11.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/vendor/build.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7590 2023-07-05 12:53:46.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/aws_glue_artifact/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-08 20:24:07.907804 aws_glue_artifact-0.1.2/aws_glue_artifact.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4685 2023-07-08 20:24:07.000000 aws_glue_artifact-0.1.2/aws_glue_artifact.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      858 2023-07-08 20:24:07.000000 aws_glue_artifact-0.1.2/aws_glue_artifact.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-08 20:24:07.000000 aws_glue_artifact-0.1.2/aws_glue_artifact.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      203 2023-07-08 20:24:07.000000 aws_glue_artifact-0.1.2/aws_glue_artifact.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       18 2023-07-08 20:24:07.000000 aws_glue_artifact-0.1.2/aws_glue_artifact.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      826 2023-07-08 20:22:14.000000 aws_glue_artifact-0.1.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-07 15:40:31.000000 aws_glue_artifact-0.1.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       84 2023-07-07 18:17:43.000000 aws_glue_artifact-0.1.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-08 20:24:07.910201 aws_glue_artifact-0.1.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7566 2023-07-07 14:00:49.000000 aws_glue_artifact-0.1.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-08 20:24:07.909790 aws_glue_artifact-0.1.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      303 2023-07-07 19:16:06.000000 aws_glue_artifact-0.1.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2166 2023-07-07 19:12:16.000000 aws_glue_artifact-0.1.2/tests/test_model.py
```

### Comparing `aws_glue_artifact-0.1.1/AUTHORS.rst` & `aws_glue_artifact-0.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/LICENSE.txt` & `aws_glue_artifact-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/PKG-INFO` & `aws_glue_artifact-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_glue_artifact
-Version: 0.1.1
+Version: 0.1.2
 Summary: AWS Glue Artifact versioning and alias Management for blue/green, canary deployment, and roll back for production failure.
 Home-page: https://github.com/MacHu-GWU/aws_glue_artifact-project
-Download-URL: https://pypi.python.org/pypi/aws_glue_artifact/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_glue_artifact/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `aws_glue_artifact-0.1.1/README.rst` & `aws_glue_artifact-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/aws_glue_artifact/__init__.py` & `aws_glue_artifact-0.1.2/aws_glue_artifact/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/aws_glue_artifact/model.py` & `aws_glue_artifact-0.1.2/aws_glue_artifact/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -154,19 +154,32 @@
 
     def __post_init__(self):
         self.dir_glue_python_lib = Path(self.dir_glue_python_lib).absolute()
         self.dir_glue_build = Path(self.dir_glue_build).absolute()
         self._common_post_init(suffix=".zip")
 
     @property
+    def dir_glue_build_temp(self) -> Path:
+        """
+        example: ``${dir_glue_build}/tmp/``
+        """
+        return self.dir_glue_build.joinpath("tmp")
+
+    @property
     def dir_glue_python_lib_build(self) -> Path:
-        return self.dir_glue_build.joinpath(self.dir_glue_python_lib.basename)
+        """
+        example: ``${dir_glue_build}/tmp/${glue_python_lib}/``
+        """
+        return self.dir_glue_build_temp.joinpath(self.dir_glue_python_lib.basename)
 
     @property
     def path_glue_python_lib_build_zip(self) -> Path:
+        """
+        example: ``${dir_glue_build}/${glue_python_lib}.zip``
+        """
         return self.dir_glue_build.joinpath(f"{self.dir_glue_python_lib.basename}.zip")
 
     def put_artifact(
         self,
         metadata: T.Dict[str, str] = NOTHING,
         tags: T.Dict[str, str] = NOTHING,
     ) -> Artifact:
@@ -178,15 +191,18 @@
         """
         self.dir_glue_build.remove_if_exists()
         self.dir_glue_build.mkdir_if_not_exists()
         build_python_lib(
             dir_python_lib_source=self.dir_glue_python_lib,
             dir_python_lib_target=self.dir_glue_python_lib_build,
         )
-        self.dir_glue_python_lib_build.make_zip_archive(
+        self.dir_glue_build_temp.joinpath("aws-glue-artifact.txt").write_text(
+            "built by aws-glue-artifact: https://github.com/MacHu-GWU/aws_glue_artifact-project"
+        )
+        self.dir_glue_build_temp.make_zip_archive(
             dst=self.path_glue_python_lib_build_zip,
             include_dir=False,
         )
         glue_python_lib_sha256 = hashes.of_paths(paths=[self.dir_glue_python_lib_build])
         final_metadata = {
             "glue_python_lib_sha256": glue_python_lib_sha256,
         }
```

### Comparing `aws_glue_artifact-0.1.1/aws_glue_artifact/paths.py` & `aws_glue_artifact-0.1.2/aws_glue_artifact/paths.py`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/aws_glue_artifact/tests/mock_aws.py` & `aws_glue_artifact-0.1.2/aws_glue_artifact/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/aws_glue_artifact/vendor/build.py` & `aws_glue_artifact-0.1.2/aws_glue_artifact/vendor/build.py`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/aws_glue_artifact/vendor/hashes.py` & `aws_glue_artifact-0.1.2/aws_glue_artifact/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/aws_glue_artifact/vendor/pytest_cov_helper.py` & `aws_glue_artifact-0.1.2/aws_glue_artifact/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/aws_glue_artifact.egg-info/PKG-INFO` & `aws_glue_artifact-0.1.2/aws_glue_artifact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-glue-artifact
-Version: 0.1.1
+Version: 0.1.2
 Summary: AWS Glue Artifact versioning and alias Management for blue/green, canary deployment, and roll back for production failure.
 Home-page: https://github.com/MacHu-GWU/aws_glue_artifact-project
-Download-URL: https://pypi.python.org/pypi/aws_glue_artifact/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_glue_artifact/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `aws_glue_artifact-0.1.1/aws_glue_artifact.egg-info/SOURCES.txt` & `aws_glue_artifact-0.1.2/aws_glue_artifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/requirements-doc.txt` & `aws_glue_artifact-0.1.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/setup.py` & `aws_glue_artifact-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `aws_glue_artifact-0.1.1/tests/test_model.py` & `aws_glue_artifact-0.1.2/tests/test_model.py`

 * *Files identical despite different names*

