# Comparing `tmp/opsvis-1.0.9.tar.gz` & `tmp/opsvis-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsvis-1.0.9.tar", last modified: Thu Jun 16 17:33:55 2022, max compression
+gzip compressed data, was "opsvis-1.1.1.tar", last modified: Sat Jul  8 09:04:17 2023, max compression
```

## Comparing `opsvis-1.0.9.tar` & `opsvis-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sewi      (1000) sewi      (1000)        0 2022-06-16 17:33:55.894154 opsvis-1.0.9/
--rw-r--r--   0 sewi      (1000) sewi      (1000)    35149 2020-08-24 10:31:43.000000 opsvis-1.0.9/LICENSE
--rw-r--r--   0 sewi      (1000) sewi      (1000)     1006 2022-06-16 17:33:55.894154 opsvis-1.0.9/PKG-INFO
--rw-r--r--   0 sewi      (1000) sewi      (1000)      477 2021-09-28 08:54:43.000000 opsvis-1.0.9/README.md
-drwxr-xr-x   0 sewi      (1000) sewi      (1000)        0 2022-06-16 17:33:55.894154 opsvis-1.0.9/opsvis/
--rw-r--r--   0 sewi      (1000) sewi      (1000)      277 2022-04-09 09:24:42.000000 opsvis-1.0.9/opsvis/__init__.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    20830 2022-06-16 17:31:41.000000 opsvis-1.0.9/opsvis/anim.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    40345 2022-06-16 17:31:41.000000 opsvis-1.0.9/opsvis/defo.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)     8441 2022-06-16 17:31:41.000000 opsvis-1.0.9/opsvis/fibsec.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)      195 2022-06-16 17:31:41.000000 opsvis-1.0.9/opsvis/importing_modules.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    65880 2022-06-16 17:31:41.000000 opsvis-1.0.9/opsvis/model.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    23625 2022-06-16 17:31:41.000000 opsvis-1.0.9/opsvis/secforces.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)     3930 2022-06-16 17:31:41.000000 opsvis-1.0.9/opsvis/settings.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    34720 2022-06-16 17:31:41.000000 opsvis-1.0.9/opsvis/stress.py
-drwxr-xr-x   0 sewi      (1000) sewi      (1000)        0 2022-06-16 17:33:55.894154 opsvis-1.0.9/opsvis.egg-info/
--rw-r--r--   0 sewi      (1000) sewi      (1000)     1006 2022-06-16 17:33:55.000000 opsvis-1.0.9/opsvis.egg-info/PKG-INFO
--rw-r--r--   0 sewi      (1000) sewi      (1000)      357 2022-06-16 17:33:55.000000 opsvis-1.0.9/opsvis.egg-info/SOURCES.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)        1 2022-06-16 17:33:55.000000 opsvis-1.0.9/opsvis.egg-info/dependency_links.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)       11 2022-06-16 17:33:55.000000 opsvis-1.0.9/opsvis.egg-info/requires.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)        7 2022-06-16 17:33:55.000000 opsvis-1.0.9/opsvis.egg-info/top_level.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)      104 2021-09-23 09:12:02.000000 opsvis-1.0.9/pyproject.toml
--rw-r--r--   0 sewi      (1000) sewi      (1000)      668 2022-06-16 17:33:55.894154 opsvis-1.0.9/setup.cfg
+drwxr-xr-x   0 sewi      (1000) sewi      (1000)        0 2023-07-08 09:04:17.084185 opsvis-1.1.1/
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    35149 2020-08-24 10:31:43.000000 opsvis-1.1.1/LICENSE
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     1042 2023-07-08 09:04:17.084185 opsvis-1.1.1/PKG-INFO
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      477 2021-09-28 08:54:43.000000 opsvis-1.1.1/README.md
+drwxr-xr-x   0 sewi      (1000) sewi      (1000)        0 2023-07-08 09:04:17.084185 opsvis-1.1.1/opsvis/
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      154 2023-05-13 19:50:46.000000 opsvis-1.1.1/opsvis/__init__.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    20912 2023-05-14 06:27:30.000000 opsvis-1.1.1/opsvis/anim.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    46210 2023-05-13 20:08:22.000000 opsvis-1.1.1/opsvis/defo.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     9106 2023-05-13 20:08:22.000000 opsvis-1.1.1/opsvis/fibsec.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      195 2023-05-13 20:08:21.000000 opsvis-1.1.1/opsvis/importing_modules.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    72650 2023-05-13 20:08:22.000000 opsvis-1.1.1/opsvis/model.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    29592 2023-07-08 08:59:53.000000 opsvis-1.1.1/opsvis/secforces.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     4529 2023-05-13 20:08:21.000000 opsvis-1.1.1/opsvis/settings.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    34781 2023-05-13 20:08:22.000000 opsvis-1.1.1/opsvis/stress.py
+drwxr-xr-x   0 sewi      (1000) sewi      (1000)        0 2023-07-08 09:04:17.084185 opsvis-1.1.1/opsvis.egg-info/
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     1042 2023-07-08 09:04:17.000000 opsvis-1.1.1/opsvis.egg-info/PKG-INFO
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      357 2023-07-08 09:04:17.000000 opsvis-1.1.1/opsvis.egg-info/SOURCES.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)        1 2023-07-08 09:04:17.000000 opsvis-1.1.1/opsvis.egg-info/dependency_links.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)       11 2023-07-08 09:04:17.000000 opsvis-1.1.1/opsvis.egg-info/requires.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)        7 2023-07-08 09:04:17.000000 opsvis-1.1.1/opsvis.egg-info/top_level.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      104 2021-09-23 09:12:02.000000 opsvis-1.1.1/pyproject.toml
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      704 2023-07-08 09:04:17.088185 opsvis-1.1.1/setup.cfg
```

### Comparing `opsvis-1.0.9/LICENSE` & `opsvis-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opsvis-1.0.9/PKG-INFO` & `opsvis-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: opsvis
-Version: 1.0.9
+Version: 1.1.1
 Summary: OpenSeesPy (OpenSees) Python postprocessing and visualization module
 Home-page: https://github.com/sewkokot/opsvis
 Author: Seweryn Kokot
 Author-email: sewkokot@gmail.com
 Project-URL: Bug Tracker, https://github.com/sewkokot/opsvis/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # opsvis
```

### Comparing `opsvis-1.0.9/opsvis/anim.py` & `opsvis-1.1.1/opsvis/anim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import openseespy.opensees as ops
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation
 
-from settings import *
-from defo import *
+from .settings import *
+from .defo import *
 
 
 def _anim_mode_2d(modeNo, sfac, nep, unDefoFlag, fmt_defo, fmt_undefo,
                   interpFlag, endDispFlag, fig_wi_he,
                   fig_lbrt, xlim, ylim, ax):
 
     if not ax:
@@ -68,58 +68,58 @@
 
             # fig, ax = plt.subplots(figsize=(fig_wi/2.54, fig_he/2.54))
             ax.axis('equal')
             ax.set_xlim(xlim[0], xlim[1])
             ax.set_ylim(ylim[0], ylim[1])
 
             nel = len(ele_tags)
-            Ex = np.zeros((nel, 2))
-            Ey = np.zeros((nel, 2))
+            Ecrd = np.zeros((nel, 2, 2))
+            # Ex = np.zeros((nel, 2))
+            # Ey = np.zeros((nel, 2))
             Ed = np.zeros((nel, 6))
             # time vector for one cycle (period)
             n_cycles = 10
             n_frames = n_cycles * 32 + 1
             t = np.linspace(0., n_cycles*2*np.pi, n_frames)
             lines = []
 
             for i, ele_tag in enumerate(ele_tags):
-                nd1, nd2 = ops.eleNodes(ele_tag)
+                ele_node_tags = ops.eleNodes(ele_tag)
+
+                for j, ele_node_tag in enumerate(ele_node_tags):
+                    Ecrd[i, j, :] = ops.nodeCoord(ele_node_tag)
 
+                # nd1, nd2 = ops.eleNodes(ele_tag)
                 # element x, y coordinates
-                Ex[i, :] = np.array([ops.nodeCoord(nd1)[0],
-                                     ops.nodeCoord(nd2)[0]])
-                Ey[i, :] = np.array([ops.nodeCoord(nd1)[1],
-                                     ops.nodeCoord(nd2)[1]])
-
-                Ed[i, :] = np.array([ops.nodeEigenvector(nd1, modeNo)[0],
-                                     ops.nodeEigenvector(nd1, modeNo)[1],
-                                     ops.nodeEigenvector(nd1, modeNo)[2],
-                                     ops.nodeEigenvector(nd2, modeNo)[0],
-                                     ops.nodeEigenvector(nd2, modeNo)[1],
-                                     ops.nodeEigenvector(nd2, modeNo)[2]])
+                # Ex[i, :] = np.array([ops.nodeCoord(nd1)[0],
+                #                      ops.nodeCoord(nd2)[0]])
+                # Ey[i, :] = np.array([ops.nodeCoord(nd1)[1],
+                #                      ops.nodeCoord(nd2)[1]])
+
+                Ed[i, :] = np.array([*ops.nodeEigenvector(ele_node_tags[0], modeNo)[:3],
+                                     *ops.nodeEigenvector(ele_node_tags[1], modeNo)[:3]])
 
                 lines.append(ax.plot([], [], **fmt_defo)[0])
 
             def init():
                 for j, ele_tag in enumerate(ele_tags):
                     lines[j].set_data([], [])
                 return lines
 
             def animate(i):
                 for j, ele_tag in enumerate(ele_tags):
 
                     if interpFlag:
-                        xcdi, ycdi = beam_defo_interp_2d(Ex[j, :],
-                                                         Ey[j, :],
+                        xcdi, ycdi = beam_defo_interp_2d(Ecrd[j, :, :],
                                                          Ed[j, :],
                                                          sfac*np.sin(t[i]),
                                                          nep)
                         lines[j].set_data(xcdi, ycdi)
                     else:
-                        xdi, ydi = beam_disp_ends(Ex[j, :], Ey[j, :], Ed[j, :],
+                        xdi, ydi = beam_disp_ends(Ecrd[j, :, :], Ed[j, :],
                                                   sfac*np.cos(t[i]))
                         lines[j].set_data(xdi, ydi)
 
                     # plt.plot(xcdi, ycdi, **fmt_defo)
 
                 return lines
 
@@ -381,30 +381,35 @@
 
             ax.axis('equal')
             ax.set_xlim(xlim[0], xlim[1])
             ax.set_ylim(ylim[0], ylim[1])
             # ax.grid()
 
             nel = len(ele_tags)
-            Ex = np.zeros((nel, 2))
-            Ey = np.zeros((nel, 2))
+            Ecrd = np.zeros((nel, 2, 2))
+            # Ex = np.zeros((nel, 2))
+            # Ey = np.zeros((nel, 2))
             # no of frames equal to time intervals
             n_frames, _, _ = np.shape(Eds)
             lines = []
 
             # time_text = ax.set_title('')  # does not work
             time_text = ax.text(.05, .95, '', transform=ax.transAxes)
             for i, ele_tag in enumerate(ele_tags):
-                nd1, nd2 = ops.eleNodes(ele_tag)
+                ele_node_tags = ops.eleNodes(ele_tag)
 
-                # element x, y coordinates
-                Ex[i, :] = np.array([ops.nodeCoord(nd1)[0],
-                                     ops.nodeCoord(nd2)[0]])
-                Ey[i, :] = np.array([ops.nodeCoord(nd1)[1],
-                                     ops.nodeCoord(nd2)[1]])
+                for j, ele_node_tag in enumerate(ele_node_tags):
+                    Ecrd[i, j, :] = ops.nodeCoord(ele_node_tag)
+                # nd1, nd2 = ops.eleNodes(ele_tag)
+
+                # # element x, y coordinates
+                # Ex[i, :] = np.array([ops.nodeCoord(nd1)[0],
+                #                      ops.nodeCoord(nd2)[0]])
+                # Ey[i, :] = np.array([ops.nodeCoord(nd1)[1],
+                #                      ops.nodeCoord(nd2)[1]])
 
                 lines.append(ax.plot([], [], **fmt_defo)[0])
 
             def init():
                 for j, ele_tag in enumerate(ele_tags):
                     lines[j].set_data([], [])
 
@@ -412,22 +417,21 @@
 
                 return tuple(lines) + (time_text,)
 
             def animate(i):
                 for j, ele_tag in enumerate(ele_tags):
 
                     if interpFlag:
-                        xcdi, ycdi = beam_defo_interp_2d(Ex[j, :],
-                                                         Ey[j, :],
+                        xcdi, ycdi = beam_defo_interp_2d(Ecrd[j, :, :],
                                                          Eds[i, j, :],
                                                          sfac,
                                                          nep)
                         lines[j].set_data(xcdi, ycdi)
                     else:
-                        xdi, ydi = beam_disp_ends(Ex[j, :], Ey[j, :],
+                        xdi, ydi = beam_disp_ends(Ecrd[j, :, :],
                                                   Eds[i, j, :], sfac)
                         lines[j].set_data(xdi, ydi)
 
                     # plt.plot(xcdi, ycdi, **fmt_defo)
 
                 # time_text.set_text(f'f')
                 time_text.set_text(f'frame: {i+1}/{n_frames}, \
```

### Comparing `opsvis-1.0.9/opsvis/defo.py` & `opsvis-1.1.1/opsvis/defo.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from mpl_toolkits.mplot3d import Axes3D
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 from matplotlib.collections import PolyCollection
 from matplotlib.patches import Circle, Polygon, Wedge
 from matplotlib.animation import FuncAnimation
 import matplotlib.tri as tri
 
-from settings import *
-import model as opsvmodel
+from .settings import *
+from . import model as opsvmodel
 
 
 def _plot_defo_mode_2d(modeNo, sfac, nep, unDefoFlag, fmt_defo, fmt_undefo,
                        fmt_defo_faces, fmt_undefo_faces,
                        interpFlag, endDispFlag, fmt_nodes,
                        fig_wi_he, fig_lbrt, node_supports, ax):
 
@@ -46,66 +46,144 @@
             ed = np.zeros((nen, ndf))
 
             for i, ele_node_tag in enumerate(ele_node_tags):
                 ecrd[i, :] = ops.nodeCoord(ele_node_tag)
 
             if modeNo:
                 for i, ele_node_tag in enumerate(ele_node_tags):
-                    ed[i, :] = ops.nodeEigenvector(ele_node_tag, modeNo)
+                    ed[i, :] = ops.nodeEigenvector(ele_node_tag, modeNo)[:2]
             else:
                 for i, ele_node_tag in enumerate(ele_node_tags):
-                    ed[i, :] = ops.nodeDisp(ele_node_tag)
+                    ed[i, :] = ops.nodeDisp(ele_node_tag)[:2]
 
             # displaced element coordinates (scaled by sfac factor)
             xy = ecrd + sfac * ed
 
             if unDefoFlag:
                 ax.plot(ecrd[:, 0], ecrd[:, 1], **fmt_undefo)
 
             ax.plot(xy[:, 0], xy[:, 1], **fmt_defo)
 
-        # beam/frame element plot_defo
-        elif (ele_classtag == EleClassTag.ElasticBeam2d or
-              ele_classtag == EleClassTag.ForceBeamColumn2d or
-              ele_classtag == EleClassTag.DispBeamColumn2d):
-
-            nen, ndf = 2, 3
+        elif (ele_classtag == EleClassTag.ZeroLength
+              or ele_classtag == EleClassTag.ZeroLengthSection
+              or ele_classtag == EleClassTag.CoupledZeroLength
+              or ele_classtag == EleClassTag.TwoNodeLink):
 
+            # nen, ndf = 2, 3
+            ndf = ops.getNDF()[0]
             ele_node_tags = ops.eleNodes(ele_tag)
+            nen = len(ele_node_tags)
 
             ecrd = np.zeros((nen, 2))
             ed = np.zeros((nen, ndf))
 
             for i, ele_node_tag in enumerate(ele_node_tags):
                 ecrd[i, :] = ops.nodeCoord(ele_node_tag)
 
             if modeNo:
                 for i, ele_node_tag in enumerate(ele_node_tags):
                     ed[i, :] = ops.nodeEigenvector(ele_node_tag, modeNo)
             else:
                 for i, ele_node_tag in enumerate(ele_node_tags):
                     ed[i, :] = ops.nodeDisp(ele_node_tag)
 
+
+            # fix for a sdof system, or specify sfac explicitly
+            if np.isclose(sfac, 0.0):
+                sfac = 1.0
+
+            # displaced element coordinates (scaled by sfac factor)
+            xy = ecrd + sfac * ed[:, :2]
+
             if unDefoFlag:
                 ax.plot(ecrd[:, 0], ecrd[:, 1], **fmt_undefo)
 
+            ax.plot(xy[:, 0], xy[:, 1], **fmt_defo_zeroLenght)
+
+        # beam/frame element plot_defo
+        elif (ele_classtag == EleClassTag.ElasticBeam2d
+              or ele_classtag == EleClassTag.ForceBeamColumn2d
+              or ele_classtag == EleClassTag.DispBeamColumn2d
+              or ele_classtag == EleClassTag.TimoshenkoBeamColumn2d
+              or ele_classtag == EleClassTag.ElasticTimoshenkoBeam2d):
+
+            nen, ndf = 2, 3
+
+            ele_node_tags = ops.eleNodes(ele_tag)
+
+            ecrd_nodes = np.zeros((nen, 2))
+            # ecrd = np.zeros((nen, 2))
+            ed = np.zeros((nen, ndf))
+
+            for i, ele_node_tag in enumerate(ele_node_tags):
+                # ecrd[i, :] = ops.nodeCoord(ele_node_tag)
+                ecrd_nodes[i, :] = ops.nodeCoord(ele_node_tag)
+
+            ecrd_eles0 = np.copy(ecrd_nodes)
+            ecrd_eles = np.copy(ecrd_nodes)
+
+            if modeNo:
+                for i, ele_node_tag in enumerate(ele_node_tags):
+                    ed[i, :] = ops.nodeEigenvector(ele_node_tag, modeNo)
+            else:
+                for i, ele_node_tag in enumerate(ele_node_tags):
+                    ed[i, :] = ops.nodeDisp(ele_node_tag)
+
+            ele_offsets = np.array(ops.eleResponse(ele_tag, 'offsets'))
+            nz_offsets = np.nonzero(ele_offsets)[0]  # tuple of arrays
+            if np.any(nz_offsets):
+                Lro_l, fi0_l = ro_length_init_rot(ele_offsets[0], ele_offsets[1])
+                Lro_r, fi0_r = ro_length_init_rot(ele_offsets[3], ele_offsets[4])
+                # ed[0, 2] - rotations
+                x_ro_rot_l, y_ro_rot_l = ro_rotated(Lro_l, fi0_l, ed[0, 2]*sfac)
+                x_ro_rot_r, y_ro_rot_r = ro_rotated(Lro_r, fi0_r, ed[1, 2]*sfac)
+                # modify ecrd_eles
+                ecrd_eles0[:, 0] += ele_offsets[[0, 3]]
+                ecrd_eles0[:, 1] += ele_offsets[[1, 4]]
+                ecrd_eles[:, 0] += [x_ro_rot_l, x_ro_rot_r]
+                ecrd_eles[:, 1] += [y_ro_rot_l, y_ro_rot_r]
+            else:
+                pass
+
+            if unDefoFlag:
+                ax.plot(ecrd_eles0[:, 0], ecrd_eles0[:, 1], **fmt_undefo)
+
             # interpolated displacement field
             if interpFlag:
-                xcdi, ycdi = beam_defo_interp_2d(ecrd[:, 0], ecrd[:, 1],
-                                                 ed.flatten(), sfac, nep)
+                xcdi, ycdi = beam_defo_interp_2d(ecrd_eles, ed.flatten(), sfac, nep)
             else:
-                xcdi, ycdi = beam_disp_ends(ecrd[:, 0], ecrd[:, 1],
-                                            ed.flatten(), sfac)
+                xcdi, ycdi = beam_disp_ends(ecrd_eles, ed.flatten(), sfac)
 
             ax.plot(xcdi, ycdi, **fmt_defo)
 
+            # plot rigid offsets
+            # xdi, ydi = beam_disp_ro(ecrd_eles[:, 0],
+            #                         ecrd_eles[:, 1],
+            #                         ed.flatten(), sfac)
+            ax.plot([ecrd_nodes[0, 0] + sfac * ed[0, 0],
+                     ecrd_eles[0, 0] + sfac * ed[0, 0]] ,
+                    [ecrd_nodes[0, 1] + sfac * ed[0, 1],
+                     ecrd_eles[0, 1] + sfac * ed[0, 1]] ,
+                    **fmt_model_rigid_offset)
+            ax.plot([ecrd_nodes[1, 0] + sfac * ed[1, 0],
+                     ecrd_eles[1, 0] + sfac * ed[1, 0]] ,
+                    [ecrd_nodes[1, 1] + sfac * ed[1, 1],
+                     ecrd_eles[1, 1] + sfac * ed[1, 1]],
+                    **fmt_model_rigid_offset)
+
+            # ax.plot([ecrd_nodes[1, 0], ecrd_eles[1, 0]],
+            #         [ecrd_nodes[1, 1], ecrd_eles[1, 1]],
+            #         **fmt_model_rigid_offset)
+
+            # ax.plot([ecrd[0, 0] + sfac*ed[0], ecrd[1, 0] + sfac*ed[3]],
+            #         [ecrd[0, 1] + sfac*ed[1], ecrd[1, 1] + sfac*ed[4]], **fmt_model_rigid_offset)
+
             # translations of ends
             if endDispFlag:
-                xdi, ydi = beam_disp_ends(ecrd[:, 0], ecrd[:, 1],
-                                          ed.flatten(), sfac)
+                xdi, ydi = beam_disp_ends(ecrd_eles, ed.flatten(), sfac)
                 ax.plot(xdi, ydi, **fmt_nodes)
 
         # 2d triangular (tri31) elements plot_defo
         elif (ele_classtag == EleClassTag.tri3n):
 
             nen, ndf = 3, 2
             nodes_geo_order = [0, 1, 2, 0]
@@ -301,19 +379,53 @@
 
     ax.axis('equal')
     ax.grid(False)
 
     return ax
 
 
+def ro_length_init_rot(xo, yo):
+    """Return lenght and initial rotation of the rigid offset in 2d
+    """
+
+    L = np.sqrt(xo**2. + yo**2.)
+    # fi0 = np.arctan(yo/xo)
+    fi0 = np.arctan2(yo, xo)
+
+    return L, fi0
+
+
+def ro_length_init_rot_3d(xo, yo, zo, along='x'):
+    """Return lenght and initial rotation of the rigid offset in 3d
+    """
+    L = np.sqrt(xo**2. + yo**2. + zo**2.)
+    if along == 'x':
+        fi0 = np.arctan2(zo, xo)
+    elif along == 'y':
+        fi0 = np.arctan2(zo, xo)
+    elif along == 'z':
+        fi0 = 0.
+
+
+    return L, fi0
+
+
+def ro_rotated(L, fi0, fi):
+    dfi = fi0 + fi
+    x = L * np.cos(dfi)
+    y = L * np.sin(dfi)
+    return x, y
+
+
 def _plot_defo_mode_3d(modeNo, sfac, nep, unDefoFlag, fmt_defo, fmt_undefo,
                        fmt_defo_faces, fmt_undefo_faces,
                        interpFlag, endDispFlag, fmt_nodes, az_el,
-                       fig_wi_he, fig_lbrt, ax):
+                       fig_wi_he, fig_lbrt, node_supports, ax):
 
+    node_tags = ops.getNodeTags()
     ele_tags = ops.getEleTags()
 
     azim, elev = az_el
 
     if not ax:
         if fig_wi_he:
             fig_wi, fig_he = fig_wi_he
@@ -337,17 +449,18 @@
     ax.view_init(azim=azim, elev=elev)
 
     for i, ele_tag in enumerate(ele_tags):
         ele_classtag = ops.getEleClassTags(ele_tag)[0]
         nen = np.shape(ops.eleNodes(ele_tag))[0]
 
         # if (ele_classtag == EleClassTag.truss):
-        if (ele_classtag == EleClassTag.ElasticBeam3d or
-            ele_classtag == EleClassTag.ForceBeamColumn3d or
-            ele_classtag == EleClassTag.DispBeamColumn3d):
+        if (ele_classtag == EleClassTag.ElasticBeam3d
+            or ele_classtag == EleClassTag.ForceBeamColumn3d
+            or ele_classtag == EleClassTag.DispBeamColumn3d
+            or ele_classtag == EleClassTag.ElasticTimoshenkoBeam3d):
 
             nen, ndf = 2, 6
 
             ele_node_tags = ops.eleNodes(ele_tag)
 
             ecrd = np.zeros((nen, 3))
             ed = np.zeros((nen, ndf))
@@ -369,32 +482,27 @@
 
             if unDefoFlag:
                 plt.plot(ecrd[:, 0], ecrd[:, 1], ecrd[:, 2], **fmt_undefo)
 
             if interpFlag:
                 # xcd, ycd, zcd = beam_defo_interp_3d(ex, ey, ez, g,
                 #                                     ed, sfac, nep)
-                xcd, ycd, zcd = beam_defo_interp_3d(ecrd[:, 0], ecrd[:, 1],
-                                                    ecrd[:, 2], g,
+                xcd, ycd, zcd = beam_defo_interp_3d(ecrd, g,
                                                     ed.flatten(), sfac, nep)
             else:
-                xcd, ycd, zcd = beam_disp_ends3d(ecrd[:, 0], ecrd[:, 1],
-                                                 ecrd[:, 2],
-                                                 ed.flatten(), sfac)
+                xcd, ycd, zcd = beam_disp_ends3d(ecrd, ed.flatten(), sfac)
 
             ax.plot(xcd, ycd, zcd, **fmt_defo)
             ax.set_xlabel('X')
             ax.set_ylabel('Y')
             ax.set_zlabel('Z')
 
             # translations of ends
             if endDispFlag:
-                xd, yd, zd = beam_disp_ends3d(ecrd[:, 0], ecrd[:, 1],
-                                              ecrd[:, 2],
-                                              ed.flatten(), sfac)
+                xd, yd, zd = beam_disp_ends3d(ecrd, ed.flatten(), sfac)
                 ax.plot(xd, yd, zd, **fmt_nodes)
 
         elif (ele_classtag == EleClassTag.truss
               or ele_classtag == EleClassTag.trussSection):
 
             nen, ndf = 2, 3
 
@@ -404,30 +512,69 @@
             ed = np.zeros((nen, ndf))
 
             for i, ele_node_tag in enumerate(ele_node_tags):
                 ecrd[i, :] = ops.nodeCoord(ele_node_tag)
 
             if modeNo:
                 for i, ele_node_tag in enumerate(ele_node_tags):
-                    ed[i, :] = ops.nodeEigenvector(ele_node_tag, modeNo)
+                    ed[i, :] = ops.nodeEigenvector(ele_node_tag, modeNo)[:3]
             else:
                 for i, ele_node_tag in enumerate(ele_node_tags):
-                    ed[i, :] = ops.nodeDisp(ele_node_tag)
+                    ed[i, :] = ops.nodeDisp(ele_node_tag)[:3]
 
             if unDefoFlag:
                 plt.plot(ecrd[:, 0], ecrd[:, 1], ecrd[:, 2], **fmt_undefo)
 
             ax.set_xlabel('X')
             ax.set_ylabel('Y')
             ax.set_zlabel('Z')
 
             # displaced element coordinates (scaled by sfac factor)
             xyz = ecrd + sfac * ed
             ax.plot(xyz[:, 0], xyz[:, 1], xyz[:, 2], **fmt_defo)
 
+        elif (ele_classtag == EleClassTag.ZeroLength
+              or ele_classtag == EleClassTag.ZeroLengthSection
+              or ele_classtag == EleClassTag.CoupledZeroLength
+              or ele_classtag == EleClassTag.TwoNodeLink):
+
+            # nen, ndf = 2, 6
+            ndf = ops.getNDF()[0]
+            ele_node_tags = ops.eleNodes(ele_tag)
+            nen = len(ele_node_tags)
+
+            ecrd = np.zeros((nen, 3))
+            ed = np.zeros((nen, ndf))
+
+            for i, ele_node_tag in enumerate(ele_node_tags):
+                ecrd[i, :] = ops.nodeCoord(ele_node_tag)
+
+            if modeNo:
+                for i, ele_node_tag in enumerate(ele_node_tags):
+                    ed[i, :] = ops.nodeEigenvector(ele_node_tag, modeNo)
+            else:
+                for i, ele_node_tag in enumerate(ele_node_tags):
+                    ed[i, :] = ops.nodeDisp(ele_node_tag)
+
+            if unDefoFlag:
+                plt.plot(ecrd[:, 0], ecrd[:, 1], ecrd[:, 2], **fmt_undefo)
+
+            ax.set_xlabel('X')
+            ax.set_ylabel('Y')
+            ax.set_zlabel('Z')
+
+            # fix for a sdof system, or specify sfac explicitly
+            if np.isclose(sfac, 0.0):
+                sfac = 1.0
+
+            # displaced element coordinates (scaled by sfac factor)
+            xyz = ecrd + sfac * ed[:, :3]
+
+            ax.plot(xyz[:, 0], xyz[:, 1], xyz[:, 2], **fmt_defo_zeroLenght)
+
         # plot: shell in 3d
         elif (ele_classtag == EleClassTag.ShellMITC4 or
               ele_classtag == EleClassTag.ASDShellQ4):
 
             # ndf is limited to translations x, y, z (no rotations)
             nen, ndf = 4, 3
             nodes_geo_order = [0, 1, 2, 3, 0]
@@ -505,15 +652,16 @@
             for j in range(3):
                 ax.plot(xyz[[j, 3], 0],
                          xyz[[j, 3], 1],
                          xyz[[j, 3], 2], 'b.-',
                          lw=0.4, ms=2, mfc='g', mec='g')
 
         # tetra10n, 3d defo
-        elif (ele_classtag == EleClassTag.TenNodeTetrahedron):
+        elif (ele_classtag in {EleClassTag.TenNodeTetrahedron,
+                               EleClassTag.TenNodeTetrahedronSK}):
 
             nen, ndf = 10, 3
             nodes_geo_order = [0, 4, 1, 5, 2, 6, 0]
 
             ele_node_tags = ops.eleNodes(ele_tag)
 
             ecrd = np.zeros((nen, 3))
@@ -652,14 +800,17 @@
 
             for j in range(4):
                 ax.plot(xyz[[j, 16+j, 4+j], 0],
                         xyz[[j, 16+j, 4+j], 1],
                         xyz[[j, 16+j, 4+j], 2], 'b.-',
                         lw=0.4, ms=2, mfc='g', mec='g')
 
+    if node_supports:
+        opsvmodel._plot_supports(node_tags, ax)
+
     ax.set_box_aspect((np.ptp(ax.get_xlim3d()),
                        np.ptp(ax.get_ylim3d()),
                        np.ptp(ax.get_zlim3d())))
 
     return ax
 
 
@@ -735,18 +886,19 @@
             dlmax = max(dxmax, dymax)
             max_u_abs = max(max_ux, max_uy)
 
             max_u_abs = max_u_abs_from_beam_defo_interp_2d(max_u_abs, nep)
 
             sfac = ratio * dlmax/max_u_abs
 
-        ax = _plot_defo_mode_2d(0, sfac, nep, unDefoFlag, fmt_defo, fmt_undefo,
-                                fmt_defo_faces, fmt_undefo_faces,
-                                interpFlag, endDispFlag, fmt_nodes,
-                                fig_wi_he, fig_lbrt, node_supports, ax)
+        ax = _plot_defo_mode_2d(0, sfac, nep, unDefoFlag, fmt_defo,
+                                fmt_undefo, fmt_defo_faces,
+                                fmt_undefo_faces, interpFlag,
+                                endDispFlag, fmt_nodes, fig_wi_he,
+                                fig_lbrt, node_supports, ax)
 
     elif ndim == 3:
         if not sfac:
             for node_tag in node_tags:
                 x_crd = ops.nodeCoord(node_tag)[0]
                 y_crd = ops.nodeCoord(node_tag)[1]
                 z_crd = ops.nodeCoord(node_tag)[2]
@@ -770,18 +922,20 @@
             dlmax = max(dxmax, dymax, dzmax)
             max_u_abs = max(max_ux, max_uy, max_uz)
 
             max_u_abs = max_u_abs_from_beam_defo_interp_3d(max_u_abs, nep)
 
             sfac = ratio * dlmax/max_u_abs
 
-        ax = _plot_defo_mode_3d(0, sfac, nep, unDefoFlag, fmt_defo, fmt_undefo,
-                                fmt_defo_faces, fmt_undefo_faces,
-                                interpFlag, endDispFlag,
-                                fmt_nodes, az_el, fig_wi_he, fig_lbrt, ax)
+        ax = _plot_defo_mode_3d(0, sfac, nep, unDefoFlag, fmt_defo,
+                                fmt_undefo, fmt_defo_faces,
+                                fmt_undefo_faces, interpFlag,
+                                endDispFlag, fmt_nodes, az_el,
+                                fig_wi_he, fig_lbrt, node_supports,
+                                ax)
 
     else:
         print(f'\nWarning! ndim: {ndim} not supported yet.')
 
     return sfac
 
 
@@ -862,18 +1016,19 @@
 
             dxmax = max_x - min_x
             dymax = max_y - min_y
             dlmax = max(dxmax, dymax)
             max_u_abs = max(max_ux, max_uy)
             sfac = ratio * dlmax/max_u_abs
 
-        ax = _plot_defo_mode_2d(modeNo, sfac, nep, unDefoFlag, fmt_defo, fmt_undefo,
-                                fmt_defo_faces, fmt_undefo_faces,
-                                interpFlag, endDispFlag, fmt_nodes,
-                                fig_wi_he, fig_lbrt, node_supports, ax)
+        ax = _plot_defo_mode_2d(modeNo, sfac, nep, unDefoFlag,
+                                fmt_defo, fmt_undefo, fmt_defo_faces,
+                                fmt_undefo_faces, interpFlag,
+                                endDispFlag, fmt_nodes, fig_wi_he,
+                                fig_lbrt, node_supports, ax)
 
     elif ndim == 3:
         if not sfac:
             for node_tag in node_tags:
                 x_crd = ops.nodeCoord(node_tag)[0]
                 y_crd = ops.nodeCoord(node_tag)[1]
                 z_crd = ops.nodeCoord(node_tag)[2]
@@ -894,53 +1049,68 @@
             dxmax = max_x - min_x
             dymax = max_y - min_y
             dzmax = max_z - min_z
             dlmax = max(dxmax, dymax, dzmax)
             max_u_abs = max(max_ux, max_uy, max_uz)
             sfac = ratio * dlmax/max_u_abs
 
-        ax = _plot_defo_mode_3d(modeNo, sfac, nep, unDefoFlag, fmt_defo,
-                                fmt_undefo, fmt_defo_faces, fmt_undefo_faces,
-                                interpFlag, endDispFlag, fmt_nodes,
-                                az_el, fig_wi_he, fig_lbrt, ax)
+        ax = _plot_defo_mode_3d(modeNo, sfac, nep, unDefoFlag,
+                                fmt_defo, fmt_undefo, fmt_defo_faces,
+                                fmt_undefo_faces, interpFlag,
+                                endDispFlag, fmt_nodes, az_el,
+                                fig_wi_he, fig_lbrt, node_supports,
+                                ax)
 
     else:
         print(f'\nWarning! ndim: {ndim} not supported yet.')
 
 
-def beam_disp_ends(ex, ey, d, sfac):
+def beam_disp_ends(ecrd, d, sfac):
+    """
+    Calculate the element deformation at element ends only.
+    """
+
+    #  indx: 0   1   2   3   4   5
+    # Ed = ux1 uy1 ur1 ux2 uy2 ur2
+    exd = np.array([ecrd[0, 0] + sfac * d[0], ecrd[1, 0] + sfac * d[3]])
+    eyd = np.array([ecrd[0, 1] + sfac * d[1], ecrd[1, 1] + sfac * d[4]])
+
+    return exd, eyd
+
+
+def beam_disp_ro(ecrd, d, sfac):
     """
     Calculate the element deformation at element ends only.
     """
 
     #  indx: 0   1   2   3   4   5
     # Ed = ux1 uy1 ur1 ux2 uy2 ur2
-    exd = np.array([ex[0] + sfac*d[0], ex[1] + sfac*d[3]])
-    eyd = np.array([ey[0] + sfac*d[1], ey[1] + sfac*d[4]])
+    exd = np.array([ecrd[0, 0] + sfac * d[0], ecrd[1, 0] + sfac * d[3]])
+    eyd = np.array([ecrd[0, 1] + sfac * d[1], ecrd[1, 1] + sfac * d[4]])
 
     return exd, eyd
 
 
-def beam_defo_interp_2d(ex, ey, u, sfac, nep=17):
+def beam_defo_interp_2d(ecrd, u, sfac, nep=17):
     """
     Interpolate element displacements at nep points.
 
     Parametrs:
-    ex, ey : element x, y coordinates,
+    ecrd : element x, y coordinates (2 x ndm),
     u : element nodal displacements
     sfac : scale factor for deformation plot
     nep : number of evaluation points (including end nodes)
 
     Returns:
     crd_xc, crd_yc : x, y coordinates of interpolated (at nep points)
     beam deformation required for plot_defo() function
     """
 
 
-    G, L, cosa, cosb = opsvmodel.rot_transf_2d(ex, ey)
+    G, L, cosa, cosb = opsvmodel.rot_transf_2d(ecrd)
 
     u_l = G @ u
 
     # longitudinal deformation (1)
     N_a = beam_axial_shape_functions(L, nep)
     u_ac = N_a @ np.array([u_l[0], u_l[3]])
 
@@ -960,66 +1130,64 @@
                    [cosb, cosa]])
 
     u_xyc = G1 @ u_atc
 
     # discretize element coordinates
     # first  row = X + [0 dx 2dx ... 4-dx 4]
     # second row = Y + [0 dy 2dy ... 3-dy 3]
-    xy_c = np.vstack((np.linspace(ex[0], ex[1], num=nep),
-                      np.linspace(ey[0], ey[1], num=nep)))
+    xy_c = np.vstack((np.linspace(ecrd[0, 0], ecrd[1, 0], num=nep),
+                      np.linspace(ecrd[0, 1], ecrd[1, 1], num=nep)))
 
     # Continuous x, y displacement coordinates
     crd_xc = xy_c[0, :] + sfac * u_xyc[0, :]
     crd_yc = xy_c[1, :] + sfac * u_xyc[1, :]
     # latex_array(ecrd_xc)
     # latex_array(ecrd_yc)
 
     return crd_xc, crd_yc
 
 
-def beam_disp_ends3d(ex, ey, ez, d, sfac):
+def beam_disp_ends3d(ecrd, d, sfac):
     """
     Calculate the element deformation at element ends only.
     """
 
     #  indx: 0   1   2   3   4   5   6   7   8   9  10  11
     # Ed = ux1 uy1 uz1 rx1 ry1 rz1 ux2 uy2 uz2 rx2 ry2 rz2
-    exd = np.array([ex[0] + sfac*d[0], ex[1] + sfac*d[6]])
-    eyd = np.array([ey[0] + sfac*d[1], ey[1] + sfac*d[7]])
-    ezd = np.array([ez[0] + sfac*d[2], ez[1] + sfac*d[8]])
+    exd = np.array([ecrd[0, 0] + sfac * d[0], ecrd[1, 0] + sfac * d[6]])
+    eyd = np.array([ecrd[0, 1] + sfac * d[1], ecrd[1, 1] + sfac * d[7]])
+    ezd = np.array([ecrd[0, 2] + sfac * d[2], ecrd[1, 2] + sfac * d[8]])
 
     return exd, eyd, ezd
 
 
-def beam_defo_interp_3d(ex, ey, ez, g, u, sfac, nep=17):
+def beam_defo_interp_3d(ecrd, g, u, sfac, nep=17):
     """
     3d beam version of beam_defo_interp_2d.
     """
-    G, L = opsvmodel.rot_transf_3d(ex, ey, ez, g)
+    G, L = opsvmodel.rot_transf_3d(ecrd, g)
     ul = G @ u
 
-    _, crd_yc = beam_defo_interp_2d(np.array([0., L]),
-                                    np.array([0., 0.]),
+    _, crd_yc = beam_defo_interp_2d(np.array([[0., 0.], [L, 0.]]),
                                     np.array([ul[0], ul[1], ul[5], ul[6],
                                               ul[7], ul[11]]), sfac, nep)
-    crd_xc, crd_zc = beam_defo_interp_2d(np.array([0., L]),
-                                         np.array([0., 0.]),
+    crd_xc, crd_zc = beam_defo_interp_2d(np.array([[0., 0.], [L, 0.]]),
                                          np.array([ul[0], ul[2], -ul[4], ul[6],
                                                    ul[8], -ul[10]]), sfac, nep)
 
     xl = np.linspace(0., L, num=nep)
     crd_xc = crd_xc - xl
 
     crd_xyzc = np.vstack([crd_xc, crd_yc, crd_zc])
 
     u_xyzc = np.transpose(g) @ crd_xyzc
 
-    xyz_c = np.vstack((np.linspace(ex[0], ex[1], num=nep),
-                       np.linspace(ey[0], ey[1], num=nep),
-                       np.linspace(ez[0], ez[1], num=nep)))
+    xyz_c = np.vstack((np.linspace(ecrd[0, 0], ecrd[1, 0], num=nep),
+                       np.linspace(ecrd[0, 1], ecrd[1, 1], num=nep),
+                       np.linspace(ecrd[0, 2], ecrd[1, 2], num=nep)))
 
     crd_xc = xyz_c[0, :] + u_xyzc[0, :]
     crd_yc = xyz_c[1, :] + u_xyzc[1, :]
     crd_zc = xyz_c[2, :] + u_xyzc[2, :]
 
     return crd_xc, crd_yc, crd_zc
 
@@ -1049,19 +1217,17 @@
 
             for i, ele_node_tag in enumerate(ele_node_tags):
                 ecrd[i, :] = ops.nodeCoord(ele_node_tag)
 
             for i, ele_node_tag in enumerate(ele_node_tags):
                 ed[i, :] = ops.nodeDisp(ele_node_tag)
 
-            ex = ecrd[:, 0]
-            ey = ecrd[:, 1]
             u = ed.flatten()
 
-            G, L, *_ = opsvmodel.rot_transf_2d(ex, ey)
+            G, L, *_ = opsvmodel.rot_transf_2d(ecrd)
 
             u_l = G @ u
 
             N_t = beam_transverse_shape_functions(L, nep)
 
             u_tc = N_t @ np.array([u_l[1], u_l[2], u_l[4], u_l[5]])
 
@@ -1102,20 +1268,17 @@
 
             for i, ele_node_tag in enumerate(ele_node_tags):
                 ecrd[i, :] = ops.nodeCoord(ele_node_tag)
 
             for i, ele_node_tag in enumerate(ele_node_tags):
                 ed[i, :] = ops.nodeDisp(ele_node_tag)
 
-            ex = ecrd[:, 0]
-            ey = ecrd[:, 1]
-            ez = ecrd[:, 2]
             u = ed.flatten()
 
-            G, L = opsvmodel.rot_transf_3d(ex, ey, ez, g)
+            G, L = opsvmodel.rot_transf_3d(ecrd, g)
             ul = G @ u
 
             N_t = beam_transverse_shape_functions(L, nep)
 
             # account for two cross section axis
             # (1) first cross section axis
             u_tc = N_t @ np.array([ul[1], ul[5], ul[7], ul[11]])
```

### Comparing `opsvis-1.0.9/opsvis/fibsec.py` & `opsvis-1.1.1/opsvis/fibsec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import openseespy.opensees as ops
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.patches import Circle, Polygon, Wedge
 
-from settings import *
+from .settings import *
 
 
 # plot_fiber_section is inspired by plotSection matlab function
 # written by D. Vamvatsikos available at
 # http://users.ntua.gr/divamva/software.html (plotSection.zip)
 def plot_fiber_section(fib_sec_list, fillflag=1,
                        matcolor=['y', 'b', 'r', 'g', 'm', 'k']):
@@ -187,28 +187,45 @@
     for dat in fib_sec_list:
         if dat[0] == 'section':
             secTag, GJ = dat[2], dat[4]
             ops.section('Fiber', secTag, '-GJ', GJ)
 
         if dat[0] == 'layer':
             matTag = dat[2]
+            n_bars = dat[3]
+            As = dat[4]
             if dat[1] == 'straight':
-                n_bars = dat[3]
-                As = dat[4]
                 Iy, Iz, Jy, Jz = dat[5], dat[6], dat[7], dat[8]
                 ops.layer('straight', matTag, n_bars, As, Iy, Iz, Jy, Jz)
 
+            elif dat[1] == 'circ':
+                yC, zC, radius = dat[5], dat[6], dat[7]
+
+                if len(dat) > 8:
+                    begAng, endAng = dat[8], dat[9]
+                    ops.layer('circ', matTag, n_bars, As, yC, zC, radius,
+                              begAng, endAng)
+                else:
+                    ops.layer('circ', matTag, n_bars, As, yC, zC, radius)
+
         if dat[0] == 'patch':
             matTag = dat[2]
             nIJ = dat[3]
             nJK = dat[4]
 
             if dat[1] == 'quad' or dat[1] == 'quadr':
                 Iy, Iz, Jy, Jz = dat[5], dat[6], dat[7], dat[8]
                 Ky, Kz, Ly, Lz = dat[9], dat[10], dat[11], dat[12]
                 ops.patch('quad', matTag, nIJ, nJK, Iy, Iz, Jy, Jz, Ky, Kz,
                           Ly, Lz)
 
-            if dat[1] == 'rect':
+            elif dat[1] == 'rect':
                 Iy, Iz, Ky, Kz = dat[5], dat[6], dat[7], dat[8]
                 Jy, Jz, Ly, Lz = Ky, Iz, Iy, Kz
                 ops.patch('rect', matTag, nIJ, nJK, Iy, Iz, Ky, Kz)
+
+            elif dat[1] == 'circ':
+                yC, zC, intRad, extRad = dat[5], dat[6], dat[7], dat[8]
+
+                begAng, endAng = dat[9], dat[10]
+                ops.patch('circ', matTag, nIJ, nJK, yC, zC, intRad, extRad,
+                          begAng, endAng)
```

### Comparing `opsvis-1.0.9/opsvis/model.py` & `opsvis-1.1.1/opsvis/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d import Axes3D
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 from matplotlib.collections import PolyCollection
 from matplotlib.patches import Circle, Polygon, Wedge
 from matplotlib.animation import FuncAnimation
+from matplotlib.path import Path
 import matplotlib.tri as tri
 
-from settings import *
-from defo import *
-from matplotlib.path import Path
+from .settings import *
+from .defo import *
 
 
 def _plot_model_2d(node_labels, element_labels, offset_nd_label, axis_off,
                    fig_wi_he, fig_lbrt, nodes_only, fmt_model,
-                   fmt_model_nodes_only, node_supports, ax):
+                   fmt_model_nodes_only, node_supports, gauss_points, fmt_gauss_points,
+                   fmt_model_truss, truss_node_offset, ax):
 
     if not ax:
         if fig_wi_he:
             fig_wi, fig_he = fig_wi_he
             fig, ax = plt.subplots(figsize=(fig_wi / 2.54, fig_he / 2.54))
         else:
             fig, ax = plt.subplots()
@@ -83,32 +84,99 @@
         ele_classtag = ops.getEleClassTags(ele_tag)[0]
 
         if (ele_classtag == EleClassTag.ElasticBeam2d
                 or ele_classtag == EleClassTag.ForceBeamColumn2d
                 or ele_classtag == EleClassTag.DispBeamColumn2d
                 or ele_classtag == EleClassTag.TimoshenkoBeamColumn2d
                 or ele_classtag == EleClassTag.ElasticTimoshenkoBeam2d
-                or ele_classtag == EleClassTag.truss
-                or ele_classtag == EleClassTag.trussSection
                 or ele_classtag == EleClassTag.MVLEM
                 or ele_classtag == EleClassTag.SFI_MVLEM):
 
             nen = 2
             ele_node_tags = ops.eleNodes(ele_tag)
+            ecrd_nodes = np.zeros((nen, 2))
+            for i, ele_node_tag in enumerate(ele_node_tags):
+                ecrd_nodes[i, :] = ops.nodeCoord(ele_node_tag)
+
+            ecrd_eles = np.copy(ecrd_nodes)
+
+            ele_offsets = np.array(ops.eleResponse(ele_tag, 'offsets'))
+            nz_offsets = np.nonzero(ele_offsets)[0]  # tuple of arrays
+            if np.any(nz_offsets):
+                # modify ecrd_eles
+                ecrd_eles[:, 0] += ele_offsets[[0, 3]]
+                ecrd_eles[:, 1] += ele_offsets[[1, 4]]
+                ax.plot([ecrd_nodes[0, 0], ecrd_eles[0, 0]],
+                        [ecrd_nodes[0, 1], ecrd_eles[0, 1]],
+                        **fmt_model_rigid_offset)
+                ax.plot([ecrd_nodes[1, 0], ecrd_eles[1, 0]],
+                        [ecrd_nodes[1, 1], ecrd_eles[1, 1]],
+                        **fmt_model_rigid_offset)
+
+            else:
+                pass
+
+            ax.plot(ecrd_eles[:, 0], ecrd_eles[:, 1], **fmt_model)
+
+            if gauss_points:
+                Lgps = ops.eleResponse(ele_tag, 'integrationPoints')
+                for Lgpi in Lgps:
+                    dxi = (ecrd_eles[1, 0] - ecrd_eles[0, 0]) * Lgpi / bar_length(ecrd_eles)
+                    dyi = (ecrd_eles[1, 1] - ecrd_eles[0, 1]) * Lgpi / bar_length(ecrd_eles)
+                    ax.plot(ecrd_eles[0, 0] + dxi, ecrd_eles[0, 1] + dyi, **fmt_gauss_points)
+
+            # location of label
+            xt = sum(ecrd_eles[:, 0]) / nen
+            yt = sum(ecrd_eles[:, 1]) / nen
+
+            if element_labels:
+                if ecrd_eles[1, 0] - ecrd_eles[0, 0] == 0:
+                    va = 'center'
+                    ha = 'left'
+                    offset_x, offset_y = _offset, 0.0
+                elif ecrd_eles[1, 1] - ecrd_eles[0, 1] == 0:
+                    va = 'bottom'
+                    ha = 'center'
+                    offset_x, offset_y = 0.0, _offset
+                else:
+                    va = 'bottom'
+                    ha = 'left'
+                    offset_x, offset_y = 0.03, 0.03
+
+                ax.text(xt+offset_x, yt+offset_y, f'{ele_tag}', va=va, ha=ha,
+                        color='red')
+
+        if (ele_classtag == EleClassTag.truss
+                or ele_classtag == EleClassTag.trussSection):
+
+            nen = 2
+            ele_node_tags = ops.eleNodes(ele_tag)
 
             ecrd = np.zeros((nen, 2))
 
             for i, ele_node_tag in enumerate(ele_node_tags):
                 ecrd[i, :] = ops.nodeCoord(ele_node_tag)
 
+
             # location of label
             xt = sum(ecrd[:, 0]) / nen
             yt = sum(ecrd[:, 1]) / nen
 
-            ax.plot(ecrd[:, 0], ecrd[:, 1], **fmt_model)
+            if truss_node_offset:
+                Lx = ecrd[1, 0] - ecrd[0, 0]
+                Ly = ecrd[1, 1] - ecrd[0, 1]
+                dLx = truss_node_offset * Lx
+                dLy = truss_node_offset * Ly
+
+                ecrd[0, 0] += dLx
+                ecrd[1, 0] -= dLx
+                ecrd[0, 1] += dLy
+                ecrd[1, 1] -= dLy
+
+            ax.plot(ecrd[:, 0], ecrd[:, 1], **fmt_model_truss)
 
             if element_labels:
                 if ecrd[1, 0] - ecrd[0, 0] == 0:
                     va = 'center'
                     ha = 'left'
                     offset_x, offset_y = _offset, 0.0
                 elif ecrd[1, 1] - ecrd[0, 1] == 0:
@@ -307,15 +375,15 @@
     ax.grid(False)
 
     return ax
 
 
 def _plot_supports(node_tags, ax):
 
-    ndf = ops.getNDF()[0]
+    ndim = ops.getNDM()[0]
 
     # fix 2d support: square
     verts = [(-1., 0.),
              (1., 0.),
              (1., -2.),
              (-1., -2.),
              (-1., 0.)]
@@ -391,65 +459,57 @@
              Path.CURVE3,
              Path.LINETO,
              Path.MOVETO,
              Path.LINETO]
 
     path_roller_vert = Path(verts, codes)
 
-    for node_tag in node_tags:
-        nd_crd = ops.nodeCoord(node_tag)
+    m_color = 'm'
+    m_fstyle = 'full'
+    m_size = 16
 
-        node_dofs = ops.nodeDOFs(node_tag)
+    fixed_nodes = ops.getFixedNodes()
 
-        m_type = None
-        m_color = 'm'
-        m_fstyle = 'full'
+    for node_tag in fixed_nodes:
+        nd_crd = ops.nodeCoord(node_tag)
 
-        if ndf < 3:
-            if (node_dofs[0] == -1 and node_dofs[1] == -1):
-                m_type = path_pin
-                m_fstyle = 'full'
-                m_size = 16
-            elif (node_dofs[0] == -1):
-                m_type = path_roller_vert
-                m_fstyle = 'full'
-                m_size = 16
-            elif (node_dofs[1] == -1):
-                m_type = path_roller_horiz
-                m_fstyle = 'full'
-                m_size = 16
+        fixed_dofs = ops.getFixedDOFs(node_tag)
 
-        else:
-            if (node_dofs[0] == -1 and node_dofs[1] == -1 and node_dofs[2] == -1):
+        if ndim == 2:
+            if (fixed_dofs == [1, 2, 3]):
                 m_type = path_fix
-                m_fstyle = 'full'
-                m_size = 16
-            elif (node_dofs[0] == -1 and node_dofs[1] == -1):
+            elif (fixed_dofs == [1, 2]):
                 m_type = path_pin
-                m_fstyle = 'full'
-                m_size = 16
-            elif (node_dofs[0] == -1):
+            elif (fixed_dofs == [1]):
                 m_type = path_roller_vert
-                m_fstyle = 'full'
-                m_size = 16
-            elif (node_dofs[1] == -1):
+            elif (fixed_dofs == [2]):
                 m_type = path_roller_horiz
-                m_fstyle = 'full'
-                m_size = 16
 
-        if m_type:
             ax.plot(nd_crd[0], nd_crd[1], marker=m_type, markersize=m_size,
                     color=m_color, fillstyle=m_fstyle)
 
+        elif ndim == 3:
+            if (fixed_dofs == [1, 2, 3, 4, 5, 6]):
+                m_type = path_fix
+            elif (fixed_dofs == [1, 2, 3]):
+                m_type = path_pin
+            else:
+                m_type = None
+
+            ax.plot(nd_crd[0], nd_crd[1], nd_crd[2], marker=m_type, markersize=m_size,
+                    color=m_color, fillstyle=m_fstyle)
+
     return ax
 
 
-def _plot_model_3d(node_labels, element_labels, offset_nd_label, axis_off,
-                   az_el, fig_wi_he, fig_lbrt, local_axes, nodes_only,
-                   fmt_model, ax):
+def _plot_model_3d(node_labels, element_labels, offset_nd_label,
+                   axis_off, az_el, fig_wi_he, fig_lbrt, local_axes,
+                   nodes_only, fmt_model, node_supports, gauss_points,
+                   fmt_gauss_points, fmt_model_truss,
+                   truss_node_offset, ax):
 
     node_tags = ops.getNodeTags()
     ele_tags = ops.getEleTags()
 
     azim, elev = az_el
 
     if not ax:
@@ -507,99 +567,144 @@
         _offset = 0.
     else:
         max_crd = np.amax([max_x_crd, max_y_crd, max_z_crd])
         _offset = 0.005 * max_crd
 
     if node_labels:
         for node_tag in node_tags:
-            ax.text(ops.nodeCoord(node_tag)[0]+_offset,
-                    ops.nodeCoord(node_tag)[1]+_offset,
-                    ops.nodeCoord(node_tag)[2]+_offset,
+            ax.text(ops.nodeCoord(node_tag)[0] + _offset,
+                    ops.nodeCoord(node_tag)[1] + _offset,
+                    ops.nodeCoord(node_tag)[2] + _offset,
                     f'{node_tag}', va='bottom', ha='left', color='blue')
 
     for i, ele_tag in enumerate(ele_tags):
         ele_classtag = ops.getEleClassTags(ele_tag)[0]
         nen = np.shape(ops.eleNodes(ele_tag))[0]
 
         if (ele_classtag == EleClassTag.ElasticBeam3d or
             ele_classtag == EleClassTag.ForceBeamColumn3d or
             ele_classtag == EleClassTag.DispBeamColumn3d or
             ele_classtag == EleClassTag.ElasticTimoshenkoBeam3d):
 
             nen = 2
             ele_node_tags = ops.eleNodes(ele_tag)
+            ecrd_nodes = np.zeros((nen, 3))
+            for i, ele_node_tag in enumerate(ele_node_tags):
+                ecrd_nodes[i, :] = ops.nodeCoord(ele_node_tag)
 
-            ecrd = np.zeros((nen, 3))
+            ecrd_eles = np.copy(ecrd_nodes)
 
-            for i, ele_node_tag in enumerate(ele_node_tags):
-                ecrd[i, :] = ops.nodeCoord(ele_node_tag)
+            ele_offsets = np.array(ops.eleResponse(ele_tag, 'offsets'))
+            nz_offsets = np.nonzero(ele_offsets)[0]  # tuple of arrays
+            if np.any(nz_offsets):
+                # modify ecrd_eles
+                ecrd_eles[:, 0] += ele_offsets[[0, 3]]
+                ecrd_eles[:, 1] += ele_offsets[[1, 4]]
+                ecrd_eles[:, 2] += ele_offsets[[2, 5]]
+                ax.plot([ecrd_nodes[0, 0], ecrd_eles[0, 0]],
+                        [ecrd_nodes[0, 1], ecrd_eles[0, 1]],
+                        [ecrd_nodes[0, 2], ecrd_eles[0, 2]],
+                        **fmt_model_rigid_offset)
+                ax.plot([ecrd_nodes[1, 0], ecrd_eles[1, 0]],
+                        [ecrd_nodes[1, 1], ecrd_eles[1, 1]],
+                        [ecrd_nodes[1, 2], ecrd_eles[1, 2]],
+                        **fmt_model_rigid_offset)
 
-            # location of label
-            xt = sum(ecrd[:, 0]) / nen
-            yt = sum(ecrd[:, 1]) / nen
-            zt = sum(ecrd[:, 2]) / nen
+            else:
+                pass
 
-            ax.plot(ecrd[:, 0], ecrd[:, 1], ecrd[:, 2], **fmt_model)
+            ax.plot(ecrd_eles[:, 0],
+                    ecrd_eles[:, 1],
+                    ecrd_eles[:, 2], **fmt_model)
+            # ax.plot(ecrd[:, 0], ecrd[:, 1], ecrd[:, 2], **fmt_model)
+
+            # location of label
+            xt = sum(ecrd_eles[:, 0]) / nen
+            yt = sum(ecrd_eles[:, 1]) / nen
+            zt = sum(ecrd_eles[:, 2]) / nen
 
             # fixme: placement of node_tag labels
             if element_labels:
-                if ecrd[1, 0] - ecrd[0, 0] == 0:
+                if ecrd_eles[1, 0] - ecrd_eles[0, 0] == 0:
                     va = 'center'
                     ha = 'left'
                     offset_x, offset_y, offset_z = _offset, 0.0, 0.0
-                elif ecrd[1, 1] - ecrd[0, 1] == 0:
+                elif ecrd_eles[1, 1] - ecrd_eles[0, 1] == 0:
                     va = 'bottom'
                     ha = 'center'
                     offset_x, offset_y, offset_z = 0.0, _offset, 0.0
-                elif ecrd[1, 2] - ecrd[0, 2] == 0:
+                elif ecrd_eles[1, 2] - ecrd_eles[0, 2] == 0:
                     va = 'bottom'
                     ha = 'center'
                     offset_x, offset_y, offset_z = 0.0, 0.0, _offset
                 else:
                     va = 'bottom'
                     ha = 'left'
                     offset_x, offset_y, offset_z = 0.03, 0.03, 0.03
 
-                ax.text(xt+offset_x, yt+offset_y, zt+offset_z, f'{ele_tag}',
+                ax.text(xt + offset_x,
+                        yt + offset_y,
+                        zt + offset_z, f'{ele_tag}',
                         va=va, ha=ha, color='red')
 
             if local_axes:
                 # eo = Eo[i, :]
                 xloc = ops.eleResponse(ele_tag, 'xlocal')
                 yloc = ops.eleResponse(ele_tag, 'ylocal')
                 zloc = ops.eleResponse(ele_tag, 'zlocal')
                 g = np.vstack((xloc, yloc, zloc))
-                L = bar_length(ecrd[:, 0], ecrd[:, 1], ecrd[:, 2])
-                alen = 0.1*L
+                L = bar_length(ecrd_eles)
+                alen = 0.1 * L
 
                 # plot local axis directional vectors: workaround quiver = arrow
                 ax.quiver(xt, yt, zt, g[0, 0], g[0, 1], g[0, 2], color='g',
                           lw=2, length=alen, alpha=.8, normalize=True)
                 ax.quiver(xt, yt, zt, g[1, 0], g[1, 1], g[1, 2], color='b',
                           lw=2, length=alen, alpha=.8, normalize=True)
                 ax.quiver(xt, yt, zt, g[2, 0], g[2, 1], g[2, 2], color='r',
                           lw=2, length=alen, alpha=.8, normalize=True)
 
+            if gauss_points:
+                Lgps = ops.eleResponse(ele_tag, 'integrationPoints')
+                for Lgpi in Lgps:
+                    dxi = (ecrd_eles[1, 0] - ecrd_eles[0, 0]) * Lgpi / bar_length(ecrd_eles)
+                    dyi = (ecrd_eles[1, 1] - ecrd_eles[0, 1]) * Lgpi / bar_length(ecrd_eles)
+                    dzi = (ecrd_eles[1, 2] - ecrd_eles[0, 2]) * Lgpi / bar_length(ecrd_eles)
+                    ax.plot(ecrd_eles[0, 0] + dxi, ecrd_eles[0, 1] + dyi, ecrd_eles[0, 2] + dzi, **fmt_gauss_points)
+
         elif (ele_classtag == EleClassTag.truss
               or ele_classtag == EleClassTag.trussSection):
 
             nen = 2
             ele_node_tags = ops.eleNodes(ele_tag)
-
             ecrd = np.zeros((nen, 3))
-
             for i, ele_node_tag in enumerate(ele_node_tags):
                 ecrd[i, :] = ops.nodeCoord(ele_node_tag)
 
             # location of label
             xt = sum(ecrd[:, 0]) / nen
             yt = sum(ecrd[:, 1]) / nen
             zt = sum(ecrd[:, 2]) / nen
 
-            ax.plot(ecrd[:, 0], ecrd[:, 1], ecrd[:, 2], **fmt_model)
+            if truss_node_offset:
+                Lx = ecrd[1, 0] - ecrd[0, 0]
+                Ly = ecrd[1, 1] - ecrd[0, 1]
+                Lz = ecrd[1, 2] - ecrd[0, 2]
+                dLx = truss_node_offset * Lx
+                dLy = truss_node_offset * Ly
+                dLz = truss_node_offset * Lz
+
+                ecrd[0, 0] += dLx
+                ecrd[1, 0] -= dLx
+                ecrd[0, 1] += dLy
+                ecrd[1, 1] -= dLy
+                ecrd[0, 2] += dLz
+                ecrd[1, 2] -= dLz
+
+            ax.plot(ecrd[:, 0], ecrd[:, 1], ecrd[:, 2], **fmt_model_truss)
 
             # fixme: placement of node_tag labels
             if element_labels:
                 if ecrd[1, 0] - ecrd[0, 0] == 0:
                     va = 'center'
                     ha = 'left'
                     offset_x, offset_y, offset_z = _offset, 0.0, 0.0
@@ -671,15 +776,16 @@
             # if node_labels:
             #     for node_tag in node_tags:
             #         ax.text(ops.nodeCoord(node_tag)[0]+_offset,
             #                 ops.nodeCoord(node_tag)[1]+_offset,
             #                 ops.nodeCoord(node_tag)[2]+_offset,
             #                 f'{node_tag}', va='bottom', ha='left', color='blue')
 
-        elif ele_classtag == EleClassTag.TenNodeTetrahedron:
+        elif (ele_classtag in {EleClassTag.TenNodeTetrahedron,
+                               EleClassTag.TenNodeTetrahedronSK}):
 
             nen = 10
             nodes_geo_order = [0, 4, 1, 5, 2, 6, 0]
 
             ele_node_tags = ops.eleNodes(ele_tag)
 
             ecrd = np.zeros((nen, 3))
@@ -900,17 +1006,15 @@
         # elif nen == 20:
         elif (ele_classtag == EleClassTag.brick20n):
 
             nen = 20
             nodes_geo_order = np.array([0, 8, 1, 9, 2, 10, 3, 11, 0], dtype=int)  # bottom face nodes loop
 
             ele_node_tags = ops.eleNodes(ele_tag)
-
             ecrd = np.zeros((nen, 3))
-
             for i, ele_node_tag in enumerate(ele_node_tags):
                 ecrd[i, :] = ops.nodeCoord(ele_node_tag)
 
             ax.plot(ecrd[nodes_geo_order, 0],
                     ecrd[nodes_geo_order, 1],
                     ecrd[nodes_geo_order, 2],
                     **fmt_model, mfc='g', mec='g')
@@ -987,27 +1091,33 @@
             #         [ecrd[1, 1], ecrd[1, 1], ecrd[3, 1], ecrd[3, 1],
             #          ecrd[1, 1]], **fmt_model_joint2d)
 
             if element_labels:
                 ax.text(xt, yt, zt, f'{ele_tag}', va='top', ha='left',
                         color='red')
 
+    if node_supports:
+        _plot_supports(node_tags, ax)
+
     ax.set_box_aspect((np.ptp(ax.get_xlim3d()),
                        np.ptp(ax.get_ylim3d()),
                        np.ptp(ax.get_zlim3d())))
 
     return ax
 
 
 def plot_model(node_labels=1, element_labels=1, offset_nd_label=False,
                axis_off=0, az_el=az_el, fig_wi_he=False,
                fig_lbrt=False, local_axes=True, nodes_only=False,
                fmt_model=fmt_model,
                fmt_model_nodes_only=fmt_model_nodes_only,
-               node_supports=True, ax=False):
+               node_supports=True, gauss_points=True,
+               fmt_gauss_points=fmt_gauss_points,
+               fmt_model_truss=fmt_model_truss,
+               truss_node_offset=0.96, ax=False):
     """Plot defined model of the structure.
 
     Args:
         node_labels (int): 1 - plot node labels, 0 - do not plot them;
             (default: 1)
 
         element_labels (int): 1 - plot element labels, 0 - do not plot
@@ -1035,14 +1145,23 @@
         fmt_model (dict): A dictionary containing formatting the line and markers
             of the model elements. The formatting options can be: linewidth, color,
             marker, markersize. See matplotlib.plot documentation for more details,
             if necessary.
 
         node_supports (bool): True - show the supports. Default: True.
 
+        gauss_points (bool): True - show the integration (Gauss) points. Default: True.
+
+        fmt_gauss_points (dict): A dictionary containing formatting the marker
+            of the gauss point.
+
+        truss_node_offset (float): If non-zero, the nodes are offset to show pin markers.
+            The number should preferably be between 0.90-0.97.
+            Zero (0) or False means no offset. Default: 0.96.
+
         ax: axis object.
 
     Usage:
 
     ``plot_model()`` - plot model with node and element labels.
 
     ``plot_model(node_labels=0, element_labels=0)`` - plot model without node
@@ -1060,25 +1179,30 @@
 
     # az_el - azimut, elevation used for 3d plots only
     node_tags = ops.getNodeTags()
 
     ndim = ops.getNDM()[0]
 
     if ndim == 2:
-        ax = _plot_model_2d(node_labels, element_labels, offset_nd_label,
-                            axis_off, fig_wi_he, fig_lbrt, nodes_only,
-                            fmt_model, fmt_model_nodes_only,
-                            node_supports, ax)
+        ax = _plot_model_2d(node_labels, element_labels,
+                            offset_nd_label, axis_off, fig_wi_he,
+                            fig_lbrt, nodes_only, fmt_model,
+                            fmt_model_nodes_only, node_supports,
+                            gauss_points, fmt_gauss_points,
+                            fmt_model_truss, truss_node_offset, ax)
         if axis_off:
             ax.axis('off')
 
     elif ndim == 3:
-        ax = _plot_model_3d(node_labels, element_labels, offset_nd_label, axis_off,
-                            az_el, fig_wi_he, fig_lbrt, local_axes, nodes_only,
-                            fmt_model, ax)
+        ax = _plot_model_3d(node_labels, element_labels,
+                            offset_nd_label, axis_off, az_el,
+                            fig_wi_he, fig_lbrt, local_axes,
+                            nodes_only, fmt_model, node_supports,
+                            gauss_points, fmt_gauss_points,
+                            fmt_model_truss, truss_node_offset, ax)
         if axis_off:
             ax.axis('off')
 
     else:
         print(f'\nWarning! ndim: {ndim} not supported yet.')
 
     # plt.show()  # call this from main py file for more control
@@ -1094,15 +1218,15 @@
     print('\nWarning! plot_supports_and_loads_2d has been removed.')  # noqa: E501
     print('\nWarning! Use plot_model(node_supports=True) for showing supports and')  # noqa: E501
     print('\nWarning! plot_loads_2d() for showing loads')  # noqa: E501
 
 
 def plot_loads_2d(nep=17, sfac=False, fig_wi_he=False,
                   fig_lbrt=False, fmt_model_loads=fmt_model_loads,
-                  node_supports=True, ax=False):
+                  node_supports=True, truss_node_offset=0, ax=False):
     """Display the nodal and element loads applied to the 2d models.
 
     Args:
         nep (int): number of arrows when displacing element distributed loads
             (default: 17)
 
         node_supports (bool): True - show the node support conditions.
@@ -1118,15 +1242,16 @@
             fig, ax = plt.subplots()
 
         if fig_lbrt:
             fleft, fbottom, fright, ftop = fig_lbrt
             fig.subplots_adjust(left=fleft, bottom=fbottom, right=fright, top=ftop)
 
     ax = plot_model(node_labels=0, element_labels=0, fmt_model=fmt_model_loads,
-                    node_supports=node_supports, ax=ax)
+                    node_supports=node_supports,
+                    truss_node_offset=truss_node_offset, ax=ax)
     # ax.axis('equal')
 
     if not sfac:
         ratio = 0.1
         min_x, max_x = ax.get_xlim()
         min_y, max_y = ax.get_ylim()
         xsfac = ratio * abs(max_x - min_x)
@@ -1143,37 +1268,48 @@
     ### get Ew data
     Ew = get_Ew_data_from_ops_domain()
 
     for ele_tag in ele_tags:
 
         ele_class_tag = ops.getEleClassTags(ele_tag)[0]
 
-        if (ele_class_tag == EleClassTag.ElasticBeam2d or
-            ele_class_tag == EleClassTag.ForceBeamColumn2d or
-            ele_class_tag == EleClassTag.DispBeamColumn2d):
+        if (ele_class_tag == EleClassTag.ElasticBeam2d
+            or ele_class_tag == EleClassTag.ForceBeamColumn2d
+            or ele_class_tag == EleClassTag.DispBeamColumn2d
+            or ele_class_tag == EleClassTag.TimoshenkoBeamColumn2d
+            or ele_class_tag == EleClassTag.ElasticTimoshenkoBeam2d):
 
             # by default no element load
             ele_load_data = []
             if ele_tag in Ew:
                 ele_load_data = Ew[ele_tag]
 
-            nd1, nd2 = ops.eleNodes(ele_tag)
+            nen = 2
+            ele_node_tags = ops.eleNodes(ele_tag)
+            ecrd_nodes = np.zeros((nen, 2))
+            for i, ele_node_tag in enumerate(ele_node_tags):
+                ecrd_nodes[i, :] = ops.nodeCoord(ele_node_tag)
+
+            ecrd_eles = np.copy(ecrd_nodes)
 
-            # element x, y coordinates
-            ex = np.array([ops.nodeCoord(nd1)[0],
-                           ops.nodeCoord(nd2)[0]])
-            ey = np.array([ops.nodeCoord(nd1)[1],
-                           ops.nodeCoord(nd2)[1]])
+            ele_offsets = np.array(ops.eleResponse(ele_tag, 'offsets'))
+            nz_offsets = np.nonzero(ele_offsets)[0]  # tuple of arrays
+            if np.any(nz_offsets):
+                # modify ecrd_eles
+                ecrd_eles[:, 0] += ele_offsets[[0, 3]]
+                ecrd_eles[:, 1] += ele_offsets[[1, 4]]
+            else:
+                pass
 
             # step 1: first plot model itself
-            # ax.plot(ex, ey, 'k-', solid_capstyle='round', solid_joinstyle='round',
+            # ax.plot(ecrd[:, 0], ecrd[:, 1], 'k-', solid_capstyle='round', solid_joinstyle='round',
             #         dash_capstyle='butt', dash_joinstyle='round')
 
             # step 2
-            Lxy = np.array([ex[1]-ex[0], ey[1]-ey[0]])
+            Lxy = ecrd_eles[1, :] - ecrd_eles[0, :]
             L = np.sqrt(Lxy @ Lxy)
             cosa, cosb = Lxy / L
 
             # if not sfac:
             #     sfac = ratio * L
 
             xl = np.linspace(0., L, nep)
@@ -1193,59 +1329,59 @@
 
                 if ele_load_type == '-beamPoint':
                     Pt, aL, Pa = ele_load_data_i[1:4]
                     a = aL * L
                     s = sfac * np.sign(Pt)
 
                     s_0 = np.zeros(2)
-                    # s_0 = [ex[0], ey[0]]
+                    # s_0 = [ecrd[0, 0], ecrd[0, 1]]
 
-                    s_0[0] = ex[0] + a * cosa
-                    s_0[1] = ey[0] + a * cosb
+                    s_0[0] = ecrd_eles[0, 0] + a * cosa
+                    s_0[1] = ecrd_eles[0, 1] + a * cosb
 
                     s_p = np.copy(s_0)
 
                     s_p[0] -= s * cosb
                     s_p[1] += s * cosa
 
 
                     # plot arrows
                     ax.arrow(s_0[0], s_0[1],
-                             s_p[0]-s_0[0], s_p[1]-s_0[1],
+                             s_p[0] - s_0[0], s_p[1] - s_0[1],
                              # width = 0.01,
                              head_starts_at_zero=True,  # default False
                              # overhang=0.2,
                              # lw = 1,
-                             head_width=0.1*sfac, head_length=0.2*sfac,
+                             head_width=0.1 * sfac, head_length=0.2 * sfac,
                              fc='b', ec='b',
                              length_includes_head=False, shape='full')
-                    ax.text(sum(ex)/2, sum(ey)/2, f'{Pt}', color='b')
+                    ax.text(sum(ecrd_eles[:, 0])/2, sum(ecrd_eles[:, 1])/2, f'{abs(Pt)}', color='b')
                     # ax.annotate("", xy=(s_p[0], s_p[1]),
                     #             xytext=(s_0[0], s_0[1]),
                     #             arrowprops=dict(arrowstyle="->", color='r', lw=3,
                     #                             connectionstyle="arc3"))
 
                 elif ele_load_type == '-beamUniform':
 
                     n_ele_load_data = len(ele_load_data_i)
 
                     # constant uniform element load
                     if n_ele_load_data == 3:
                         # eload_type, Wy, Wx = ele_load_data[0], ele_load_data[1], ele_load_data[2]
                         Wy, Wx = ele_load_data_i[1], ele_load_data_i[2]
-                        text_string = f'q = {Wy}, {Wx}'
+                        text_string = f'q = {abs(Wy)}, {abs(Wx)}'
 
                         # s = sfac * Wy * one
                         s = sfac * one * np.sign(Wy)
-                        # plt.text(sum(ex)/2, sum(ey)/2, f'q = {Wy}, {Wx}', va='bottom', ha='center', color='r')
+                        # plt.text(sum(ecrd[:, 0])/2, sum(ecrd[:, 1])/2, f'q = {Wy}, {Wx}', va='bottom', ha='center', color='r')
 
                     # triangular or trapezoidal element load
                     elif n_ele_load_data == 7:
                         wta, waa, aL, bL, wtb, wab = ele_load_data_i[1:7]
-                        text_string = f'q = {wta}, {waa}, {aL}, {bL}, {wtb}, {wab}'
+                        text_string = f'q = {abs(wta)}, {abs(waa)}, {aL}, {bL}, {abs(wtb)}, {abs(wab)}'
                         a, b = aL * L, bL * L
                         bma = b - a
                         s = np.zeros(nep)
 
                         indx = 0
                         for x in np.nditer(xl):
                             xma = x - a
@@ -1259,15 +1395,16 @@
                                 pass
 
                             indx += 1
 
                     s = s * sfac
 
                     s_0 = np.zeros((nep, 2))
-                    s_0[0, :] = [ex[0], ey[0]]
+                    # s_0[0, :] = [ex[0], ey[0]]
+                    s_0[0, :] = [ecrd_eles[0, 0], ecrd_eles[0, 1]]
 
                     s_0[1:, 0] = s_0[0, 0] + xl[1:] * cosa
                     s_0[1:, 1] = s_0[0, 1] + xl[1:] * cosb
 
                     s_p = np.copy(s_0)
 
                     s_p[:, 0] -= s * cosb
@@ -1288,15 +1425,15 @@
                         # ax.annotate("", xy=(s_p[i, 0], s_p[i, 1]),
                         #             xytext=(s_0[i, 0], s_0[i, 1]),
                         #             arrowprops=dict(arrowstyle="->", color='r', lw=1,
                         #                             connectionstyle="arc3"))
 
                     # connecting beg-end line - redundant ?
                     # plt.plot([s_p[0, 0], s_p[-1, 0]],[s_p[0, 1], s_p[-1, 1]], 'r')
-                    ax.text(sum(ex)/2, sum(ey)/2, text_string, va='bottom', ha='center', color='r')
+                    ax.text(sum(ecrd_eles[:, 0])/2, sum(ecrd_eles[:, 1])/2, text_string, va='bottom', ha='center', color='r')
 
                     if Wx != 0:
                         # for i, xl in enumerate(xl2[:-1]):
                         #     plt.arrow(sa[i, 0], sa[i, 1],
                         #               sa[i+1, 0]-sa[i, 0], sa[i+1, 1]-sa[i, 1],
                         #               width = 0.01,
                         #               # lw = 1,
@@ -1308,15 +1445,16 @@
 
                         ax.quiver(s_0[:-1, 0], s_0[:-1, 1],
                                   s_0[1:, 0]-s_0[:-1, 0], s_0[1:, 1]-s_0[:-1, 1],
                                   scale_units='xy', angles='xy', scale=0.8, color='m')
 
                     if waa != 0 or wab != 0:
                         sa = np.zeros((5, 2))
-                        sa[0, :] = [ex[0], ey[0]]
+                        # sa[0, :] = [ex[0], ey[0]]
+                        sa[0, :] = [ecrd_eles[0, 0], ecrd_eles[0, 1]]
                         sa[1:, 0] = sa[0, 0] + xl3[1:] * cosa
                         sa[1:, 1] = sa[0, 1] + xl3[1:] * cosb
 
                         for i, xl in enumerate(xl3[:-1]):
                             ax.arrow(sa[i, 0], sa[i, 1],
                                      sa[i+1, 0]-sa[i, 0], sa[i+1, 1]-sa[i, 1],
                                      # width = 0.05,
@@ -1342,15 +1480,15 @@
                         #              xytext=(s_0[i, 0], s_0[i, 1]), textcoords='data',
                         #              arrowprops=dict(arrowstyle="->", color='r', lw=2,
                         #                              connectionstyle="arc3"))
 
     for node_tag in node_tags:
         nd_crd = ops.nodeCoord(node_tag)
 
-        # 2. nodal loads
+        # 2. nodal loads 2d
         nodal_loads = ops.nodeUnbalance(node_tag)
         nodal_loads_idx = np.nonzero(nodal_loads)
 
         if nodal_loads_idx[0].size:
             for kier in nodal_loads_idx[0]:
                 # horizontal or vertical nodal force (load)
                 if kier == 0 or kier == 1:
@@ -1377,30 +1515,30 @@
                              # width = 0.01,
                              # head_starts_at_zero=True,  # default False
                              # overhang=0.2,
                              lw=3,
                              head_width=0.1*sfac, head_length=0.2*sfac,
                              fc='b', ec='b',
                              length_includes_head=True, shape='full')
-                    ax.text(nd_crd[0]+dx, nd_crd[1]+dy, f' {nodal_loads[kier]:.5g}', color='b')
+                    ax.text(nd_crd[0]+dx, nd_crd[1]+dy, f' {abs(nodal_loads[kier]):.5g}', color='b')
 
                 # concentrated bending moment
                 elif kier == 2:
                     kier2 = np.sign(nodal_loads[kier])
                     if kier2 > 0:
                         pos_or_neg = 'anti-clockwise'
                         # marker_type=r'$\circlearrowleft$'
                         marker_type=r'$\curvearrowleft$'
                     elif kier2 < 0:
                         pos_or_neg = 'clockwise'
                         # marker_type=r'$\circlearrowright$'
                         marker_type=r'$\curvearrowright$'
 
                     ax.plot(nd_crd[0], nd_crd[1], marker=marker_type, markersize=35, color='b')
-                    ax.text(nd_crd[0], nd_crd[1], f'{nodal_loads[kier]:.5g}', color='b', va='bottom', ha='left')
+                    ax.text(nd_crd[0], nd_crd[1], f'{abs(nodal_loads[kier]):.5g}', color='b', va='bottom', ha='left')
 
     ax.axis('equal')
     ax.grid(False)
 
     return ax
 
 
@@ -1578,63 +1716,59 @@
     ax.set_ylabel('Y')
     ax.set_zlabel('Z')
 
     ax.view_init(azim=azim, elev=elev)
 
     for i, ele_tag in enumerate(ele_tags):
 
-        nd1, nd2 = ops.eleNodes(ele_tag)
-
-        # element x, y coordinates
-        ex = np.array([ops.nodeCoord(nd1)[0],
-                       ops.nodeCoord(nd2)[0]])
-        ey = np.array([ops.nodeCoord(nd1)[1],
-                       ops.nodeCoord(nd2)[1]])
-        ez = np.array([ops.nodeCoord(nd1)[2],
-                       ops.nodeCoord(nd2)[2]])
+        ele_node_tags = ops.eleNodes(ele_tag)
+        nen = 2
+        ecrd = np.zeros((nen, 3))
+        for i, ele_node_tag in enumerate(ele_node_tags):
+            ecrd[i, :] = ops.nodeCoord(ele_node_tag)
 
         # mesh outline
-        ax.plot(ex, ey, ez, 'k--', solid_capstyle='round',
+        ax.plot(ecrd[:, 0], ecrd[:, 1], ecrd[:, 2], 'k--', solid_capstyle='round',
                 solid_joinstyle='round', dash_capstyle='butt',
                 dash_joinstyle='round')
 
         # eo = Eo[i, :]
         xloc = ops.eleResponse(ele_tag, 'xlocal')
         yloc = ops.eleResponse(ele_tag, 'ylocal')
         zloc = ops.eleResponse(ele_tag, 'zlocal')
         g = np.vstack((xloc, yloc, zloc))
 
-        G, L = rot_transf_3d(ex, ey, ez, g)
+        G, L = rot_transf_3d(ecrd, g)
 
         # by default empty
         shape_type, shape_args = ['circ', [0.]]
         if ele_tag in ele_shapes:
             shape_type, shape_args = ele_shapes[ele_tag]
 
         if shape_type == 'rect' or shape_type == 'I':
             if shape_type == 'rect':
-                verts = _plot_extruded_shapes_3d_rect(ex, ey, ez, g,
+                verts = _plot_extruded_shapes_3d_rect(ecrd, g,
                                                       shape_args)
 
             elif shape_type == 'I':
-                verts = _plot_extruded_shapes_3d_double_T(ex, ey, ez, g,
+                verts = _plot_extruded_shapes_3d_double_T(ecrd, g,
                                                           shape_args)
 
             # plot 3d sides
             ax.add_collection3d(Poly3DCollection(verts, linewidths=0.6,
                                                  edgecolors='k', alpha=.25))
 
         elif shape_type == 'circ':
-            X, Y, Z = _plot_extruded_shapes_3d_circ(ex, ey, ez, g,
+            X, Y, Z = _plot_extruded_shapes_3d_circ(ecrd, g,
                                                     shape_args)
             ax.plot_surface(X, Y, Z, linewidths=0.4, edgecolors='k',
                             alpha=.25)
 
         # common for all members
-        Xm, Ym, Zm = sum(ex)/2, sum(ey)/2, sum(ez)/2
+        Xm, Ym, Zm = sum(ecrd[:, 0]) / 2, sum(ecrd[:, 1]) / 2, sum(ecrd[:, 2]) / 2
 
         alen = 0.1*L
 
         # plot local axis directional vectors: workaround quiver = arrow
         ax.quiver(Xm, Ym, Zm, g[0, 0], g[0, 1], g[0, 2], color='g',
                   lw=2, length=alen, alpha=.8, normalize=True)
         ax.quiver(Xm, Ym, Zm, g[1, 0], g[1, 1], g[1, 2], color='b',
@@ -1643,60 +1777,60 @@
                   lw=2, length=alen, alpha=.8, normalize=True)
 
     ax.set_box_aspect((np.ptp(ax.get_xlim3d()),
                        np.ptp(ax.get_ylim3d()),
                        np.ptp(ax.get_zlim3d())))
 
 
-def _plot_extruded_shapes_3d_double_T(ex, ey, ez, g, shape_args):
+def _plot_extruded_shapes_3d_double_T(ecrd, g, shape_args):
     bf, d, tw, tf = shape_args
 
-    za, zb = tw/2, bf/2
-    ya, yb = d/2 - tf, d/2
+    za, zb = tw / 2, bf / 2
+    ya, yb = d / 2 - tf, d / 2
 
-    g10a, g11a, g12a = g[1, 0]*ya, g[1, 1]*ya, g[1, 2]*ya
-    g10b, g11b, g12b = g[1, 0]*yb, g[1, 1]*yb, g[1, 2]*yb
+    g10a, g11a, g12a = g[1, 0] * ya, g[1, 1] * ya, g[1, 2] * ya
+    g10b, g11b, g12b = g[1, 0] * yb, g[1, 1] * yb, g[1, 2] * yb
 
-    g20a, g21a, g22a = g[2, 0]*za, g[2, 1]*za, g[2, 2]*za
-    g20b, g21b, g22b = g[2, 0]*zb, g[2, 1]*zb, g[2, 2]*zb
+    g20a, g21a, g22a = g[2, 0] * za, g[2, 1] * za, g[2, 2] * za
+    g20b, g21b, g22b = g[2, 0] * zb, g[2, 1] * zb, g[2, 2] * zb
 
     pts = np.zeros((24, 3))
     # beg node (I) cross-section vertices crds, counter-clockwise order
-    pts[0] = [ex[0] - g10b - g20b, ey[0] - g11b - g21b, ez[0] - g12b - g22b]
-    pts[1] = [ex[0] - g10a - g20b, ey[0] - g11a - g21b, ez[0] - g12a - g22b]
-    pts[2] = [ex[0] - g10a - g20a, ey[0] - g11a - g21a, ez[0] - g12a - g22a]
-
-    pts[3] = [ex[0] + g10a - g20a, ey[0] + g11a - g21a, ez[0] + g12a - g22a]
-    pts[4] = [ex[0] + g10a - g20b, ey[0] + g11a - g21b, ez[0] + g12a - g22b]
-    pts[5] = [ex[0] + g10b - g20b, ey[0] + g11b - g21b, ez[0] + g12b - g22b]
-
-    pts[6] = [ex[0] + g10b + g20b, ey[0] + g11b + g21b, ez[0] + g12b + g22b]
-    pts[7] = [ex[0] + g10a + g20b, ey[0] + g11a + g21b, ez[0] + g12a + g22b]
-    pts[8] = [ex[0] + g10a + g20a, ey[0] + g11a + g21a, ez[0] + g12a + g22a]
-
-    pts[9] = [ex[0] - g10a + g20a, ey[0] - g11a + g21a, ez[0] - g12a + g22a]
-    pts[10] = [ex[0] - g10a + g20b, ey[0] - g11a + g21b, ez[0] - g12a + g22b]
-    pts[11] = [ex[0] - g10b + g20b, ey[0] - g11b + g21b, ez[0] - g12b + g22b]
+    pts[0] = [ecrd[0, 0] - g10b - g20b, ecrd[0, 1] - g11b - g21b, ecrd[0, 2] - g12b - g22b]
+    pts[1] = [ecrd[0, 0] - g10a - g20b, ecrd[0, 1] - g11a - g21b, ecrd[0, 2] - g12a - g22b]
+    pts[2] = [ecrd[0, 0] - g10a - g20a, ecrd[0, 1] - g11a - g21a, ecrd[0, 2] - g12a - g22a]
+
+    pts[3] = [ecrd[0, 0] + g10a - g20a, ecrd[0, 1] + g11a - g21a, ecrd[0, 2] + g12a - g22a]
+    pts[4] = [ecrd[0, 0] + g10a - g20b, ecrd[0, 1] + g11a - g21b, ecrd[0, 2] + g12a - g22b]
+    pts[5] = [ecrd[0, 0] + g10b - g20b, ecrd[0, 1] + g11b - g21b, ecrd[0, 2] + g12b - g22b]
+
+    pts[6] = [ecrd[0, 0] + g10b + g20b, ecrd[0, 1] + g11b + g21b, ecrd[0, 2] + g12b + g22b]
+    pts[7] = [ecrd[0, 0] + g10a + g20b, ecrd[0, 1] + g11a + g21b, ecrd[0, 2] + g12a + g22b]
+    pts[8] = [ecrd[0, 0] + g10a + g20a, ecrd[0, 1] + g11a + g21a, ecrd[0, 2] + g12a + g22a]
+
+    pts[9] = [ecrd[0, 0] - g10a + g20a, ecrd[0, 1] - g11a + g21a, ecrd[0, 2] - g12a + g22a]
+    pts[10] = [ecrd[0, 0] - g10a + g20b, ecrd[0, 1] - g11a + g21b, ecrd[0, 2] - g12a + g22b]
+    pts[11] = [ecrd[0, 0] - g10b + g20b, ecrd[0, 1] - g11b + g21b, ecrd[0, 2] - g12b + g22b]
 
     # end node (J) cross-section vertices
-    pts[12] = [ex[1] - g10b - g20b, ey[1] - g11b - g21b, ez[1] - g12b - g22b]
-    pts[13] = [ex[1] - g10a - g20b, ey[1] - g11a - g21b, ez[1] - g12a - g22b]
-    pts[14] = [ex[1] - g10a - g20a, ey[1] - g11a - g21a, ez[1] - g12a - g22a]
-
-    pts[15] = [ex[1] + g10a - g20a, ey[1] + g11a - g21a, ez[1] + g12a - g22a]
-    pts[16] = [ex[1] + g10a - g20b, ey[1] + g11a - g21b, ez[1] + g12a - g22b]
-    pts[17] = [ex[1] + g10b - g20b, ey[1] + g11b - g21b, ez[1] + g12b - g22b]
-
-    pts[18] = [ex[1] + g10b + g20b, ey[1] + g11b + g21b, ez[1] + g12b + g22b]
-    pts[19] = [ex[1] + g10a + g20b, ey[1] + g11a + g21b, ez[1] + g12a + g22b]
-    pts[20] = [ex[1] + g10a + g20a, ey[1] + g11a + g21a, ez[1] + g12a + g22a]
-
-    pts[21] = [ex[1] - g10a + g20a, ey[1] - g11a + g21a, ez[1] - g12a + g22a]
-    pts[22] = [ex[1] - g10a + g20b, ey[1] - g11a + g21b, ez[1] - g12a + g22b]
-    pts[23] = [ex[1] - g10b + g20b, ey[1] - g11b + g21b, ez[1] - g12b + g22b]
+    pts[12] = [ecrd[1, 0] - g10b - g20b, ecrd[1, 1] - g11b - g21b, ecrd[1, 2] - g12b - g22b]
+    pts[13] = [ecrd[1, 0] - g10a - g20b, ecrd[1, 1] - g11a - g21b, ecrd[1, 2] - g12a - g22b]
+    pts[14] = [ecrd[1, 0] - g10a - g20a, ecrd[1, 1] - g11a - g21a, ecrd[1, 2] - g12a - g22a]
+
+    pts[15] = [ecrd[1, 0] + g10a - g20a, ecrd[1, 1] + g11a - g21a, ecrd[1, 2] + g12a - g22a]
+    pts[16] = [ecrd[1, 0] + g10a - g20b, ecrd[1, 1] + g11a - g21b, ecrd[1, 2] + g12a - g22b]
+    pts[17] = [ecrd[1, 0] + g10b - g20b, ecrd[1, 1] + g11b - g21b, ecrd[1, 2] + g12b - g22b]
+
+    pts[18] = [ecrd[1, 0] + g10b + g20b, ecrd[1, 1] + g11b + g21b, ecrd[1, 2] + g12b + g22b]
+    pts[19] = [ecrd[1, 0] + g10a + g20b, ecrd[1, 1] + g11a + g21b, ecrd[1, 2] + g12a + g22b]
+    pts[20] = [ecrd[1, 0] + g10a + g20a, ecrd[1, 1] + g11a + g21a, ecrd[1, 2] + g12a + g22a]
+
+    pts[21] = [ecrd[1, 0] - g10a + g20a, ecrd[1, 1] - g11a + g21a, ecrd[1, 2] - g12a + g22a]
+    pts[22] = [ecrd[1, 0] - g10a + g20b, ecrd[1, 1] - g11a + g21b, ecrd[1, 2] - g12a + g22b]
+    pts[23] = [ecrd[1, 0] - g10b + g20b, ecrd[1, 1] - g11b + g21b, ecrd[1, 2] - g12b + g22b]
 
     # list of sides
     verts = [[pts[0], pts[1], pts[2], pts[3], pts[4], pts[5], pts[6],
               pts[7], pts[8], pts[9], pts[10], pts[11]],  # beg
              [pts[12], pts[13], pts[14], pts[15], pts[16], pts[17],
               pts[18], pts[19], pts[20], pts[21], pts[22], pts[23]],  # end
              [pts[0], pts[12], pts[23], pts[11]],  # bot 1
@@ -1711,91 +1845,91 @@
              [pts[2], pts[1], pts[13], pts[14]],  # 10
              [pts[7], pts[8], pts[20], pts[19]],  # 11
              [pts[3], pts[4], pts[16], pts[15]]]  # 12
 
     return verts
 
 
-def _plot_extruded_shapes_3d_rect(ex, ey, ez, g, shape_args):
+def _plot_extruded_shapes_3d_rect(ecrd, g, shape_args):
     b, d = shape_args
-    b2, d2 = b/2, d/2
+    b2, d2 = b / 2, d / 2
 
-    g10, g11, g12 = g[1, 0]*d2, g[1, 1]*d2, g[1, 2]*d2
-    g20, g21, g22 = g[2, 0]*b2, g[2, 1]*b2, g[2, 2]*b2
+    g10, g11, g12 = g[1, 0] * d2, g[1, 1] * d2, g[1, 2] * d2
+    g20, g21, g22 = g[2, 0] * b2, g[2, 1] * b2, g[2, 2] * b2
 
     pts = np.zeros((8, 3))
     # beg node cross-section vertices
     # collected i-beg, j-end node coordinates, counter-clockwise order
-    pts[0] = [ex[0] - g10 - g20, ey[0] - g11 - g21, ez[0] - g12 - g22]
-    pts[1] = [ex[0] + g10 - g20, ey[0] + g11 - g21, ez[0] + g12 - g22]
-    pts[2] = [ex[0] + g10 + g20, ey[0] + g11 + g21, ez[0] + g12 + g22]
-    pts[3] = [ex[0] - g10 + g20, ey[0] - g11 + g21, ez[0] - g12 + g22]
+    pts[0] = [ecrd[0, 0] - g10 - g20, ecrd[0, 1] - g11 - g21, ecrd[0, 2] - g12 - g22]
+    pts[1] = [ecrd[0, 0] + g10 - g20, ecrd[0, 1] + g11 - g21, ecrd[0, 2] + g12 - g22]
+    pts[2] = [ecrd[0, 0] + g10 + g20, ecrd[0, 1] + g11 + g21, ecrd[0, 2] + g12 + g22]
+    pts[3] = [ecrd[0, 0] - g10 + g20, ecrd[0, 1] - g11 + g21, ecrd[0, 2] - g12 + g22]
     # end node cross-section vertices
-    pts[4] = [ex[1] - g10 - g20, ey[1] - g11 - g21, ez[1] - g12 - g22]
-    pts[5] = [ex[1] + g10 - g20, ey[1] + g11 - g21, ez[1] + g12 - g22]
-    pts[6] = [ex[1] + g10 + g20, ey[1] + g11 + g21, ez[1] + g12 + g22]
-    pts[7] = [ex[1] - g10 + g20, ey[1] - g11 + g21, ez[1] - g12 + g22]
+    pts[4] = [ecrd[1, 0] - g10 - g20, ecrd[1, 1] - g11 - g21, ecrd[1, 2] - g12 - g22]
+    pts[5] = [ecrd[1, 0] + g10 - g20, ecrd[1, 1] + g11 - g21, ecrd[1, 2] + g12 - g22]
+    pts[6] = [ecrd[1, 0] + g10 + g20, ecrd[1, 1] + g11 + g21, ecrd[1, 2] + g12 + g22]
+    pts[7] = [ecrd[1, 0] - g10 + g20, ecrd[1, 1] - g11 + g21, ecrd[1, 2] - g12 + g22]
 
     # list of 4-node sides
     verts = [[pts[0], pts[1], pts[2], pts[3]],  # beg
              [pts[4], pts[5], pts[6], pts[7]],  # end
              [pts[0], pts[4], pts[5], pts[1]],  # bottom
              [pts[3], pts[7], pts[6], pts[2]],  # top
              [pts[0], pts[4], pts[7], pts[3]],  # front
              [pts[1], pts[5], pts[6], pts[2]]]  # back
 
     return verts
 
 
-def _plot_extruded_shapes_3d_circ(ex, ey, ez, g, shape_args):
+def _plot_extruded_shapes_3d_circ(ecrd, g, shape_args):
     d = shape_args[0]
-    r = d/2
+    r = d / 2
 
-    Lxyz = np.array([ex[1]-ex[0], ey[1]-ey[0], ez[1]-ez[0]])
+    Lxyz = ecrd[1, :] - ecrd[0, :]
     L = np.sqrt(Lxyz @ Lxyz)
 
     xl = np.linspace(0, L, 3)  # subdivde member length
     alpha = np.linspace(0, 2 * np.pi, 10)  # subdivide circle
 
     xl, alpha = np.meshgrid(xl, alpha)
-    X = (ex[0] + g[0, 0] * xl + r * np.sin(alpha) * g[1, 0]
+    X = (ecrd[0, 0] + g[0, 0] * xl + r * np.sin(alpha) * g[1, 0]
          + r * np.cos(alpha) * g[2, 0])
-    Y = (ey[0] + g[0, 1] * xl + r * np.sin(alpha) * g[1, 1]
+    Y = (ecrd[0, 1] + g[0, 1] * xl + r * np.sin(alpha) * g[1, 1]
          + r * np.cos(alpha) * g[2, 1])
-    Z = (ez[0] + g[0, 2] * xl + r * np.sin(alpha) * g[1, 2]
+    Z = (ecrd[0, 2] + g[0, 2] * xl + r * np.sin(alpha) * g[1, 2]
          + r * np.cos(alpha) * g[2, 2])
 
     return X, Y, Z
 
 
-def bar_length(ex, ey, ez=np.array([0., 0.])):
-    Lxyz = np.array([ex[1]-ex[0], ey[1]-ey[0], ez[1]-ez[0]])
+def bar_length(ecrd):
+    Lxyz = ecrd[1, :] - ecrd[0, :]
     L = np.sqrt(Lxyz @ Lxyz)
 
     return L
 
 
-def rot_transf_2d(ex, ey):
+def rot_transf_2d(ecrd):
 
-    Lxy = np.array([ex[1] - ex[0], ey[1] - ey[0]])
+    Lxy = ecrd[1, :] - ecrd[0, :]
     L = np.sqrt(Lxy @ Lxy)
     cosa, cosb = Lxy / L
     G = np.array([[cosa, cosb, 0., 0., 0., 0.],
                   [-cosb, cosa, 0., 0., 0., 0.],
                   [0., 0., 1., 0., 0., 0.],
                   [0., 0., 0., cosa, cosb, 0.],
                   [0., 0., 0., -cosb, cosa, 0.],
                   [0., 0., 0., 0., 0., 1.]])
 
     return G, L, cosa, cosb
 
 
-def rot_transf_3d(ex, ey, ez, g):
+def rot_transf_3d(ecrd, g):
 
-    Lxyz = np.array([ex[1] - ex[0], ey[1] - ey[0], ez[1] - ez[0]])
+    Lxyz = ecrd[1, :] - ecrd[0, :]
     L = np.sqrt(Lxyz @ Lxyz)
 
     z = np.zeros((3, 3))
     G = np.block([[g, z, z, z],
                   [z, g, z, z],
                   [z, z, g, z],
                   [z, z, z, g]])
```

### Comparing `opsvis-1.0.9/opsvis/secforces.py` & `opsvis-1.1.1/opsvis/secforces.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from mpl_toolkits.mplot3d import Axes3D
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 from matplotlib.collections import PolyCollection
 from matplotlib.patches import Circle, Polygon, Wedge
 from matplotlib.animation import FuncAnimation
 import matplotlib.tri as tri
 
-from settings import *
-import model
+from .settings import *
+from . import model
 
 
-def section_force_distribution_2d(ex, ey, pl, nep=2,
+def section_force_distribution_2d(ecrd, pl, nep=2,
                                   ele_load_data=[['-beamUniform', 0., 0.]]):
     """
     Calculate section forces (N, V, M) for an elastic 2D Euler-Bernoulli beam.
 
     Input:
-    ex, ey - x, y element coordinates in global system
+    ecrd - x, y element coordinates in global system
     nep - number of evaluation points, by default (2) at element ends
     ele_load_list - list of transverse and longitudinal element load
       syntax: [ele_load_type, Wy, Wx]
       For now only '-beamUniform' element load type is acceptable
 
     Output:
     s = [N V M]; shape: (nep,3)
@@ -35,21 +35,19 @@
         number of evaluation points, by default (2) at element ends
         If the element load is between the points then nep is increased by 1 or 2
 
     TODO: add '-beamPoint' element load type
     """
 
 
-    Lxy = np.array([ex[1]-ex[0], ey[1]-ey[0]])
+    Lxy = ecrd[1, :] - ecrd[0, :]
     L = np.sqrt(Lxy @ Lxy)
 
     nlf = len(pl)
     xl = np.linspace(0., L, nep)
-    one = np.ones(nep)
-
 
     for ele_load_data_i in ele_load_data:
         ele_load_type = ele_load_data_i[0]
 
         if nlf == 1:  # trusses
             N_1 = pl[0]
         elif nlf == 6:  # plane frames
@@ -64,28 +62,14 @@
 
             n_ele_load_data = len(ele_load_data_i)
 
             if n_ele_load_data == 3:
                 # eload_type, Wy, Wx = ele_load_data[0], ele_load_data[1], ele_load_data[2]
                 Wy, Wx = ele_load_data_i[1], ele_load_data_i[2]
 
-                if nlf == 6:
-                    s = np.zeros((nep, 3))
-                elif nlf == 1:
-                    s = np.zeros((nep, 1))
-
-                N = -1.*(N_1 * one + Wx * xl)
-
-                if nlf == 6:
-                    V = V_1 * one + Wy * xl
-                    M = -M_1 * one + V_1 * xl + 0.5 * Wy * xl**2
-                    s += np.column_stack((N, V, M))
-                elif nlf == 1:
-                    s += np.column_stack((N))
-
             elif n_ele_load_data == 7:
                 wta, waa, aL, bL, wtb, wab = ele_load_data_i[1:7]
                 a, b = aL*L, bL*L
 
                 bma = b - a
 
                 if a in xl:
@@ -95,40 +79,97 @@
                     nep += 1
                 if b in xl:
                     pass
                 else:
                     xl = np.insert(xl, xl.searchsorted(b), b)
                     nep += 1
 
+        elif ele_load_type == '-beamPoint':
+            Pt, aL, Pa = ele_load_data_i[1:4]
+            a = aL * L
+
+            if a in xl:
+                # idx = xl.searchsorted(a)
+                # np.concatenate((xl[:idx], [a], xl[idx:]))
+                xl = np.insert(xl, xl.searchsorted(a+0.001), a+0.001)
+                nep += 1
+
+            else:
+                # idx = xl.searchsorted(a)
+                # xl = np.concatenate((xl[:idx], [a], xl[idx:]))
+                # idx = xl.searchsorted(a+0.001)
+                # xl = np.concatenate((xl[:idx], [a+0.001], xl[idx:]))
+                xl = np.insert(xl, xl.searchsorted(a), a)
+                xl = np.insert(xl, xl.searchsorted(a+0.001), a+0.001)
+                nep += 2
+
+
+    # xl is modified on the fly
+    one = np.ones(nep)
+
+    N = -1. * N_1 * one
+
+    if nlf == 6:
+        # s = np.zeros((nep, 3))
+        V = V_1 * one
+        M = -M_1 * one + V_1 * xl
+        s = np.column_stack((N, V, M))
+
+    elif nlf == 1:
+        # s = np.zeros((nep, 1))
+        s = np.column_stack((N))
+
+    for ele_load_data_i in ele_load_data:
+        ele_load_type = ele_load_data_i[0]
+
+        if ele_load_type == '-beamUniform':
+            # raise ValueError
+            # raise NameError
+
+            n_ele_load_data = len(ele_load_data_i)
+
+            if n_ele_load_data == 3:
+                # eload_type, Wy, Wx = ele_load_data[0], ele_load_data[1], ele_load_data[2]
+                Wy, Wx = ele_load_data_i[1], ele_load_data_i[2]
+
+                N = -1.*(Wx * xl)
+
                 if nlf == 6:
-                    s = np.zeros((nep, 3))
+                    V = Wy * xl
+                    M = 0.5 * Wy * xl**2
+                    s += np.column_stack((N, V, M))
                 elif nlf == 1:
-                    s = np.zeros((nep, 1))
+                    s += np.column_stack((N))
 
+            elif n_ele_load_data == 7:
+                wta, waa, aL, bL, wtb, wab = ele_load_data_i[1:7]
+                a, b = aL*L, bL*L
+
+                bma = b - a
 
                 indx = 0
                 for x in np.nditer(xl):
                     xma = x - a
                     wtx = wta + (wtb - wta) * xma / bma
                     # xc = a + bma * (wtb + 2*wta) / (3 * (wta + wtb))
                     if wtx == 0:
                         xc = 0.
                     else:
                         xc = a + xma * (wtx + 2*wta) / (3 * (wta + wtx))
 
                     Ax = 0.5 * (wtx+wta) * xma
-                    V1x = V_1 * x
+                    # V1x = V_1 * x
                     Axxc = Ax * xc
 
                     if x < a:
                         pass
                     elif x >= a and x <= b:
-                        s[indx, 0] = -1.*(N_1 + (wab - waa) * x)
-                        s[indx, 1] = V_1 + Ax
-                        s[indx, 2] = -M_1 + V1x + Axxc
+                        s[indx, 0] += -1.*((wab - waa) * x)
+                        s[indx, 1] += Ax
+                        s[indx, 2] += Axxc
 
                     elif x > b:
                         pass
 
                     indx += 1
 
                 if aL == 0 and bL == 0:
@@ -137,71 +178,46 @@
                 else:
                     N = 0
 
         elif ele_load_type == '-beamPoint':
             Pt, aL, Pa = ele_load_data_i[1:4]
             a = aL * L
 
-            if a in xl:
-                # idx = xl.searchsorted(a)
-                # np.concatenate((xl[:idx], [a], xl[idx:]))
-                xl = np.insert(xl, xl.searchsorted(a+0.001), a+0.001)
-                nep += 1
-
-            else:
-                # idx = xl.searchsorted(a)
-                # xl = np.concatenate((xl[:idx], [a], xl[idx:]))
-                # idx = xl.searchsorted(a+0.001)
-                # xl = np.concatenate((xl[:idx], [a+0.001], xl[idx:]))
-                xl = np.insert(xl, xl.searchsorted(a), a)
-                xl = np.insert(xl, xl.searchsorted(a+0.001), a+0.001)
-                nep += 2
-
-            if nlf == 6:
-                s = np.zeros((nep, 3))
-            elif nlf == 1:
-                s = np.zeros((nep, 1))
-
-
             indx = 0
             for x in np.nditer(xl):
                 if x <= a:
-                    s[indx, 0] = -1. * N_1
-                    s[indx, 1] = V_1
-                    s[indx, 2] = -M_1 + V_1 * x
+                    pass
+                    # s[indx, 0] += -1. * N_1
+                    # s[indx, 1] += V_1
+                    # s[indx, 2] += -M_1 + V_1 * x
                 elif x > a:
-                    s[indx, 0] = -1. * (N_1 + Pa)
-                    s[indx, 1] = V_1 + Pt
-                    s[indx, 2] = -M_1 + V_1 * x + Pt * (x-a)
+                    s[indx, 0] += -1. * (Pa)
+                    s[indx, 1] += Pt
+                    s[indx, 2] += Pt * (x-a)
 
                 indx += 1
 
-
     # if eload_type == '-beamUniform':
     # else:
 
     return s, xl, nep
 
 
-def section_force_distribution_3d(ex, ey, ez, pl, nep=2,
+def section_force_distribution_3d(ecrd, pl, nep=2,
                                   ele_load_data=[['-beamUniform', 0., 0., 0.]]):
     """
     Calculate section forces (N, Vy, Vz, T, My, Mz) for an elastic 3d beam.
 
     Longer description
 
     Parameters
     ----------
 
-    ex : list
-        x element coordinates
-    ey : list
-        y element coordinates
-    ez : list
-        z element coordinates
+    ecrd : ndarray
+        x, y, z element coordinates
     pl : ndarray
     nep : int
         number of evaluation points, by default (2) at element ends
 
     ele_load_list : list
         list of transverse and longitudinal element load
         syntax: [ele_load_type, Wy, Wz, Wx]
@@ -227,122 +243,116 @@
 
     Notes
     -----
 
     Todo: add '-beamPoint' element load type
 
     """
-
-
-    Lxyz = np.array([ex[1]-ex[0], ey[1]-ey[0], ez[1]-ez[0]])
+    Lxyz = ecrd[1, :] - ecrd[0, :]
     L = np.sqrt(Lxyz @ Lxyz)
 
     nlf = len(pl)
     xl = np.linspace(0., L, nep)
-    one = np.ones(nep)
-
 
     for ele_load_data_i in ele_load_data:
         ele_load_type = ele_load_data_i[0]
 
-        if nlf == 1:  # trusses
-            N_1 = pl[0]
-        elif nlf == 12:  # plane frames
-            # N_1, V_1, M_1 = pl[0], pl[1], pl[2]
-            # N_1, V_1, M_1 = pl[:3]
+        if nlf == 1:
+            N1 = pl[0]
+        elif nlf == 12:
             N1, Vy1, Vz1, T1, My1, Mz1 = pl[:6]
         else:
             print('\nWarning! Not supported. Number of nodal forces: {nlf}')
 
         if ele_load_type == '-beamUniform':
-            # raise ValueError
-            # raise NameError
-
             n_ele_load_data = len(ele_load_data_i)
 
             if n_ele_load_data == 4:
-                # eload_type, Wy, Wx = ele_load_data[0], ele_load_data[1], ele_load_data[2]
-                Wy, Wz, Wx = ele_load_data_i[1], ele_load_data_i[2], ele_load_data_i[3]
-                # Wy, Wx = ele_load_data_i[1], ele_load_data_i[2]
-
-                # eload_type = ele_load_data[0]
-
-                if nlf == 12:
-                    s = np.zeros((nep, 3))
-                elif nlf == 1:
-                    s = np.zeros((nep, 1))
-
-                N = -1. * (N1 * one + Wx * xl)
-
-                if nlf == 12:
-                    Vy = Vy1 * one + Wy * xl
-                    Vz = Vz1 * one + Wz * xl
-                    T = -T1 * one
-                    Mz = -Mz1 * one + Vy1 * xl + 0.5 * Wy * xl**2
-                    My = -My1 * one - Vz1 * xl - 0.5 * Wz * xl**2
-
-                    s = np.column_stack((N, Vy, Vz, T, My, Mz))
-
-                elif nlf == 1:
-                    s += np.column_stack((N))
+                pass
 
         elif ele_load_type == '-beamPoint':
             Py, Pz, aL, Px = ele_load_data_i[1:5]
             a = aL * L
 
             if a in xl:
-                # idx = xl.searchsorted(a)
-                # np.concatenate((xl[:idx], [a], xl[idx:]))
                 xl = np.insert(xl, xl.searchsorted(a+0.001), a+0.001)
                 nep += 1
 
             else:
-                # idx = xl.searchsorted(a)
-                # xl = np.concatenate((xl[:idx], [a], xl[idx:]))
-                # idx = xl.searchsorted(a+0.001)
-                # xl = np.concatenate((xl[:idx], [a+0.001], xl[idx:]))
                 xl = np.insert(xl, xl.searchsorted(a), a)
                 xl = np.insert(xl, xl.searchsorted(a+0.001), a+0.001)
                 nep += 2
 
-            if nlf == 12:
-                s = np.zeros((nep, 6))
-            elif nlf == 1:
-                s = np.zeros((nep, 1))
+    one = np.ones(nep)
+
+    N = -1. * (N1 * one)
+
+    if nlf == 12:
+        Vy = Vy1 * one
+        Vz = Vz1 * one
+        T = -T1 * one
+        Mz = -Mz1 * one + Vy1 * xl
+        My = -My1 * one - Vz1 * xl
+
+        s = np.column_stack((N, Vy, Vz, T, My, Mz))
+
+    elif nlf == 1:
+        s = np.column_stack((N))
+
+    for ele_load_data_i in ele_load_data:
+        ele_load_type = ele_load_data_i[0]
+
+        if ele_load_type == '-beamUniform':
+            n_ele_load_data = len(ele_load_data_i)
+
+            if n_ele_load_data == 4:
+                Wy, Wz, Wx = ele_load_data_i[1:4]
 
+                N = -1. * (Wx * xl)
+
+                if nlf == 12:
+                    Vy = Wy * xl
+                    Vz = Wz * xl
+                    T = np.zeros_like(one)
+                    Mz = 0.5 * Wy * xl**2
+                    My = -0.5 * Wz * xl**2
+
+                    s += np.column_stack((N, Vy, Vz, T, My, Mz))
+
+                elif nlf == 1:
+                    s += np.column_stack((N))
+
+        elif ele_load_type == '-beamPoint':
+            Py, Pz, aL, Px = ele_load_data_i[1:5]
+            a = aL * L
 
             indx = 0
             for x in np.nditer(xl):
                 if x <= a:
-                    s[indx, 0] = -1. * N1  # N
-                    s[indx, 1] = Vy1  # Vy
-                    s[indx, 2] = Vz1  # Vz
-                    s[indx, 3] = -T1  # T
-                    s[indx, 4] = -My1 - Vz1 * x  # My
-                    s[indx, 5] = -Mz1 + Vy1 * x  # Mz
+                    pass
                 elif x > a:
-                    s[indx, 0] = -1. * (N1 + Px)  # N
-                    s[indx, 1] = Vy1 + Py  # Vy
-                    s[indx, 2] = Vz1 + Pz  # Vz
-                    s[indx, 3] = -T1  # T
-                    s[indx, 4] = -My1 - Vz1 * x - Pz * (x-a)  # My
-                    s[indx, 5] = -Mz1 + Vy1 * x + Py * (x-a)  # Mz
+                    s[indx, 0] += -1. * Px
+                    s[indx, 1] += Py
+                    s[indx, 2] += Pz
+                    s[indx, 4] += - Pz * (x - a)
+                    s[indx, 5] += Py * (x - a)
 
                 indx += 1
 
     return s, xl, nep
 
 
 def section_force_diagram_2d(sf_type, sfac=1., nep=17,
                              fmt_secforce1=fmt_secforce1,
                              fmt_secforce2=fmt_secforce2,
                              fig_wi_he=False, fig_lbrt=False,
                              ref_vert_lines=True,
                              end_max_values=True,
-                             node_supports=True, ax=False):
+                             node_supports=True, ax=False,
+                             alt_model_plot=1):
     """Display section forces diagram for 2d beam column model.
 
     This function plots a section forces diagram for 2d beam column elements
     with or without element loads. For now only '-beamUniform' constant
     transverse or axial element loads are supported.
 
     Args:
@@ -369,15 +379,28 @@
 
         end_max_values (bool): True means show the values at element ends and
             extreme (max, min) value between the ends.
 
         node_supports (bool): True - show the supports.
             Default: True.
 
-        ax: axis object.
+        ax: the axes object.
+
+    Returns:
+        minVal (float): the minimum overall value of the section force.
+
+        maxVal (float): the maximum overall value of the section force.
+
+        ax: the axes object.
+
+        alt_model_plot (int): 1 - for using the plot_model command,  2 - for using
+            simplified model plotting. Other integer - for no model plotting.
+            In this case the model can be plotted outside this command
+            using the axes (ax) object. Default is 1.
+
     Usage:
         See example: demo_portal_frame.py
     """
 
     if not ax:
         if fig_wi_he:
             fig_wi, fig_he = fig_wi_he
@@ -385,118 +408,156 @@
         else:
             fig, ax = plt.subplots()
 
         if fig_lbrt:
             fleft, fbottom, fright, ftop = fig_lbrt
             fig.subplots_adjust(left=fleft, bottom=fbottom, right=fright, top=ftop)
 
-    ax = model.plot_model(node_labels=0, element_labels=0,
-                          fmt_model=fmt_model_secforce,
-                          node_supports=False, ax=ax)
+    if alt_model_plot == 1:
+        ax = model.plot_model(node_labels=0, element_labels=0,
+                              fmt_model=fmt_model_secforce,
+                              node_supports=False,
+                              fmt_model_truss=fmt_model_secforce,
+                              truss_node_offset=0, ax=ax)
+    else:
+        pass
 
+    fmt_secforce1_orig = fmt_secforce1
     maxVal, minVal = -np.inf, np.inf
     ele_tags = ops.getEleTags()
 
     Ew = model.get_Ew_data_from_ops_domain()
 
     for ele_tag in ele_tags:
 
         ele_class_tag = ops.getEleClassTags(ele_tag)[0]
 
-        if (ele_class_tag == EleClassTag.ElasticBeam2d or
-            ele_class_tag == EleClassTag.ForceBeamColumn2d or
-            ele_class_tag == EleClassTag.DispBeamColumn2d or
-            ele_class_tag == EleClassTag.truss):
-
-            nd1, nd2 = ops.eleNodes(ele_tag)
-
-            # element x, y coordinates
-            ex = np.array([ops.nodeCoord(nd1)[0],
-                           ops.nodeCoord(nd2)[0]])
-            ey = np.array([ops.nodeCoord(nd1)[1],
-                           ops.nodeCoord(nd2)[1]])
+        if (ele_class_tag == EleClassTag.ElasticBeam2d
+            or ele_class_tag == EleClassTag.ForceBeamColumn2d
+            or ele_class_tag == EleClassTag.DispBeamColumn2d
+            or ele_class_tag in [EleClassTag.truss, EleClassTag.trussSection]
+            or ele_class_tag == EleClassTag.TimoshenkoBeamColumn2d
+            or ele_class_tag == EleClassTag.ElasticTimoshenkoBeam2d):
+
+            ele_node_tags = ops.eleNodes(ele_tag)
+            ecrd = np.zeros((2, 2))
+            for i, ele_node_tag in enumerate(ele_node_tags):
+                ecrd[i, :] = ops.nodeCoord(ele_node_tag)
 
-            Lxy = np.array([ex[1]-ex[0], ey[1]-ey[0]])
+            Lxy = ecrd[1, :] - ecrd[0, :]
             L = np.sqrt(Lxy @ Lxy)
             cosa, cosb = Lxy / L
 
-            if ele_class_tag == EleClassTag.truss:
-                axial_force = ops.eleResponse(ele_tag, 'axialForce')[0]
-                ss = -axial_force * np.ones(nep)
-                xl = np.linspace(0., L, nep)
-
-                if axial_force > 0:
-                    va = 'top'
-                    fmt_color = 'b'
-                    fmt_secforce1 = fmt_secforce_tension
-                else:
-                    va = 'bottom'
-                    fmt_color = 'r'
-                    fmt_secforce1 = fmt_secforce_compression
+            if ele_class_tag in [EleClassTag.truss, EleClassTag.trussSection]:
+                if sf_type == 'N' or sf_type == 'axial':
+                    axial_force = ops.eleResponse(ele_tag, 'axialForce')[0]
+                    ss = -axial_force * np.ones(nep)
+                    xl = np.linspace(0., L, nep)
+
+                    if axial_force > 0:
+                        va = 'top'
+                        fmt_color = 'b'
+                        fmt_secforce1 = fmt_secforce_tension
+                    else:
+                        va = 'bottom'
+                        fmt_color = 'r'
+                        fmt_secforce1 = fmt_secforce_compression
+
+                else:  # for sf_type = 'V' or 'M'
+                    xl = np.linspace(0., L, 2)
+                    ss = np.zeros(2)
 
-            else:
+            else:  # for other elements than truss
                 # by default no element load
                 eload_data = [['-beamUniform', 0., 0.]]
                 if ele_tag in Ew:
                     eload_data = Ew[ele_tag]
 
                 pl = ops.eleResponse(ele_tag, 'localForces')
 
-                s_all, xl, nep = section_force_distribution_2d(ex, ey, pl, nep, eload_data)
+                # rigid offsets for 2d
+                ele_offsets = np.array(ops.eleResponse(ele_tag, 'offsets'))
+                nz_offsets = np.nonzero(ele_offsets)[0]  # tuple of arrays
+                if np.any(nz_offsets):
+                    # modify ecrd_eles
+                    # ex += ele_offsets[[0, 3]]
+                    # ey += ele_offsets[[1, 4]]
+                    ecrd[:, 0] += ele_offsets[[0, 3]]
+                    ecrd[:, 1] += ele_offsets[[1, 4]]
+                    # modify the following due to rigid offsets
+                    # Lxy = np.array([ex[1]-ex[0], ey[1]-ey[0]])
+                    Lxy = ecrd[1, :] - ecrd[0, :]
+                    L = np.sqrt(Lxy @ Lxy)
+                    cosa, cosb = Lxy / L
+                else:
+                    pass
+
+                s_all, xl, nep = section_force_distribution_2d(ecrd, pl, nep, eload_data)
 
                 if sf_type == 'N' or sf_type == 'axial':
                     ss = s_all[:, 0]
                 elif sf_type == 'V' or sf_type == 'shear' or sf_type == 'T':
                     ss = s_all[:, 1]
                 elif sf_type == 'M' or sf_type == 'moment':
                     ss = s_all[:, 2]
 
 
-            # minVal = min(minVal, np.min(ss))
-            # maxVal = max(maxVal, np.max(ss))
-            minVal, minVal_ind = np.amin(ss), np.argmin(ss)
-            maxVal, maxVal_ind = np.amax(ss), np.argmax(ss)
+            if len(ss) == 2:  # for truss with zero shear force and moment
+                pass
+
+            else:
+                # minVal = min(minVal, np.min(ss))
+                # maxVal = max(maxVal, np.max(ss))
+                minVal, minVal_ind = np.amin(ss), np.argmin(ss)
+                maxVal, maxVal_ind = np.amax(ss), np.argmax(ss)
 
-            s = ss * sfac
+                s = ss * sfac
 
-            s_0 = np.zeros((nep, 2))
-            s_0[0, :] = [ex[0], ey[0]]
+                s_0 = np.zeros((nep, 2))
+                s_0[0, :] = [ecrd[0, 0], ecrd[0, 1]]
 
-            s_0[1:, 0] = s_0[0, 0] + xl[1:] * cosa
-            s_0[1:, 1] = s_0[0, 1] + xl[1:] * cosb
+                s_0[1:, 0] = s_0[0, 0] + xl[1:] * cosa
+                s_0[1:, 1] = s_0[0, 1] + xl[1:] * cosb
 
-            s_p = np.copy(s_0)
+                s_p = np.copy(s_0)
 
-            # positive M are opposite to N and V
-            if sf_type == 'M' or sf_type == 'moment':
-                s *= -1.
+                # positive M are opposite to N and V
+                if sf_type == 'M' or sf_type == 'moment':
+                    s *= -1.
 
-            s_p[:, 0] -= s * cosb
-            s_p[:, 1] += s * cosa
+                s_p[:, 0] -= s * cosb
+                s_p[:, 1] += s * cosa
 
-            ax.axis('equal')
+                ax.axis('equal')
 
-            # section force curve
-            ax.plot(s_p[:, 0], s_p[:, 1], **fmt_secforce1)
+                # section force curve
+                ax.plot(s_p[:, 0], s_p[:, 1], **fmt_secforce1)
+                fmt_secforce1 = fmt_secforce1_orig
 
-            # reference perpendicular lines
-            if ref_vert_lines:
-                for i in np.arange(nep):
-                    ax.plot([s_0[i, 0], s_p[i, 0]], [s_0[i, 1], s_p[i, 1]],
+                # reference perpendicular lines
+                if ref_vert_lines:
+                    for i in np.arange(nep):
+                        ax.plot([s_0[i, 0], s_p[i, 0]], [s_0[i, 1], s_p[i, 1]],
+                                **fmt_secforce2)
+                else:
+                    ax.plot([s_0[0, 0], s_p[0, 0]], [s_0[0, 1], s_p[0, 1]],
+                            **fmt_secforce2)
+                    ax.plot([s_0[-1, 0], s_p[-1, 0]], [s_0[-1, 1], s_p[-1, 1]],
                             **fmt_secforce2)
-            else:
-                ax.plot([s_0[0, 0], s_p[0, 0]], [s_0[0, 1], s_p[0, 1]],
-                        **fmt_secforce2)
-                ax.plot([s_0[-1, 0], s_p[-1, 0]], [s_0[-1, 1], s_p[-1, 1]],
-                        **fmt_secforce2)
 
-            if ele_class_tag == EleClassTag.truss:
+            if ele_class_tag in [EleClassTag.truss, EleClassTag.trussSection]:
                 ha = 'center'
-                ax.text(s_p[int(nep / 2), 0], s_p[int(nep / 2), 1],
-                        f'{abs(axial_force):.1f}', va=va, ha=ha, color=fmt_color)
+                va = 'bottom'
+                if sf_type == 'N' or sf_type == 'axial':
+                    ax.text(s_p[int(nep / 2), 0], s_p[int(nep / 2), 1],
+                            f'{abs(axial_force):.1f}', va=va, ha=ha, color=fmt_color)
+                # else:
+                #     ax.text(s_p[int(nep / 2), 0], s_p[int(nep / 2), 1],
+                #             '0.0', va=va, ha=ha)
+
             else:
                 if end_max_values:
                     ha = 'left'
                     va = 'bottom'
                     ax.text(s_p[0, 0], s_p[0, 1],
                             f'{ss[0]:.5g}', va=va, ha=ha)
                     ax.text(s_p[-1, 0], s_p[-1, 1],
@@ -520,30 +581,27 @@
 
 
 def section_force_diagram_3d(sf_type, sfac=1., nep=17,
                              fmt_secforce1=fmt_secforce1,
                              fmt_secforce2=fmt_secforce2,
                              ref_vert_lines=True,
                              end_max_values=True,
-                             dir_plt=0, ax=False):
+                             dir_plt=0, node_supports=True, ax=False,
+                             alt_model_plot=1):
     """Display section forces diagram of a 3d beam column model.
 
     This function plots section forces diagrams for 3d beam column elements
     with or without element loads. For now only '-beamUniform' constant
     transverse or axial element loads are supported.
 
     Args:
         sf_type (str): type of section force: 'N' - normal force,
             'Vy' or 'Vz' - shear force, 'My' or 'Mz' - bending moments,
             'T' - torsional moment.
 
-        Ew (dict): Ew Python dictionary contains information on non-zero
-            element loads, therfore each item of the Python dictionary
-            is in the form: 'ele_tag: ['-beamUniform', Wy, Wz, Wx]'.
-
         sfac (float): scale factor by wich the values of section forces are
             multiplied.
 
         nep (int): number of evaluation points including both end nodes
             (default: 17)
 
         fmt_secforce1 (dict): line format dictionary for section force distribution
@@ -555,158 +613,243 @@
             extreme (max, min) value between the ends.
 
         dir_plt {0, 1, 2}: direction in which to plot the load effects:
             0 (default) - as defined in the code for each load effect type
             1 - in the y-axis (default for N, Vy, T, Mz)
             2 - in the z-axis (default for Vz, My)
 
+        ax: Optional axis to plot to.
+
+        alt_model_plot (int): 1 - for using the plot_model command,  2 - for using
+            simplified model plotting. Other integer - for no model plotting.
+            In this case the model can be plotted outside this command
+            using the axes (ax) object. Default is 1.
+
+    Returns:
+        minVal (float): the minimum overall value of the section force.
+
+        maxVal (float): the maximum overall value of the section force.
+
+        ax: the axes object.
+
     Usage:
         See example: demo_cantilever_3el_3d.py
 
     Todo:
 
     Add support for other element loads available in OpenSees: partial
     (trapezoidal) uniform element load, and 'beamPoint' element load.
     """
 
-    maxVal, minVal = -np.inf, np.inf
-    ele_tags = ops.getEleTags()
+    # If supplied axis can be plotted to
+    if hasattr(ax, "name") and (ax.name == "3d"):
+        pass
+    else:
+        azim, elev = az_el
+        fig_wi, fig_he = fig_wi_he
+        fleft, fbottom, fright, ftop = fig_lbrt
 
-    azim, elev = az_el
-    fig_wi, fig_he = fig_wi_he
-    fleft, fbottom, fright, ftop = fig_lbrt
+        fig = plt.figure(figsize=(fig_wi / 2.54, fig_he / 2.54))
+        fig.subplots_adjust(left=0.08, bottom=0.08, right=0.985, top=0.94)
 
-    fig = plt.figure(figsize=(fig_wi/2.54, fig_he/2.54))
-    fig.subplots_adjust(left=.08, bottom=.08, right=.985, top=.94)
+        ax = fig.add_subplot(111, projection=Axes3D.name)
 
-    ax = fig.add_subplot(111, projection=Axes3D.name)
-    # ax.axis('equal')
+        ax.view_init(azim=azim, elev=elev)
 
     ax.set_xlabel('X')
     ax.set_ylabel('Y')
     ax.set_zlabel('Z')
 
     ax.view_init(azim=azim, elev=elev)
 
-    ax = model.plot_model(node_labels=0, element_labels=0,
-                          fmt_model=fmt_model_secforce,
-                          node_supports=False, ax=ax)
+    if alt_model_plot == 1:
+        ax = model.plot_model(node_labels=0, element_labels=0,
+                              fmt_model=fmt_model_secforce,
+                              node_supports=False,
+                              fmt_model_truss=fmt_model_secforce,
+                              truss_node_offset=0, ax=ax)
+    else:
+        pass
+
+    fmt_secforce1_orig = fmt_secforce1
+    maxVal, minVal = -np.inf, np.inf
+    ele_tags = ops.getEleTags()
 
     Ew = model.get_Ew_data_from_ops_domain_3d()
 
     for i, ele_tag in enumerate(ele_tags):
 
-        # by default no element load
-        eload_data = [['-beamUniform', 0., 0., 0.]]
-        if ele_tag in Ew:
-            eload_data = Ew[ele_tag]
-
-        nd1, nd2 = ops.eleNodes(ele_tag)
-
-        # element x, y coordinates
-        ex = np.array([ops.nodeCoord(nd1)[0],
-                       ops.nodeCoord(nd2)[0]])
-        ey = np.array([ops.nodeCoord(nd1)[1],
-                       ops.nodeCoord(nd2)[1]])
-        ez = np.array([ops.nodeCoord(nd1)[2],
-                       ops.nodeCoord(nd2)[2]])
-
-        # eo = Eo[i, :]
-        xloc = ops.eleResponse(ele_tag, 'xlocal')
-        yloc = ops.eleResponse(ele_tag, 'ylocal')
-        zloc = ops.eleResponse(ele_tag, 'zlocal')
-        g = np.vstack((xloc, yloc, zloc))
-
-        G, _ = model.rot_transf_3d(ex, ey, ez, g)
-
-        g = G[:3, :3]
-
-        pl = ops.eleResponse(ele_tag, 'localForces')
-
-        s_all, xl, nep = section_force_distribution_3d(ex, ey, ez, pl, nep,
-                                                       eload_data)
-
-        # 1:'y' 2:'z'
-        if sf_type == 'N':
-            ss = s_all[:, 0]
-            dir_plt_tmp = 1
-        elif sf_type == 'Vy':
-            ss = s_all[:, 1]
-            dir_plt_tmp = 1
-        elif sf_type == 'Vz':
-            ss = s_all[:, 2]
-            dir_plt_tmp = 2
-        elif sf_type == 'T':
-            ss = s_all[:, 3]
-            dir_plt_tmp = 1
-        elif sf_type == 'My':
-            ss = s_all[:, 4]
-            dir_plt_tmp = 2
-        elif sf_type == 'Mz':
-            ss = s_all[:, 5]
-            dir_plt_tmp = 1
-
-        if dir_plt == 0:
-            dir_plt = dir_plt_tmp
-
-        # minVal = min(minVal, np.min(ss))
-        # maxVal = max(maxVal, np.max(ss))
-        minVal, minVal_ind = np.amin(ss), np.argmin(ss)
-        maxVal, maxVal_ind = np.amax(ss), np.argmax(ss)
-
-        s = ss * sfac
-
-        # FIXME - can be simplified
-        s_0 = np.zeros((nep, 3))
-        s_0[0, :] = [ex[0], ey[0], ez[0]]
-
-        s_0[1:, 0] = s_0[0, 0] + xl[1:] * g[0, 0]
-        s_0[1:, 1] = s_0[0, 1] + xl[1:] * g[0, 1]
-        s_0[1:, 2] = s_0[0, 2] + xl[1:] * g[0, 2]
-
-        s_p = np.copy(s_0)
-
-        # positive M are opposite to N and V
-        # if sf_type == 'Mz' or sf_type == 'My':
-        if sf_type == 'Mz':
-            s *= -1.
-
-        s_p[:, 0] += s * g[dir_plt, 0]
-        s_p[:, 1] += s * g[dir_plt, 1]
-        s_p[:, 2] += s * g[dir_plt, 2]
-
-        # plt.axis('equal')
-
-        # section force curve
-        ax.plot(s_p[:, 0], s_p[:, 1], s_p[:, 2], **fmt_secforce1)
-
-        # reference perpendicular lines
-        if ref_vert_lines:
-            for i in np.arange(nep):
-                ax.plot([s_0[i, 0], s_p[i, 0]],
-                        [s_0[i, 1], s_p[i, 1]],
-                        [s_0[i, 2], s_p[i, 2]], **fmt_secforce2)
-        else:
-            ax.plot([s_0[0, 0], s_p[0, 0]],
-                    [s_0[0, 1], s_p[0, 1]],
-                    [s_0[0, 2], s_p[0, 2]], **fmt_secforce2)
-            ax.plot([s_0[-1, 0], s_p[-1, 0]],
-                    [s_0[-1, 1], s_p[-1, 1]],
-                    [s_0[-1, 2], s_p[-1, 2]], **fmt_secforce2)
-
-        if end_max_values:
-            ha = 'left'
-            va = 'bottom'
-            ax.text(s_p[0, 0], s_p[0, 1], s_p[0, 2],
-                    f'{ss[0]:.5g}', va=va, ha=ha)
-            ax.text(s_p[-1, 0], s_p[-1, 1], s_p[-1, 2],
-                    f'{ss[-1]:.5g}', va=va, ha=ha)
-
-            if minVal_ind != 0 or minVal_ind != nep - 1:
-                ax.text(s_p[minVal_ind, 0], s_p[minVal_ind, 1], s_p[minVal_ind, 2],
-                        f'{ss[minVal_ind]:.5g}', va=va, ha=ha)
-
-            if maxVal_ind != 0 or maxVal_ind != nep - 1:
-                ax.text(s_p[maxVal_ind, 0], s_p[maxVal_ind, 1], s_p[maxVal_ind, 2],
-                        f'{ss[maxVal_ind]:.5g}', va=va, ha=ha)
+        ele_class_tag = ops.getEleClassTags(ele_tag)[0]
+
+        if (ele_class_tag == EleClassTag.ElasticBeam3d
+            or ele_class_tag == EleClassTag.ForceBeamColumn3d
+            or ele_class_tag == EleClassTag.DispBeamColumn3d
+            or ele_class_tag in [EleClassTag.truss, EleClassTag.trussSection]
+            or ele_class_tag == EleClassTag.TimoshenkoBeamColumn3d
+            or ele_class_tag == EleClassTag.ElasticTimoshenkoBeam3d):
+
+            ele_node_tags = ops.eleNodes(ele_tag)
+            ecrd = np.zeros((2, 3))
+            for i, ele_node_tag in enumerate(ele_node_tags):
+                ecrd[i, :] = ops.nodeCoord(ele_node_tag)
+
+            # eo = Eo[i, :]
+            xloc = ops.eleResponse(ele_tag, 'xlocal')
+            yloc = ops.eleResponse(ele_tag, 'ylocal')
+            zloc = ops.eleResponse(ele_tag, 'zlocal')
+            g = np.vstack((xloc, yloc, zloc))
+
+            # rigid offsets for 3d
+            ele_offsets = np.array(ops.eleResponse(ele_tag, 'offsets'))
+            nz_offsets = np.nonzero(ele_offsets)[0]  # tuple of arrays
+            if np.any(nz_offsets):
+                # modify ecrd_eles
+                # ex += ele_offsets[[0, 3]]
+                # ey += ele_offsets[[1, 4]]
+                ecrd[:, 0] += ele_offsets[[0, 3]]
+                ecrd[:, 1] += ele_offsets[[1, 4]]
+                ecrd[:, 2] += ele_offsets[[2, 5]]
+                # modify the following due to rigid offsets
+            else:
+                pass
+
+            G, _ = model.rot_transf_3d(ecrd, g)
+
+            g = G[:3, :3]
+
+            if ele_class_tag in [EleClassTag.truss, EleClassTag.trussSection]:
+                if sf_type == 'N' or sf_type == 'axial':
+                    axial_force = ops.eleResponse(ele_tag, 'axialForce')[0]
+                    ss = -axial_force * np.ones(nep)
+                    xl = np.linspace(0., L, nep)
+
+                    if axial_force > 0:
+                        va = 'top'
+                        fmt_color = 'b'
+                        fmt_secforce1 = fmt_secforce_tension
+                    else:
+                        va = 'bottom'
+                        fmt_color = 'r'
+                        fmt_secforce1 = fmt_secforce_compression
+
+                else:  # for sf_type = 'V' or 'M'
+                    xl = np.linspace(0., L, 2)
+                    ss = np.zeros(2)
+
+            else:
+                # by default no element load
+                eload_data = [['-beamUniform', 0., 0., 0.]]
+                if ele_tag in Ew:
+                    eload_data = Ew[ele_tag]
+
+                pl = ops.eleResponse(ele_tag, 'localForces')
+
+                s_all, xl, nep = section_force_distribution_3d(ecrd, pl, nep,
+                                                               eload_data)
+
+                # 1:'y' 2:'z'
+                if sf_type == 'N':
+                    ss = s_all[:, 0]
+                    dir_plt_tmp = 1
+                elif sf_type == 'Vy':
+                    ss = s_all[:, 1]
+                    dir_plt_tmp = 1
+                elif sf_type == 'Vz':
+                    ss = s_all[:, 2]
+                    dir_plt_tmp = 2
+                elif sf_type == 'T':
+                    ss = s_all[:, 3]
+                    dir_plt_tmp = 1
+                elif sf_type == 'My':
+                    ss = s_all[:, 4]
+                    dir_plt_tmp = 2
+                elif sf_type == 'Mz':
+                    ss = s_all[:, 5]
+                    dir_plt_tmp = 1
+
+                if dir_plt == 0:
+                    dir_plt = dir_plt_tmp
+
+
+            if len(ss) == 2:  # for truss with zero shear force and moment
+                pass
+
+            else:
+                # minVal = min(minVal, np.min(ss))
+                # maxVal = max(maxVal, np.max(ss))
+                minVal, minVal_ind = np.amin(ss), np.argmin(ss)
+                maxVal, maxVal_ind = np.amax(ss), np.argmax(ss)
+
+                s = ss * sfac
+
+                # FIXME - can be simplified
+                s_0 = np.zeros((nep, 3))
+                s_0[0, :] = [ecrd[0, 0], ecrd[0, 1], ecrd[0, 2]]
+
+                s_0[1:, 0] = s_0[0, 0] + xl[1:] * g[0, 0]
+                s_0[1:, 1] = s_0[0, 1] + xl[1:] * g[0, 1]
+                s_0[1:, 2] = s_0[0, 2] + xl[1:] * g[0, 2]
+
+                s_p = np.copy(s_0)
+
+                # positive M are opposite to N and V
+                # if sf_type == 'Mz' or sf_type == 'My':
+                if sf_type == 'Mz':
+                    s *= -1.
+
+                s_p[:, 0] += s * g[dir_plt, 0]
+                s_p[:, 1] += s * g[dir_plt, 1]
+                s_p[:, 2] += s * g[dir_plt, 2]
+
+                # plt.axis('equal')
+
+                # section force curve
+                ax.plot(s_p[:, 0], s_p[:, 1], s_p[:, 2], **fmt_secforce1)
+                fmt_secforce1 = fmt_secforce1_orig
+
+                # reference perpendicular lines
+                if ref_vert_lines:
+                    for i in np.arange(nep):
+                        ax.plot([s_0[i, 0], s_p[i, 0]],
+                                [s_0[i, 1], s_p[i, 1]],
+                                [s_0[i, 2], s_p[i, 2]], **fmt_secforce2)
+                else:
+                    ax.plot([s_0[0, 0], s_p[0, 0]],
+                            [s_0[0, 1], s_p[0, 1]],
+                            [s_0[0, 2], s_p[0, 2]], **fmt_secforce2)
+                    ax.plot([s_0[-1, 0], s_p[-1, 0]],
+                            [s_0[-1, 1], s_p[-1, 1]],
+                            [s_0[-1, 2], s_p[-1, 2]], **fmt_secforce2)
+
+            # dodane FIXME
+            if ele_class_tag in [EleClassTag.truss, EleClassTag.trussSection]:
+                ha = 'center'
+                va = 'bottom'
+                if sf_type == 'N' or sf_type == 'axial':
+                    ax.text(s_p[int(nep / 2), 0], s_p[int(nep / 2), 1], s_p[int(nep / 2), 2],
+                            f'{abs(axial_force):.1f}', va=va, ha=ha, color=fmt_color)
+                # else:
+                #     ax.text(s_p[int(nep / 2), 0], s_p[int(nep / 2), 1],
+                #             '0.0', va=va, ha=ha)
+
+            else:
+                if end_max_values:
+                    ha = 'left'
+                    va = 'bottom'
+                    ax.text(s_p[0, 0], s_p[0, 1], s_p[0, 2],
+                            f'{ss[0]:.5g}', va=va, ha=ha)
+                    ax.text(s_p[-1, 0], s_p[-1, 1], s_p[-1, 2],
+                            f'{ss[-1]:.5g}', va=va, ha=ha)
+
+                    if minVal_ind != 0 or minVal_ind != nep - 1:
+                        ax.text(s_p[minVal_ind, 0], s_p[minVal_ind, 1], s_p[minVal_ind, 2],
+                                f'{ss[minVal_ind]:.5g}', va=va, ha=ha)
+
+                    if maxVal_ind != 0 or maxVal_ind != nep - 1:
+                        ax.text(s_p[maxVal_ind, 0], s_p[maxVal_ind, 1], s_p[maxVal_ind, 2],
+                                f'{ss[maxVal_ind]:.5g}', va=va, ha=ha)
+
+    if node_supports:
+        node_tags = ops.getNodeTags()
+        ax = model._plot_supports(node_tags, ax)
 
     return minVal, maxVal, ax
```

### Comparing `opsvis-1.0.9/opsvis/settings.py` & `opsvis-1.1.1/opsvis/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 # check documentation on matplotlib's plot
 
 # element end nodes
 fmt_nodes = {'color': 'red', 'linestyle': 'None', 'linewidth': 1.2, 'marker': 's', 'markersize': 6}
 
 # initial model
 fmt_model = {'color': 'blue', 'linestyle': 'solid', 'linewidth': 1.2, 'marker': '.', 'markersize': 6}
+fmt_model_truss = {'color': 'green', 'linestyle': 'solid', 'linewidth': 1.2, 'marker': 'o', 'markersize': 6, 'markerfacecolor': 'white'}
 fmt_model_nodes_only = {'color': 'blue', 'linestyle': 'solid', 'linewidth': 1.2, 'marker': '.', 'markersize': 6}
 fmt_model_loads = {'color': 'black', 'linestyle': 'solid', 'linewidth': 1.2, 'marker': '', 'markersize': 1}
+fmt_model_rigid_offset = {'color': 'black', 'linestyle': 'solid', 'linewidth': 3.2, 'marker': '.', 'markersize': 1}
 
 fmt_model_joint2d = {'color': 'black', 'linestyle': 'solid', 'linewidth': 1.2, 'marker': '', 'markersize': 1}
 fmt_model_secforce = {'color': 'black', 'linestyle': 'solid', 'linewidth': 1.2, 'marker': '', 'markersize': 1}
 
 # deformed model
 fmt_defo = {'color': 'blue', 'linestyle': 'solid', 'linewidth': 1.2, 'marker': '', 'markersize': 1}
 fmt_defo_faces = {'linewidths': 1, 'edgecolors': 'k', 'alpha': 0.5}
+fmt_defo_zeroLenght = {'color': 'blue', 'linestyle': 'dashed', 'linewidth': 1.2, 'marker': '*', 'markersize': 6, 'markerfacecolor': 'white'}
 
 # undeformed model
 fmt_undefo = {'color': 'green', 'linestyle': (0, (1, 5)), 'linewidth': 1.2, 'marker': '', 'markersize': 1}
 fmt_undefo_faces = {'linewidths': 1, 'linestyles': 'dotted', 'edgecolors': 'g', 'facecolors': 'w', 'alpha': 0.5}
 
 # section forces
 fmt_secforce1 = {'color': 'blue', 'linestyle': 'solid', 'linewidth': 2.0, 'marker': '',
@@ -29,14 +32,16 @@
 fmt_secforce2 = {'color': 'blue', 'linestyle': 'solid', 'linewidth': 1.0, 'marker': '',
                  'markersize': 1, 'solid_capstyle': 'round', 'solid_joinstyle': 'round',
                  'dash_capstyle': 'butt', 'dash_joinstyle': 'round'}
 
 fmt_secforce_tension = {'color': 'blue', 'linestyle': 'solid', 'linewidth': 2.0, 'marker': '', 'markersize': 1}
 fmt_secforce_compression = {'color': 'red', 'linestyle': 'solid', 'linewidth': 2.0, 'marker': '', 'markersize': 1}
 
+fmt_gauss_points = {'color': 'firebrick', 'linestyle': 'None', 'linewidth': 2.0, 'marker': 'X', 'markersize': 5}
+
 # figure left right bottom top offsets
 fig_lbrt = (.04, .04, .96, .96)
 fig_lbrt_model = (.08, .08, .985, .94)
 fig_lbrt_secforces = (.04, .08, .985, .92)
 fig_lbrt_defo = (.08, .08, .985, .92)
 fig_lbrt_mode = (.08, .08, .985, .92)
 
@@ -50,36 +55,39 @@
 class EleClassTag:
     """ELE_TAG constants defined in SRC/classTags.h"""
     truss = 12
     trussSection = 13
     CorotTruss = 14
     ZeroLength = 19
     ZeroLengthSection = 20
+    CoupledZeroLength = 26
     ElasticBeam2d = 3
     ElasticBeam3d = 5
     DispBeamColumn2d = 62
     DispBeamColumn3d = 64
     ForceBeamColumn2d = 73
     ForceBeamColumn3d = 74
     TimoshenkoBeamColumn2d = 63
+    TimoshenkoBeamColumn3d = 631
     ElasticTimoshenkoBeam2d = 145
     ElasticTimoshenkoBeam3d = 146
     tri3n = 33
     tri6n = 209
     quad4n = 31
     quad4n3d = 32
     quad9n = 207
     quad8n = 208
     SSPquad = 119
     EnhancedQuad = 59
     brick20n = 49
     brick8n = 56
     SSPbrick = 121
     FourNodeTetrahedron = 179
-    TenNodeTetrahedron = 1790
+    TenNodeTetrahedron = 256
+    TenNodeTetrahedronSK = 1790
     ASDShellQ4 = 203
     ASDShellT3 = 204
     ShellMITC4 = 53
     ShellMITC9 = 54
     Joint2D = 82
     Joint3D = 83
     MVLEM = 162
```

### Comparing `opsvis-1.0.9/opsvis/stress.py` & `opsvis-1.1.1/opsvis/stress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import openseespy.opensees as ops
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.tri as tri
 
-from settings import *
+from .settings import *
 
 
 def stress_2d_ele_tags_only(ele_tags):
 
     Stress2dEleClasstags = set([EleClassTag.tri3n,
                                 EleClassTag.tri6n,
                                 EleClassTag.quad4n,
@@ -748,14 +748,16 @@
         ele_node_tags = ops.eleNodes(ele_tag)
 
         for j, ele_node_tag in enumerate(ele_node_tags):
             eles_conn[i, j] = node_tags.index(ele_node_tag)
 
     if (ele_classtag == EleClassTag.tri3n):
         tris_conn = eles_conn
+        nds_crd_all = nds_crd
+        nds_val_all = nds_val
 
     elif (ele_classtag == EleClassTag.quad4n):
         tris_conn, nds_c_crd, nds_c_val = \
             quads_to_4tris(eles_conn, nds_crd, nds_val)
 
         nds_crd_all = np.vstack((nds_crd, nds_c_crd))
         nds_val_all = np.hstack((nds_val, nds_c_val))
```

### Comparing `opsvis-1.0.9/opsvis.egg-info/PKG-INFO` & `opsvis-1.1.1/opsvis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: opsvis
-Version: 1.0.9
+Version: 1.1.1
 Summary: OpenSeesPy (OpenSees) Python postprocessing and visualization module
 Home-page: https://github.com/sewkokot/opsvis
 Author: Seweryn Kokot
 Author-email: sewkokot@gmail.com
 Project-URL: Bug Tracker, https://github.com/sewkokot/opsvis/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # opsvis
```

### Comparing `opsvis-1.0.9/setup.cfg` & `opsvis-1.1.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = opsvis
-version = 1.0.9
+version = 1.1.1
 author = Seweryn Kokot
 author_email = sewkokot@gmail.com
 description = OpenSeesPy (OpenSees) Python postprocessing and visualization module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sewkokot/opsvis
 project_urls = 
 	Bug Tracker = https://github.com/sewkokot/opsvis/issues
 classifiers = 
 	Programming Language :: Python :: 3
-	License :: OSI Approved :: MIT License
+	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 install_requires = 
 	openseespy
 python_requires = >=3.6
```

