# Comparing `tmp/make_argocd_fly-0.0.7.tar.gz` & `tmp/make_argocd_fly-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make_argocd_fly-0.0.7.tar", last modified: Fri Jul  7 12:50:03 2023, max compression
+gzip compressed data, was "make_argocd_fly-0.0.8.tar", last modified: Sat Jul  8 19:42:39 2023, max compression
```

## Comparing `make_argocd_fly-0.0.7.tar` & `make_argocd_fly-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-07 12:50:03.265939 make_argocd_fly-0.0.7/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.7/LICENSE
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.7/MANIFEST.in
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     3715 2023-07-07 12:50:03.265939 make_argocd_fly-0.0.7/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     3361 2023-07-07 12:47:38.000000 make_argocd_fly-0.0.7/README.md
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-07 12:50:03.265939 make_argocd_fly-0.0.7/make_argocd_fly/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.7/make_argocd_fly/__init__.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      808 2023-07-07 12:36:36.000000 make_argocd_fly-0.0.7/make_argocd_fly/application.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.7/make_argocd_fly/config.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.7/make_argocd_fly/log_config.yml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5938 2023-07-07 10:19:53.000000 make_argocd_fly-0.0.7/make_argocd_fly/pipeline.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      688 2023-07-06 21:07:13.000000 make_argocd_fly-0.0.7/make_argocd_fly/renderer.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4255 2023-07-07 09:12:59.000000 make_argocd_fly-0.0.7/make_argocd_fly/resource.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      930 2023-07-06 18:44:06.000000 make_argocd_fly-0.0.7/make_argocd_fly/utils.py
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-07 12:50:03.265939 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     3715 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      522 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/SOURCES.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/dependency_links.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/entry_points.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/requires.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-07 12:50:03.000000 make_argocd_fly-0.0.7/make_argocd_fly.egg-info/top_level.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      724 2023-07-07 12:49:49.000000 make_argocd_fly-0.0.7/pyproject.toml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.7/requirements.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-07 12:50:03.265939 make_argocd_fly-0.0.7/setup.cfg
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-08 19:42:39.774965 make_argocd_fly-0.0.8/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.8/LICENSE
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.8/MANIFEST.in
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     3715 2023-07-08 19:42:39.774965 make_argocd_fly-0.0.8/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     3361 2023-07-07 12:47:38.000000 make_argocd_fly-0.0.8/README.md
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-08 19:42:39.774965 make_argocd_fly-0.0.8/make_argocd_fly/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.8/make_argocd_fly/__init__.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      808 2023-07-07 12:36:36.000000 make_argocd_fly-0.0.8/make_argocd_fly/application.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.8/make_argocd_fly/config.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.8/make_argocd_fly/log_config.yml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5940 2023-07-08 19:41:14.000000 make_argocd_fly-0.0.8/make_argocd_fly/pipeline.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      688 2023-07-06 21:07:13.000000 make_argocd_fly-0.0.8/make_argocd_fly/renderer.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4255 2023-07-07 09:12:59.000000 make_argocd_fly-0.0.8/make_argocd_fly/resource.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      930 2023-07-06 18:44:06.000000 make_argocd_fly-0.0.8/make_argocd_fly/utils.py
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-08 19:42:39.774965 make_argocd_fly-0.0.8/make_argocd_fly.egg-info/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     3715 2023-07-08 19:42:39.000000 make_argocd_fly-0.0.8/make_argocd_fly.egg-info/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      522 2023-07-08 19:42:39.000000 make_argocd_fly-0.0.8/make_argocd_fly.egg-info/SOURCES.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-08 19:42:39.000000 make_argocd_fly-0.0.8/make_argocd_fly.egg-info/dependency_links.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-08 19:42:39.000000 make_argocd_fly-0.0.8/make_argocd_fly.egg-info/entry_points.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-08 19:42:39.000000 make_argocd_fly-0.0.8/make_argocd_fly.egg-info/requires.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-08 19:42:39.000000 make_argocd_fly-0.0.8/make_argocd_fly.egg-info/top_level.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      724 2023-07-08 19:42:11.000000 make_argocd_fly-0.0.8/pyproject.toml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.8/requirements.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-08 19:42:39.774965 make_argocd_fly-0.0.8/setup.cfg
```

### Comparing `make_argocd_fly-0.0.7/LICENSE` & `make_argocd_fly-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.7/PKG-INFO` & `make_argocd_fly-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make_argocd_fly
-Version: 0.0.7
+Version: 0.0.8
 Summary: A project to generate ArgoCD application resources
 Author-email: Andrei Lapin <karandash8@gmail.com>
 License: GPLv3+
 Keywords: argocd,kustomize,jinja2
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `make_argocd_fly-0.0.7/README.md` & `make_argocd_fly-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.7/make_argocd_fly/application.py` & `make_argocd_fly-0.0.8/make_argocd_fly/application.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.7/make_argocd_fly/config.py` & `make_argocd_fly-0.0.8/make_argocd_fly/config.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.7/make_argocd_fly/pipeline.py` & `make_argocd_fly-0.0.8/make_argocd_fly/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
 # TODO: rework this nonsense
 def run(viewer: ResourceViewer, writer: ResourceWriter, config: Config) -> None:
   # write apps in a tmp dir and run kustomize
   for env_name, env_data in config.envs.items():
     if os.path.exists(config.config['tmp_dir']):
       shutil.rmtree(config.config['tmp_dir'])
-    tmp_writer = build_resource_writer(config.config['tmp_dir'], None)
 
     for app_name in env_data['apps'].keys():
       app = viewer.get_child(app_name)
       if not app:
         continue
 
+      tmp_writer = build_resource_writer(config.config['tmp_dir'], None)
       yml_children = app.get_files_children('.yml$')
       for yml_child in yml_children:
         dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
         for resource_kind, resource_name, resource_yml in multi_resource_parser(yml_child.content):
           tmp_writer.store_resource(dir_rel_path, resource_kind, resource_name, resource_yml)
       tmp_writer.write_resources()
```

### Comparing `make_argocd_fly-0.0.7/make_argocd_fly/renderer.py` & `make_argocd_fly-0.0.8/make_argocd_fly/renderer.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.7/make_argocd_fly/resource.py` & `make_argocd_fly-0.0.8/make_argocd_fly/resource.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.7/make_argocd_fly/utils.py` & `make_argocd_fly-0.0.8/make_argocd_fly/utils.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.7/make_argocd_fly.egg-info/PKG-INFO` & `make_argocd_fly-0.0.8/make_argocd_fly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make-argocd-fly
-Version: 0.0.7
+Version: 0.0.8
 Summary: A project to generate ArgoCD application resources
 Author-email: Andrei Lapin <karandash8@gmail.com>
 License: GPLv3+
 Keywords: argocd,kustomize,jinja2
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `make_argocd_fly-0.0.7/make_argocd_fly.egg-info/SOURCES.txt` & `make_argocd_fly-0.0.8/make_argocd_fly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.7/pyproject.toml` & `make_argocd_fly-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "make_argocd_fly"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     {name = "Andrei Lapin", email = "karandash8@gmail.com"},
 ]
 description = "A project to generate ArgoCD application resources"
 requires-python = ">=3.10"
 keywords = ["argocd", "kustomize", "jinja2"]
 license = {text = "GPLv3+"}
```

