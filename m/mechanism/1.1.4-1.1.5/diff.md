# Comparing `tmp/mechanism-1.1.4.tar.gz` & `tmp/mechanism-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanism-1.1.4.tar", last modified: Mon Jan 23 14:49:53 2023, max compression
+gzip compressed data, was "mechanism-1.1.5.tar", last modified: Sat Jul  8 19:47:29 2023, max compression
```

## Comparing `mechanism-1.1.4.tar` & `mechanism-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-01-23 14:49:53.744456 mechanism-1.1.4/
--rw-rw-rw-   0        0        0       26 2021-12-25 06:04:05.000000 mechanism-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0    19899 2023-01-23 14:49:53.743320 mechanism-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2021-12-25 03:35:22.000000 mechanism-1.1.4/license.txt
-drwxrwxrwx   0        0        0        0 2023-01-23 14:49:53.732891 mechanism-1.1.4/mechanism/
--rw-rw-rw-   0        0        0      779 2022-01-05 05:07:15.000000 mechanism-1.1.4/mechanism/__init__.py
--rw-rw-rw-   0        0        0     1980 2022-07-30 00:19:18.000000 mechanism-1.1.4/mechanism/appearance.json
--rw-rw-rw-   0        0        0    34067 2022-06-29 00:33:58.000000 mechanism-1.1.4/mechanism/cams.py
--rw-rw-rw-   0        0        0     7559 2021-09-30 00:43:13.000000 mechanism-1.1.4/mechanism/dataframe.py
--rw-rw-rw-   0        0        0    15503 2023-01-23 14:43:13.000000 mechanism-1.1.4/mechanism/gears.py
--rw-rw-rw-   0        0        0    40580 2022-10-28 23:38:16.000000 mechanism-1.1.4/mechanism/mechanism.py
--rw-rw-rw-   0        0        0     1971 2022-07-30 00:26:42.000000 mechanism-1.1.4/mechanism/player.py
--rw-rw-rw-   0        0        0    12646 2022-06-29 00:01:19.000000 mechanism-1.1.4/mechanism/vectors.py
-drwxrwxrwx   0        0        0        0 2023-01-23 14:49:53.741508 mechanism-1.1.4/mechanism.egg-info/
--rw-rw-rw-   0        0        0    19899 2023-01-23 14:49:53.000000 mechanism-1.1.4/mechanism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-01-23 14:49:53.000000 mechanism-1.1.4/mechanism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-23 14:49:53.000000 mechanism-1.1.4/mechanism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-01-23 14:49:53.000000 mechanism-1.1.4/mechanism.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-23 14:49:53.000000 mechanism-1.1.4/mechanism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-23 14:49:53.744456 mechanism-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1343 2023-01-23 14:43:13.000000 mechanism-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 19:47:29.018834 mechanism-1.1.5/
+-rw-rw-rw-   0        0        0       26 2021-12-25 06:04:05.000000 mechanism-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    19899 2023-07-08 19:47:29.018834 mechanism-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2021-12-25 03:35:22.000000 mechanism-1.1.5/license.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 19:47:29.003208 mechanism-1.1.5/mechanism/
+-rw-rw-rw-   0        0        0      779 2022-01-05 05:07:15.000000 mechanism-1.1.5/mechanism/__init__.py
+-rw-rw-rw-   0        0        0     1980 2022-07-30 00:19:18.000000 mechanism-1.1.5/mechanism/appearance.json
+-rw-rw-rw-   0        0        0    34067 2022-06-29 00:33:58.000000 mechanism-1.1.5/mechanism/cams.py
+-rw-rw-rw-   0        0        0     7559 2021-09-30 00:43:13.000000 mechanism-1.1.5/mechanism/dataframe.py
+-rw-rw-rw-   0        0        0    15503 2023-01-23 14:43:13.000000 mechanism-1.1.5/mechanism/gears.py
+-rw-rw-rw-   0        0        0    41243 2023-07-05 14:04:54.000000 mechanism-1.1.5/mechanism/mechanism.py
+-rw-rw-rw-   0        0        0     1971 2022-07-30 00:26:42.000000 mechanism-1.1.5/mechanism/player.py
+-rw-rw-rw-   0        0        0    12646 2022-06-29 00:01:19.000000 mechanism-1.1.5/mechanism/vectors.py
+drwxrwxrwx   0        0        0        0 2023-07-08 19:47:29.018834 mechanism-1.1.5/mechanism.egg-info/
+-rw-rw-rw-   0        0        0    19899 2023-07-08 19:47:28.000000 mechanism-1.1.5/mechanism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-07-08 19:47:28.000000 mechanism-1.1.5/mechanism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 19:47:28.000000 mechanism-1.1.5/mechanism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 19:47:28.000000 mechanism-1.1.5/mechanism.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 19:47:28.000000 mechanism-1.1.5/mechanism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 19:47:29.018834 mechanism-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2023-07-08 19:42:00.000000 mechanism-1.1.5/setup.py
```

### Comparing `mechanism-1.1.4/PKG-INFO` & `mechanism-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanism
-Version: 1.1.4
+Version: 1.1.5
 Summary: A package that provides a kinematic analysis of mechanisms and cams and custom tooth profile for spur gears.
 Home-page: https://github.com/gabemorris12/mechanism
 Author: Gabe Morris
 Author-email: gabemorris1231@gmail.com
 License: MIT
 Keywords: mechanism,kinematic,cams,linkages,analysis,animations
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mechanism-1.1.4/license.txt` & `mechanism-1.1.5/license.txt`

 * *Files identical despite different names*

### Comparing `mechanism-1.1.4/mechanism/__init__.py` & `mechanism-1.1.5/mechanism/__init__.py`

 * *Files identical despite different names*

### Comparing `mechanism-1.1.4/mechanism/appearance.json` & `mechanism-1.1.5/mechanism/appearance.json`

 * *Files identical despite different names*

### Comparing `mechanism-1.1.4/mechanism/cams.py` & `mechanism-1.1.5/mechanism/cams.py`

 * *Files identical despite different names*

### Comparing `mechanism-1.1.4/mechanism/dataframe.py` & `mechanism-1.1.5/mechanism/dataframe.py`

 * *Files identical despite different names*

### Comparing `mechanism-1.1.4/mechanism/gears.py` & `mechanism-1.1.5/mechanism/gears.py`

 * *Files identical despite different names*

### Comparing `mechanism-1.1.4/mechanism/mechanism.py` & `mechanism-1.1.5/mechanism/mechanism.py`

 * *Files 1% similar despite different names*

```diff
@@ -785,27 +785,28 @@
         x_max = np.amax(x_positions)
         y_min = np.amin(y_positions)
         y_max = np.amax(y_positions)
 
         return (x_min, x_max), (y_min, y_max)
 
     def get_animation(self, velocity=False, acceleration=False, scale=0.1, stamp=None, stamp_loc=(0.05, 0.9),
-                      grid=True, cushion=1):
+                      grid=True, cushion=1, show_joints=False):
         """
         :param velocity: bool; Plots velocity vectors if True
         :param acceleration: bool; Plots acceleration vectors if True
         :param scale: float; If velocity or acceleration is specified, the scale will define the relative length of the
                       maximum magnitude to the diagonal of the bounding box. A scale of 0.1 (default) would indicate
                       that the maximum magnitude of the velocity/acceleration is 1/10 the diagonal of the bounding box.
         :param stamp: np.ndarray; Shows a text stamp in the animation for displaying any kind of input. Must be the same
                       size as the input and correspond to the input motion.
         :param stamp_loc: tuple; Position of the stamp in axes transform units. A location of (0.5, 0.75) would place
                           the stamp 50% along the x direction and 75% along the y direction.
         :param grid: bool; Add the grid if true.
         :param cushion: int, float; Add a cushion around the plot.
+        :param show_joints: bool; Show joint names if true.
         :return: An animation, figure, and axes object.
         """
         fig, ax = plt.subplots()
         ax.set_aspect('equal')
         x_limits, y_limits = self.get_bounds()
 
         vel_arrow_patches, acc_arrow_patches = [], []
@@ -842,19 +843,23 @@
         else:
             x_min, x_max = x_limits
             y_min, y_max = y_limits
         ax.set_xlim(x_min - cushion, x_max + cushion)
         ax.set_ylim(y_min - cushion, y_max + cushion)
 
         plot_dict = {}
+        joints = {}
         for v in self.vectors:
             if not v.pos.show:
                 continue
 
             plot_dict.update({v.pos: ax.plot([], [], **v.pos.kwargs)[0]})
+            if show_joints:
+                for j in v.joints:
+                    joints.update({j: ax.text(x=0.0, y=0.0, s=j.name, visible=False, zorder=5)})
 
         for j in self.joints:
             if j.follow:
                 ax.plot(j.x_positions, j.y_positions, **j.kwargs)
 
         text_list = []
         if stamp is not None:
@@ -862,37 +867,43 @@
             text = ax.text(stamp_loc[0], stamp_loc[1], '', transform=ax.transAxes,
                            bbox=dict(facecolor='white', edgecolor='white'), zorder=6)
             text_list.append(text)
 
         def init():
             for line in plot_dict.values():
                 line.set_data([], [])
+            for j_ in joints.values():
+                j_.set(visible=True)
             for arrow in vel_arrow_patches:
                 arrow.set_positions(posA=(0, 0), posB=(0, 0))
             for arrow in acc_arrow_patches:
                 arrow.set_positions(posA=(0, 0), posB=(0, 0))
             if text_list:
                 text.set_text('')
-            return list(plot_dict.values()) + vel_arrow_patches + acc_arrow_patches + text_list
+            return list(plot_dict.values()) + vel_arrow_patches + acc_arrow_patches + text_list + list(joints.values())
 
         def animate(i):
             for vec, line in plot_dict.items():
                 j1, j2 = vec.joints
                 line.set_data((j1.x_positions[i], j2.x_positions[i]), (j1.y_positions[i], j2.y_positions[i]))
+                if show_joints:
+                    offset = 0.2
+                    joints[j1].set_position((j1.x_positions[i] + offset, j1.y_positions[i] + offset))
+                    joints[j2].set_position((j2.x_positions[i] + offset, j2.y_positions[i] + offset))
             if velocity:
                 for joint, arrow in zip(self.joints, vel_arrow_patches):
                     x_head, y_head = np.real(joint._vel_heads)[i], np.imag(joint._vel_heads)[i]
                     arrow.set_positions(posA=(joint.x_positions[i], joint.y_positions[i]), posB=(x_head, y_head))
             if acceleration:
                 for joint, arrow in zip(self.joints, acc_arrow_patches):
                     x_head, y_head = np.real(joint._acc_heads)[i], np.imag(joint._acc_heads)[i]
                     arrow.set_positions(posA=(joint.x_positions[i], joint.y_positions[i]), posB=(x_head, y_head))
             if text_list:
                 text.set_text(f'{stamp[i]:.3f}')
-            return list(plot_dict.values()) + vel_arrow_patches + acc_arrow_patches + text_list
+            return list(plot_dict.values()) + vel_arrow_patches + acc_arrow_patches + text_list + list(joints.values())
 
         # noinspection PyTypeChecker
         ani = Player(fig, animate, frames=self.pos.shape[0], interval=50, blit=True, init_func=init)
 
         return ani, fig, ax
 
     def __getitem__(self, item):
```

### Comparing `mechanism-1.1.4/mechanism/player.py` & `mechanism-1.1.5/mechanism/player.py`

 * *Files identical despite different names*

### Comparing `mechanism-1.1.4/mechanism/vectors.py` & `mechanism-1.1.5/mechanism/vectors.py`

 * *Files identical despite different names*

### Comparing `mechanism-1.1.4/mechanism.egg-info/PKG-INFO` & `mechanism-1.1.5/mechanism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanism
-Version: 1.1.4
+Version: 1.1.5
 Summary: A package that provides a kinematic analysis of mechanisms and cams and custom tooth profile for spur gears.
 Home-page: https://github.com/gabemorris12/mechanism
 Author: Gabe Morris
 Author-email: gabemorris1231@gmail.com
 License: MIT
 Keywords: mechanism,kinematic,cams,linkages,analysis,animations
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mechanism-1.1.4/setup.py` & `mechanism-1.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 THIS_DIR = r'C:\Users\gmbra\Downloads\Python Programs\mechanism'
 
-VERSION = '1.1.4'
+VERSION = '1.1.5'
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'License :: OSI Approved :: MIT License',
     'Operating System :: Microsoft :: Windows',
     'Programming Language :: Python :: 3.10'
 ]
```

