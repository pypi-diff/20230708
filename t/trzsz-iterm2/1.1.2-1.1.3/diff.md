# Comparing `tmp/trzsz-iterm2-1.1.2.tar.gz` & `tmp/trzsz-iterm2-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trzsz-iterm2-1.1.2.tar", last modified: Sun Mar 26 07:39:09 2023, max compression
+gzip compressed data, was "trzsz-iterm2-1.1.3.tar", last modified: Sat Jul  8 14:07:04 2023, max compression
```

## Comparing `trzsz-iterm2-1.1.2.tar` & `trzsz-iterm2-1.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:09.196866 trzsz-iterm2-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-03-26 07:39:09.196866 trzsz-iterm2-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 07:39:09.196866 trzsz-iterm2-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:09.192866 trzsz-iterm2-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14713 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/tests/test_text_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:09.192866 trzsz-iterm2-1.1.2/tests/trzsz/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/tests/trzsz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:09.192866 trzsz-iterm2-1.1.2/tests/trzsz/iterm2/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/tests/trzsz/iterm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/tests/trzsz/iterm2/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/tests/trzsz/iterm2/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/tests/trzsz/iterm2/text_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/tests/trzsz/iterm2/zenity_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:09.192866 trzsz-iterm2-1.1.2/trzsz/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/trzsz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:09.192866 trzsz-iterm2-1.1.2/trzsz/iterm2/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/trzsz/iterm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/trzsz/iterm2/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/trzsz/iterm2/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/trzsz/iterm2/text_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-03-26 07:39:03.000000 trzsz-iterm2-1.1.2/trzsz/iterm2/zenity_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:09.196866 trzsz-iterm2-1.1.2/trzsz_iterm2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-03-26 07:39:09.000000 trzsz-iterm2-1.1.2/trzsz_iterm2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-26 07:39:09.000000 trzsz-iterm2-1.1.2/trzsz_iterm2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 07:39:09.000000 trzsz-iterm2-1.1.2/trzsz_iterm2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-26 07:39:09.000000 trzsz-iterm2-1.1.2/trzsz_iterm2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-26 07:39:09.000000 trzsz-iterm2-1.1.2/trzsz_iterm2.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 07:39:09.000000 trzsz-iterm2-1.1.2/trzsz_iterm2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-26 07:39:09.000000 trzsz-iterm2-1.1.2/trzsz_iterm2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-26 07:39:09.000000 trzsz-iterm2-1.1.2/trzsz_iterm2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.590315 trzsz-iterm2-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-07-08 14:07:04.590315 trzsz-iterm2-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.586315 trzsz-iterm2-1.1.3/iterm2-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/iterm2-tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15852 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/iterm2-tests/test_text_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.586315 trzsz-iterm2-1.1.3/iterm2-tests/trzsz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/iterm2-tests/trzsz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.586315 trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/text_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/zenity_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:07:04.590315 trzsz-iterm2-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.586315 trzsz-iterm2-1.1.3/trzsz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/trzsz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.586315 trzsz-iterm2-1.1.3/trzsz/iterm2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/trzsz/iterm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/trzsz/iterm2/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/trzsz/iterm2/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/trzsz/iterm2/text_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-08 14:07:00.000000 trzsz-iterm2-1.1.3/trzsz/iterm2/zenity_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.590315 trzsz-iterm2-1.1.3/trzsz_iterm2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-07-08 14:07:04.000000 trzsz-iterm2-1.1.3/trzsz_iterm2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-08 14:07:04.000000 trzsz-iterm2-1.1.3/trzsz_iterm2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:07:04.000000 trzsz-iterm2-1.1.3/trzsz_iterm2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-08 14:07:04.000000 trzsz-iterm2-1.1.3/trzsz_iterm2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 14:07:04.000000 trzsz-iterm2-1.1.3/trzsz_iterm2.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:07:04.000000 trzsz-iterm2-1.1.3/trzsz_iterm2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 14:07:04.000000 trzsz-iterm2-1.1.3/trzsz_iterm2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 14:07:04.000000 trzsz-iterm2-1.1.3/trzsz_iterm2.egg-info/top_level.txt
```

### Comparing `trzsz-iterm2-1.1.2/PKG-INFO` & `trzsz-iterm2-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trzsz-iterm2
-Version: 1.1.2
+Version: 1.1.3
 Summary: trzsz is a simple file transfer tools, similar to lrzsz ( rz / sz ) and compatible with tmux, which works with iTerm2 and has a nice progress bar.
 Home-page: https://trzsz.github.io
 Author: Lonny Wong
 Author-email: lonnywong@qq.com
 License: MIT License
 Keywords: trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `trzsz-iterm2-1.1.2/README.md` & `trzsz-iterm2-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `trzsz-iterm2-1.1.2/setup.py` & `trzsz-iterm2-1.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,20 +19,20 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import re
 from setuptools import setup, find_packages
 
-version_regex = r'[ \t]*__version__[ \t]*=[ \t]*[\'"](\d+\.\d+\.\d+)[\'"]'
-with open('trzsz/iterm2/__version__.py', 'r') as f:
-    version = re.search(version_regex, f.read()).group(1)
+VERSION_REGEX = r'[ \t]*__version__[ \t]*=[ \t]*[\'"](\d+\.\d+\.\d+)[\'"]'
+with open('trzsz/iterm2/__version__.py', 'r', encoding='utf8') as file:
+    version = re.search(VERSION_REGEX, file.read()).group(1)
 
-with open('README.md', 'rb') as f:
-    long_description = f.read().decode('utf8')
+with open('README.md', 'rb') as file:
+    long_description = file.read().decode('utf8')
 
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Intended Audience :: System Administrators',
@@ -47,27 +47,27 @@
 entry_points = {
     'console_scripts': [
         'trzsz-iterm2 = trzsz.iterm2.main:main',
     ],
 }
 
 setup(
-    name                            = 'trzsz-iterm2',
-    version                         = version,
-    author                          = 'Lonny Wong',
-    author_email                    = 'lonnywong@qq.com',
-    packages                        = find_packages(),
-    namespace_packages              = ['trzsz'],
-    long_description                = long_description,
-    long_description_content_type   = 'text/markdown',
-    url                             = 'https://trzsz.github.io',
-    python_requires                 = '>=3.7',
-    install_requires                = [ 'trzsz-libs == ' + version, 'iterm2 >= 2.7' ],
-    license                         = 'MIT License',
-    classifiers                     = classifiers,
-    entry_points                    = entry_points,
-    keywords                        = 'trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar',
-    zip_safe                        = False,
-    description                     = 'trzsz is a simple file transfer tools, ' \
-                                      'similar to lrzsz ( rz / sz ) and compatible with tmux, ' \
-                                      'which works with iTerm2 and has a nice progress bar.',
+    name='trzsz-iterm2',
+    version=version,
+    author='Lonny Wong',
+    author_email='lonnywong@qq.com',
+    packages=find_packages(),
+    namespace_packages=['trzsz'],
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://trzsz.github.io',
+    python_requires='>=3.7',
+    install_requires=['trzsz-libs == ' + version, 'iterm2 >= 2.7'],
+    license='MIT License',
+    classifiers=classifiers,
+    entry_points=entry_points,
+    keywords='trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar',
+    zip_safe=False,
+    description='trzsz is a simple file transfer tools, '
+    'similar to lrzsz ( rz / sz ) and compatible with tmux, '
+    'which works with iTerm2 and has a nice progress bar.',
 )
```

### Comparing `trzsz-iterm2-1.1.2/tests/test_text_progress.py` & `trzsz-iterm2-1.1.3/iterm2-tests/test_text_progress.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,161 +19,188 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import re
 import unittest
 import unittest.mock
-from .trzsz.iterm2.text_progress import *
+from .trzsz.iterm2 import text_progress
+
 
 class GridSize():
+
     def __init__(self, width):
         self.width = width
 
+
 class Session():
+
     def __init__(self, width):
         self.grid_size = GridSize(width)
 
-def output_length(s):
-    return display_length(re.sub(r'(\u2588|\u2591)', '*', re.sub(r'\u001b\[\d+[mD]', '', re.sub(r'\r', '', s))))
+
+def output_length(output):
+    return text_progress.display_length(
+        re.sub(r'(\u2588|\u2591)', '*', re.sub(r'\u001b\[\d+[mD]', '', re.sub(r'\r', '', output))))
+
 
 class TestTextProgressBar(unittest.TestCase):
+
     def setUp(self):
         self.loop = {}
         self.session = Session(100)
-        self.tgb = TextProgressBar(self.loop, self.session)
+        self.tgb = text_progress.TextProgressBar(self.loop, self.session)
         self.mock_inject = unittest.mock.Mock()
         # pylint: disable=protected-access
         self.tgb._inject_to_iterm2 = self.mock_inject
 
     @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564135])
     def test_empty_file(self, mock_time):
         self.tgb.on_num(1)
         self.tgb.on_name('中文😀test.txt')
         self.tgb.on_size(0)
         self.tgb.on_step(0)
         self.assertEqual(mock_time.call_count, 2)
-        self.mock_inject.assert_not_called()
+        self.mock_inject.assert_called_once()
+        self.assertIn('中文😀test.txt [', self.mock_inject.call_args[0][0])
+        self.assertIn('] 100% | 0.00 B | --- B/s | --- ETA', self.mock_inject.call_args[0][0])
+        self.assertEqual(output_length(self.mock_inject.call_args[0][0]), 100)
 
-    @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564135])
-    def test_nan_speed(self, mock_time):
+    @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564135.1])
+    def test_zero_step(self, mock_time):
         self.tgb.on_num(1)
         self.tgb.on_name('中文😀test.txt')
         self.tgb.on_size(100)
         self.tgb.on_step(0)
         self.assertEqual(mock_time.call_count, 2)
         self.mock_inject.assert_called_once()
         self.assertIn('中文😀test.txt [', self.mock_inject.call_args[0][0])
-        self.assertIn('] 0% | 0.00B | NaN/s | NaN ETA', self.mock_inject.call_args[0][0])
+        self.assertIn('] 0% | 0.00 B | --- B/s | --- ETA', self.mock_inject.call_args[0][0])
         self.assertEqual(output_length(self.mock_inject.call_args[0][0]), 100)
 
-    @unittest.mock.patch('time.time', side_effect=[1646564135 + i for i in range(36)])
+    @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564135.2])
+    def test_last_step(self, mock_time):
+        self.tgb.on_num(1)
+        self.tgb.on_name('中文😀test.txt')
+        self.tgb.on_size(100)
+        self.tgb.on_step(100)
+        self.assertEqual(mock_time.call_count, 2)
+        self.mock_inject.assert_called_once()
+        self.assertIn('中文😀test.txt [', self.mock_inject.call_args[0][0])
+        self.assertIn('] 100% | 100 B | 500 B/s | 00:00 ETA', self.mock_inject.call_args[0][0])
+        self.assertEqual(output_length(self.mock_inject.call_args[0][0]), 100)
+
+    @unittest.mock.patch('time.time', side_effect=[1646564135 + i for i in range(101)])
     def test_newest_speed(self, mock_time):
         self.tgb.on_num(1)
         self.tgb.on_name('中文😀test.txt')
         self.tgb.on_size(100000)
         step = 100
-        for i in range(35):
+        for i in range(100):
             step += i * 10
             self.tgb.on_step(step)
-        self.assertEqual(mock_time.call_count, 36)
-        self.assertEqual(self.mock_inject.call_count, 35)
+        self.assertEqual(mock_time.call_count, 101)
+        self.assertEqual(self.mock_inject.call_count, 100)
         total = 100.0
-        for i in range(35):
+        for i in range(100):
             total += i * 10
             percentage = int(round((total * 100) / 100000))
-            if i < 10:
+            if i < 30:
                 speed = total / (i + 1)
             else:
-                t = 0.0
-                for j in range(i - 10 + 1, i + 1):
-                    t += j * 10
-                speed = t / 10
-            total_str = f'{(total / 1024):.2f}K' if total >= 1024 else f'{total:.0f}'
+                latest_total = 0.0
+                for j in range(i - 30 + 1, i + 1):
+                    latest_total += j * 10
+                speed = latest_total / 30
+            total_str = f'{total:.0f} B'
+            if total >= 10240:
+                total_str = f'{(total / 1024):.1f} KB'
+            elif total >= 1024:
+                total_str = f'{(total / 1024):.2f} KB'
             speed_str = f'{speed:.0f}' if speed >= 100 else f'{speed:.1f}'
             eta = int(round((100000 - total) / speed))
             minute = str(eta // 60).rjust(2, '0')
             second = str(eta % 60).rjust(2, '0')
             self.assertIn('中文😀test.txt [', self.mock_inject.call_args_list[i].args[0])
-            self.assertIn(f'] {percentage}% | {total_str}B | {speed_str}B/s | {minute}:{second} ETA',
+            self.assertIn(f'] {percentage}% | {total_str} | {speed_str} B/s | {minute}:{second} ETA',
                           self.mock_inject.call_args_list[i].args[0])
             self.assertEqual(output_length(self.mock_inject.call_args_list[i].args[0]), 100)
 
     @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564135.001, 1646564135.099])
     def test_output_once_only(self, mock_time):
         self.tgb.on_num(1)
         self.tgb.on_name('中文😀test.txt')
         self.tgb.on_size(100)
         self.tgb.on_step(1)
         self.tgb.on_step(2)
         self.assertEqual(mock_time.call_count, 3)
         self.mock_inject.assert_called_once()
         self.assertIn('中文😀test.txt [', self.mock_inject.call_args[0][0])
-        self.assertIn('] 1% | 1.00B | 1000B/s | 00:00 ETA', self.mock_inject.call_args[0][0])
+        self.assertIn('] 1% | 1.00 B | 1000 B/s | 00:00 ETA', self.mock_inject.call_args[0][0])
         self.assertEqual(output_length(self.mock_inject.call_args[0][0]), 100)
 
     @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564136])
     def test_super_fast(self, mock_time):
         self.tgb.on_num(1)
         self.tgb.on_name('中文😀test.txt')
         self.tgb.on_size(1024 * 1024 * 1024 * 1024 * 1024)
         self.tgb.on_step(10.1 * 1024 * 1024 * 1024 * 1024)
         self.assertEqual(mock_time.call_count, 2)
         self.mock_inject.assert_called_once()
         self.assertIn('中文😀test.txt [', self.mock_inject.call_args[0][0])
-        self.assertIn('] 1% | 10.1TB | 10.1TB/s | 01:40 ETA', self.mock_inject.call_args[0][0])
+        self.assertIn('] 1% | 10.1 TB | 10.1 TB/s | 01:40 ETA', self.mock_inject.call_args[0][0])
         self.assertEqual(output_length(self.mock_inject.call_args[0][0]), 100)
 
     @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564136])
     def test_very_slow(self, mock_time):
         self.tgb.on_num(1)
         self.tgb.on_name('中文😀test.txt')
         self.tgb.on_size(1024 * 1024)
         self.tgb.on_step(1)
         self.assertEqual(mock_time.call_count, 2)
         self.mock_inject.assert_called_once()
         self.assertIn('中文😀test.txt [', self.mock_inject.call_args[0][0])
-        self.assertIn('] 0% | 1.00B | 1.00B/s | 291:16:15 ETA', self.mock_inject.call_args[0][0])
+        self.assertIn('] 0% | 1.00 B | 1.00 B/s | 291:16:15 ETA', self.mock_inject.call_args[0][0])
         self.assertEqual(output_length(self.mock_inject.call_args[0][0]), 100)
 
     @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564136, 1646564138])
     def test_long_name(self, mock_time):
         self.tgb.on_num(1)
         self.tgb.on_name('中文😀非常长非常长非常长非常长非常长非常长非常长非常长.txt')
         self.tgb.on_size(1000 * 1024)
         self.tgb.columns = 110
         self.tgb.on_step(100 * 1024)
         self.tgb.columns = 100
         self.tgb.on_step(200 * 1024)
         self.assertEqual(mock_time.call_count, 3)
         self.assertEqual(self.mock_inject.call_count, 2)
         self.assertIn('中文😀非常长非常长非常长非常长非常长非常长非常... [', self.mock_inject.call_args_list[0].args[0])
-        self.assertIn('] 10% | 100KB | 100KB/s | 00:09 ETA', self.mock_inject.call_args_list[0].args[0])
+        self.assertIn('] 10% | 100 KB | 100 KB/s | 00:09 ETA', self.mock_inject.call_args_list[0].args[0])
         self.assertEqual(output_length(self.mock_inject.call_args_list[0].args[0]), 110)
         self.assertIn('中文😀非常长非常长非常长非常长非常长... [', self.mock_inject.call_args_list[1].args[0])
-        self.assertIn('] 20% | 200KB | 66.7KB/s | 00:12 ETA', self.mock_inject.call_args_list[1].args[0])
+        self.assertIn('] 20% | 200 KB | 66.7 KB/s | 00:12 ETA', self.mock_inject.call_args_list[1].args[0])
         self.assertEqual(output_length(self.mock_inject.call_args_list[1].args[0]), 100)
 
     @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564136, 1646564138])
     def test_no_total(self, mock_time):
         self.tgb.on_num(1)
         self.tgb.on_name('中文😀非常长非常长非常长非常长非常长非常长非常长非常长.txt')
         self.tgb.on_size(1000 * 1024 * 1024 * 1024)
-        self.tgb.columns = 90
+        self.tgb.columns = 95
         self.tgb.on_step(100 * 1024 * 1024)
-        self.tgb.columns = 80
+        self.tgb.columns = 85
         self.tgb.on_step(200 * 1024 * 1024 * 1024)
         self.assertEqual(mock_time.call_count, 3)
         self.assertEqual(self.mock_inject.call_count, 2)
         self.assertIn('中文😀非常长非常长非常长非常长非常长... [', self.mock_inject.call_args_list[0].args[0])
-        self.assertIn('] 0% | 100MB/s | 2:50:39 ETA', self.mock_inject.call_args_list[0].args[0])
-        self.assertEqual(output_length(self.mock_inject.call_args_list[0].args[0]), 90)
+        self.assertIn('] 0% | 100 MB/s | 2:50:39 ETA', self.mock_inject.call_args_list[0].args[0])
+        self.assertEqual(output_length(self.mock_inject.call_args_list[0].args[0]), 95)
         self.assertIn('中文😀非常长非常长非常长非... [', self.mock_inject.call_args_list[1].args[0])
-        self.assertIn('] 20% | 66.7GB/s | 00:12 ETA', self.mock_inject.call_args_list[1].args[0])
-        self.assertEqual(output_length(self.mock_inject.call_args_list[1].args[0]), 80)
+        self.assertIn('] 20% | 66.7 GB/s | 00:12 ETA', self.mock_inject.call_args_list[1].args[0])
+        self.assertEqual(output_length(self.mock_inject.call_args_list[1].args[0]), 85)
 
     @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564136, 1646564138])
     def test_no_speed(self, mock_time):
         self.tgb.on_num(1)
         self.tgb.on_name('中文😀longlonglonglonglonglongname.txt')
         self.tgb.on_size(1000)
         self.tgb.columns = 70
@@ -229,25 +256,25 @@
         self.tgb.on_size(2000)
         self.tgb.on_step(300)
         self.tgb.on_done()
         self.assertEqual(mock_time.call_count, 4)
         self.assertEqual(self.mock_inject.call_count, 4)
         self.assertNotIn('\r', self.mock_inject.call_args_list[0].args[0])
         self.assertIn('(1/2) 中文😀test.txt [', self.mock_inject.call_args_list[0].args[0])
-        self.assertIn('] 10% | 100B | 100B/s | 00:09 ETA', self.mock_inject.call_args_list[0].args[0])
+        self.assertIn('] 10% | 100 B | 100 B/s | 00:09 ETA', self.mock_inject.call_args_list[0].args[0])
         self.assertEqual(output_length(self.mock_inject.call_args_list[0].args[0]), 100)
         self.assertEqual('\r', self.mock_inject.call_args_list[1].args[0])
         self.assertIn('(2/2) 英文😀test.txt [', self.mock_inject.call_args_list[2].args[0])
-        self.assertIn('] 15% | 300B | 150B/s | 00:11 ETA', self.mock_inject.call_args_list[2].args[0])
+        self.assertIn('] 15% | 300 B | 150 B/s | 00:11 ETA', self.mock_inject.call_args_list[2].args[0])
         self.assertEqual(output_length(self.mock_inject.call_args_list[2].args[0]), 100)
         self.assertEqual('\r', self.mock_inject.call_args_list[3].args[0])
 
     @unittest.mock.patch('time.time', side_effect=[1646564135, 1646564136, 1646564137, 1646564138, 1646564139])
     def test_tmux_pane(self, mock_time):
-        self.tgb = TextProgressBar(self.loop, self.session, 80)
+        self.tgb = text_progress.TextProgressBar(self.loop, self.session, 80)
         # pylint: disable=protected-access
         self.tgb._inject_to_iterm2 = self.mock_inject
         self.tgb.on_num(2)
         self.tgb.on_name('中文😀test.txt')
         self.tgb.on_size(1000)
         self.tgb.on_step(100)
         self.tgb.on_step(200)
@@ -258,28 +285,29 @@
         self.tgb.on_done()
 
         self.assertEqual(mock_time.call_count, 5)
         self.assertEqual(self.mock_inject.call_count, 5)
         self.assertNotIn('\r', self.mock_inject.call_args_list[0].args[0])
         self.assertNotIn('\x1b[80D', self.mock_inject.call_args_list[0].args[0])
         self.assertIn('(1/2) 中文😀test.txt [', self.mock_inject.call_args_list[0].args[0])
-        self.assertIn('] 10% | 100B | 100B/s | 00:09 ETA', self.mock_inject.call_args_list[0].args[0])
+        self.assertIn('] 10% | 100 B | 100 B/s | 00:09 ETA', self.mock_inject.call_args_list[0].args[0])
         self.assertEqual(output_length(self.mock_inject.call_args_list[0].args[0]), 80)
 
         self.assertNotIn('\r', self.mock_inject.call_args_list[1].args[0])
         self.assertIn('\x1b[80D', self.mock_inject.call_args_list[1].args[0])
         self.assertIn('(1/2) 中文😀test.txt [', self.mock_inject.call_args_list[1].args[0])
-        self.assertIn('] 20% | 200B | 100B/s | 00:08 ETA', self.mock_inject.call_args_list[1].args[0])
+        self.assertIn('] 20% | 200 B | 100 B/s | 00:08 ETA', self.mock_inject.call_args_list[1].args[0])
         self.assertEqual(output_length(self.mock_inject.call_args_list[1].args[0]), 80)
 
         self.assertIn('\x1b[80D', self.mock_inject.call_args_list[2].args[0])
 
         self.assertNotIn('\r', self.mock_inject.call_args_list[3].args[0])
         self.assertNotIn('\x1b[80D', self.mock_inject.call_args_list[3].args[0])
         self.assertIn('(2/2) 中文😀test2.txt [', self.mock_inject.call_args_list[3].args[0])
-        self.assertIn('] 30% | 300B | 300B/s | 00:02 ETA', self.mock_inject.call_args_list[3].args[0])
+        self.assertIn('] 30% | 300 B | 300 B/s | 00:02 ETA', self.mock_inject.call_args_list[3].args[0])
         self.assertEqual(output_length(self.mock_inject.call_args_list[3].args[0]), 80)
 
         self.assertIn('\x1b[80D', self.mock_inject.call_args_list[4].args[0])
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `trzsz-iterm2-1.1.2/tests/trzsz/__init__.py` & `trzsz-iterm2-1.1.3/iterm2-tests/trzsz/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2021 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `trzsz-iterm2-1.1.2/tests/trzsz/iterm2/__init__.py` & `trzsz-iterm2-1.1.3/iterm2-tests/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2021 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `trzsz-iterm2-1.1.2/tests/trzsz/iterm2/__version__.py` & `trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,8 +16,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = '1.1.2'
+__version__ = '1.1.3'
```

### Comparing `trzsz-iterm2-1.1.2/tests/trzsz/iterm2/main.py` & `trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -27,36 +27,40 @@
 import select
 import asyncio
 import argparse
 import tempfile
 import threading
 import subprocess
 import iterm2
-from trzsz.libs.utils import *
+from trzsz.libs import utils
+from trzsz.libs import transfer
 from trzsz.iterm2.__version__ import __version__
 from trzsz.iterm2.text_progress import TextProgressBar
 from trzsz.iterm2.zenity_progress import ZenityProgressBar
 
+
 class ProgressType(enum.Enum):
-    text = 'text'
-    zenity = 'zenity'
+    TEXT = 'text'
+    ZENITY = 'zenity'
 
     def __str__(self):
         return self.value
 
+
 def run_osascript(script):
     try:
         out = subprocess.check_output(['osascript', '-l', 'JavaScript', '-e', script], stderr=subprocess.STDOUT)
         return out.decode('utf8').strip()
-    except subprocess.CalledProcessError as e:
-        if b"Application can't be found." in e.output:
-            sys.stderr.write(e.output + '\n')
-            raise TrzszError('Only supports iTerm2', trace=False)
+    except subprocess.CalledProcessError as ex:
+        if b"Application can't be found." in ex.output:
+            sys.stderr.write(ex.output + '\n')
+            raise utils.TrzszError('Only supports iTerm2', trace=False)
         raise
 
+
 def choose_download_path(loop, connection):
     if connection and iterm2.capabilities.supports_file_panels(connection):
         panel = iterm2.OpenPanel()
         panel.message = 'Choose a folder to save file(s)'
         panel.options.clear()
         panel.options.append(iterm2.OpenPanel.Options.CAN_CHOOSE_DIRECTORIES)
         panel.options.append(iterm2.OpenPanel.Options.CAN_CREATE_DIRECTORIES)
@@ -82,14 +86,15 @@
             });
             return dest_path.toString();
         } catch (e) {
             return "";
         }
     })();''')
 
+
 def choose_upload_paths(loop, connection, directory):
     if connection and iterm2.capabilities.supports_file_panels(connection):
         panel = iterm2.OpenPanel()
         panel.message = 'Choose some files to send'
         panel.options.clear()
         panel.options.append(iterm2.OpenPanel.Options.CAN_CHOOSE_FILES)
         if directory:
@@ -101,14 +106,15 @@
         event = threading.Event()
         future.add_done_callback(lambda x: event.set())
         event.wait()
         result = future.result()
         if result:
             return result.files
         return None
+    # pylint: disable-next=consider-using-f-string
     file_list = run_osascript('''(function () {
         const app = Application("iTerm2");
         app.includeStandardAdditions = true;
         app.activate();
         try {
             var files = app.%s({
                 withPrompt: "Choose some files to send",
@@ -123,160 +129,177 @@
             return file_list;
         } catch (e) {
             return "";
         }
     })();''' % ('chooseFolder' if directory else 'chooseFile'))
     return [f for f in file_list.split('\n') if f]
 
+
 def download_files(args, loop, connection, session, remote_is_windows):
     dest_path = args.destpath or choose_download_path(loop, connection)
 
     if not dest_path:
-        send_action(False, __version__, remote_is_windows)
+        transfer.send_action(False, __version__, remote_is_windows)
         return
 
-    check_path_writable(dest_path)
+    utils.check_path_writable(dest_path)
 
-    reconfigure_stdin()
+    utils.reconfigure_stdin()
 
-    send_action(True, __version__, remote_is_windows)
-    config = recv_config()
+    transfer.send_action(True, __version__, remote_is_windows)
+    config = transfer.recv_config()
 
     callback = None
-    if not config.get('quiet', False):
-        if args.progress == ProgressType.text and loop and session:
-            callback = TextProgressBar(loop, session, config.get('tmux_pane_width'))
+    if not config.quiet:
+        if args.progress == ProgressType.TEXT and loop and session:
+            callback = TextProgressBar(loop, session, config.tmux_pane_width)
         else:
             callback = ZenityProgressBar('Download')
 
-    local_list = recv_files(dest_path, callback)
+    local_list = transfer.recv_files(dest_path, callback)
+
+    transfer.client_exit(utils.format_saved_files(local_list, dest_path))
+
+
+class GlobalVariables:
+
+    def __init__(self):
+        self.upload_file_list = None
+
 
-    client_exit('Saved %s to %s' % (', '.join(local_list), dest_path))
+GLOBAL = GlobalVariables()
 
-upload_file_list = None
 
-def upload_files(args, loop, connection, session, directory, remote_is_windows):
-    global upload_file_list
-    if upload_file_list:
-        file_list = upload_file_list
-        upload_file_list = None
+def upload_files(args, loop, connection, session, directory, remote_is_windows):  # pylint: disable=too-many-arguments
+    if GLOBAL.upload_file_list:
+        file_list = GLOBAL.upload_file_list
+        GLOBAL.upload_file_list = None
     else:
         paths = choose_upload_paths(loop, connection, directory)
         if not paths:
-            send_action(False, __version__, remote_is_windows)
+            transfer.send_action(False, __version__, remote_is_windows)
             return
-        file_list = check_paths_readable(paths, directory)
+        file_list = utils.check_paths_readable(paths, directory)
 
-    reconfigure_stdin()
+    utils.reconfigure_stdin()
 
-    send_action(True, __version__, remote_is_windows)
-    config = recv_config()
+    transfer.send_action(True, __version__, remote_is_windows)
+    config = transfer.recv_config()
 
-    if config.get('overwrite') is True:
-        check_duplicate_names(file_list)
+    if config.overwrite is True:
+        utils.check_duplicate_names(file_list)
 
     callback = None
-    if not config.get('quiet', False):
-        if args.progress == ProgressType.text and loop and session:
-            callback = TextProgressBar(loop, session, config.get('tmux_pane_width'))
+    if not config.quiet:
+        if args.progress == ProgressType.TEXT and loop and session:
+            callback = TextProgressBar(loop, session, config.tmux_pane_width)
         else:
             callback = ZenityProgressBar('Upload')
 
-    remote_list = send_files(file_list, callback)
+    remote_list = transfer.send_files(file_list, callback)
+
+    transfer.client_exit(utils.format_saved_files(remote_list, ''))
 
-    client_exit('Received %s' % ', '.join(remote_list))
 
 async def keystroke_filter(connection, session):
     all_keys = iterm2.KeystrokePattern()
     all_keys.keycodes = list(iterm2.Keycode)
-    filter = iterm2.KeystrokeFilter(connection, [all_keys], session.session_id)
-    async with filter as mon:
+    async with iterm2.KeystrokeFilter(connection, [all_keys], session.session_id):
         while True:
             await asyncio.sleep(1)
 
+
 async def keystroke_monitor(connection, session):
     async with iterm2.KeystrokeMonitor(connection) as mon:
         while True:
             keystroke = await mon.async_get()
             if keystroke.characters == '\x03':
                 app = await iterm2.async_get_app(connection)
                 current_session = app.current_window.current_tab.current_session
                 if current_session.session_id == session.session_id:
-                    stop_transferring()
+                    utils.stop_transferring()
+
 
 async def get_running_session(force):
     session_id = os.environ.get('ITERM_SESSION_ID')
     if not session_id:
         if force:
-            raise TrzszError('Please upgrade iTerm2', trace=False)
+            raise utils.TrzszError('Please upgrade iTerm2', trace=False)
         return None, None
     try:
         connection = await iterm2.Connection.async_create()
         app = await iterm2.async_get_app(connection)
         current_session = app.current_window.current_tab.current_session
         if current_session.session_id in session_id:
             return connection, current_session
         for win in app.windows:
             for tab in win.tabs:
                 for session in tab.sessions:
                     if session.session_id in session_id:
                         return connection, session
     except Exception:
         if force:
-            raise TrzszError('Please enable iTerm2 Python API', trace=False)
+            raise utils.TrzszError('Please enable iTerm2 Python API', trace=False)
         return None, None
     if force:
-        raise TrzszError("Can't find the session in iTerm2", trace=False)
+        raise utils.TrzszError("Can't find the session in iTerm2", trace=False)
     return None, None
 
+
 def unique_id_exists(unique_id):
     if not unique_id or len(unique_id) < 8:
         return False
     if len(unique_id) == 14 and unique_id.endswith('00'):
         return False
     unique_id = unique_id[1:] + '\n'
     unique_id_path = os.path.join(tempfile.gettempdir(), 'trzsz_unique_id')
     try:
-        unique_id_list = open(unique_id_path, 'r').readlines()
+        with open(unique_id_path, 'r', encoding='utf8') as file:
+            unique_id_list = file.readlines()
     except EnvironmentError:
         unique_id_list = []
     if unique_id in unique_id_list:
         return True
     try:
         unique_id_list.append(unique_id)
-        open(unique_id_path, 'w').writelines(unique_id_list[-50:])
+        with open(unique_id_path, 'w', encoding='utf8') as file:
+            file.writelines(unique_id_list[-50:])
     except EnvironmentError:
         pass
     return False
 
+
 def side_thread(loop):
     asyncio.set_event_loop(loop)
     loop.run_forever()
 
+
 def read_server_output(timeout):
     output = []
     while True:
-        r, w, x = select.select([sys.stdin], [], [], timeout)
-        if not r:
+        rlist, _wlist, _xlist = select.select([sys.stdin], [], [], timeout)
+        if not rlist:
             break
-        out = os.read(sys.stdin.fileno(), 10240)
+        out = os.read(sys.stdin.fileno(), 32 * 1024)
         if not out:
             break
         output.append(out)
     return b''.join(output)
 
-trzsz_trigger_regex = r':TRZSZ:TRANSFER:([SRD]):(\d+\.\d+\.\d+)(:\d+)?'
+
+TRZSZ_TRIGGER_REGEX = r':TRZSZ:TRANSFER:([SRD]):(\d+\.\d+\.\d+)(:\d+)?'
+
 
 def drag_files_to_upload(file_paths, loop, session):
     if not loop or not session:
         sys.stderr.write('Please enable iTerm2 Python API')
         return None
 
     try:
-        file_list = check_paths_readable(file_paths, True)
+        file_list = utils.check_paths_readable(file_paths, True)
 
         sys.stdout.write('\x03')
         sys.stdout.flush()
         read_server_output(0.2)
 
         has_dir = False
         for file in file_list:
@@ -285,85 +308,85 @@
                 break
         if has_dir:
             sys.stdout.write('trz -d\r')
         else:
             sys.stdout.write('trz\r')
         sys.stdout.flush()
 
-        for i in range(20):
+        for _ in range(20):
             output = read_server_output(0.05)
             idx = output.find(b'\n')
             if idx > 0 and output[:idx].rstrip() in (b'trz', b'trz -d'):
                 output = b'\r\n' + output[idx + 1:]
-            trigger_match = re.search(trzsz_trigger_regex, output.decode('ascii'))
+            trigger_match = re.search(TRZSZ_TRIGGER_REGEX, output.decode('latin1'))
             if trigger_match:
                 loop.create_task(session.async_inject(output.replace(b'TRANSFER', b'DRAGFILE')))
-                global upload_file_list
-                upload_file_list = file_list
+                GLOBAL.upload_file_list = file_list
                 return trigger_match
             loop.create_task(session.async_inject(output))
         return None
 
-    except Exception as e:
-        sys.stderr.write(TrzszError.get_err_msg(e))
+    except Exception as ex:
+        sys.stderr.write(utils.TrzszError.get_err_msg(ex))
         return None
 
+
 def main():
     try:
-        parser = argparse.ArgumentParser(description='iTerm2 coprocess of trzsz which similar to lrzsz ' \
-                                                     '( rz / sz ) and compatible with tmux.')
+        parser = argparse.ArgumentParser(description='iTerm2 coprocess of trzsz which similar to lrzsz '
+                                         '( rz / sz ) and compatible with tmux.')
         parser.add_argument('-v', '--version', action='version', version='%(prog)s (trzsz) py ' + __version__)
         parser.add_argument('-p',
                             '--progress',
                             type=ProgressType,
                             choices=list(ProgressType),
-                            default=ProgressType.zenity,
+                            default=ProgressType.ZENITY,
                             help='the progress bar type. (default: zenity)')
         parser.add_argument('-d',
                             '--destpath',
                             type=str,
                             default=None,
                             help='the default save destination path. (default: choose each time)')
         parser.add_argument('args', nargs='+', help='iTerm2 trigger parameters. (generally should be \\1)')
         args = parser.parse_args()
 
         loop = asyncio.new_event_loop()
-        force = args.progress == ProgressType.text and args.args[0] != 'dragfiles'
+        force = args.progress == ProgressType.TEXT and args.args[0] != 'dragfiles'
         connection, session = loop.run_until_complete(get_running_session(force))
         if connection and session:
             thread = threading.Thread(target=side_thread, args=(loop, ), daemon=True)
             thread.start()
             asyncio.run_coroutine_threadsafe(keystroke_filter(connection, session), loop)
             asyncio.run_coroutine_threadsafe(keystroke_monitor(connection, session), loop)
 
         if len(args.args) > 1 and args.args[0] == 'dragfiles':
             trigger_match = drag_files_to_upload(args.args[1:], loop, session)
             if not trigger_match:
                 return
         else:
-            trigger_match = re.search(trzsz_trigger_regex, args.args[0])
+            trigger_match = re.search(TRZSZ_TRIGGER_REGEX, args.args[0])
             if not trigger_match:
-                raise TrzszError('Please check iTerm2 Trigger configuration', trace=False)
+                raise utils.TrzszError('Please check iTerm2 Trigger configuration', trace=False)
 
         mode = trigger_match.group(1)
-        version = trigger_match.group(2)
         unique_id = trigger_match.group(3)
         remote_is_windows = False
         if unique_id == ':1' or (len(unique_id) == 14 and unique_id.endswith('10')):
             remote_is_windows = True
 
         if unique_id_exists(unique_id):
             return
         if mode == 'S':
             download_files(args, loop, connection, session, remote_is_windows)
         elif mode == 'R':
             upload_files(args, loop, connection, session, False, remote_is_windows)
         elif mode == 'D':
             upload_files(args, loop, connection, session, True, remote_is_windows)
         else:
-            raise TrzszError('Unknown transfer mode: %s' % mode, trace=False)
+            raise utils.TrzszError(f'Unknown transfer mode: {mode}', trace=False)
+
+    except Exception as ex:
+        transfer.client_error(ex)
 
-    except Exception as e:
-        client_error(e)
 
 if __name__ == '__main__':
     main()
```

### Comparing `trzsz-iterm2-1.1.2/tests/trzsz/iterm2/text_progress.py` & `trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/text_progress.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,42 +17,43 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import time
-from trzsz.libs.utils import TrzszCallback
+from trzsz.libs import utils
 
-def display_length(s):
-    l = 0
-    for c in s:
-        l += 1 if len(c.encode('utf8')) == 1 else 2
-    return l
-
-def ellipsis_string(s, m):
-    m -= 3
-    l = 0
-    r = []
-    for c in s:
-        if len(c.encode('utf8')) > 1:
-            if l + 2 > m:
+
+def display_length(output):
+    length = 0
+    for char in output:
+        length += 1 if len(char.encode('utf8')) == 1 else 2
+    return length
+
+
+def ellipsis_string(text, max_len):
+    max_len -= 3
+    length = 0
+    result = []
+    for char in text:
+        if len(char.encode('utf8')) > 1:
+            if length + 2 > max_len:
                 break
-            l += 2
+            length += 2
         else:
-            if l + 1 > m:
+            if length + 1 > max_len:
                 break
-            l += 1
-        r.append(c)
-    r.append('...')
-    return ''.join(r), l + 3
+            length += 1
+        result.append(char)
+    result.append('...')
+    return ''.join(result), length + 3
+
 
 def size_to_str(size):
-    if size < 0:
-        return 'NaN'
     unit = 'B'
     while True:
         if size < 1024:
             break
         size = size / 1024
         unit = 'KB'
         if size < 1024:
@@ -65,35 +66,37 @@
         unit = 'GB'
         if size < 1024:
             break
         size = size / 1024
         unit = 'TB'
         break
     if size >= 100:
-        return f'{size:.0f}{unit}'
+        return f'{size:.0f} {unit}'
     if size >= 10:
-        return f'{size:.1f}{unit}'
-    return f'{size:.2f}{unit}'
+        return f'{size:.1f} {unit}'
+    return f'{size:.2f} {unit}'
+
 
 def time_to_str(seconds):
-    if seconds < 0:
-        return 'NaN'
     result = ''
     if seconds >= 3600:
         result += str(int(seconds / 3600)) + ':'
         seconds %= 3600
     minute = int(seconds / 60)
     result += (str(minute) if minute >= 10 else ('0' + str(minute))) + ':'
     second = round(seconds % 60)
     result += str(second) if second >= 10 else ('0' + str(second))
     return result
 
-SPEED_ARRAY_SIZE = 10
 
-class TextProgressBar(TrzszCallback):
+SPEED_ARRAY_SIZE = 30
+
+
+class TextProgressBar(utils.TrzszCallback):  # pylint: disable=too-many-instance-attributes
+
     def __init__(self, loop, session, tmux_pane_width=None):
         self.num = 0
         self.idx = 0
         self.name = ''
         self.size = 0
         self.step = 0
         self.start_time = 0
@@ -101,58 +104,64 @@
         self.first_write = True
         self.speed_cnt = 0
         self.speed_idx = 0
         self.time_array = [0] * SPEED_ARRAY_SIZE
         self.step_array = [0] * SPEED_ARRAY_SIZE
         self.loop = loop
         self.session = session
-        self.tmux_pane_width = tmux_pane_width or -1
+        self.tmux_pane_width = tmux_pane_width or 0
         self.columns = self.tmux_pane_width if self.tmux_pane_width > 0 else session.grid_size.width
 
     def on_num(self, num):
         self.num = num
 
     def on_name(self, name):
         self.name = name
         self.idx += 1
         self.start_time = time.time()
         self.time_array[0] = self.start_time
         self.step_array[0] = 0
         self.speed_cnt = 1
         self.speed_idx = 1
+        self.step = -1
 
     def on_size(self, size):
         self.size = size
 
     def on_step(self, step):
+        if step <= self.step:
+            return
         self.step = step
         self._show_progress()
 
     def on_done(self):
         if not self.first_write:
             if self.tmux_pane_width > 0:
                 self._inject_to_iterm2(f'\x1b[{self.columns}D')
             else:
                 self._inject_to_iterm2('\r')
             self.first_write = True
 
     def _show_progress(self):
         now = time.time()
-        if now - self.update_time < 0.5:
+        if now - self.update_time < 0.2:
             return
         self.update_time = now
 
-        if self.size == 0:
-            return
-        percentage = str(round(self.step * 100 / self.size)) + '%'
+        percentage = "100%"
+        if self.size != 0:
+            percentage = str(round(self.step * 100 / self.size)) + '%'
         total = size_to_str(self.step)
         speed = self._get_speed(now)
-        speed_str = size_to_str(speed) + '/s'
-        eta = time_to_str(round((self.size - self.step) / speed)) + ' ETA'
-        progress_text = self._progress_text(percentage, total, speed_str, eta)
+        speed_str = '--- B/s'
+        eta_str = '--- ETA'
+        if speed > 0:
+            speed_str = size_to_str(speed) + '/s'
+            eta_str = time_to_str(round((self.size - self.step) / speed)) + ' ETA'
+        progress_text = self._progress_text(percentage, total, speed_str, eta_str)
 
         if self.first_write:
             self.first_write = False
             self._inject_to_iterm2(progress_text)
             return
         if self.tmux_pane_width > 0:
             self._inject_to_iterm2(f'\x1b[{self.columns}D{progress_text}')
@@ -174,15 +183,15 @@
 
         self.speed_idx += 1
         if self.speed_idx >= SPEED_ARRAY_SIZE:
             self.speed_idx %= SPEED_ARRAY_SIZE
 
         return speed
 
-    def _progress_text(self, percentage, total, speed, eta):
+    def _progress_text(self, percentage, total, speed, eta):  # pylint: disable=too-many-branches
         bar_min_len = 24
         left = f'({self.idx}/{self.num}) {self.name}' if self.num > 1 else self.name
         left_len = display_length(left)
         right = f' {percentage} | {total} | {speed} | {eta}'
         while True:
             if self.columns - left_len - len(right) >= bar_min_len:
                 break
@@ -219,12 +228,14 @@
             left += ' '
         return (left + self._progress_bar(bar_len) + right).strip()
 
     def _progress_bar(self, bar_len):
         if bar_len < 12:
             return ''
         total = bar_len - 2
-        complete = round(total * self.step / self.size)
+        complete = total
+        if self.size != 0:
+            complete = round(total * self.step / self.size)
         return '[\u001b[36m' + '\u2588' * complete + '\u2591' * (total - complete) + '\u001b[0m]'
 
     def _inject_to_iterm2(self, data):
         self.loop.create_task(self.session.async_inject(data.encode('utf8')))
```

### Comparing `trzsz-iterm2-1.1.2/tests/trzsz/iterm2/zenity_progress.py` & `trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/zenity_progress.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,17 +17,19 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import subprocess
-from trzsz.libs.utils import stop_transferring, TrzszCallback
+from trzsz.libs import utils
+
+
+class ZenityProgressBar(utils.TrzszCallback):
 
-class ZenityProgressBar(TrzszCallback):
     def __init__(self, action):
         self.num = 0
         self.idx = 0
         self.name = ''
         self.size = 0
         self.proc = None
         self.action = action
@@ -37,26 +39,26 @@
         if self.proc:
             self.proc.terminate()
             self.proc = None
 
     def on_num(self, num):
         self.num = num
         try:
-            title = '%s file(s)' % self.action
+            title = f'{self.action} file(s)'
+            # pylint: disable-next=consider-using-with
             self.proc = subprocess.Popen(['/usr/local/bin/zenity', '--progress', '--title', title, '--text', ''],
                                          stdin=subprocess.PIPE,
                                          stdout=subprocess.PIPE,
                                          stderr=subprocess.PIPE)
         except EnvironmentError:
             pass
 
     def _update_progress(self, step):
         percentage = step * 100 // self.size if self.size else 0
-        progress = '%d\n# %sing %s %d%% ( %d / %d ) ...\n' \
-                   % (percentage, self.action, self.name, percentage, self.idx, self.num)
+        progress = f'{percentage}\n# {self.action}ing {self.name} {percentage}% ( {self.idx} / {self.num} ) ...\n'
         if progress == self.progress:
             return
         self.progress = progress
         self.proc.stdin.write(progress.encode('utf8'))
         self.proc.stdin.flush()
 
     def on_name(self, name):
@@ -64,33 +66,33 @@
         self.size = 0
         self.name = name
         if not self.proc:
             return
         try:
             self._update_progress(0)
         except EnvironmentError:
-            stop_transferring()
+            utils.stop_transferring()
 
     def on_size(self, size):
         self.size = size
 
     def on_step(self, step):
         if not self.proc:
             return
         try:
             self._update_progress(step)
         except EnvironmentError:
             if self.idx < self.num or step < self.size:
-                stop_transferring()
+                utils.stop_transferring()
 
     def on_done(self):
         if not self.proc:
             return
         try:
-            self.proc.stdin.write(('# %s %s finished.\n' % (self.action, self.name)).encode('utf8'))
+            self.proc.stdin.write(f'# {self.action} {self.name} finished.\n'.encode('utf8'))
             self.proc.stdin.flush()
         except EnvironmentError:
             if self.idx < self.num:
-                stop_transferring()
+                utils.stop_transferring()
         if self.idx == self.num:
             self.proc.terminate()
             self.proc = None
```

### Comparing `trzsz-iterm2-1.1.2/trzsz/__init__.py` & `trzsz-iterm2-1.1.3/trzsz/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2021 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `trzsz-iterm2-1.1.2/trzsz/iterm2/__init__.py` & `trzsz-iterm2-1.1.3/iterm2-tests/trzsz/iterm2/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2021 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `trzsz-iterm2-1.1.2/trzsz/iterm2/__version__.py` & `trzsz-iterm2-1.1.3/trzsz/iterm2/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,8 +16,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = '1.1.2'
+__version__ = '1.1.3'
```

### Comparing `trzsz-iterm2-1.1.2/trzsz/iterm2/main.py` & `trzsz-iterm2-1.1.3/trzsz/iterm2/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -27,36 +27,40 @@
 import select
 import asyncio
 import argparse
 import tempfile
 import threading
 import subprocess
 import iterm2
-from trzsz.libs.utils import *
+from trzsz.libs import utils
+from trzsz.libs import transfer
 from trzsz.iterm2.__version__ import __version__
 from trzsz.iterm2.text_progress import TextProgressBar
 from trzsz.iterm2.zenity_progress import ZenityProgressBar
 
+
 class ProgressType(enum.Enum):
-    text = 'text'
-    zenity = 'zenity'
+    TEXT = 'text'
+    ZENITY = 'zenity'
 
     def __str__(self):
         return self.value
 
+
 def run_osascript(script):
     try:
         out = subprocess.check_output(['osascript', '-l', 'JavaScript', '-e', script], stderr=subprocess.STDOUT)
         return out.decode('utf8').strip()
-    except subprocess.CalledProcessError as e:
-        if b"Application can't be found." in e.output:
-            sys.stderr.write(e.output + '\n')
-            raise TrzszError('Only supports iTerm2', trace=False)
+    except subprocess.CalledProcessError as ex:
+        if b"Application can't be found." in ex.output:
+            sys.stderr.write(ex.output + '\n')
+            raise utils.TrzszError('Only supports iTerm2', trace=False)
         raise
 
+
 def choose_download_path(loop, connection):
     if connection and iterm2.capabilities.supports_file_panels(connection):
         panel = iterm2.OpenPanel()
         panel.message = 'Choose a folder to save file(s)'
         panel.options.clear()
         panel.options.append(iterm2.OpenPanel.Options.CAN_CHOOSE_DIRECTORIES)
         panel.options.append(iterm2.OpenPanel.Options.CAN_CREATE_DIRECTORIES)
@@ -82,14 +86,15 @@
             });
             return dest_path.toString();
         } catch (e) {
             return "";
         }
     })();''')
 
+
 def choose_upload_paths(loop, connection, directory):
     if connection and iterm2.capabilities.supports_file_panels(connection):
         panel = iterm2.OpenPanel()
         panel.message = 'Choose some files to send'
         panel.options.clear()
         panel.options.append(iterm2.OpenPanel.Options.CAN_CHOOSE_FILES)
         if directory:
@@ -101,14 +106,15 @@
         event = threading.Event()
         future.add_done_callback(lambda x: event.set())
         event.wait()
         result = future.result()
         if result:
             return result.files
         return None
+    # pylint: disable-next=consider-using-f-string
     file_list = run_osascript('''(function () {
         const app = Application("iTerm2");
         app.includeStandardAdditions = true;
         app.activate();
         try {
             var files = app.%s({
                 withPrompt: "Choose some files to send",
@@ -123,160 +129,177 @@
             return file_list;
         } catch (e) {
             return "";
         }
     })();''' % ('chooseFolder' if directory else 'chooseFile'))
     return [f for f in file_list.split('\n') if f]
 
+
 def download_files(args, loop, connection, session, remote_is_windows):
     dest_path = args.destpath or choose_download_path(loop, connection)
 
     if not dest_path:
-        send_action(False, __version__, remote_is_windows)
+        transfer.send_action(False, __version__, remote_is_windows)
         return
 
-    check_path_writable(dest_path)
+    utils.check_path_writable(dest_path)
 
-    reconfigure_stdin()
+    utils.reconfigure_stdin()
 
-    send_action(True, __version__, remote_is_windows)
-    config = recv_config()
+    transfer.send_action(True, __version__, remote_is_windows)
+    config = transfer.recv_config()
 
     callback = None
-    if not config.get('quiet', False):
-        if args.progress == ProgressType.text and loop and session:
-            callback = TextProgressBar(loop, session, config.get('tmux_pane_width'))
+    if not config.quiet:
+        if args.progress == ProgressType.TEXT and loop and session:
+            callback = TextProgressBar(loop, session, config.tmux_pane_width)
         else:
             callback = ZenityProgressBar('Download')
 
-    local_list = recv_files(dest_path, callback)
+    local_list = transfer.recv_files(dest_path, callback)
+
+    transfer.client_exit(utils.format_saved_files(local_list, dest_path))
+
+
+class GlobalVariables:
+
+    def __init__(self):
+        self.upload_file_list = None
+
 
-    client_exit('Saved %s to %s' % (', '.join(local_list), dest_path))
+GLOBAL = GlobalVariables()
 
-upload_file_list = None
 
-def upload_files(args, loop, connection, session, directory, remote_is_windows):
-    global upload_file_list
-    if upload_file_list:
-        file_list = upload_file_list
-        upload_file_list = None
+def upload_files(args, loop, connection, session, directory, remote_is_windows):  # pylint: disable=too-many-arguments
+    if GLOBAL.upload_file_list:
+        file_list = GLOBAL.upload_file_list
+        GLOBAL.upload_file_list = None
     else:
         paths = choose_upload_paths(loop, connection, directory)
         if not paths:
-            send_action(False, __version__, remote_is_windows)
+            transfer.send_action(False, __version__, remote_is_windows)
             return
-        file_list = check_paths_readable(paths, directory)
+        file_list = utils.check_paths_readable(paths, directory)
 
-    reconfigure_stdin()
+    utils.reconfigure_stdin()
 
-    send_action(True, __version__, remote_is_windows)
-    config = recv_config()
+    transfer.send_action(True, __version__, remote_is_windows)
+    config = transfer.recv_config()
 
-    if config.get('overwrite') is True:
-        check_duplicate_names(file_list)
+    if config.overwrite is True:
+        utils.check_duplicate_names(file_list)
 
     callback = None
-    if not config.get('quiet', False):
-        if args.progress == ProgressType.text and loop and session:
-            callback = TextProgressBar(loop, session, config.get('tmux_pane_width'))
+    if not config.quiet:
+        if args.progress == ProgressType.TEXT and loop and session:
+            callback = TextProgressBar(loop, session, config.tmux_pane_width)
         else:
             callback = ZenityProgressBar('Upload')
 
-    remote_list = send_files(file_list, callback)
+    remote_list = transfer.send_files(file_list, callback)
+
+    transfer.client_exit(utils.format_saved_files(remote_list, ''))
 
-    client_exit('Received %s' % ', '.join(remote_list))
 
 async def keystroke_filter(connection, session):
     all_keys = iterm2.KeystrokePattern()
     all_keys.keycodes = list(iterm2.Keycode)
-    filter = iterm2.KeystrokeFilter(connection, [all_keys], session.session_id)
-    async with filter as mon:
+    async with iterm2.KeystrokeFilter(connection, [all_keys], session.session_id):
         while True:
             await asyncio.sleep(1)
 
+
 async def keystroke_monitor(connection, session):
     async with iterm2.KeystrokeMonitor(connection) as mon:
         while True:
             keystroke = await mon.async_get()
             if keystroke.characters == '\x03':
                 app = await iterm2.async_get_app(connection)
                 current_session = app.current_window.current_tab.current_session
                 if current_session.session_id == session.session_id:
-                    stop_transferring()
+                    utils.stop_transferring()
+
 
 async def get_running_session(force):
     session_id = os.environ.get('ITERM_SESSION_ID')
     if not session_id:
         if force:
-            raise TrzszError('Please upgrade iTerm2', trace=False)
+            raise utils.TrzszError('Please upgrade iTerm2', trace=False)
         return None, None
     try:
         connection = await iterm2.Connection.async_create()
         app = await iterm2.async_get_app(connection)
         current_session = app.current_window.current_tab.current_session
         if current_session.session_id in session_id:
             return connection, current_session
         for win in app.windows:
             for tab in win.tabs:
                 for session in tab.sessions:
                     if session.session_id in session_id:
                         return connection, session
     except Exception:
         if force:
-            raise TrzszError('Please enable iTerm2 Python API', trace=False)
+            raise utils.TrzszError('Please enable iTerm2 Python API', trace=False)
         return None, None
     if force:
-        raise TrzszError("Can't find the session in iTerm2", trace=False)
+        raise utils.TrzszError("Can't find the session in iTerm2", trace=False)
     return None, None
 
+
 def unique_id_exists(unique_id):
     if not unique_id or len(unique_id) < 8:
         return False
     if len(unique_id) == 14 and unique_id.endswith('00'):
         return False
     unique_id = unique_id[1:] + '\n'
     unique_id_path = os.path.join(tempfile.gettempdir(), 'trzsz_unique_id')
     try:
-        unique_id_list = open(unique_id_path, 'r').readlines()
+        with open(unique_id_path, 'r', encoding='utf8') as file:
+            unique_id_list = file.readlines()
     except EnvironmentError:
         unique_id_list = []
     if unique_id in unique_id_list:
         return True
     try:
         unique_id_list.append(unique_id)
-        open(unique_id_path, 'w').writelines(unique_id_list[-50:])
+        with open(unique_id_path, 'w', encoding='utf8') as file:
+            file.writelines(unique_id_list[-50:])
     except EnvironmentError:
         pass
     return False
 
+
 def side_thread(loop):
     asyncio.set_event_loop(loop)
     loop.run_forever()
 
+
 def read_server_output(timeout):
     output = []
     while True:
-        r, w, x = select.select([sys.stdin], [], [], timeout)
-        if not r:
+        rlist, _wlist, _xlist = select.select([sys.stdin], [], [], timeout)
+        if not rlist:
             break
-        out = os.read(sys.stdin.fileno(), 10240)
+        out = os.read(sys.stdin.fileno(), 32 * 1024)
         if not out:
             break
         output.append(out)
     return b''.join(output)
 
-trzsz_trigger_regex = r':TRZSZ:TRANSFER:([SRD]):(\d+\.\d+\.\d+)(:\d+)?'
+
+TRZSZ_TRIGGER_REGEX = r':TRZSZ:TRANSFER:([SRD]):(\d+\.\d+\.\d+)(:\d+)?'
+
 
 def drag_files_to_upload(file_paths, loop, session):
     if not loop or not session:
         sys.stderr.write('Please enable iTerm2 Python API')
         return None
 
     try:
-        file_list = check_paths_readable(file_paths, True)
+        file_list = utils.check_paths_readable(file_paths, True)
 
         sys.stdout.write('\x03')
         sys.stdout.flush()
         read_server_output(0.2)
 
         has_dir = False
         for file in file_list:
@@ -285,85 +308,85 @@
                 break
         if has_dir:
             sys.stdout.write('trz -d\r')
         else:
             sys.stdout.write('trz\r')
         sys.stdout.flush()
 
-        for i in range(20):
+        for _ in range(20):
             output = read_server_output(0.05)
             idx = output.find(b'\n')
             if idx > 0 and output[:idx].rstrip() in (b'trz', b'trz -d'):
                 output = b'\r\n' + output[idx + 1:]
-            trigger_match = re.search(trzsz_trigger_regex, output.decode('ascii'))
+            trigger_match = re.search(TRZSZ_TRIGGER_REGEX, output.decode('latin1'))
             if trigger_match:
                 loop.create_task(session.async_inject(output.replace(b'TRANSFER', b'DRAGFILE')))
-                global upload_file_list
-                upload_file_list = file_list
+                GLOBAL.upload_file_list = file_list
                 return trigger_match
             loop.create_task(session.async_inject(output))
         return None
 
-    except Exception as e:
-        sys.stderr.write(TrzszError.get_err_msg(e))
+    except Exception as ex:
+        sys.stderr.write(utils.TrzszError.get_err_msg(ex))
         return None
 
+
 def main():
     try:
-        parser = argparse.ArgumentParser(description='iTerm2 coprocess of trzsz which similar to lrzsz ' \
-                                                     '( rz / sz ) and compatible with tmux.')
+        parser = argparse.ArgumentParser(description='iTerm2 coprocess of trzsz which similar to lrzsz '
+                                         '( rz / sz ) and compatible with tmux.')
         parser.add_argument('-v', '--version', action='version', version='%(prog)s (trzsz) py ' + __version__)
         parser.add_argument('-p',
                             '--progress',
                             type=ProgressType,
                             choices=list(ProgressType),
-                            default=ProgressType.zenity,
+                            default=ProgressType.ZENITY,
                             help='the progress bar type. (default: zenity)')
         parser.add_argument('-d',
                             '--destpath',
                             type=str,
                             default=None,
                             help='the default save destination path. (default: choose each time)')
         parser.add_argument('args', nargs='+', help='iTerm2 trigger parameters. (generally should be \\1)')
         args = parser.parse_args()
 
         loop = asyncio.new_event_loop()
-        force = args.progress == ProgressType.text and args.args[0] != 'dragfiles'
+        force = args.progress == ProgressType.TEXT and args.args[0] != 'dragfiles'
         connection, session = loop.run_until_complete(get_running_session(force))
         if connection and session:
             thread = threading.Thread(target=side_thread, args=(loop, ), daemon=True)
             thread.start()
             asyncio.run_coroutine_threadsafe(keystroke_filter(connection, session), loop)
             asyncio.run_coroutine_threadsafe(keystroke_monitor(connection, session), loop)
 
         if len(args.args) > 1 and args.args[0] == 'dragfiles':
             trigger_match = drag_files_to_upload(args.args[1:], loop, session)
             if not trigger_match:
                 return
         else:
-            trigger_match = re.search(trzsz_trigger_regex, args.args[0])
+            trigger_match = re.search(TRZSZ_TRIGGER_REGEX, args.args[0])
             if not trigger_match:
-                raise TrzszError('Please check iTerm2 Trigger configuration', trace=False)
+                raise utils.TrzszError('Please check iTerm2 Trigger configuration', trace=False)
 
         mode = trigger_match.group(1)
-        version = trigger_match.group(2)
         unique_id = trigger_match.group(3)
         remote_is_windows = False
         if unique_id == ':1' or (len(unique_id) == 14 and unique_id.endswith('10')):
             remote_is_windows = True
 
         if unique_id_exists(unique_id):
             return
         if mode == 'S':
             download_files(args, loop, connection, session, remote_is_windows)
         elif mode == 'R':
             upload_files(args, loop, connection, session, False, remote_is_windows)
         elif mode == 'D':
             upload_files(args, loop, connection, session, True, remote_is_windows)
         else:
-            raise TrzszError('Unknown transfer mode: %s' % mode, trace=False)
+            raise utils.TrzszError(f'Unknown transfer mode: {mode}', trace=False)
+
+    except Exception as ex:
+        transfer.client_error(ex)
 
-    except Exception as e:
-        client_error(e)
 
 if __name__ == '__main__':
     main()
```

### Comparing `trzsz-iterm2-1.1.2/trzsz/iterm2/text_progress.py` & `trzsz-iterm2-1.1.3/trzsz/iterm2/text_progress.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,42 +17,43 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import time
-from trzsz.libs.utils import TrzszCallback
+from trzsz.libs import utils
 
-def display_length(s):
-    l = 0
-    for c in s:
-        l += 1 if len(c.encode('utf8')) == 1 else 2
-    return l
-
-def ellipsis_string(s, m):
-    m -= 3
-    l = 0
-    r = []
-    for c in s:
-        if len(c.encode('utf8')) > 1:
-            if l + 2 > m:
+
+def display_length(output):
+    length = 0
+    for char in output:
+        length += 1 if len(char.encode('utf8')) == 1 else 2
+    return length
+
+
+def ellipsis_string(text, max_len):
+    max_len -= 3
+    length = 0
+    result = []
+    for char in text:
+        if len(char.encode('utf8')) > 1:
+            if length + 2 > max_len:
                 break
-            l += 2
+            length += 2
         else:
-            if l + 1 > m:
+            if length + 1 > max_len:
                 break
-            l += 1
-        r.append(c)
-    r.append('...')
-    return ''.join(r), l + 3
+            length += 1
+        result.append(char)
+    result.append('...')
+    return ''.join(result), length + 3
+
 
 def size_to_str(size):
-    if size < 0:
-        return 'NaN'
     unit = 'B'
     while True:
         if size < 1024:
             break
         size = size / 1024
         unit = 'KB'
         if size < 1024:
@@ -65,35 +66,37 @@
         unit = 'GB'
         if size < 1024:
             break
         size = size / 1024
         unit = 'TB'
         break
     if size >= 100:
-        return f'{size:.0f}{unit}'
+        return f'{size:.0f} {unit}'
     if size >= 10:
-        return f'{size:.1f}{unit}'
-    return f'{size:.2f}{unit}'
+        return f'{size:.1f} {unit}'
+    return f'{size:.2f} {unit}'
+
 
 def time_to_str(seconds):
-    if seconds < 0:
-        return 'NaN'
     result = ''
     if seconds >= 3600:
         result += str(int(seconds / 3600)) + ':'
         seconds %= 3600
     minute = int(seconds / 60)
     result += (str(minute) if minute >= 10 else ('0' + str(minute))) + ':'
     second = round(seconds % 60)
     result += str(second) if second >= 10 else ('0' + str(second))
     return result
 
-SPEED_ARRAY_SIZE = 10
 
-class TextProgressBar(TrzszCallback):
+SPEED_ARRAY_SIZE = 30
+
+
+class TextProgressBar(utils.TrzszCallback):  # pylint: disable=too-many-instance-attributes
+
     def __init__(self, loop, session, tmux_pane_width=None):
         self.num = 0
         self.idx = 0
         self.name = ''
         self.size = 0
         self.step = 0
         self.start_time = 0
@@ -101,58 +104,64 @@
         self.first_write = True
         self.speed_cnt = 0
         self.speed_idx = 0
         self.time_array = [0] * SPEED_ARRAY_SIZE
         self.step_array = [0] * SPEED_ARRAY_SIZE
         self.loop = loop
         self.session = session
-        self.tmux_pane_width = tmux_pane_width or -1
+        self.tmux_pane_width = tmux_pane_width or 0
         self.columns = self.tmux_pane_width if self.tmux_pane_width > 0 else session.grid_size.width
 
     def on_num(self, num):
         self.num = num
 
     def on_name(self, name):
         self.name = name
         self.idx += 1
         self.start_time = time.time()
         self.time_array[0] = self.start_time
         self.step_array[0] = 0
         self.speed_cnt = 1
         self.speed_idx = 1
+        self.step = -1
 
     def on_size(self, size):
         self.size = size
 
     def on_step(self, step):
+        if step <= self.step:
+            return
         self.step = step
         self._show_progress()
 
     def on_done(self):
         if not self.first_write:
             if self.tmux_pane_width > 0:
                 self._inject_to_iterm2(f'\x1b[{self.columns}D')
             else:
                 self._inject_to_iterm2('\r')
             self.first_write = True
 
     def _show_progress(self):
         now = time.time()
-        if now - self.update_time < 0.5:
+        if now - self.update_time < 0.2:
             return
         self.update_time = now
 
-        if self.size == 0:
-            return
-        percentage = str(round(self.step * 100 / self.size)) + '%'
+        percentage = "100%"
+        if self.size != 0:
+            percentage = str(round(self.step * 100 / self.size)) + '%'
         total = size_to_str(self.step)
         speed = self._get_speed(now)
-        speed_str = size_to_str(speed) + '/s'
-        eta = time_to_str(round((self.size - self.step) / speed)) + ' ETA'
-        progress_text = self._progress_text(percentage, total, speed_str, eta)
+        speed_str = '--- B/s'
+        eta_str = '--- ETA'
+        if speed > 0:
+            speed_str = size_to_str(speed) + '/s'
+            eta_str = time_to_str(round((self.size - self.step) / speed)) + ' ETA'
+        progress_text = self._progress_text(percentage, total, speed_str, eta_str)
 
         if self.first_write:
             self.first_write = False
             self._inject_to_iterm2(progress_text)
             return
         if self.tmux_pane_width > 0:
             self._inject_to_iterm2(f'\x1b[{self.columns}D{progress_text}')
@@ -174,15 +183,15 @@
 
         self.speed_idx += 1
         if self.speed_idx >= SPEED_ARRAY_SIZE:
             self.speed_idx %= SPEED_ARRAY_SIZE
 
         return speed
 
-    def _progress_text(self, percentage, total, speed, eta):
+    def _progress_text(self, percentage, total, speed, eta):  # pylint: disable=too-many-branches
         bar_min_len = 24
         left = f'({self.idx}/{self.num}) {self.name}' if self.num > 1 else self.name
         left_len = display_length(left)
         right = f' {percentage} | {total} | {speed} | {eta}'
         while True:
             if self.columns - left_len - len(right) >= bar_min_len:
                 break
@@ -219,12 +228,14 @@
             left += ' '
         return (left + self._progress_bar(bar_len) + right).strip()
 
     def _progress_bar(self, bar_len):
         if bar_len < 12:
             return ''
         total = bar_len - 2
-        complete = round(total * self.step / self.size)
+        complete = total
+        if self.size != 0:
+            complete = round(total * self.step / self.size)
         return '[\u001b[36m' + '\u2588' * complete + '\u2591' * (total - complete) + '\u001b[0m]'
 
     def _inject_to_iterm2(self, data):
         self.loop.create_task(self.session.async_inject(data.encode('utf8')))
```

### Comparing `trzsz-iterm2-1.1.2/trzsz/iterm2/zenity_progress.py` & `trzsz-iterm2-1.1.3/trzsz/iterm2/zenity_progress.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,17 +17,19 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import subprocess
-from trzsz.libs.utils import stop_transferring, TrzszCallback
+from trzsz.libs import utils
+
+
+class ZenityProgressBar(utils.TrzszCallback):
 
-class ZenityProgressBar(TrzszCallback):
     def __init__(self, action):
         self.num = 0
         self.idx = 0
         self.name = ''
         self.size = 0
         self.proc = None
         self.action = action
@@ -37,26 +39,26 @@
         if self.proc:
             self.proc.terminate()
             self.proc = None
 
     def on_num(self, num):
         self.num = num
         try:
-            title = '%s file(s)' % self.action
+            title = f'{self.action} file(s)'
+            # pylint: disable-next=consider-using-with
             self.proc = subprocess.Popen(['/usr/local/bin/zenity', '--progress', '--title', title, '--text', ''],
                                          stdin=subprocess.PIPE,
                                          stdout=subprocess.PIPE,
                                          stderr=subprocess.PIPE)
         except EnvironmentError:
             pass
 
     def _update_progress(self, step):
         percentage = step * 100 // self.size if self.size else 0
-        progress = '%d\n# %sing %s %d%% ( %d / %d ) ...\n' \
-                   % (percentage, self.action, self.name, percentage, self.idx, self.num)
+        progress = f'{percentage}\n# {self.action}ing {self.name} {percentage}% ( {self.idx} / {self.num} ) ...\n'
         if progress == self.progress:
             return
         self.progress = progress
         self.proc.stdin.write(progress.encode('utf8'))
         self.proc.stdin.flush()
 
     def on_name(self, name):
@@ -64,33 +66,33 @@
         self.size = 0
         self.name = name
         if not self.proc:
             return
         try:
             self._update_progress(0)
         except EnvironmentError:
-            stop_transferring()
+            utils.stop_transferring()
 
     def on_size(self, size):
         self.size = size
 
     def on_step(self, step):
         if not self.proc:
             return
         try:
             self._update_progress(step)
         except EnvironmentError:
             if self.idx < self.num or step < self.size:
-                stop_transferring()
+                utils.stop_transferring()
 
     def on_done(self):
         if not self.proc:
             return
         try:
-            self.proc.stdin.write(('# %s %s finished.\n' % (self.action, self.name)).encode('utf8'))
+            self.proc.stdin.write(f'# {self.action} {self.name} finished.\n'.encode('utf8'))
             self.proc.stdin.flush()
         except EnvironmentError:
             if self.idx < self.num:
-                stop_transferring()
+                utils.stop_transferring()
         if self.idx == self.num:
             self.proc.terminate()
             self.proc = None
```

### Comparing `trzsz-iterm2-1.1.2/trzsz_iterm2.egg-info/PKG-INFO` & `trzsz-iterm2-1.1.3/trzsz_iterm2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trzsz-iterm2
-Version: 1.1.2
+Version: 1.1.3
 Summary: trzsz is a simple file transfer tools, similar to lrzsz ( rz / sz ) and compatible with tmux, which works with iTerm2 and has a nice progress bar.
 Home-page: https://trzsz.github.io
 Author: Lonny Wong
 Author-email: lonnywong@qq.com
 License: MIT License
 Keywords: trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar
 Classifier: Development Status :: 5 - Production/Stable
```

