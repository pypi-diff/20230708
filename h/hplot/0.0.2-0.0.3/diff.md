# Comparing `tmp/hplot-0.0.2-py3-none-any.whl.zip` & `tmp/hplot-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 12657 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      109 b- defN 23-Jul-05 07:25 hplot/__init__.py
--rw-rw-rw-  2.0 fat      553 b- defN 23-Jul-05 07:13 hplot/config.py
--rw-rw-rw-  2.0 fat     5756 b- defN 23-Jul-05 12:28 hplot/plot_box.py
--rw-rw-rw-  2.0 fat     6746 b- defN 23-Jul-05 07:28 hplot/plot_plt.py
--rw-rw-rw-  2.0 fat     8848 b- defN 23-Jul-05 07:28 hplot/plot_sns.py
--rw-rw-rw-  2.0 fat      384 b- defN 23-Jul-04 06:51 hplot/prepare_data.py
--rw-rw-rw-  2.0 fat      353 b- defN 23-Jul-04 06:51 hplot/utils.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-05 12:35 hplot-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      518 b- defN 23-Jul-05 12:35 hplot-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-05 12:35 hplot-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-05 12:35 hplot-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      888 b- defN 23-Jul-05 12:35 hplot-0.0.2.dist-info/RECORD
-12 files, 35811 bytes uncompressed, 11189 bytes compressed:  68.8%
+Zip file size: 11810 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      111 b- defN 23-Jul-08 14:02 hplot/__init__.py
+-rw-rw-rw-  2.0 fat      551 b- defN 23-Jul-08 14:02 hplot/config.py
+-rw-rw-rw-  2.0 fat     5277 b- defN 23-Jul-08 14:34 hplot/plot_box.py
+-rw-rw-rw-  2.0 fat     6367 b- defN 23-Jul-08 14:33 hplot/plot_plt.py
+-rw-rw-rw-  2.0 fat     7789 b- defN 23-Jul-08 14:34 hplot/plot_sns.py
+-rw-rw-rw-  2.0 fat      353 b- defN 23-Jul-08 14:02 hplot/utils.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-08 14:42 hplot-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      555 b- defN 23-Jul-08 14:42 hplot-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-08 14:42 hplot-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-08 14:42 hplot-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      811 b- defN 23-Jul-08 14:42 hplot-0.0.3.dist-info/RECORD
+11 files, 33470 bytes uncompressed, 10460 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -9,29 +9,26 @@
 
 Filename: hplot/plot_plt.py
 Comment: 
 
 Filename: hplot/plot_sns.py
 Comment: 
 
-Filename: hplot/prepare_data.py
-Comment: 
-
 Filename: hplot/utils.py
 Comment: 
 
-Filename: hplot-0.0.2.dist-info/LICENSE
+Filename: hplot-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: hplot-0.0.2.dist-info/METADATA
+Filename: hplot-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: hplot-0.0.2.dist-info/WHEEL
+Filename: hplot-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: hplot-0.0.2.dist-info/top_level.txt
+Filename: hplot-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: hplot-0.0.2.dist-info/RECORD
+Filename: hplot-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hplot/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
 from hplot.plot_plt import plot_plt
 from hplot.plot_sns import plot_sns
-from hplot.plot_box import plot_box
+from hplot.plot_box import plot_box
```

## hplot/config.py

```diff
@@ -1,8 +1,7 @@
-
 class AttrDict(dict):
     """
     A extended dict of which the keys can be used as attribution
     """
 
     __setattr__ = dict.__setitem__
     __getattr__ = dict.__getitem__
```

## hplot/plot_box.py

```diff
@@ -1,41 +1,42 @@
-import matplotlib.pyplot as plt
-import matplotlib.colors as mcolors
+import os
 from itertools import cycle
-from matplotlib import rcParams
 
-from hplot.utils import cm2inch
-from hplot.config import default_cfg
-import numpy as np
-import seaborn as sns
+import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
+import seaborn as sns
+from matplotlib import rcParams
+
+from hplot.config import default_cfg
+from hplot.utils import cm2inch
 
 
 class PloterBox:
     def __init__(
-            self,
-            data,
-            fname=None,
-            *,
-            width=0.5,
-            linewidth=1.0,
-            xlabel=None,
-            ylabel=None,
-            display=True,
-            fig_size=None,
-            usetex=False,
-            dpi=None,
-            pad=None,
-            theme=None,
-            tick_size=None,
-            tick_label_font=None,
-            legend_font_dict=None,
-            label_font_dict=None,
-            ) -> None:
+        self,
+        data,
+        fname=None,
+        *,
+        width=0.5,
+        linewidth=1.0,
+        xlabel=None,
+        ylabel=None,
+        display=True,
+        fig_size=None,
+        usetex=False,
+        dpi=None,
+        pad=None,
+        theme=None,
+        tick_size=None,
+        tick_label_font=None,
+        legend_font_dict=None,
+        label_font_dict=None,
+    ) -> None:
         self.data = data
         self.fname = fname
         self.width = width
         self.linewidth = linewidth
         self.xlabel = xlabel
         self.ylabel = ylabel
         self.display = display
@@ -44,18 +45,20 @@
         self.pad = pad
         self.theme = theme
         self.usetex = usetex
         self.tick_size = tick_size
         self.tick_label_font = tick_label_font
         self.legend_font_dict = legend_font_dict
         self.label_font_dict = label_font_dict
-
+        plt.cla()
+        plt.clf()
+        plt.close()
         self.ax = None
         self.fig = None
-        self.__preprocess() 
+        self.__preprocess()
 
     def __preprocess(self):
         rcParams.update({"mathtext.fontset": "stix"})
         assert isinstance(self.data, (dict, list, tuple))
 
         if isinstance(self.data, dict):
             self.data = [self.data]
@@ -78,20 +81,19 @@
 
         # use tex to render fonts, tex install required
         if self.usetex:
             from matplotlib import rc
 
             rc("font", **{"family": "serif", "serif": ["Times New Roman"]})
             rc("text", usetex=True)
-        
+
     def plot(self):
         if self.theme is not None:
             sns.set_theme(style=self.theme)
         self.fig, self.ax = plt.subplots(figsize=cm2inch(*self.fig_size), dpi=self.dpi)
-        
 
         data_dict = dict()
 
         for subdata in self.data:
             data_dict[subdata["label"]] = subdata["y"]
 
         df = pd.DataFrame(data_dict)
@@ -103,23 +105,26 @@
         [label.set_fontname(self.tick_label_font) for label in labels]
 
         # label
         if self.xlabel is not None:
             plt.xlabel(self.xlabel, fontdict=self.label_font_dict)
         if self.ylabel is not None:
             plt.ylabel(self.ylabel, fontdict=self.label_font_dict)
-        
+
     def save(self):
         plt.tight_layout(pad=self.pad)
         if self.fname is None:
             pass
         else:
+            dir_path = os.path.dirname(self.fname)
+            os.makedirs(dir_path, exist_ok=True)
             plt.savefig(self.fname)
 
     def show(self):
+        self.fig.set_tight_layout(True)
         plt.tight_layout(pad=self.pad)
         plt.show()
 
     def close(self):
         sns.set_theme(style="white")
         plt.close()
 
@@ -176,28 +181,7 @@
     ploter.plot()
 
     if fname is not None:
         ploter.save()
     if display:
         ploter.show()
     ploter.close()
-
-
-
-def test():
-    d1 = np.random.randn(100)
-    d2 = d1 * 0.8 + 0.5
-    sns.set_theme(style="darkgrid")
-    # plt.boxplot([d, d * 0.8 + 0.5], labels=["a", "b"])
-    # sns.boxplot(data=[d, d * 0.8 + 0.5], palette="Set3")
-    df = pd.DataFrame({"a": d1, "b": d2})
-    sns.boxplot(data=df)
-
-    plt.show()
-
-
-if __name__ == "__main__":
-    d1 = np.random.randn(100)
-    d2 = d1 * 0.8 + 0.5
-    data = [{"label": "a", "y": d1}, {"label": "b", "y": d2}]
-    
-    plot_box(data, fname="test.png", display=True, width=0.2, linewidth=0.1)
```

## hplot/plot_plt.py

```diff
@@ -1,14 +1,16 @@
-import matplotlib.pyplot as plt
-import matplotlib.colors as mcolors
+import os
 from itertools import cycle
+
+import matplotlib.colors as mcolors
+import matplotlib.pyplot as plt
 from matplotlib import rcParams
 
-from hplot.utils import cm2inch
 from hplot.config import default_cfg
+from hplot.utils import cm2inch
 
 
 class PloterPlt:
     def __init__(
         self,
         data,
         fname=None,
@@ -59,15 +61,17 @@
         self.tick_label_font = tick_label_font
         self.legend_font_dict = legend_font_dict
         self.label_font_dict = label_font_dict
 
         self.num_data = None
         self.fig = None
         self.ax = None
-
+        plt.cla()
+        plt.clf()
+        plt.close()
         self.__preprocess()
 
     def __preprocess(self):
         rcParams.update({"mathtext.fontset": "stix"})
         assert isinstance(self.data, (dict, list, tuple))
 
         if isinstance(self.data, dict):
@@ -101,15 +105,15 @@
             tableau_colors = cycle(mcolors.TABLEAU_COLORS)
             self.color_list = [next(tableau_colors) for _ in range(self.num_data)]
 
     def plot(self):
         self.fig, self.ax = plt.subplots(figsize=cm2inch(*self.fig_size), dpi=self.dpi)
 
         # plot figure
-        for (i, d) in enumerate(self.data):
+        for i, d in enumerate(self.data):
             plt.plot(d["x"], d["y"], color=self.color_list[i])
 
         # legend
         plt.tick_params(labelsize=self.tick_size)
         labels = self.ax.get_xticklabels() + self.ax.get_yticklabels()
         [label.set_fontname(self.tick_label_font) for label in labels]
 
@@ -130,17 +134,20 @@
             plt.yticks(self.yticks, self.ytick_labels)
 
     def save(self):
         plt.tight_layout(pad=self.pad)
         if self.fname is None:
             pass
         else:
+            dir_path = os.path.dirname(self.fname)
+            os.makedirs(dir_path, exist_ok=True)
             plt.savefig(self.fname)
 
     def show(self):
+        self.fig.set_tight_layout(True)
         plt.tight_layout(pad=self.pad)
         plt.show()
 
     def close(self):
         plt.close()
 
 
@@ -209,33 +216,7 @@
     ploter.plot()
     if fname is not None:
         ploter.save()
     if display:
         ploter.show()
 
     ploter.close()
-
-
-if __name__ == "__main__":
-    import numpy as np
-
-    x = np.linspace(-2, 2, 200)
-    y1 = np.sin(2 * 3.14 * x)
-    y2 = np.cos(2 * 3.14 * x)
-
-    data = [dict(x=x, y=y1), dict(x=x, y=y2)]
-
-    plot_plt(
-        data,
-        "plot_plt_example.png",
-        xlabel="x",
-        ylabel="y",
-        legend=["sin", "cos"],
-        legend_loc="lower right",
-        xlim=[-3, +3],
-        ylim=[-2, +2],
-        xticks=[-2, +2],
-        xtick_labels=["xstart", "xend"],
-        yticks=[-1, +1],
-        ytick_labels=["ystart", "yend"],
-        display=True,
-    )
```

## hplot/plot_sns.py

```diff
@@ -1,14 +1,16 @@
+import os
+
 import matplotlib.pyplot as plt
-from matplotlib import rcParams
 import numpy as np
-
 import seaborn as sns
-from hplot.utils import cm2inch
+from matplotlib import rcParams
+
 from hplot.config import default_cfg
+from hplot.utils import cm2inch
 
 
 class PloterSns:
     def __init__(
         self,
         data,
         fname,
@@ -54,15 +56,17 @@
         self.fig_size = fig_size
         self.dpi = dpi
         self.pad = pad
         self.tick_size = tick_size
         self.tick_label_font = tick_label_font
         self.legend_font_dict = legend_font_dict
         self.label_font_dict = label_font_dict
-
+        plt.cla()
+        plt.clf()
+        plt.close()
         self.num_data = None
         self.fig = None
         self.ax = None
         self.__preprocess()
 
     def __preprocess(self):
         rcParams.update({"mathtext.fontset": "stix"})
@@ -115,15 +119,15 @@
         x = x.reshape(-1)
         y = y.reshape(-1)
         return x, y, label
 
     def plot(self):
         self.fig, self.ax = plt.subplots(figsize=cm2inch(*self.fig_size), dpi=self.dpi)
         # plot figure
-        for (i, d) in enumerate(self.data):
+        for i, d in enumerate(self.data):
             x, y, label = self._ppc_data(d)
             sns.lineplot(x=x, y=y, label=label)
 
         # tick
         plt.tick_params(labelsize=self.tick_size)
         labels = self.ax.get_xticklabels() + self.ax.get_yticklabels()
         [label.set_fontname(self.tick_label_font) for label in labels]
@@ -156,17 +160,20 @@
             plt.yticks(self.yticks, self.ytick_labels)
 
     def save(self):
         plt.tight_layout(pad=self.pad)
         if self.fname is None:
             pass
         else:
+            dir_path = os.path.dirname(self.fname)
+            os.makedirs(dir_path, exist_ok=True)
             plt.savefig(self.fname)
 
     def show(self):
+        self.fig.set_tight_layout(True)
         plt.tight_layout(pad=self.pad)
         plt.show()
 
     def close(self):
         plt.close()
 
 
@@ -184,15 +191,15 @@
     xticks=None,
     yticks=None,
     xtick_labels=None,
     ytick_labels=None,
     display=True,
     fig_size=None,
     dpi=None,
-    **kwargs
+    **kwargs,
 ):
     """
     plot a curve using seaborn
     :param data: data: list[dict]:
         data used to plot figures,
         example: [dict(x=x1_list, y=y1_list, label=label1), dict(x=x2_list, y=y2_list, label=label2)]
         when there is no repeat experiment data, xi_list=x, shape of x is [d,],
@@ -236,48 +243,16 @@
         xticks=xticks,
         yticks=yticks,
         xtick_labels=xtick_labels,
         ytick_labels=ytick_labels,
         display=display,
         fig_size=fig_size,
         dpi=dpi,
-        **kwargs
+        **kwargs,
     )
     ploter.plot()
     if fname is not None:
         ploter.save()
     if display:
         ploter.show()
 
     ploter.close()
-
-
-if __name__ == "__main__":
-    import numpy as np
-
-    x = np.linspace(-2, 2, 500)
-    y1 = 0.7 * np.sin(2 * 3.14 * x) + 0.3 * np.sin(2 * 3.14 * x) * np.random.randn(*x.shape)
-    y2 = 0.7 * np.sin(2 * 3.14 * x) + 0.3 * np.sin(2 * 3.14 * x) * np.random.randn(*x.shape)
-    y3 = 0.7 * np.sin(2 * 3.14 * x) + 0.3 * np.sin(2 * 3.14 * x) * np.random.randn(*x.shape)
-    data = [dict(x=[x, x, x], y=[y1, y2, y3], label="sin")]
-    x = np.linspace(-2, 2, 500)
-    y1 = 0.7 * np.cos(2 * 3.14 * x) + 0.3 * np.cos(2 * 3.14 * x) * np.random.randn(*x.shape)
-    y2 = 0.7 * np.cos(2 * 3.14 * x) + 0.3 * np.cos(2 * 3.14 * x) * np.random.randn(*x.shape)
-    y3 = 0.7 * np.cos(2 * 3.14 * x) + 0.3 * np.cos(2 * 3.14 * x) * np.random.randn(*x.shape)
-    y = np.stack([y1, y2, y3])
-    data.append(dict(x=[x, x, x], y=[y1, y2, y3], label="cos"))
-    plot_sns(
-        data,
-        "plot_sns_example.png",
-        xlabel="x",
-        ylabel="y",
-        legend=["SIN-FUNC", "COS-FUNC"],
-        legend_loc="lower right",
-        legend_frameon=True,
-        xlim=[-3, +3],
-        ylim=[-2, +2],
-        xticks=[-2, +2],
-        xtick_labels=["xstart", "xend"],
-        yticks=[-1, +1],
-        ytick_labels=["ystart", "yend"],
-        display=True,
-    )
```

## Comparing `hplot-0.0.2.dist-info/LICENSE` & `hplot-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hplot-0.0.2.dist-info/METADATA` & `hplot-0.0.3.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: hplot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Some plot utils for research
 Author: AeroH
 Author-email: zhang.yuh@outlook.com
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: numpy (==1.23.1)
-Requires-Dist: pytest (==7.1.2)
-Requires-Dist: matplotlib (==3.5.1)
-Requires-Dist: pandas (==1.4.2)
-Requires-Dist: scipy (==1.9.0)
-Requires-Dist: seaborn (==0.11.2)
+Requires-Dist: numpy (==1.25.0)
+Requires-Dist: pytest (==7.4.0)
+Requires-Dist: pytest-cov (==4.1.0)
+Requires-Dist: matplotlib (==3.7.2)
+Requires-Dist: pandas (==2.0.3)
+Requires-Dist: scipy (==1.11.1)
+Requires-Dist: seaborn (==0.12.2)
 Requires-Dist: wrapt (==1.14.1)
-Requires-Dist: tabulate (==0.8.10)
+Requires-Dist: tabulate (==0.9.0)
 Requires-Dist: psutil (==5.9.1)
 Requires-Dist: tqdm
```

