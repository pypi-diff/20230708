# Comparing `tmp/pyams_sequence-1.2.3.tar.gz` & `tmp/pyams_sequence-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_sequence-1.2.3.tar", last modified: Thu Apr 13 12:32:47 2023, max compression
+gzip compressed data, was "dist/pyams_sequence-1.2.4.tar", last modified: Fri Jul  7 21:58:54 2023, max compression
```

## Comparing `pyams_sequence-1.2.3.tar` & `pyams_sequence-1.2.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2710 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/docs/
--rwxrwxrwx   0 root         (0) root         (0)      773 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2648 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/api/
--rw-rw-rw-   0 root         (0) root         (0)     1475 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4111 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/api/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    10379 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1988 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/include.py
--rw-rw-rw-   0 root         (0) root         (0)     4882 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2938 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po
--rw-rw-rw-   0 root         (0) root         (0)     2607 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/locales/pyams_sequence.pot
--rw-rw-rw-   0 root         (0) root         (0)     4616 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/sequence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/tests/
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     6172 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/widget/
--rw-rw-rw-   0 root         (0) root         (0)     3604 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/widget/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2748 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2134 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1421 2023-04-13 12:32:26.000000 pyams_sequence-1.2.3/src/pyams_sequence/zmi/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2710 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1201 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      288 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-13 12:32:47.000000 pyams_sequence-1.2.3/src/pyams_sequence.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      862 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2648 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence/
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4143 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    10379 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     4882 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/locales/pyams_sequence.pot
+-rw-rw-rw-   0 root         (0) root         (0)     4616 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/sequence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6172 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence/widget/
+-rw-rw-rw-   0 root         (0) root         (0)     3604 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/widget/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2023-07-07 21:58:36.000000 pyams_sequence-1.2.4/src/pyams_sequence/zmi/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-07-07 21:58:53.000000 pyams_sequence-1.2.4/src/pyams_sequence.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-07 21:58:54.000000 pyams_sequence-1.2.4/src/pyams_sequence.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:58:53.000000 pyams_sequence-1.2.4/src/pyams_sequence.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:58:53.000000 pyams_sequence-1.2.4/src/pyams_sequence.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 21:58:53.000000 pyams_sequence-1.2.4/src/pyams_sequence.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      288 2023-07-07 21:58:53.000000 pyams_sequence-1.2.4/src/pyams_sequence.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-07 21:58:53.000000 pyams_sequence-1.2.4/src/pyams_sequence.egg-info/top_level.txt
```

### Comparing `pyams_sequence-1.2.3/LICENSE` & `pyams_sequence-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/PKG-INFO` & `pyams_sequence-1.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_sequence
-Version: 1.2.3
+Version: 1.2.4
 Summary: PyAMS sequences management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -52,14 +52,20 @@
 Custom schemas fields and forms widgets are available to select internal references into
 content management interface.
 
 
 Changelog
 =========
 
+1.2.4
+-----
+ - REST API update
+ - updated permissions
+ - updated sequence target getter
+
 1.2.3
 -----
  - added support for Python 3.10 and 3.11
  - updated Colander API schemas for better OpenAPI specifications
 
 1.2.2
 -----
```

### Comparing `pyams_sequence-1.2.3/docs/HISTORY.rst` & `pyams_sequence-1.2.4/docs/HISTORY.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.2.4
+-----
+ - REST API update
+ - updated permissions
+ - updated sequence target getter
+
 1.2.3
 -----
  - added support for Python 3.10 and 3.11
  - updated Colander API schemas for better OpenAPI specifications
 
 1.2.2
 -----
```

### Comparing `pyams_sequence-1.2.3/docs/README.rst` & `pyams_sequence-1.2.4/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/setup.py` & `pyams_sequence-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.2.3'
+version = '1.2.4'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/__init__.py` & `pyams_sequence-1.2.4/src/pyams_sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/api/__init__.py` & `pyams_sequence-1.2.4/src/pyams_sequence/api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 """PyAMS_sequence.skin main module
 
 This module provides references search function.
 """
 
 from pyramid.view import view_config
 
-from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
+from pyams_security.interfaces.base import USE_INTERNAL_API_PERMISSION
 from pyams_sequence.interfaces import ISequentialIntIds
 from pyams_sequence.sequence import get_sequence_dict
 from pyams_utils.registry import get_utility
 
-
 __docformat__ = 'restructuredtext'
 
 
-@view_config(name='find-references.json', permission=VIEW_SYSTEM_PERMISSION,
+@view_config(name='find-references.json',
+             permission=USE_INTERNAL_API_PERMISSION,
              renderer='json', xhr=True)
 def find_references(request):
     """Find all references matching given query"""
     query = request.params.get('term')
     if not query:
         return []
     sequence = get_utility(ISequentialIntIds)
```

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/api/rest.py` & `pyams_sequence-1.2.4/src/pyams_sequence/api/rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 
 """PyAMS_sequence.api.reference module
 
-This modules defines REST API used to search internal references.
+This module defines REST API used to search internal references.
 """
 
 import sys
 
 from colander import MappingSchema, SchemaNode, SequenceSchema, String, drop
 from cornice import Service
 from cornice.validators import colander_validator
 from pyramid.httpexceptions import HTTPOk
 
-from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
+from pyams_security.interfaces.base import USE_INTERNAL_API_PERMISSION
 from pyams_security.rest import check_cors_origin, set_cors_headers
 from pyams_sequence.interfaces import ISequentialIntIds, REST_REFERENCES_SEARCH_ROUTE
 from pyams_sequence.sequence import get_sequence_dict
 from pyams_utils.registry import query_utility
 from pyams_utils.rest import BaseResponseSchema, STATUS, rest_responses
 
 
@@ -87,21 +87,21 @@
 
 
 references_get_responses = rest_responses.copy()
 references_get_responses[HTTPOk.code] = ReferencesGetResponse(
     description="References search results")
 
 
-@references_service.get(permission=VIEW_SYSTEM_PERMISSION,
+@references_service.get(permission=USE_INTERNAL_API_PERMISSION,
                         schema=ReferencesGetRequest(),
                         validators=(check_cors_origin, colander_validator, set_cors_headers),
                         response_schemas=references_get_responses)
 def find_references(request):
     """Returns list of references matching given query"""
-    params = request.params if TEST_MODE else request.validated
+    params = request.params if TEST_MODE else request.validated.get('querystring', {})
     query = params.get('term')
     if not query:
         return {
             'status': STATUS.ERROR.value,
             'message': 'Missing arguments',
             'results': []
         }
```

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/doctests/README.rst` & `pyams_sequence-1.2.4/src/pyams_sequence/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/generations/__init__.py` & `pyams_sequence-1.2.4/src/pyams_sequence/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/include.py` & `pyams_sequence-1.2.4/src/pyams_sequence/include.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/interfaces.py` & `pyams_sequence-1.2.4/src/pyams_sequence/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo` & `pyams_sequence-1.2.4/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.mo`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po` & `pyams_sequence-1.2.4/src/pyams_sequence/locales/fr/LC_MESSAGES/pyams_sequence.po`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/locales/pyams_sequence.pot` & `pyams_sequence-1.2.4/src/pyams_sequence/locales/pyams_sequence.pot`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/reference.py` & `pyams_sequence-1.2.4/src/pyams_sequence/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/schema.py` & `pyams_sequence-1.2.4/src/pyams_sequence/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/sequence.py` & `pyams_sequence-1.2.4/src/pyams_sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/tests/__init__.py` & `pyams_sequence-1.2.4/src/pyams_sequence/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/tests/test_utilsdocs.py` & `pyams_sequence-1.2.4/src/pyams_sequence/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/tests/test_utilsdocstrings.py` & `pyams_sequence-1.2.4/src/pyams_sequence/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/utility.py` & `pyams_sequence-1.2.4/src/pyams_sequence/utility.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/widget/__init__.py` & `pyams_sequence-1.2.4/src/pyams_sequence/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/widget/interfaces.py` & `pyams_sequence-1.2.4/src/pyams_sequence/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/workflow.py` & `pyams_sequence-1.2.4/src/pyams_sequence/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,17 @@
         if versions:
             content = versions[-1]
     if ISequentialIdInfo(content, None) is not None:
         return content
     return None
 
 
-def get_sequence_target(oid, state):
+def get_sequence_target(oid, state=None):
     """Get content matching given OID"""
     sequence = get_utility(ISequentialIntIds)
     content = sequence.query_object_from_oid(oid)
-    if IWorkflowVersion.providedBy(content) or IWorkflowManagedContent.providedBy(content):
+    if state and (IWorkflowVersion.providedBy(content) or IWorkflowManagedContent.providedBy(content)):
         versions = IWorkflowVersions(content).get_versions(state, sort=True)  # pylint: disable=assignment-from-no-return
         if versions:
             content = versions[0]
             return content
     return content
```

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/zmi/__init__.py` & `pyams_sequence-1.2.4/src/pyams_sequence/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence/zmi/reference.py` & `pyams_sequence-1.2.4/src/pyams_sequence/zmi/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence.egg-info/PKG-INFO` & `pyams_sequence-1.2.4/src/pyams_sequence.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-sequence
-Version: 1.2.3
+Version: 1.2.4
 Summary: PyAMS sequences management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -52,14 +52,20 @@
 Custom schemas fields and forms widgets are available to select internal references into
 content management interface.
 
 
 Changelog
 =========
 
+1.2.4
+-----
+ - REST API update
+ - updated permissions
+ - updated sequence target getter
+
 1.2.3
 -----
  - added support for Python 3.10 and 3.11
  - updated Colander API schemas for better OpenAPI specifications
 
 1.2.2
 -----
```

### Comparing `pyams_sequence-1.2.3/src/pyams_sequence.egg-info/SOURCES.txt` & `pyams_sequence-1.2.4/src/pyams_sequence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

