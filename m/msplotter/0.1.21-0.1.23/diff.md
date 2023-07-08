# Comparing `tmp/msplotter-0.1.21.tar.gz` & `tmp/msplotter-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msplotter-0.1.21.tar", last modified: Thu Jun  8 15:41:19 2023, max compression
+gzip compressed data, was "msplotter-0.1.23.tar", last modified: Sat Jul  8 02:41:38 2023, max compression
```

## Comparing `msplotter-0.1.21.tar` & `msplotter-0.1.23.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-08 15:41:19.150391 msplotter-0.1.21/
--rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.21/LICENSE
--rw-r--r--   0 msp        (501) staff       (20)     5233 2023-06-08 15:41:19.149861 msplotter-0.1.21/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)     4543 2023-06-08 15:22:57.000000 msplotter-0.1.21/README.md
--rw-r--r--   0 msp        (501) staff       (20)      961 2023-06-07 03:02:16.000000 msplotter-0.1.21/pyproject.toml
--rw-r--r--   0 msp        (501) staff       (20)       38 2023-06-08 15:41:19.150520 msplotter-0.1.21/setup.cfg
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-08 15:41:19.115291 msplotter-0.1.21/src/
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-08 15:41:19.127976 msplotter-0.1.21/src/msp/
--rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.21/src/msp/__init__.py
--rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.21/src/msp/__main__.py
--rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.21/src/msp/arrows.py
--rw-r--r--   0 msp        (501) staff       (20)     5096 2023-06-04 02:40:56.000000 msplotter-0.1.21/src/msp/colormap_picker.py
--rw-r--r--   0 msp        (501) staff       (20)    13276 2023-06-06 20:31:15.000000 msplotter-0.1.21/src/msp/gui.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-08 15:41:19.142853 msplotter-0.1.21/src/msp/images/
--rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.21/src/msp/images/Blues.png
--rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/BuGn.png
--rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/BuPu.png
--rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/GnBu.png
--rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/Greens.png
--rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/Greys.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/OrRd.png
--rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/Oranges.png
--rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/PuBu.png
--rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/PuBuGn.png
--rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/PuRd.png
--rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/Purples.png
--rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/RdPu.png
--rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/Reds.png
--rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/YlGn.png
--rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/YlGnBu.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/YlOrBr.png
--rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/YlOrRd.png
--rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.21/src/msp/images/logo.png
--rw-r--r--   0 msp        (501) staff       (20)    29972 2023-06-05 16:00:41.000000 msplotter-0.1.21/src/msp/msplotter.py
--rw-r--r--   0 msp        (501) staff       (20)     2320 2023-06-04 02:29:30.000000 msplotter-0.1.21/src/msp/plot.py
--rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.21/src/msp/slider_widget.py
--rw-r--r--   0 msp        (501) staff       (20)    13847 2023-06-07 15:34:36.000000 msplotter-0.1.21/src/msp/user_input.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-08 15:41:19.149054 msplotter-0.1.21/src/msplotter.egg-info/
--rw-r--r--   0 msp        (501) staff       (20)     5233 2023-06-08 15:41:19.000000 msplotter-0.1.21/src/msplotter.egg-info/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)      914 2023-06-08 15:41:19.000000 msplotter-0.1.21/src/msplotter.egg-info/SOURCES.txt
--rw-r--r--   0 msp        (501) staff       (20)        1 2023-06-08 15:41:19.000000 msplotter-0.1.21/src/msplotter.egg-info/dependency_links.txt
--rw-r--r--   0 msp        (501) staff       (20)       48 2023-06-08 15:41:19.000000 msplotter-0.1.21/src/msplotter.egg-info/entry_points.txt
--rw-r--r--   0 msp        (501) staff       (20)       55 2023-06-08 15:41:19.000000 msplotter-0.1.21/src/msplotter.egg-info/requires.txt
--rw-r--r--   0 msp        (501) staff       (20)        4 2023-06-08 15:41:19.000000 msplotter-0.1.21/src/msplotter.egg-info/top_level.txt
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-08 02:41:38.431542 msplotter-0.1.23/
+-rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.23/LICENSE
+-rw-r--r--   0 msp        (501) staff       (20)     5234 2023-07-08 02:41:38.430505 msplotter-0.1.23/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)     4544 2023-06-08 15:44:32.000000 msplotter-0.1.23/README.md
+-rw-r--r--   0 msp        (501) staff       (20)      961 2023-07-06 15:23:32.000000 msplotter-0.1.23/pyproject.toml
+-rw-r--r--   0 msp        (501) staff       (20)       38 2023-07-08 02:41:38.431685 msplotter-0.1.23/setup.cfg
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-08 02:41:38.400503 msplotter-0.1.23/src/
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-08 02:41:38.411350 msplotter-0.1.23/src/msp/
+-rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.23/src/msp/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.23/src/msp/__main__.py
+-rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.23/src/msp/arrows.py
+-rw-r--r--   0 msp        (501) staff       (20)     5096 2023-06-04 02:40:56.000000 msplotter-0.1.23/src/msp/colormap_picker.py
+-rw-r--r--   0 msp        (501) staff       (20)    12930 2023-07-08 00:07:06.000000 msplotter-0.1.23/src/msp/gui.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-08 02:41:38.426090 msplotter-0.1.23/src/msp/images/
+-rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.23/src/msp/images/Blues.png
+-rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/BuGn.png
+-rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/BuPu.png
+-rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/GnBu.png
+-rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/Greens.png
+-rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/Greys.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/OrRd.png
+-rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/Oranges.png
+-rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/PuBu.png
+-rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/PuBuGn.png
+-rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/PuRd.png
+-rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/Purples.png
+-rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/RdPu.png
+-rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/Reds.png
+-rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/YlGn.png
+-rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/YlGnBu.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/YlOrBr.png
+-rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/YlOrRd.png
+-rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/logo.png
+-rw-r--r--   0 msp        (501) staff       (20)    30089 2023-07-07 15:34:46.000000 msplotter-0.1.23/src/msp/msplotter.py
+-rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.23/src/msp/plot.py
+-rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.23/src/msp/slider_widget.py
+-rw-r--r--   0 msp        (501) staff       (20)    14412 2023-07-08 00:53:57.000000 msplotter-0.1.23/src/msp/user_input.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-08 02:41:38.429759 msplotter-0.1.23/src/msplotter.egg-info/
+-rw-r--r--   0 msp        (501) staff       (20)     5234 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)      914 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/SOURCES.txt
+-rw-r--r--   0 msp        (501) staff       (20)        1 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/dependency_links.txt
+-rw-r--r--   0 msp        (501) staff       (20)       48 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/entry_points.txt
+-rw-r--r--   0 msp        (501) staff       (20)       55 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/requires.txt
+-rw-r--r--   0 msp        (501) staff       (20)        4 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/top_level.txt
```

### Comparing `msplotter-0.1.21/LICENSE` & `msplotter-0.1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/PKG-INFO` & `msplotter-0.1.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.21
+Version: 0.1.23
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -41,15 +41,15 @@
 - [blastn](https://www.ncbi.nlm.nih.gov/books/NBK569861/) must be installed locally and in the path
 
 ## Installation
 
 Create a virtual environment and install msplotter using pip as follows:
 
 ```bash
-pip intall msplotter
+pip install msplotter
 ```
 
 ## Usage and options
 
 To view all the options run:
 
 ```bash
```

### Comparing `msplotter-0.1.21/README.md` & `msplotter-0.1.23/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 - [blastn](https://www.ncbi.nlm.nih.gov/books/NBK569861/) must be installed locally and in the path
 
 ## Installation
 
 Create a virtual environment and install msplotter using pip as follows:
 
 ```bash
-pip intall msplotter
+pip install msplotter
 ```
 
 ## Usage and options
 
 To view all the options run:
 
 ```bash
```

### Comparing `msplotter-0.1.21/pyproject.toml` & `msplotter-0.1.23/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msplotter"
-version = "0.1.21"
+version = "0.1.23"
 authors = [
     {name = "Ivan Muñoz-Gutierrez", email = "ivan.munoz.gutierrez@gmail.com"},
 ]
 description = "Make a graphical representation of a blastn alignment"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [
```

### Comparing `msplotter-0.1.21/src/msp/arrows.py` & `msplotter-0.1.23/src/msp/arrows.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/colormap_picker.py` & `msplotter-0.1.23/src/msp/colormap_picker.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/gui.py` & `msplotter-0.1.23/src/msp/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 
 class App(customtkinter.CTk):
     """msplotter GUI."""
     def __init__(self):
         super().__init__()
         # Variables for BLASTing and plotting.
-        self.fig = None                        # matplotlib object.
+        self.figure_plt = None                        # matplotlib object.
         self.gb_files: list = None
-        self.figure = None                     # msplotter object.
+        self.figure_msp = None                     # msplotter object.
         self.identity_color: str = "Greys"
         self.colormap_range: tuple = (0, 0.75)
         self.annotate_sequences: bool = False
         self.annotate_genes: bool = False
         # Set layout parameters
         self.geometry('600x520')
         self.title('MSPlotter')
@@ -252,16 +252,14 @@
         self.display_window.insert(
             'end',
             f'The homology regions are going to be shown in `{cmap_name}` ' +
             f'with a range of colors between `{round(cmap_range[0])}-'
             f'{round(cmap_range[1])}`.'
         )
         self.display_window.configure(state='disabled')
-        # print(f'Selected cmap: {self.identity_color}')
-        # print(f'Selected cmap range: {self.colormap_range}')
 
     def update_annotate_seq_var(self):
         if self.annotate_seq_var.get() == 'No':
             self.annotate_sequences = False
         else:
             self.annotate_sequences = True
 
@@ -297,38 +295,32 @@
         # Make a list of `BlastnAlignment` classes from the xml blastn results.
         alignments = msp.get_alignment_records(xml_results)
         # Delete xml documents.
         msp.delete_files(xml_results)
         # Make a list of `GenBankRecord` classes from the gb files.
         gb_records = msp.get_gb_records(self.gb_files)
         # Make figure.
-        self.figure = msp.MakeFigure(
+        self.figure_msp = msp.MakeFigure(
             alignments,
             gb_records,
             alignments_position=self.align_plot_var.get().lower(),
             identity_color=self.identity_color,
             color_map_range=self.colormap_range,
-            # figure_name=self.gui_input.output_path,
-            # figure_format=self.gui_input.figure_format,
             annotate_sequences=self.annotate_sequences,
             annotate_genes=self.annotate_genes,
-            # sequence_name=info.sequence_name
             use_gui=True
         )
-        # # Plot figure using msplotter
-        # self.figure.make_figure()
-        # self.figure.display_figure()
         # Plot figure using the Plot class
-        self.fig = self.figure.make_figure()
+        self.figure_plt = self.figure_msp.make_figure()
         # Plot figure
-        Plot(self.fig, self.figure)
+        Plot(self.figure_plt, self.figure_msp)
 
     def on_closing(self):
-        if self.fig is not None:
-            self.figure.close_figure()
+        if self.figure_plt is not None:
+            self.figure_msp.close_figure()
         self.quit()
         self.destroy()
 
 
 def app_gui():
     app = App()
     app.mainloop()
```

### Comparing `msplotter-0.1.21/src/msp/images/Blues.png` & `msplotter-0.1.23/src/msp/images/Blues.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/BuGn.png` & `msplotter-0.1.23/src/msp/images/BuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/BuPu.png` & `msplotter-0.1.23/src/msp/images/BuPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/GnBu.png` & `msplotter-0.1.23/src/msp/images/GnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/Greens.png` & `msplotter-0.1.23/src/msp/images/Greens.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/OrRd.png` & `msplotter-0.1.23/src/msp/images/OrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/Oranges.png` & `msplotter-0.1.23/src/msp/images/Oranges.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/PuBu.png` & `msplotter-0.1.23/src/msp/images/PuBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/PuBuGn.png` & `msplotter-0.1.23/src/msp/images/PuBuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/PuRd.png` & `msplotter-0.1.23/src/msp/images/PuRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/Purples.png` & `msplotter-0.1.23/src/msp/images/Purples.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/RdPu.png` & `msplotter-0.1.23/src/msp/images/RdPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/Reds.png` & `msplotter-0.1.23/src/msp/images/Reds.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/YlGn.png` & `msplotter-0.1.23/src/msp/images/YlGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/YlGnBu.png` & `msplotter-0.1.23/src/msp/images/YlGnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/YlOrBr.png` & `msplotter-0.1.23/src/msp/images/YlOrBr.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/YlOrRd.png` & `msplotter-0.1.23/src/msp/images/YlOrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/images/logo.png` & `msplotter-0.1.23/src/msp/images/logo.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/msplotter.py` & `msplotter-0.1.23/src/msp/msplotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,14 @@
 For example, to show a gene in green add the tag `/Color="#00ff00"`. To reduce
 the manual manipulation of the GenBank file, you can edit the file with
 `Geneious` or another software and export the file with the new annotations.
 
 MSPlotter uses the `matplotlib` library. Therefore, you can modify the
 parameters in the `MakeFigure` class to customize your figure.
 
-Usage examples
---------------
-To make a figure with default parameters
-$ python msplotter -i path/file_1.gb path/file_2.gb path/file_3.gb
-
-To save a figure in pdf format
-$ python msplotter -i path/file_1.gb path/file_2.gb path/file_3.gb -f pdf
-
-Notes
------
-1. MSPlotter was designed to plot three sequences with lengths between 8 to 23
-   kb. However, the matplotlib parameters can be adjusted for larger, smaller,
-   or more sequences.
-2. blastn must be installed locally and in the path.
-
-Credits
--------
-1. Inspired by easyfig
-        Sullivan et al (2011) Bioinformatics 27(7):1009-1010
-        https://mjsull.github.io/Easyfig/
-
 License
 -------
 This file is part of MSPloter
 BSD 3-Clause License
 Copyright (c) 2023, Ivan Munoz Gutierrez
 """
 import os
@@ -47,14 +26,15 @@
 import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 import numpy as np
 from Bio import SeqIO
 from Bio.Blast import NCBIXML
 from Bio.Blast.Applications import NcbiblastnCommandline
 from Bio.SeqRecord import SeqRecord
+from pathlib import Path
 
 from msp.arrows import Arrow
 
 
 class GenBankRecord:
     """Store relevant info from a GenBank file.
 
@@ -304,18 +284,21 @@
         List of `BlastnAlignment` classes created from xml blastn results.
     num_alignments : int
         Number of alignments.
     gb_records : list
         List of `GenBankRecord` classes created from gb files.
     alignments_position : str
         Position of the alignments in the plot (default: `left`).
-    add_annotations_genes : Bool
+    annotate_genes : bool
         Annotate genes in plot (default: False).
-    add_annotations_sequences : Bool
-        Annotate sequences in plot (default: False).
+    annotate_genes_on_sequence : tuple with the str `top`, and/or `bottom`
+        Annotate genes at the top, bottom or both.
+    annotate_sequences : bool
+        Annotate sequences in plot (defalult: False). If True, the `top` and
+        `bottom` sequences are annotated.
     sequence_name : str
         String to access either `name` or `accession` from GenBankRecord class
         (default: `accession`). Either `name` or `accession` is used to
         annotate the sequence if `add_annotations_sequences` attribute is True.
     y_separation : int
         Distance between sequences in the y-axis (default: 10).
     sequence_color : str
@@ -323,32 +306,43 @@
         use any color name allowed by `Matplotlib`.
     sequence_width : int
         Width of lines representing sequences (default: 3).
     identity_color : str
         Color used to represent regions of homology (default: `Greys`). This
         color represent a `Matplotlib` colormap. Therefore, you should provide
         a valid colormap name.
+    color_map_range : tupple
+        Tyupple with a min and max value between 0 and 1. The min and max
+        values are used in color_map to determine the range of the color_map
+        to use (default: (0, 0.75)).
+    color_map : matplotlib colormaps object
+        Color map to represent homology regions.
     homology_padding : float
         Padding between lines representing sequences and regions of homology
         (default: 0.1). The number provided represents a fraction of the
         y_separation.
     save_figure : bool
-        Save plotted figure (deault: `True`).
-    figure_name : str
-        Name to save figure (default: `figure_1.pdf`).
+        Save plotted figure.
+    figure_name : Path
+        Output path with figure's name.
     figure_format : str
-        Format to save figure (default: `pdf`).
+        Format to save figure.
+    dpi : float
+        Resolution of figure in dots per inch (default: 300.0).
+    user_gui : bool
+        Run app in a graphical user interface (default: False).
     """
     def __init__(
         self, alignments, gb_records, alignments_position="left",
         annotate_genes=False, annotate_genes_on_sequence=("top", "bottom"),
         annotate_sequences=False, sequence_name="accession", y_separation=10,
         sequence_color="black", sequence_width=3, identity_color="Greys",
-        color_map_range=(0, 0.75), homology_padding=0.1, figure_name=None,
-        figure_format=None, use_gui=False
+        color_map_range=(0, 0.75), homology_padding=0.1,
+        figure_name=(Path.cwd() / 'figure.png'),
+        figure_format='png', dpi=300.0, use_gui=False
     ):
         self.alignments = alignments
         self.num_alignments = len(alignments)
         self.gb_records = gb_records
         self.alignments_position = alignments_position
         self.annotate_genes = annotate_genes
         self.annotate_genes_on_sequence = annotate_genes_on_sequence
@@ -371,14 +365,15 @@
             round(self.get_lowest_and_highest_homology()[0] * 100)
         )
         self.highest_homology = int(
             round(self.get_lowest_and_highest_homology()[1] * 100)
         )
         self.figure_name = figure_name
         self.figure_format = figure_format
+        self.dpi = dpi
         self.save_figure = self.check_save_figure()
         self.use_gui = use_gui
 
     def get_lowest_and_highest_homology(self) -> tuple:
         """Get the lowest and highest homologies in the alignment."""
         lowest = 100
         highest = 0
@@ -471,19 +466,19 @@
 
     def make_colormap(self, identity_color, min_val=0.0, max_val=1.0, n=100):
         """Make color map for homology regions."""
         try:
             cmap = plt.colormaps[identity_color]
         except KeyError:
             sys.exit(
-                f"Error: the identity color '{identity_color}' provided is " +
-                "not valid.\nUse the help option to find valid colors or " +
-                "visit:\n" +
-                "https://matplotlib.org/stable/tutorials/colors/colormaps.html\n" +
-                "for a complete list of valid options."
+                f"Error: the identity color '{identity_color}' provided is "
+                "not valid.\nUse the help option to find valid colors or "
+                "visit:\n"
+                "https://matplotlib.org/stable/tutorials/colors/colormaps.html"
+                "\nfor a complete list of valid options."
             )
         if min_val == 0 and max_val == 1:
             return cmap
         else:
             name = 'trunc_cmap'
             truncated_cmap = cmap(np.linspace(min_val, max_val, n))
             new_cmap = colors.LinearSegmentedColormap.from_list(
@@ -762,15 +757,17 @@
         if (self.figure_format is None) and (self.figure_name is None):
             return False
         else:
             return True
 
     def save_plot(self) -> None:
         """Save plot."""
-        plt.savefig(fname=self.figure_name, format=self.figure_format)
+        plt.savefig(
+            fname=self.figure_name, format=self.figure_format, dpi=self.dpi
+        )
 
     def display_figure(self) -> None:
         """Display and save figure."""
         # # Adjust the padding between and around subplots.
         # plt.tight_layout()
         # Save figure.
         if self.save_figure and not self.use_gui:
@@ -807,14 +804,15 @@
     figure = MakeFigure(
         alignments,
         gb_records,
         alignments_position=user_input.alignments_position,
         identity_color=user_input.identity_color,
         figure_name=user_input.output_path,
         figure_format=user_input.figure_format,
+        dpi=user_input.dpi,
         annotate_genes=user_input.annotate_genes,
         annotate_genes_on_sequence=user_input.annotate_genes_on_sequence,
         annotate_sequences=user_input.annotate_sequences,
         sequence_name=user_input.annotate_sequences_with
     )
     figure.make_figure()
     figure.display_figure()
```

### Comparing `msplotter-0.1.21/src/msp/slider_widget.py` & `msplotter-0.1.23/src/msp/slider_widget.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.21/src/msp/user_input.py` & `msplotter-0.1.23/src/msp/user_input.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,27 +20,29 @@
     """Store information provided by user via the command line."""
     def __init__(
             self,
             input_files: Union[list[Path], None] = None,
             output_folder: Union[None, Path] = None,
             figure_name: Union[None, str] = None,
             figure_format: Union[None, str] = None,
+            dpi: Union[None, float] = None,
             output_path: Union[None, Path] = None,
             alignments_position: Union[None, str] = None,
             identity_color: Union[None, str] = None,
             annotate_sequences: Union[None, bool] = None,
             annotate_sequences_with: Union[None, str] = None,
             annotate_genes: Union[None, bool] = None,
             annotate_genes_on_sequence: Union[None, tuple[str]] = None,
             gui: Union[None, bool] = None,
     ):
         self.input_files = input_files
         self.output_folder = output_folder
         self.figure_name = figure_name
         self.figure_format = figure_format
+        self.dpi = dpi
         self.output_path = output_path
         self.alignments_position = alignments_position
         self.identity_color = identity_color
         self.annotate_sequences = annotate_sequences
         self.annotate_sequences_with = annotate_sequences_with
         self.annotate_genes = annotate_genes
         self.annotate_genes_on_sequence = annotate_genes_on_sequence
@@ -58,15 +60,15 @@
             "Make a graphical representation of a blastn alignment."
         )
     )
     # Make argument groups.
     helper = parser.add_argument_group('Help')
     required = parser.add_argument_group('Required')
     optional = parser.add_argument_group('Optional')
-    gui = parser.add_argument_group('Graphic User Interfase')
+    gui = parser.add_argument_group('Graphical User Interfase')
     # ================== #
     # Help arguments     #
     # ================== #
     helper.add_argument(
         '-h', '--help', action='help',
         help='Show this help message and exit.'
     )
@@ -97,61 +99,71 @@
         help=(
             'Name of figure.\nDefault: `figure`.'
         )
     )
     optional.add_argument(
         '-f', '--format',
         help=(
-            'Format of figure.\nDefault: `pdf`.'
+            'Format of figure. Options: pdf, png, and svg.\n'
+            'For a complete list of valid options visit:\n'
+            'https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.savefig.html\n'
+            'Default: `png`.'
+        )
+    )
+    optional.add_argument(
+        '-d', '--dpi',
+        help=(
+            'Resolution in dots per inch.\n'
+            'Default: 300 (high resolution for print).'
         )
     )
     optional.add_argument(
         '--alignments_position',
         help=(
-            'Orientation of the alignments in the plot.\n' +
-            'Options: `left`, `center`, and `rigth`.\n' +
+            'Orientation of the alignments in the plot.\n'
+            'Options: `left`, `center`, and `rigth`.\n'
             'Default: `left`.'
         )
     )
     optional.add_argument(
         '--identity_color',
         help=(
-            'Color map representing homology regions.\n' +
-            'For a complete list of valid options visit:\n' +
-            'https://matplotlib.org/stable/tutorials/colors/colormaps.html\n' +
-            'Some options: `Greys`, `Purples`, `Blues`, and `Oranges`.\n' +
+            'Color map representing homology regions.\n'
+            'For a complete list of valid options visit:\n'
+            'https://matplotlib.org/stable/tutorials/colors/colormaps.html\n'
+            'Some options: `Greys`, `Purples`, `Blues`, and `Oranges`.\n'
             'Default: `Greys`.'
         )
     )
     optional.add_argument(
         '--annotate_sequences', nargs='?', const='accession',
         help=(
-            'Annotate sequences in the plot.\n' +
-            'Options: `accession`, `name`, and `fname`.\n' +
-            '`accession` and `name` are obtained from the `ACCESSION`\n' +
-            'and `LOCUS` gb file tags, repectively. `fname` is the file\n' +
-            'name.\n' +
-            'If the flag is provided without argument, the sequences will\n' +
+            'Annotate sequences in the plot.\n'
+            'Options: `accession`, `name`, and `fname`.\n'
+            '`accession` and `name` are obtained from the `ACCESSION`\n'
+            'and `LOCUS` gb file tags, repectively. `fname` is the file\n'
+            'name.\n'
+            'If the flag is provided without argument, the sequences will\n'
             'be annotated using `accession` numbers.'
         )
     )
     optional.add_argument(
         '--annotate_genes', nargs='?', const='top',
         help=(
-            'Annotate genes from top and bottom sequences.\n' +
-            'Options: `top`, `bottom`, and `both`.\n' +
-            'If the flag is provided without argument, only the genes at\n' +
+            'Annotate genes from top and bottom sequences.\n'
+            'Options: `top`, `bottom`, and `both`.\n'
+            'If the flag is provided without argument, only the genes at\n'
             'the top of the plot will be annotated.'
         )
     )
     # ================== #
     # GUI arguments      #
     # ================== #
     gui.add_argument(
-        '-g', '--gui', help='Run app in a graphic user interface.',
+        '-g', '--gui', help='Run app in a graphical user interface.',
         action='store_true'
     )
 
     # Parse command line arguments
     command_line_info = parser.parse_args()
     # Get command line arguments
     user_input = get_command_line_arguments(command_line_info)
@@ -184,21 +196,26 @@
     else:
         user_input.output_folder = Path.cwd()
     # If user doesn't provide figure_name, use `figure` as name.
     if figure_name := command_line_info.name:
         user_input.figure_name = figure_name
     else:
         user_input.figure_name = 'figure'
-    # If user doesn't provide figure format, use `pdf`.
+    # If user doesn't provide figure format, use `png`.
     if figure_format := command_line_info.format:
         user_input.figure_format = figure_format
     else:
-        user_input.figure_format = 'pdf'
+        user_input.figure_format = 'png'
     # If user provided figure_name and/or figure_format check correctness.
     check_figure_name_and_format(user_input)
+    # If user doesn't provide dpi, make 300 as default.
+    if dpi := command_line_info.dpi:
+        user_input.dpi = float(dpi)
+    else:
+        user_input.dpi = 300.0
     # Create output_path using output_folder, figure_name, and figure_format
     user_input.output_path = make_output_path(user_input)
     # If user didn't provide alignments position, use 'left'
     if alignments_position := command_line_info.alignments_position:
         user_input.alignments_position = check_alignments_position(
                 alignments_position
             )
@@ -256,16 +273,16 @@
     """Check mandatory arguments and conflicts with gui."""
     if not user_input.input_files and not user_input.gui:
         sys.exit('Error: the `--input` argument is mandatory.')
     if (
         (user_input.input_files and user_input.gui)
     ):
         sys.exit(
-            'Error: too many arguments.\nIf you want to activate the GUI ' +
-            'you only need to provide the `--gui` flag.\n' +
+            'Error: too many arguments.\nIf you want to activate the GUI '
+            'you only need to provide the `--gui` flag.\n'
             'Otherwise, no need to provide the `--gui` flag.'
         )
 
 
 def check_input_files(input_files: list[str]) -> list[Path]:
     """Check input files."""
     # Convert list of input files into list of paths.
@@ -297,16 +314,16 @@
     if len(extension) == 1:
         user_input.figure_name = (
             user_input.figure_name + '.' + user_input.figure_format
         )
     # If figure name has extension check if it matches figure format.
     elif extension[-1] != user_input.figure_format:
         sys.exit(
-            'Error: file name extension does no match figure format.\n' +
-            'The default format is `pdf`. If you want a different format ' +
+            'Error: file name extension does no match figure format.\n'
+            'The default format is `png`. If you want a different format '
             'provide it using the `--format` flag.'
         )
 
 
 def make_output_path(user_input: Namespace) -> Path:
     """Make output path."""
     if len(user_input.figure_name.split('.')) == 0:
@@ -324,16 +341,16 @@
         alignments_position == "left"
         or alignments_position == "center"
         or alignments_position == "right"
     ):
         return alignments_position
     else:
         sys.exit(
-            f'Error: parameter `alignment_position: {alignments_position}` ' +
-            'is not valid.\n' +
+            f'Error: parameter `alignment_position: {alignments_position}` '
+            'is not valid.\n'
             'Valid parameters are: `left`, `center`, or `right`.'
         )
 
 
 def check_annotate_sequences(annotate_sequences: str) -> Union[None, str]:
     """Check correct input for annotate sequences."""
     #TODO it looks like fname is off
@@ -341,27 +358,27 @@
         annotate_sequences == 'accession'
         or annotate_sequences == 'name'
         or annotate_sequences == 'fname'
     ):
         return annotate_sequences
     else:
         sys.exit(
-            f'Error: parameter `annotate_sequence: {annotate_sequences}` is ' +
-            'not valid.\n' +
+            f'Error: parameter `annotate_sequence: {annotate_sequences}` is '
+            'not valid.\n'
             'Valid parameter are: `accession`, `name`, or `fname`.'
         )
 
 
 def get_annotate_genes_info(annotate_genes: str) -> Union[None, tuple[str]]:
     """Get information to annotate genes in plot."""
     if annotate_genes == 'top':
         return ('top')
     elif annotate_genes == 'bottom':
         return ('bottom')
     elif annotate_genes == 'both':
         return ('top', 'bottom')
     else:
         sys.exit(
-            f'Error: parameter `annotate_genes: {annotate_genes}` is not ' +
-            'valid.\n' +
+            f'Error: parameter `annotate_genes: {annotate_genes}` is not '
+            'valid.\n'
             'Valid parameters are: `top`, `bottom` or `both`.'
         )
```

### Comparing `msplotter-0.1.21/src/msplotter.egg-info/PKG-INFO` & `msplotter-0.1.23/src/msplotter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.21
+Version: 0.1.23
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -41,15 +41,15 @@
 - [blastn](https://www.ncbi.nlm.nih.gov/books/NBK569861/) must be installed locally and in the path
 
 ## Installation
 
 Create a virtual environment and install msplotter using pip as follows:
 
 ```bash
-pip intall msplotter
+pip install msplotter
 ```
 
 ## Usage and options
 
 To view all the options run:
 
 ```bash
```

### Comparing `msplotter-0.1.21/src/msplotter.egg-info/SOURCES.txt` & `msplotter-0.1.23/src/msplotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

