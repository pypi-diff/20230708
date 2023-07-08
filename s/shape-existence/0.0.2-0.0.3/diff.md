# Comparing `tmp/shape_existence-0.0.2.tar.gz` & `tmp/shape_existence-0.0.3.tar.gz`

## Comparing `shape_existence-0.0.2.tar` & `shape_existence-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 shape_existence-0.0.2/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 shape_existence-0.0.2/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/shape_existence/__init__.py
--rw-r--r--   0        0        0    21252 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/shape_existence/complexes_and_proofs.py
--rw-r--r--   0        0        0    13379 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/shape_existence/flexible_cqp.py
--rw-r--r--   0        0        0    16698 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/shape_existence/fractions_and_interval_arithmetic.py
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 shape_existence-0.0.2/src/shape_existence/obj_stuff.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 shape_existence-0.0.2/LICENSE
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 shape_existence-0.0.2/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 shape_existence-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 shape_existence-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 shape_existence-0.0.3/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 shape_existence-0.0.3/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 shape_existence-0.0.3/src/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shape_existence-0.0.3/src/shape_existence/__init__.py
+-rw-r--r--   0        0        0    21252 2020-02-02 00:00:00.000000 shape_existence-0.0.3/src/shape_existence/complexes_and_proofs.py
+-rw-r--r--   0        0        0    13379 2020-02-02 00:00:00.000000 shape_existence-0.0.3/src/shape_existence/flexible_cqp.py
+-rw-r--r--   0        0        0    16698 2020-02-02 00:00:00.000000 shape_existence-0.0.3/src/shape_existence/fractions_and_interval_arithmetic.py
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 shape_existence-0.0.3/src/shape_existence/obj_stuff.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 shape_existence-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 shape_existence-0.0.3/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 shape_existence-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 shape_existence-0.0.3/PKG-INFO
```

### Comparing `shape_existence-0.0.2/.DS_Store` & `shape_existence-0.0.3/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 000e  ................
 00000050: 0000 0001 0000 1000 6277 7370 626c 6f62  ........bwspblob
-00000060: 0000 00c9 0000 0000 0000 0000 0000 0000  ................
+00000060: 0000 00c7 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -60,75 +60,75 @@
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 000e 0000 0004  ................
 00000410: 0064 0069 0073 0074 6277 7370 626c 6f62  .d.i.s.tbwspblob
-00000420: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
+00000420: 0000 00c7 6270 6c69 7374 3030 d701 0203  ....bplist00....
 00000430: 0405 0607 0809 0909 090d 095d 5368 6f77  ...........]Show
 00000440: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 00000450: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
 00000460: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00000470: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00000480: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00000490: 735b 5368 6f77 5369 6465 6261 7208 0909  s[ShowSidebar...
-000004a0: 0909 5f10 187b 7b2d 3138 2c20 3138 367d  .._..{{-18, 186}
-000004b0: 2c20 7b37 3430 2c20 3538 397d 7d09 0817  , {740, 589}}...
-000004c0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-000004d0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-000004e0: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
-000004f0: 0400 6400 6900 7300 7476 5372 6e6c 6f6e  ..d.i.s.tvSrnlon
-00000500: 6700 0000 0100 0000 0300 7300 7200 6362  g.........s.r.cb
-00000510: 7773 7062 6c6f 6200 0000 c762 706c 6973  wspblob....bplis
-00000520: 7430 30d7 0102 0304 0506 0708 0909 0909  t00.............
-00000530: 0d09 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-00000540: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
-00000550: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
-00000560: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
-00000570: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
-00000580: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-00000590: 6562 6172 0809 0909 095f 1016 7b7b 2d31  ebar....._..{{-1
-000005a0: 332c 2033 7d2c 207b 3632 392c 2037 3732  3, 3}, {629, 772
-000005b0: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-000005c0: 7e97 0000 0000 0000 0101 0000 0000 0000  ~...............
-000005d0: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-000005e0: 0098 0000 0003 0073 0072 0063 6c67 3153  .......s.r.clg1S
-000005f0: 636f 6d70 0000 0000 0000 0000 0000 0003  comp............
-00000600: 0073 0072 0063 6d6f 4444 626c 6f62 0000  .s.r.cmoDDblob..
-00000610: 0008 d042 6e9c 5e2c c541 0000 0003 0073  ...Bn.^,.A.....s
-00000620: 0072 0063 6d6f 6444 626c 6f62 0000 0008  .r.cmodDblob....
-00000630: d042 6e9c 5e2c c541 0000 0003 0073 0072  .Bn.^,.A.....s.r
-00000640: 0063 7068 3153 636f 6d70 0000 0000 0000  .cph1Scomp......
-00000650: 0000 0000 0003 0073 0072 0063 7653 726e  .......s.r.cvSrn
-00000660: 6c6f 6e67 0000 0001 0000 0005 0074 0065  long.........t.e
-00000670: 0073 0074 0073 6277 7370 626c 6f62 0000  .s.t.sbwspblob..
-00000680: 00c7 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00000690: 0607 0809 0909 090d 095d 5368 6f77 5374  .........]ShowSt
-000006a0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-000006b0: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-000006c0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-000006d0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-000006e0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-000006f0: 5368 6f77 5369 6465 6261 7208 0909 0909  ShowSidebar.....
-00000700: 5f10 167b 7b2d 3133 2c20 337d 2c20 7b36  _..{{-13, 3}, {6
-00000710: 3239 2c20 3737 327d 7d09 0817 2531 3d49  29, 772}}...%1=I
-00000720: 606d 797a 7b7c 7d7e 9700 0000 0000 0001  `myz{|}~........
-00000730: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-00000740: 0000 0000 0000 0000 9800 0000 0500 7400  ..............t.
-00000750: 6500 7300 7400 736c 6731 5363 6f6d 7000  e.s.t.slg1Scomp.
-00000760: 0000 0000 0000 0000 0000 0500 7400 6500  ............t.e.
-00000770: 7300 7400 736d 6f44 4462 6c6f 6200 0000  s.t.smoDDblob...
-00000780: 08f3 cdae 985e 2cc5 4100 0000 0500 7400  .....^,.A.....t.
-00000790: 6500 7300 7400 736d 6f64 4462 6c6f 6200  e.s.t.smodDblob.
-000007a0: 0000 08f3 cdae 985e 2cc5 4100 0000 0500  .......^,.A.....
-000007b0: 7400 6500 7300 7400 7370 6831 5363 6f6d  t.e.s.t.sph1Scom
-000007c0: 7000 0000 0000 0000 0000 0000 0500 7400  p.............t.
-000007d0: 6500 7300 7400 7376 5372 6e6c 6f6e 6700  e.s.t.svSrnlong.
-000007e0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+000004a0: 0909 5f10 167b 7b2d 3133 2c20 337d 2c20  .._..{{-13, 3}, 
+000004b0: 7b36 3239 2c20 3737 327d 7d09 0817 2531  {629, 772}}...%1
+000004c0: 3d49 606d 797a 7b7c 7d7e 9700 0000 0000  =I`myz{|}~......
+000004d0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
+000004e0: 0000 0000 0000 0000 0000 9800 0000 0400  ................
+000004f0: 6400 6900 7300 7476 5372 6e6c 6f6e 6700  d.i.s.tvSrnlong.
+00000500: 0000 0100 0000 0300 7300 7200 6362 7773  ........s.r.cbws
+00000510: 7062 6c6f 6200 0000 c762 706c 6973 7430  pblob....bplist0
+00000520: 30d7 0102 0304 0506 0708 0909 0909 0d09  0...............
+00000530: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
+00000540: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
+00000550: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
+00000560: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
+00000570: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
+00000580: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
+00000590: 6172 0809 0909 095f 1016 7b7b 2d31 332c  ar....._..{{-13,
+000005a0: 2033 7d2c 207b 3632 392c 2037 3732 7d7d   3}, {629, 772}}
+000005b0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e97  ...%1=I`myz{|}~.
+000005c0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+000005d0: 0000 0000 0000 0000 0000 0000 0000 0098  ................
+000005e0: 0000 0003 0073 0072 0063 6c67 3153 636f  .....s.r.clg1Sco
+000005f0: 6d70 0000 0000 0000 0000 0000 0003 0073  mp.............s
+00000600: 0072 0063 6d6f 4444 626c 6f62 0000 0008  .r.cmoDDblob....
+00000610: d042 6e9c 5e2c c541 0000 0003 0073 0072  .Bn.^,.A.....s.r
+00000620: 0063 6d6f 6444 626c 6f62 0000 0008 d042  .cmodDblob.....B
+00000630: 6e9c 5e2c c541 0000 0003 0073 0072 0063  n.^,.A.....s.r.c
+00000640: 7068 3153 636f 6d70 0000 0000 0000 0000  ph1Scomp........
+00000650: 0000 0003 0073 0072 0063 7653 726e 6c6f  .....s.r.cvSrnlo
+00000660: 6e67 0000 0001 0000 0005 0074 0065 0073  ng.........t.e.s
+00000670: 0074 0073 6277 7370 626c 6f62 0000 00c7  .t.sbwspblob....
+00000680: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+00000690: 0809 0909 090d 095d 5368 6f77 5374 6174  .......]ShowStat
+000006a0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+000006b0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+000006c0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+000006d0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+000006e0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+000006f0: 6f77 5369 6465 6261 7208 0909 0909 5f10  owSidebar....._.
+00000700: 167b 7b2d 3133 2c20 337d 2c20 7b36 3239  .{{-13, 3}, {629
+00000710: 2c20 3737 327d 7d09 0817 2531 3d49 606d  , 772}}...%1=I`m
+00000720: 797a 7b7c 7d7e 9700 0000 0000 0001 0100  yz{|}~..........
+00000730: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+00000740: 0000 0000 0000 9800 0000 0500 7400 6500  ............t.e.
+00000750: 7300 7400 736c 6731 5363 6f6d 7000 0000  s.t.slg1Scomp...
+00000760: 0000 0000 0000 0000 0500 7400 6500 7300  ..........t.e.s.
+00000770: 7400 736d 6f44 4462 6c6f 6200 0000 08f3  t.smoDDblob.....
+00000780: cdae 985e 2cc5 4100 0000 0500 7400 6500  ...^,.A.....t.e.
+00000790: 7300 7400 736d 6f64 4462 6c6f 6200 0000  s.t.smodDblob...
+000007a0: 08f3 cdae 985e 2cc5 4100 0000 0500 7400  .....^,.A.....t.
+000007b0: 6500 7300 7400 7370 6831 5363 6f6d 7000  e.s.t.sph1Scomp.
+000007c0: 0000 0000 0000 0000 0000 0500 7400 6500  ............t.e.
+000007d0: 7300 7400 7376 5372 6e6c 6f6e 6700 0000  s.t.svSrnlong...
+000007e0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000800: 0000 0000 0000 0001 0000 0000 0000 080b  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `shape_existence-0.0.2/src/.DS_Store` & `shape_existence-0.0.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.2/src/shape_existence/complexes_and_proofs.py` & `shape_existence-0.0.3/src/shape_existence/complexes_and_proofs.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,18 +310,18 @@
         d = self.d
         V = len(self.asc.k_simplices(0))
         E = len(self.asc.k_simplices(1))
         verbose_print(tabbed_string(f" d  = {d}"))
         verbose_print(tabbed_string(f"|V| = {V}"))
         verbose_print(tabbed_string(f"|E| = {E}")) 
         if not (d * V >= E):
-            fail_string = "Failed: not d|V| <= |E|"
+            fail_string = "Failed: not d|V| >= |E|"
             verbose_print(tabbed_string(fail_string))
             return False, fail_string
-        verbose_print(tabbed_string("Success: d|V| <= |E|"))
+        verbose_print(tabbed_string("Success: d|V| >= |E|"))
 
         #check self-intersection
         verbose_print("\nChecking self-intersection:")
         coll_dist_squared = self.square_collision_distance()
         coll_dist = coll_dist_squared.sqrt()
         verbose_print(tabbed_string(f"Square collision distance = {coll_dist_squared}"))
         verbose_print(tabbed_string(f"Collision distance in {coll_dist}"))
```

### Comparing `shape_existence-0.0.2/src/shape_existence/flexible_cqp.py` & `shape_existence-0.0.3/src/shape_existence/flexible_cqp.py`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.2/src/shape_existence/fractions_and_interval_arithmetic.py` & `shape_existence-0.0.3/src/shape_existence/fractions_and_interval_arithmetic.py`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.2/src/shape_existence/obj_stuff.py` & `shape_existence-0.0.3/src/shape_existence/obj_stuff.py`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.2/LICENSE` & `shape_existence-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.2/README.md` & `shape_existence-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `shape_existence-0.0.2/pyproject.toml` & `shape_existence-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "shape_existence"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Matthew Ellison", email="matthew.v.ellison@gmail.com" },
 ]
 description = "A package to prove the existence of non-intersecting realizations of abstract simplicial complexes with specified edge lengths."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `shape_existence-0.0.2/PKG-INFO` & `shape_existence-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shape_existence
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to prove the existence of non-intersecting realizations of abstract simplicial complexes with specified edge lengths.
 Project-URL: Homepage, https://github.com/mve17/shape_existence
 Project-URL: Bug Tracker, https://github.com/mve17/shape_existence/issues
 Author-email: Matthew Ellison <matthew.v.ellison@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

