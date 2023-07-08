# Comparing `tmp/streamlit_carousel-0.0.2.tar.gz` & `tmp/streamlit_carousel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_carousel-0.0.2.tar", last modified: Sat Jul  8 16:46:06 2023, max compression
+gzip compressed data, was "streamlit_carousel-0.0.3.tar", last modified: Sat Jul  8 16:55:15 2023, max compression
```

## Comparing `streamlit_carousel-0.0.2.tar` & `streamlit_carousel-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.291706 streamlit_carousel-0.0.2/
--rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_carousel-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       53 2023-07-08 16:44:00.000000 streamlit_carousel-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4918 2023-07-08 16:46:06.291706 streamlit_carousel-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2997 2023-07-08 16:34:50.000000 streamlit_carousel-0.0.2/README.md
--rw-rw-rw-   0        0        0      907 2023-07-08 16:36:00.000000 streamlit_carousel-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 16:46:06.291706 streamlit_carousel-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-07-08 16:35:57.000000 streamlit_carousel-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.244831 streamlit_carousel-0.0.2/streamlit_carousel/
--rw-rw-rw-   0        0        0     4863 2023-07-08 16:19:18.000000 streamlit_carousel-0.0.2/streamlit_carousel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.229206 streamlit_carousel-0.0.2/streamlit_carousel/carousel/
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.260454 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/
--rw-rw-rw-   0        0        0     1058 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/asset-manifest.json
--rw-rw-rw-   0        0        0     1910 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/index.html
--rw-rw-rw-   0        0        0      660 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/precache-manifest.22851dbcebea0476fd3c97bc108bb6e8.js
--rw-rw-rw-   0        0        0     1183 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/service-worker.js
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.229206 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.260454 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/css/
--rw-rw-rw-   0        0        0   241050 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css
--rw-rw-rw-   0        0        0   583870 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.291706 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/
--rw-rw-rw-   0        0        0   616599 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js
--rw-rw-rw-   0        0        0     2181 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1664534 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.map
--rw-rw-rw-   0        0        0     1351 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js
--rw-rw-rw-   0        0        0     3998 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js.map
--rw-rw-rw-   0        0        0     1578 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js
--rw-rw-rw-   0        0        0     8297 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js.map
-drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.260454 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/
--rw-rw-rw-   0        0        0     4918 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.273029 streamlit_carousel-0.0.3/
+-rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_carousel-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-07-08 16:44:00.000000 streamlit_carousel-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4918 2023-07-08 16:55:15.272029 streamlit_carousel-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2997 2023-07-08 16:34:50.000000 streamlit_carousel-0.0.3/README.md
+-rw-rw-rw-   0        0        0      907 2023-07-08 16:53:42.000000 streamlit_carousel-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 16:55:15.273029 streamlit_carousel-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-07-08 16:53:38.000000 streamlit_carousel-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.219026 streamlit_carousel-0.0.3/streamlit_carousel/
+-rw-rw-rw-   0        0        0     4866 2023-07-08 16:54:10.000000 streamlit_carousel-0.0.3/streamlit_carousel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.202027 streamlit_carousel-0.0.3/streamlit_carousel/carousel/
+drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.240027 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/
+-rw-rw-rw-   0        0        0     1058 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     1946 2023-07-08 16:50:20.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/index.html
+-rw-rw-rw-   0        0        0      660 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/precache-manifest.22851dbcebea0476fd3c97bc108bb6e8.js
+-rw-rw-rw-   0        0        0     1183 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.204027 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.245028 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/css/
+-rw-rw-rw-   0        0        0   241050 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css
+-rw-rw-rw-   0        0        0   583870 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.270026 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/
+-rw-rw-rw-   0        0        0   616599 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js
+-rw-rw-rw-   0        0        0     2181 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1664534 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.map
+-rw-rw-rw-   0        0        0     1351 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js
+-rw-rw-rw-   0        0        0     3998 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js.map
+-rw-rw-rw-   0        0        0     1578 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js
+-rw-rw-rw-   0        0        0     8297 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js.map
+drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.231027 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/
+-rw-rw-rw-   0        0        0     4918 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/top_level.txt
```

### Comparing `streamlit_carousel-0.0.2/LICENSE` & `streamlit_carousel-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/PKG-INFO` & `streamlit_carousel-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_carousel
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Streamlit implementation of the React Bootstrap Carousel component.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit_carousel-0.0.2/README.md` & `streamlit_carousel-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/pyproject.toml` & `streamlit_carousel-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit_carousel"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Streamlit implementation of the React Bootstrap Carousel component."
 readme = "README.md"
 authors = [{ name = "Thomas Bouamoud", email = "thomas.bouamoud@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `streamlit_carousel-0.0.2/setup.py` & `streamlit_carousel-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_carousel",
-    version="0.0.2",
+    version="0.0.3",
     author="Thomas Bouamoud",
     author_email="thomas.bouamoud@gmail.com",
     description="A Streamlit implementation of the React Bootstrap Carousel component.",
     long_description="https://react-bootstrap.netlify.app/docs/components/carousel/",
     long_description_content_type="text/plain",
     url="https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/__init__.py` & `streamlit_carousel-0.0.3/streamlit_carousel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 if not _RELEASE:
     _bootstrap_carousel = components.declare_component(
         "streamlit_carousel", url="http://localhost:3000",
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
-    modal_dir = os.path.join(parent_dir, "modal/build")
+    modal_dir = os.path.join(parent_dir, "carousel/build")
     _bootstrap_carousel = components.declare_component(
         "streamlit_carousel", path=modal_dir
     )
 
 
 class Item(TypedDict):
     title: str
```

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/asset-manifest.json` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/index.html` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js`

 * *Files 18% similar despite different names*

```diff
@@ -1,120 +1,99 @@
-00000000: 3c21 646f 6374 7970 6520 6874 6d6c 3e3c  <!doctype html><
-00000010: 6874 6d6c 206c 616e 673d 2265 6e22 2073  html lang="en" s
-00000020: 7479 6c65 3d22 6261 636b 6772 6f75 6e64  tyle="background
-00000030: 3a23 6666 6666 6666 3031 2169 6d70 6f72  :#ffffff01!impor
-00000040: 7461 6e74 223e 3c68 6561 643e 3c6c 696e  tant"><head><lin
-00000050: 6b20 6872 6566 3d22 2e2f 7374 6174 6963  k href="./static
-00000060: 2f63 7373 2f32 2e37 3737 6431 3834 362e  /css/2.777d1846.
-00000070: 6368 756e 6b2e 6373 7322 2072 656c 3d22  chunk.css" rel="
-00000080: 7374 796c 6573 6865 6574 223e 3c2f 6865  stylesheet"></he
-00000090: 6164 3e3c 626f 6479 3e3c 6e6f 7363 7269  ad><body><noscri
-000000a0: 7074 3e59 6f75 206e 6565 6420 746f 2065  pt>You need to e
-000000b0: 6e61 626c 6520 4a61 7661 5363 7269 7074  nable JavaScript
-000000c0: 2074 6f20 7275 6e20 7468 6973 2061 7070   to run this app
-000000d0: 2e3c 2f6e 6f73 6372 6970 743e 3c64 6976  .</noscript><div
-000000e0: 2069 643d 2272 6f6f 7422 3e3c 2f64 6976   id="root"></div
-000000f0: 3e3c 7363 7269 7074 3e21 6675 6e63 7469  ><script>!functi
-00000100: 6f6e 2865 297b 6675 6e63 7469 6f6e 2072  on(e){function r
-00000110: 2872 297b 666f 7228 7661 7220 6e2c 6c2c  (r){for(var n,l,
-00000120: 613d 725b 305d 2c69 3d72 5b31 5d2c 663d  a=r[0],i=r[1],f=
-00000130: 725b 325d 2c70 3d30 2c73 3d5b 5d3b 703c  r[2],p=0,s=[];p<
-00000140: 612e 6c65 6e67 7468 3b70 2b2b 296c 3d61  a.length;p++)l=a
-00000150: 5b70 5d2c 4f62 6a65 6374 2e70 726f 746f  [p],Object.proto
-00000160: 7479 7065 2e68 6173 4f77 6e50 726f 7065  type.hasOwnPrope
-00000170: 7274 792e 6361 6c6c 286f 2c6c 2926 266f  rty.call(o,l)&&o
-00000180: 5b6c 5d26 2673 2e70 7573 6828 6f5b 6c5d  [l]&&s.push(o[l]
-00000190: 5b30 5d29 2c6f 5b6c 5d3d 303b 666f 7228  [0]),o[l]=0;for(
-000001a0: 6e20 696e 2069 294f 626a 6563 742e 7072  n in i)Object.pr
-000001b0: 6f74 6f74 7970 652e 6861 734f 776e 5072  ototype.hasOwnPr
-000001c0: 6f70 6572 7479 2e63 616c 6c28 692c 6e29  operty.call(i,n)
-000001d0: 2626 2865 5b6e 5d3d 695b 6e5d 293b 666f  &&(e[n]=i[n]);fo
-000001e0: 7228 6326 2663 2872 293b 732e 6c65 6e67  r(c&&c(r);s.leng
-000001f0: 7468 3b29 732e 7368 6966 7428 2928 293b  th;)s.shift()();
-00000200: 7265 7475 726e 2075 2e70 7573 682e 6170  return u.push.ap
-00000210: 706c 7928 752c 667c 7c5b 5d29 2c74 2829  ply(u,f||[]),t()
-00000220: 7d66 756e 6374 696f 6e20 7428 297b 666f  }function t(){fo
-00000230: 7228 7661 7220 652c 723d 303b 723c 752e  r(var e,r=0;r<u.
-00000240: 6c65 6e67 7468 3b72 2b2b 297b 666f 7228  length;r++){for(
-00000250: 7661 7220 743d 755b 725d 2c6e 3d21 302c  var t=u[r],n=!0,
-00000260: 613d 313b 613c 742e 6c65 6e67 7468 3b61  a=1;a<t.length;a
-00000270: 2b2b 297b 7661 7220 693d 745b 615d 3b30  ++){var i=t[a];0
-00000280: 213d 3d6f 5b69 5d26 2628 6e3d 2131 297d  !==o[i]&&(n=!1)}
-00000290: 6e26 2628 752e 7370 6c69 6365 2872 2d2d  n&&(u.splice(r--
-000002a0: 2c31 292c 653d 6c28 6c2e 733d 745b 305d  ,1),e=l(l.s=t[0]
-000002b0: 2929 7d72 6574 7572 6e20 657d 7661 7220  ))}return e}var 
-000002c0: 6e3d 7b7d 2c6f 3d7b 313a 307d 2c75 3d5b  n={},o={1:0},u=[
-000002d0: 5d3b 6675 6e63 7469 6f6e 206c 2872 297b  ];function l(r){
-000002e0: 6966 286e 5b72 5d29 7265 7475 726e 206e  if(n[r])return n
-000002f0: 5b72 5d2e 6578 706f 7274 733b 7661 7220  [r].exports;var 
-00000300: 743d 6e5b 725d 3d7b 693a 722c 6c3a 2131  t=n[r]={i:r,l:!1
-00000310: 2c65 7870 6f72 7473 3a7b 7d7d 3b72 6574  ,exports:{}};ret
-00000320: 7572 6e20 655b 725d 2e63 616c 6c28 742e  urn e[r].call(t.
-00000330: 6578 706f 7274 732c 742c 742e 6578 706f  exports,t,t.expo
-00000340: 7274 732c 6c29 2c74 2e6c 3d21 302c 742e  rts,l),t.l=!0,t.
-00000350: 6578 706f 7274 737d 6c2e 6d3d 652c 6c2e  exports}l.m=e,l.
-00000360: 633d 6e2c 6c2e 643d 6675 6e63 7469 6f6e  c=n,l.d=function
-00000370: 2865 2c72 2c74 297b 6c2e 6f28 652c 7229  (e,r,t){l.o(e,r)
-00000380: 7c7c 4f62 6a65 6374 2e64 6566 696e 6550  ||Object.defineP
-00000390: 726f 7065 7274 7928 652c 722c 7b65 6e75  roperty(e,r,{enu
-000003a0: 6d65 7261 626c 653a 2130 2c67 6574 3a74  merable:!0,get:t
-000003b0: 7d29 7d2c 6c2e 723d 6675 6e63 7469 6f6e  })},l.r=function
-000003c0: 2865 297b 2275 6e64 6566 696e 6564 2221  (e){"undefined"!
-000003d0: 3d74 7970 656f 6620 5379 6d62 6f6c 2626  =typeof Symbol&&
-000003e0: 5379 6d62 6f6c 2e74 6f53 7472 696e 6754  Symbol.toStringT
-000003f0: 6167 2626 4f62 6a65 6374 2e64 6566 696e  ag&&Object.defin
-00000400: 6550 726f 7065 7274 7928 652c 5379 6d62  eProperty(e,Symb
-00000410: 6f6c 2e74 6f53 7472 696e 6754 6167 2c7b  ol.toStringTag,{
-00000420: 7661 6c75 653a 224d 6f64 756c 6522 7d29  value:"Module"})
-00000430: 2c4f 626a 6563 742e 6465 6669 6e65 5072  ,Object.definePr
-00000440: 6f70 6572 7479 2865 2c22 5f5f 6573 4d6f  operty(e,"__esMo
-00000450: 6475 6c65 222c 7b76 616c 7565 3a21 307d  dule",{value:!0}
-00000460: 297d 2c6c 2e74 3d66 756e 6374 696f 6e28  )},l.t=function(
-00000470: 652c 7229 7b69 6628 3126 7226 2628 653d  e,r){if(1&r&&(e=
-00000480: 6c28 6529 292c 3826 7229 7265 7475 726e  l(e)),8&r)return
-00000490: 2065 3b69 6628 3426 7226 2622 6f62 6a65   e;if(4&r&&"obje
-000004a0: 6374 223d 3d74 7970 656f 6620 6526 2665  ct"==typeof e&&e
-000004b0: 2626 652e 5f5f 6573 4d6f 6475 6c65 2972  &&e.__esModule)r
-000004c0: 6574 7572 6e20 653b 7661 7220 743d 4f62  eturn e;var t=Ob
-000004d0: 6a65 6374 2e63 7265 6174 6528 6e75 6c6c  ject.create(null
-000004e0: 293b 6966 286c 2e72 2874 292c 4f62 6a65  );if(l.r(t),Obje
-000004f0: 6374 2e64 6566 696e 6550 726f 7065 7274  ct.definePropert
-00000500: 7928 742c 2264 6566 6175 6c74 222c 7b65  y(t,"default",{e
-00000510: 6e75 6d65 7261 626c 653a 2130 2c76 616c  numerable:!0,val
-00000520: 7565 3a65 7d29 2c32 2672 2626 2273 7472  ue:e}),2&r&&"str
-00000530: 696e 6722 213d 7479 7065 6f66 2065 2966  ing"!=typeof e)f
-00000540: 6f72 2876 6172 206e 2069 6e20 6529 6c2e  or(var n in e)l.
-00000550: 6428 742c 6e2c 6675 6e63 7469 6f6e 2872  d(t,n,function(r
-00000560: 297b 7265 7475 726e 2065 5b72 5d7d 2e62  ){return e[r]}.b
-00000570: 696e 6428 6e75 6c6c 2c6e 2929 3b72 6574  ind(null,n));ret
-00000580: 7572 6e20 747d 2c6c 2e6e 3d66 756e 6374  urn t},l.n=funct
-00000590: 696f 6e28 6529 7b76 6172 2072 3d65 2626  ion(e){var r=e&&
-000005a0: 652e 5f5f 6573 4d6f 6475 6c65 3f66 756e  e.__esModule?fun
-000005b0: 6374 696f 6e28 297b 7265 7475 726e 2065  ction(){return e
-000005c0: 2e64 6566 6175 6c74 7d3a 6675 6e63 7469  .default}:functi
-000005d0: 6f6e 2829 7b72 6574 7572 6e20 657d 3b72  on(){return e};r
-000005e0: 6574 7572 6e20 6c2e 6428 722c 2261 222c  eturn l.d(r,"a",
-000005f0: 7229 2c72 7d2c 6c2e 6f3d 6675 6e63 7469  r),r},l.o=functi
-00000600: 6f6e 2865 2c72 297b 7265 7475 726e 204f  on(e,r){return O
-00000610: 626a 6563 742e 7072 6f74 6f74 7970 652e  bject.prototype.
-00000620: 6861 734f 776e 5072 6f70 6572 7479 2e63  hasOwnProperty.c
-00000630: 616c 6c28 652c 7229 7d2c 6c2e 703d 222e  all(e,r)},l.p=".
-00000640: 2f22 3b76 6172 2061 3d74 6869 732e 7765  /";var a=this.we
-00000650: 6270 6163 6b4a 736f 6e70 7374 7265 616d  bpackJsonpstream
-00000660: 6c69 745f 6361 726f 7573 656c 3d74 6869  lit_carousel=thi
-00000670: 732e 7765 6270 6163 6b4a 736f 6e70 7374  s.webpackJsonpst
-00000680: 7265 616d 6c69 745f 6361 726f 7573 656c  reamlit_carousel
-00000690: 7c7c 5b5d 2c69 3d61 2e70 7573 682e 6269  ||[],i=a.push.bi
-000006a0: 6e64 2861 293b 612e 7075 7368 3d72 2c61  nd(a);a.push=r,a
-000006b0: 3d61 2e73 6c69 6365 2829 3b66 6f72 2876  =a.slice();for(v
-000006c0: 6172 2066 3d30 3b66 3c61 2e6c 656e 6774  ar f=0;f<a.lengt
-000006d0: 683b 662b 2b29 7228 615b 665d 293b 7661  h;f++)r(a[f]);va
-000006e0: 7220 633d 693b 7428 297d 285b 5d29 3c2f  r c=i;t()}([])</
-000006f0: 7363 7269 7074 3e3c 7363 7269 7074 2073  script><script s
-00000700: 7263 3d22 2e2f 7374 6174 6963 2f6a 732f  rc="./static/js/
-00000710: 322e 3464 6333 3137 6362 2e63 6875 6e6b  2.4dc317cb.chunk
-00000720: 2e6a 7322 3e3c 2f73 6372 6970 743e 3c73  .js"></script><s
-00000730: 6372 6970 7420 7372 633d 222e 2f73 7461  cript src="./sta
-00000740: 7469 632f 6a73 2f6d 6169 6e2e 6635 3936  tic/js/main.f596
-00000750: 6136 3235 2e63 6875 6e6b 2e6a 7322 3e3c  a625.chunk.js"><
-00000760: 2f73 6372 6970 743e 3c2f 626f 6479 3e3c  /script></body><
-00000770: 2f68 746d 6c3e                           /html>
+00000000: 2166 756e 6374 696f 6e28 6529 7b66 756e  !function(e){fun
+00000010: 6374 696f 6e20 7228 7229 7b66 6f72 2876  ction r(r){for(v
+00000020: 6172 206e 2c6c 2c61 3d72 5b30 5d2c 693d  ar n,l,a=r[0],i=
+00000030: 725b 315d 2c66 3d72 5b32 5d2c 703d 302c  r[1],f=r[2],p=0,
+00000040: 733d 5b5d 3b70 3c61 2e6c 656e 6774 683b  s=[];p<a.length;
+00000050: 702b 2b29 6c3d 615b 705d 2c4f 626a 6563  p++)l=a[p],Objec
+00000060: 742e 7072 6f74 6f74 7970 652e 6861 734f  t.prototype.hasO
+00000070: 776e 5072 6f70 6572 7479 2e63 616c 6c28  wnProperty.call(
+00000080: 6f2c 6c29 2626 6f5b 6c5d 2626 732e 7075  o,l)&&o[l]&&s.pu
+00000090: 7368 286f 5b6c 5d5b 305d 292c 6f5b 6c5d  sh(o[l][0]),o[l]
+000000a0: 3d30 3b66 6f72 286e 2069 6e20 6929 4f62  =0;for(n in i)Ob
+000000b0: 6a65 6374 2e70 726f 746f 7479 7065 2e68  ject.prototype.h
+000000c0: 6173 4f77 6e50 726f 7065 7274 792e 6361  asOwnProperty.ca
+000000d0: 6c6c 2869 2c6e 2926 2628 655b 6e5d 3d69  ll(i,n)&&(e[n]=i
+000000e0: 5b6e 5d29 3b66 6f72 2863 2626 6328 7229  [n]);for(c&&c(r)
+000000f0: 3b73 2e6c 656e 6774 683b 2973 2e73 6869  ;s.length;)s.shi
+00000100: 6674 2829 2829 3b72 6574 7572 6e20 752e  ft()();return u.
+00000110: 7075 7368 2e61 7070 6c79 2875 2c66 7c7c  push.apply(u,f||
+00000120: 5b5d 292c 7428 297d 6675 6e63 7469 6f6e  []),t()}function
+00000130: 2074 2829 7b66 6f72 2876 6172 2065 2c72   t(){for(var e,r
+00000140: 3d30 3b72 3c75 2e6c 656e 6774 683b 722b  =0;r<u.length;r+
+00000150: 2b29 7b66 6f72 2876 6172 2074 3d75 5b72  +){for(var t=u[r
+00000160: 5d2c 6e3d 2130 2c61 3d31 3b61 3c74 2e6c  ],n=!0,a=1;a<t.l
+00000170: 656e 6774 683b 612b 2b29 7b76 6172 2069  ength;a++){var i
+00000180: 3d74 5b61 5d3b 3021 3d3d 6f5b 695d 2626  =t[a];0!==o[i]&&
+00000190: 286e 3d21 3129 7d6e 2626 2875 2e73 706c  (n=!1)}n&&(u.spl
+000001a0: 6963 6528 722d 2d2c 3129 2c65 3d6c 286c  ice(r--,1),e=l(l
+000001b0: 2e73 3d74 5b30 5d29 297d 7265 7475 726e  .s=t[0]))}return
+000001c0: 2065 7d76 6172 206e 3d7b 7d2c 6f3d 7b31   e}var n={},o={1
+000001d0: 3a30 7d2c 753d 5b5d 3b66 756e 6374 696f  :0},u=[];functio
+000001e0: 6e20 6c28 7229 7b69 6628 6e5b 725d 2972  n l(r){if(n[r])r
+000001f0: 6574 7572 6e20 6e5b 725d 2e65 7870 6f72  eturn n[r].expor
+00000200: 7473 3b76 6172 2074 3d6e 5b72 5d3d 7b69  ts;var t=n[r]={i
+00000210: 3a72 2c6c 3a21 312c 6578 706f 7274 733a  :r,l:!1,exports:
+00000220: 7b7d 7d3b 7265 7475 726e 2065 5b72 5d2e  {}};return e[r].
+00000230: 6361 6c6c 2874 2e65 7870 6f72 7473 2c74  call(t.exports,t
+00000240: 2c74 2e65 7870 6f72 7473 2c6c 292c 742e  ,t.exports,l),t.
+00000250: 6c3d 2130 2c74 2e65 7870 6f72 7473 7d6c  l=!0,t.exports}l
+00000260: 2e6d 3d65 2c6c 2e63 3d6e 2c6c 2e64 3d66  .m=e,l.c=n,l.d=f
+00000270: 756e 6374 696f 6e28 652c 722c 7429 7b6c  unction(e,r,t){l
+00000280: 2e6f 2865 2c72 297c 7c4f 626a 6563 742e  .o(e,r)||Object.
+00000290: 6465 6669 6e65 5072 6f70 6572 7479 2865  defineProperty(e
+000002a0: 2c72 2c7b 656e 756d 6572 6162 6c65 3a21  ,r,{enumerable:!
+000002b0: 302c 6765 743a 747d 297d 2c6c 2e72 3d66  0,get:t})},l.r=f
+000002c0: 756e 6374 696f 6e28 6529 7b22 756e 6465  unction(e){"unde
+000002d0: 6669 6e65 6422 213d 3d74 7970 656f 6620  fined"!==typeof 
+000002e0: 5379 6d62 6f6c 2626 5379 6d62 6f6c 2e74  Symbol&&Symbol.t
+000002f0: 6f53 7472 696e 6754 6167 2626 4f62 6a65  oStringTag&&Obje
+00000300: 6374 2e64 6566 696e 6550 726f 7065 7274  ct.definePropert
+00000310: 7928 652c 5379 6d62 6f6c 2e74 6f53 7472  y(e,Symbol.toStr
+00000320: 696e 6754 6167 2c7b 7661 6c75 653a 224d  ingTag,{value:"M
+00000330: 6f64 756c 6522 7d29 2c4f 626a 6563 742e  odule"}),Object.
+00000340: 6465 6669 6e65 5072 6f70 6572 7479 2865  defineProperty(e
+00000350: 2c22 5f5f 6573 4d6f 6475 6c65 222c 7b76  ,"__esModule",{v
+00000360: 616c 7565 3a21 307d 297d 2c6c 2e74 3d66  alue:!0})},l.t=f
+00000370: 756e 6374 696f 6e28 652c 7229 7b69 6628  unction(e,r){if(
+00000380: 3126 7226 2628 653d 6c28 6529 292c 3826  1&r&&(e=l(e)),8&
+00000390: 7229 7265 7475 726e 2065 3b69 6628 3426  r)return e;if(4&
+000003a0: 7226 2622 6f62 6a65 6374 223d 3d3d 7479  r&&"object"===ty
+000003b0: 7065 6f66 2065 2626 6526 2665 2e5f 5f65  peof e&&e&&e.__e
+000003c0: 734d 6f64 756c 6529 7265 7475 726e 2065  sModule)return e
+000003d0: 3b76 6172 2074 3d4f 626a 6563 742e 6372  ;var t=Object.cr
+000003e0: 6561 7465 286e 756c 6c29 3b69 6628 6c2e  eate(null);if(l.
+000003f0: 7228 7429 2c4f 626a 6563 742e 6465 6669  r(t),Object.defi
+00000400: 6e65 5072 6f70 6572 7479 2874 2c22 6465  neProperty(t,"de
+00000410: 6661 756c 7422 2c7b 656e 756d 6572 6162  fault",{enumerab
+00000420: 6c65 3a21 302c 7661 6c75 653a 657d 292c  le:!0,value:e}),
+00000430: 3226 7226 2622 7374 7269 6e67 2221 3d74  2&r&&"string"!=t
+00000440: 7970 656f 6620 6529 666f 7228 7661 7220  ypeof e)for(var 
+00000450: 6e20 696e 2065 296c 2e64 2874 2c6e 2c66  n in e)l.d(t,n,f
+00000460: 756e 6374 696f 6e28 7229 7b72 6574 7572  unction(r){retur
+00000470: 6e20 655b 725d 7d2e 6269 6e64 286e 756c  n e[r]}.bind(nul
+00000480: 6c2c 6e29 293b 7265 7475 726e 2074 7d2c  l,n));return t},
+00000490: 6c2e 6e3d 6675 6e63 7469 6f6e 2865 297b  l.n=function(e){
+000004a0: 7661 7220 723d 6526 2665 2e5f 5f65 734d  var r=e&&e.__esM
+000004b0: 6f64 756c 653f 6675 6e63 7469 6f6e 2829  odule?function()
+000004c0: 7b72 6574 7572 6e20 652e 6465 6661 756c  {return e.defaul
+000004d0: 747d 3a66 756e 6374 696f 6e28 297b 7265  t}:function(){re
+000004e0: 7475 726e 2065 7d3b 7265 7475 726e 206c  turn e};return l
+000004f0: 2e64 2872 2c22 6122 2c72 292c 727d 2c6c  .d(r,"a",r),r},l
+00000500: 2e6f 3d66 756e 6374 696f 6e28 652c 7229  .o=function(e,r)
+00000510: 7b72 6574 7572 6e20 4f62 6a65 6374 2e70  {return Object.p
+00000520: 726f 746f 7479 7065 2e68 6173 4f77 6e50  rototype.hasOwnP
+00000530: 726f 7065 7274 792e 6361 6c6c 2865 2c72  roperty.call(e,r
+00000540: 297d 2c6c 2e70 3d22 2e2f 223b 7661 7220  )},l.p="./";var 
+00000550: 613d 7468 6973 2e77 6562 7061 636b 4a73  a=this.webpackJs
+00000560: 6f6e 7073 7472 6561 6d6c 6974 5f63 6172  onpstreamlit_car
+00000570: 6f75 7365 6c3d 7468 6973 2e77 6562 7061  ousel=this.webpa
+00000580: 636b 4a73 6f6e 7073 7472 6561 6d6c 6974  ckJsonpstreamlit
+00000590: 5f63 6172 6f75 7365 6c7c 7c5b 5d2c 693d  _carousel||[],i=
+000005a0: 612e 7075 7368 2e62 696e 6428 6129 3b61  a.push.bind(a);a
+000005b0: 2e70 7573 683d 722c 613d 612e 736c 6963  .push=r,a=a.slic
+000005c0: 6528 293b 666f 7228 7661 7220 663d 303b  e();for(var f=0;
+000005d0: 663c 612e 6c65 6e67 7468 3b66 2b2b 2972  f<a.length;f++)r
+000005e0: 2861 5b66 5d29 3b76 6172 2063 3d69 3b74  (a[f]);var c=i;t
+000005f0: 2829 7d28 5b5d 293b 0a2f 2f23 2073 6f75  ()}([]);.//# sou
+00000600: 7263 654d 6170 7069 6e67 5552 4c3d 7275  rceMappingURL=ru
+00000610: 6e74 696d 652d 6d61 696e 2e35 6534 3038  ntime-main.5e408
+00000620: 6638 392e 6a73 2e6d 6170                 f89.js.map
```

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/precache-manifest.22851dbcebea0476fd3c97bc108bb6e8.js` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/precache-manifest.22851dbcebea0476fd3c97bc108bb6e8.js`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/service-worker.js` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css.map` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.LICENSE.txt` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.map` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js.map` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js.map` & `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel.egg-info/PKG-INFO` & `streamlit_carousel-0.0.3/streamlit_carousel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-carousel
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Streamlit implementation of the React Bootstrap Carousel component.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit_carousel-0.0.2/streamlit_carousel.egg-info/SOURCES.txt` & `streamlit_carousel-0.0.3/streamlit_carousel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

