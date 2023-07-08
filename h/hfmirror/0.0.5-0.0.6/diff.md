# Comparing `tmp/hfmirror-0.0.5.tar.gz` & `tmp/hfmirror-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfmirror-0.0.5.tar", last modified: Mon May  8 11:17:56 2023, max compression
+gzip compressed data, was "hfmirror-0.0.6.tar", last modified: Sat Jul  8 15:02:24 2023, max compression
```

## Comparing `hfmirror-0.0.5.tar` & `hfmirror-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 11:17:22.000000 hfmirror-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 11:17:22.000000 hfmirror-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-08 11:17:56.348106 hfmirror-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-08 11:17:22.000000 hfmirror-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.344106 hfmirror-0.0.5/hfmirror/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/sourceforge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/storage/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/storage/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror/sync/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-08 11:17:56.000000 hfmirror-0.0.5/hfmirror.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-08 11:17:56.000000 hfmirror-0.0.5/hfmirror.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:17:56.000000 hfmirror-0.0.5/hfmirror.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 11:17:56.000000 hfmirror-0.0.5/hfmirror.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 11:17:56.000000 hfmirror-0.0.5/hfmirror.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-08 11:17:22.000000 hfmirror-0.0.5/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 11:17:22.000000 hfmirror-0.0.5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-08 11:17:22.000000 hfmirror-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:17:56.348106 hfmirror-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-08 11:17:22.000000 hfmirror-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:02:24.503412 hfmirror-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 15:01:48.000000 hfmirror-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-08 15:01:48.000000 hfmirror-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-08 15:02:24.503412 hfmirror-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-07-08 15:01:48.000000 hfmirror-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:02:24.499412 hfmirror-0.0.6/hfmirror/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:02:24.499412 hfmirror-0.0.6/hfmirror/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:02:24.499412 hfmirror-0.0.6/hfmirror/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/resource/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/resource/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/resource/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/resource/sourceforge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/resource/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:02:24.503412 hfmirror-0.0.6/hfmirror/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/storage/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/storage/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:02:24.503412 hfmirror-0.0.6/hfmirror/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:02:24.503412 hfmirror-0.0.6/hfmirror/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/utils/filepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/utils/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-08 15:01:48.000000 hfmirror-0.0.6/hfmirror/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:02:24.499412 hfmirror-0.0.6/hfmirror.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-08 15:02:24.000000 hfmirror-0.0.6/hfmirror.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-08 15:02:24.000000 hfmirror-0.0.6/hfmirror.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:02:24.000000 hfmirror-0.0.6/hfmirror.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-08 15:02:24.000000 hfmirror-0.0.6/hfmirror.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 15:02:24.000000 hfmirror-0.0.6/hfmirror.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-08 15:01:48.000000 hfmirror-0.0.6/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-08 15:01:48.000000 hfmirror-0.0.6/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-08 15:01:48.000000 hfmirror-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 15:02:24.503412 hfmirror-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-08 15:01:48.000000 hfmirror-0.0.6/setup.py
```

### Comparing `hfmirror-0.0.5/LICENSE` & `hfmirror-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/PKG-INFO` & `hfmirror-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfmirror
-Version: 0.0.5
+Version: 0.0.6
 Summary: Mirror for resources to local and huggingface.
 Home-page: https://github.com/narugo1992/hfmirror
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE
 
 # hfmirror
 
 [![PyPI](https://img.shields.io/pypi/v/hfmirror)](https://pypi.org/project/hfmirror/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hfmirror)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/7eedd99825928ca780ec3aef60f7ce8d/raw/loc.json)
```

### Comparing `hfmirror-0.0.5/README.md` & `hfmirror-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/resource/github.py` & `hfmirror-0.0.6/hfmirror/resource/github.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/resource/item.py` & `hfmirror-0.0.6/hfmirror/resource/item.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/resource/resource.py` & `hfmirror-0.0.6/hfmirror/resource/resource.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/resource/sourceforge.py` & `hfmirror-0.0.6/hfmirror/resource/sourceforge.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/resource/version.py` & `hfmirror-0.0.6/hfmirror/resource/version.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/storage/base.py` & `hfmirror-0.0.6/hfmirror/storage/base.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/storage/huggingface.py` & `hfmirror-0.0.6/hfmirror/storage/huggingface.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/storage/local.py` & `hfmirror-0.0.6/hfmirror/storage/local.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/sync/sync.py` & `hfmirror-0.0.6/hfmirror/sync/sync.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from hbutils.string import plural_word
 from hbutils.system.filesystem.tempfile import TemporaryDirectory
 from tqdm import tqdm as _TqdmType
 from tqdm.auto import tqdm
 
 from ..resource import SyncResource, SyncTree, ResourceNotChange
 from ..storage import BaseStorage
+from ..utils import FilePool
 
 
 def _count_trees(tree: SyncTree):
     tree_cnt, file_cnt = 1, 0
     for _, item in tree.items.items():
         if isinstance(item, SyncTree):
             l_tree_cnt, l_file_cnt = _count_trees(item)
@@ -23,20 +24,27 @@
         else:
             file_cnt += 1
 
     return tree_cnt, file_cnt
 
 
 class SyncTask:
-    def __init__(self, resource: SyncResource, storage: BaseStorage, meta_filename='.meta.json'):
+    def __init__(self, resource: SyncResource, storage: BaseStorage, meta_filename='.meta.json',
+                 batch: int = 50):
         self.resource = resource
         self.storage = storage
         self.meta_filename = meta_filename
 
-    def _sync_tree(self, tree: SyncTree, segments: List[str], tqdms: Tuple[_TqdmType, _TqdmType]):
+        # batch < 0, do not submit until the end of sync
+        # batch == 0, submit immediately every time
+        # batch > 0, submit changes when changes over `batch`
+        self.batch = batch
+
+    def _sync_tree(self, tree: SyncTree, segments: List[str], tqdms: Tuple[_TqdmType, _TqdmType],
+                   preserved: Tuple[FilePool, List]):
         tree_tqdm, file_tqdm = tqdms
         tree_tqdm.set_description('/'.join(segments))
         items, folders = [], []
         for key in sorted(tree.items.keys()):
             value = tree.items[key]
             if isinstance(value, SyncTree):
                 folders.append((key, value))
@@ -50,15 +58,15 @@
             old_item_names = {item['name'] for item in chain(old_metadata['files'], old_metadata['folders'])}
         else:
             old_files = {}
             old_item_names = set()
 
         m_folders = []
         for key, folder in folders:
-            self._sync_tree(folder, [*segments, key], tqdms)
+            self._sync_tree(folder, [*segments, key], tqdms, preserved)
             m_folders.append({'name': key, 'metadata': folder.metadata})
 
         m_files = []
         need_load_files = []
         for key, item in tqdm(items, desc=f"Mark for {'/'.join(segments)}"):
             old_file_data = old_files.get(key)
             if old_file_data and old_file_data['type'] == item.__type__:
@@ -81,14 +89,15 @@
             m_files.append({
                 'name': key,
                 'type': item.__type__,
                 'mark': mark,
                 'metadata': item.metadata,
             })
 
+        file_pool, preserved_changes = preserved
         with TemporaryDirectory() as td:
             local_metafile = os.path.join(td, self.meta_filename)
             with open(local_metafile, 'w', encoding='utf-8') as f:
                 json.dump({
                     'path': '/'.join(segments),
                     'metadata': tree.metadata,
                     'files': m_files,
@@ -99,20 +108,38 @@
             with nested_with(*[item.load_file() for _, item in need_load_files]) as file_paths:
                 changes = [(local_metafile, [*segments, self.meta_filename])]  # .meta.json
                 for local_file, (key, _) in zip(file_paths, need_load_files):  # items to add
                     changes.append((local_file, [*segments, key]))
                 for key in sorted(old_item_names - new_item_names):  # items to delete
                     changes.append((None, [*segments, key]))
 
-                self.storage.batch_change_files(changes)
+                if self.batch == 0:
+                    self.storage.batch_change_files(changes)
+                else:
+                    for local_file, remote_segs in changes:
+                        if local_file is not None:
+                            preserved_changes.append((file_pool.put_file(local_file), remote_segs))
+                        else:
+                            preserved_changes.append((None, remote_segs))
+
+                    if 0 < self.batch <= len(preserved_changes):
+                        self.storage.batch_change_files(preserved_changes)
+                        preserved_changes.clear()
+                        file_pool.cleanup()
 
             file_tqdm.update(len(need_load_files))
             file_tqdm.set_description(plural_word(file_tqdm.n, 'file'))
 
         tree_tqdm.update()
 
     def sync(self):
         tree: SyncTree = self.resource.sync_tree()
         total_trees, total_files = _count_trees(tree)
+
         tree_tqdm = tqdm(total=total_trees)
         file_tqdm = tqdm(total=total_files)
-        self._sync_tree(tree, [], (tree_tqdm, file_tqdm))
+        file_pool, preserved_changes = FilePool(), []
+        self._sync_tree(tree, [], (tree_tqdm, file_tqdm), (file_pool, preserved_changes))
+        if preserved_changes:
+            self.storage.batch_change_files(preserved_changes)
+            preserved_changes.clear()
+            file_pool.cleanup()
```

### Comparing `hfmirror-0.0.5/hfmirror/utils/download.py` & `hfmirror-0.0.6/hfmirror/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/utils/hash.py` & `hfmirror-0.0.6/hfmirror/utils/hash.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/utils/segments.py` & `hfmirror-0.0.6/hfmirror/utils/segments.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/utils/session.py` & `hfmirror-0.0.6/hfmirror/utils/session.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror/utils/text.py` & `hfmirror-0.0.6/hfmirror/utils/text.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.5/hfmirror.egg-info/PKG-INFO` & `hfmirror-0.0.6/hfmirror.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfmirror
-Version: 0.0.5
+Version: 0.0.6
 Summary: Mirror for resources to local and huggingface.
 Home-page: https://github.com/narugo1992/hfmirror
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE
 
 # hfmirror
 
 [![PyPI](https://img.shields.io/pypi/v/hfmirror)](https://pypi.org/project/hfmirror/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hfmirror)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/7eedd99825928ca780ec3aef60f7ce8d/raw/loc.json)
```

### Comparing `hfmirror-0.0.5/hfmirror.egg-info/SOURCES.txt` & `hfmirror-0.0.6/hfmirror.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,11 +23,12 @@
 hfmirror/storage/base.py
 hfmirror/storage/huggingface.py
 hfmirror/storage/local.py
 hfmirror/sync/__init__.py
 hfmirror/sync/sync.py
 hfmirror/utils/__init__.py
 hfmirror/utils/download.py
+hfmirror/utils/filepool.py
 hfmirror/utils/hash.py
 hfmirror/utils/segments.py
 hfmirror/utils/session.py
 hfmirror/utils/text.py
```

### Comparing `hfmirror-0.0.5/hfmirror.egg-info/requires.txt` & `hfmirror-0.0.6/hfmirror.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 hbutils>=0.9.0
 tqdm>=4.0.0
 click>=7.0.0
 requests
 pyquery
 pygithub
-huggingface_hub
+huggingface_hub>=0.14.0
 
 [doc]
 Jinja2~=3.0.0
 sphinx~=3.2.0
 sphinx_rtd_theme~=0.4.3
 enum_tools
 sphinx-toolbox
```

### Comparing `hfmirror-0.0.5/setup.py` & `hfmirror-0.0.6/setup.py`

 * *Files identical despite different names*

