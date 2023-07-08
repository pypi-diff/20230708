# Comparing `tmp/cshogi-0.5.5.tar.gz` & `tmp/cshogi-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshogi-0.5.5.tar", last modified: Sun May  7 09:09:05 2023, max compression
+gzip compressed data, was "cshogi-0.5.6.tar", last modified: Sat Jul  8 03:26:47 2023, max compression
```

## Comparing `cshogi-0.5.5.tar` & `cshogi-0.5.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.030838 cshogi-0.5.5/
--rw-rw-rw-   0        0        0    35823 2023-05-07 09:08:23.000000 cshogi-0.5.5/LICENSE
--rw-rw-rw-   0        0        0      358 2023-05-07 09:09:05.030838 cshogi-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     5135 2023-05-07 09:08:23.000000 cshogi-0.5.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/
--rw-rw-rw-   0        0        0     2774 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/CSA.py
--rw-rw-rw-   0        0        0    18556 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/KI2.py
--rw-rw-rw-   0        0        0    17360 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/KIF.py
--rw-rw-rw-   0        0        0     2988 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/PGN.py
--rw-rw-rw-   0        0        0       27 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/__init__.py
--rw-rw-rw-   0        0        0    28993 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/_cshogi.pyx
--rw-rw-rw-   0        0        0    25971 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/dlshogi/
--rw-rw-rw-   0        0        0      327 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/dlshogi/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/elo.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/gym_shogi/
--rw-rw-rw-   0        0        0      132 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/gym_shogi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/gym_shogi/envs/
--rw-rw-rw-   0        0        0      118 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/gym_shogi/envs/__init__.py
--rw-rw-rw-   0        0        0     2259 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/gym_shogi/envs/shogi_env.pyx
--rw-rw-rw-   0        0        0      755 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/gym_shogi/envs/shogi_vec_env.pyx
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/usi/
--rw-rw-rw-   0        0        0     6725 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/usi/Engine.py
--rw-rw-rw-   0        0        0       26 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/usi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/web/
--rw-rw-rw-   0        0        0    13662 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/web/app.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/web/static/
--rw-rw-rw-   0        0        0    13931 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/web/static/board.js
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi/web/templates/
--rw-rw-rw-   0        0        0    17362 2023-05-07 09:08:23.000000 cshogi-0.5.5/cshogi/web/templates/board.html
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.015257 cshogi-0.5.5/cshogi.egg-info/
--rw-rw-rw-   0        0        0      358 2023-05-07 09:09:04.000000 cshogi-0.5.5/cshogi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2023-05-07 09:09:04.000000 cshogi-0.5.5/cshogi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 09:09:04.000000 cshogi-0.5.5/cshogi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 09:09:04.000000 cshogi-0.5.5/cshogi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 09:09:05.030838 cshogi-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0     2006 2023-05-07 09:08:23.000000 cshogi-0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.030838 cshogi-0.5.5/src/
--rw-rw-rw-   0        0        0     8208 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/bitboard.cpp
--rw-rw-rw-   0        0        0     2225 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/book.cpp
--rw-rw-rw-   0        0        0     1350 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/common.cpp
--rw-rw-rw-   0        0        0    28484 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/dfpn.cpp
--rw-rw-rw-   0        0        0    50568 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/generateMoves.cpp
--rw-rw-rw-   0        0        0     1789 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/hand.cpp
--rw-rw-rw-   0        0        0    19051 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/init.cpp
--rw-rw-rw-   0        0        0     6937 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/mate.cpp
--rw-rw-rw-   0        0        0     2163 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/move.cpp
--rw-rw-rw-   0        0        0     1172 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/mt64bit.cpp
--rw-rw-rw-   0        0        0   174059 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/position.cpp
--rw-rw-rw-   0        0        0     3308 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/search.cpp
--rw-rw-rw-   0        0        0     1416 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/square.cpp
--rw-rw-rw-   0        0        0     6627 2023-05-07 09:08:23.000000 cshogi-0.5.5/src/usi.cpp
-drwxrwxrwx   0        0        0        0 2023-05-07 09:09:05.030838 cshogi-0.5.5/test/
--rw-rw-rw-   0        0        0      824 2023-05-07 09:08:23.000000 cshogi-0.5.5/test/test_usi_engine.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.229791 cshogi-0.5.6/
+-rw-rw-rw-   0        0        0    35823 2023-07-08 03:26:06.000000 cshogi-0.5.6/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-07-08 03:26:47.229791 cshogi-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5135 2023-07-08 03:26:06.000000 cshogi-0.5.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/
+-rw-rw-rw-   0        0        0     2774 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/CSA.py
+-rw-rw-rw-   0        0        0    18556 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/KI2.py
+-rw-rw-rw-   0        0        0    17360 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/KIF.py
+-rw-rw-rw-   0        0        0     2988 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/PGN.py
+-rw-rw-rw-   0        0        0       27 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/__init__.py
+-rw-rw-rw-   0        0        0    29185 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/_cshogi.pyx
+-rw-rw-rw-   0        0        0    25971 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/dlshogi/
+-rw-rw-rw-   0        0        0      327 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/dlshogi/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/elo.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/gym_shogi/
+-rw-rw-rw-   0        0        0      132 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/gym_shogi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/gym_shogi/envs/
+-rw-rw-rw-   0        0        0      118 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/gym_shogi/envs/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/gym_shogi/envs/shogi_env.pyx
+-rw-rw-rw-   0        0        0      755 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/gym_shogi/envs/shogi_vec_env.pyx
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/usi/
+-rw-rw-rw-   0        0        0     6725 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/usi/Engine.py
+-rw-rw-rw-   0        0        0       26 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/usi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/web/
+-rw-rw-rw-   0        0        0    13662 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/web/app.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/web/static/
+-rw-rw-rw-   0        0        0    13931 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/web/static/board.js
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/web/templates/
+-rw-rw-rw-   0        0        0    17362 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/web/templates/board.html
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-07-08 03:26:47.000000 cshogi-0.5.6/cshogi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-07-08 03:26:47.000000 cshogi-0.5.6/cshogi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 03:26:47.000000 cshogi-0.5.6/cshogi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 03:26:47.000000 cshogi-0.5.6/cshogi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 03:26:47.229791 cshogi-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     2040 2023-07-08 03:26:06.000000 cshogi-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.229791 cshogi-0.5.6/src/
+-rw-rw-rw-   0        0        0     8208 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/bitboard.cpp
+-rw-rw-rw-   0        0        0     3267 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/book.cpp
+-rw-rw-rw-   0        0        0     1350 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/common.cpp
+-rw-rw-rw-   0        0        0    28484 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/dfpn.cpp
+-rw-rw-rw-   0        0        0    50568 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/generateMoves.cpp
+-rw-rw-rw-   0        0        0     1789 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/hand.cpp
+-rw-rw-rw-   0        0        0    19051 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/init.cpp
+-rw-rw-rw-   0        0        0     6937 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/mate.cpp
+-rw-rw-rw-   0        0        0     2163 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/move.cpp
+-rw-rw-rw-   0        0        0     1172 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/mt64bit.cpp
+-rw-rw-rw-   0        0        0   174059 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/position.cpp
+-rw-rw-rw-   0        0        0     3308 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/search.cpp
+-rw-rw-rw-   0        0        0     1416 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/square.cpp
+-rw-rw-rw-   0        0        0     6627 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/usi.cpp
+drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.229791 cshogi-0.5.6/test/
+-rw-rw-rw-   0        0        0      824 2023-07-08 03:26:06.000000 cshogi-0.5.6/test/test_usi_engine.py
```

### Comparing `cshogi-0.5.5/LICENSE` & `cshogi-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/README.rst` & `cshogi-0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/CSA.py` & `cshogi-0.5.6/cshogi/CSA.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/KI2.py` & `cshogi-0.5.6/cshogi/KI2.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/KIF.py` & `cshogi-0.5.6/cshogi/KIF.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/PGN.py` & `cshogi-0.5.6/cshogi/PGN.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/_cshogi.pyx` & `cshogi-0.5.6/cshogi/_cshogi.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -276,14 +276,15 @@
 		void piece_planes(char* mem)
 		void piece_planes_rotate(char* mem)
 		void _dlshogi_make_input_features(char* mem1, char* mem2)
 		void push_pass()
 		void pop_pass()
 		bool isOK()
 		unsigned long long bookKey()
+		unsigned long long bookKeyAfter(const unsigned long long key, const int move)
 
 	int __piece_to_piece_type(const int p)
 	int __hand_piece_to_piece_type(const int hp)
 
 cdef class Board:
 	cdef __Board __board
 
@@ -499,14 +500,17 @@
 
 	def is_ok(self):
 		return self.__board.isOK()
 
 	def book_key(self):
 		return self.__board.bookKey()
 
+	def book_key_after(self, unsigned long long key, int move):
+		return self.__board.bookKeyAfter(key, move)
+
 	def to_svg(self, lastmove=None, scale=1.0):
 		import xml.etree.ElementTree as ET
 
 		width = 230
 		height = 192
 
 		svg = ET.Element("svg", {
```

### Comparing `cshogi-0.5.5/cshogi/cli.py` & `cshogi-0.5.6/cshogi/cli.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/elo.py` & `cshogi-0.5.6/cshogi/elo.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/gym_shogi/envs/shogi_env.pyx` & `cshogi-0.5.6/cshogi/gym_shogi/envs/shogi_env.pyx`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/gym_shogi/envs/shogi_vec_env.pyx` & `cshogi-0.5.6/cshogi/gym_shogi/envs/shogi_vec_env.pyx`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/usi/Engine.py` & `cshogi-0.5.6/cshogi/usi/Engine.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/web/app.py` & `cshogi-0.5.6/cshogi/web/app.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/web/static/board.js` & `cshogi-0.5.6/cshogi/web/static/board.js`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi/web/templates/board.html` & `cshogi-0.5.6/cshogi/web/templates/board.html`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/cshogi.egg-info/SOURCES.txt` & `cshogi-0.5.6/cshogi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/setup.py` & `cshogi-0.5.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ﻿from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 
 class my_build_ext(build_ext):
     def build_extensions(self):
         if self.compiler.compiler_type == 'unix':
             for e in self.extensions:
-                e.extra_compile_args = ['-msse4.2', '-mavx2']
+                e.extra_compile_args = ['-msse4.2', '-mavx2', '-Wno-enum-constexpr-conversion']
 
         build_ext.build_extensions(self)
 
     def finalize_options(self):
         build_ext.finalize_options(self)
         __builtins__.__NUMPY_SETUP__ = False
         import numpy
@@ -28,15 +28,15 @@
     Extension('cshogi.gym_shogi.envs.shogi_vec_env',
         ['cshogi/gym_shogi/envs/shogi_vec_env.pyx'],
         language='c++'),
 ]
 
 setup(
     name='cshogi',
-    version='0.5.5',
+    version='0.5.6',
     packages=['cshogi', 'cshogi.usi', 'cshogi.gym_shogi', 'cshogi.gym_shogi.envs', 'cshogi.dlshogi', 'cshogi.web', 'cshogi.web.templates', 'cshogi.web.static'],
     package_data={'cshogi.web.templates': ['*'], 'cshogi.web.static': ['*']},
     ext_modules=ext_modules,
     cmdclass={'build_ext': my_build_ext},
     author='Tadao Yamaoka',
     url='https://github.com/TadaoYamaoka/cshogi',
     description = 'A fast Python shogi library',
```

### Comparing `cshogi-0.5.5/src/bitboard.cpp` & `cshogi-0.5.6/src/bitboard.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/book.cpp` & `cshogi-0.5.6/src/book.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
   You should have received a copy of the GNU General Public License
   along with this program.  If not, see <http://www.gnu.org/licenses/>.
 */
 
 #include "book.hpp"
 #include "position.hpp"
+#include "move.hpp"
 
 MT64bit Book::mt64bit_; // 定跡のhash生成用なので、seedは固定でデフォルト値を使う。
 Key Book::ZobPiece[PieceNone][SquareNum];
 Key Book::ZobHand[HandPieceNum][19]; // 持ち駒の同一種類の駒の数ごと
 Key Book::ZobTurn;
 
 void Book::init() {
@@ -51,10 +52,38 @@
     for (HandPiece hp = HPawn; hp < HandPieceNum; ++hp)
         key ^= ZobHand[hp][hand.numOf(hp)];
     if (pos.turn() == White)
         key ^= ZobTurn;
     return key;
 }
 
+Key Book::bookKeyAfter(const Position& pos, const Key key, const Move move) {
+    Key key_after = key;
+    const Square to = move.to();
+    if (move.isDrop()) {
+        const Piece pc = colorAndPieceTypeToPiece(pos.turn(), move.pieceTypeDropped());
+        key_after ^= ZobPiece[pc][to];
+    }
+    else {
+        const Square from = move.from();
+        key_after ^= ZobPiece[pos.piece(from)][from];
+
+        const Piece pc = colorAndPieceTypeToPiece(pos.turn(), move.pieceTypeTo());
+        key_after ^= ZobPiece[pc][to];
+
+        if (move.isCapture())
+            key_after ^= ZobPiece[pos.piece(to)][to];
+    }
+    const Hand hand = pos.hand(pos.turn());
+    for (HandPiece hp = HPawn; hp < HandPieceNum; ++hp)
+        key_after ^= ZobHand[hp][hand.numOf(hp)];
+    const Hand hand_after = pos.hand(oppositeColor(pos.turn()));
+    for (HandPiece hp = HPawn; hp < HandPieceNum; ++hp)
+        key_after ^= ZobHand[hp][hand_after.numOf(hp)];
+
+    key_after ^= ZobTurn;
+    return key_after;
+}
+
 inline bool countCompare(const BookEntry& b1, const BookEntry& b2) {
     return b1.count < b2.count;
 }
```

### Comparing `cshogi-0.5.5/src/common.cpp` & `cshogi-0.5.6/src/common.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/dfpn.cpp` & `cshogi-0.5.6/src/dfpn.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/generateMoves.cpp` & `cshogi-0.5.6/src/generateMoves.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/hand.cpp` & `cshogi-0.5.6/src/hand.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/init.cpp` & `cshogi-0.5.6/src/init.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/mate.cpp` & `cshogi-0.5.6/src/mate.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/move.cpp` & `cshogi-0.5.6/src/move.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/mt64bit.cpp` & `cshogi-0.5.6/src/mt64bit.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/position.cpp` & `cshogi-0.5.6/src/position.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/search.cpp` & `cshogi-0.5.6/src/search.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/square.cpp` & `cshogi-0.5.6/src/square.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/src/usi.cpp` & `cshogi-0.5.6/src/usi.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.5/test/test_usi_engine.py` & `cshogi-0.5.6/test/test_usi_engine.py`

 * *Files identical despite different names*

