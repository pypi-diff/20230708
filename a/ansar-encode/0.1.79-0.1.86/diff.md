# Comparing `tmp/ansar-encode-0.1.79.tar.gz` & `tmp/ansar-encode-0.1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-encode-0.1.79.tar", last modified: Sun Jun 18 03:36:28 2023, max compression
+gzip compressed data, was "ansar-encode-0.1.86.tar", last modified: Sat Jul  8 04:01:22 2023, max compression
```

## Comparing `ansar-encode-0.1.79.tar` & `ansar-encode-0.1.86.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:14.000000 ansar-encode-0.1.79/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)     1484 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.79/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      311 2023-06-18 03:22:42.000000 ansar-encode-0.1.79/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     1983 2023-06-18 03:18:21.000000 ansar-encode-0.1.79/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.778816 ansar-encode-0.1.79/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.778816 ansar-encode-0.1.79/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    12110 2023-06-18 03:18:22.000000 ansar-encode-0.1.79/src/ansar/command/show_release.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/src/ansar/encode/
--rw-rw-r--   0 scott     (1000) scott     (1000)     4961 2023-06-18 03:36:25.000000 ansar-encode-0.1.79/src/ansar/encode/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37157 2023-06-18 03:22:16.000000 ansar-encode-0.1.79/src/ansar/encode/codec.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    16861 2023-06-18 03:22:16.000000 ansar-encode-0.1.79/src/ansar/encode/convert.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11277 2023-06-18 03:20:47.000000 ansar-encode-0.1.79/src/ansar/encode/file.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19686 2023-06-18 03:20:48.000000 ansar-encode-0.1.79/src/ansar/encode/folder.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3737 2023-06-18 03:22:17.000000 ansar-encode-0.1.79/src/ansar/encode/json.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33784 2023-06-18 03:22:17.000000 ansar-encode-0.1.79/src/ansar/encode/message.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10974 2023-06-18 03:22:17.000000 ansar-encode-0.1.79/src/ansar/encode/portable.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3340 2023-06-18 03:20:51.000000 ansar-encode-0.1.79/src/ansar/encode/release.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6353 2023-06-18 03:22:18.000000 ansar-encode-0.1.79/src/ansar/encode/runtime.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1820 2023-06-18 03:20:53.000000 ansar-encode-0.1.79/src/ansar/encode/version.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11523 2023-06-18 03:20:54.000000 ansar-encode-0.1.79/src/ansar/encode/xml.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/src/ansar_encode.egg-info/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1484 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-07-08 04:01:22.973003 ansar-encode-0.1.86/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:14.000000 ansar-encode-0.1.86/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1495 2023-07-08 04:01:22.973003 ansar-encode-0.1.86/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.86/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      752 2023-07-08 04:00:20.000000 ansar-encode-0.1.86/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-07-08 04:01:22.973003 ansar-encode-0.1.86/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1996 2023-07-08 03:51:47.000000 ansar-encode-0.1.86/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-07-08 04:01:22.969003 ansar-encode-0.1.86/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-07-08 04:01:22.969003 ansar-encode-0.1.86/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-07-08 04:01:22.969003 ansar-encode-0.1.86/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12110 2023-06-18 03:18:22.000000 ansar-encode-0.1.86/src/ansar/command/show_release.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-07-08 04:01:22.969003 ansar-encode-0.1.86/src/ansar/encode/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4961 2023-07-08 04:01:19.000000 ansar-encode-0.1.86/src/ansar/encode/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37288 2023-06-25 04:23:20.000000 ansar-encode-0.1.86/src/ansar/encode/codec.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    16861 2023-06-18 03:22:16.000000 ansar-encode-0.1.86/src/ansar/encode/convert.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11277 2023-06-18 03:20:47.000000 ansar-encode-0.1.86/src/ansar/encode/file.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19686 2023-06-18 03:20:48.000000 ansar-encode-0.1.86/src/ansar/encode/folder.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3737 2023-06-18 03:22:17.000000 ansar-encode-0.1.86/src/ansar/encode/json.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33784 2023-06-18 03:22:17.000000 ansar-encode-0.1.86/src/ansar/encode/message.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10974 2023-06-18 03:22:17.000000 ansar-encode-0.1.86/src/ansar/encode/portable.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3340 2023-06-18 03:20:51.000000 ansar-encode-0.1.86/src/ansar/encode/release.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6353 2023-06-18 03:22:18.000000 ansar-encode-0.1.86/src/ansar/encode/runtime.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1820 2023-06-18 03:20:53.000000 ansar-encode-0.1.86/src/ansar/encode/version.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11523 2023-06-18 03:20:54.000000 ansar-encode-0.1.86/src/ansar/encode/xml.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-07-08 04:01:22.969003 ansar-encode-0.1.86/src/ansar_encode.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1495 2023-07-08 04:01:22.000000 ansar-encode-0.1.86/src/ansar_encode.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-07-08 04:01:22.000000 ansar-encode-0.1.86/src/ansar_encode.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-07-08 04:01:22.000000 ansar-encode-0.1.86/src/ansar_encode.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-07-08 04:01:22.000000 ansar-encode-0.1.86/src/ansar_encode.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-07-08 04:01:22.000000 ansar-encode-0.1.86/src/ansar_encode.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-07-08 04:01:22.000000 ansar-encode-0.1.86/src/ansar_encode.egg-info/top_level.txt
```

### Comparing `ansar-encode-0.1.79/LICENSE` & `ansar-encode-0.1.86/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/PKG-INFO` & `ansar-encode-0.1.86/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.79
+Version: 0.1.86
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
-Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
+Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
```

### Comparing `ansar-encode-0.1.79/README.md` & `ansar-encode-0.1.86/README.md`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/setup.py` & `ansar-encode-0.1.86/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,39 +34,39 @@
 with open("README.md", "r", encoding="utf-8") as f:
 	long_description = f.read()
 
 with open("DOC_LATEST_LINK", "r", encoding="utf-8") as f:
 	d = f.read()
 DOC_LINK = d[:-1]
 
-REQUIRES = [
-	"defusedxml>=0.7.1",
-	"python-dateutil>=2.8.1",
-]
+#REQUIRES = [
+#	"defusedxml>=0.7.1",
+#	"python-dateutil>=2.8.1",
+#]
 
 setuptools.setup(
 	name=PACKAGE,
 	version=VERSION,
 	author="Scott Woods",
 	author_email="scott.18.ansar@gmail.com.com",
 	description=DESCRIPTION,
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	# url="https://gitlab.com/scott.ansar/ansar-encode",
 	project_urls={
 		"Documentation": DOC_LINK,
 	},
-	classifiers=[
-		"Development Status :: 4 - Beta",
-		"Intended Audience :: Developers",
-		"Programming Language :: Python :: 3",
-		"License :: OSI Approved :: MIT License",
-		"Operating System :: OS Independent",
-		"Topic :: Software Development :: Libraries",
-	],
+	#classifiers=[
+	#	"Development Status :: 4 - Beta",
+	#	"Intended Audience :: Developers",
+	#	"Programming Language :: Python :: 3",
+	#	"License :: OSI Approved :: MIT License",
+	#	"Operating System :: OS Independent",
+	#	"Topic :: Software Development :: Libraries",
+	#],
 	# Where multiple packages might be found, esp if using standard
 	# layout for "find_packages".
 	package_dir={
 		"": "src",
 	},
 	# First folder under "where" defines the name of the
 	# namespace. Folders under that (with __init__.py files)
@@ -76,9 +76,9 @@
 	),
 	entry_points = {
 		'console_scripts': [
 			'ansar-releasing=ansar.command.show_release:main',
 		],
 	},
 	python_requires=">=3.6",
-	install_requires=REQUIRES,
+	#install_requires=REQUIRES,
 )
```

### Comparing `ansar-encode-0.1.79/src/ansar/command/show_release.py` & `ansar-encode-0.1.86/src/ansar/command/show_release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar/encode/__init__.py` & `ansar-encode-0.1.86/src/ansar/encode/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Persistence of complex application data.
 
 Repo: git@github.com:mr-ansar/ansar-encode.git
 Branch: main
-Commit: df86792c81859d23fa9c0345405b3806544ee3ec
-Version: 0.1.78 (2023-06-18@15:36:25+NZST)
+Commit: cd7d8e3a345006ecd23bab230ce48c2ffac43907
+Version: 0.1.85 (2023-07-08@16:01:19+NZST)
 """
 
 from .portable import Boolean
 from .portable import Byte, Character, Rune
 from .portable import Integer2, Integer4, Integer8
 from .portable import Unsigned2, Unsigned4, Unsigned8
 from .portable import Float4, Float8
```

### Comparing `ansar-encode-0.1.79/src/ansar/encode/codec.py` & `ansar-encode-0.1.86/src/ansar/encode/codec.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,16 +333,16 @@
     return w
 
 def p2w_target(c, p, t):
     # TODO
     # Perhaps the JSON encoder passes this
     # through as a list anyway. No need for
     # transform?
-    w = list(p)
-    return w
+    #w = list(p)
+    return p
 
 def p2w_address(c, p, t):
     # Check to see if an address is being
     # passed back over the connection it
     # arrived on. Prevents trombone behaviour.
     # Detection happens *here* at the remote
     # end of the trombone because this codec
@@ -350,18 +350,20 @@
     # where it came from. Add the invalid point
     # id. See w2p_address.
     if c.return_proxy is not None:
         a = c.return_proxy
         if p[-1] == a:
             # Need to advise remote that address
             # is returning to where it came from.
-            w = list(p[:-1])    # DROP THIS PROXY
+            #w = list(p[:-1])    # DROP THIS PROXY
+            w = p[:-1]          # DROP THIS PROXY
             w.append(0)         # SPECIAL MARK
             return w
-    w = list(p)
+    #w = list(p)
+    w = p
     return w
 
 def p2w_any(c, p, t):
     a = p.__class__
     if a == Incognito:          # Created during a previous decoding operation.
         t = p.type_name         # Global identifier
         w = p.decoded_word      # Generic body
@@ -408,16 +410,16 @@
     (uuid.UUID, UUID): p2w_uuid,
     (list, ArrayOf): p2w_array,
     (list, VectorOf): p2w_vector,
     (set, SetOf): p2w_set,
     (dict, MapOf): p2w_map,
     (deque, DequeOf): p2w_deque,
     (TypeType, Type): p2w_type,
-    (tuple, TargetAddress): p2w_target,
-    (tuple, Address): p2w_address,
+    (list, TargetAddress): p2w_target,
+    (list, Address): p2w_address,
 
     # PointerTo - can be any of the above.
     (bool, PointerTo): p2w_pointer,
     (int, PointerTo): p2w_pointer,
     (float, PointerTo): p2w_pointer,
     (bytearray, PointerTo): p2w_pointer,
     (bytes, PointerTo): p2w_pointer,
@@ -732,34 +734,37 @@
         except CircularReference:
             p.append(None)
             c.patch_work.append([d, patch])
     return p
 
 def w2p_target(c, w, t):
     if c.local_termination is None:
-        p = tuple(w)
+        #p = tuple(w)
+        p = w
     elif len(w) < 2:
         p = c.local_termination,
     else:
-        p = tuple(w[:-1])
+        #p = tuple(w[:-1])
+        p = w[:-1]
     return p
 
 def w2p_address(c, w, t):
     if c.return_proxy is not None:
         # Clean out any trombone detected
         # in the remote. See p2w_address.
         a = w[-1]
         if a == 0:      # SPECIAL MARK
             # Address has returned home
             # No need to append a trip back
             # over this connection.
             w.pop()
         else:
             w.append(c.return_proxy)
-    p = tuple(w)                 # Now convert.
+    #p = tuple(w)                 # Now convert.
+    p = w                 # Now convert.
     return p
 
 def w2p_null_pointer(c, w, t):
     return [0, None]
 
 # Covert inbound 2-word tuple into the original
 # object
@@ -944,23 +949,23 @@
         :type decorate_names: bool
         """
         self.extension = extension
         self.w2t = w2t
         self.t2w = t2w
 
         if return_proxy is None:
-            self.return_proxy = 0,  # Tuple
-        elif not isinstance(return_proxy, tuple) or len(return_proxy) != 1:
+            self.return_proxy = 0
+        elif not isinstance(return_proxy, (tuple, list)) or len(return_proxy) != 1:
             raise CodecUsage('unusable address passed as return proxy')
         else:
             self.return_proxy = return_proxy[0]
 
         if local_termination is None:
-            self.local_termination = 0,     # Tuple
-        elif not isinstance(local_termination, tuple) or len(local_termination) != 1:
+            self.local_termination = 0
+        elif not isinstance(local_termination, (tuple, list)) or len(local_termination) != 1:
             raise CodecUsage('unusable address passed as local termination')
         else:
             self.local_termination = local_termination[0]
 
         self.pretty_format = pretty_format
         self.decorate_names = decorate_names
```

### Comparing `ansar-encode-0.1.79/src/ansar/encode/convert.py` & `ansar-encode-0.1.86/src/ansar/encode/convert.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar/encode/file.py` & `ansar-encode-0.1.86/src/ansar/encode/file.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar/encode/folder.py` & `ansar-encode-0.1.86/src/ansar/encode/folder.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar/encode/json.py` & `ansar-encode-0.1.86/src/ansar/encode/json.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar/encode/message.py` & `ansar-encode-0.1.86/src/ansar/encode/message.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar/encode/portable.py` & `ansar-encode-0.1.86/src/ansar/encode/portable.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar/encode/release.py` & `ansar-encode-0.1.86/src/ansar/encode/release.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar/encode/runtime.py` & `ansar-encode-0.1.86/src/ansar/encode/runtime.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar/encode/version.py` & `ansar-encode-0.1.86/src/ansar/encode/version.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar/encode/xml.py` & `ansar-encode-0.1.86/src/ansar/encode/xml.py`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.79/src/ansar_encode.egg-info/PKG-INFO` & `ansar-encode-0.1.86/src/ansar_encode.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.79
+Version: 0.1.86
 Summary: Persistence of complex application data
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
-Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
+Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
```

### Comparing `ansar-encode-0.1.79/src/ansar_encode.egg-info/SOURCES.txt` & `ansar-encode-0.1.86/src/ansar_encode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

