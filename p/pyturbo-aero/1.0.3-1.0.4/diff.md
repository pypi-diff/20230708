# Comparing `tmp/pyturbo_aero-1.0.3.tar.gz` & `tmp/pyturbo_aero-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyturbo_aero-1.0.3.tar", max compression
+gzip compressed data, was "pyturbo_aero-1.0.4.tar", max compression
```

## Comparing `pyturbo_aero-1.0.3.tar` & `pyturbo_aero-1.0.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      557 2023-07-07 19:53:58.446323 pyturbo_aero-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       95 2023-07-05 19:18:15.890587 pyturbo_aero-1.0.3/pyturbo/__init__.py
--rw-r--r--   0        0        0      152 2023-07-05 19:18:15.890674 pyturbo_aero-1.0.3/pyturbo/aero/__init__.py
--rw-r--r--   0        0        0    44984 2023-07-05 19:18:15.890863 pyturbo_aero-1.0.3/pyturbo/aero/airfoil2D.py
--rw-r--r--   0        0        0    67047 2023-07-05 19:18:15.891147 pyturbo_aero-1.0.3/pyturbo/aero/airfoil3D.py
--rw-r--r--   0        0        0    34367 2023-07-05 19:18:15.891285 pyturbo_aero-1.0.3/pyturbo/aero/airfoil_wavy.py
--rw-r--r--   0        0        0    18449 2023-07-05 19:18:15.891395 pyturbo_aero-1.0.3/pyturbo/aero/passage2D.py
--rw-r--r--   0        0        0      742 2023-07-05 19:18:15.891510 pyturbo_aero-1.0.3/pyturbo/helper/__init__.py
--rw-r--r--   0        0        0     2520 2023-07-05 19:18:15.891580 pyturbo_aero-1.0.3/pyturbo/helper/arc.py
--rw-r--r--   0        0        0    16030 2023-07-05 19:18:15.891686 pyturbo_aero-1.0.3/pyturbo/helper/bezier.py
--rw-r--r--   0        0        0     1295 2023-07-05 19:18:15.891760 pyturbo_aero-1.0.3/pyturbo/helper/bisect.py
--rw-r--r--   0        0        0      107 2023-07-05 19:18:15.891818 pyturbo_aero-1.0.3/pyturbo/helper/centroid.py
--rw-r--r--   0        0        0      477 2023-07-05 19:18:15.891878 pyturbo_aero-1.0.3/pyturbo/helper/convert_to_ndarray.py
--rw-r--r--   0        0        0      490 2023-07-05 19:18:15.891933 pyturbo_aero-1.0.3/pyturbo/helper/csapi.py
--rw-r--r--   0        0        0      832 2023-07-05 19:18:15.891992 pyturbo_aero-1.0.3/pyturbo/helper/derivative.py
--rw-r--r--   0        0        0      239 2023-07-05 19:18:15.892049 pyturbo_aero-1.0.3/pyturbo/helper/dist.py
--rw-r--r--   0        0        0      527 2023-07-05 19:18:15.892110 pyturbo_aero-1.0.3/pyturbo/helper/exp_ratio.py
--rw-r--r--   0        0        0     9841 2023-07-05 19:18:15.892197 pyturbo_aero-1.0.3/pyturbo/helper/line2D.py
--rw-r--r--   0        0        0     1068 2023-07-05 19:18:15.892260 pyturbo_aero-1.0.3/pyturbo/helper/min_max_check.py
--rw-r--r--   0        0        0     9654 2023-07-05 19:18:15.892355 pyturbo_aero-1.0.3/pyturbo/helper/pspline.py
--rw-r--r--   0        0        0     1542 2023-07-05 19:18:15.892422 pyturbo_aero-1.0.3/pyturbo/helper/ray.py
--rw-r--r--   0        0        0      505 2023-07-05 19:18:15.892489 pyturbo_aero-1.0.3/pyturbo/helper/rotate_array_values.py
--rw-r--r--   0        0        0      368 2023-07-05 19:18:15.892555 pyturbo_aero-1.0.3/pyturbo/helper/unique_xy.py
--rw-r--r--   0        0        0     1873 2023-07-05 19:18:15.892618 pyturbo_aero-1.0.3/pyturbo/helper/wave.py
--rw-r--r--   0        0        0      500 2023-07-05 19:18:15.892721 pyturbo_aero-1.0.3/pyturbo/ml/gramian_angular_field.py
--rw-r--r--   0        0        0    37766 2023-07-05 19:18:15.893024 pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/2D_airfoil.png
--rw-r--r--   0        0        0    23891 2023-07-05 19:18:15.893201 pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/Deriv_2.png
--rw-r--r--   0        0        0    25329 2023-07-05 19:18:15.893382 pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/camber_line.png
--rw-r--r--   0        0        0    28623 2023-07-05 19:18:15.893565 pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/s_c.png
--rw-r--r--   0        0        0    61651 2023-07-05 19:18:15.893934 pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_shell.png
--rw-r--r--   0        0        0   213435 2023-07-05 19:18:15.894939 pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_wavy_const_te_radius.PNG
--rw-r--r--   0        0        0   160990 2023-07-05 19:18:15.895327 pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_wavy_variable_te_radius.PNG
--rw-r--r--   0        0        0   146610 2023-07-05 19:18:15.896025 pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_whisker.PNG
--rw-r--r--   0        0        0   420888 2023-07-05 19:18:15.897914 pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator_3D.png
--rw-r--r--   0        0        0    16958 2023-07-05 19:18:15.898104 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/circle_cross_section.png
--rw-r--r--   0        0        0    11380 2023-07-05 19:18:15.898209 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_close_loop_no_return.png
--rw-r--r--   0        0        0    13018 2023-07-05 19:18:15.898311 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_close_loop_return.png
--rw-r--r--   0        0        0    11751 2023-07-05 19:18:15.898407 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_periodic_loop.png
--rw-r--r--   0        0        0   164008 2023-07-05 19:18:15.899158 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pattern_close_loop_no_return.PNG
--rw-r--r--   0        0        0    63687 2023-07-05 19:18:15.899487 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pattern_close_loop_return.PNG
--rw-r--r--   0        0        0    59183 2023-07-05 19:18:15.899796 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/periodic_loop.PNG
--rw-r--r--   0        0        0    17135 2023-07-05 19:18:15.899938 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/rectangle_cross_section.png
--rw-r--r--   0        0        0    17732 2023-07-05 19:18:15.900074 pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/rectangle_cross_section_fillet.png
--rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 pyturbo_aero-1.0.3/setup.py
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 pyturbo_aero-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      557 2023-07-08 00:52:29.969025 pyturbo_aero-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-07-05 19:18:15.890587 pyturbo_aero-1.0.4/pyturbo/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-05 19:18:15.890674 pyturbo_aero-1.0.4/pyturbo/aero/__init__.py
+-rw-r--r--   0        0        0    45020 2023-07-07 20:13:40.408916 pyturbo_aero-1.0.4/pyturbo/aero/airfoil2D.py
+-rw-r--r--   0        0        0    67220 2023-07-08 01:18:15.603440 pyturbo_aero-1.0.4/pyturbo/aero/airfoil3D.py
+-rw-r--r--   0        0        0    34367 2023-07-05 19:18:15.891285 pyturbo_aero-1.0.4/pyturbo/aero/airfoil_wavy.py
+-rw-r--r--   0        0        0    18449 2023-07-05 19:18:15.891395 pyturbo_aero-1.0.4/pyturbo/aero/passage2D.py
+-rw-r--r--   0        0        0      742 2023-07-05 19:18:15.891510 pyturbo_aero-1.0.4/pyturbo/helper/__init__.py
+-rw-r--r--   0        0        0     2520 2023-07-05 19:18:15.891580 pyturbo_aero-1.0.4/pyturbo/helper/arc.py
+-rw-r--r--   0        0        0    16034 2023-07-08 01:35:31.999382 pyturbo_aero-1.0.4/pyturbo/helper/bezier.py
+-rw-r--r--   0        0        0     1295 2023-07-05 19:18:15.891760 pyturbo_aero-1.0.4/pyturbo/helper/bisect.py
+-rw-r--r--   0        0        0      107 2023-07-05 19:18:15.891818 pyturbo_aero-1.0.4/pyturbo/helper/centroid.py
+-rw-r--r--   0        0        0      477 2023-07-05 19:18:15.891878 pyturbo_aero-1.0.4/pyturbo/helper/convert_to_ndarray.py
+-rw-r--r--   0        0        0      490 2023-07-05 19:18:15.891933 pyturbo_aero-1.0.4/pyturbo/helper/csapi.py
+-rw-r--r--   0        0        0      832 2023-07-05 19:18:15.891992 pyturbo_aero-1.0.4/pyturbo/helper/derivative.py
+-rw-r--r--   0        0        0      239 2023-07-05 19:18:15.892049 pyturbo_aero-1.0.4/pyturbo/helper/dist.py
+-rw-r--r--   0        0        0      527 2023-07-05 19:18:15.892110 pyturbo_aero-1.0.4/pyturbo/helper/exp_ratio.py
+-rw-r--r--   0        0        0     9841 2023-07-05 19:18:15.892197 pyturbo_aero-1.0.4/pyturbo/helper/line2D.py
+-rw-r--r--   0        0        0     1068 2023-07-05 19:18:15.892260 pyturbo_aero-1.0.4/pyturbo/helper/min_max_check.py
+-rw-r--r--   0        0        0     9654 2023-07-05 19:18:15.892355 pyturbo_aero-1.0.4/pyturbo/helper/pspline.py
+-rw-r--r--   0        0        0     1542 2023-07-05 19:18:15.892422 pyturbo_aero-1.0.4/pyturbo/helper/ray.py
+-rw-r--r--   0        0        0      505 2023-07-05 19:18:15.892489 pyturbo_aero-1.0.4/pyturbo/helper/rotate_array_values.py
+-rw-r--r--   0        0        0      368 2023-07-05 19:18:15.892555 pyturbo_aero-1.0.4/pyturbo/helper/unique_xy.py
+-rw-r--r--   0        0        0     1873 2023-07-05 19:18:15.892618 pyturbo_aero-1.0.4/pyturbo/helper/wave.py
+-rw-r--r--   0        0        0      500 2023-07-05 19:18:15.892721 pyturbo_aero-1.0.4/pyturbo/ml/gramian_angular_field.py
+-rw-r--r--   0        0        0    37766 2023-07-05 19:18:15.893024 pyturbo_aero-1.0.4/pyturbo/wiki/2D_design/2D_airfoil.png
+-rw-r--r--   0        0        0    23891 2023-07-05 19:18:15.893201 pyturbo_aero-1.0.4/pyturbo/wiki/2D_design/Deriv_2.png
+-rw-r--r--   0        0        0    25329 2023-07-05 19:18:15.893382 pyturbo_aero-1.0.4/pyturbo/wiki/2D_design/camber_line.png
+-rw-r--r--   0        0        0    28623 2023-07-05 19:18:15.893565 pyturbo_aero-1.0.4/pyturbo/wiki/2D_design/s_c.png
+-rw-r--r--   0        0        0    61651 2023-07-05 19:18:15.893934 pyturbo_aero-1.0.4/pyturbo/wiki/3D_design/stator3D_shell.png
+-rw-r--r--   0        0        0   213435 2023-07-05 19:18:15.894939 pyturbo_aero-1.0.4/pyturbo/wiki/3D_design/stator3D_wavy_const_te_radius.PNG
+-rw-r--r--   0        0        0   160990 2023-07-05 19:18:15.895327 pyturbo_aero-1.0.4/pyturbo/wiki/3D_design/stator3D_wavy_variable_te_radius.PNG
+-rw-r--r--   0        0        0   146610 2023-07-05 19:18:15.896025 pyturbo_aero-1.0.4/pyturbo/wiki/3D_design/stator3D_whisker.PNG
+-rw-r--r--   0        0        0   420888 2023-07-05 19:18:15.897914 pyturbo_aero-1.0.4/pyturbo/wiki/3D_design/stator_3D.png
+-rw-r--r--   0        0        0    16958 2023-07-05 19:18:15.898104 pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/circle_cross_section.png
+-rw-r--r--   0        0        0    11380 2023-07-05 19:18:15.898209 pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/pathline_close_loop_no_return.png
+-rw-r--r--   0        0        0    13018 2023-07-05 19:18:15.898311 pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/pathline_close_loop_return.png
+-rw-r--r--   0        0        0    11751 2023-07-05 19:18:15.898407 pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/pathline_periodic_loop.png
+-rw-r--r--   0        0        0   164008 2023-07-05 19:18:15.899158 pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/pattern_close_loop_no_return.PNG
+-rw-r--r--   0        0        0    63687 2023-07-05 19:18:15.899487 pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/pattern_close_loop_return.PNG
+-rw-r--r--   0        0        0    59183 2023-07-05 19:18:15.899796 pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/periodic_loop.PNG
+-rw-r--r--   0        0        0    17135 2023-07-05 19:18:15.899938 pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/rectangle_cross_section.png
+-rw-r--r--   0        0        0    17732 2023-07-05 19:18:15.900074 pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/rectangle_cross_section_fillet.png
+-rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 pyturbo_aero-1.0.4/setup.py
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 pyturbo_aero-1.0.4/PKG-INFO
```

### Comparing `pyturbo_aero-1.0.3/pyproject.toml` & `pyturbo_aero-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyturbo-aero"
-version = "1.0.3"
+version = "1.0.4"
 description = "PyTurbo_Aero is a Turbomachinery blade design library that lets you create a full 3D blades and passages."
 authors = ["Paht Juangphanich <paht.juangphanich@nasa.gov>"]
 packages = [
     { include = "pyturbo" }
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `pyturbo_aero-1.0.3/pyturbo/aero/airfoil2D.py` & `pyturbo_aero-1.0.4/pyturbo/aero/airfoil2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,18 +231,18 @@
         yo = y_wedge_ps-m*(x_wedge_ps-xo)
         
         
         #yo = (y_wedge_ps-m*x_wedge_ps)/(1+m*yc/xc)
         #xo = -yo*yc/xc
         
         # mc = (yo-y_wedge_ps)/(xo-x_wedge_ps) # Check
-        self.psBezierX[-2] = xo # set the last bezier point on the pressure side such that it matches the slope of the TE Arc
-        self.psBezierY[-2] = yo
-        self.psBezierX[-1] = x_wedge_ps
-        self.psBezierY[-1] = y_wedge_ps
+        self.psBezierX[-2] = xo[0] # set the last bezier point on the pressure side such that it matches the slope of the TE Arc
+        self.psBezierY[-2] = yo[0]
+        self.psBezierX[-1] = x_wedge_ps[0]
+        self.psBezierY[-1] = y_wedge_ps[0]
         b = bezier(self.psBezierX,self.psBezierY) # Extends the bezier curve
         self.psBezier = b
         
         # Suction side
         if (int(max(self.t_ss))<1): # in case a camber percent (i.e. 0.7) is set
             t = self.t_ss[-1]
         else:
@@ -265,18 +265,18 @@
         # Compute first derivative on the arc
         [xx,yy] = self.TE_ss_arc.get_point([0,0.01,0.02])
         dydx1 = derivative.derivative_1(xx,yy)
         m = dydx1[0]
         xo = (y_wedge_ss-yc-m*x_wedge_ss+m2*xc)/(m2-m) # interception of the 2nd to last point
         yo = y_wedge_ss-m*(x_wedge_ss-xo)
         # mc = (yo-y_wedge_ss)/(xo-x_wedge_ss) # Check
-        self.ssBezierX[-2] = xo
-        self.ssBezierY[-2] = yo
-        self.ssBezierX[-1] = x_wedge_ss
-        self.ssBezierY[-1] = y_wedge_ss
+        self.ssBezierX[-2] = xo[0]
+        self.ssBezierY[-2] = yo[0]
+        self.ssBezierX[-1] = x_wedge_ss[0]
+        self.ssBezierY[-1] = y_wedge_ss[0]
         b = bezier(self.ssBezierX,self.ssBezierY)
         self.ssBezier = b      
     
     def ss_thickness_add(self,thicknessArray:List[float],camberPercent:float=None,thickness_loc:List[float]=None,expansion_ratio:float=1.2):
         """Adds thickness to the suction side by specifying bezier control points 
 
         Args:
@@ -329,16 +329,16 @@
             if (i>=len(thicknessArray)):
                 self.ssBezierX.append(0)
                 self.ssBezierY.append(0)
             else:
                 t_ray = thicknessArray[i]
                 xn = x-cos(radians(theta))*t_ray
                 yn = y-sin(radians(theta))*t_ray
-                self.ssBezierX.append(xn)
-                self.ssBezierY.append(yn)
+                self.ssBezierX.append(xn[0])
+                self.ssBezierY.append(yn[0])
 
         self.ssBezier = bezier(self.ssBezierX,self.ssBezierY)
 
     # Adds thickness to pressure side
     def ps_thickness_add(self,thicknessArray:List[float],expansion_ratio:float=1.2):
         """Add thickness to the pressure side 
 
@@ -388,16 +388,16 @@
             elif (i>len(thicknessArray)):
                 self.psBezierX.append(0) # These two points are computed
                 self.psBezierY.append(0)
             else:
                 t_ray = thicknessArray[i-1]
                 xn = x+cos(radians(theta))*t_ray
                 yn = y+sin(radians(theta))*t_ray
-                self.psBezierX.append(xn)
-                self.psBezierY.append(yn)
+                self.psBezierX.append(xn[0])
+                self.psBezierY.append(yn[0])
             
         self.psBezier = bezier(self.psBezierX,self.psBezierY)
 
     def add_pitch(self,x_pitch:float):
         """Adds extra pitch by shifting the turbine blade over by a x direction
 
         Args:
```

### Comparing `pyturbo_aero-1.0.3/pyturbo/aero/airfoil3D.py` & `pyturbo_aero-1.0.4/pyturbo/aero/airfoil3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,87 +146,87 @@
         self.te_center_x = np.zeros(len(self.profileArray))
         self.te_center_y = np.zeros(len(self.profileArray))
         if (len(self.profileArray) >= 2):
             # Stack the airfoils about LE
             if (stackType == stack_type.leading_edge):
                 hub = self.profileArray[0]
                 [hx, hy] = hub.camberBezier.get_point(0)
-                self.bezierX.append(hx)
-                self.bezierY.append(hy)
+                self.bezierX.append(hx[0])
+                self.bezierY.append(hy[0])
                 self.bezierZ.append(0)
 
                 [hx_te, hy_te] = hub.camberBezier.get_point(1)
-                self.te_center_x[0] = hx_te
-                self.te_center_y[0] = hy_te
+                self.te_center_x[0] = hx_te[0]
+                self.te_center_y[0] = hy_te[0]
 
                 for i in range(1, len(self.profileArray)):
                     [x, y] = self.profileArray[i].camberBezier.get_point(0)
-                    dx = hx-x
-                    dy = hy-y
+                    dx = hx[0]-x[0]
+                    dy = hy[0]-y[0]
                     # Shift the points based on camber
                     self.profileArray[i].shift(dx, dy)
-                    self.bezierX.append(hx)
-                    self.bezierY.append(hy)
+                    self.bezierX.append(hx[0])
+                    self.bezierY.append(hy[0])
                     self.bezierZ.append(self.profileSpan[i]*self.span)
 
                     [hx_te, hy_te] = self.profileArray[i].camberBezier.get_point(
                         1)
-                    self.te_center_x[i] = hx_te
-                    self.te_center_y[i] = hy_te
+                    self.te_center_x[i] = hx_te[0]
+                    self.te_center_y[i] = hy_te[0]
             # Stack the airfoils about TE
             elif (stackType == stack_type.trailing_edge):
                 hub = self.profileArray[0]
                 [hx, hy] = hub.camberBezier.get_point(1)
-                self.bezierX.append(hx)
-                self.bezierY.append(hy)
+                self.bezierX.append(hx[0])
+                self.bezierY.append(hy[0])
                 self.bezierZ.append(0)
 
                 [hx_te, hy_te] = hub.camberBezier.get_point(1)
-                self.te_center_x[0] = hx_te
-                self.te_center_y[0] = hy_te
+                self.te_center_x[0] = hx_te[0]
+                self.te_center_y[0] = hy_te[0]
 
                 for i in range(1, len(self.profileArray)):
                     [x, y] = self.profileArray[i].camberBezier.get_point(1)
                     dx = 0
                     dy = 0
                     # Shift the points based on camber
                     self.profileArray[i].shift(dx, dy)
-                    self.bezierX.append(hx)
-                    self.bezierY.append(hy)
+                    self.bezierX.append(hx[0])
+                    self.bezierY.append(hy[0])
                     self.bezierZ.append(self.profileSpan[i]*self.span)
 
                     [hx_te, hy_te] = self.profileArray[i].camberBezier.get_point(
                         1)
-                    self.te_center_x[i] = hx_te
-                    self.te_center_y[i] = hy_te
+                    self.te_center_x[i] = hx_te[0]
+                    self.te_center_y[i] = hy_te[0]
 
             elif (stackType == stack_type.centroid):
                 [hx, hy] = self.profileArray[0].get_centroid()
-                self.bezierX.append(hx)
-                self.bezierY.append(hy)
+                self.bezierX.append(hx[0])
+                self.bezierY.append(hy[0])
                 self.bezierZ.append(0)
 
                 [hx_te, hy_te] = self.profileArray[0].camberBezier.get_point(1)
-                self.te_center_x[0] = hx_te
-                self.te_center_y[0] = hy_te
+                self.te_center_x[0] = hx_te[0]
+                self.te_center_y[0] = hy_te[0]
 
                 for i in range(1, len(self.profileArray)):
                     [x, y] = self.profileArray[i].get_centroid()
-                    dx = hx-x
-                    dy = hy-y
+                    dx = hx[0]-x[0]
+                    dy = hy[0]-y[0]
                     # Shift the points based on camber
                     self.profileArray[i].shift(dx, dy)
-                    self.bezierX.append(hx)
-                    self.bezierY.append(hy)
+                    self.bezierX.append(hx[0])
+                    self.bezierY.append(hy[0])
                     self.bezierZ.append(self.profileSpan[i]*self.span)
 
                     [hx_te, hy_te] = self.profileArray[i].camberBezier.get_point(
                         1)
-                    self.te_center_x[i] = hx_te
-                    self.te_center_y[i] = hy_te
+                    self.te_center_x[i] = hx_te[0]
+                    self.te_center_y[i] = hy_te[0]
 
             self.bezierX = convert_to_ndarray(self.bezierX)
             self.bezierY = convert_to_ndarray(self.bezierY)
             self.bezierZ = convert_to_ndarray(self.bezierZ)
             self.b3 = bezier3(self.bezierX,self.bezierY,self.bezierZ)
             self.bImportedBlade = False
 
@@ -244,32 +244,32 @@
         self.sweepZ = self.sweepZ*self.span
         [_,ind_com1,ind_com2] = np.intersect1d(self.bezierZ, self.sweepZ,return_indices=True)        
         self.bezierY[ind_com1] = self.bezierY[ind_com1] + self.sweepY[ind_com2]*self.span
 
 
         # add sweep where z does not exist 
         i1 = np.setxor1d(self.sweepZ, self.bezierZ) # tells what items in leanZ do not exist in bezierZ
-        i1 = np.where(self.sweepZ == i1) # get the index
-        self.bezierZ = np.append(self.bezierZ, self.sweepZ[i1])
-        self.bezierY = np.append(self.bezierY, self.sweepY[i1]*self.span+self.bezierY[0])
-        xx = self.sweepZ; xx[i1] = self.bezierX[0]
-        self.bezierX = np.append(self.bezierX, xx[i1])
-
+        if i1.size >0:
+            i1 = np.where(self.sweepZ == i1) # get the index
+            self.bezierZ = np.append(self.bezierZ, self.sweepZ[i1])
+            self.bezierY = np.append(self.bezierY, self.sweepY[i1]*self.span+self.bezierY[0])
+            xx = self.sweepZ; xx[i1] = self.bezierX[0]
+            self.bezierX = np.append(self.bezierX, xx[i1])
 
         # SORT
         # A = sortrows([self.bezierZ' self.bezierX' self.bezierY'])
         indx = np.argsort(self.bezierZ)
         self.bezierZ = self.bezierZ[indx]
         self.bezierX = self.bezierX[indx]
         self.bezierY = self.bezierY[indx]
 
         if (self.bImportedBlade): # imported blade doesn't have 2D airfoil profiles defined, just points
             self.profiles_shift()
 
-    def lean_add(self,leanX:List[float],leanZ:List[float]):
+    def lean(self,leanX:List[float],leanZ:List[float]):
         """Leans the blade towards the suction or pressure side. This applies points that are fitted by a bezier curve. Profiles are adjusted to follow this curve simulating lean.
 
         Args:
             leanX (List[float]): lean points 
             leanZ (List[float]): spanwise location of the lean points
         """
         leanX = convert_to_ndarray(leanX)
@@ -282,19 +282,20 @@
         # Add lean where z exists, basically adds more lean 
         [_,ind_com1,ind_com2] = np.intersect1d(self.bezierZ,leanZ,return_indices=True)
         self.bezierX[ind_com1] = self.bezierX[ind_com1]+leanX[ind_com2]*self.span
 
         #  Add Lean where Z does not exist
         # [~,i1] = setxor(leanZ,self.bezierZ); %  MATLAB CODE tells what items in leanZ do not exist in bezierZ
         i1 = np.setxor1d(leanZ,self.bezierZ)
-        i1 = np.where(leanZ == i1) # get the index
-        self.bezierZ = np.append(self.bezierZ, leanZ[i1])
-        self.bezierX = np.append(self.bezierX, self.leanX[i1]*self.span+self.bezierX[0])
-        yy = leanZ; yy[i1] = self.bezierY[0] #TODO Need to check this
-        self.bezierY = np.append(self.bezierY, yy[i1])
+        if i1.size >0:
+            i1 = np.where(leanZ == i1) # get the index
+            self.bezierZ = np.append(self.bezierZ, leanZ[i1])
+            self.bezierX = np.append(self.bezierX, self.leanX[i1]*self.span+self.bezierX[0])
+            yy = leanZ; yy[i1] = self.bezierY[0] #TODO Need to check this
+            self.bezierY = np.append(self.bezierY, yy[i1])
 
         # Sort
         indx = np.argsort(self.bezierZ)
         self.bezierZ = self.bezierZ[indx]
         self.bezierX = self.bezierX[indx]
         self.bezierY = self.bezierY[indx]
         
@@ -342,16 +343,16 @@
         # --- Make a spline for each profile for each point
         # new code below
         # tmpXps = np.zeros((self.npts,n_profiles)); tmpYps = np.zeros((self.npts,n_profiles))
         # tmpXss = np.zeros((self.npts,n_profiles)); tmpYss = np.zeros((self.npts,n_profiles))
         for j in range(n_profiles):
             # [tmpXps[:,j], tmpYps[:,j]] = self.profileArray[j]._psBezier.get_point(t)
             # [tmpXss[:,j], tmpYss[:,j]] = self.profileArray[j]._ssBezier.get_point(t)
-            [self.spline_xpps[:,j], self.spline_ypps[:,j]] = self.profileArray[j]._psBezier.get_point(t,equal_space=True)
-            [self.spline_xpss[:,j], self.spline_ypss[:,j]] = self.profileArray[j]._ssBezier.get_point(t,equal_space=True)
+            [self.spline_xpps[:,j], self.spline_ypps[:,j]] = self.profileArray[j].psBezier.get_point(t,equal_space=True)
+            [self.spline_xpss[:,j], self.spline_ypss[:,j]] = self.profileArray[j].ssBezier.get_point(t,equal_space=True)
             self.spline_zpp[:,j] = self.profileSpan[j]*self.span              # Span
         
             
         for i in range(self.npts): 
             self.xps[:,i]= csapi(self.spline_zpp[i,:],self.spline_xpps[i,:],self.zz) # Natural spline
             self.yps[:,i]= csapi(self.spline_zpp[i,:],self.spline_ypps[i,:],self.zz)
             
@@ -386,16 +387,16 @@
         self.control_y_ss = np.zeros((self.npts,n_profiles))
         self.c_te_x_ps = np.zeros((self.nte,n_profiles))
         self.c_te_x_ss = np.zeros((self.nte,n_profiles))
         self.c_te_y_ps = np.zeros((self.nte,n_profiles))
         self.c_te_y_ss = np.zeros((self.nte,n_profiles))
         
         for i in range(n_profiles):                
-            [self.control_x_ps[:,i], self.control_y_ps[:,i]] = self.profileArray[i]._psBezier.get_point(t)
-            [self.control_x_ss[:,i], self.control_y_ss[:,i]] = self.profileArray[i]._ssBezier.get_point(t)
+            [self.control_x_ps[:,i], self.control_y_ps[:,i]] = self.profileArray[i].psBezier.get_point(t)
+            [self.control_x_ss[:,i], self.control_y_ss[:,i]] = self.profileArray[i].ssBezier.get_point(t)
             # add trailing edge
             [self.c_te_x_ps[:,i], self.c_te_y_ps[:,i]] = self.profileArray[i].TE_ps_arc.get_point(t_te)
             [self.c_te_x_ss[:,i], self.c_te_y_ss[:,i]] = self.profileArray[i].TE_ss_arc.get_point(t_te)
 
         # Shift all the generated turbine profiles points based on the bezier curve
         self.profiles_shift()
```

### Comparing `pyturbo_aero-1.0.3/pyturbo/aero/airfoil_wavy.py` & `pyturbo_aero-1.0.4/pyturbo/aero/airfoil_wavy.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/aero/passage2D.py` & `pyturbo_aero-1.0.4/pyturbo/aero/passage2D.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/__init__.py` & `pyturbo_aero-1.0.4/pyturbo/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/arc.py` & `pyturbo_aero-1.0.4/pyturbo/helper/arc.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/bezier.py` & `pyturbo_aero-1.0.4/pyturbo/helper/bezier.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                 u = self.c[j]*pow(1-t[i], self.n-j-1)*pow(t[i],j)
                 tempx += u*self.x[j]
                 tempy += u*self.y[j]
                 
             Bx[i],By[i] = tempx,tempy
 
         if (equal_space and len(Bx)>2):
-            Bx,By = self.equal_space(t,Bx,By)
+            Bx,By = self.__equal_space__(t,Bx,By)
             return Bx,By
         return Bx,By
 
     def plot2D(self,equal_space=False):
         """Creates a 2D Plot of a bezier curve 
 
         Args:
```

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/bisect.py` & `pyturbo_aero-1.0.4/pyturbo/helper/bisect.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/derivative.py` & `pyturbo_aero-1.0.4/pyturbo/helper/derivative.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/exp_ratio.py` & `pyturbo_aero-1.0.4/pyturbo/helper/exp_ratio.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/line2D.py` & `pyturbo_aero-1.0.4/pyturbo/helper/line2D.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/min_max_check.py` & `pyturbo_aero-1.0.4/pyturbo/helper/min_max_check.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/pspline.py` & `pyturbo_aero-1.0.4/pyturbo/helper/pspline.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/ray.py` & `pyturbo_aero-1.0.4/pyturbo/helper/ray.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/helper/wave.py` & `pyturbo_aero-1.0.4/pyturbo/helper/wave.py`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/2D_airfoil.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/2D_design/2D_airfoil.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/Deriv_2.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/2D_design/Deriv_2.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/camber_line.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/2D_design/camber_line.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/2D_design/s_c.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/2D_design/s_c.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_shell.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/3D_design/stator3D_shell.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_wavy_const_te_radius.PNG` & `pyturbo_aero-1.0.4/pyturbo/wiki/3D_design/stator3D_wavy_const_te_radius.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_wavy_variable_te_radius.PNG` & `pyturbo_aero-1.0.4/pyturbo/wiki/3D_design/stator3D_wavy_variable_te_radius.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator3D_whisker.PNG` & `pyturbo_aero-1.0.4/pyturbo/wiki/3D_design/stator3D_whisker.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/3D_design/stator_3D.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/3D_design/stator_3D.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/circle_cross_section.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/circle_cross_section.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_close_loop_no_return.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/pathline_close_loop_no_return.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_close_loop_return.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/pathline_close_loop_return.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pathline_periodic_loop.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/pathline_periodic_loop.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pattern_close_loop_no_return.PNG` & `pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/pattern_close_loop_no_return.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/pattern_close_loop_return.PNG` & `pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/pattern_close_loop_return.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/periodic_loop.PNG` & `pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/periodic_loop.PNG`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/rectangle_cross_section.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/rectangle_cross_section.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/pyturbo/wiki/HeatPipe/rectangle_cross_section_fillet.png` & `pyturbo_aero-1.0.4/pyturbo/wiki/HeatPipe/rectangle_cross_section_fillet.png`

 * *Files identical despite different names*

### Comparing `pyturbo_aero-1.0.3/setup.py` & `pyturbo_aero-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'pandas>=1.4',
  'plotly',
  'scipy>1.8.0',
  'tqdm']
 
 setup_kwargs = {
     'name': 'pyturbo-aero',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'PyTurbo_Aero is a Turbomachinery blade design library that lets you create a full 3D blades and passages.',
     'long_description': 'None',
     'author': 'Paht Juangphanich',
     'author_email': 'paht.juangphanich@nasa.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pyturbo_aero-1.0.3/PKG-INFO` & `pyturbo_aero-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyturbo-aero
-Version: 1.0.3
+Version: 1.0.4
 Summary: PyTurbo_Aero is a Turbomachinery blade design library that lets you create a full 3D blades and passages.
 Author: Paht Juangphanich
 Author-email: paht.juangphanich@nasa.gov
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

