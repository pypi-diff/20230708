# Comparing `tmp/ua-parser-0.8.0.tar.gz` & `tmp/ua-parser-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ua-parser-0.8.0.tar", last modified: Mon Apr  9 17:04:15 2018, max compression
+gzip compressed data, was "dist/ua-parser-0.9.0.tar", last modified: Tue Feb  4 16:29:44 2020, max compression
```

## Comparing `ua-parser-0.8.0.tar` & `ua-parser-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2018-04-09 17:04:15.000000 ua-parser-0.8.0/
--rw-r--r--   0 matt       (501) staff       (20)     1242 2018-04-09 17:04:15.000000 ua-parser-0.8.0/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)       37 2016-06-20 15:21:16.000000 ua-parser-0.8.0/MANIFEST.in
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2018-04-09 17:04:15.000000 ua-parser-0.8.0/ua_parser.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     1242 2018-04-09 17:04:14.000000 ua-parser-0.8.0/ua_parser.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)        1 2018-04-09 17:04:14.000000 ua-parser-0.8.0/ua_parser.egg-info/not-zip-safe
--rw-r--r--   0 matt       (501) staff       (20)      300 2018-04-09 17:04:14.000000 ua-parser-0.8.0/ua_parser.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)       10 2018-04-09 17:04:14.000000 ua-parser-0.8.0/ua_parser.egg-info/top_level.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2018-04-09 17:04:14.000000 ua-parser-0.8.0/ua_parser.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)     8181 2018-04-09 17:00:45.000000 ua-parser-0.8.0/setup.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2018-04-09 17:04:15.000000 ua-parser-0.8.0/ua_parser/
--rw-r--r--   0 matt       (501) staff       (20)       20 2018-04-09 17:01:06.000000 ua-parser-0.8.0/ua_parser/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     9766 2015-12-22 00:43:32.000000 ua-parser-0.8.0/ua_parser/user_agent_parser_test.py
--rw-r--r--   0 matt       (501) staff       (20)   147302 2018-04-09 17:04:15.000000 ua-parser-0.8.0/ua_parser/_regexes.py
--rw-r--r--   0 matt       (501) staff       (20)    19496 2018-04-09 15:12:46.000000 ua-parser-0.8.0/ua_parser/user_agent_parser.py
--rw-r--r--   0 matt       (501) staff       (20)       88 2018-04-09 17:04:15.000000 ua-parser-0.8.0/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)     3372 2016-06-20 15:21:16.000000 ua-parser-0.8.0/README.rst
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2020-02-04 16:29:44.000000 ua-parser-0.9.0/
+-rw-r--r--   0 matt       (501) staff       (20)     1341 2020-02-04 16:29:44.000000 ua-parser-0.9.0/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)       63 2020-01-09 21:53:40.000000 ua-parser-0.9.0/MANIFEST.in
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2020-02-04 16:29:44.000000 ua-parser-0.9.0/ua_parser.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)     1341 2020-02-04 16:29:44.000000 ua-parser-0.9.0/ua_parser.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)        1 2020-02-04 16:29:44.000000 ua-parser-0.9.0/ua_parser.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (501) staff       (20)      318 2020-02-04 16:29:44.000000 ua-parser-0.9.0/ua_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)       10 2020-02-04 16:29:44.000000 ua-parser-0.9.0/ua_parser.egg-info/top_level.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2020-02-04 16:29:44.000000 ua-parser-0.9.0/ua_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)     8376 2020-02-04 16:29:03.000000 ua-parser-0.9.0/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2020-02-04 16:29:44.000000 ua-parser-0.9.0/ua_parser/
+-rw-r--r--   0 matt       (501) staff       (20)      550 2015-10-11 09:33:07.000000 ua-parser-0.9.0/ua_parser/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)       20 2020-02-04 16:29:13.000000 ua-parser-0.9.0/ua_parser/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)    10289 2020-01-09 22:09:48.000000 ua-parser-0.9.0/ua_parser/user_agent_parser_test.py
+-rw-r--r--   0 matt       (501) staff       (20)   157838 2020-02-04 16:29:44.000000 ua-parser-0.9.0/ua_parser/_regexes.py
+-rw-r--r--   0 matt       (501) staff       (20)    17936 2020-01-09 21:56:42.000000 ua-parser-0.9.0/ua_parser/user_agent_parser.py
+-rw-r--r--   0 matt       (501) staff       (20)       67 2020-02-04 16:29:44.000000 ua-parser-0.9.0/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)     3372 2016-06-20 15:21:16.000000 ua-parser-0.9.0/README.rst
```

### Comparing `ua-parser-0.8.0/PKG-INFO` & `ua-parser-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.1
 Name: ua-parser
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python port of Browserscope's user agent parser
 Home-page: https://github.com/ua-parser/uap-python
 Author: PBS
 Author-email: no-reply@pbs.org
-License: LICENSE.txt
+License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,9 +21,11 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `ua-parser-0.8.0/ua_parser.egg-info/PKG-INFO` & `ua-parser-0.9.0/ua_parser.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.1
 Name: ua-parser
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python port of Browserscope's user agent parser
 Home-page: https://github.com/ua-parser/uap-python
 Author: PBS
 Author-email: no-reply@pbs.org
-License: LICENSE.txt
+License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,9 +21,11 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `ua-parser-0.8.0/ua_parser/user_agent_parser_test.py` & `ua-parser-0.9.0/ua_parser/user_agent_parser_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,232 +21,270 @@
 or like:
 # python -m user_agent_parser_test ParseTest.testBrowserscopeStrings
 """
 
 
 from __future__ import unicode_literals, absolute_import
 
-__author__ = 'slamm@google.com (Stephen Lamm)'
+__author__ = "slamm@google.com (Stephen Lamm)"
 
 import os
 import re
 import unittest
 import yaml
 
+try:
+    # Try and use libyaml bindings if available since faster
+    from yaml import CSafeLoader as SafeLoader
+except ImportError:
+    from yaml import SafeLoader
+
 from ua_parser import user_agent_parser
 
-TEST_RESOURCES_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)),
-                                  '../uap-core')
+TEST_RESOURCES_DIR = os.path.join(
+    os.path.abspath(os.path.dirname(__file__)), "../uap-core"
+)
 
 
 class ParseTest(unittest.TestCase):
     def testBrowserscopeStrings(self):
-        self.runUserAgentTestsFromYAML(os.path.join(
-            TEST_RESOURCES_DIR, 'tests/test_ua.yaml'))
+        self.runUserAgentTestsFromYAML(
+            os.path.join(TEST_RESOURCES_DIR, "tests/test_ua.yaml")
+        )
 
     def testBrowserscopeStringsOS(self):
-        self.runOSTestsFromYAML(os.path.join(
-            TEST_RESOURCES_DIR, 'tests/test_os.yaml'))
+        self.runOSTestsFromYAML(os.path.join(TEST_RESOURCES_DIR, "tests/test_os.yaml"))
 
     def testStringsOS(self):
-        self.runOSTestsFromYAML(os.path.join(
-            TEST_RESOURCES_DIR, 'test_resources/additional_os_tests.yaml'))
+        self.runOSTestsFromYAML(
+            os.path.join(TEST_RESOURCES_DIR, "test_resources/additional_os_tests.yaml")
+        )
 
     def testStringsDevice(self):
-        self.runDeviceTestsFromYAML(os.path.join(
-            TEST_RESOURCES_DIR, 'tests/test_device.yaml'))
+        self.runDeviceTestsFromYAML(
+            os.path.join(TEST_RESOURCES_DIR, "tests/test_device.yaml")
+        )
 
     def testMozillaStrings(self):
-        self.runUserAgentTestsFromYAML(os.path.join(
-            TEST_RESOURCES_DIR, 'test_resources/firefox_user_agent_strings.yaml'))
+        self.runUserAgentTestsFromYAML(
+            os.path.join(
+                TEST_RESOURCES_DIR, "test_resources/firefox_user_agent_strings.yaml"
+            )
+        )
 
     # NOTE: The YAML file used here is one output by makePGTSComparisonYAML()
     # below, as opposed to the pgts_browser_list-orig.yaml file.  The -orig
     # file is by no means perfect, but identifies many browsers that we
     # classify as "Other".  This test itself is mostly useful to know when
     # somthing in UA parsing changes.  An effort should be made to try and
     # reconcile the differences between the two YAML files.
     def testPGTSStrings(self):
-        self.runUserAgentTestsFromYAML(os.path.join(
-            TEST_RESOURCES_DIR, 'test_resources/pgts_browser_list.yaml'))
+        self.runUserAgentTestsFromYAML(
+            os.path.join(TEST_RESOURCES_DIR, "test_resources/pgts_browser_list.yaml")
+        )
 
     def testParseAll(self):
-        user_agent_string = 'Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10.4; fr; rv:1.9.1.5) Gecko/20091102 Firefox/3.5.5,gzip(gfe),gzip(gfe)'
+        user_agent_string = "Mozilla/5.0 (Macintosh; U; Intel Mac OS X 10.4; fr; rv:1.9.1.5) Gecko/20091102 Firefox/3.5.5,gzip(gfe),gzip(gfe)"
         expected = {
-            'device': {
-                'family': 'Other',
-                'brand': None,
-                'model': None
-            },
-            'os': {
-                'family': 'Mac OS X',
-                'major': '10',
-                'minor': '4',
-                'patch': None,
-                'patch_minor': None
+            "device": {"family": "Other", "brand": None, "model": None},
+            "os": {
+                "family": "Mac OS X",
+                "major": "10",
+                "minor": "4",
+                "patch": None,
+                "patch_minor": None,
             },
-            'user_agent': {
-                'family': 'Firefox',
-                'major': '3',
-                'minor': '5',
-                'patch': '5'
+            "user_agent": {
+                "family": "Firefox",
+                "major": "3",
+                "minor": "5",
+                "patch": "5",
             },
-            'string': user_agent_string
+            "string": user_agent_string,
         }
 
         result = user_agent_parser.Parse(user_agent_string)
         self.assertEqual(
-            result, expected,
-            "UA: {0}\n expected<{1}> != actual<{2}>".format(user_agent_string, expected, result))
+            result,
+            expected,
+            "UA: {0}\n expected<{1}> != actual<{2}>".format(
+                user_agent_string, expected, result
+            ),
+        )
+
     # Make a YAML file for manual comparsion with pgts_browser_list-orig.yaml
     def makePGTSComparisonYAML(self):
         import codecs
-        outfile = codecs.open('outfile.yaml', 'w', 'utf-8')
+
+        outfile = codecs.open("outfile.yaml", "w", "utf-8")
         print >> outfile, "test_cases:"
 
-        yamlFile = open(os.path.join(TEST_RESOURCES_DIR,
-                                     'pgts_browser_list.yaml'))
-        yamlContents = yaml.load(yamlFile)
+        yamlFile = open(os.path.join(TEST_RESOURCES_DIR, "pgts_browser_list.yaml"))
+        yamlContents = yaml.load(yamlFile, Loader=SafeLoader)
         yamlFile.close()
 
-        for test_case in yamlContents['test_cases']:
-            user_agent_string = test_case['user_agent_string']
+        for test_case in yamlContents["test_cases"]:
+            user_agent_string = test_case["user_agent_string"]
             kwds = {}
-            if 'js_ua' in test_case:
-                kwds = eval(test_case['js_ua'])
+            if "js_ua" in test_case:
+                kwds = eval(test_case["js_ua"])
 
-            (family, major, minor, patch) = user_agent_parser.ParseUserAgent(user_agent_string, **kwds)
+            (family, major, minor, patch) = user_agent_parser.ParseUserAgent(
+                user_agent_string, **kwds
+            )
 
             # Escape any double-quotes in the UA string
             user_agent_string = re.sub(r'"', '\\"', user_agent_string)
-            print >> outfile, '    - user_agent_string: "' + user_agent_string + '"' + "\n" +\
-                              '      family: "' + family + "\"\n" +\
-                              "      major: " + ('' if (major is None) else "'" + major + "'") + "\n" +\
-                              "      minor: " + ('' if (minor is None) else "'" + minor + "'") + "\n" +\
-                              "      patch: " + ('' if (patch is None) else "'" + patch + "'")
+            print >> outfile, '    - user_agent_string: "' + user_agent_string + '"' + "\n" + '      family: "' + family + '"\n' + "      major: " + (
+                "" if (major is None) else "'" + major + "'"
+            ) + "\n" + "      minor: " + (
+                "" if (minor is None) else "'" + minor + "'"
+            ) + "\n" + "      patch: " + (
+                "" if (patch is None) else "'" + patch + "'"
+            )
         outfile.close()
 
     # Run a set of test cases from a YAML file
     def runUserAgentTestsFromYAML(self, file_name):
         yamlFile = open(os.path.join(TEST_RESOURCES_DIR, file_name))
-        yamlContents = yaml.load(yamlFile)
+        yamlContents = yaml.load(yamlFile, Loader=SafeLoader)
         yamlFile.close()
 
-        for test_case in yamlContents['test_cases']:
+        for test_case in yamlContents["test_cases"]:
             # Inputs to Parse()
-            user_agent_string = test_case['user_agent_string']
+            user_agent_string = test_case["user_agent_string"]
             kwds = {}
-            if 'js_ua' in test_case:
-                kwds = eval(test_case['js_ua'])
+            if "js_ua" in test_case:
+                kwds = eval(test_case["js_ua"])
 
             # The expected results
-            expected = {'family': test_case['family'],
-                        'major': test_case['major'],
-                        'minor': test_case['minor'],
-                        'patch': test_case['patch']}
+            expected = {
+                "family": test_case["family"],
+                "major": test_case["major"],
+                "minor": test_case["minor"],
+                "patch": test_case["patch"],
+            }
 
             result = {}
             result = user_agent_parser.ParseUserAgent(user_agent_string, **kwds)
             self.assertEqual(
-                result, expected,
+                result,
+                expected,
                 "UA: {0}\n expected<{1}, {2}, {3}, {4}> != actual<{5}, {6}, {7}, {8}>".format(
                     user_agent_string,
-                    expected['family'], expected['major'], expected['minor'], expected['patch'],
-                    result['family'], result['major'], result['minor'], result['patch']))
+                    expected["family"],
+                    expected["major"],
+                    expected["minor"],
+                    expected["patch"],
+                    result["family"],
+                    result["major"],
+                    result["minor"],
+                    result["patch"],
+                ),
+            )
 
     def runOSTestsFromYAML(self, file_name):
         yamlFile = open(os.path.join(TEST_RESOURCES_DIR, file_name))
-        yamlContents = yaml.load(yamlFile)
+        yamlContents = yaml.load(yamlFile, Loader=SafeLoader)
         yamlFile.close()
 
-        for test_case in yamlContents['test_cases']:
+        for test_case in yamlContents["test_cases"]:
             # Inputs to Parse()
-            user_agent_string = test_case['user_agent_string']
+            user_agent_string = test_case["user_agent_string"]
             kwds = {}
-            if 'js_ua' in test_case:
-                kwds = eval(test_case['js_ua'])
+            if "js_ua" in test_case:
+                kwds = eval(test_case["js_ua"])
 
             # The expected results
             expected = {
-                'family': test_case['family'],
-                'major': test_case['major'],
-                'minor': test_case['minor'],
-                'patch': test_case['patch'],
-                'patch_minor': test_case['patch_minor']
+                "family": test_case["family"],
+                "major": test_case["major"],
+                "minor": test_case["minor"],
+                "patch": test_case["patch"],
+                "patch_minor": test_case["patch_minor"],
             }
 
             result = user_agent_parser.ParseOS(user_agent_string, **kwds)
             self.assertEqual(
-                result, expected,
+                result,
+                expected,
                 "UA: {0}\n expected<{1} {2} {3} {4} {5}> != actual<{6} {7} {8} {9} {10}>".format(
                     user_agent_string,
-                    expected['family'],
-                    expected['major'],
-                    expected['minor'],
-                    expected['patch'],
-                    expected['patch_minor'],
-                    result['family'],
-                    result['major'],
-                    result['minor'],
-                    result['patch'],
-                    result['patch_minor']))
+                    expected["family"],
+                    expected["major"],
+                    expected["minor"],
+                    expected["patch"],
+                    expected["patch_minor"],
+                    result["family"],
+                    result["major"],
+                    result["minor"],
+                    result["patch"],
+                    result["patch_minor"],
+                ),
+            )
 
     def runDeviceTestsFromYAML(self, file_name):
         yamlFile = open(os.path.join(TEST_RESOURCES_DIR, file_name))
-        yamlContents = yaml.load(yamlFile)
+        yamlContents = yaml.load(yamlFile, Loader=SafeLoader)
         yamlFile.close()
 
-        for test_case in yamlContents['test_cases']:
+        for test_case in yamlContents["test_cases"]:
             # Inputs to Parse()
-            user_agent_string = test_case['user_agent_string']
+            user_agent_string = test_case["user_agent_string"]
             kwds = {}
-            if 'js_ua' in test_case:
-                kwds = eval(test_case['js_ua'])
+            if "js_ua" in test_case:
+                kwds = eval(test_case["js_ua"])
 
             # The expected results
             expected = {
-                'family': test_case['family'],
-                'brand': test_case['brand'],
-                'model': test_case['model']
+                "family": test_case["family"],
+                "brand": test_case["brand"],
+                "model": test_case["model"],
             }
 
             result = user_agent_parser.ParseDevice(user_agent_string, **kwds)
             self.assertEqual(
-                result, expected,
+                result,
+                expected,
                 "UA: {0}\n expected<{1} {2} {3}> != actual<{4} {5} {6}>".format(
                     user_agent_string,
-                    expected['family'],
-                    expected['brand'],
-                    expected['model'],
-                    result['family'],
-                    result['brand'],
-                    result['model']))
+                    expected["family"],
+                    expected["brand"],
+                    expected["model"],
+                    result["family"],
+                    result["brand"],
+                    result["model"],
+                ),
+            )
 
 
 class GetFiltersTest(unittest.TestCase):
     def testGetFiltersNoMatchesGiveEmptyDict(self):
-        user_agent_string = 'foo'
+        user_agent_string = "foo"
         filters = user_agent_parser.GetFilters(
-            user_agent_string, js_user_agent_string=None)
+            user_agent_string, js_user_agent_string=None
+        )
         self.assertEqual({}, filters)
 
     def testGetFiltersJsUaPassedThrough(self):
-        user_agent_string = 'foo'
+        user_agent_string = "foo"
         filters = user_agent_parser.GetFilters(
-            user_agent_string, js_user_agent_string='bar')
-        self.assertEqual({'js_user_agent_string': 'bar'}, filters)
+            user_agent_string, js_user_agent_string="bar"
+        )
+        self.assertEqual({"js_user_agent_string": "bar"}, filters)
 
     def testGetFiltersJsUserAgentFamilyAndVersions(self):
         user_agent_string = (
-            'Mozilla/4.0 (compatible; MSIE 8.0; '
-            'Windows NT 5.1; Trident/4.0; GTB6; .NET CLR 2.0.50727; '
-            '.NET CLR 3.0.4506.2152; .NET CLR 3.5.30729)')
+            "Mozilla/4.0 (compatible; MSIE 8.0; "
+            "Windows NT 5.1; Trident/4.0; GTB6; .NET CLR 2.0.50727; "
+            ".NET CLR 3.0.4506.2152; .NET CLR 3.5.30729)"
+        )
         filters = user_agent_parser.GetFilters(
-            user_agent_string, js_user_agent_string='bar',
-            js_user_agent_family='foo')
-        self.assertEqual({
-            'js_user_agent_string': 'bar',
-            'js_user_agent_family': 'foo'}, filters)
+            user_agent_string, js_user_agent_string="bar", js_user_agent_family="foo"
+        )
+        self.assertEqual(
+            {"js_user_agent_string": "bar", "js_user_agent_family": "foo"}, filters
+        )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `ua-parser-0.8.0/ua_parser/_regexes.py` & `ua-parser-0.9.0/ua_parser/_regexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,27 +36,27 @@
     UserAgentParser(
         '(MusicDownloader)Lite/(\\d+)\\.(\\d+)\\.(\\d+) CFNetwork',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '^(.*)-iPad/(\\d+)\\.?(\\d+)?.?(\\d+)?.?(\\d+)? CFNetwork',
+        '^(.*)-iPad\\/(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)(?:\\.(\\d+)|) CFNetwork',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '^(.*)-iPhone/(\\d+)\\.?(\\d+)?.?(\\d+)?.?(\\d+)? CFNetwork',
+        '^(.*)-iPhone/(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)(?:\\.(\\d+)|) CFNetwork',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '^(.*)/(\\d+)\\.?(\\d+)?.?(\\d+)?.?(\\d+)? CFNetwork',
+        '^(.*)/(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)(?:\\.(\\d+)|) CFNetwork',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(espn\\.go)',
         'ESPN',
@@ -84,44 +84,62 @@
     UserAgentParser(
         ' (Rivo) RHYTHM',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(CFNetwork)(?:/(\\d+)\\.(\\d+)\\.?(\\d+)?)?',
+        '(CFNetwork)(?:/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)|)',
         'CFNetwork',
         None,
         None,
     ),
     UserAgentParser(
-        '(Pingdom.com_bot_version_)(\\d+)\\.(\\d+)',
+        '(Pingdom\\.com_bot_version_)(\\d+)\\.(\\d+)',
         'PingdomBot',
         None,
         None,
     ),
     UserAgentParser(
         '(PingdomTMS)/(\\d+)\\.(\\d+)\\.(\\d+)',
         'PingdomBot',
         None,
         None,
     ),
     UserAgentParser(
+        ' (PTST)/(\\d+)(?:\\.(\\d+)|)$',
+        'WebPageTest.org bot',
+        None,
+        None,
+    ),
+    UserAgentParser(
+        'X11; (Datanyze); Linux',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
         '(NewRelicPinger)/(\\d+)\\.(\\d+)',
         'NewRelicPingerBot',
         None,
         None,
     ),
     UserAgentParser(
         '(Tableau)/(\\d+)\\.(\\d+)',
         'Tableau',
         None,
         None,
     ),
     UserAgentParser(
+        '(Salesforce)(?:.)\\/(\\d+)\\.(\\d?)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
         '(\\(StatusCake\\))',
         'StatusCakeBot',
         None,
         None,
     ),
     UserAgentParser(
         '(facebookexternalhit)/(\\d+)\\.(\\d+)',
@@ -132,117 +150,183 @@
     UserAgentParser(
         'Google.*/\\+/web/snippet',
         'GooglePlusBot',
         None,
         None,
     ),
     UserAgentParser(
-        'via ggpht.com GoogleImageProxy',
+        'via ggpht\\.com GoogleImageProxy',
         'GmailImageProxy',
         None,
         None,
     ),
     UserAgentParser(
+        'YahooMailProxy; https://help\\.yahoo\\.com/kb/yahoo-mail-proxy-SLN28749\\.html',
+        'YahooMailProxy',
+        None,
+        None,
+    ),
+    UserAgentParser(
         '(Twitterbot)/(\\d+)\\.(\\d+)',
-        'TwitterBot',
+        'Twitterbot',
         None,
         None,
     ),
     UserAgentParser(
-        '/((?:Ant-)?Nutch|[A-z]+[Bb]ot|[A-z]+[Ss]pider|Axtaris|fetchurl|Isara|ShopSalad|Tailsweep)[ \\-](\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?',
+        '/((?:Ant-|)Nutch|[A-z]+[Bb]ot|[A-z]+[Ss]pider|Axtaris|fetchurl|Isara|ShopSalad|Tailsweep)[ \\-](\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '\\b(008|Altresium|Argus|BaiduMobaider|BoardReader|DNSGroup|DataparkSearch|EDI|Goodzer|Grub|INGRID|Infohelfer|LinkedInBot|LOOQ|Nutch|PathDefender|Peew|PostPost|Steeler|Twitterbot|VSE|WebCrunch|WebZIP|Y!J-BR[A-Z]|YahooSeeker|envolk|sproose|wminer)/(\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?',
+        '\\b(008|Altresium|Argus|BaiduMobaider|BoardReader|DNSGroup|DataparkSearch|EDI|Goodzer|Grub|INGRID|Infohelfer|LinkedInBot|LOOQ|Nutch|OgScrper|PathDefender|Peew|PostPost|Steeler|Twitterbot|VSE|WebCrunch|WebZIP|Y!J-BR[A-Z]|YahooSeeker|envolk|sproose|wminer)/(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(MSIE) (\\d+)\\.(\\d+)([a-z]\\d?)?;.* MSIECrawler',
+        '(MSIE) (\\d+)\\.(\\d+)([a-z]\\d|[a-z]|);.* MSIECrawler',
         'MSIECrawler',
         None,
         None,
     ),
     UserAgentParser(
-        '(DAVdroid)/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(DAVdroid)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Google-HTTP-Java-Client|Apache-HttpClient|http%20client|Python-urllib|HttpMonitor|TLSProber|WinHTTP|JNLP|okhttp)(?:[ /](\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?)?',
+        '(Google-HTTP-Java-Client|Apache-HttpClient|Go-http-client|scalaj-http|http%20client|Python-urllib|HttpMonitor|TLSProber|WinHTTP|JNLP|okhttp|aihttp|reqwest|axios|unirest-(?:java|python|ruby|nodejs|php|net))(?:[ /](\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Pinterest(?:bot)?)/(\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?[;\\s\\(]+\\+https://www.pinterest.com/bot.html',
+        '(Pinterest(?:bot|))/(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)[;\\s(]+\\+https://www.pinterest.com/bot.html',
         'Pinterestbot',
         None,
         None,
     ),
     UserAgentParser(
-        '(1470\\.net crawler|50\\.nu|8bo Crawler Bot|Aboundex|Accoona-[A-z]+-Agent|AdsBot-Google(?:-[a-z]+)?|altavista|AppEngine-Google|archive.*?\\.org_bot|archiver|Ask Jeeves|[Bb]ai[Dd]u[Ss]pider(?:-[A-Za-z]+)*|bingbot|BingPreview|blitzbot|BlogBridge|Bloglovin|BoardReader(?: [A-Za-z]+)*|boitho.com-dc|BotSeer|BUbiNG|\\b\\w*favicon\\w*\\b|\\bYeti(?:-[a-z]+)?|Catchpoint(?: bot)?|[Cc]harlotte|Checklinks|clumboot|Comodo HTTP\\(S\\) Crawler|Comodo-Webinspector-Crawler|ConveraCrawler|CRAWL-E|CrawlConvera|Daumoa(?:-feedfetcher)?|Feed Seeker Bot|Feedbin|findlinks|Flamingo_SearchEngine|FollowSite Bot|furlbot|Genieo|gigabot|GomezAgent|gonzo1|(?:[a-zA-Z]+-)?Googlebot(?:-[a-zA-Z]+)?|Google SketchUp|grub-client|gsa-crawler|heritrix|HiddenMarket|holmes|HooWWWer|htdig|ia_archiver|ICC-Crawler|Icarus6j|ichiro(?:/mobile)?|IconSurf|IlTrovatore(?:-Setaccio)?|InfuzApp|Innovazion Crawler|InternetArchive|IP2[a-z]+Bot|jbot\\b|KaloogaBot|Kraken|Kurzor|larbin|LEIA|LesnikBot|Linguee Bot|LinkAider|LinkedInBot|Lite Bot|Llaut|lycos|Mail\\.RU_Bot|masscan|masidani_bot|Mediapartners-Google|Microsoft .*? Bot|mogimogi|mozDex|MJ12bot|msnbot(?:-media *)?|msrbot|Mtps Feed Aggregation System|netresearch|Netvibes|NewsGator[^/]*|^NING|Nutch[^/]*|Nymesis|ObjectsSearch|Orbiter|OOZBOT|PagePeeker|PagesInventory|PaxleFramework|Peeplo Screenshot Bot|PlantyNet_WebRobot|Pompos|Qwantify|Read%20Later|Reaper|RedCarpet|Retreiver|Riddler|Rival IQ|scooter|Scrapy|Scrubby|searchsight|seekbot|semanticdiscovery|SemrushBot|Simpy|SimplePie|SEOstats|SimpleRSS|SiteCon|Slackbot-LinkExpanding|Slack-ImgProxy|Slurp|snappy|Speedy Spider|Squrl Java|Stringer|TheUsefulbot|ThumbShotsBot|Thumbshots\\.ru|Tiny Tiny RSS|TwitterBot|WhatsApp|URL2PNG|Vagabondo|VoilaBot|^vortex|Votay bot|^voyager|WASALive.Bot|Web-sniffer|WebThumb|WeSEE:[A-z]+|WhatWeb|WIRE|WordPress|Wotbox|www\\.almaden\\.ibm\\.com|Xenu(?:.s)? Link Sleuth|Xerka [A-z]+Bot|yacy(?:bot)?|Yahoo[a-z]*Seeker|Yahoo! Slurp|Yandex\\w+|YodaoBot(?:-[A-z]+)?|YottaaMonitor|Yowedo|^Zao|^Zao-Crawler|ZeBot_www\\.ze\\.bz|ZooShot|ZyBorg)(?:[ /]v?(\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?)?',
+        '(CSimpleSpider|Cityreview Robot|CrawlDaddy|CrawlFire|Finderbots|Index crawler|Job Roboter|KiwiStatus Spider|Lijit Crawler|QuerySeekerSpider|ScollSpider|Trends Crawler|USyd-NLP-Spider|SiteCat Webbot|BotName\\/\\$BotVersion|123metaspider-Bot|1470\\.net crawler|50\\.nu|8bo Crawler Bot|Aboundex|Accoona-[A-z]{1,30}-Agent|AdsBot-Google(?:-[a-z]{1,30}|)|altavista|AppEngine-Google|archive.{0,30}\\.org_bot|archiver|Ask Jeeves|[Bb]ai[Dd]u[Ss]pider(?:-[A-Za-z]{1,30})(?:-[A-Za-z]{1,30}|)|bingbot|BingPreview|blitzbot|BlogBridge|Bloglovin|BoardReader Blog Indexer|BoardReader Favicon Fetcher|boitho.com-dc|BotSeer|BUbiNG|\\b\\w{0,30}favicon\\w{0,30}\\b|\\bYeti(?:-[a-z]{1,30}|)|Catchpoint(?: bot|)|[Cc]harlotte|Checklinks|clumboot|Comodo HTTP\\(S\\) Crawler|Comodo-Webinspector-Crawler|ConveraCrawler|CRAWL-E|CrawlConvera|Daumoa(?:-feedfetcher|)|Feed Seeker Bot|Feedbin|findlinks|Flamingo_SearchEngine|FollowSite Bot|furlbot|Genieo|gigabot|GomezAgent|gonzo1|(?:[a-zA-Z]{1,30}-|)Googlebot(?:-[a-zA-Z]{1,30}|)|Google SketchUp|grub-client|gsa-crawler|heritrix|HiddenMarket|holmes|HooWWWer|htdig|ia_archiver|ICC-Crawler|Icarus6j|ichiro(?:/mobile|)|IconSurf|IlTrovatore(?:-Setaccio|)|InfuzApp|Innovazion Crawler|InternetArchive|IP2[a-z]{1,30}Bot|jbot\\b|KaloogaBot|Kraken|Kurzor|larbin|LEIA|LesnikBot|Linguee Bot|LinkAider|LinkedInBot|Lite Bot|Llaut|lycos|Mail\\.RU_Bot|masscan|masidani_bot|Mediapartners-Google|Microsoft .{0,30} Bot|mogimogi|mozDex|MJ12bot|msnbot(?:-media {0,2}|)|msrbot|Mtps Feed Aggregation System|netresearch|Netvibes|NewsGator[^/]{0,30}|^NING|Nutch[^/]{0,30}|Nymesis|ObjectsSearch|OgScrper|Orbiter|OOZBOT|PagePeeker|PagesInventory|PaxleFramework|Peeplo Screenshot Bot|PlantyNet_WebRobot|Pompos|Qwantify|Read%20Later|Reaper|RedCarpet|Retreiver|Riddler|Rival IQ|scooter|Scrapy|Scrubby|searchsight|seekbot|semanticdiscovery|SemrushBot|Simpy|SimplePie|SEOstats|SimpleRSS|SiteCon|Slackbot-LinkExpanding|Slack-ImgProxy|Slurp|snappy|Speedy Spider|Squrl Java|Stringer|TheUsefulbot|ThumbShotsBot|Thumbshots\\.ru|Tiny Tiny RSS|Twitterbot|WhatsApp|URL2PNG|Vagabondo|VoilaBot|^vortex|Votay bot|^voyager|WASALive.Bot|Web-sniffer|WebThumb|WeSEE:[A-z]{1,30}|WhatWeb|WIRE|WordPress|Wotbox|www\\.almaden\\.ibm\\.com|Xenu(?:.s|) Link Sleuth|Xerka [A-z]{1,30}Bot|yacy(?:bot|)|YahooSeeker|Yahoo! Slurp|Yandex\\w{1,30}|YodaoBot(?:-[A-z]{1,30}|)|YottaaMonitor|Yowedo|^Zao|^Zao-Crawler|ZeBot_www\\.ze\\.bz|ZooShot|ZyBorg)(?:[ /]v?(\\d+)(?:\\.(\\d+)(?:\\.(\\d+)|)|)|)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '\\b(Boto3?|JetS3t|aws-(?:cli|sdk-(?:cpp|go|java|nodejs|ruby2?|dotnet-(?:\\d{1,2}|core)))|s3fs)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '\\[(FBAN/MessengerForiOS|FB_IAB/MESSENGER);FBAV/(\\d+)(?:\\.(\\d+)(?:\\.(\\d+)|)|)',
+        'Facebook Messenger',
         None,
         None,
+    ),
+    UserAgentParser(
+        '\\[FB.*;(FBAV)/(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
+        'Facebook',
+        None,
         None,
     ),
     UserAgentParser(
-        '(?:\\/[A-Za-z0-9\\.]+)? *([A-Za-z0-9 \\-_\\!\\[\\]:]*(?:[Aa]rchiver|[Ii]ndexer|[Ss]craper|[Bb]ot|[Ss]pider|[Cc]rawl[a-z]*))/(\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?',
+        '\\[FB.*;',
+        'Facebook',
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(?:\\/[A-Za-z0-9\\.]+|) {0,5}([A-Za-z0-9 \\-_\\!\\[\\]:]{0,50}(?:[Aa]rchiver|[Ii]ndexer|[Ss]craper|[Bb]ot|[Ss]pider|[Cc]rawl[a-z]{0,50}))[/ ](\\d+)(?:\\.(\\d+)(?:\\.(\\d+)|)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(?:\\/[A-Za-z0-9\\.]+)? *([A-Za-z0-9 _\\!\\[\\]:]*(?:[Aa]rchiver|[Ii]ndexer|[Ss]craper|[Bb]ot|[Ss]pider|[Cc]rawl[a-z]*)) (\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?',
+        '((?:[A-Za-z][A-Za-z0-9 -]{0,50}|)[^C][^Uu][Bb]ot)\\b(?:(?:[ /]| v)(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '((?:[A-z0-9]+|[A-z\\-]+ ?)?(?: the )?(?:[Ss][Pp][Ii][Dd][Ee][Rr]|[Ss]crape|[A-Za-z0-9-]*(?:[^C][^Uu])[Bb]ot|[Cc][Rr][Aa][Ww][Ll])[A-z0-9]*)(?:(?:[ /]| v)(\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?)?',
+        '((?:[A-z0-9]{1,50}|[A-z\\-]{1,50} ?|)(?: the |)(?:[Ss][Pp][Ii][Dd][Ee][Rr]|[Ss]crape|[Cc][Rr][Aa][Ww][Ll])[A-z0-9]{0,50})(?:(?:[ /]| v)(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(HbbTV)/(\\d+)\\.(\\d+)\\.(\\d+) \\(',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Chimera|SeaMonkey|Camino)/(\\d+)\\.(\\d+)\\.?([ab]?\\d+[a-z]*)?',
+        '(Chimera|SeaMonkey|Camino|Waterfox)/(\\d+)\\.(\\d+)\\.?([ab]?\\d+[a-z]*|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '\\[FB.*;(FBAV)/(\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?',
-        'Facebook',
+        '(SailfishBrowser)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
+        'Sailfish Browser',
         None,
         None,
     ),
     UserAgentParser(
         '\\[(Pinterest)/[^\\]]+\\]',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Pinterest)(?: for Android(?: Tablet)?)?/(\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?',
+        '(Pinterest)(?: for Android(?: Tablet|)|)/(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        'Mozilla.*Mobile.*(Instagram).(\\d+)\\.(\\d+)\\.(\\d+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(PaleMoon)/(\\d+)\\.(\\d+)\\.?(\\d+)?',
+        'Mozilla.*Mobile.*(Flipboard).(\\d+)\\.(\\d+)\\.(\\d+)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        'Mozilla.*Mobile.*(Flipboard-Briefing).(\\d+)\\.(\\d+)\\.(\\d+)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        'Mozilla.*Mobile.*(Onefootball)\\/Android.(\\d+)\\.(\\d+)\\.(\\d+)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(Snapchat)\\/(\\d+)\\.(\\d+)\\.(\\d+)\\.(\\d+)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(Firefox)/(\\d+)\\.(\\d+) Basilisk/(\\d+)',
+        'Basilisk',
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(PaleMoon)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'Pale Moon',
         None,
         None,
     ),
     UserAgentParser(
         '(Fennec)/(\\d+)\\.(\\d+)\\.?([ab]?\\d+[a-z]*)',
         'Firefox Mobile',
@@ -264,15 +348,15 @@
     UserAgentParser(
         '(?:Mobile|Tablet);.*(Firefox)/(\\d+)\\.(\\d+)',
         'Firefox Mobile',
         None,
         None,
     ),
     UserAgentParser(
-        '(Namoroka|Shiretoko|Minefield)/(\\d+)\\.(\\d+)\\.(\\d+(?:pre)?)',
+        '(Namoroka|Shiretoko|Minefield)/(\\d+)\\.(\\d+)\\.(\\d+(?:pre|))',
         'Firefox ($1)',
         None,
         None,
     ),
     UserAgentParser(
         '(Firefox)/(\\d+)\\.(\\d+)(a\\d+[a-z]*)',
         'Firefox Alpha',
@@ -282,45 +366,45 @@
     UserAgentParser(
         '(Firefox)/(\\d+)\\.(\\d+)(b\\d+[a-z]*)',
         'Firefox Beta',
         None,
         None,
     ),
     UserAgentParser(
-        '(Firefox)-(?:\\d+\\.\\d+)?/(\\d+)\\.(\\d+)(a\\d+[a-z]*)',
+        '(Firefox)-(?:\\d+\\.\\d+|)/(\\d+)\\.(\\d+)(a\\d+[a-z]*)',
         'Firefox Alpha',
         None,
         None,
     ),
     UserAgentParser(
-        '(Firefox)-(?:\\d+\\.\\d+)?/(\\d+)\\.(\\d+)(b\\d+[a-z]*)',
+        '(Firefox)-(?:\\d+\\.\\d+|)/(\\d+)\\.(\\d+)(b\\d+[a-z]*)',
         'Firefox Beta',
         None,
         None,
     ),
     UserAgentParser(
-        '(Namoroka|Shiretoko|Minefield)/(\\d+)\\.(\\d+)([ab]\\d+[a-z]*)?',
+        '(Namoroka|Shiretoko|Minefield)/(\\d+)\\.(\\d+)([ab]\\d+[a-z]*|)',
         'Firefox ($1)',
         None,
         None,
     ),
     UserAgentParser(
         '(Firefox).*Tablet browser (\\d+)\\.(\\d+)\\.(\\d+)',
         'MicroB',
         None,
         None,
     ),
     UserAgentParser(
-        '(MozillaDeveloperPreview)/(\\d+)\\.(\\d+)([ab]\\d+[a-z]*)?',
+        '(MozillaDeveloperPreview)/(\\d+)\\.(\\d+)([ab]\\d+[a-z]*|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(FxiOS)/(\\d+)\\.(\\d+)(\\.(\\d+))?(\\.(\\d+))?',
+        '(FxiOS)/(\\d+)\\.(\\d+)(\\.(\\d+)|)(\\.(\\d+)|)',
         'Firefox iOS',
         None,
         None,
     ),
     UserAgentParser(
         '(Flock)/(\\d+)\\.(\\d+)(b\\d+?)',
         None,
@@ -342,15 +426,15 @@
     UserAgentParser(
         '(Navigator)/(\\d+)\\.(\\d+)([ab]\\d+)',
         'Netscape',
         None,
         None,
     ),
     UserAgentParser(
-        '(Netscape6)/(\\d+)\\.(\\d+)\\.?([ab]?\\d+)?',
+        '(Netscape6)/(\\d+)\\.(\\d+)\\.?([ab]?\\d+|)',
         'Netscape',
         None,
         None,
     ),
     UserAgentParser(
         '(MyIBrow)/(\\d+)\\.(\\d+)',
         'My Internet Browser',
@@ -360,21 +444,21 @@
     UserAgentParser(
         '(UC? ?Browser|UCWEB|U3)[ /]?(\\d+)\\.(\\d+)\\.(\\d+)',
         'UC Browser',
         None,
         None,
     ),
     UserAgentParser(
-        '(Opera Tablet).*Version/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(Opera Tablet).*Version/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Opera Mini)(?:/att)?/?(\\d+)?(?:\\.(\\d+))?(?:\\.(\\d+))?',
+        '(Opera Mini)(?:/att|)/?(\\d+|)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(Opera)/.+Opera Mobi.+Version/(\\d+)\\.(\\d+)',
         'Opera Mobile',
@@ -396,15 +480,15 @@
     UserAgentParser(
         'Opera Mobi',
         'Opera Mobile',
         None,
         None,
     ),
     UserAgentParser(
-        '(Opera)/9.80.*Version/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(Opera)/9.80.*Version/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(?:Mobile Safari).*(OPR)/(\\d+)\\.(\\d+)\\.(\\d+)',
         'Opera Mobile',
@@ -432,15 +516,15 @@
     UserAgentParser(
         'Chrome/.+( MMS)/(\\d+).(\\d+).(\\d+)',
         'Opera Neon',
         None,
         None,
     ),
     UserAgentParser(
-        '(hpw|web)OS/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(hpw|web)OS/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'webOS Browser',
         None,
         None,
     ),
     UserAgentParser(
         '(luakit)',
         'LuaKit',
@@ -456,39 +540,39 @@
     UserAgentParser(
         'Gecko/\\d+ (Lightning)/(\\d+)\\.(\\d+)\\.?((?:[ab]?\\d+[a-z]*)|(?:\\d*))',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Firefox)/(\\d+)\\.(\\d+)\\.(\\d+(?:pre)?) \\(Swiftfox\\)',
+        '(Firefox)/(\\d+)\\.(\\d+)\\.(\\d+(?:pre|)) \\(Swiftfox\\)',
         'Swiftfox',
         None,
         None,
     ),
     UserAgentParser(
-        '(Firefox)/(\\d+)\\.(\\d+)([ab]\\d+[a-z]*)? \\(Swiftfox\\)',
+        '(Firefox)/(\\d+)\\.(\\d+)([ab]\\d+[a-z]*|) \\(Swiftfox\\)',
         'Swiftfox',
         None,
         None,
     ),
     UserAgentParser(
-        '(rekonq)/(\\d+)\\.(\\d+)\\.?(\\d+)? Safari',
+        '(rekonq)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|) Safari',
         'Rekonq',
         None,
         None,
     ),
     UserAgentParser(
         'rekonq',
         'Rekonq',
         None,
         None,
     ),
     UserAgentParser(
-        '(conkeror|Conkeror)/(\\d+)\\.(\\d+)\\.?(\\d+)?',
+        '(conkeror|Conkeror)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'Conkeror',
         None,
         None,
     ),
     UserAgentParser(
         '(konqueror)/(\\d+)\\.(\\d+)\\.(\\d+)',
         'Konqueror',
@@ -546,21 +630,21 @@
     UserAgentParser(
         '(Nintendo 3DS)',
         'NetFront NX',
         None,
         None,
     ),
     UserAgentParser(
-        '(Silk)/(\\d+)\\.(\\d+)(?:\\.([0-9\\-]+))?',
+        '(Silk)/(\\d+)\\.(\\d+)(?:\\.([0-9\\-]+)|)',
         'Amazon Silk',
         None,
         None,
     ),
     UserAgentParser(
-        '(Puffin)/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(Puffin)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         'Windows Phone .*(Edge)/(\\d+)\\.(\\d+)',
         'Edge Mobile',
@@ -570,50 +654,80 @@
     UserAgentParser(
         '(SamsungBrowser)/(\\d+)\\.(\\d+)',
         'Samsung Internet',
         None,
         None,
     ),
     UserAgentParser(
-        '(SznProhlizec)/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(SznProhlizec)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         u'Seznam prohl\xed\u017ee\u010d',
         None,
         None,
     ),
     UserAgentParser(
-        '(coc_coc_browser)/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(coc_coc_browser)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'Coc Coc',
         None,
         None,
     ),
     UserAgentParser(
-        '(baidubrowser)[/\\s](\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?',
+        '(baidubrowser)[/\\s](\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
         'Baidu Browser',
         None,
         None,
     ),
     UserAgentParser(
         '(FlyFlow)/(\\d+)\\.(\\d+)',
         'Baidu Explorer',
         None,
         None,
     ),
     UserAgentParser(
-        '(MxBrowser)/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(MxBrowser)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'Maxthon',
         None,
         None,
     ),
     UserAgentParser(
         '(Crosswalk)/(\\d+)\\.(\\d+)\\.(\\d+)\\.(\\d+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
+        '(Line)/(\\d+)\\.(\\d+)\\.(\\d+)',
+        'LINE',
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(MiuiBrowser)/(\\d+)\\.(\\d+)\\.(\\d+)',
+        'MiuiBrowser',
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(Mint Browser)/(\\d+)\\.(\\d+)\\.(\\d+)',
+        'Mint Browser',
+        None,
+        None,
+    ),
+    UserAgentParser(
+        'Mozilla.+Android.+(GSA)/(\\d+)\\.(\\d+)\\.(\\d+)',
+        'Google',
+        None,
+        None,
+    ),
+    UserAgentParser(
+        'Version/.+(Chrome)/(\\d+)\\.(\\d+)\\.(\\d+)\\.(\\d+)',
+        'Chrome Mobile WebView',
+        None,
+        None,
+    ),
+    UserAgentParser(
         '; wv\\).+(Chrome)/(\\d+)\\.(\\d+)\\.(\\d+)\\.(\\d+)',
         'Chrome Mobile WebView',
         None,
         None,
     ),
     UserAgentParser(
         '(CrMo)/(\\d+)\\.(\\d+)\\.(\\d+)\\.(\\d+)',
@@ -654,27 +768,27 @@
     UserAgentParser(
         '(SE 2\\.X) MetaSr (\\d+)\\.(\\d+)',
         'Sogou Explorer',
         None,
         None,
     ),
     UserAgentParser(
-        '(MQQBrowser/Mini)(?:(\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?)?',
+        '(MQQBrowser/Mini)(?:(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)|)',
         'QQ Browser Mini',
         None,
         None,
     ),
     UserAgentParser(
-        '(MQQBrowser)(?:/(\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?)?',
+        '(MQQBrowser)(?:/(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)|)',
         'QQ Browser Mobile',
         None,
         None,
     ),
     UserAgentParser(
-        '(QQBrowser)(?:/(\\d+)(?:\\.(\\d+)\\.(\\d+)(?:\\.(\\d+))?)?)?',
+        '(QQBrowser)(?:/(\\d+)(?:\\.(\\d+)\\.(\\d+)(?:\\.(\\d+)|)|)|)',
         'QQ Browser',
         None,
         None,
     ),
     UserAgentParser(
         '(Rackspace Monitoring)/(\\d+)\\.(\\d+)',
         'RackspaceBot',
@@ -702,33 +816,51 @@
     UserAgentParser(
         '(AOL) (\\d+)\\.(\\d+); AOLBuild (\\d+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(PodCruncher|Downcast)[ /]?(\\d+)\\.?(\\d+)?\\.?(\\d+)?\\.?(\\d+)?',
+        '(PodCruncher|Downcast)[ /]?(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         ' (BoxNotes)/(\\d+)\\.(\\d+)\\.(\\d+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
+        '(Whale)/(\\d+)\\.(\\d+)\\.(\\d+)\\.(\\d+) Mobile(?:[ /]|$)',
+        'Whale',
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(Whale)/(\\d+)\\.(\\d+)\\.(\\d+)',
+        'Whale',
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(Ghost)/(\\d+)\\.(\\d+)\\.(\\d+)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
         '(Slack_SSB)/(\\d+)\\.(\\d+)\\.(\\d+)',
         'Slack Desktop Client',
         None,
         None,
     ),
     UserAgentParser(
-        '(HipChat)/?(\\d+)?',
+        '(HipChat)/?(\\d+|)',
         'HipChat Desktop Client',
         None,
         None,
     ),
     UserAgentParser(
         '\\b(MobileIron|FireWeb|Jasmine|ANTGalio|Midori|Fresco|Lobo|PaleMoon|Maxthon|Lynx|OmniWeb|Dillo|Camino|Demeter|Fluid|Fennec|Epiphany|Shiira|Sunrise|Spotify|Flock|Netscape|Lunascape|WebPilot|NetFront|Netfront|Konqueror|SeaMonkey|Kazehakase|Vienna|Iceape|Iceweasel|IceWeasel|Iron|K-Meleon|Sleipnir|Galeon|GranParadiso|Opera Mini|iCab|NetNewsWire|ThunderBrowse|Iris|UP\\.Browser|Bunjalloo|Google Earth|Raven for Mac|Openwave|MacOutlook|Electron|OktaMobile)/(\\d+)\\.(\\d+)\\.(\\d+)',
         None,
@@ -750,64 +882,70 @@
     UserAgentParser(
         'Microsoft Outlook 15\\.\\d+\\.\\d+',
         'Outlook',
         '2013',
         None,
     ),
     UserAgentParser(
-        'Microsoft Outlook (?:Mail )?16\\.\\d+\\.\\d+',
+        'Microsoft Outlook (?:Mail )?16\\.\\d+\\.\\d+|MSOffice 16',
         'Outlook',
         '2016',
         None,
     ),
     UserAgentParser(
+        'Microsoft Office (Word) 2014',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
         'Outlook-Express\\/7\\.0.*',
         'Windows Live Mail',
         None,
         None,
     ),
     UserAgentParser(
-        '(Airmail) (\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(Airmail) (\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Thunderbird)/(\\d+)\\.(\\d+)(?:\\.(\\d+(?:pre)?))?',
+        '(Thunderbird)/(\\d+)\\.(\\d+)(?:\\.(\\d+(?:pre|))|)',
         'Thunderbird',
         None,
         None,
     ),
     UserAgentParser(
         '(Postbox)/(\\d+)\\.(\\d+)\\.(\\d+)',
         'Postbox',
         None,
         None,
     ),
     UserAgentParser(
-        '(Barca(?:Pro)?)/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(Barca(?:Pro)?)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'Barca',
         None,
         None,
     ),
     UserAgentParser(
-        '(Lotus-Notes)/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(Lotus-Notes)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'Lotus Notes',
         None,
         None,
     ),
     UserAgentParser(
         '(Vivaldi)/(\\d+)\\.(\\d+)\\.(\\d+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Edge)/(\\d+)(?:\\.(\\d+))?',
-        None,
+        '(Edge?)/(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
+        'Edge',
         None,
         None,
     ),
     UserAgentParser(
         '(brave)/(\\d+)\\.(\\d+)\\.(\\d+) Chrome',
         'Brave',
         None,
@@ -816,45 +954,45 @@
     UserAgentParser(
         '(Chrome)/(\\d+)\\.(\\d+)\\.(\\d+)[\\d.]* Iron[^/]',
         'Iron',
         None,
         None,
     ),
     UserAgentParser(
-        '\\b(Dolphin)(?: |HDCN/|/INT\\-)(\\d+)\\.(\\d+)\\.?(\\d+)?',
+        '\\b(Dolphin)(?: |HDCN/|/INT\\-)(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(HeadlessChrome)(?:/(\\d+)\\.(\\d+)\\.(\\d+))?',
+        '(HeadlessChrome)(?:/(\\d+)\\.(\\d+)\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(Evolution)/(\\d+)\\.(\\d+)\\.(\\d+\\.\\d+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(RCM CardDAV plugin)/(\\d+)\\.(\\d+)\\.(\\d+(?:-dev)?)',
+        '(RCM CardDAV plugin)/(\\d+)\\.(\\d+)\\.(\\d+(?:-dev|))',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(bingbot|Bolt|AdobeAIR|Jasmine|IceCat|Skyfire|Midori|Maxthon|Lynx|Arora|IBrowse|Dillo|Camino|Shiira|Fennec|Phoenix|Flock|Netscape|Lunascape|Epiphany|WebPilot|Opera Mini|Opera|NetFront|Netfront|Konqueror|Googlebot|SeaMonkey|Kazehakase|Vienna|Iceape|Iceweasel|IceWeasel|Iron|K-Meleon|Sleipnir|Galeon|GranParadiso|iCab|iTunes|MacAppStore|NetNewsWire|Space Bison|Stainless|Orca|Dolfin|BOLT|Minimo|Tizen Browser|Polaris|Abrowser|Planetweb|ICE Browser|mDolphin|qutebrowser|Otter|QupZilla|MailBar|kmail2|YahooMobileMail|ExchangeWebServices|ExchangeServicesClient|Dragon|Outlook-iOS-Android)/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(bingbot|Bolt|AdobeAIR|Jasmine|IceCat|Skyfire|Midori|Maxthon|Lynx|Arora|IBrowse|Dillo|Camino|Shiira|Fennec|Phoenix|Flock|Netscape|Lunascape|Epiphany|WebPilot|Opera Mini|Opera|NetFront|Netfront|Konqueror|Googlebot|SeaMonkey|Kazehakase|Vienna|Iceape|Iceweasel|IceWeasel|Iron|K-Meleon|Sleipnir|Galeon|GranParadiso|iCab|iTunes|MacAppStore|NetNewsWire|Space Bison|Stainless|Orca|Dolfin|BOLT|Minimo|Tizen Browser|Polaris|Abrowser|Planetweb|ICE Browser|mDolphin|qutebrowser|Otter|QupZilla|MailBar|kmail2|YahooMobileMail|ExchangeWebServices|ExchangeServicesClient|Dragon|Outlook-iOS-Android)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Chromium|Chrome)/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(Chromium|Chrome)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(IEMobile)[ /](\\d+)\\.(\\d+)',
         'IE Mobile',
@@ -876,21 +1014,21 @@
     UserAgentParser(
         '^(AlexaMediaPlayer|VLC)/(\\d+)\\.(\\d+)\\.([^.\\s]+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '^(AntennaPod|WMPlayer|Zune|Podkicker|Radio|ExoPlayerDemo|Overcast|PocketTunes|NSPlayer|okhttp|DoggCatcher|QuickNews|QuickTime|Peapod|Podcasts|GoldenPod|VLC|Spotify|Miro|MediaGo|Juice|iPodder|gPodder|Banshee)/(\\d+)\\.(\\d+)\\.?(\\d+)?\\.?(\\d+)?',
+        '^(AntennaPod|WMPlayer|Zune|Podkicker|Radio|ExoPlayerDemo|Overcast|PocketTunes|NSPlayer|okhttp|DoggCatcher|QuickNews|QuickTime|Peapod|Podcasts|GoldenPod|VLC|Spotify|Miro|MediaGo|Juice|iPodder|gPodder|Banshee)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '^(Peapod|Liferea)/([^.\\s]+)\\.([^.\\s]+)?\\.?([^.\\s]+)?',
+        '^(Peapod|Liferea)/([^.\\s]+)\\.([^.\\s]+|)\\.?([^.\\s]+|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '^(bPod|Player FM) BMID/(\\S+)',
         None,
@@ -936,21 +1074,21 @@
     UserAgentParser(
         '(Player FM)$',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(LG Player|Doppler|FancyMusic|MediaMonkey|Clementine) (\\d+)\\.(\\d+)\\.?([^.\\s]+)?\\.?([^.\\s]+)?',
+        '(LG Player|Doppler|FancyMusic|MediaMonkey|Clementine) (\\d+)\\.(\\d+)\\.?([^.\\s]+|)\\.?([^.\\s]+|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(philpodder)/(\\d+)\\.(\\d+)\\.?([^.\\s]+)?\\.?([^.\\s]+)?',
+        '(philpodder)/(\\d+)\\.(\\d+)\\.?([^.\\s]+|)\\.?([^.\\s]+|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(Player FM|Pocket Casts|DoggCatcher|Spotify|MediaMonkey|MediaGo|BashPodder)',
         None,
@@ -978,33 +1116,33 @@
     UserAgentParser(
         'EspnDownloadManager',
         'ESPN',
         None,
         None,
     ),
     UserAgentParser(
-        '(ESPN) Radio (\\d+)\\.(\\d+)\\.?(\\d+)? ?(?:rv:(\\d+))? ',
+        '(ESPN) Radio (\\d+)\\.(\\d+)(?:\\.(\\d+)|) ?(?:rv:(\\d+)|) ',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(podracer|jPodder) v ?(\\d+)\\.(\\d+)\\.?(\\d+)?',
+        '(podracer|jPodder) v ?(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(ZDM)/(\\d+)\\.(\\d+)[; ]?',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Zune|BeyondPod) (\\d+)\\.?(\\d+)?[\\);]',
+        '(Zune|BeyondPod) (\\d+)(?:\\.(\\d+)|)[\\);]',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(WMPlayer)/(\\d+)\\.(\\d+)\\.(\\d+)\\.(\\d+)',
         None,
@@ -1014,15 +1152,15 @@
     UserAgentParser(
         '^(Lavf)',
         'WMPlayer',
         None,
         None,
     ),
     UserAgentParser(
-        '^(RSSRadio)[ /]?(\\d+)?',
+        '^(RSSRadio)[ /]?(\\d+|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(RSS_Radio) (\\d+)\\.(\\d+)',
         'RSSRadio',
@@ -1032,15 +1170,15 @@
     UserAgentParser(
         '(Podkicker) \\S+/(\\d+)\\.(\\d+)\\.(\\d+)',
         'Podkicker',
         None,
         None,
     ),
     UserAgentParser(
-        '^(HTC) Streaming Player \\S+ / \\S+ / \\S+ / (\\d+)\\.(\\d+)\\.?(\\d+)?',
+        '^(HTC) Streaming Player \\S+ / \\S+ / \\S+ / (\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '^(Stitcher)/iOS',
         None,
@@ -1068,27 +1206,27 @@
     UserAgentParser(
         '(vlc)/(\\d+)\\.(\\d+)\\.(\\d+)',
         'VLC',
         None,
         None,
     ),
     UserAgentParser(
-        '^(foobar)\\S+/([^.\\s]+)\\.([^.\\s]+)?\\.?([^.\\s]+)?',
+        '^(foobar)\\S+/([^.\\s]+)\\.([^.\\s]+|)\\.?([^.\\s]+|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '^(Clementine)\\S+ ([^.\\s]+)\\.([^.\\s]+)?\\.?([^.\\s]+)?',
+        '^(Clementine)\\S+ ([^.\\s]+)\\.([^.\\s]+|)\\.?([^.\\s]+|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(amarok)/([^.\\s]+)\\.([^.\\s]+)?\\.?([^.\\s]+)?',
+        '(amarok)/([^.\\s]+)\\.([^.\\s]+|)\\.?([^.\\s]+|)',
         'Amarok',
         None,
         None,
     ),
     UserAgentParser(
         '(Custom)-Feed Reader',
         None,
@@ -1098,15 +1236,15 @@
     UserAgentParser(
         '(iRider|Crazy Browser|SkipStone|iCab|Lunascape|Sleipnir|Maemo Browser) (\\d+)\\.(\\d+)\\.(\\d+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(iCab|Lunascape|Opera|Android|Jasmine|Polaris|Microsoft SkyDriveSync|The Bat!) (\\d+)\\.(\\d+)\\.?(\\d+)?',
+        '(iCab|Lunascape|Opera|Android|Jasmine|Polaris|Microsoft SkyDriveSync|The Bat!) (\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(Kindle)/(\\d+)\\.(\\d+)',
         None,
@@ -1164,27 +1302,33 @@
     UserAgentParser(
         '(ownCloud-android)/(\\d+)\\.(\\d+)\\.(\\d+)',
         'Owncloud',
         None,
         None,
     ),
     UserAgentParser(
+        '(OC)/(\\d+)\\.(\\d+)\\.(\\d+)\\.(\\d+) \\(Skype for Business\\)',
+        'Skype',
+        None,
+        None,
+    ),
+    UserAgentParser(
         '(Obigo)InternetBrowser',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(Obigo)\\-Browser',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Obigo|OBIGO)[^\\d]*(\\d+)(?:.(\\d+))?',
+        '(Obigo|OBIGO)[^\\d]*(\\d+)(?:.(\\d+)|)',
         'Obigo',
         None,
         None,
     ),
     UserAgentParser(
         '(MAXTHON|Maxthon) (\\d+)\\.(\\d+)',
         'Maxthon',
@@ -1218,45 +1362,51 @@
     UserAgentParser(
         '(Embider)/(\\d+)\\.(\\d+)',
         'Polaris',
         None,
         None,
     ),
     UserAgentParser(
-        '(BonEcho)/(\\d+)\\.(\\d+)\\.?([ab]?\\d+)?',
+        '(BonEcho)/(\\d+)\\.(\\d+)\\.?([ab]?\\d+|)',
         'Bon Echo',
         None,
         None,
     ),
     UserAgentParser(
-        '(iPod|iPhone|iPad).+Version/(\\d+)\\.(\\d+)(?:\\.(\\d+))?.*[ +]Safari',
+        '(iPod|iPhone|iPad).+GSA/(\\d+)\\.(\\d+)\\.(\\d+) Mobile',
+        'Google',
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(iPod|iPhone|iPad).+Version/(\\d+)\\.(\\d+)(?:\\.(\\d+)|).*[ +]Safari',
         'Mobile Safari',
         None,
         None,
     ),
     UserAgentParser(
-        '(iPod|iPod touch|iPhone|iPad);.*CPU.*OS[ +](\\d+)_(\\d+)(?:_(\\d+))?.* AppleNews\\/\\d+\\.\\d+\\.\\d+?',
+        '(iPod|iPod touch|iPhone|iPad);.*CPU.*OS[ +](\\d+)_(\\d+)(?:_(\\d+)|).* AppleNews\\/\\d+\\.\\d+\\.\\d+?',
         'Mobile Safari UI/WKWebView',
         None,
         None,
     ),
     UserAgentParser(
-        '(iPod|iPhone|iPad).+Version/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(iPod|iPhone|iPad).+Version/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'Mobile Safari UI/WKWebView',
         None,
         None,
     ),
     UserAgentParser(
-        '(iPod|iPod touch|iPhone|iPad);.*CPU.*OS[ +](\\d+)_(\\d+)(?:_(\\d+))?.*Mobile.*[ +]Safari',
+        '(iPod|iPod touch|iPhone|iPad);.*CPU.*OS[ +](\\d+)_(\\d+)(?:_(\\d+)|).*Mobile.*[ +]Safari',
         'Mobile Safari',
         None,
         None,
     ),
     UserAgentParser(
-        '(iPod|iPod touch|iPhone|iPad);.*CPU.*OS[ +](\\d+)_(\\d+)(?:_(\\d+))?.*Mobile',
+        '(iPod|iPod touch|iPhone|iPad);.*CPU.*OS[ +](\\d+)_(\\d+)(?:_(\\d+)|).*Mobile',
         'Mobile Safari UI/WKWebView',
         None,
         None,
     ),
     UserAgentParser(
         '(iPod|iPhone|iPad).* Safari',
         'Mobile Safari',
@@ -1266,14 +1416,20 @@
     UserAgentParser(
         '(iPod|iPhone|iPad)',
         'Mobile Safari UI/WKWebView',
         None,
         None,
     ),
     UserAgentParser(
+        '(Watch)(\\d+),(\\d+)',
+        'Apple $1 App',
+        None,
+        None,
+    ),
+    UserAgentParser(
         '(Outlook-iOS)/\\d+\\.\\d+\\.prod\\.iphone \\((\\d+)\\.(\\d+)\\.(\\d+)\\)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(AvantGo) (\\d+).(\\d+)',
@@ -1428,21 +1584,21 @@
     UserAgentParser(
         '(PhantomJS)/(\\d+)\\.(\\d+)\\.(\\d+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(AppleWebKit)/(\\d+)\\.?(\\d+)?\\+ .* Safari',
+        '(AppleWebKit)/(\\d+)(?:\\.(\\d+)|)\\+ .* Safari',
         'WebKit Nightly',
         None,
         None,
     ),
     UserAgentParser(
-        '(Version)/(\\d+)\\.(\\d+)(?:\\.(\\d+))?.*Safari/',
+        '(Version)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|).*Safari/',
         'Safari',
         None,
         None,
     ),
     UserAgentParser(
         '(Safari)/\\d+',
         None,
@@ -1500,15 +1656,15 @@
     UserAgentParser(
         '(Trident)/(4)\\.(0)',
         'IE',
         '8',
         None,
     ),
     UserAgentParser(
-        '(Espial)/(\\d+)(?:\\.(\\d+))?(?:\\.(\\d+))?',
+        '(Espial)/(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '(AppleWebKit)/(\\d+)\\.(\\d+)\\.(\\d+)',
         'Apple Mail',
@@ -1518,15 +1674,15 @@
     UserAgentParser(
         '(Firefox)/(\\d+)\\.(\\d+)\\.(\\d+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Firefox)/(\\d+)\\.(\\d+)(pre|[ab]\\d+[a-z]*)?',
+        '(Firefox)/(\\d+)\\.(\\d+)(pre|[ab]\\d+[a-z]*|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '([MS]?IE) (\\d+)\\.(\\d+)',
         'IE',
@@ -1536,21 +1692,69 @@
     UserAgentParser(
         '(python-requests)/(\\d+)\\.(\\d+)',
         'Python Requests',
         None,
         None,
     ),
     UserAgentParser(
-        '\\b(Windows-Update-Agent|Microsoft-CryptoAPI|SophosUpdateManager|SophosAgent|Debian APT-HTTP|Ubuntu APT-HTTP|libcurl-agent|libwww-perl|urlgrabber|curl|Wget|OpenBSD ftp|jupdate)(?:[ /](\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?)?',
+        '\\b(Windows-Update-Agent|Microsoft-CryptoAPI|SophosUpdateManager|SophosAgent|Debian APT-HTTP|Ubuntu APT-HTTP|libcurl-agent|libwww-perl|urlgrabber|curl|PycURL|Wget|aria2|Axel|OpenBSD ftp|lftp|jupdate|insomnia|fetch libfetch|akka-http|got)(?:[ /](\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)|)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(Python/3\\.\\d{1,3} aiohttp)/(\\d+)\\.(\\d+)\\.(\\d+)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(Python/3\\.\\d{1,3} aiohttp)/(\\d+)\\.(\\d+)\\.(\\d+)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '(Java)[/ ]{0,1}\\d+\\.(\\d+)\\.(\\d+)[_-]*([a-zA-Z0-9]+|)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '^(Cyberduck)/(\\d+)\\.(\\d+)\\.(\\d+)(?:\\.\\d+|)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '^(S3 Browser) (\\d+)-(\\d+)-(\\d+)(?:\\s*http://s3browser\\.com|)',
         None,
         None,
         None,
     ),
     UserAgentParser(
-        '(Java)[/ ]{0,1}\\d+\\.(\\d+)\\.(\\d+)[_-]*([a-zA-Z0-9]+)*',
+        '(S3Gof3r)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '\\b(ibm-cos-sdk-(?:core|java|js|python))/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '^(rusoto)/(\\d+)\\.(\\d+)\\.(\\d+)',
+        None,
+        None,
+        None,
+    ),
+    UserAgentParser(
+        '^(rclone)/v(\\d+)\\.(\\d+)',
         None,
         None,
         None,
     ),
     UserAgentParser(
         '^(Roku)/DVP-(\\d+)\\.(\\d+)',
         None,
@@ -1565,14 +1769,20 @@
     ),
     UserAgentParser(
         '^(Box(?: Sync)?)/(\\d+)\\.(\\d+)\\.(\\d+)',
         None,
         None,
         None,
     ),
+    UserAgentParser(
+        '^(ViaFree|Viafree)-(?:tvOS-)?[A-Z]{2}/(\\d+)\\.(\\d+)\\.(\\d+)',
+        'ViaFree',
+        None,
+        None,
+    ),
 ]
 
 DEVICE_PARSERS = [
     DeviceParser(
         '(?:(?:iPhone|Windows CE|Windows Phone|Android).*(?:(?:Bot|Yeti)-Mobile|YRSpider|BingPreview|bots?/\\d|(?:bot|spider)\\.html)|AdsBot-Google-Mobile.*iPhone)',
         'i',
         'Spider',
@@ -1583,22 +1793,36 @@
         '(?:DoCoMo|\\bMOT\\b|\\bLG\\b|Nokia|Samsung|SonyEricsson).*(?:(?:Bot|Yeti)-Mobile|bots?/\\d|(?:bot|crawler)\\.html|(?:jump|google|Wukong)bot|ichiro/mobile|/spider|YahooSeeker)',
         'i',
         'Spider',
         'Spider',
         'Feature Phone',
     ),
     DeviceParser(
+        ' PTST/\\d+(?:\\.)?\\d+$',
+        None,
+        'Spider',
+        'Spider',
+        None,
+    ),
+    DeviceParser(
+        'X11; Datanyze; Linux',
+        None,
+        'Spider',
+        'Spider',
+        None,
+    ),
+    DeviceParser(
         '\\bSmartWatch *\\( *([^;]+) *; *([^;]+) *;',
         None,
         '$1 $2',
         '$1',
         '$2',
     ),
     DeviceParser(
-        'Android Application[^\\-]+ - (Sony) ?(Ericsson)? (.+) \\w+ - ',
+        'Android Application[^\\-]+ - (Sony) ?(Ericsson|) (.+) \\w+ - ',
         None,
         '$1 $2',
         '$1$2',
         '$3',
     ),
     DeviceParser(
         'Android Application[^\\-]+ - (?:HTC|HUAWEI|LGE|LENOVO|MEDION|TCT) (HTC|HUAWEI|LG|LENOVO|MEDION|ALCATEL)[ _\\-](.+) \\w+ - ',
@@ -1625,15 +1849,15 @@
         '; *(?:3Q_)([^;/]+) +Build',
         None,
         '3Q $1',
         '3Q',
         '$1',
     ),
     DeviceParser(
-        'Android [34].*; *(A100|A101|A110|A200|A210|A211|A500|A501|A510|A511|A700(?: Lite| 3G)?|A701|B1-A71|A1-\\d{3}|B1-\\d{3}|V360|V370|W500|W500P|W501|W501P|W510|W511|W700|Slider SL101|DA22[^;/]+) Build',
+        'Android [34].*; *(A100|A101|A110|A200|A210|A211|A500|A501|A510|A511|A700(?: Lite| 3G|)|A701|B1-A71|A1-\\d{3}|B1-\\d{3}|V360|V370|W500|W500P|W501|W501P|W510|W511|W700|Slider SL101|DA22[^;/]+) Build',
         None,
         '$1',
         'Acer',
         '$1',
     ),
     DeviceParser(
         '; *Acer Iconia Tab ([^;/]+) Build',
@@ -1653,22 +1877,22 @@
         '; *(Acer |ACER )([^;/]+) Build',
         None,
         '$1$2',
         'Acer',
         '$2',
     ),
     DeviceParser(
-        '; *(Advent )?(Vega(?:Bean|Comb)?).* Build',
+        '; *(Advent |)(Vega(?:Bean|Comb|)).* Build',
         None,
         '$1$2',
         'Advent',
         '$2',
     ),
     DeviceParser(
-        '; *(Ainol )?((?:NOVO|[Nn]ovo)[^;/]+) Build',
+        '; *(Ainol |)((?:NOVO|[Nn]ovo)[^;/]+) Build',
         None,
         '$1$2',
         'Ainol',
         '$2',
     ),
     DeviceParser(
         '; *AIRIS[ _\\-]?([^/;\\)]+) *(?:;|\\)|Build)',
@@ -1695,15 +1919,15 @@
         '; *(one ?touch) (EVO7|T10|T20) Build',
         None,
         'Alcatel One Touch $2',
         'Alcatel',
         'One Touch $2',
     ),
     DeviceParser(
-        '; *(?:alcatel[ _])?(?:(?:one[ _]?touch[ _])|ot[ \\-])([^;/]+);? Build',
+        '; *(?:alcatel[ _]|)(?:(?:one[ _]?touch[ _])|ot[ \\-])([^;/]+);? Build',
         'i',
         'Alcatel One Touch $1',
         'Alcatel',
         'One Touch $1',
     ),
     DeviceParser(
         '; *(TCL)[ _]([^;/]+) Build',
@@ -1744,15 +1968,15 @@
         '; *(ALLVIEW[ _]?|Allview[ _]?)((?:Speed|SPEED).*) Build/',
         None,
         '$1$2',
         'Allview',
         '$2',
     ),
     DeviceParser(
-        '; *(ALLVIEW[ _]?|Allview[ _]?)?(AX1_Shine|AX2_Frenzy) Build',
+        '; *(ALLVIEW[ _]?|Allview[ _]?|)(AX1_Shine|AX2_Frenzy) Build',
         None,
         '$1$2',
         'Allview',
         '$2',
     ),
     DeviceParser(
         '; *(ALLVIEW[ _]?|Allview[ _]?)([^;/]*) Build',
@@ -1800,15 +2024,15 @@
         '; *(MW(?:0[789]|10)[^;/]+) Build',
         None,
         '$1',
         'Aoc',
         '$1',
     ),
     DeviceParser(
-        '; *(G7|M1013|M1015G|M11[CG]?|M-?12[B]?|M15|M19[G]?|M30[ACQ]?|M31[GQ]|M32|M33[GQ]|M36|M37|M38|M701T|M710|M712B|M713|M715G|M716G|M71(?:G|GS|T)?|M72[T]?|M73[T]?|M75[GT]?|M77G|M79T|M7L|M7LN|M81|M810|M81T|M82|M92|M92KS|M92S|M717G|M721|M722G|M723|M725G|M739|M785|M791|M92SK|M93D) Build',
+        '; *(G7|M1013|M1015G|M11[CG]?|M-?12[B]?|M15|M19[G]?|M30[ACQ]?|M31[GQ]|M32|M33[GQ]|M36|M37|M38|M701T|M710|M712B|M713|M715G|M716G|M71(?:G|GS|T|)|M72[T]?|M73[T]?|M75[GT]?|M77G|M79T|M7L|M7LN|M81|M810|M81T|M82|M92|M92KS|M92S|M717G|M721|M722G|M723|M725G|M739|M785|M791|M92SK|M93D) Build',
         None,
         'Aoson $1',
         'Aoson',
         '$1',
     ),
     DeviceParser(
         '; *Aoson ([^;/]+) Build',
@@ -1884,22 +2108,22 @@
         '; *(?:ARNOVA|Arnova) ?([^;/]+) Build',
         None,
         'Arnova $1',
         'Arnova',
         '$1',
     ),
     DeviceParser(
-        '; *(?:ASSISTANT )?(AP)-?([1789]\\d{2}[A-Z]{0,2}|80104) Build',
+        '; *(?:ASSISTANT |)(AP)-?([1789]\\d{2}[A-Z]{0,2}|80104) Build',
         None,
         'Assistant $1-$2',
         'Assistant',
         '$1-$2',
     ),
     DeviceParser(
-        '; *(ME17\\d[^;/]*|ME3\\d{2}[^;/]+|K00[A-Z]|Nexus 10|Nexus 7(?: 2013)?|PadFone[^;/]*|Transformer[^;/]*|TF\\d{3}[^;/]*|eeepc) Build',
+        '; *(ME17\\d[^;/]*|ME3\\d{2}[^;/]+|K00[A-Z]|Nexus 10|Nexus 7(?: 2013|)|PadFone[^;/]*|Transformer[^;/]*|TF\\d{3}[^;/]*|eeepc) Build',
         None,
         'Asus $1',
         'Asus',
         '$1',
     ),
     DeviceParser(
         '; *ASUS[ _]*([^;/]+) Build',
@@ -2423,15 +2647,15 @@
         '; *(G[^F]?FIVE) ([^;/]+) Build',
         None,
         '$1 $2',
         'Gfive',
         '$2',
     ),
     DeviceParser(
-        '; *(Gionee)[ _\\-]([^;/]+)(?:/[^;/]+)? Build',
+        '; *(Gionee)[ _\\-]([^;/]+)(?:/[^;/]+|) Build',
         'i',
         '$1 $2',
         'Gionee',
         '$2',
     ),
     DeviceParser(
         '; *(GN\\d+[A-Z]?|INFINITY_PASSION|Ctrl_V1) Build',
@@ -2472,15 +2696,15 @@
         '; *(Glass \\d+) Build',
         None,
         '$1',
         'Google',
         '$1',
     ),
     DeviceParser(
-        '; *(Pixel \\w+) Build',
+        '; *(Pixel.*) Build',
         None,
         '$1',
         'Google',
         '$1',
     ),
     DeviceParser(
         '; *(GSmart)[ -]([^/]+) Build',
@@ -2584,15 +2808,15 @@
         '; *([^/]+_tenderloin) Build',
         None,
         'HP TouchPad',
         'HP',
         'TouchPad',
     ),
     DeviceParser(
-        '; *(HUAWEI |Huawei-)?([UY][^;/]+) Build/(?:Huawei|HUAWEI)([UY][^\\);]+)\\)',
+        '; *(HUAWEI |Huawei-|)([UY][^;/]+) Build/(?:Huawei|HUAWEI)([UY][^\\);]+)\\)',
         None,
         '$1$2',
         'Huawei',
         '$2',
     ),
     DeviceParser(
         '; *([^;/]+) Build[/ ]Huawei(MT1-U06|[A-Z]+\\d+[^\\);]+)[^\\);]*\\)',
@@ -2612,15 +2836,15 @@
         '; *((?:HUAWEI|Huawei)[ \\-]?)(MediaPad) Build',
         None,
         '$1$2',
         'Huawei',
         '$2',
     ),
     DeviceParser(
-        '; *((?:HUAWEI[ _]?|Huawei[ _])?Ascend[ _])([^;/]+) Build',
+        '; *((?:HUAWEI[ _]?|Huawei[ _]|)Ascend[ _])([^;/]+) Build',
         None,
         '$1$2',
         'Huawei',
         '$2',
     ),
     DeviceParser(
         '; *((?:HUAWEI|Huawei)[ _\\-]?)((?:G700-|MT-)[^;/]+) Build',
@@ -2675,85 +2899,92 @@
         '; *(Orange Daytona|Pulse|Pulse Mini|Vodafone 858|C8500|C8600|C8650|C8660|Nexus 6P|ATH-.+?) Build[/ ]',
         None,
         'Huawei $1',
         'Huawei',
         '$1',
     ),
     DeviceParser(
+        '; *((?:[A-Z]{3})\\-L[A-Za0-9]{2})[\\)]',
+        None,
+        'Huawei $1',
+        'Huawei',
+        '$1',
+    ),
+    DeviceParser(
         '; *HTC[ _]([^;]+); Windows Phone',
         None,
         'HTC $1',
         'HTC',
         '$1',
     ),
     DeviceParser(
         '; *(?:HTC[ _/])+([^ _/]+)(?:[/\\\\]1\\.0 | V|/| +)\\d+\\.\\d[\\d\\.]*(?: *Build|\\))',
         None,
         'HTC $1',
         'HTC',
         '$1',
     ),
     DeviceParser(
-        '; *(?:HTC[ _/])+([^ _/]+)(?:[ _/]([^ _/]+))?(?:[/\\\\]1\\.0 | V|/| +)\\d+\\.\\d[\\d\\.]*(?: *Build|\\))',
+        '; *(?:HTC[ _/])+([^ _/]+)(?:[ _/]([^ _/]+)|)(?:[/\\\\]1\\.0 | V|/| +)\\d+\\.\\d[\\d\\.]*(?: *Build|\\))',
         None,
         'HTC $1 $2',
         'HTC',
         '$1 $2',
     ),
     DeviceParser(
-        '; *(?:HTC[ _/])+([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ _/]+))?)?(?:[/\\\\]1\\.0 | V|/| +)\\d+\\.\\d[\\d\\.]*(?: *Build|\\))',
+        '; *(?:HTC[ _/])+([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ _/]+)|)|)(?:[/\\\\]1\\.0 | V|/| +)\\d+\\.\\d[\\d\\.]*(?: *Build|\\))',
         None,
         'HTC $1 $2 $3',
         'HTC',
         '$1 $2 $3',
     ),
     DeviceParser(
-        '; *(?:HTC[ _/])+([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ _/]+))?)?)?(?:[/\\\\]1\\.0 | V|/| +)\\d+\\.\\d[\\d\\.]*(?: *Build|\\))',
+        '; *(?:HTC[ _/])+([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ _/]+)|)|)|)(?:[/\\\\]1\\.0 | V|/| +)\\d+\\.\\d[\\d\\.]*(?: *Build|\\))',
         None,
         'HTC $1 $2 $3 $4',
         'HTC',
         '$1 $2 $3 $4',
     ),
     DeviceParser(
-        '; *(?:(?:HTC|htc)(?:_blocked)*[ _/])+([^ _/;]+)(?: *Build|[;\\)]| - )',
+        '; *(?:(?:HTC|htc)(?:_blocked|)[ _/])+([^ _/;]+)(?: *Build|[;\\)]| - )',
         None,
         'HTC $1',
         'HTC',
         '$1',
     ),
     DeviceParser(
-        '; *(?:(?:HTC|htc)(?:_blocked)*[ _/])+([^ _/]+)(?:[ _/]([^ _/;\\)]+))?(?: *Build|[;\\)]| - )',
+        '; *(?:(?:HTC|htc)(?:_blocked|)[ _/])+([^ _/]+)(?:[ _/]([^ _/;\\)]+)|)(?: *Build|[;\\)]| - )',
         None,
         'HTC $1 $2',
         'HTC',
         '$1 $2',
     ),
     DeviceParser(
-        '; *(?:(?:HTC|htc)(?:_blocked)*[ _/])+([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ _/;\\)]+))?)?(?: *Build|[;\\)]| - )',
+        '; *(?:(?:HTC|htc)(?:_blocked|)[ _/])+([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ _/;\\)]+)|)|)(?: *Build|[;\\)]| - )',
         None,
         'HTC $1 $2 $3',
         'HTC',
         '$1 $2 $3',
     ),
     DeviceParser(
-        '; *(?:(?:HTC|htc)(?:_blocked)*[ _/])+([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ /;]+))?)?)?(?: *Build|[;\\)]| - )',
+        '; *(?:(?:HTC|htc)(?:_blocked|)[ _/])+([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ _/]+)(?:[ _/]([^ /;]+)|)|)|)(?: *Build|[;\\)]| - )',
         None,
         'HTC $1 $2 $3 $4',
         'HTC',
         '$1 $2 $3 $4',
     ),
     DeviceParser(
         'HTC Streaming Player [^\\/]*/[^\\/]*/ htc_([^/]+) /',
         None,
         'HTC $1',
         'HTC',
         '$1',
     ),
     DeviceParser(
-        '(?:[;,] *|^)(?:htccn_chs-)?HTC[ _-]?([^;]+?)(?: *Build|clay|Android|-?Mozilla| Opera| Profile| UNTRUSTED|[;/\\(\\)]|$)',
+        '(?:[;,] *|^)(?:htccn_chs-|)HTC[ _-]?([^;]+?)(?: *Build|clay|Android|-?Mozilla| Opera| Profile| UNTRUSTED|[;/\\(\\)]|$)',
         'i',
         'HTC $1',
         'HTC',
         '$1',
     ),
     DeviceParser(
         '; *(A6277|ADR6200|ADR6300|ADR6350|ADR6400[A-Z]*|ADR6425[A-Z]*|APX515CKT|ARIA|Desire[^_ ]*|Dream|EndeavorU|Eris|Evo|Flyer|HD2|Hero|HERO200|Hero CDMA|HTL21|Incredible|Inspire[A-Z0-9]*|Legend|Liberty|Nexus ?(?:One|HD2)|One|One S C2|One[ _]?(?:S|V|X\\+?)\\w*|PC36100|PG06100|PG86100|S31HT|Sensation|Wildfire)(?: Build|[/;\\(\\)])',
@@ -2787,29 +3018,29 @@
         '; *(X700|Hold X|MB-6900) Build',
         None,
         'Hyundai $1',
         'Hyundai',
         '$1',
     ),
     DeviceParser(
-        '; *(?:iBall[ _\\-])?(Andi)[ _]?(\\d[^;/]*) Build',
+        '; *(?:iBall[ _\\-]|)(Andi)[ _]?(\\d[^;/]*) Build',
         'i',
         '$1 $2',
         'iBall',
         '$1 $2',
     ),
     DeviceParser(
         '; *(IBall)(?:[ _]([^;/]+)|) Build',
         'i',
         '$1 $2',
         'iBall',
         '$2',
     ),
     DeviceParser(
-        '; *(NT-\\d+[^ ;/]*|Net[Tt]AB [^;/]+|Mercury [A-Z]+|iconBIT)(?: S/N:[^;/]+)? Build',
+        '; *(NT-\\d+[^ ;/]*|Net[Tt]AB [^;/]+|Mercury [A-Z]+|iconBIT)(?: S/N:[^;/]+|) Build',
         None,
         '$1',
         'IconBIT',
         '$1',
     ),
     DeviceParser(
         '; *(IMO)[ _]([^;/]+) Build',
@@ -2857,29 +3088,29 @@
         '; *(TAB) ?([78][12]4) Build',
         None,
         'Intenso $1',
         'Intenso',
         '$1 $2',
     ),
     DeviceParser(
-        '; *(?:Intex[ _])?(AQUA|Aqua)([ _\\.\\-])([^;/]+) *(?:Build|;)',
+        '; *(?:Intex[ _]|)(AQUA|Aqua)([ _\\.\\-])([^;/]+) *(?:Build|;)',
         None,
         '$1$2$3',
         'Intex',
         '$1 $3',
     ),
     DeviceParser(
-        '; *(?:INTEX|Intex)(?:[_ ]([^\\ _;/]+))(?:[_ ]([^\\ _;/]+))? *(?:Build|;)',
+        '; *(?:INTEX|Intex)(?:[_ ]([^\\ _;/]+))(?:[_ ]([^\\ _;/]+)|) *(?:Build|;)',
         None,
         '$1 $2',
         'Intex',
         '$1 $2',
     ),
     DeviceParser(
-        '; *([iI]Buddy)[ _]?(Connect)(?:_|\\?_| )?([^;/]*) *(?:Build|;)',
+        '; *([iI]Buddy)[ _]?(Connect)(?:_|\\?_| |)([^;/]*) *(?:Build|;)',
         None,
         '$1 $2 $3',
         'Intex',
         'iBuddy $2 $3',
     ),
     DeviceParser(
         '; *(I-Buddy)[ _]([^;/]+) *(?:Build|;)',
@@ -2892,15 +3123,15 @@
         '; *(iOCEAN) ([^/]+) Build',
         'i',
         '$1 $2',
         'iOCEAN',
         '$2',
     ),
     DeviceParser(
-        '; *(TP\\d+(?:\\.\\d+)?\\-\\d[^;/]+) Build',
+        '; *(TP\\d+(?:\\.\\d+|)\\-\\d[^;/]+) Build',
         None,
         'ionik $1',
         'ionik',
         '$1',
     ),
     DeviceParser(
         '; *(M702pro) Build',
@@ -3144,15 +3375,15 @@
         '; *(Zio|Hydro|Torque|Event|EVENT|Echo|Milano|Rise|URBANO PROGRESSO|WX04K|WX06K|WX10K|KYL21|101K|C5[12]\\d{2}) Build/',
         None,
         '$1',
         'Kyocera',
         '$1',
     ),
     DeviceParser(
-        '; *(?:LAVA[ _])?IRIS[ _\\-]?([^/;\\)]+) *(?:;|\\)|Build)',
+        '; *(?:LAVA[ _]|)IRIS[ _\\-]?([^/;\\)]+) *(?:;|\\)|Build)',
         'i',
         'Iris $1',
         'Lava',
         'Iris $1',
     ),
     DeviceParser(
         '; *LAVA[ _]([^;/]+) Build',
@@ -3207,29 +3438,29 @@
         '; *(ThinkPad) ?(Tablet) Build/',
         None,
         'Lenovo $1 $2',
         'Lenovo',
         '$1 $2',
     ),
     DeviceParser(
-        '; *(?:LNV-)?(?:=?[Ll]enovo[ _\\-]?|LENOVO[ _])+(.+?)(?:Build|[;/\\)])',
+        '; *(?:LNV-|)(?:=?[Ll]enovo[ _\\-]?|LENOVO[ _])(.+?)(?:Build|[;/\\)])',
         None,
         'Lenovo $1',
         'Lenovo',
         '$1',
     ),
     DeviceParser(
-        '[;,] (?:Vodafone )?(SmartTab) ?(II) ?(\\d+) Build/',
+        '[;,] (?:Vodafone |)(SmartTab) ?(II) ?(\\d+) Build/',
         None,
         'Lenovo $1 $2 $3',
         'Lenovo',
         '$1 $2 $3',
     ),
     DeviceParser(
-        '; *(?:Ideapad )?K1 Build/',
+        '; *(?:Ideapad |)K1 Build/',
         None,
         'Lenovo Ideapad K1',
         'Lenovo',
         'Ideapad K1',
     ),
     DeviceParser(
         '; *(3GC101|3GW10[01]|A390) Build/',
@@ -3256,15 +3487,15 @@
         '; *(E[34][0-9]{2}|LS[6-8][0-9]{2}|VS[6-9][0-9]+[^;/]+|Nexus 4|Nexus 5X?|GT540f?|Optimus (?:2X|G|4X HD)|OptimusX4HD) *(?:Build|;)',
         None,
         '$1',
         'LG',
         '$1',
     ),
     DeviceParser(
-        '[;:] *(L-\\d+[A-Z]|LGL\\d+[A-Z]?)(?:/V\\d+)? *(?:Build|[;\\)])',
+        '[;:] *(L-\\d+[A-Z]|LGL\\d+[A-Z]?)(?:/V\\d+|) *(?:Build|[;\\)])',
         None,
         '$1',
         'LG',
         '$1',
     ),
     DeviceParser(
         '; *(LG-)([A-Z]{1,2}\\d{2,}[^,;/\\)\\(]*?)(?:Build| V\\d+|[,;/\\)\\(]|$)',
@@ -3340,15 +3571,15 @@
         '; *(M-MP[^;/]+|SmartPad ?\\d{2,}[^;/]+) Build',
         None,
         'Mediacom $1',
         'Mediacom',
         '$1',
     ),
     DeviceParser(
-        '; *(?:MD_)?LIFETAB[ _]([^;/]+) Build',
+        '; *(?:MD_|)LIFETAB[ _]([^;/]+) Build',
         'i',
         'Medion Lifetab $1',
         'Medion',
         'Lifetab $1',
     ),
     DeviceParser(
         '; *MEDION ([^;/]+) Build',
@@ -3417,15 +3648,15 @@
         '; *(Cynus)[ _](F5|T\\d|.+?) *(?:Build|[;/\\)])',
         'i',
         '$1 $2',
         'Mobistel',
         '$1 $2',
     ),
     DeviceParser(
-        '; *(MODECOM )?(FreeTab) ?([^;/]+) Build',
+        '; *(MODECOM |)(FreeTab) ?([^;/]+) Build',
         'i',
         '$1$2 $3',
         'Modecom',
         '$2 $3',
     ),
     DeviceParser(
         '; *(MODECOM )([^;/]+) Build',
@@ -3487,15 +3718,15 @@
         '; *((?:MP[DQ]C|MPG\\d{1,4}|MP\\d{3,4}|MID(?:(?:10[234]|114|43|7[247]|8[24]|7)C|8[01]1))[^;/]*) Build',
         None,
         '$1',
         'Mpman',
         '$1',
     ),
     DeviceParser(
-        '; *(?:MSI[ _])?(Primo\\d+|Enjoy[ _\\-][^;/]+) Build',
+        '; *(?:MSI[ _]|)(Primo\\d+|Enjoy[ _\\-][^;/]+) Build',
         'i',
         '$1',
         'Msi',
         '$1',
     ),
     DeviceParser(
         '; *Multilaser[ _]([^;/]+) Build',
@@ -3515,15 +3746,15 @@
         '; *(My)\\|?(Phone)[ _]([^;/]+) Build',
         None,
         '$1$2 $3',
         'MyPhone',
         '$3',
     ),
     DeviceParser(
-        '; *(A\\d+)[ _](Duo)? Build',
+        '; *(A\\d+)[ _](Duo|) Build',
         'i',
         '$1 $2',
         'MyPhone',
         '$1 $2',
     ),
     DeviceParser(
         '; *(myTab[^;/]*) Build',
@@ -3557,15 +3788,15 @@
         '; *(LT-NA7) Build/',
         None,
         '$1',
         'Nec',
         'Lifetouch Note',
     ),
     DeviceParser(
-        '; *(NXM\\d+[A-z0-9_]*|Next\\d[A-z0-9_ \\-]*|NEXT\\d[A-z0-9_ \\-]*|Nextbook [A-z0-9_ ]*|DATAM803HC|M805)(?: Build|[\\);])',
+        '; *(NXM\\d+[A-Za-z0-9_]*|Next\\d[A-Za-z0-9_ \\-]*|NEXT\\d[A-Za-z0-9_ \\-]*|Nextbook [A-Za-z0-9_ ]*|DATAM803HC|M805)(?: Build|[\\);])',
         None,
         '$1',
         'Nextbook',
         '$1',
     ),
     DeviceParser(
         '; *(Nokia)([ _\\-]*)([^;/]*) Build',
@@ -3578,15 +3809,15 @@
         '; *(Nook ?|Barnes & Noble Nook |BN )([^;/]+) Build',
         None,
         '$1$2',
         'Nook',
         '$2',
     ),
     DeviceParser(
-        '; *(NOOK )?(BNRV200|BNRV200A|BNTV250|BNTV250A|BNTV400|BNTV600|LogicPD Zoom2) Build',
+        '; *(NOOK |)(BNRV200|BNRV200A|BNTV250|BNTV250A|BNTV400|BNTV600|LogicPD Zoom2) Build',
         None,
         '$1$2',
         'Nook',
         '$2',
     ),
     DeviceParser(
         '; Build/(Nook)',
@@ -3669,15 +3900,15 @@
         '; (ONE [a-zA-Z]\\d+) Build/',
         None,
         'OnePlus $1',
         'OnePlus',
         '$1',
     ),
     DeviceParser(
-        '; (ONEPLUS [a-zA-Z]\\d+) Build/',
+        '; (ONEPLUS [a-zA-Z]\\d+)(?: Build/|)',
         None,
         'OnePlus $1',
         'OnePlus',
         '$1',
     ),
     DeviceParser(
         '; *(TP-\\d+) Build/',
@@ -3711,22 +3942,22 @@
         '; *(dL1|DL1) Build',
         None,
         'Panasonic $1',
         'Panasonic',
         '$1',
     ),
     DeviceParser(
-        '; *(SKY[ _])?(IM\\-[AT]\\d{3}[^;/]+).* Build/',
+        '; *(SKY[ _]|)(IM\\-[AT]\\d{3}[^;/]+).* Build/',
         None,
         'Pantech $1$2',
         'Pantech',
         '$1$2',
     ),
     DeviceParser(
-        '; *((?:ADR8995|ADR910L|ADR930L|ADR930VW|PTL21|P8000)(?: 4G)?) Build/',
+        '; *((?:ADR8995|ADR910L|ADR930L|ADR930VW|PTL21|P8000)(?: 4G|)) Build/',
         None,
         '$1',
         'Pantech',
         '$1',
     ),
     DeviceParser(
         '; *Pantech([^;/]+).* Build/',
@@ -3795,15 +4026,15 @@
         '; *(MOMO[^;/]+) Build',
         None,
         '$1',
         'Ployer',
         '$1',
     ),
     DeviceParser(
-        '; *(?:Polaroid[ _])?((?:MIDC\\d{3,}|PMID\\d{2,}|PTAB\\d{3,})[^;/]*)(\\/[^;/]*)? Build/',
+        '; *(?:Polaroid[ _]|)((?:MIDC\\d{3,}|PMID\\d{2,}|PTAB\\d{3,})[^;/]*)(\\/[^;/]*|) Build/',
         None,
         '$1',
         'Polaroid',
         '$1',
     ),
     DeviceParser(
         '; *(?:Polaroid )(Tablet) Build/',
@@ -3823,15 +4054,15 @@
         '; *(TB07STA|TB10STA|TB07FTA|TB10FTA) Build/',
         None,
         '$1',
         'Positivo',
         '$1',
     ),
     DeviceParser(
-        '; *(?:Positivo )?((?:YPY|Ypy)[^;/]+) Build/',
+        '; *(?:Positivo |)((?:YPY|Ypy)[^;/]+) Build/',
         None,
         '$1',
         'Positivo',
         '$1',
     ),
     DeviceParser(
         '; *(MOB-[^;/]+) Build/',
@@ -3851,29 +4082,29 @@
         '; *((?:TAB-PLAYTAB|TAB-PROTAB|PROTAB|PlayTabPro|Mobii[ _\\-]|TAB-P)[^;/]*) Build/',
         None,
         'POV $1',
         'POV',
         '$1',
     ),
     DeviceParser(
-        '; *(?:Prestigio )?((?:PAP|PMP)\\d[^;/]+) Build/',
+        '; *(?:Prestigio |)((?:PAP|PMP)\\d[^;/]+) Build/',
         None,
         'Prestigio $1',
         'Prestigio',
         '$1',
     ),
     DeviceParser(
         '; *(PLT[0-9]{4}.*) Build/',
         None,
         '$1',
         'Proscan',
         '$1',
     ),
     DeviceParser(
-        '; *(A2|A5|A8|A900)_?(Classic)? Build',
+        '; *(A2|A5|A8|A900)_?(Classic|) Build',
         None,
         '$1 $2',
         'Qmobile',
         '$1 $2',
     ),
     DeviceParser(
         '; *(Q[Mm]obile)_([^_]+)_([^_]+) Build',
@@ -3935,50 +4166,50 @@
         ' Build/(RK\\d+)',
         None,
         '$1',
         'Rockchip',
         '$1',
     ),
     DeviceParser(
-        '; *(SAMSUNG |Samsung )?((?:Galaxy (?:Note II|S\\d)|GT-I9082|GT-I9205|GT-N7\\d{3}|SM-N9005)[^;/]*)\\/?[^;/]* Build/',
+        '; *(SAMSUNG |Samsung |)((?:Galaxy (?:Note II|S\\d)|GT-I9082|GT-I9205|GT-N7\\d{3}|SM-N9005)[^;/]*)\\/?[^;/]* Build/',
         None,
         'Samsung $1$2',
         'Samsung',
         '$2',
     ),
     DeviceParser(
-        '; *(Google )?(Nexus [Ss](?: 4G)?) Build/',
+        '; *(Google |)(Nexus [Ss](?: 4G|)) Build/',
         None,
         'Samsung $1$2',
         'Samsung',
         '$2',
     ),
     DeviceParser(
         '; *(SAMSUNG |Samsung )([^\\/]*)\\/[^ ]* Build/',
         None,
         'Samsung $2',
         'Samsung',
         '$2',
     ),
     DeviceParser(
-        '; *(Galaxy(?: Ace| Nexus| S ?II+|Nexus S| with MCR 1.2| Mini Plus 4G)?) Build/',
+        '; *(Galaxy(?: Ace| Nexus| S ?II+|Nexus S| with MCR 1.2| Mini Plus 4G|)) Build/',
         None,
         'Samsung $1',
         'Samsung',
         '$1',
     ),
     DeviceParser(
-        '; *(SAMSUNG[ _\\-] *)+([^;/]+) Build',
+        '; *(SAMSUNG[ _\\-]|)(?:SAMSUNG[ _\\-])([^;/]+) Build',
         None,
         'Samsung $2',
         'Samsung',
         '$2',
     ),
     DeviceParser(
-        '; *(SAMSUNG-)?(GT\\-[BINPS]\\d{4}[^\\/]*)(\\/[^ ]*) Build',
+        '; *(SAMSUNG-|)(GT\\-[BINPS]\\d{4}[^\\/]*)(\\/[^ ]*) Build',
         None,
         'Samsung $1$2$3',
         'Samsung',
         '$2',
     ),
     DeviceParser(
         '(?:; *|^)((?:GT\\-[BIiNPS]\\d{4}|I9\\d{2}0[A-Za-z\\+]?\\b)[^;/\\)]*?)(?:Build|Linux|MIUI|[;/\\)])',
@@ -3991,35 +4222,49 @@
         '; (SAMSUNG-)([A-Za-z0-9\\-]+).* Build/',
         None,
         'Samsung $1$2',
         'Samsung',
         '$2',
     ),
     DeviceParser(
-        '; *((?:SCH|SGH|SHV|SHW|SPH|SC|SM)\\-[A-Za-z0-9 ]+)(/?[^ ]*)? Build',
+        '; *((?:SCH|SGH|SHV|SHW|SPH|SC|SM)\\-[A-Za-z0-9 ]+)(/?[^ ]*|) Build',
         None,
         'Samsung $1',
         'Samsung',
         '$1',
     ),
     DeviceParser(
-        ' ((?:SCH)\\-[A-Za-z0-9 ]+)(/?[^ ]*)? Build',
+        '; *((?:SC)\\-[A-Za-z0-9 ]+)(/?[^ ]*|)\\)',
+        None,
+        'Samsung $1',
+        'Samsung',
+        '$1',
+    ),
+    DeviceParser(
+        ' ((?:SCH)\\-[A-Za-z0-9 ]+)(/?[^ ]*|) Build',
         None,
         'Samsung $1',
         'Samsung',
         '$1',
     ),
     DeviceParser(
         '; *(Behold ?(?:2|II)|YP\\-G[^;/]+|EK-GC100|SCL21|I9300) Build',
         None,
         'Samsung $1',
         'Samsung',
         '$1',
     ),
     DeviceParser(
+        '; *((?:SCH|SGH|SHV|SHW|SPH|SC|SM)\\-[A-Za-z0-9]{5,6})[\\)]',
+        None,
+        'Samsung $1',
+        'Samsung',
+        '$1',
+    ),
+    DeviceParser(
         '; *(SH\\-?\\d\\d[^;/]+|SBM\\d[^;/]+) Build',
         None,
         '$1',
         'Sharp',
         '$1',
     ),
     DeviceParser(
@@ -4145,15 +4390,15 @@
         '; *(Sony ?Ericsson ?)([^;/]+) Build',
         None,
         '$1$2',
         'SonyEricsson',
         '$2',
     ),
     DeviceParser(
-        '; *((?:SK|ST|E|X|LT|MK|MT|WT)\\d{2}[a-z0-9]*(?:-o)?|R800i|U20i) Build',
+        '; *((?:SK|ST|E|X|LT|MK|MT|WT)\\d{2}[a-z0-9]*(?:-o|)|R800i|U20i) Build',
         None,
         '$1',
         'SonyEricsson',
         '$1',
     ),
     DeviceParser(
         '; *(Xperia (?:A8|Arc|Acro|Active|Live with Walkman|Mini|Neo|Play|Pro|Ray|X\\d+)[^;/]*) Build',
@@ -4222,15 +4467,15 @@
         '(PlayStation (?:Portable|Vita|\\d+))',
         None,
         '$1',
         'Sony',
         '$1',
     ),
     DeviceParser(
-        '; *((?:CSL_Spice|Spice|SPICE|CSL)[ _\\-]?)?([Mm][Ii])([ _\\-])?(\\d{3}[^;/]*) Build/',
+        '; *((?:CSL_Spice|Spice|SPICE|CSL)[ _\\-]?|)([Mm][Ii])([ _\\-]|)(\\d{3}[^;/]*) Build/',
         None,
         '$1$2$3$4',
         'Spice',
         'Mi$4',
     ),
     DeviceParser(
         '; *(Sprint )(.+?) *(?:Build|[;/])',
@@ -4362,15 +4607,15 @@
         '; *(T-Mobile G1) Build',
         None,
         '$1',
         'HTC',
         'Dream',
     ),
     DeviceParser(
-        '\\b(T-Mobile ?)?(myTouch)[ _]?([34]G)[ _]?([^\\/]*) (?:Mozilla|Build)',
+        '\\b(T-Mobile ?|)(myTouch)[ _]?([34]G)[ _]?([^\\/]*) (?:Mozilla|Build)',
         None,
         '$1$2 $3 $4',
         'HTC',
         '$2 $3 $4',
     ),
     DeviceParser(
         '\\b(T-Mobile)_([^_]+)_(.*) Build',
@@ -4411,15 +4656,15 @@
         '; *([Ff]olio ?100) Build/',
         None,
         '$1',
         'Toshiba',
         'Folio 100',
     ),
     DeviceParser(
-        '; *(AT[0-9]{2,3}(?:\\-A|LE\\-A|PE\\-A|SE|a)?|AT7-A|AT1S0|Hikari-iFrame/WDPF-[^;/]+|THRiVE|Thrive) Build/',
+        '; *(AT[0-9]{2,3}(?:\\-A|LE\\-A|PE\\-A|SE|a|)|AT7-A|AT1S0|Hikari-iFrame/WDPF-[^;/]+|THRiVE|Thrive) Build/',
         None,
         'Toshiba $1',
         'Toshiba',
         '$1',
     ),
     DeviceParser(
         '; *(TM-MID\\d+[^;/]+|TOUCHMATE|MID-750) Build',
@@ -4523,22 +4768,22 @@
         '(Vodafone) (.*) Build/',
         None,
         '$1 $2',
         '$1',
         '$2',
     ),
     DeviceParser(
-        '; *(?:Walton[ _\\-])?(Primo[ _\\-][^;/]+) Build',
+        '; *(?:Walton[ _\\-]|)(Primo[ _\\-][^;/]+) Build',
         'i',
         'Walton $1',
         'Walton',
         '$1',
     ),
     DeviceParser(
-        '; *(?:WIKO[ \\-])?(CINK\\+?|BARRY|BLOOM|DARKFULL|DARKMOON|DARKNIGHT|DARKSIDE|FIZZ|HIGHWAY|IGGY|OZZY|RAINBOW|STAIRWAY|SUBLIM|WAX|CINK [^;/]+) Build/',
+        '; *(?:WIKO[ \\-]|)(CINK\\+?|BARRY|BLOOM|DARKFULL|DARKMOON|DARKNIGHT|DARKSIDE|FIZZ|HIGHWAY|IGGY|OZZY|RAINBOW|STAIRWAY|SUBLIM|WAX|CINK [^;/]+) Build/',
         'i',
         'Wiko $1',
         'Wiko',
         '$1',
     ),
     DeviceParser(
         '; *WellcoM-([^;/]+) Build',
@@ -4565,29 +4810,50 @@
         '; *(?:Woxter|Wxt) ([^;/]+) Build',
         None,
         'Woxter $1',
         'Woxter',
         '$1',
     ),
     DeviceParser(
-        '; *(?:Xenta |Luna )?(TAB[234][0-9]{2}|TAB0[78]-\\d{3}|TAB0?9-\\d{3}|TAB1[03]-\\d{3}|SMP\\d{2}-\\d{3}) Build/',
+        '; *(?:Xenta |Luna |)(TAB[234][0-9]{2}|TAB0[78]-\\d{3}|TAB0?9-\\d{3}|TAB1[03]-\\d{3}|SMP\\d{2}-\\d{3}) Build/',
         None,
         'Yarvik $1',
         'Yarvik',
         '$1',
     ),
     DeviceParser(
         '; *([A-Z]{2,4})(M\\d{3,}[A-Z]{2})([^;\\)\\/]*)(?: Build|[;\\)])',
         None,
         'Yifang $1$2$3',
         'Yifang',
         '$2',
     ),
     DeviceParser(
-        '; *((MI|HM|MI-ONE|Redmi)[ -](NOTE |Note )?[^;/]*) (Build|MIUI)/',
+        '; *((Mi|MI|HM|MI-ONE|Redmi)[ -](NOTE |Note |)[^;/]*) (Build|MIUI)/',
+        None,
+        'XiaoMi $1',
+        'XiaoMi',
+        '$1',
+    ),
+    DeviceParser(
+        '; *((Mi|MI|HM|MI-ONE|Redmi)[ -](NOTE |Note |)[^;/\\)]*)',
+        None,
+        'XiaoMi $1',
+        'XiaoMi',
+        '$1',
+    ),
+    DeviceParser(
+        '; *(MIX) (Build|MIUI)/',
+        None,
+        'XiaoMi $1',
+        'XiaoMi',
+        '$1',
+    ),
+    DeviceParser(
+        '; *((MIX) ([^;/]*)) (Build|MIUI)/',
         None,
         'XiaoMi $1',
         'XiaoMi',
         '$1',
     ),
     DeviceParser(
         '; *XOLO[ _]([^;/]*tab.*) Build',
@@ -4796,15 +5062,15 @@
         '; ?(Kindle) Build\\b',
         None,
         'Kindle',
         'Amazon',
         'Kindle',
     ),
     DeviceParser(
-        '; ?(Silk)/(\\d+)\\.(\\d+)(?:\\.([0-9\\-]+))? Build\\b',
+        '; ?(Silk)/(\\d+)\\.(\\d+)(?:\\.([0-9\\-]+)|) Build\\b',
         None,
         'Kindle Fire',
         'Amazon',
         'Kindle Fire$2',
     ),
     DeviceParser(
         ' (Kindle)/(\\d+\\.\\d+)',
@@ -4852,127 +5118,148 @@
         '\\bUSCC[_\\-]?([^ ;/\\)]+)',
         None,
         '$1',
         'Cellular',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?)?(?:ALCATEL)[^;]*; *([^;,\\)]+)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|)(?:ALCATEL)[^;]*; *([^;,\\)]+)',
         None,
         'Alcatel $1',
         'Alcatel',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|WpsLondonTest; ?)?(?:ASUS|Asus)[^;]*; *([^;,\\)]+)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|WpsLondonTest; ?|)(?:ASUS|Asus)[^;]*; *([^;,\\)]+)',
         None,
         'Asus $1',
         'Asus',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?)?(?:DELL|Dell)[^;]*; *([^;,\\)]+)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|)(?:DELL|Dell)[^;]*; *([^;,\\)]+)',
         None,
         'Dell $1',
         'Dell',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|WpsLondonTest; ?)?(?:HTC|Htc|HTC_blocked[^;]*)[^;]*; *(?:HTC)?([^;,\\)]+)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|WpsLondonTest; ?|)(?:HTC|Htc|HTC_blocked[^;]*)[^;]*; *(?:HTC|)([^;,\\)]+)',
         None,
         'HTC $1',
         'HTC',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?)?(?:HUAWEI)[^;]*; *(?:HUAWEI )?([^;,\\)]+)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|)(?:HUAWEI)[^;]*; *(?:HUAWEI |)([^;,\\)]+)',
         None,
         'Huawei $1',
         'Huawei',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?)?(?:LG|Lg)[^;]*; *(?:LG[ \\-])?([^;,\\)]+)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|)(?:LG|Lg)[^;]*; *(?:LG[ \\-]|)([^;,\\)]+)',
         None,
         'LG $1',
         'LG',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?)?(?:rv:11; )?(?:NOKIA|Nokia)[^;]*; *(?:NOKIA ?|Nokia ?|LUMIA ?|[Ll]umia ?)*(\\d{3,}[^;\\)]*)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|)(?:rv:11; |)(?:NOKIA|Nokia)[^;]*; *(?:NOKIA ?|Nokia ?|LUMIA ?|[Ll]umia ?|)(\\d{3,10}[^;\\)]*)',
         None,
         'Lumia $1',
         'Nokia',
         'Lumia $1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?)?(?:NOKIA|Nokia)[^;]*; *(RM-\\d{3,})',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|)(?:NOKIA|Nokia)[^;]*; *(RM-\\d{3,})',
         None,
         'Nokia $1',
         'Nokia',
         '$1',
     ),
     DeviceParser(
-        '(?:Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)]|WPDesktop;) ?(?:ARM; ?Touch; ?|Touch; ?)?(?:NOKIA|Nokia)[^;]*; *(?:NOKIA ?|Nokia ?|LUMIA ?|[Ll]umia ?)*([^;\\)]+)',
+        '(?:Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)]|WPDesktop;) ?(?:ARM; ?Touch; ?|Touch; ?|)(?:NOKIA|Nokia)[^;]*; *(?:NOKIA ?|Nokia ?|LUMIA ?|[Ll]umia ?|)([^;\\)]+)',
         None,
         'Nokia $1',
         'Nokia',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?)?(?:Microsoft(?: Corporation)?)[^;]*; *([^;,\\)]+)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|)(?:Microsoft(?: Corporation|))[^;]*; *([^;,\\)]+)',
         None,
         'Microsoft $1',
         'Microsoft',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|WpsLondonTest; ?)?(?:SAMSUNG)[^;]*; *(?:SAMSUNG )?([^;,\\.\\)]+)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|WpsLondonTest; ?|)(?:SAMSUNG)[^;]*; *(?:SAMSUNG |)([^;,\\.\\)]+)',
         None,
         'Samsung $1',
         'Samsung',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|WpsLondonTest; ?)?(?:TOSHIBA|FujitsuToshibaMobileCommun)[^;]*; *([^;,\\)]+)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|WpsLondonTest; ?|)(?:TOSHIBA|FujitsuToshibaMobileCommun)[^;]*; *([^;,\\)]+)',
         None,
         'Toshiba $1',
         'Toshiba',
         '$1',
     ),
     DeviceParser(
-        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|WpsLondonTest; ?)?([^;]+); *([^;,\\)]+)',
+        'Windows Phone [^;]+; .*?IEMobile/[^;\\)]+[;\\)] ?(?:ARM; ?Touch; ?|Touch; ?|WpsLondonTest; ?|)([^;]+); *([^;,\\)]+)',
         None,
         '$1 $2',
         '$1',
         '$2',
     ),
     DeviceParser(
         '(?:^|; )SAMSUNG\\-([A-Za-z0-9\\-]+).* Bada/',
         None,
         'Samsung $1',
         'Samsung',
         '$1',
     ),
     DeviceParser(
-        '\\(Mobile; ALCATEL ?(One|ONE) ?(Touch|TOUCH) ?([^;/]+)(?:/[^;]+)?; rv:[^\\)]+\\) Gecko/[^\\/]+ Firefox/',
+        '\\(Mobile; ALCATEL ?(One|ONE) ?(Touch|TOUCH) ?([^;/]+)(?:/[^;]+|); rv:[^\\)]+\\) Gecko/[^\\/]+ Firefox/',
         None,
         'Alcatel $1 $2 $3',
         'Alcatel',
         'One Touch $3',
     ),
     DeviceParser(
         '\\(Mobile; (?:ZTE([^;]+)|(OpenC)); rv:[^\\)]+\\) Gecko/[^\\/]+ Firefox/',
         None,
         'ZTE $1$2',
         'ZTE',
         '$1$2',
     ),
     DeviceParser(
-        'Nokia(N[0-9]+)([A-z_\\-][A-z0-9_\\-]*)',
+        '\\(Mobile; ALCATEL([A-Za-z0-9\\-]+); rv:[^\\)]+\\) Gecko/[^\\/]+ Firefox/[^\\/]+ KaiOS/',
+        None,
+        'Alcatel $1',
+        'Alcatel',
+        '$1',
+    ),
+    DeviceParser(
+        '\\(Mobile; LYF\\/([A-Za-z0-9\\-]+)\\/.+;.+rv:[^\\)]+\\) Gecko/[^\\/]+ Firefox/[^\\/]+ KAIOS/',
+        None,
+        'LYF $1',
+        'LYF',
+        '$1',
+    ),
+    DeviceParser(
+        '\\(Mobile; Nokia_([A-Za-z0-9\\-]+)_.+; rv:[^\\)]+\\) Gecko/[^\\/]+ Firefox/[^\\/]+ KAIOS/',
+        None,
+        'Nokia $1',
+        'Nokia',
+        '$1',
+    ),
+    DeviceParser(
+        'Nokia(N[0-9]+)([A-Za-z_\\-][A-Za-z0-9_\\-]*)',
         None,
         'Nokia $1',
         'Nokia',
         '$1$2',
     ),
     DeviceParser(
         '(?:NOKIA|Nokia)(?:\\-| *)(?:([A-Za-z0-9]+)\\-[0-9a-f]{32}|([A-Za-z0-9\\-]+)(?:UCBrowser)|([A-Za-z0-9\\-]+))',
@@ -4992,15 +5279,15 @@
         '\\(Symbian; U; S60 V5; [A-z]{2}\\-[A-z]{2}; (SonyEricsson|Samsung|Nokia|LG)([^;/]+)\\)',
         None,
         '$1 $2',
         '$1',
         '$2',
     ),
     DeviceParser(
-        '\\(Symbian(?:/3)?; U; ([^;]+);',
+        '\\(Symbian(?:/3|); U; ([^;]+);',
         None,
         'Nokia $1',
         'Nokia',
         '$1',
     ),
     DeviceParser(
         'BB10; ([A-Za-z0-9\\- ]+)\\)',
@@ -5055,15 +5342,15 @@
         'Treo([A-Za-z0-9]+)',
         None,
         'Palm Treo $1',
         'Palm',
         'Treo $1',
     ),
     DeviceParser(
-        'webOS.*(P160U(?:NA)?)/(\\d+).(\\d+)',
+        'webOS.*(P160U(?:NA|))/(\\d+).(\\d+)',
         None,
         'HP Veer',
         'HP',
         'Veer',
     ),
     DeviceParser(
         '(Touch[Pp]ad)/\\d+\\.\\d+',
@@ -5125,14 +5412,35 @@
         '(iPhone)(?:;| Simulator;)',
         None,
         '$1',
         'Apple',
         '$1',
     ),
     DeviceParser(
+        '(Watch)(\\d+,\\d+)',
+        None,
+        'Apple $1',
+        'Apple',
+        'Apple $1 $2',
+    ),
+    DeviceParser(
+        '(Apple Watch)(?:;| Simulator;)',
+        None,
+        '$1',
+        'Apple',
+        '$1',
+    ),
+    DeviceParser(
+        '(HomePod)(?:;| Simulator;)',
+        None,
+        '$1',
+        'Apple',
+        '$1',
+    ),
+    DeviceParser(
         'iPhone',
         None,
         'iPhone',
         'Apple',
         'iPhone',
     ),
     DeviceParser(
@@ -5188,15 +5496,22 @@
         '(?:; |\\/|^)((?:Transformer (?:Pad|Prime) |Transformer |PadFone[ _]?)[A-Za-z0-9]*)',
         None,
         'Asus $1',
         'Asus',
         '$1',
     ),
     DeviceParser(
-        '(?:asus.*?ASUS|Asus|ASUS|asus)[\\- ;]*((?:Transformer (?:Pad|Prime) |Transformer |Padfone |Nexus[ _])?[A-Za-z0-9]+)',
+        '(?:asus.*?ASUS|Asus|ASUS|asus)[\\- ;]*((?:Transformer (?:Pad|Prime) |Transformer |Padfone |Nexus[ _]|)[A-Za-z0-9]+)',
+        None,
+        'Asus $1',
+        'Asus',
+        '$1',
+    ),
+    DeviceParser(
+        '(?:ASUS)_([A-Za-z0-9\\-]+)',
         None,
         'Asus $1',
         'Asus',
         '$1',
     ),
     DeviceParser(
         '\\bBIRD[ \\-\\.]([A-Za-z0-9]+)',
@@ -5230,15 +5545,15 @@
         '([A-Za-z0-9]+);FOMA',
         None,
         'DoCoMo $1',
         'DoCoMo',
         '$1',
     ),
     DeviceParser(
-        '\\b(?:HTC/|HTC/[a-z0-9]+/)?HTC[ _\\-;]? *(.*?)(?:-?Mozilla|fingerPrint|[;/\\(\\)]|$)',
+        '\\b(?:HTC/|HTC/[a-z0-9]+/|)HTC[ _\\-;]? *(.*?)(?:-?Mozilla|fingerPrint|[;/\\(\\)]|$)',
         None,
         'HTC $1',
         'HTC',
         '$1',
     ),
     DeviceParser(
         'Huawei([A-Za-z0-9]+)',
@@ -5251,14 +5566,21 @@
         'HUAWEI-([A-Za-z0-9]+)',
         None,
         'Huawei $1',
         'Huawei',
         '$1',
     ),
     DeviceParser(
+        'HUAWEI ([A-Za-z0-9\\-]+)',
+        None,
+        'Huawei $1',
+        'Huawei',
+        '$1',
+    ),
+    DeviceParser(
         'vodafone([A-Za-z0-9]+)',
         None,
         'Huawei Vodafone $1',
         'Huawei',
         'Vodafone $1',
     ),
     DeviceParser(
@@ -5293,22 +5615,22 @@
         '(HbbTV)/[0-9]+\\.[0-9]+\\.[0-9]+ \\([^;]*; *(LG)E *; *([^;]*) *;[^;]*;[^;]*;\\)',
         None,
         '$1',
         '$2',
         '$3',
     ),
     DeviceParser(
-        '(HbbTV)/1\\.1\\.1.*CE-HTML/1\\.\\d;(Vendor/)*(THOM[^;]*?)[;\\s](?:.*SW-Version/.*)*(LF[^;]+);?',
+        '(HbbTV)/1\\.1\\.1.*CE-HTML/1\\.\\d;(Vendor/|)(THOM[^;]*?)[;\\s].{0,30}(LF[^;]+);?',
         None,
         '$1',
         'Thomson',
         '$4',
     ),
     DeviceParser(
-        '(HbbTV)(?:/1\\.1\\.1)?(?: ?\\(;;;;;\\))?; *CE-HTML(?:/1\\.\\d)?; *([^ ]+) ([^;]+);',
+        '(HbbTV)(?:/1\\.1\\.1|) ?(?: \\(;;;;;\\)|); *CE-HTML(?:/1\\.\\d|); *([^ ]+) ([^;]+);',
         None,
         '$1',
         '$2',
         '$3',
     ),
     DeviceParser(
         '(HbbTV)/1\\.1\\.1 \\(;;;;;\\) Maple_2011',
@@ -5328,15 +5650,15 @@
         '(HbbTV)/[0-9]+\\.[0-9]+\\.[0-9]+',
         None,
         '$1',
         None,
         None,
     ),
     DeviceParser(
-        'LGE; (?:Media\\/)?([^;]*);[^;]*;[^;]*;?\\); "?LG NetCast(\\.TV|\\.Media|)-\\d+',
+        'LGE; (?:Media\\/|)([^;]*);[^;]*;[^;]*;?\\); "?LG NetCast(\\.TV|\\.Media|)-\\d+',
         None,
         'NetCast$2',
         'LG',
         '$1',
     ),
     DeviceParser(
         'InettvBrowser/[0-9]+\\.[0-9A-Z]+ \\([^;]*;(Sony)([^;]*);[^;]*;[^\\)]*\\)',
@@ -5363,15 +5685,15 @@
         'Series60/\\d\\.\\d (LG)[\\-]?([A-Za-z0-9 \\-]+)',
         None,
         '$1 $2',
         '$1',
         '$2',
     ),
     DeviceParser(
-        '\\b(?:LGE[ \\-]LG\\-(?:AX)?|LGE |LGE?-LG|LGE?[ \\-]|LG[ /\\-]|lg[\\-])([A-Za-z0-9]+)\\b',
+        '\\b(?:LGE[ \\-]LG\\-(?:AX|)|LGE |LGE?-LG|LGE?[ \\-]|LG[ /\\-]|lg[\\-])([A-Za-z0-9]+)\\b',
         None,
         'LG $1',
         'LG',
         '$1',
     ),
     DeviceParser(
         '(?:^LG[\\-]?|^LGE[\\-/]?)([A-Za-z]+[0-9]+[A-Za-z]*)',
@@ -5531,15 +5853,15 @@
         'Android [^;]+; ([^ ]+) (Sony)/',
         None,
         '$2 $1',
         '$2',
         '$1',
     ),
     DeviceParser(
-        '(Sony)(?:BDP\\/|\\/)?([^ /;\\)]+)[ /;\\)]',
+        '(Sony)(?:BDP\\/|\\/|)([^ /;\\)]+)[ /;\\)]',
         None,
         '$1 $2',
         '$1',
         '$2',
     ),
     DeviceParser(
         'Puffin/[\\d\\.]+IT',
@@ -5566,57 +5888,57 @@
         'Puffin/[\\d\\.]+AP',
         None,
         'Generic Smartphone',
         'Generic',
         'Smartphone',
     ),
     DeviceParser(
-        'Android[\\- ][\\d]+\\.[\\d]+; [A-Za-z]{2}\\-[A-Za-z]{0,2}; WOWMobile (.+) Build[/ ]',
+        'Android[\\- ][\\d]+\\.[\\d]+; [A-Za-z]{2}\\-[A-Za-z]{0,2}; WOWMobile (.+)( Build[/ ]|\\))',
         None,
         None,
         'Generic_Android',
         '$1',
     ),
     DeviceParser(
-        'Android[\\- ][\\d]+\\.[\\d]+\\-update1; [A-Za-z]{2}\\-[A-Za-z]{0,2} *; *(.+?) Build[/ ]',
+        'Android[\\- ][\\d]+\\.[\\d]+\\-update1; [A-Za-z]{2}\\-[A-Za-z]{0,2} *; *(.+?)( Build[/ ]|\\))',
         None,
         None,
         'Generic_Android',
         '$1',
     ),
     DeviceParser(
-        'Android[\\- ][\\d]+(?:\\.[\\d]+){1,2}; *[A-Za-z]{2}[_\\-][A-Za-z]{0,2}\\-? *; *(.+?) Build[/ ]',
+        'Android[\\- ][\\d]+(?:\\.[\\d]+)(?:\\.[\\d]+|); *[A-Za-z]{2}[_\\-][A-Za-z]{0,2}\\-? *; *(.+?)( Build[/ ]|\\))',
         None,
         None,
         'Generic_Android',
         '$1',
     ),
     DeviceParser(
-        'Android[\\- ][\\d]+(?:\\.[\\d]+){1,2}; *[A-Za-z]{0,2}\\- *; *(.+?) Build[/ ]',
+        'Android[\\- ][\\d]+(?:\\.[\\d]+)(?:\\.[\\d]+|); *[A-Za-z]{0,2}\\- *; *(.+?)( Build[/ ]|\\))',
         None,
         None,
         'Generic_Android',
         '$1',
     ),
     DeviceParser(
-        'Android[\\- ][\\d]+(?:\\.[\\d]+){1,2}; *[a-z]{0,2}[_\\-]?[A-Za-z]{0,2};? Build[/ ]',
+        'Android[\\- ][\\d]+(?:\\.[\\d]+)(?:\\.[\\d]+|); *[a-z]{0,2}[_\\-]?[A-Za-z]{0,2};?( Build[/ ]|\\))',
         None,
         'Generic Smartphone',
         'Generic',
         'Smartphone',
     ),
     DeviceParser(
-        'Android[\\- ][\\d]+(?:\\.[\\d]+){1,2}; *\\-?[A-Za-z]{2}; *(.+?) Build[/ ]',
+        'Android[\\- ][\\d]+(?:\\.[\\d]+)(?:\\.[\\d]+|); *\\-?[A-Za-z]{2}; *(.+?)( Build[/ ]|\\))',
         None,
         None,
         'Generic_Android',
         '$1',
     ),
     DeviceParser(
-        'Android[\\- ][\\d]+(?:\\.[\\d]+){1,2}(?:;.*)?; *(.+?) Build[/ ]',
+        'Android[\\- ][\\d]+(?:\\.[\\d]+)(?:\\.[\\d]+|)(?:;.*|); *(.+?)( Build[/ ]|\\))',
         None,
         None,
         'Generic_Android',
         '$1',
     ),
     DeviceParser(
         '(GoogleTV)',
@@ -5657,15 +5979,15 @@
         '(hiptop|avantgo|plucker|xiino|blazer|elaine)',
         'i',
         'Generic Smartphone',
         'Generic',
         'Smartphone',
     ),
     DeviceParser(
-        '(bot|BUbiNG|zao|borg|DBot|oegp|silk|Xenu|zeal|^NING|CCBot|crawl|htdig|lycos|slurp|teoma|voila|yahoo|Sogou|CiBra|Nutch|^Java/|^JNLP/|Daumoa|Genieo|ichiro|larbin|pompos|Scrapy|snappy|speedy|spider|msnbot|msrbot|vortex|^vortex|crawler|favicon|indexer|Riddler|scooter|scraper|scrubby|WhatWeb|WinHTTP|bingbot|BingPreview|openbot|gigabot|furlbot|polybot|seekbot|^voyager|archiver|Icarus6j|mogimogi|Netvibes|blitzbot|altavista|charlotte|findlinks|Retreiver|TLSProber|WordPress|SeznamBot|ProoXiBot|wsr\\-agent|Squrl Java|EtaoSpider|PaperLiBot|SputnikBot|A6\\-Indexer|netresearch|searchsight|baiduspider|YisouSpider|ICC\\-Crawler|http%20client|Python-urllib|dataparksearch|converacrawler|Screaming Frog|AppEngine-Google|YahooCacheSystem|fast\\-webcrawler|Sogou Pic Spider|semanticdiscovery|Innovazion Crawler|facebookexternalhit|Google.*/\\+/web/snippet|Google-HTTP-Java-Client|BlogBridge|IlTrovatore-Setaccio|InternetArchive|GomezAgent|WebThumbnail|heritrix|NewsGator|PagePeeker|Reaper|ZooShot|holmes|NL-Crawler|Pingdom|StatusCake|WhatsApp|masscan|Google Web Preview|Qwantify)',
+        '(bot|BUbiNG|zao|borg|DBot|oegp|silk|Xenu|zeal|^NING|CCBot|crawl|htdig|lycos|slurp|teoma|voila|yahoo|Sogou|CiBra|Nutch|^Java/|^JNLP/|Daumoa|Daum|Genieo|ichiro|larbin|pompos|Scrapy|snappy|speedy|spider|msnbot|msrbot|vortex|^vortex|crawler|favicon|indexer|Riddler|scooter|scraper|scrubby|WhatWeb|WinHTTP|bingbot|BingPreview|openbot|gigabot|furlbot|polybot|seekbot|^voyager|archiver|Icarus6j|mogimogi|Netvibes|blitzbot|altavista|charlotte|findlinks|Retreiver|TLSProber|WordPress|SeznamBot|ProoXiBot|wsr\\-agent|Squrl Java|EtaoSpider|PaperLiBot|SputnikBot|A6\\-Indexer|netresearch|searchsight|baiduspider|YisouSpider|ICC\\-Crawler|http%20client|Python-urllib|dataparksearch|converacrawler|Screaming Frog|AppEngine-Google|YahooCacheSystem|fast\\-webcrawler|Sogou Pic Spider|semanticdiscovery|Innovazion Crawler|facebookexternalhit|Google.*/\\+/web/snippet|Google-HTTP-Java-Client|BlogBridge|IlTrovatore-Setaccio|InternetArchive|GomezAgent|WebThumbnail|heritrix|NewsGator|PagePeeker|Reaper|ZooShot|holmes|NL-Crawler|Pingdom|StatusCake|WhatsApp|masscan|Google Web Preview|Qwantify|Yeti|OgScrper)',
         'i',
         'Spider',
         'Spider',
         'Desktop',
     ),
     DeviceParser(
         '^(1207|3gso|4thp|501i|502i|503i|504i|505i|506i|6310|6590|770s|802s|a wa|acer|acs\\-|airn|alav|asus|attw|au\\-m|aur |aus |abac|acoo|aiko|alco|alca|amoi|anex|anny|anyw|aptu|arch|argo|bmobile|bell|bird|bw\\-n|bw\\-u|beck|benq|bilb|blac|c55/|cdm\\-|chtm|capi|comp|cond|dall|dbte|dc\\-s|dica|ds\\-d|ds12|dait|devi|dmob|doco|dopo|dorado|el(?:38|39|48|49|50|55|58|68)|el[3456]\\d{2}dual|erk0|esl8|ex300|ez40|ez60|ez70|ezos|ezze|elai|emul|eric|ezwa|fake|fly\\-|fly_|g\\-mo|g1 u|g560|gf\\-5|grun|gene|go.w|good|grad|hcit|hd\\-m|hd\\-p|hd\\-t|hei\\-|hp i|hpip|hs\\-c|htc |htc\\-|htca|htcg)',
@@ -5749,31 +6071,31 @@
         None,
         None,
         'UE32F4500',
         None,
         None,
     ),
     OSParser(
-        'HbbTV/1.1.1 \\(; (Philips);.*NETTV/4',
+        'HbbTV/1\\.1\\.1 \\(; (Philips);.*NETTV/4',
         None,
         '2013',
         None,
         None,
         None,
     ),
     OSParser(
-        'HbbTV/1.1.1 \\(; (Philips);.*NETTV/3',
+        'HbbTV/1\\.1\\.1 \\(; (Philips);.*NETTV/3',
         None,
         '2012',
         None,
         None,
         None,
     ),
     OSParser(
-        'HbbTV/1.1.1 \\(; (Philips);.*NETTV/2',
+        'HbbTV/1\\.1\\.1 \\(; (Philips);.*NETTV/2',
         None,
         '2011',
         None,
         None,
         None,
     ),
     OSParser(
@@ -5797,23 +6119,23 @@
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(CPU[ +]OS|iPhone[ +]OS|CPU[ +]iPhone)[ +]+(\\d+)[_\\.](\\d+)(?:[_\\.](\\d+))?.*Outlook-iOS-Android',
+        '(CPU[ +]OS|iPhone[ +]OS|CPU[ +]iPhone)[ +]+(\\d+)[_\\.](\\d+)(?:[_\\.](\\d+)|).*Outlook-iOS-Android',
         'iOS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(Android)[ \\-/](\\d+)\\.(\\d+)(?:[.\\-]([a-z0-9]+))?',
+        '(Android)[ \\-/](\\d+)(?:\\.(\\d+)|)(?:[.\\-]([a-z0-9]+)|)',
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -5853,39 +6175,47 @@
         None,
         '3',
         None,
         None,
         None,
     ),
     OSParser(
-        '^UCWEB.*; (Adr) (\\d+)\\.(\\d+)(?:[.\\-]([a-z0-9]+))?;',
+        '^UCWEB.*; (Adr) (\\d+)\\.(\\d+)(?:[.\\-]([a-z0-9]+)|);',
         'Android',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '^UCWEB.*; (iPad|iPh|iPd) OS (\\d+)_(\\d+)(?:_(\\d+))?;',
+        '^UCWEB.*; (iPad|iPh|iPd) OS (\\d+)_(\\d+)(?:_(\\d+)|);',
         'iOS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '^UCWEB.*; (wds) (\\d+)\\.(\\d+)(?:\\.(\\d+))?;',
+        '^UCWEB.*; (wds) (\\d+)\\.(\\d+)(?:\\.(\\d+)|);',
         'Windows Phone',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '^(JUC).*; ?U; ?(?:Android)?(\\d+)\\.(\\d+)(?:[\\.\\-]([a-z0-9]+))?',
+        '^(JUC).*; ?U; ?(?:Android|)(\\d+)\\.(\\d+)(?:[\\.\\-]([a-z0-9]+)|)',
+        'Android',
+        None,
+        None,
+        None,
+        None,
+    ),
+    OSParser(
+        '(android)\\s(?:mobile\\/)(\\d+)(?:\\.(\\d+)(?:\\.(\\d+)|)|)',
         'Android',
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -5893,14 +6223,22 @@
         'Android',
         None,
         None,
         None,
         None,
     ),
     OSParser(
+        '(x86_64|aarch64)\\ (\\d+)\\.(\\d+)\\.(\\d+).*Chrome.*(?:CitrixChromeApp)$',
+        'Chrome OS',
+        None,
+        None,
+        None,
+        None,
+    ),
+    OSParser(
         '(XBLWP7)',
         'Windows Phone',
         None,
         None,
         None,
         None,
     ),
@@ -5909,14 +6247,22 @@
         'Windows Mobile',
         None,
         None,
         None,
         None,
     ),
     OSParser(
+        '(Windows 10)',
+        'Windows',
+        '10',
+        None,
+        None,
+        None,
+    ),
+    OSParser(
         '(Windows (?:NT 5\\.2|NT 5\\.1))',
         'Windows',
         'XP',
         None,
         None,
         None,
     ),
@@ -5941,22 +6287,14 @@
         'Windows',
         'ME',
         None,
         None,
         None,
     ),
     OSParser(
-        '(Windows 98|Windows XP|Windows ME|Windows 95|Windows CE|Windows 7|Windows NT 4\\.0|Windows Vista|Windows 2000|Windows 3.1)',
-        None,
-        None,
-        None,
-        None,
-        None,
-    ),
-    OSParser(
         '(Windows NT 6\\.2; ARM;)',
         'Windows',
         'RT',
         None,
         None,
         None,
     ),
@@ -5967,24 +6305,24 @@
         None,
         None,
         None,
     ),
     OSParser(
         '(Windows NT 6\\.3; ARM;)',
         'Windows',
-        'RT 8.1',
-        None,
+        'RT 8',
+        '1',
         None,
         None,
     ),
     OSParser(
         '(Windows NT 6\\.3)',
         'Windows',
-        '8.1',
-        None,
+        '8',
+        '1',
         None,
         None,
     ),
     OSParser(
         '(Windows NT 6\\.4)',
         'Windows',
         '10',
@@ -6021,15 +6359,15 @@
         'Windows',
         'CE',
         None,
         None,
         None,
     ),
     OSParser(
-        'Win ?(95|98|3.1|NT|ME|2000)',
+        'Win(?:dows)? ?(95|98|3.1|NT|ME|2000|XP|Vista|7|CE)',
         'Windows',
         '$1',
         None,
         None,
         None,
     ),
     OSParser(
@@ -6061,22 +6399,30 @@
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '((?:Mac[ +]?|; )OS[ +]X)[\\s+/](?:(\\d+)[_.](\\d+)(?:[_.](\\d+))?|Mach-O)',
+        '((?:Mac[ +]?|; )OS[ +]X)[\\s+/](?:(\\d+)[_.](\\d+)(?:[_.](\\d+)|)|Mach-O)',
         'Mac OS X',
         None,
         None,
         None,
         None,
     ),
     OSParser(
+        '\\w+\\s+Mac OS X\\s+\\w+\\s+(\\d+).(\\d+).(\\d+).*',
+        'Mac OS X',
+        '$1',
+        '$2',
+        '$3',
+        None,
+    ),
+    OSParser(
         ' (Dar)(win)/(9).(\\d+).*\\((?:i386|x86_64|Power Macintosh)\\)',
         'Mac OS X',
         '10',
         '5',
         None,
         None,
     ),
@@ -6125,31 +6471,31 @@
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '^Box.*;(Darwin)/(10)\\.(1\\d)(?:\\.(\\d+))?',
+        '^Box.*;(Darwin)/(10)\\.(1\\d)(?:\\.(\\d+)|)',
         'Mac OS X',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(Apple\\s?TV)(?:/(\\d+)\\.(\\d+))?',
+        '(Apple\\s?TV)(?:/(\\d+)\\.(\\d+)|)',
         'ATV OS X',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(CPU[ +]OS|iPhone[ +]OS|CPU[ +]iPhone|CPU IPhone OS)[ +]+(\\d+)[_\\.](\\d+)(?:[_\\.](\\d+))?',
+        '(CPU[ +]OS|iPhone[ +]OS|CPU[ +]iPhone|CPU IPhone OS)[ +]+(\\d+)[_\\.](\\d+)(?:[_\\.](\\d+)|)',
         'iOS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -6277,22 +6623,54 @@
         'Mac OS X',
         '10',
         '11',
         None,
         None,
     ),
     OSParser(
+        'CFNetwork/7.* Darwin/15\\.4\\.\\d+',
+        'iOS',
+        '9',
+        '3',
+        '1',
+        None,
+    ),
+    OSParser(
+        'CFNetwork/7.* Darwin/15\\.5\\.\\d+',
+        'iOS',
+        '9',
+        '3',
+        '2',
+        None,
+    ),
+    OSParser(
+        'CFNetwork/7.* Darwin/15\\.6\\.\\d+',
+        'iOS',
+        '9',
+        '3',
+        '5',
+        None,
+    ),
+    OSParser(
         '(CF)(Network)/758\\.(\\d)',
         'iOS',
         '9',
         None,
         None,
         None,
     ),
     OSParser(
+        'CFNetwork/808\\.3 Darwin/16\\.3\\.\\d+',
+        'iOS',
+        '10',
+        '2',
+        '1',
+        None,
+    ),
+    OSParser(
         '(CF)(Network)/808\\.(\\d)',
         'iOS',
         '10',
         None,
         None,
         None,
     ),
@@ -6429,31 +6807,79 @@
         'iOS',
         '11',
         '2',
         None,
         None,
     ),
     OSParser(
+        'CFNetwork/8.* Darwin/17\\.4\\.\\d+',
+        'iOS',
+        '11',
+        '2',
+        '6',
+        None,
+    ),
+    OSParser(
+        'CFNetwork/8.* Darwin/17\\.5\\.\\d+',
+        'iOS',
+        '11',
+        '3',
+        None,
+        None,
+    ),
+    OSParser(
+        'CFNetwork/9.* Darwin/17\\.6\\.\\d+',
+        'iOS',
+        '11',
+        '4',
+        None,
+        None,
+    ),
+    OSParser(
+        'CFNetwork/9.* Darwin/17\\.7\\.\\d+',
+        'iOS',
+        '11',
+        '4',
+        '1',
+        None,
+    ),
+    OSParser(
         'CFNetwork/8.* Darwin/(17)\\.\\d+',
         'iOS',
         '11',
         None,
         None,
         None,
     ),
     OSParser(
+        'CFNetwork/9.* Darwin/18\\.0\\.\\d+',
+        'iOS',
+        '12',
+        '0',
+        None,
+        None,
+    ),
+    OSParser(
+        'CFNetwork/9.* Darwin/(18)\\.\\d+',
+        'iOS',
+        '12',
+        None,
+        None,
+        None,
+    ),
+    OSParser(
         'CFNetwork/.* Darwin/',
         'iOS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '\\b(iOS[ /]|iOS; |iPhone(?:/| v|[ _]OS[/,]|; | OS : |\\d,\\d/|\\d,\\d; )|iPad/)(\\d{1,2})[_\\.](\\d{1,2})(?:[_\\.](\\d+))?',
+        '\\b(iOS[ /]|iOS; |iPhone(?:/| v|[ _]OS[/,]|; | OS : |\\d,\\d/|\\d,\\d; )|iPad/)(\\d{1,2})[_\\.](\\d{1,2})(?:[_\\.](\\d+)|)',
         'iOS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -6461,31 +6887,47 @@
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
+        '(watchOS)/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
+        'WatchOS',
+        None,
+        None,
+        None,
+        None,
+    ),
+    OSParser(
         'Outlook-(iOS)/\\d+\\.\\d+\\.prod\\.iphone',
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(tvOS)/(\\d+).(\\d+)',
+        '(iPod|iPhone|iPad)',
+        'iOS',
+        None,
+        None,
+        None,
+        None,
+    ),
+    OSParser(
+        '(tvOS)[/ ](\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'tvOS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(CrOS) [a-z0-9_]+ (\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(CrOS) [a-z0-9_]+ (\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'Chrome OS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -6493,23 +6935,23 @@
         'Debian',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(Linux Mint)(?:/(\\d+))?',
+        '(Linux Mint)(?:/(\\d+)|)',
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(Mandriva)(?: Linux)?/(?:[\\d.-]+m[a-z]{2}(\\d+).(\\d))?',
+        '(Mandriva)(?: Linux|)/(?:[\\d.-]+m[a-z]{2}(\\d+).(\\d)|)',
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -6589,23 +7031,23 @@
         'BlackBerry OS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(Black[Bb]erry)[0-9a-z]+/(\\d+)\\.(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(Black[Bb]erry)[0-9a-z]+/(\\d+)\\.(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'BlackBerry OS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(Black[Bb]erry).+Version/(\\d+)\\.(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(Black[Bb]erry).+Version/(\\d+)\\.(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'BlackBerry OS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -6629,14 +7071,22 @@
         'BlackBerry OS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
+        '(K[Aa][Ii]OS)\\/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
+        'KaiOS',
+        None,
+        None,
+        None,
+        None,
+    ),
+    OSParser(
         '\\((?:Mobile|Tablet);.+Gecko/18.0 Firefox/\\d+\\.\\d+',
         'Firefox OS',
         '1',
         '0',
         '1',
         None,
     ),
@@ -6725,15 +7175,15 @@
         'Brew MP',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(GoogleTV)(?: (\\d+)\\.(\\d+)(?:\\.(\\d+))?|/[\\da-z]+)',
+        '(GoogleTV)(?: (\\d+)\\.(\\d+)(?:\\.(\\d+)|)|/[\\da-z]+)',
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -6741,23 +7191,23 @@
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(CrKey)(?:[/](\\d+)\\.(\\d+)(?:\\.(\\d+))?)?',
+        '(CrKey)(?:[/](\\d+)\\.(\\d+)(?:\\.(\\d+)|)|)',
         'Chromecast',
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(hpw|web)OS/(\\d+)\\.(\\d+)(?:\\.(\\d+))?',
+        '(hpw|web)OS/(\\d+)\\.(\\d+)(?:\\.(\\d+)|)',
         'webOS',
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -6765,23 +7215,23 @@
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(Fedora|Red Hat|PCLinuxOS|Puppy|Ubuntu|Kindle|Bada|Lubuntu|BackTrack|Slackware|(?:Free|Open|Net|\\b)BSD)[/ ](\\d+)\\.(\\d+)(?:\\.(\\d+)(?:\\.(\\d+))?)?',
+        '(Fedora|Red Hat|PCLinuxOS|Puppy|Ubuntu|Kindle|Bada|Sailfish|Lubuntu|BackTrack|Slackware|(?:Free|Open|Net|\\b)BSD)[/ ](\\d+)\\.(\\d+)(?:\\.(\\d+)|)(?:\\.(\\d+)|)',
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(Linux)[ /](\\d+)\\.(\\d+)(?:\\.(\\d+))?.*gentoo',
+        '(Linux)[ /](\\d+)\\.(\\d+)(?:\\.(\\d+)|).*gentoo',
         'Gentoo',
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -6805,15 +7255,15 @@
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
-        '(Linux)(?:[ /](\\d+)\\.(\\d+)(?:\\.(\\d+))?)?',
+        '(Linux)(?:[ /](\\d+)\\.(\\d+)(?:\\.(\\d+)|)|)',
         None,
         None,
         None,
         None,
         None,
     ),
     OSParser(
@@ -6821,14 +7271,46 @@
         'Solaris',
         None,
         None,
         None,
         None,
     ),
     OSParser(
+        '\\(linux-gnu\\)',
+        'Linux',
+        None,
+        None,
+        None,
+        None,
+    ),
+    OSParser(
+        '\\(x86_64-redhat-linux-gnu\\)',
+        'Red Hat',
+        None,
+        None,
+        None,
+        None,
+    ),
+    OSParser(
+        '\\((freebsd)(\\d+)\\.(\\d+)\\)',
+        'FreeBSD',
+        None,
+        None,
+        None,
+        None,
+    ),
+    OSParser(
+        'linux',
+        'Linux',
+        None,
+        None,
+        None,
+        None,
+    ),
+    OSParser(
         '^(Roku)/DVP-(\\d+)\\.(\\d+)',
         None,
         None,
         None,
         None,
         None,
     ),
```

### Comparing `ua-parser-0.8.0/ua_parser/user_agent_parser.py` & `ua-parser-0.9.0/ua_parser/user_agent_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 """Python implementation of the UA parser."""
 
 from __future__ import absolute_import
 
 import os
 import re
 
-__author__ = 'Lindsey Simon <elsigh@gmail.com>'
+__author__ = "Lindsey Simon <elsigh@gmail.com>"
 
 
 class UserAgentParser(object):
-    def __init__(self, pattern, family_replacement=None, v1_replacement=None, v2_replacement=None):
+    def __init__(
+        self, pattern, family_replacement=None, v1_replacement=None, v2_replacement=None
+    ):
         """Initialize UserAgentParser.
 
         Args:
           pattern: a regular expression string
           family_replacement: a string to override the matched family (optional)
           v1_replacement: a string to override the matched v1 (optional)
           v2_replacement: a string to override the matched v2 (optional)
@@ -38,50 +40,57 @@
         self.v1_replacement = v1_replacement
         self.v2_replacement = v2_replacement
 
     def MatchSpans(self, user_agent_string):
         match_spans = []
         match = self.user_agent_re.search(user_agent_string)
         if match:
-            match_spans = [match.span(group_index)
-                           for group_index in range(1, match.lastindex + 1)]
+            match_spans = [
+                match.span(group_index) for group_index in range(1, match.lastindex + 1)
+            ]
         return match_spans
 
     def Parse(self, user_agent_string):
         family, v1, v2, v3 = None, None, None, None
         match = self.user_agent_re.search(user_agent_string)
         if match:
             if self.family_replacement:
-                if re.search(r'\$1', self.family_replacement):
-                    family = re.sub(r'\$1', match.group(1), self.family_replacement)
+                if re.search(r"\$1", self.family_replacement):
+                    family = re.sub(r"\$1", match.group(1), self.family_replacement)
                 else:
                     family = self.family_replacement
             else:
                 family = match.group(1)
 
             if self.v1_replacement:
                 v1 = self.v1_replacement
             elif match.lastindex and match.lastindex >= 2:
-                v1 = match.group(2)
+                v1 = match.group(2) or None
 
             if self.v2_replacement:
                 v2 = self.v2_replacement
             elif match.lastindex and match.lastindex >= 3:
-                v2 = match.group(3)
+                v2 = match.group(3) or None
 
             if match.lastindex and match.lastindex >= 4:
-                v3 = match.group(4)
+                v3 = match.group(4) or None
 
         return family, v1, v2, v3
 
 
 class OSParser(object):
-    def __init__(self, pattern, os_replacement=None,
-                 os_v1_replacement=None, os_v2_replacement=None,
-                 os_v3_replacement=None, os_v4_replacement=None):
+    def __init__(
+        self,
+        pattern,
+        os_replacement=None,
+        os_v1_replacement=None,
+        os_v2_replacement=None,
+        os_v3_replacement=None,
+        os_v4_replacement=None,
+    ):
         """Initialize UserAgentParser.
 
         Args:
           pattern: a regular expression string
           os_replacement: a string to override the matched os (optional)
           os_v1_replacement: a string to override the matched v1 (optional)
           os_v2_replacement: a string to override the matched v2 (optional)
@@ -96,110 +105,113 @@
         self.os_v3_replacement = os_v3_replacement
         self.os_v4_replacement = os_v4_replacement
 
     def MatchSpans(self, user_agent_string):
         match_spans = []
         match = self.user_agent_re.search(user_agent_string)
         if match:
-            match_spans = [match.span(group_index)
-                           for group_index in range(1, match.lastindex + 1)]
+            match_spans = [
+                match.span(group_index) for group_index in range(1, match.lastindex + 1)
+            ]
         return match_spans
 
     def Parse(self, user_agent_string):
         os, os_v1, os_v2, os_v3, os_v4 = None, None, None, None, None
         match = self.user_agent_re.search(user_agent_string)
         if match:
             if self.os_replacement:
-                if re.search(r'\$1', self.os_replacement):
-                    os = re.sub(r'\$1', match.group(1), self.os_replacement)
-                else:
-                    os = self.os_replacement
+                os = MultiReplace(self.os_replacement, match)
             elif match.lastindex:
                 os = match.group(1)
 
             if self.os_v1_replacement:
-                if re.search(r'\$1', self.os_v1_replacement):
-                    os_v1 = re.sub(r'\$1', match.group(1), self.os_v1_replacement)
-                else:
-                    os_v1 = self.os_v1_replacement
+                os_v1 = MultiReplace(self.os_v1_replacement, match)
             elif match.lastindex and match.lastindex >= 2:
                 os_v1 = match.group(2)
 
             if self.os_v2_replacement:
-                os_v2 = self.os_v2_replacement
+                os_v2 = MultiReplace(self.os_v2_replacement, match)
             elif match.lastindex and match.lastindex >= 3:
                 os_v2 = match.group(3)
 
             if self.os_v3_replacement:
-                os_v3 = self.os_v3_replacement
+                os_v3 = MultiReplace(self.os_v3_replacement, match)
             elif match.lastindex and match.lastindex >= 4:
                 os_v3 = match.group(4)
 
             if self.os_v4_replacement:
-                os_v4 = self.os_v4_replacement
+                os_v4 = MultiReplace(self.os_v4_replacement, match)
             elif match.lastindex and match.lastindex >= 5:
                 os_v4 = match.group(5)
 
         return os, os_v1, os_v2, os_v3, os_v4
 
 
+def MultiReplace(string, match):
+    def _repl(m):
+        index = int(m.group(1)) - 1
+        group = match.groups()
+        if index < len(group):
+            return group[index]
+        return ""
+
+    _string = re.sub(r"\$(\d)", _repl, string)
+    _string = re.sub(r"^\s+|\s+$", "", _string)
+    if _string == "":
+        return None
+    return _string
+
+
 class DeviceParser(object):
-    def __init__(self, pattern, regex_flag=None, device_replacement=None, brand_replacement=None,
-                 model_replacement=None):
+    def __init__(
+        self,
+        pattern,
+        regex_flag=None,
+        device_replacement=None,
+        brand_replacement=None,
+        model_replacement=None,
+    ):
         """Initialize UserAgentParser.
 
         Args:
           pattern: a regular expression string
           device_replacement: a string to override the matched device (optional)
         """
         self.pattern = pattern
-        if regex_flag == 'i':
+        if regex_flag == "i":
             self.user_agent_re = re.compile(self.pattern, re.IGNORECASE)
         else:
             self.user_agent_re = re.compile(self.pattern)
         self.device_replacement = device_replacement
         self.brand_replacement = brand_replacement
         self.model_replacement = model_replacement
 
     def MatchSpans(self, user_agent_string):
         match_spans = []
         match = self.user_agent_re.search(user_agent_string)
         if match:
-            match_spans = [match.span(group_index)
-                           for group_index in range(1, match.lastindex + 1)]
+            match_spans = [
+                match.span(group_index) for group_index in range(1, match.lastindex + 1)
+            ]
         return match_spans
 
-    def MultiReplace(self, string, match):
-        def _repl(m):
-            index = int(m.group(1)) - 1
-            group = match.groups()
-            if index < len(group):
-                return group[index]
-            return ''
-
-        _string = re.sub(r'\$(\d)', _repl, string)
-        _string = re.sub(r'^\s+|\s+$', '', _string)
-        if _string == '':
-            return None
-        return _string
-
     def Parse(self, user_agent_string):
         device, brand, model = None, None, None
         match = self.user_agent_re.search(user_agent_string)
         if match:
             if self.device_replacement:
-                device = self.MultiReplace(self.device_replacement, match)
+                device = MultiReplace(self.device_replacement, match)
             else:
                 device = match.group(1)
 
             if self.brand_replacement:
-                brand = self.MultiReplace(self.brand_replacement, match)
+                brand = MultiReplace(self.brand_replacement, match)
 
             if self.model_replacement:
-                model = self.MultiReplace(self.model_replacement, match)
+                model = MultiReplace(self.model_replacement, match)
             elif len(match.groups()) > 0:
                 model = match.group(1)
 
         return device, brand, model
 
 
 MAX_CACHE_SIZE = 20
@@ -218,65 +230,66 @@
     key = (user_agent_string, repr(jsParseBits))
     cached = _parse_cache.get(key)
     if cached is not None:
         return cached
     if len(_parse_cache) > MAX_CACHE_SIZE:
         _parse_cache.clear()
     v = {
-        'user_agent': ParseUserAgent(user_agent_string, **jsParseBits),
-        'os': ParseOS(user_agent_string, **jsParseBits),
-        'device': ParseDevice(user_agent_string, **jsParseBits),
-        'string': user_agent_string
+        "user_agent": ParseUserAgent(user_agent_string, **jsParseBits),
+        "os": ParseOS(user_agent_string, **jsParseBits),
+        "device": ParseDevice(user_agent_string, **jsParseBits),
+        "string": user_agent_string,
     }
     _parse_cache[key] = v
     return v
 
 
 def ParseUserAgent(user_agent_string, **jsParseBits):
     """ Parses the user-agent string for user agent (browser) info.
     Args:
       user_agent_string: The full user-agent string.
       jsParseBits: javascript override bits.
     Returns:
       A dictionary containing parsed bits.
     """
-    if 'js_user_agent_family' in jsParseBits and jsParseBits['js_user_agent_family'] != '':
-        family = jsParseBits['js_user_agent_family']
-        if 'js_user_agent_v1' in jsParseBits:
-            v1 = jsParseBits['js_user_agent_v1'] or None
-        if 'js_user_agent_v2' in jsParseBits:
-            v2 = jsParseBits['js_user_agent_v2'] or None
-        if 'js_user_agent_v3' in jsParseBits:
-            v3 = jsParseBits['js_user_agent_v3'] or None
+    if (
+        "js_user_agent_family" in jsParseBits
+        and jsParseBits["js_user_agent_family"] != ""
+    ):
+        family = jsParseBits["js_user_agent_family"]
+        v1 = jsParseBits.get("js_user_agent_v1") or None
+        v2 = jsParseBits.get("js_user_agent_v2") or None
+        v3 = jsParseBits.get("js_user_agent_v3") or None
     else:
         for uaParser in USER_AGENT_PARSERS:
             family, v1, v2, v3 = uaParser.Parse(user_agent_string)
             if family:
                 break
 
     # Override for Chrome Frame IFF Chrome is enabled.
-    if 'js_user_agent_string' in jsParseBits:
-        js_user_agent_string = jsParseBits['js_user_agent_string']
+    if "js_user_agent_string" in jsParseBits:
+        js_user_agent_string = jsParseBits["js_user_agent_string"]
         if (
-            js_user_agent_string and js_user_agent_string.find('Chrome/') > -1 and
-            user_agent_string.find('chromeframe') > -1
+            js_user_agent_string
+            and js_user_agent_string.find("Chrome/") > -1
+            and user_agent_string.find("chromeframe") > -1
         ):
             jsOverride = {}
             jsOverride = ParseUserAgent(js_user_agent_string)
-            family = 'Chrome Frame (%s %s)' % (family, v1)
-            v1 = jsOverride['major']
-            v2 = jsOverride['minor']
-            v3 = jsOverride['patch']
+            family = "Chrome Frame (%s %s)" % (family, v1)
+            v1 = jsOverride["major"]
+            v2 = jsOverride["minor"]
+            v3 = jsOverride["patch"]
 
-    family = family or 'Other'
+    family = family or "Other"
     return {
-        'family': family,
-        'major': v1,
-        'minor': v2,
-        'patch': v3
+        "family": family,
+        "major": v1 or None,
+        "minor": v2 or None,
+        "patch": v3 or None,
     }
 
 
 def ParseOS(user_agent_string, **jsParseBits):
     """ Parses the user-agent string for operating system info
     Args:
       user_agent_string: The full user-agent string.
@@ -284,21 +297,21 @@
     Returns:
       A dictionary containing parsed bits.
     """
     for osParser in OS_PARSERS:
         os, os_v1, os_v2, os_v3, os_v4 = osParser.Parse(user_agent_string)
         if os:
             break
-    os = os or 'Other'
+    os = os or "Other"
     return {
-        'family': os,
-        'major': os_v1,
-        'minor': os_v2,
-        'patch': os_v3,
-        'patch_minor': os_v4
+        "family": os,
+        "major": os_v1,
+        "minor": os_v2,
+        "patch": os_v3,
+        "patch_minor": os_v4,
     }
 
 
 def ParseDevice(user_agent_string):
     """ Parses the user-agent string for device info.
     Args:
         user_agent_string: The full user-agent string.
@@ -308,63 +321,61 @@
     """
     for deviceParser in DEVICE_PARSERS:
         device, brand, model = deviceParser.Parse(user_agent_string)
         if device:
             break
 
     if device is None:
-        device = 'Other'
+        device = "Other"
 
-    return {
-        'family': device,
-        'brand': brand,
-        'model': model
-    }
+    return {"family": device, "brand": brand, "model": model}
 
 
 def PrettyUserAgent(family, v1=None, v2=None, v3=None):
     """Pretty user agent string."""
     if v3:
         if v3[0].isdigit():
-            return '%s %s.%s.%s' % (family, v1, v2, v3)
+            return "%s %s.%s.%s" % (family, v1, v2, v3)
         else:
-            return '%s %s.%s%s' % (family, v1, v2, v3)
+            return "%s %s.%s%s" % (family, v1, v2, v3)
     elif v2:
-        return '%s %s.%s' % (family, v1, v2)
+        return "%s %s.%s" % (family, v1, v2)
     elif v1:
-        return '%s %s' % (family, v1)
+        return "%s %s" % (family, v1)
     return family
 
 
 def PrettyOS(os, os_v1=None, os_v2=None, os_v3=None, os_v4=None):
     """Pretty os string."""
     if os_v4:
-        return '%s %s.%s.%s.%s' % (os, os_v1, os_v2, os_v3, os_v4)
+        return "%s %s.%s.%s.%s" % (os, os_v1, os_v2, os_v3, os_v4)
     if os_v3:
         if os_v3[0].isdigit():
-            return '%s %s.%s.%s' % (os, os_v1, os_v2, os_v3)
+            return "%s %s.%s.%s" % (os, os_v1, os_v2, os_v3)
         else:
-            return '%s %s.%s%s' % (os, os_v1, os_v2, os_v3)
+            return "%s %s.%s%s" % (os, os_v1, os_v2, os_v3)
     elif os_v2:
-        return '%s %s.%s' % (os, os_v1, os_v2)
+        return "%s %s.%s" % (os, os_v1, os_v2)
     elif os_v1:
-        return '%s %s' % (os, os_v1)
+        return "%s %s" % (os, os_v1)
     return os
 
 
-def ParseWithJSOverrides(user_agent_string,
-                         js_user_agent_string=None,
-                         js_user_agent_family=None,
-                         js_user_agent_v1=None,
-                         js_user_agent_v2=None,
-                         js_user_agent_v3=None):
+def ParseWithJSOverrides(
+    user_agent_string,
+    js_user_agent_string=None,
+    js_user_agent_family=None,
+    js_user_agent_v1=None,
+    js_user_agent_v2=None,
+    js_user_agent_v3=None,
+):
     """ backwards compatible. use one of the other Parse methods instead! """
 
     # Override via JS properties.
-    if js_user_agent_family is not None and js_user_agent_family != '':
+    if js_user_agent_family is not None and js_user_agent_family != "":
         family = js_user_agent_family
         v1 = None
         v2 = None
         v3 = None
         if js_user_agent_v1 is not None:
             v1 = js_user_agent_v1
         if js_user_agent_v2 is not None:
@@ -375,45 +386,49 @@
         for parser in USER_AGENT_PARSERS:
             family, v1, v2, v3 = parser.Parse(user_agent_string)
             if family:
                 break
 
     # Override for Chrome Frame IFF Chrome is enabled.
     if (
-        js_user_agent_string and js_user_agent_string.find('Chrome/') > -1 and
-        user_agent_string.find('chromeframe') > -1
+        js_user_agent_string
+        and js_user_agent_string.find("Chrome/") > -1
+        and user_agent_string.find("chromeframe") > -1
     ):
-        family = 'Chrome Frame (%s %s)' % (family, v1)
+        family = "Chrome Frame (%s %s)" % (family, v1)
         ua_dict = ParseUserAgent(js_user_agent_string)
-        v1 = ua_dict['major']
-        v2 = ua_dict['minor']
-        v3 = ua_dict['patch']
+        v1 = ua_dict["major"]
+        v2 = ua_dict["minor"]
+        v3 = ua_dict["patch"]
 
-    return family or 'Other', v1, v2, v3
+    return family or "Other", v1, v2, v3
 
 
 def Pretty(family, v1=None, v2=None, v3=None):
     """ backwards compatible. use PrettyUserAgent instead! """
     if v3:
         if v3[0].isdigit():
-            return '%s %s.%s.%s' % (family, v1, v2, v3)
+            return "%s %s.%s.%s" % (family, v1, v2, v3)
         else:
-            return '%s %s.%s%s' % (family, v1, v2, v3)
+            return "%s %s.%s%s" % (family, v1, v2, v3)
     elif v2:
-        return '%s %s.%s' % (family, v1, v2)
+        return "%s %s.%s" % (family, v1, v2)
     elif v1:
-        return '%s %s' % (family, v1)
+        return "%s %s" % (family, v1)
     return family
 
 
-def GetFilters(user_agent_string, js_user_agent_string=None,
-               js_user_agent_family=None,
-               js_user_agent_v1=None,
-               js_user_agent_v2=None,
-               js_user_agent_v3=None):
+def GetFilters(
+    user_agent_string,
+    js_user_agent_string=None,
+    js_user_agent_family=None,
+    js_user_agent_v1=None,
+    js_user_agent_v2=None,
+    js_user_agent_v3=None,
+):
     """Return the optional arguments that should be saved and used to query.
 
     js_user_agent_string is always returned if it is present. We really only need
     it for Chrome Frame. However, I added it in the generally case to find other
     cases when it is different. When the recording of js_user_agent_string was
     added, we created new records for all new user agents.
 
@@ -433,118 +448,95 @@
       js_user_agent_v2: v1 override - see above.
       js_user_agent_v3: v1 override - see above.
     Returns:
       {js_user_agent_string: '[...]', js_family_name: '[...]', etc...}
     """
     filters = {}
     filterdict = {
-        'js_user_agent_string': js_user_agent_string,
-        'js_user_agent_family': js_user_agent_family,
-        'js_user_agent_v1': js_user_agent_v1,
-        'js_user_agent_v2': js_user_agent_v2,
-        'js_user_agent_v3': js_user_agent_v3
+        "js_user_agent_string": js_user_agent_string,
+        "js_user_agent_family": js_user_agent_family,
+        "js_user_agent_v1": js_user_agent_v1,
+        "js_user_agent_v2": js_user_agent_v2,
+        "js_user_agent_v3": js_user_agent_v3,
     }
     for key, value in filterdict.items():
-        if value is not None and value != '':
+        if value is not None and value != "":
             filters[key] = value
     return filters
 
 
 # Build the list of user agent parsers from YAML
 UA_PARSER_YAML = os.environ.get("UA_PARSER_YAML")
 if UA_PARSER_YAML:
     # This will raise an ImportError if missing, obviously since it's no
     # longer a requirement
     import yaml
+
     try:
         # Try and use libyaml bindings if available since faster
         from yaml import CSafeLoader as SafeLoader
     except ImportError:
         from yaml import SafeLoader
 
     with open(UA_PARSER_YAML) as fp:
         regexes = yaml.load(fp, Loader=SafeLoader)
 
     USER_AGENT_PARSERS = []
-    for _ua_parser in regexes['user_agent_parsers']:
-        _regex = _ua_parser['regex']
+    for _ua_parser in regexes["user_agent_parsers"]:
+        _regex = _ua_parser["regex"]
 
-        _family_replacement = None
-        if 'family_replacement' in _ua_parser:
-            _family_replacement = _ua_parser['family_replacement']
-
-        _v1_replacement = None
-        if 'v1_replacement' in _ua_parser:
-            _v1_replacement = _ua_parser['v1_replacement']
-
-        _v2_replacement = None
-        if 'v2_replacement' in _ua_parser:
-            _v2_replacement = _ua_parser['v2_replacement']
-
-        USER_AGENT_PARSERS.append(UserAgentParser(_regex,
-                                                  _family_replacement,
-                                                  _v1_replacement,
-                                                  _v2_replacement))
+        _family_replacement = _ua_parser.get("family_replacement")
+        _v1_replacement = _ua_parser.get("v1_replacement")
+        _v2_replacement = _ua_parser.get("v2_replacement")
+
+        USER_AGENT_PARSERS.append(
+            UserAgentParser(
+                _regex, _family_replacement, _v1_replacement, _v2_replacement
+            )
+        )
 
     OS_PARSERS = []
-    for _os_parser in regexes['os_parsers']:
-        _regex = _os_parser['regex']
+    for _os_parser in regexes["os_parsers"]:
+        _regex = _os_parser["regex"]
 
-        _os_replacement = None
-        if 'os_replacement' in _os_parser:
-            _os_replacement = _os_parser['os_replacement']
-
-        _os_v1_replacement = None
-        if 'os_v1_replacement' in _os_parser:
-            _os_v1_replacement = _os_parser['os_v1_replacement']
-
-        _os_v2_replacement = None
-        if 'os_v2_replacement' in _os_parser:
-            _os_v2_replacement = _os_parser['os_v2_replacement']
-
-        _os_v3_replacement = None
-        if 'os_v3_replacement' in _os_parser:
-            _os_v3_replacement = _os_parser['os_v3_replacement']
-
-        _os_v4_replacement = None
-        if 'os_v4_replacement' in _os_parser:
-            _os_v4_replacement = _os_parser['os_v4_replacement']
-
-        OS_PARSERS.append(OSParser(_regex,
-                                   _os_replacement,
-                                   _os_v1_replacement,
-                                   _os_v2_replacement,
-                                   _os_v3_replacement,
-                                   _os_v4_replacement))
+        _os_replacement = _os_parser.get("os_replacement")
+        _os_v1_replacement = _os_parser.get("os_v1_replacement")
+        _os_v2_replacement = _os_parser.get("os_v2_replacement")
+        _os_v3_replacement = _os_parser.get("os_v3_replacement")
+        _os_v4_replacement = _os_parser.get("os_v4_replacement")
+
+        OS_PARSERS.append(
+            OSParser(
+                _regex,
+                _os_replacement,
+                _os_v1_replacement,
+                _os_v2_replacement,
+                _os_v3_replacement,
+                _os_v4_replacement,
+            )
+        )
 
     DEVICE_PARSERS = []
-    for _device_parser in regexes['device_parsers']:
-        _regex = _device_parser['regex']
+    for _device_parser in regexes["device_parsers"]:
+        _regex = _device_parser["regex"]
 
-        _regex_flag = None
-        if 'regex_flag' in _device_parser:
-            _regex_flag = _device_parser['regex_flag']
-
-        _device_replacement = None
-        if 'device_replacement' in _device_parser:
-            _device_replacement = _device_parser['device_replacement']
-
-        _brand_replacement = None
-        if 'brand_replacement' in _device_parser:
-            _brand_replacement = _device_parser['brand_replacement']
-
-        _model_replacement = None
-        if 'model_replacement' in _device_parser:
-            _model_replacement = _device_parser['model_replacement']
-
-        DEVICE_PARSERS.append(DeviceParser(_regex,
-                                           _regex_flag,
-                                           _device_replacement,
-                                           _brand_replacement,
-                                           _model_replacement))
+        _regex_flag = _device_parser.get("regex_flag")
+        _device_replacement = _device_parser.get("device_replacement")
+        _brand_replacement = _device_parser.get("brand_replacement")
+        _model_replacement = _device_parser.get("model_replacement")
+
+        DEVICE_PARSERS.append(
+            DeviceParser(
+                _regex,
+                _regex_flag,
+                _device_replacement,
+                _brand_replacement,
+                _model_replacement,
+            )
+        )
 
     # Clean our our temporary vars explicitly
     # so they can't be reused or imported
     del regexes
     del yaml
     del SafeLoader
 else:
```

### Comparing `ua-parser-0.8.0/README.rst` & `ua-parser-0.9.0/README.rst`

 * *Files identical despite different names*

