# Comparing `tmp/CTkMessagebox-2.0.tar.gz` & `tmp/CTkMessagebox-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkMessagebox-2.0.tar", last modified: Sun May 21 15:11:45 2023, max compression
+gzip compressed data, was "CTkMessagebox-2.1.tar", last modified: Sat Jul  8 07:27:14 2023, max compression
```

## Comparing `CTkMessagebox-2.0.tar` & `CTkMessagebox-2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 15:11:45.324717 CTkMessagebox-2.0/
-drwxrwxrwx   0        0        0        0 2023-05-21 15:11:45.283712 CTkMessagebox-2.0/CTkMessagebox/
--rw-rw-rw-   0        0        0      232 2023-05-21 14:38:38.000000 CTkMessagebox-2.0/CTkMessagebox/__init__.py
--rw-rw-rw-   0        0        0    13914 2023-05-21 15:02:20.000000 CTkMessagebox-2.0/CTkMessagebox/ctkmessagebox.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:11:45.322717 CTkMessagebox-2.0/CTkMessagebox/icons/
--rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-2.0/CTkMessagebox/icons/cancel.png
--rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-2.0/CTkMessagebox/icons/check.png
--rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-2.0/CTkMessagebox/icons/info.png
--rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-2.0/CTkMessagebox/icons/question.png
--rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-2.0/CTkMessagebox/icons/warning.png
-drwxrwxrwx   0        0        0        0 2023-05-21 15:11:45.301716 CTkMessagebox-2.0/CTkMessagebox.egg-info/
--rw-rw-rw-   0        0        0     6291 2023-05-21 15:11:45.000000 CTkMessagebox-2.0/CTkMessagebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-05-21 15:11:45.000000 CTkMessagebox-2.0/CTkMessagebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2023-05-21 15:11:45.000000 CTkMessagebox-2.0/CTkMessagebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-21 15:11:45.000000 CTkMessagebox-2.0/CTkMessagebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 15:11:45.000000 CTkMessagebox-2.0/CTkMessagebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-2.0/LICENSE
--rw-rw-rw-   0        0        0     6291 2023-05-21 15:11:45.325717 CTkMessagebox-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5593 2023-05-21 15:11:13.000000 CTkMessagebox-2.0/README.md
--rw-rw-rw-   0        0        0      625 2023-05-21 15:11:45.327717 CTkMessagebox-2.0/setup.cfg
--rw-rw-rw-   0        0        0     1361 2023-05-21 14:38:15.000000 CTkMessagebox-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 07:27:14.185962 CTkMessagebox-2.1/
+drwxrwxrwx   0        0        0        0 2023-07-08 07:27:14.170336 CTkMessagebox-2.1/CTkMessagebox/
+-rw-rw-rw-   0        0        0      232 2023-07-08 07:24:55.000000 CTkMessagebox-2.1/CTkMessagebox/__init__.py
+-rw-rw-rw-   0        0        0    14359 2023-07-08 07:23:07.000000 CTkMessagebox-2.1/CTkMessagebox/ctkmessagebox.py
+drwxrwxrwx   0        0        0        0 2023-07-08 07:27:14.185962 CTkMessagebox-2.1/CTkMessagebox/icons/
+-rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-2.1/CTkMessagebox/icons/cancel.png
+-rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-2.1/CTkMessagebox/icons/check.png
+-rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-2.1/CTkMessagebox/icons/info.png
+-rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-2.1/CTkMessagebox/icons/question.png
+-rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-2.1/CTkMessagebox/icons/warning.png
+drwxrwxrwx   0        0        0        0 2023-07-08 07:27:14.185962 CTkMessagebox-2.1/CTkMessagebox.egg-info/
+-rw-rw-rw-   0        0        0     7104 2023-07-08 07:27:14.000000 CTkMessagebox-2.1/CTkMessagebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-07-08 07:27:14.000000 CTkMessagebox-2.1/CTkMessagebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2023-07-08 07:27:14.000000 CTkMessagebox-2.1/CTkMessagebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-08 07:27:14.000000 CTkMessagebox-2.1/CTkMessagebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-08 07:27:14.000000 CTkMessagebox-2.1/CTkMessagebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-2.1/LICENSE
+-rw-rw-rw-   0        0        0     7104 2023-07-08 07:27:14.185962 CTkMessagebox-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6406 2023-07-08 07:24:42.000000 CTkMessagebox-2.1/README.md
+-rw-rw-rw-   0        0        0      625 2023-07-08 07:27:14.185962 CTkMessagebox-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1361 2023-07-08 07:25:32.000000 CTkMessagebox-2.1/setup.py
```

### Comparing `CTkMessagebox-2.0/CTkMessagebox/ctkmessagebox.py` & `CTkMessagebox-2.1/CTkMessagebox/ctkmessagebox.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 CustomTkinter Messagebox
 Author: Akash Bora
-Version: 2.0
+Version: 2.1
 """
 
 import customtkinter
 from PIL import Image
 import os
 import sys
 import time
@@ -29,15 +29,15 @@
                  fg_color: str = "default",
                  text_color: str = "default",
                  title_color: str = "default",
                  button_text_color: str = "default",
                  button_width: int = None,
                  button_height: int = None,
                  cancel_button_color: str = None,
-                 cancel_button: str = "circle", # types: circle, cross or none
+                 cancel_button: str = None, # types: circle, cross or none
                  button_hover_color: str = "default",
                  icon: str = "info",
                  icon_size: tuple = None,
                  corner_radius: int = 15,
                  font: tuple = None,
                  header: bool = False,
                  topmost: bool = True,
@@ -71,34 +71,38 @@
     
         if topmost:
             self.attributes("-topmost", True)
         else:
             self.transient(self.master_window)
     
         if sys.platform.startswith("win"):
-            self.transparent_color = self._apply_appearance_mode(self._fg_color)
+            self.transparent_color = self._apply_appearance_mode(self.cget("fg_color"))
             self.attributes("-transparentcolor", self.transparent_color)
+            default_cancel_button = "cross"
         elif sys.platform.startswith("darwin"):
             self.transparent_color = 'systemTransparent'
             self.attributes("-transparent", True)
+            default_cancel_button = "circle"
         else:
             self.transparent_color = '#000001'
             corner_radius = 0
+            default_cancel_button = "cross"
 
         self.lift()
         self.config(background=self.transparent_color)
         self.protocol("WM_DELETE_WINDOW", self.button_event)
         self.grid_columnconfigure(0, weight=1)
         self.grid_rowconfigure(0, weight=1)    
         self.x = self.winfo_x()
         self.y = self.winfo_y()
         self._title = title
         self.message = message
         self.font = font
-        self.cancel_button = cancel_button
+        
+        self.cancel_button = cancel_button if cancel_button else default_cancel_button      
         self.round_corners = corner_radius if corner_radius<=30 else 30
         self.button_width = button_width if button_width else self.width/4
         self.button_height = button_height if button_height else 28
         if self.fade: self.attributes("-alpha", 0)
         
         if self.button_height>self.height/4: self.button_height = self.height/4 -20
         self.dot_color = cancel_button_color
@@ -116,17 +120,23 @@
         else:
             self.bg_color = bg_color
 
         if fg_color=="default":
             self.fg_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkFrame"]["top_fg_color"])
         else:
             self.fg_color = fg_color
-
+            
         default_button_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkButton"]["fg_color"])
-        
+
+        if sys.platform.startswith("win"):
+            if self.bg_color==self.transparent_color or self.fg_color==self.transparent_color:
+                self.configure(fg_color="#000001")
+                self.transparent_color = "#000001"
+                self.attributes("-transparentcolor", self.transparent_color)
+
         if button_color=="default":
             self.button_color = (default_button_color, default_button_color, default_button_color)
         else:
             if type(button_color) is tuple:
                 if len(button_color)==2:                
                     self.button_color = (button_color[0], button_color[1], default_button_color)
                 elif len(button_color)==1:
@@ -187,24 +197,22 @@
         else:
             self.frame_top.grid_rowconfigure((0,1,2), weight=1)
             
         self.frame_top.bind("<B1-Motion>", self.move_window)
         self.frame_top.bind("<ButtonPress-1>", self.oldxyset)
 
         if self.cancel_button=="cross":
-            self.button_close = customtkinter.CTkButton(self.frame_top, corner_radius=10, width=0, height=0, hover=False,
+            self.button_close = customtkinter.CTkButton(self.frame_top, corner_radius=10, width=0, height=0, hover=False, border_width=0,
                                                         text_color=self.dot_color if self.dot_color else self.title_color,
                                                         text="✕", fg_color="transparent", command=self.button_event)
             self.button_close.grid(row=0, column=3, sticky="ne", padx=5+self.border_width, pady=5+self.border_width)
-            self.button_close.configure(cursor="arrow")
         elif self.cancel_button=="circle":
-            self.button_close = customtkinter.CTkButton(self.frame_top, corner_radius=10, width=10, height=10, hover=False,
+            self.button_close = customtkinter.CTkButton(self.frame_top, corner_radius=10, width=10, height=10, hover=False, border_width=0,
                                                         text="", fg_color=self.dot_color if self.dot_color else "#c42b1c", command=self.button_event)     
             self.button_close.grid(row=0, column=3, sticky="ne", padx=10, pady=10)       
-            self.button_close.configure(cursor="arrow")
             
         self.title_label = customtkinter.CTkLabel(self.frame_top, width=1, text=self._title, text_color=self.title_color, font=self.font)
         self.title_label.grid(row=0, column=0, columnspan=4, sticky="nw", padx=(15,30), pady=5)
         self.title_label.bind("<B1-Motion>", self.move_window)
         self.title_label.bind("<ButtonPress-1>", self.oldxyset)
         
         self.info = customtkinter.CTkButton(self.frame_top,  width=1, height=self.height/2, corner_radius=0, text=self.message, font=self.font,
```

### Comparing `CTkMessagebox-2.0/CTkMessagebox/icons/cancel.png` & `CTkMessagebox-2.1/CTkMessagebox/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.0/CTkMessagebox/icons/check.png` & `CTkMessagebox-2.1/CTkMessagebox/icons/check.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.0/CTkMessagebox/icons/info.png` & `CTkMessagebox-2.1/CTkMessagebox/icons/info.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.0/CTkMessagebox/icons/question.png` & `CTkMessagebox-2.1/CTkMessagebox/icons/question.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.0/CTkMessagebox/icons/warning.png` & `CTkMessagebox-2.1/CTkMessagebox/icons/warning.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.0/CTkMessagebox.egg-info/PKG-INFO` & `CTkMessagebox-2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,394 +1,401 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2043 546b  : 2.1..Name: CTk
-00000020: 4d65 7373 6167 6562 6f78 0d0a 5665 7273  Messagebox..Vers
-00000030: 696f 6e3a 2032 2e30 0d0a 5375 6d6d 6172  ion: 2.0..Summar
-00000040: 793a 2041 206d 6f64 6572 6e20 6d65 7373  y: A modern mess
-00000050: 6167 6562 6f78 2066 6f72 2063 7573 746f  agebox for custo
-00000060: 6d74 6b69 6e74 6572 0d0a 486f 6d65 2d70  mtkinter..Home-p
-00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
-00000080: 6875 622e 636f 6d2f 416b 6173 6361 7065  hub.com/Akascape
-00000090: 2f43 546b 4d65 7373 6167 6562 6f78 0d0a  /CTkMessagebox..
-000000a0: 4175 7468 6f72 3a20 416b 6173 6820 426f  Author: Akash Bo
-000000b0: 7261 0d0a 4c69 6365 6e73 653a 2043 7265  ra..License: Cre
-000000c0: 6174 6976 6520 436f 6d6d 6f6e 7320 5a65  ative Commons Ze
-000000d0: 726f 2076 312e 3020 556e 6976 6572 7361  ro v1.0 Universa
-000000e0: 6c0d 0a4b 6579 776f 7264 733a 2063 7573  l..Keywords: cus
-000000f0: 746f 6d74 6b69 6e74 6572 2c63 7573 746f  tomtkinter,custo
-00000100: 6d74 6b69 6e74 6572 2d64 6961 6c6f 672c  mtkinter-dialog,
-00000110: 6375 7374 6f6d 746b 696e 7465 722d 6d65  customtkinter-me
-00000120: 7373 6167 6562 6f78 2c63 7573 746f 6d74  ssagebox,customt
-00000130: 6b69 6e74 6572 2d6d 6573 7361 6765 2d62  kinter-message-b
-00000140: 6f78 2c74 6b69 6e74 6572 2d6d 6573 7361  ox,tkinter-messa
-00000150: 6765 626f 782c 6375 7374 6f6d 746b 696e  gebox,customtkin
-00000160: 7465 722d 746b 696e 7465 722d 6d65 7373  ter-tkinter-mess
-00000170: 6167 6562 6f78 2c6d 6573 7361 6765 626f  agebox,messagebo
-00000180: 782d 7769 6467 6574 2c6d 6f64 6572 6e2d  x-widget,modern-
-00000190: 746b 696e 7465 722d 6d65 7373 6167 6562  tkinter-messageb
-000001a0: 6f78 2c63 746b 6d65 7373 6167 6562 6f78  ox,ctkmessagebox
-000001b0: 0d0a 436c 6173 7369 6669 6572 3a20 4c69  ..Classifier: Li
-000001c0: 6365 6e73 6520 3a3a 2043 4330 2031 2e30  cense :: CC0 1.0
-000001d0: 2055 6e69 7665 7273 616c 2028 4343 3020   Universal (CC0 
-000001e0: 312e 3029 2050 7562 6c69 6320 446f 6d61  1.0) Public Doma
-000001f0: 696e 2044 6564 6963 6174 696f 6e0d 0a43  in Dedication..C
-00000200: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000210: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000220: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-00000230: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000240: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000250: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-00000260: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
-00000270: 203e 3d33 2e36 0d0a 4465 7363 7269 7074   >=3.6..Descript
-00000280: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00000290: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0d  : text/markdown.
-000002a0: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-000002b0: 4943 454e 5345 0d0a 0d0a 2320 4354 6b4d  ICENSE....# CTkM
-000002c0: 6573 7361 6765 626f 780d 0a2a 2a41 206d  essagebox..**A m
-000002d0: 6f64 6572 6e20 616e 6420 6675 6c6c 7920  odern and fully 
-000002e0: 6375 7374 6f6d 697a 6162 6c65 206d 6573  customizable mes
-000002f0: 7361 6765 626f 7820 666f 7220 5b63 7573  sagebox for [cus
-00000300: 746f 6d74 6b69 6e74 6572 5d28 6874 7470  tomtkinter](http
-00000310: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-00000320: 6f6d 5363 6869 6d61 6e73 6b79 2f43 7573  omSchimansky/Cus
-00000330: 746f 6d54 6b69 6e74 6572 292a 2a0d 0a0d  tomTkinter)**...
-00000340: 0a23 2323 2046 6561 7475 7265 733a 0d0a  .### Features:..
-00000350: 2d20 4375 7374 6f6d 697a 6520 616c 6c20  - Customize all 
-00000360: 656c 656d 656e 7473 2069 6e73 6964 6520  elements inside 
-00000370: 7468 6520 6d65 7373 6167 6562 6f78 0d0a  the messagebox..
-00000380: 2d20 4164 6420 6375 7374 6f6d 2069 636f  - Add custom ico
-00000390: 6e73 206f 7220 696d 6167 6573 0d0a 2d20  ns or images..- 
-000003a0: 4164 6420 6d75 6c74 6970 6c65 206f 7074  Add multiple opt
-000003b0: 696f 6e73 2061 6363 6f72 6469 6e67 2074  ions according t
-000003c0: 6f20 796f 7572 2077 6973 680d 0a2d 204e  o your wish..- N
-000003d0: 6f20 7567 6c79 206c 6f6f 6b69 6e67 2068  o ugly looking h
-000003e0: 6561 6465 7220 6f72 2062 6f72 6465 7273  eader or borders
-000003f0: 0d0a 2d20 436f 6d65 7320 7769 7468 202a  ..- Comes with *
-00000400: 2a35 2064 6566 6175 6c74 2069 636f 6e73  *5 default icons
-00000410: 2a2a 0d0a 2d20 5370 6177 6e73 2061 7420  **..- Spawns at 
-00000420: 6365 6e74 6572 206f 6620 7468 6520 7363  center of the sc
-00000430: 7265 656e 2f61 7070 0d0a 2d20 4472 6167  reen/app..- Drag
-00000440: 6761 626c 6520 7769 6e64 6f77 0d0a 2d20  gable window..- 
-00000450: 4661 6465 2d69 6e2f 4661 6465 2d6f 7574  Fade-in/Fade-out
-00000460: 2077 696e 646f 7720 6566 6665 6374 0d0a   window effect..
-00000470: 0d0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-00000480: 6e0d 0a60 6060 0d0a 7069 7020 696e 7374  n..```..pip inst
-00000490: 616c 6c20 4354 6b4d 6573 7361 6765 626f  all CTkMessagebo
-000004a0: 780d 0a60 6060 0d0a 0d0a 5b3c 696d 6720  x..```....[<img 
-000004b0: 616c 743d 2247 6974 4875 6220 7265 706f  alt="GitHub repo
-000004c0: 2073 697a 6522 2073 7263 3d22 6874 7470   size" src="http
-000004d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000004e0: 696f 2f67 6974 6875 622f 7265 706f 2d73  io/github/repo-s
-000004f0: 697a 652f 416b 6173 6361 7065 2f43 546b  ize/Akascape/CTk
-00000500: 4d65 7373 6167 6562 6f78 3f26 636f 6c6f  Messagebox?&colo
-00000510: 723d 6772 6565 6e26 6c61 6265 6c3d 536f  r=green&label=So
-00000520: 7572 6365 2532 3043 6f64 6526 6c6f 676f  urce%20Code&logo
-00000530: 3d50 7974 686f 6e26 6c6f 676f 436f 6c6f  =Python&logoColo
-00000540: 723d 7965 6c6c 6f77 2673 7479 6c65 3d66  r=yellow&style=f
-00000550: 6f72 2d74 6865 2d62 6164 6765 2220 2077  or-the-badge"  w
-00000560: 6964 7468 3d22 3330 3022 3e5d 2868 7474  idth="300">](htt
-00000570: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000580: 416b 6173 6361 7065 2f43 546b 4d65 7373  Akascape/CTkMess
-00000590: 6167 6562 6f78 2f61 7263 6869 7665 2f72  agebox/archive/r
-000005a0: 6566 732f 6865 6164 732f 6d61 696e 2e7a  efs/heads/main.z
-000005b0: 6970 290d 0a0d 0a5b 215b 5079 5049 5d28  ip)....[![PyPI](
-000005c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000005d0: 6c64 732e 696f 2f70 7970 692f 762f 4354  lds.io/pypi/v/CT
-000005e0: 6b4d 6573 7361 6765 626f 783f 7374 796c  kMessagebox?styl
-000005f0: 653d 666c 6174 295d 2868 7474 7073 3a2f  e=flat)](https:/
-00000600: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000610: 742f 4354 6b4d 6573 7361 6765 626f 7829  t/CTkMessagebox)
-00000620: 0d0a 5b21 5b44 6f77 6e6c 6f61 6473 5d28  ..[![Downloads](
-00000630: 6874 7470 733a 2f2f 7374 6174 6963 2e70  https://static.p
-00000640: 6570 792e 7465 6368 2f62 6164 6765 2f63  epy.tech/badge/c
-00000650: 746b 6d65 7373 6167 6562 6f78 295d 2868  tkmessagebox)](h
-00000660: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-00000670: 2f70 726f 6a65 6374 2f63 746b 6d65 7373  /project/ctkmess
-00000680: 6167 6562 6f78 290d 0a21 5b50 6c61 7466  agebox)..![Platf
-00000690: 6f72 6d5d 2868 7474 7073 3a2f 2f69 6d67  orm](https://img
-000006a0: 2e73 6869 656c 6473 2e69 6f2f 706f 7765  .shields.io/powe
-000006b0: 7273 6865 6c6c 6761 6c6c 6572 792f 702f  rshellgallery/p/
-000006c0: 5065 7374 6572 3f63 6f6c 6f72 3d62 6c75  Pester?color=blu
-000006d0: 6529 0d0a 0d0a 2323 2048 6f77 2069 7420  e)....## How it 
-000006e0: 6c6f 6f6b 733f 0d0a 215b 5363 7265 656e  looks?..![Screen
-000006f0: 7368 6f74 5d28 6874 7470 733a 2f2f 7573  shot](https://us
-00000700: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00000710: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000720: 3839 3230 3634 3031 2f32 3231 3235 3835  89206401/2212585
-00000730: 3933 2d37 3530 3538 3837 382d 6235 3938  93-75058878-b598
-00000740: 2d34 3063 332d 3832 3861 2d31 6434 3461  -40c3-828a-1d44a
-00000750: 3663 6566 6237 332e 6a70 6729 0d0a 0d0a  6cefb73.jpg)....
-00000760: 2323 2045 7861 6d70 6c65 0d0a 6060 6070  ## Example..```p
-00000770: 7974 686f 6e0d 0a66 726f 6d20 4354 6b4d  ython..from CTkM
-00000780: 6573 7361 6765 626f 7820 696d 706f 7274  essagebox import
-00000790: 2043 546b 4d65 7373 6167 6562 6f78 0d0a   CTkMessagebox..
-000007a0: 696d 706f 7274 2063 7573 746f 6d74 6b69  import customtki
-000007b0: 6e74 6572 0d0a 0d0a 6465 6620 7368 6f77  nter....def show
-000007c0: 5f69 6e66 6f28 293a 0d0a 2020 2020 2320  _info():..    # 
-000007d0: 4465 6661 756c 7420 6d65 7373 6167 6562  Default messageb
-000007e0: 6f78 2066 6f72 2073 686f 7769 6e67 2073  ox for showing s
-000007f0: 6f6d 6520 696e 666f 726d 6174 696f 6e0d  ome information.
-00000800: 0a20 2020 2043 546b 4d65 7373 6167 6562  .    CTkMessageb
-00000810: 6f78 2874 6974 6c65 3d22 496e 666f 222c  ox(title="Info",
-00000820: 206d 6573 7361 6765 3d22 5468 6973 2069   message="This i
-00000830: 7320 6120 4354 6b4d 6573 7361 6765 626f  s a CTkMessagebo
-00000840: 7821 2229 0d0a 0d0a 6465 6620 7368 6f77  x!")....def show
-00000850: 5f63 6865 636b 6d61 726b 2829 3a0d 0a20  _checkmark():.. 
-00000860: 2020 2023 2053 686f 7720 736f 6d65 2070     # Show some p
-00000870: 6f73 6974 6976 6520 6d65 7373 6167 6520  ositive message 
-00000880: 7769 7468 2074 6865 2063 6865 636b 6d61  with the checkma
-00000890: 726b 2069 636f 6e0d 0a20 2020 2043 546b  rk icon..    CTk
-000008a0: 4d65 7373 6167 6562 6f78 286d 6573 7361  Messagebox(messa
-000008b0: 6765 3d22 4354 6b4d 6573 7361 6765 626f  ge="CTkMessagebo
-000008c0: 7820 6973 2073 7563 6365 7373 6675 6c6c  x is successfull
-000008d0: 7920 696e 7374 616c 6c65 642e 222c 0d0a  y installed.",..
-000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 6963 6f6e 3d22 6368 6563 6b22 2c20    icon="check", 
-00000900: 6f70 7469 6f6e 5f31 3d22 5468 616e 6b73  option_1="Thanks
-00000910: 2229 0d0a 2020 2020 0d0a 6465 6620 7368  ")..    ..def sh
-00000920: 6f77 5f65 7272 6f72 2829 3a0d 0a20 2020  ow_error():..   
-00000930: 2023 2053 686f 7720 736f 6d65 2065 7272   # Show some err
-00000940: 6f72 206d 6573 7361 6765 0d0a 2020 2020  or message..    
-00000950: 4354 6b4d 6573 7361 6765 626f 7828 7469  CTkMessagebox(ti
-00000960: 746c 653d 2245 7272 6f72 222c 206d 6573  tle="Error", mes
-00000970: 7361 6765 3d22 536f 6d65 7468 696e 6720  sage="Something 
-00000980: 7765 6e74 2077 726f 6e67 2121 2122 2c20  went wrong!!!", 
-00000990: 6963 6f6e 3d22 6361 6e63 656c 2229 0d0a  icon="cancel")..
-000009a0: 2020 2020 0d0a 6465 6620 7368 6f77 5f77      ..def show_w
-000009b0: 6172 6e69 6e67 2829 3a0d 0a20 2020 2023  arning():..    #
-000009c0: 2053 686f 7720 736f 6d65 2072 6574 7279   Show some retry
-000009d0: 2f63 616e 6365 6c20 7761 726e 696e 6773  /cancel warnings
-000009e0: 0d0a 2020 2020 6d73 6720 3d20 4354 6b4d  ..    msg = CTkM
-000009f0: 6573 7361 6765 626f 7828 7469 746c 653d  essagebox(title=
-00000a00: 2257 6172 6e69 6e67 204d 6573 7361 6765  "Warning Message
-00000a10: 2122 2c20 6d65 7373 6167 653d 2255 6e61  !", message="Una
-00000a20: 626c 6520 746f 2063 6f6e 6e65 6374 2122  ble to connect!"
-00000a30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000a40: 2020 2020 2069 636f 6e3d 2277 6172 6e69       icon="warni
-00000a50: 6e67 222c 206f 7074 696f 6e5f 313d 2243  ng", option_1="C
-00000a60: 616e 6365 6c22 2c20 6f70 7469 6f6e 5f32  ancel", option_2
-00000a70: 3d22 5265 7472 7922 290d 0a20 2020 200d  ="Retry")..    .
-00000a80: 0a20 2020 2069 6620 6d73 672e 6765 7428  .    if msg.get(
-00000a90: 293d 3d22 5265 7472 7922 3a0d 0a20 2020  )=="Retry":..   
-00000aa0: 2020 2020 2073 686f 775f 7761 726e 696e       show_warnin
-00000ab0: 6728 290d 0a20 2020 2020 2020 200d 0a64  g()..        ..d
-00000ac0: 6566 2061 736b 5f71 7565 7374 696f 6e28  ef ask_question(
-00000ad0: 293a 0d0a 2020 2020 2320 6765 7420 7965  ):..    # get ye
-00000ae0: 732f 6e6f 2061 6e73 7765 7273 0d0a 2020  s/no answers..  
-00000af0: 2020 6d73 6720 3d20 4354 6b4d 6573 7361    msg = CTkMessa
-00000b00: 6765 626f 7828 7469 746c 653d 2245 7869  gebox(title="Exi
-00000b10: 743f 222c 206d 6573 7361 6765 3d22 446f  t?", message="Do
-00000b20: 2079 6f75 2077 616e 7420 746f 2063 6c6f   you want to clo
-00000b30: 7365 2074 6865 2070 726f 6772 616d 3f22  se the program?"
-00000b40: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000b50: 2020 2020 2020 2020 2020 2069 636f 6e3d             icon=
-00000b60: 2271 7565 7374 696f 6e22 2c20 6f70 7469  "question", opti
-00000b70: 6f6e 5f31 3d22 4361 6e63 656c 222c 206f  on_1="Cancel", o
-00000b80: 7074 696f 6e5f 323d 224e 6f22 2c20 6f70  ption_2="No", op
-00000b90: 7469 6f6e 5f33 3d22 5965 7322 290d 0a20  tion_3="Yes").. 
-00000ba0: 2020 2072 6573 706f 6e73 6520 3d20 6d73     response = ms
-00000bb0: 672e 6765 7428 290d 0a20 2020 200d 0a20  g.get()..    .. 
-00000bc0: 2020 2069 6620 7265 7370 6f6e 7365 3d3d     if response==
-00000bd0: 2259 6573 223a 0d0a 2020 2020 2020 2020  "Yes":..        
-00000be0: 6170 702e 6465 7374 726f 7928 2920 2020  app.destroy()   
-00000bf0: 2020 2020 0d0a 2020 2020 656c 7365 3a0d      ..    else:.
-00000c00: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00000c10: 436c 6963 6b20 2759 6573 2720 746f 2065  Click 'Yes' to e
-00000c20: 7869 7421 2229 0d0a 2020 2020 2020 2020  xit!")..        
-00000c30: 2020 2020 2020 0d0a 6170 7020 3d20 6375        ..app = cu
-00000c40: 7374 6f6d 746b 696e 7465 722e 4354 6b28  stomtkinter.CTk(
-00000c50: 290d 0a61 7070 2e72 6f77 636f 6e66 6967  )..app.rowconfig
-00000c60: 7572 6528 2830 2c31 2c32 2c33 2c34 2c35  ure((0,1,2,3,4,5
-00000c70: 292c 2077 6569 6768 743d 3129 0d0a 6170  ), weight=1)..ap
-00000c80: 702e 636f 6c75 6d6e 636f 6e66 6967 7572  p.columnconfigur
-00000c90: 6528 302c 2077 6569 6768 743d 3129 0d0a  e(0, weight=1)..
-00000ca0: 6170 702e 6d69 6e73 697a 6528 3230 302c  app.minsize(200,
-00000cb0: 3235 3029 0d0a 0d0a 6375 7374 6f6d 746b  250)....customtk
-00000cc0: 696e 7465 722e 4354 6b4c 6162 656c 2861  inter.CTkLabel(a
-00000cd0: 7070 2c20 7465 7874 3d22 4354 6b20 4d65  pp, text="CTk Me
-00000ce0: 7373 6167 6562 6f78 2045 7861 6d70 6c65  ssagebox Example
-00000cf0: 7322 292e 6772 6964 2870 6164 783d 3230  s").grid(padx=20
-00000d00: 290d 0a63 7573 746f 6d74 6b69 6e74 6572  )..customtkinter
-00000d10: 2e43 546b 4275 7474 6f6e 2861 7070 2c20  .CTkButton(app, 
-00000d20: 7465 7874 3d22 4368 6563 6b20 4354 6b4d  text="Check CTkM
-00000d30: 6573 7361 6765 626f 7822 2c20 636f 6d6d  essagebox", comm
-00000d40: 616e 643d 7368 6f77 5f63 6865 636b 6d61  and=show_checkma
-00000d50: 726b 292e 6772 6964 2870 6164 783d 3230  rk).grid(padx=20
-00000d60: 2c20 7061 6479 3d31 302c 2073 7469 636b  , pady=10, stick
-00000d70: 793d 226e 6577 7322 290d 0a63 7573 746f  y="news")..custo
-00000d80: 6d74 6b69 6e74 6572 2e43 546b 4275 7474  mtkinter.CTkButt
-00000d90: 6f6e 2861 7070 2c20 7465 7874 3d22 5368  on(app, text="Sh
-00000da0: 6f77 2049 6e66 6f22 2c20 636f 6d6d 616e  ow Info", comman
-00000db0: 643d 7368 6f77 5f69 6e66 6f29 2e67 7269  d=show_info).gri
-00000dc0: 6428 7061 6478 3d32 302c 2070 6164 793d  d(padx=20, pady=
-00000dd0: 3130 2c20 7374 6963 6b79 3d22 6e65 7773  10, sticky="news
-00000de0: 2229 0d0a 6375 7374 6f6d 746b 696e 7465  ")..customtkinte
-00000df0: 722e 4354 6b42 7574 746f 6e28 6170 702c  r.CTkButton(app,
-00000e00: 2074 6578 743d 2253 686f 7720 4572 726f   text="Show Erro
-00000e10: 7222 2c20 636f 6d6d 616e 643d 7368 6f77  r", command=show
-00000e20: 5f65 7272 6f72 292e 6772 6964 2870 6164  _error).grid(pad
-00000e30: 783d 3230 2c20 7061 6479 3d31 302c 2073  x=20, pady=10, s
-00000e40: 7469 636b 793d 226e 6577 7322 290d 0a63  ticky="news")..c
-00000e50: 7573 746f 6d74 6b69 6e74 6572 2e43 546b  ustomtkinter.CTk
-00000e60: 4275 7474 6f6e 2861 7070 2c20 7465 7874  Button(app, text
-00000e70: 3d22 5368 6f77 2057 6172 6e69 6e67 222c  ="Show Warning",
-00000e80: 2063 6f6d 6d61 6e64 3d73 686f 775f 7761   command=show_wa
-00000e90: 726e 696e 6729 2e67 7269 6428 7061 6478  rning).grid(padx
-00000ea0: 3d32 302c 2070 6164 793d 3130 2c20 7374  =20, pady=10, st
-00000eb0: 6963 6b79 3d22 6e65 7773 2229 0d0a 6375  icky="news")..cu
-00000ec0: 7374 6f6d 746b 696e 7465 722e 4354 6b42  stomtkinter.CTkB
-00000ed0: 7574 746f 6e28 6170 702c 2074 6578 743d  utton(app, text=
-00000ee0: 2241 736b 2051 7565 7374 696f 6e22 2c20  "Ask Question", 
-00000ef0: 636f 6d6d 616e 643d 6173 6b5f 7175 6573  command=ask_ques
-00000f00: 7469 6f6e 292e 6772 6964 2870 6164 783d  tion).grid(padx=
-00000f10: 3230 2c20 7061 6479 3d28 3130 2c32 3029  20, pady=(10,20)
-00000f20: 2c20 7374 6963 6b79 3d22 6e65 7773 2229  , sticky="news")
-00000f30: 0d0a 0d0a 6170 702e 6d61 696e 6c6f 6f70  ....app.mainloop
-00000f40: 2829 0d0a 0d0a 6060 600d 0a0d 0a23 2320  ()....```....## 
-00000f50: 4f50 5449 4f4e 530d 0a20 207c 2050 6172  OPTIONS..  | Par
-00000f60: 616d 6574 6572 7320 207c 2044 6573 6372  ameters  | Descr
-00000f70: 6970 7469 6f6e 207c 0d0a 2020 7c20 2d2d  iption |..  | --
-00000f80: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
-00000f90: 2d2d 2d2d 207c 0d0a 2020 7c20 5f6d 6173  ---- |..  | _mas
-00000fa0: 7465 725f 207c 2073 6574 2070 6172 656e  ter_ | set paren
-00000fb0: 7420 7769 6e64 6f77 2028 6f70 7469 6f6e  t window (option
-00000fc0: 616c 292c 2074 6865 2062 6f78 2077 696c  al), the box wil
-00000fd0: 6c20 7370 6177 6e20 6174 2063 656e 7465  l spawn at cente
-00000fe0: 7220 6f66 2074 6865 2070 6172 656e 7420  r of the parent 
-00000ff0: 7769 6e64 6f77 207c 0d0a 2020 7c20 5f77  window |..  | _w
-00001000: 6964 7468 5f20 7c20 7769 6474 6820 6f66  idth_ | width of
-00001010: 2074 6865 2077 696e 646f 7720 696e 2070   the window in p
-00001020: 7820 286f 7074 696f 6e61 6c29 207c 0d0a  x (optional) |..
-00001030: 2020 7c20 5f68 6569 6768 745f 207c 2068    | _height_ | h
-00001040: 6569 6768 7420 6f66 2074 6865 2077 696e  eight of the win
-00001050: 646f 7720 696e 2070 7820 286f 7074 696f  dow in px (optio
-00001060: 6e61 6c29 207c 0d0a 2020 7c20 5f66 675f  nal) |..  | _fg_
-00001070: 636f 6c6f 725f 207c 2066 6f72 6772 6f75  color_ | forgrou
-00001080: 6e64 2063 6f6c 6f72 206f 6620 7468 6520  nd color of the 
-00001090: 6d65 7373 6167 6562 6f78 205b 6d69 6464  messagebox [midd
-000010a0: 6c65 2070 6f72 7469 6f6e 5d20 7c0d 0a20  le portion] |.. 
-000010b0: 207c 205f 6267 5f63 6f6c 6f72 5f20 207c   | _bg_color_  |
-000010c0: 2062 6163 6b67 726f 756e 6420 636f 6c6f   background colo
-000010d0: 7220 6f66 2074 6865 206d 6573 7361 6765  r of the message
-000010e0: 626f 7820 7c0d 0a20 207c 202a 2a5f 7469  box |..  | **_ti
-000010f0: 746c 655f 2a2a 207c 2074 6974 6c65 206f  tle_** | title o
-00001100: 6620 7468 6520 6d65 7373 6167 6562 6f78  f the messagebox
-00001110: 207c 0d0a 2020 7c20 2a2a 5f6d 6573 7361   |..  | **_messa
-00001120: 6765 5f2a 2a20 7c20 6d61 696e 206d 6573  ge_** | main mes
-00001130: 7361 6765 206f 6620 7468 6520 6d65 7373  sage of the mess
-00001140: 6167 6562 6f78 2077 6869 6368 2077 696c  agebox which wil
-00001150: 6c20 6265 2073 686f 776e 2061 7420 7468  l be shown at th
-00001160: 6520 6365 6e74 6572 207c 0d0a 2020 7c20  e center |..  | 
-00001170: 2a2a 5f6f 7074 696f 6e5f 315f 2a2a 207c  **_option_1_** |
-00001180: 2074 6865 2074 6578 7420 6f6e 2074 6865   the text on the
-00001190: 2066 6972 7374 2062 7574 746f 6e20 5b44   first button [D
-000011a0: 6566 6175 6c74 2069 7320 274f 4b27 5d20  efault is 'OK'] 
-000011b0: 7c0d 0a20 207c 202a 2a5f 6f70 7469 6f6e  |..  | **_option
-000011c0: 5f32 5f2a 2a20 7c20 7468 6520 7465 7874  _2_** | the text
-000011d0: 206f 6e20 7468 6520 7365 636f 6e64 2062   on the second b
-000011e0: 7574 746f 6e20 7c0d 0a20 207c 202a 2a5f  utton |..  | **_
-000011f0: 6f70 7469 6f6e 5f33 5f2a 2a20 7c20 7468  option_3_** | th
-00001200: 6520 7465 7874 206f 6e20 7468 6520 6c61  e text on the la
-00001210: 7374 2062 7574 746f 6e20 7c0d 0a20 207c  st button |..  |
-00001220: 205f 6f70 7469 6f6e 735f 207c 2064 6972   _options_ | dir
-00001230: 6563 746c 7920 7061 7373 2061 206c 6973  ectly pass a lis
-00001240: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
-00001250: 206f 7074 696f 6e73 2069 6e20 6f72 6465   options in orde
-00001260: 7220 7c0d 0a20 207c 205f 6275 7474 6f6e  r |..  | _button
-00001270: 5f63 6f6c 6f72 5f20 7c20 636f 6c6f 7220  _color_ | color 
-00001280: 6f66 2074 6865 2062 7574 746f 6e73 207c  of the buttons |
-00001290: 0d0a 2020 7c20 5f74 6578 745f 636f 6c6f  ..  | _text_colo
-000012a0: 725f 207c 2063 6f6c 6f72 206f 6620 7468  r_ | color of th
-000012b0: 6520 6d65 7373 6167 652d 7465 7874 207c  e message-text |
-000012c0: 0d0a 2020 7c20 5f74 6974 6c65 5f63 6f6c  ..  | _title_col
-000012d0: 6f72 5f20 7c20 636f 6c6f 7220 6f66 2074  or_ | color of t
-000012e0: 6865 2074 6974 6c65 2d74 6578 7420 7c0d  he title-text |.
-000012f0: 0a20 207c 205f 6275 7474 6f6e 5f74 6578  .  | _button_tex
-00001300: 745f 636f 6c6f 725f 207c 2063 6f6c 6f72  t_color_ | color
-00001310: 206f 6620 7468 6520 6275 7474 6f6e 2d74   of the button-t
-00001320: 6578 7420 7c0d 0a20 207c 205f 6275 7474  ext |..  | _butt
-00001330: 6f6e 5f68 6f76 6572 5f63 6f6c 6f72 5f20  on_hover_color_ 
-00001340: 7c20 686f 7665 7220 636f 6c6f 7220 6f66  | hover color of
-00001350: 2074 6865 2062 7574 746f 6e73 207c 0d0a   the buttons |..
-00001360: 2020 7c20 5f62 7574 746f 6e5f 7769 6474    | _button_widt
-00001370: 685f 207c 2077 6964 7468 206f 6620 7468  h_ | width of th
-00001380: 6520 6275 7474 6f6e 7320 696e 2070 7820  e buttons in px 
-00001390: 7c0d 0a20 207c 205f 6275 7474 6f6e 5f68  |..  | _button_h
-000013a0: 6569 6768 745f 207c 2068 6569 6768 7420  eight_ | height 
-000013b0: 6f66 2074 6865 2062 7574 746f 6e73 2069  of the buttons i
-000013c0: 6e20 7078 207c 0d0a 2020 7c20 5f62 6f72  n px |..  | _bor
-000013d0: 6465 725f 7769 6474 685f 207c 2077 6964  der_width_ | wid
-000013e0: 7468 206f 6620 7468 6520 626f 7264 6572  th of the border
-000013f0: 2061 726f 756e 6420 7468 6520 6d61 696e   around the main
-00001400: 2066 7261 6d65 205b 4465 6661 756c 7420   frame [Default 
-00001410: 6973 2031 5d20 7c0d 0a20 207c 205f 626f  is 1] |..  | _bo
-00001420: 7264 6572 5f63 6f6c 6f72 5f20 7c20 636f  rder_color_ | co
-00001430: 6c6f 7220 6f66 2074 6865 2066 7261 6d65  lor of the frame
-00001440: 2062 6f72 6465 7220 7c0d 0a20 207c 205f   border |..  | _
-00001450: 6361 6e63 656c 5f62 7574 746f 6e5f 207c  cancel_button_ |
-00001460: 2064 6566 696e 6520 7468 6520 6361 6e63   define the canc
-00001470: 656c 2062 7574 746f 6e20 7479 7065 3a20  el button type: 
-00001480: 2a2a 6369 7263 6c65 2c20 6372 6f73 7320  **circle, cross 
-00001490: 6f72 204e 6f6e 652a 2a20 7c0d 0a20 207c  or None** |..  |
-000014a0: 205f 6361 6e63 656c 5f62 7574 746f 6e5f   _cancel_button_
-000014b0: 636f 6c6f 725f 207c 2063 6f6c 6f72 206f  color_ | color o
-000014c0: 6620 7468 6520 2a2a 636c 6f73 652a 2a20  f the **close** 
-000014d0: 6275 7474 6f6e 2c20 2a2a 7365 7420 6974  button, **set it
-000014e0: 2074 6f20 2774 7261 6e73 7061 7265 6e74   to 'transparent
-000014f0: 2720 6966 2079 6f75 2077 616e 7420 746f  ' if you want to
-00001500: 2068 6964 6520 6974 2a2a 207c 0d0a 2020   hide it** |..  
-00001510: 7c20 2a2a 5f69 636f 6e5f 2a2a 207c 2069  | **_icon_** | i
-00001520: 636f 6e20 7468 6174 2077 696c 6c20 6265  con that will be
-00001530: 2073 686f 776e 2069 6e20 7468 6520 6d65   shown in the me
-00001540: 7373 6167 6562 6f78 205b 4465 6661 756c  ssagebox [Defaul
-00001550: 7420 6973 2074 6865 2027 696e 666f 2720  t is the 'info' 
-00001560: 6963 6f6e 5d20 7c0d 0a20 207c 205f 6963  icon] |..  | _ic
-00001570: 6f6e 5f73 697a 655f 207c 2064 6566 696e  on_size_ | defin
-00001580: 6520 7468 6520 7369 7a65 206f 6620 7468  e the size of th
-00001590: 6520 6963 6f6e 2069 6d61 6765 206d 616e  e icon image man
-000015a0: 7561 6c6c 7920 2874 7570 6c65 2920 7c0d  ually (tuple) |.
-000015b0: 0a20 207c 205f 636f 726e 6572 5f72 6164  .  | _corner_rad
-000015c0: 6975 735f 207c 2063 6f72 6e65 7220 726f  ius_ | corner ro
-000015d0: 756e 646e 6573 7320 6f66 2074 6865 206d  undness of the m
-000015e0: 6573 7361 6765 626f 7820 7769 6e64 6f77  essagebox window
-000015f0: 205b 2a2a 6e6f 7420 6170 706c 6963 6162   [**not applicab
-00001600: 6c65 2069 6e20 6c69 6e75 782a 2a5d 207c  le in linux**] |
-00001610: 0d0a 2020 7c20 5f66 6f6e 745f 207c 2066  ..  | _font_ | f
-00001620: 6f6e 7420 6f66 2074 6865 206d 6573 7361  ont of the messa
-00001630: 6765 626f 7820 7465 7874 2028 7475 706c  gebox text (tupl
-00001640: 6529 207c 0d0a 2020 7c20 5f68 6561 6465  e) |..  | _heade
-00001650: 725f 207c 2061 6464 2074 6865 206f 7269  r_ | add the ori
-00001660: 6769 6e61 6c20 6865 6164 6572 2062 6163  ginal header bac
-00001670: 6b20 6966 2079 6f75 2064 6f6e 2774 206c  k if you don't l
-00001680: 696b 6520 2a2a 6f76 6572 7269 6465 7265  ike **overridere
-00001690: 6469 7265 6374 2a2a 2028 626f 6f6c 2920  direct** (bool) 
-000016a0: 7c0d 0a20 207c 205f 746f 706d 6f73 745f  |..  | _topmost_
-000016b0: 207c 2064 6973 6162 6c65 2074 6865 2074   | disable the t
-000016c0: 6f70 6d6f 7374 2077 696e 646f 7720 6f75  opmost window ou
-000016d0: 7473 6964 6520 7468 6520 6170 7020 2862  tside the app (b
-000016e0: 6f6f 6c29 207c 0d0a 2020 7c20 2a2a 5f66  ool) |..  | **_f
-000016f0: 6164 655f 696e 5f64 7572 6174 696f 6e5f  ade_in_duration_
-00001700: 2a2a 207c 2065 6e61 626c 6520 6120 6661  ** | enable a fa
-00001710: 6465 2d69 6e20 616e 6420 6661 6465 2d6f  de-in and fade-o
-00001720: 7574 2061 6e69 6d61 7469 6f6e 2028 696e  ut animation (in
-00001730: 742c 2064 6566 6175 6c74 2069 7320 3029  t, default is 0)
-00001740: 2020 7c0d 0a20 200d 0a23 2323 2049 636f    |..  ..### Ico
-00001750: 6e73 0d0a 0d0a 2a2a 4465 6661 756c 7420  ns....**Default 
-00001760: 6963 6f6e 733a 2a2a 0d0a 0d0a 215b 6963  icons:**....![ic
-00001770: 6f6e 735d 2868 7474 7073 3a2f 2f75 7365  ons](https://use
-00001780: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-00001790: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f38  sercontent.com/8
-000017a0: 3932 3036 3430 312f 3232 3132 3538 3430  9206401/22125840
-000017b0: 332d 6161 6665 6135 3735 2d38 3536 652d  3-aafea575-856e-
-000017c0: 3466 3465 2d62 3361 662d 6639 3935 3738  4f4e-b3af-f99578
-000017d0: 3563 3938 3739 2e70 6e67 290d 0a0d 0a28  5c9879.png)....(
-000017e0: 2a54 6865 7365 2069 636f 6e73 2061 7265  *These icons are
-000017f0: 2063 7265 6174 6564 2075 7369 6e67 2050   created using P
-00001800: 6169 6e74 2e4e 4554 2c20 6672 6565 2074  aint.NET, free t
-00001810: 6f20 7573 6521 2a29 0d0a 0d0a 2a2a 466f  o use!*)....**Fo
-00001820: 7220 6375 7374 6f6d 2069 6d61 6765 732c  r custom images,
-00001830: 206a 7573 7420 7573 6520 6069 636f 6e3d   just use `icon=
-00001840: 2270 6174 685f 746f 5f74 6865 5f69 6d61  "path_to_the_ima
-00001850: 6765 2e70 6e67 2260 2a2a 0d0a 0d0a 2323  ge.png"`**....##
-00001860: 2054 6861 7427 7320 616c 6c2c 2068 6f70   That's all, hop
-00001870: 6520 6974 2077 696c 6c20 6865 6c70 2069  e it will help i
-00001880: 6e20 5549 2064 6576 656c 6f70 6d65 6e74  n UI development
-00001890: 210d 0a                                  !..
+00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000010: 7222 3e43 546b 4d65 7373 6167 6562 6f78  r">CTkMessagebox
+00000020: 3c2f 6831 3e0d 0a0d 0a3c 6833 2061 6c69  </h1>....<h3 ali
+00000030: 676e 3d22 6365 6e74 6572 223e 4120 6d6f  gn="center">A mo
+00000040: 6465 726e 2061 6e64 2066 756c 6c79 2063  dern and fully c
+00000050: 7573 746f 6d69 7a61 626c 6520 6d65 7373  ustomizable mess
+00000060: 6167 6562 6f78 2066 6f72 2043 7573 746f  agebox for Custo
+00000070: 6d54 6b69 6e74 6572 2c20 4120 6d75 7374  mTkinter, A must
+00000080: 2d68 6176 6520 6578 7465 6e73 696f 6e20  -have extension 
+00000090: 7061 636b 213c 2f68 333e 0d0a 0d0a 3c64  pack!</h3>....<d
+000000a0: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+000000b0: 223e 0d0a 2020 2020 0d0a 2020 3c61 2068  ">..    ..  <a h
+000000c0: 7265 663d 2268 7474 7073 3a2f 2f63 7265  ref="https://cre
+000000d0: 6174 6976 6563 6f6d 6d6f 6e73 2e6f 7267  ativecommons.org
+000000e0: 2f70 7562 6c69 6364 6f6d 6169 6e2f 7a65  /publicdomain/ze
+000000f0: 726f 2f31 2e30 2f22 3e21 5b4c 6963 656e  ro/1.0/">![Licen
+00000100: 7365 5d28 6874 7470 733a 2f2f 696d 672e  se](https://img.
+00000110: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000120: 2f4c 6963 656e 7365 2d43 4330 5f31 2e30  /License-CC0_1.0
+00000130: 2d62 6c75 6529 3c2f 613e 0d0a 2020 3c61  -blue)</a>..  <a
+00000140: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000150: 6974 6875 622e 636f 6d2f 416b 6173 6361  ithub.com/Akasca
+00000160: 7065 2f43 546b 4d65 7373 6167 6562 6f78  pe/CTkMessagebox
+00000170: 2f61 7263 6869 7665 2f72 6566 732f 6865  /archive/refs/he
+00000180: 6164 732f 6d61 696e 2e7a 6970 223e 215b  ads/main.zip">![
+00000190: 446f 776e 6c6f 6164 5d28 6874 7470 733a  Download](https:
+000001a0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000001b0: 2f62 6164 6765 2f53 6f75 7263 655f 436f  /badge/Source_Co
+000001c0: 6465 2d44 6f77 6e6c 6f61 642d 626c 7565  de-Download-blue
+000001d0: 293c 2f61 3e0d 0a20 205b 215b 5079 5049  )</a>..  [![PyPI
+000001e0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+000001f0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000200: 4354 6b4d 6573 7361 6765 626f 783f 7374  CTkMessagebox?st
+00000210: 796c 653d 666c 6174 295d 2868 7474 7073  yle=flat)](https
+00000220: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000230: 6563 742f 4354 6b4d 6573 7361 6765 626f  ect/CTkMessagebo
+00000240: 7829 0d0a 2020 5b21 5b44 6f77 6e6c 6f61  x)..  [![Downloa
+00000250: 6473 5d28 6874 7470 733a 2f2f 7374 6174  ds](https://stat
+00000260: 6963 2e70 6570 792e 7465 6368 2f62 6164  ic.pepy.tech/bad
+00000270: 6765 2f63 746b 6d65 7373 6167 6562 6f78  ge/ctkmessagebox
+00000280: 295d 2868 7474 7073 3a2f 2f70 6570 792e  )](https://pepy.
+00000290: 7465 6368 2f70 726f 6a65 6374 2f63 746b  tech/project/ctk
+000002a0: 6d65 7373 6167 6562 6f78 290d 0a20 2021  messagebox)..  !
+000002b0: 5b50 6c61 7466 6f72 6d5d 2868 7474 7073  [Platform](https
+000002c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000002d0: 6f2f 706f 7765 7273 6865 6c6c 6761 6c6c  o/powershellgall
+000002e0: 6572 792f 702f 5065 7374 6572 3f63 6f6c  ery/p/Pester?col
+000002f0: 6f72 3d62 6c75 6529 0d0a 3c2f 6469 763e  or=blue)..</div>
+00000300: 0d0a 0d0a 0d0a 3c64 6976 2061 6c69 676e  ......<div align
+00000310: 3d22 6365 6e74 6572 223e 0d0a 0d0a 215b  ="center">....![
+00000320: 3364 5d28 6874 7470 733a 2f2f 6769 7468  3d](https://gith
+00000330: 7562 2e63 6f6d 2f41 6b61 7363 6170 652f  ub.com/Akascape/
+00000340: 4354 6b4d 6573 7361 6765 626f 782f 6173  CTkMessagebox/as
+00000350: 7365 7473 2f38 3932 3036 3430 312f 6363  sets/89206401/cc
+00000360: 6535 3737 6663 2d36 3432 362d 3463 3039  e577fc-6426-4c09
+00000370: 2d39 3666 392d 6564 6538 3863 6166 3737  -96f9-ede88caf77
+00000380: 3834 290d 0a0d 0a3c 2f64 6976 3e0d 0a0d  84)....</div>...
+00000390: 0a3c 6272 3e0d 0a0d 0a3c 6832 2061 6c69  .<br>....<h2 ali
+000003a0: 676e 3d22 6365 6e74 6572 223e 2046 6561  gn="center"> Fea
+000003b0: 7475 7265 7320 3c2f 6832 3e0d 0a0d 0a2d  tures </h2>....-
+000003c0: 2043 7573 746f 6d69 7a65 2061 6c6c 2065   Customize all e
+000003d0: 6c65 6d65 6e74 7320 696e 7369 6465 2074  lements inside t
+000003e0: 6865 206d 6573 7361 6765 626f 780d 0a2d  he messagebox..-
+000003f0: 2041 6464 2063 7573 746f 6d20 6963 6f6e   Add custom icon
+00000400: 7320 6f72 2069 6d61 6765 730d 0a2d 2041  s or images..- A
+00000410: 6464 206d 756c 7469 706c 6520 6f70 7469  dd multiple opti
+00000420: 6f6e 7320 6163 636f 7264 696e 6720 746f  ons according to
+00000430: 2079 6f75 7220 7769 7368 0d0a 2d20 4e6f   your wish..- No
+00000440: 2075 676c 7920 6c6f 6f6b 696e 6720 6865   ugly looking he
+00000450: 6164 6572 206f 7220 626f 7264 6572 730d  ader or borders.
+00000460: 0a2d 2043 6f6d 6573 2077 6974 6820 2a2a  .- Comes with **
+00000470: 3520 6465 6661 756c 7420 6963 6f6e 732a  5 default icons*
+00000480: 2a0d 0a2d 2053 7061 776e 7320 6174 2063  *..- Spawns at c
+00000490: 656e 7465 7220 6f66 2074 6865 2073 6372  enter of the scr
+000004a0: 6565 6e2f 6170 700d 0a2d 2044 7261 6767  een/app..- Dragg
+000004b0: 6162 6c65 2077 696e 646f 770d 0a2d 2046  able window..- F
+000004c0: 6164 652d 696e 2f46 6164 652d 6f75 7420  ade-in/Fade-out 
+000004d0: 7769 6e64 6f77 2065 6666 6563 740d 0a0d  window effect...
+000004e0: 0a3c 6272 3e0d 0a0d 0a3c 6832 2061 6c69  .<br>....<h2 ali
+000004f0: 676e 3d22 6365 6e74 6572 223e 2049 6e73  gn="center"> Ins
+00000500: 7461 6c6c 6174 696f 6e20 3c2f 6832 3e0d  tallation </h2>.
+00000510: 0a0d 0a3c 6469 7620 616c 6967 6e3d 2263  ...<div align="c
+00000520: 656e 7465 7222 3e0d 0a0d 0a60 6060 0d0a  enter">....```..
+00000530: 7069 7020 696e 7374 616c 6c20 4354 6b4d  pip install CTkM
+00000540: 6573 7361 6765 626f 780d 0a60 6060 0d0a  essagebox..```..
+00000550: 0d0a 5b3c 696d 6720 616c 743d 2247 6974  ..[<img alt="Git
+00000560: 4875 6220 7265 706f 2073 697a 6522 2073  Hub repo size" s
+00000570: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000580: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+00000590: 622f 7265 706f 2d73 697a 652f 416b 6173  b/repo-size/Akas
+000005a0: 6361 7065 2f43 546b 4d65 7373 6167 6562  cape/CTkMessageb
+000005b0: 6f78 3f26 636f 6c6f 723d 6772 6565 6e26  ox?&color=green&
+000005c0: 6c61 6265 6c3d 536f 7572 6365 2532 3043  label=Source%20C
+000005d0: 6f64 6526 6c6f 676f 3d50 7974 686f 6e26  ode&logo=Python&
+000005e0: 6c6f 676f 436f 6c6f 723d 7965 6c6c 6f77  logoColor=yellow
+000005f0: 2673 7479 6c65 3d66 6f72 2d74 6865 2d62  &style=for-the-b
+00000600: 6164 6765 2220 2077 6964 7468 3d22 3330  adge"  width="30
+00000610: 3022 3e5d 2868 7474 7073 3a2f 2f67 6974  0">](https://git
+00000620: 6875 622e 636f 6d2f 416b 6173 6361 7065  hub.com/Akascape
+00000630: 2f43 546b 4d65 7373 6167 6562 6f78 2f61  /CTkMessagebox/a
+00000640: 7263 6869 7665 2f72 6566 732f 6865 6164  rchive/refs/head
+00000650: 732f 6d61 696e 2e7a 6970 290d 0a0d 0a0d  s/main.zip).....
+00000660: 0a3c 2f64 6976 3e0d 0a0d 0a3c 6272 3e0d  .</div>....<br>.
+00000670: 0a0d 0a3c 6832 2061 6c69 676e 3d22 6365  ...<h2 align="ce
+00000680: 6e74 6572 223e 2048 6f77 2069 7420 6c6f  nter"> How it lo
+00000690: 6f6b 733f 203c 2f68 323e 0d0a 0d0a 3c64  oks? </h2>....<d
+000006a0: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+000006b0: 223e 0d0a 0d0a 215b 5363 7265 656e 7368  ">....![Screensh
+000006c0: 6f74 5d28 6874 7470 733a 2f2f 7573 6572  ot](https://user
+000006d0: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+000006e0: 6572 636f 6e74 656e 742e 636f 6d2f 3839  ercontent.com/89
+000006f0: 3230 3634 3031 2f32 3231 3235 3835 3933  206401/221258593
+00000700: 2d37 3530 3538 3837 382d 6235 3938 2d34  -75058878-b598-4
+00000710: 3063 332d 3832 3861 2d31 6434 3461 3663  0c3-828a-1d44a6c
+00000720: 6566 6237 332e 6a70 6729 0d0a 0d0a 3c2f  efb73.jpg)....</
+00000730: 6469 763e 0d0a 0d0a 3c62 723e 0d0a 0d0a  div>....<br>....
+00000740: 3c68 3220 616c 6967 6e3d 2263 656e 7465  <h2 align="cente
+00000750: 7222 3e20 4578 616d 706c 6520 3c2f 6832  r"> Example </h2
+00000760: 3e0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  >....```python..
+00000770: 6672 6f6d 2043 546b 4d65 7373 6167 6562  from CTkMessageb
+00000780: 6f78 2069 6d70 6f72 7420 4354 6b4d 6573  ox import CTkMes
+00000790: 7361 6765 626f 780d 0a69 6d70 6f72 7420  sagebox..import 
+000007a0: 6375 7374 6f6d 746b 696e 7465 720d 0a0d  customtkinter...
+000007b0: 0a64 6566 2073 686f 775f 696e 666f 2829  .def show_info()
+000007c0: 3a0d 0a20 2020 2023 2044 6566 6175 6c74  :..    # Default
+000007d0: 206d 6573 7361 6765 626f 7820 666f 7220   messagebox for 
+000007e0: 7368 6f77 696e 6720 736f 6d65 2069 6e66  showing some inf
+000007f0: 6f72 6d61 7469 6f6e 0d0a 2020 2020 4354  ormation..    CT
+00000800: 6b4d 6573 7361 6765 626f 7828 7469 746c  kMessagebox(titl
+00000810: 653d 2249 6e66 6f22 2c20 6d65 7373 6167  e="Info", messag
+00000820: 653d 2254 6869 7320 6973 2061 2043 546b  e="This is a CTk
+00000830: 4d65 7373 6167 6562 6f78 2122 290d 0a0d  Messagebox!")...
+00000840: 0a64 6566 2073 686f 775f 6368 6563 6b6d  .def show_checkm
+00000850: 6172 6b28 293a 0d0a 2020 2020 2320 5368  ark():..    # Sh
+00000860: 6f77 2073 6f6d 6520 706f 7369 7469 7665  ow some positive
+00000870: 206d 6573 7361 6765 2077 6974 6820 7468   message with th
+00000880: 6520 6368 6563 6b6d 6172 6b20 6963 6f6e  e checkmark icon
+00000890: 0d0a 2020 2020 4354 6b4d 6573 7361 6765  ..    CTkMessage
+000008a0: 626f 7828 6d65 7373 6167 653d 2243 546b  box(message="CTk
+000008b0: 4d65 7373 6167 6562 6f78 2069 7320 7375  Messagebox is su
+000008c0: 6363 6573 7366 756c 6c79 2069 6e73 7461  ccessfully insta
+000008d0: 6c6c 6564 2e22 2c0d 0a20 2020 2020 2020  lled.",..       
+000008e0: 2020 2020 2020 2020 2020 2069 636f 6e3d             icon=
+000008f0: 2263 6865 636b 222c 206f 7074 696f 6e5f  "check", option_
+00000900: 313d 2254 6861 6e6b 7322 290d 0a20 2020  1="Thanks")..   
+00000910: 200d 0a64 6566 2073 686f 775f 6572 726f   ..def show_erro
+00000920: 7228 293a 0d0a 2020 2020 2320 5368 6f77  r():..    # Show
+00000930: 2073 6f6d 6520 6572 726f 7220 6d65 7373   some error mess
+00000940: 6167 650d 0a20 2020 2043 546b 4d65 7373  age..    CTkMess
+00000950: 6167 6562 6f78 2874 6974 6c65 3d22 4572  agebox(title="Er
+00000960: 726f 7222 2c20 6d65 7373 6167 653d 2253  ror", message="S
+00000970: 6f6d 6574 6869 6e67 2077 656e 7420 7772  omething went wr
+00000980: 6f6e 6721 2121 222c 2069 636f 6e3d 2263  ong!!!", icon="c
+00000990: 616e 6365 6c22 290d 0a20 2020 200d 0a64  ancel")..    ..d
+000009a0: 6566 2073 686f 775f 7761 726e 696e 6728  ef show_warning(
+000009b0: 293a 0d0a 2020 2020 2320 5368 6f77 2073  ):..    # Show s
+000009c0: 6f6d 6520 7265 7472 792f 6361 6e63 656c  ome retry/cancel
+000009d0: 2077 6172 6e69 6e67 730d 0a20 2020 206d   warnings..    m
+000009e0: 7367 203d 2043 546b 4d65 7373 6167 6562  sg = CTkMessageb
+000009f0: 6f78 2874 6974 6c65 3d22 5761 726e 696e  ox(title="Warnin
+00000a00: 6720 4d65 7373 6167 6521 222c 206d 6573  g Message!", mes
+00000a10: 7361 6765 3d22 556e 6162 6c65 2074 6f20  sage="Unable to 
+00000a20: 636f 6e6e 6563 7421 222c 0d0a 2020 2020  connect!",..    
+00000a30: 2020 2020 2020 2020 2020 2020 2020 6963                ic
+00000a40: 6f6e 3d22 7761 726e 696e 6722 2c20 6f70  on="warning", op
+00000a50: 7469 6f6e 5f31 3d22 4361 6e63 656c 222c  tion_1="Cancel",
+00000a60: 206f 7074 696f 6e5f 323d 2252 6574 7279   option_2="Retry
+00000a70: 2229 0d0a 2020 2020 0d0a 2020 2020 6966  ")..    ..    if
+00000a80: 206d 7367 2e67 6574 2829 3d3d 2252 6574   msg.get()=="Ret
+00000a90: 7279 223a 0d0a 2020 2020 2020 2020 7368  ry":..        sh
+00000aa0: 6f77 5f77 6172 6e69 6e67 2829 0d0a 2020  ow_warning()..  
+00000ab0: 2020 2020 2020 0d0a 6465 6620 6173 6b5f        ..def ask_
+00000ac0: 7175 6573 7469 6f6e 2829 3a0d 0a20 2020  question():..   
+00000ad0: 2023 2067 6574 2079 6573 2f6e 6f20 616e   # get yes/no an
+00000ae0: 7377 6572 730d 0a20 2020 206d 7367 203d  swers..    msg =
+00000af0: 2043 546b 4d65 7373 6167 6562 6f78 2874   CTkMessagebox(t
+00000b00: 6974 6c65 3d22 4578 6974 3f22 2c20 6d65  itle="Exit?", me
+00000b10: 7373 6167 653d 2244 6f20 796f 7520 7761  ssage="Do you wa
+00000b20: 6e74 2074 6f20 636c 6f73 6520 7468 6520  nt to close the 
+00000b30: 7072 6f67 7261 6d3f 222c 0d0a 2020 2020  program?",..    
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2020 2020 6963 6f6e 3d22 7175 6573 7469      icon="questi
+00000b60: 6f6e 222c 206f 7074 696f 6e5f 313d 2243  on", option_1="C
+00000b70: 616e 6365 6c22 2c20 6f70 7469 6f6e 5f32  ancel", option_2
+00000b80: 3d22 4e6f 222c 206f 7074 696f 6e5f 333d  ="No", option_3=
+00000b90: 2259 6573 2229 0d0a 2020 2020 7265 7370  "Yes")..    resp
+00000ba0: 6f6e 7365 203d 206d 7367 2e67 6574 2829  onse = msg.get()
+00000bb0: 0d0a 2020 2020 0d0a 2020 2020 6966 2072  ..    ..    if r
+00000bc0: 6573 706f 6e73 653d 3d22 5965 7322 3a0d  esponse=="Yes":.
+00000bd0: 0a20 2020 2020 2020 2061 7070 2e64 6573  .        app.des
+00000be0: 7472 6f79 2829 2020 2020 2020 200d 0a20  troy()       .. 
+00000bf0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000c00: 2020 7072 696e 7428 2243 6c69 636b 2027    print("Click '
+00000c10: 5965 7327 2074 6f20 6578 6974 2122 290d  Yes' to exit!").
+00000c20: 0a20 2020 2020 2020 2020 2020 2020 200d  .              .
+00000c30: 0a61 7070 203d 2063 7573 746f 6d74 6b69  .app = customtki
+00000c40: 6e74 6572 2e43 546b 2829 0d0a 6170 702e  nter.CTk()..app.
+00000c50: 726f 7763 6f6e 6669 6775 7265 2828 302c  rowconfigure((0,
+00000c60: 312c 322c 332c 342c 3529 2c20 7765 6967  1,2,3,4,5), weig
+00000c70: 6874 3d31 290d 0a61 7070 2e63 6f6c 756d  ht=1)..app.colum
+00000c80: 6e63 6f6e 6669 6775 7265 2830 2c20 7765  nconfigure(0, we
+00000c90: 6967 6874 3d31 290d 0a61 7070 2e6d 696e  ight=1)..app.min
+00000ca0: 7369 7a65 2832 3030 2c32 3530 290d 0a0d  size(200,250)...
+00000cb0: 0a63 7573 746f 6d74 6b69 6e74 6572 2e43  .customtkinter.C
+00000cc0: 546b 4c61 6265 6c28 6170 702c 2074 6578  TkLabel(app, tex
+00000cd0: 743d 2243 546b 204d 6573 7361 6765 626f  t="CTk Messagebo
+00000ce0: 7820 4578 616d 706c 6573 2229 2e67 7269  x Examples").gri
+00000cf0: 6428 7061 6478 3d32 3029 0d0a 6375 7374  d(padx=20)..cust
+00000d00: 6f6d 746b 696e 7465 722e 4354 6b42 7574  omtkinter.CTkBut
+00000d10: 746f 6e28 6170 702c 2074 6578 743d 2243  ton(app, text="C
+00000d20: 6865 636b 2043 546b 4d65 7373 6167 6562  heck CTkMessageb
+00000d30: 6f78 222c 2063 6f6d 6d61 6e64 3d73 686f  ox", command=sho
+00000d40: 775f 6368 6563 6b6d 6172 6b29 2e67 7269  w_checkmark).gri
+00000d50: 6428 7061 6478 3d32 302c 2070 6164 793d  d(padx=20, pady=
+00000d60: 3130 2c20 7374 6963 6b79 3d22 6e65 7773  10, sticky="news
+00000d70: 2229 0d0a 6375 7374 6f6d 746b 696e 7465  ")..customtkinte
+00000d80: 722e 4354 6b42 7574 746f 6e28 6170 702c  r.CTkButton(app,
+00000d90: 2074 6578 743d 2253 686f 7720 496e 666f   text="Show Info
+00000da0: 222c 2063 6f6d 6d61 6e64 3d73 686f 775f  ", command=show_
+00000db0: 696e 666f 292e 6772 6964 2870 6164 783d  info).grid(padx=
+00000dc0: 3230 2c20 7061 6479 3d31 302c 2073 7469  20, pady=10, sti
+00000dd0: 636b 793d 226e 6577 7322 290d 0a63 7573  cky="news")..cus
+00000de0: 746f 6d74 6b69 6e74 6572 2e43 546b 4275  tomtkinter.CTkBu
+00000df0: 7474 6f6e 2861 7070 2c20 7465 7874 3d22  tton(app, text="
+00000e00: 5368 6f77 2045 7272 6f72 222c 2063 6f6d  Show Error", com
+00000e10: 6d61 6e64 3d73 686f 775f 6572 726f 7229  mand=show_error)
+00000e20: 2e67 7269 6428 7061 6478 3d32 302c 2070  .grid(padx=20, p
+00000e30: 6164 793d 3130 2c20 7374 6963 6b79 3d22  ady=10, sticky="
+00000e40: 6e65 7773 2229 0d0a 6375 7374 6f6d 746b  news")..customtk
+00000e50: 696e 7465 722e 4354 6b42 7574 746f 6e28  inter.CTkButton(
+00000e60: 6170 702c 2074 6578 743d 2253 686f 7720  app, text="Show 
+00000e70: 5761 726e 696e 6722 2c20 636f 6d6d 616e  Warning", comman
+00000e80: 643d 7368 6f77 5f77 6172 6e69 6e67 292e  d=show_warning).
+00000e90: 6772 6964 2870 6164 783d 3230 2c20 7061  grid(padx=20, pa
+00000ea0: 6479 3d31 302c 2073 7469 636b 793d 226e  dy=10, sticky="n
+00000eb0: 6577 7322 290d 0a63 7573 746f 6d74 6b69  ews")..customtki
+00000ec0: 6e74 6572 2e43 546b 4275 7474 6f6e 2861  nter.CTkButton(a
+00000ed0: 7070 2c20 7465 7874 3d22 4173 6b20 5175  pp, text="Ask Qu
+00000ee0: 6573 7469 6f6e 222c 2063 6f6d 6d61 6e64  estion", command
+00000ef0: 3d61 736b 5f71 7565 7374 696f 6e29 2e67  =ask_question).g
+00000f00: 7269 6428 7061 6478 3d32 302c 2070 6164  rid(padx=20, pad
+00000f10: 793d 2831 302c 3230 292c 2073 7469 636b  y=(10,20), stick
+00000f20: 793d 226e 6577 7322 290d 0a0d 0a61 7070  y="news")....app
+00000f30: 2e6d 6169 6e6c 6f6f 7028 290d 0a0d 0a60  .mainloop()....`
+00000f40: 6060 0d0a 0d0a 3c62 723e 0d0a 0d0a 3c68  ``....<br>....<h
+00000f50: 3220 616c 6967 6e3d 2263 656e 7465 7222  2 align="center"
+00000f60: 3e20 4f50 5449 4f4e 5320 3c2f 6832 3e0d  > OPTIONS </h2>.
+00000f70: 0a0d 0a3c 6469 7620 616c 6967 6e3d 2263  ...<div align="c
+00000f80: 656e 7465 7222 3e0d 0a0d 0a20 207c 2050  enter">....  | P
+00000f90: 6172 616d 6574 6572 7320 207c 2044 6573  arameters  | Des
+00000fa0: 6372 6970 7469 6f6e 207c 0d0a 2020 7c20  cription |..  | 
+00000fb0: 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d  -------- | -----
+00000fc0: 2d2d 2d2d 2d2d 207c 0d0a 2020 7c20 5f6d  ------ |..  | _m
+00000fd0: 6173 7465 725f 207c 2073 6574 2070 6172  aster_ | set par
+00000fe0: 656e 7420 7769 6e64 6f77 2028 6f70 7469  ent window (opti
+00000ff0: 6f6e 616c 292c 2074 6865 2062 6f78 2077  onal), the box w
+00001000: 696c 6c20 7370 6177 6e20 6174 2063 656e  ill spawn at cen
+00001010: 7465 7220 6f66 2074 6865 2070 6172 656e  ter of the paren
+00001020: 7420 7769 6e64 6f77 207c 0d0a 2020 7c20  t window |..  | 
+00001030: 5f77 6964 7468 5f20 7c20 7769 6474 6820  _width_ | width 
+00001040: 6f66 2074 6865 2077 696e 646f 7720 696e  of the window in
+00001050: 2070 7820 286f 7074 696f 6e61 6c29 207c   px (optional) |
+00001060: 0d0a 2020 7c20 5f68 6569 6768 745f 207c  ..  | _height_ |
+00001070: 2068 6569 6768 7420 6f66 2074 6865 2077   height of the w
+00001080: 696e 646f 7720 696e 2070 7820 286f 7074  indow in px (opt
+00001090: 696f 6e61 6c29 207c 0d0a 2020 7c20 5f66  ional) |..  | _f
+000010a0: 675f 636f 6c6f 725f 207c 2066 6f72 6772  g_color_ | forgr
+000010b0: 6f75 6e64 2063 6f6c 6f72 206f 6620 7468  ound color of th
+000010c0: 6520 6d65 7373 6167 6562 6f78 205b 6d69  e messagebox [mi
+000010d0: 6464 6c65 2070 6f72 7469 6f6e 5d20 7c0d  ddle portion] |.
+000010e0: 0a20 207c 205f 6267 5f63 6f6c 6f72 5f20  .  | _bg_color_ 
+000010f0: 207c 2062 6163 6b67 726f 756e 6420 636f   | background co
+00001100: 6c6f 7220 6f66 2074 6865 206d 6573 7361  lor of the messa
+00001110: 6765 626f 7820 7c0d 0a20 207c 202a 2a5f  gebox |..  | **_
+00001120: 7469 746c 655f 2a2a 207c 2074 6974 6c65  title_** | title
+00001130: 206f 6620 7468 6520 6d65 7373 6167 6562   of the messageb
+00001140: 6f78 207c 0d0a 2020 7c20 2a2a 5f6d 6573  ox |..  | **_mes
+00001150: 7361 6765 5f2a 2a20 7c20 6d61 696e 206d  sage_** | main m
+00001160: 6573 7361 6765 206f 6620 7468 6520 6d65  essage of the me
+00001170: 7373 6167 6562 6f78 2077 6869 6368 2077  ssagebox which w
+00001180: 696c 6c20 6265 2073 686f 776e 2061 7420  ill be shown at 
+00001190: 7468 6520 6365 6e74 6572 207c 0d0a 2020  the center |..  
+000011a0: 7c20 2a2a 5f6f 7074 696f 6e5f 315f 2a2a  | **_option_1_**
+000011b0: 207c 2074 6865 2074 6578 7420 6f6e 2074   | the text on t
+000011c0: 6865 2066 6972 7374 2062 7574 746f 6e20  he first button 
+000011d0: 5b44 6566 6175 6c74 2069 7320 274f 4b27  [Default is 'OK'
+000011e0: 5d20 7c0d 0a20 207c 202a 2a5f 6f70 7469  ] |..  | **_opti
+000011f0: 6f6e 5f32 5f2a 2a20 7c20 7468 6520 7465  on_2_** | the te
+00001200: 7874 206f 6e20 7468 6520 7365 636f 6e64  xt on the second
+00001210: 2062 7574 746f 6e20 7c0d 0a20 207c 202a   button |..  | *
+00001220: 2a5f 6f70 7469 6f6e 5f33 5f2a 2a20 7c20  *_option_3_** | 
+00001230: 7468 6520 7465 7874 206f 6e20 7468 6520  the text on the 
+00001240: 6c61 7374 2062 7574 746f 6e20 7c0d 0a20  last button |.. 
+00001250: 207c 205f 6f70 7469 6f6e 735f 207c 2064   | _options_ | d
+00001260: 6972 6563 746c 7920 7061 7373 2061 206c  irectly pass a l
+00001270: 6973 7420 636f 6e74 6169 6e69 6e67 2074  ist containing t
+00001280: 6865 206f 7074 696f 6e73 2069 6e20 6f72  he options in or
+00001290: 6465 7220 7c0d 0a20 207c 205f 6275 7474  der |..  | _butt
+000012a0: 6f6e 5f63 6f6c 6f72 5f20 7c20 636f 6c6f  on_color_ | colo
+000012b0: 7220 6f66 2074 6865 2062 7574 746f 6e73  r of the buttons
+000012c0: 207c 0d0a 2020 7c20 5f74 6578 745f 636f   |..  | _text_co
+000012d0: 6c6f 725f 207c 2063 6f6c 6f72 206f 6620  lor_ | color of 
+000012e0: 7468 6520 6d65 7373 6167 652d 7465 7874  the message-text
+000012f0: 207c 0d0a 2020 7c20 5f74 6974 6c65 5f63   |..  | _title_c
+00001300: 6f6c 6f72 5f20 7c20 636f 6c6f 7220 6f66  olor_ | color of
+00001310: 2074 6865 2074 6974 6c65 2d74 6578 7420   the title-text 
+00001320: 7c0d 0a20 207c 205f 6275 7474 6f6e 5f74  |..  | _button_t
+00001330: 6578 745f 636f 6c6f 725f 207c 2063 6f6c  ext_color_ | col
+00001340: 6f72 206f 6620 7468 6520 6275 7474 6f6e  or of the button
+00001350: 2d74 6578 7420 7c0d 0a20 207c 205f 6275  -text |..  | _bu
+00001360: 7474 6f6e 5f68 6f76 6572 5f63 6f6c 6f72  tton_hover_color
+00001370: 5f20 7c20 686f 7665 7220 636f 6c6f 7220  _ | hover color 
+00001380: 6f66 2074 6865 2062 7574 746f 6e73 207c  of the buttons |
+00001390: 0d0a 2020 7c20 5f62 7574 746f 6e5f 7769  ..  | _button_wi
+000013a0: 6474 685f 207c 2077 6964 7468 206f 6620  dth_ | width of 
+000013b0: 7468 6520 6275 7474 6f6e 7320 696e 2070  the buttons in p
+000013c0: 7820 7c0d 0a20 207c 205f 6275 7474 6f6e  x |..  | _button
+000013d0: 5f68 6569 6768 745f 207c 2068 6569 6768  _height_ | heigh
+000013e0: 7420 6f66 2074 6865 2062 7574 746f 6e73  t of the buttons
+000013f0: 2069 6e20 7078 207c 0d0a 2020 7c20 5f62   in px |..  | _b
+00001400: 6f72 6465 725f 7769 6474 685f 207c 2077  order_width_ | w
+00001410: 6964 7468 206f 6620 7468 6520 626f 7264  idth of the bord
+00001420: 6572 2061 726f 756e 6420 7468 6520 6d61  er around the ma
+00001430: 696e 2066 7261 6d65 205b 4465 6661 756c  in frame [Defaul
+00001440: 7420 6973 2031 5d20 7c0d 0a20 207c 205f  t is 1] |..  | _
+00001450: 626f 7264 6572 5f63 6f6c 6f72 5f20 7c20  border_color_ | 
+00001460: 636f 6c6f 7220 6f66 2074 6865 2066 7261  color of the fra
+00001470: 6d65 2062 6f72 6465 7220 7c0d 0a20 207c  me border |..  |
+00001480: 205f 6361 6e63 656c 5f62 7574 746f 6e5f   _cancel_button_
+00001490: 207c 2064 6566 696e 6520 7468 6520 6361   | define the ca
+000014a0: 6e63 656c 2062 7574 746f 6e20 7479 7065  ncel button type
+000014b0: 3a20 2a2a 6369 7263 6c65 2c20 6372 6f73  : **circle, cros
+000014c0: 7320 6f72 204e 6f6e 652a 2a20 7c0d 0a20  s or None** |.. 
+000014d0: 207c 205f 6361 6e63 656c 5f62 7574 746f   | _cancel_butto
+000014e0: 6e5f 636f 6c6f 725f 207c 2063 6f6c 6f72  n_color_ | color
+000014f0: 206f 6620 7468 6520 2a2a 636c 6f73 652a   of the **close*
+00001500: 2a20 6275 7474 6f6e 2c20 2a2a 7365 7420  * button, **set 
+00001510: 6974 2074 6f20 2774 7261 6e73 7061 7265  it to 'transpare
+00001520: 6e74 2720 6966 2079 6f75 2077 616e 7420  nt' if you want 
+00001530: 746f 2068 6964 6520 6974 2a2a 207c 0d0a  to hide it** |..
+00001540: 2020 7c20 2a2a 5f69 636f 6e5f 2a2a 207c    | **_icon_** |
+00001550: 2069 636f 6e20 7468 6174 2077 696c 6c20   icon that will 
+00001560: 6265 2073 686f 776e 2069 6e20 7468 6520  be shown in the 
+00001570: 6d65 7373 6167 6562 6f78 205b 4465 6661  messagebox [Defa
+00001580: 756c 7420 6973 2074 6865 2027 696e 666f  ult is the 'info
+00001590: 2720 6963 6f6e 5d20 7c0d 0a20 207c 205f  ' icon] |..  | _
+000015a0: 6963 6f6e 5f73 697a 655f 207c 2064 6566  icon_size_ | def
+000015b0: 696e 6520 7468 6520 7369 7a65 206f 6620  ine the size of 
+000015c0: 7468 6520 6963 6f6e 2069 6d61 6765 206d  the icon image m
+000015d0: 616e 7561 6c6c 7920 2874 7570 6c65 2920  anually (tuple) 
+000015e0: 7c0d 0a20 207c 205f 636f 726e 6572 5f72  |..  | _corner_r
+000015f0: 6164 6975 735f 207c 2063 6f72 6e65 7220  adius_ | corner 
+00001600: 726f 756e 646e 6573 7320 6f66 2074 6865  roundness of the
+00001610: 206d 6573 7361 6765 626f 7820 7769 6e64   messagebox wind
+00001620: 6f77 205b 2a2a 6e6f 7420 6170 706c 6963  ow [**not applic
+00001630: 6162 6c65 2069 6e20 6c69 6e75 782a 2a5d  able in linux**]
+00001640: 207c 0d0a 2020 7c20 5f66 6f6e 745f 207c   |..  | _font_ |
+00001650: 2066 6f6e 7420 6f66 2074 6865 206d 6573   font of the mes
+00001660: 7361 6765 626f 7820 7465 7874 2028 7475  sagebox text (tu
+00001670: 706c 6529 207c 0d0a 2020 7c20 5f68 6561  ple) |..  | _hea
+00001680: 6465 725f 207c 2061 6464 2074 6865 206f  der_ | add the o
+00001690: 7269 6769 6e61 6c20 6865 6164 6572 2062  riginal header b
+000016a0: 6163 6b20 6966 2079 6f75 2064 6f6e 2774  ack if you don't
+000016b0: 206c 696b 6520 2a2a 6f76 6572 7269 6465   like **override
+000016c0: 7265 6469 7265 6374 2a2a 2028 626f 6f6c  redirect** (bool
+000016d0: 2920 7c0d 0a20 207c 205f 746f 706d 6f73  ) |..  | _topmos
+000016e0: 745f 207c 2064 6973 6162 6c65 2074 6865  t_ | disable the
+000016f0: 2074 6f70 6d6f 7374 2077 696e 646f 7720   topmost window 
+00001700: 6f75 7473 6964 6520 7468 6520 6170 7020  outside the app 
+00001710: 2862 6f6f 6c29 207c 0d0a 2020 7c20 2a2a  (bool) |..  | **
+00001720: 5f66 6164 655f 696e 5f64 7572 6174 696f  _fade_in_duratio
+00001730: 6e5f 2a2a 207c 2065 6e61 626c 6520 6120  n_** | enable a 
+00001740: 6661 6465 2d69 6e20 616e 6420 6661 6465  fade-in and fade
+00001750: 2d6f 7574 2061 6e69 6d61 7469 6f6e 2028  -out animation (
+00001760: 696e 742c 2064 6566 6175 6c74 2069 7320  int, default is 
+00001770: 3029 2020 7c0d 0a0d 0a3c 2f64 6976 3e0d  0)  |....</div>.
+00001780: 0a0d 0a3c 6272 3e0d 0a0d 0a3c 6832 2061  ...<br>....<h2 a
+00001790: 6c69 676e 3d22 6365 6e74 6572 223e 2049  lign="center"> I
+000017a0: 636f 6e73 203c 2f68 323e 0d0a 0d0a 3c64  cons </h2>....<d
+000017b0: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+000017c0: 223e 0d0a 0d0a 2a2a 4465 6661 756c 7420  ">....**Default 
+000017d0: 6963 6f6e 733a 2a2a 0d0a 0d0a 215b 6963  icons:**....![ic
+000017e0: 6f6e 735d 2868 7474 7073 3a2f 2f75 7365  ons](https://use
+000017f0: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
+00001800: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f38  sercontent.com/8
+00001810: 3932 3036 3430 312f 3232 3132 3538 3430  9206401/22125840
+00001820: 332d 6161 6665 6135 3735 2d38 3536 652d  3-aafea575-856e-
+00001830: 3466 3465 2d62 3361 662d 6639 3935 3738  4f4e-b3af-f99578
+00001840: 3563 3938 3739 2e70 6e67 290d 0a0d 0a28  5c9879.png)....(
+00001850: 2a54 6865 7365 2069 636f 6e73 2061 7265  *These icons are
+00001860: 2063 7265 6174 6564 2075 7369 6e67 2050   created using P
+00001870: 6169 6e74 2e4e 4554 2c20 6672 6565 2074  aint.NET, free t
+00001880: 6f20 7573 6521 2a29 0d0a 0d0a 2a2a 466f  o use!*)....**Fo
+00001890: 7220 6375 7374 6f6d 2069 6d61 6765 732c  r custom images,
+000018a0: 206a 7573 7420 7573 6520 6069 636f 6e3d   just use `icon=
+000018b0: 2269 6d61 6765 5f70 6174 682e 706e 6722  "image_path.png"
+000018c0: 602a 2a0d 0a0d 0a23 2320 5468 6174 2773  `**....## That's
+000018d0: 2061 6c6c 2c20 686f 7065 2069 7420 7769   all, hope it wi
+000018e0: 6c6c 2068 656c 7020 696e 2055 4920 6465  ll help in UI de
+000018f0: 7665 6c6f 706d 656e 7421 0d0a 0d0a 3c2f  velopment!....</
+00001900: 6469 763e 0d0a                           div>..
```

### Comparing `CTkMessagebox-2.0/LICENSE` & `CTkMessagebox-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.0/PKG-INFO` & `CTkMessagebox-2.1/CTkMessagebox.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2043 546b  : 2.1..Name: CTk
 00000020: 4d65 7373 6167 6562 6f78 0d0a 5665 7273  Messagebox..Vers
-00000030: 696f 6e3a 2032 2e30 0d0a 5375 6d6d 6172  ion: 2.0..Summar
+00000030: 696f 6e3a 2032 2e31 0d0a 5375 6d6d 6172  ion: 2.1..Summar
 00000040: 793a 2041 206d 6f64 6572 6e20 6d65 7373  y: A modern mess
 00000050: 6167 6562 6f78 2066 6f72 2063 7573 746f  agebox for custo
 00000060: 6d74 6b69 6e74 6572 0d0a 486f 6d65 2d70  mtkinter..Home-p
 00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000080: 6875 622e 636f 6d2f 416b 6173 6361 7065  hub.com/Akascape
 00000090: 2f43 546b 4d65 7373 6167 6562 6f78 0d0a  /CTkMessagebox..
 000000a0: 4175 7468 6f72 3a20 416b 6173 6820 426f  Author: Akash Bo
@@ -37,358 +37,408 @@
 00000240: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
 00000250: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
 00000260: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
 00000270: 203e 3d33 2e36 0d0a 4465 7363 7269 7074   >=3.6..Descript
 00000280: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
 00000290: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0d  : text/markdown.
 000002a0: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-000002b0: 4943 454e 5345 0d0a 0d0a 2320 4354 6b4d  ICENSE....# CTkM
-000002c0: 6573 7361 6765 626f 780d 0a2a 2a41 206d  essagebox..**A m
-000002d0: 6f64 6572 6e20 616e 6420 6675 6c6c 7920  odern and fully 
-000002e0: 6375 7374 6f6d 697a 6162 6c65 206d 6573  customizable mes
-000002f0: 7361 6765 626f 7820 666f 7220 5b63 7573  sagebox for [cus
-00000300: 746f 6d74 6b69 6e74 6572 5d28 6874 7470  tomtkinter](http
-00000310: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-00000320: 6f6d 5363 6869 6d61 6e73 6b79 2f43 7573  omSchimansky/Cus
-00000330: 746f 6d54 6b69 6e74 6572 292a 2a0d 0a0d  tomTkinter)**...
-00000340: 0a23 2323 2046 6561 7475 7265 733a 0d0a  .### Features:..
-00000350: 2d20 4375 7374 6f6d 697a 6520 616c 6c20  - Customize all 
-00000360: 656c 656d 656e 7473 2069 6e73 6964 6520  elements inside 
-00000370: 7468 6520 6d65 7373 6167 6562 6f78 0d0a  the messagebox..
-00000380: 2d20 4164 6420 6375 7374 6f6d 2069 636f  - Add custom ico
-00000390: 6e73 206f 7220 696d 6167 6573 0d0a 2d20  ns or images..- 
-000003a0: 4164 6420 6d75 6c74 6970 6c65 206f 7074  Add multiple opt
-000003b0: 696f 6e73 2061 6363 6f72 6469 6e67 2074  ions according t
-000003c0: 6f20 796f 7572 2077 6973 680d 0a2d 204e  o your wish..- N
-000003d0: 6f20 7567 6c79 206c 6f6f 6b69 6e67 2068  o ugly looking h
-000003e0: 6561 6465 7220 6f72 2062 6f72 6465 7273  eader or borders
-000003f0: 0d0a 2d20 436f 6d65 7320 7769 7468 202a  ..- Comes with *
-00000400: 2a35 2064 6566 6175 6c74 2069 636f 6e73  *5 default icons
-00000410: 2a2a 0d0a 2d20 5370 6177 6e73 2061 7420  **..- Spawns at 
-00000420: 6365 6e74 6572 206f 6620 7468 6520 7363  center of the sc
-00000430: 7265 656e 2f61 7070 0d0a 2d20 4472 6167  reen/app..- Drag
-00000440: 6761 626c 6520 7769 6e64 6f77 0d0a 2d20  gable window..- 
-00000450: 4661 6465 2d69 6e2f 4661 6465 2d6f 7574  Fade-in/Fade-out
-00000460: 2077 696e 646f 7720 6566 6665 6374 0d0a   window effect..
-00000470: 0d0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-00000480: 6e0d 0a60 6060 0d0a 7069 7020 696e 7374  n..```..pip inst
-00000490: 616c 6c20 4354 6b4d 6573 7361 6765 626f  all CTkMessagebo
-000004a0: 780d 0a60 6060 0d0a 0d0a 5b3c 696d 6720  x..```....[<img 
-000004b0: 616c 743d 2247 6974 4875 6220 7265 706f  alt="GitHub repo
-000004c0: 2073 697a 6522 2073 7263 3d22 6874 7470   size" src="http
-000004d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000004e0: 696f 2f67 6974 6875 622f 7265 706f 2d73  io/github/repo-s
-000004f0: 697a 652f 416b 6173 6361 7065 2f43 546b  ize/Akascape/CTk
-00000500: 4d65 7373 6167 6562 6f78 3f26 636f 6c6f  Messagebox?&colo
-00000510: 723d 6772 6565 6e26 6c61 6265 6c3d 536f  r=green&label=So
-00000520: 7572 6365 2532 3043 6f64 6526 6c6f 676f  urce%20Code&logo
-00000530: 3d50 7974 686f 6e26 6c6f 676f 436f 6c6f  =Python&logoColo
-00000540: 723d 7965 6c6c 6f77 2673 7479 6c65 3d66  r=yellow&style=f
-00000550: 6f72 2d74 6865 2d62 6164 6765 2220 2077  or-the-badge"  w
-00000560: 6964 7468 3d22 3330 3022 3e5d 2868 7474  idth="300">](htt
-00000570: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000580: 416b 6173 6361 7065 2f43 546b 4d65 7373  Akascape/CTkMess
-00000590: 6167 6562 6f78 2f61 7263 6869 7665 2f72  agebox/archive/r
-000005a0: 6566 732f 6865 6164 732f 6d61 696e 2e7a  efs/heads/main.z
-000005b0: 6970 290d 0a0d 0a5b 215b 5079 5049 5d28  ip)....[![PyPI](
-000005c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000005d0: 6c64 732e 696f 2f70 7970 692f 762f 4354  lds.io/pypi/v/CT
-000005e0: 6b4d 6573 7361 6765 626f 783f 7374 796c  kMessagebox?styl
-000005f0: 653d 666c 6174 295d 2868 7474 7073 3a2f  e=flat)](https:/
-00000600: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000610: 742f 4354 6b4d 6573 7361 6765 626f 7829  t/CTkMessagebox)
-00000620: 0d0a 5b21 5b44 6f77 6e6c 6f61 6473 5d28  ..[![Downloads](
-00000630: 6874 7470 733a 2f2f 7374 6174 6963 2e70  https://static.p
-00000640: 6570 792e 7465 6368 2f62 6164 6765 2f63  epy.tech/badge/c
-00000650: 746b 6d65 7373 6167 6562 6f78 295d 2868  tkmessagebox)](h
-00000660: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-00000670: 2f70 726f 6a65 6374 2f63 746b 6d65 7373  /project/ctkmess
-00000680: 6167 6562 6f78 290d 0a21 5b50 6c61 7466  agebox)..![Platf
-00000690: 6f72 6d5d 2868 7474 7073 3a2f 2f69 6d67  orm](https://img
-000006a0: 2e73 6869 656c 6473 2e69 6f2f 706f 7765  .shields.io/powe
-000006b0: 7273 6865 6c6c 6761 6c6c 6572 792f 702f  rshellgallery/p/
-000006c0: 5065 7374 6572 3f63 6f6c 6f72 3d62 6c75  Pester?color=blu
-000006d0: 6529 0d0a 0d0a 2323 2048 6f77 2069 7420  e)....## How it 
-000006e0: 6c6f 6f6b 733f 0d0a 215b 5363 7265 656e  looks?..![Screen
-000006f0: 7368 6f74 5d28 6874 7470 733a 2f2f 7573  shot](https://us
-00000700: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
-00000710: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000720: 3839 3230 3634 3031 2f32 3231 3235 3835  89206401/2212585
-00000730: 3933 2d37 3530 3538 3837 382d 6235 3938  93-75058878-b598
-00000740: 2d34 3063 332d 3832 3861 2d31 6434 3461  -40c3-828a-1d44a
-00000750: 3663 6566 6237 332e 6a70 6729 0d0a 0d0a  6cefb73.jpg)....
-00000760: 2323 2045 7861 6d70 6c65 0d0a 6060 6070  ## Example..```p
-00000770: 7974 686f 6e0d 0a66 726f 6d20 4354 6b4d  ython..from CTkM
-00000780: 6573 7361 6765 626f 7820 696d 706f 7274  essagebox import
-00000790: 2043 546b 4d65 7373 6167 6562 6f78 0d0a   CTkMessagebox..
-000007a0: 696d 706f 7274 2063 7573 746f 6d74 6b69  import customtki
-000007b0: 6e74 6572 0d0a 0d0a 6465 6620 7368 6f77  nter....def show
-000007c0: 5f69 6e66 6f28 293a 0d0a 2020 2020 2320  _info():..    # 
-000007d0: 4465 6661 756c 7420 6d65 7373 6167 6562  Default messageb
-000007e0: 6f78 2066 6f72 2073 686f 7769 6e67 2073  ox for showing s
-000007f0: 6f6d 6520 696e 666f 726d 6174 696f 6e0d  ome information.
-00000800: 0a20 2020 2043 546b 4d65 7373 6167 6562  .    CTkMessageb
-00000810: 6f78 2874 6974 6c65 3d22 496e 666f 222c  ox(title="Info",
-00000820: 206d 6573 7361 6765 3d22 5468 6973 2069   message="This i
-00000830: 7320 6120 4354 6b4d 6573 7361 6765 626f  s a CTkMessagebo
-00000840: 7821 2229 0d0a 0d0a 6465 6620 7368 6f77  x!")....def show
-00000850: 5f63 6865 636b 6d61 726b 2829 3a0d 0a20  _checkmark():.. 
-00000860: 2020 2023 2053 686f 7720 736f 6d65 2070     # Show some p
-00000870: 6f73 6974 6976 6520 6d65 7373 6167 6520  ositive message 
-00000880: 7769 7468 2074 6865 2063 6865 636b 6d61  with the checkma
-00000890: 726b 2069 636f 6e0d 0a20 2020 2043 546b  rk icon..    CTk
-000008a0: 4d65 7373 6167 6562 6f78 286d 6573 7361  Messagebox(messa
-000008b0: 6765 3d22 4354 6b4d 6573 7361 6765 626f  ge="CTkMessagebo
-000008c0: 7820 6973 2073 7563 6365 7373 6675 6c6c  x is successfull
-000008d0: 7920 696e 7374 616c 6c65 642e 222c 0d0a  y installed.",..
-000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 6963 6f6e 3d22 6368 6563 6b22 2c20    icon="check", 
-00000900: 6f70 7469 6f6e 5f31 3d22 5468 616e 6b73  option_1="Thanks
-00000910: 2229 0d0a 2020 2020 0d0a 6465 6620 7368  ")..    ..def sh
-00000920: 6f77 5f65 7272 6f72 2829 3a0d 0a20 2020  ow_error():..   
-00000930: 2023 2053 686f 7720 736f 6d65 2065 7272   # Show some err
-00000940: 6f72 206d 6573 7361 6765 0d0a 2020 2020  or message..    
-00000950: 4354 6b4d 6573 7361 6765 626f 7828 7469  CTkMessagebox(ti
-00000960: 746c 653d 2245 7272 6f72 222c 206d 6573  tle="Error", mes
-00000970: 7361 6765 3d22 536f 6d65 7468 696e 6720  sage="Something 
-00000980: 7765 6e74 2077 726f 6e67 2121 2122 2c20  went wrong!!!", 
-00000990: 6963 6f6e 3d22 6361 6e63 656c 2229 0d0a  icon="cancel")..
-000009a0: 2020 2020 0d0a 6465 6620 7368 6f77 5f77      ..def show_w
-000009b0: 6172 6e69 6e67 2829 3a0d 0a20 2020 2023  arning():..    #
-000009c0: 2053 686f 7720 736f 6d65 2072 6574 7279   Show some retry
-000009d0: 2f63 616e 6365 6c20 7761 726e 696e 6773  /cancel warnings
-000009e0: 0d0a 2020 2020 6d73 6720 3d20 4354 6b4d  ..    msg = CTkM
-000009f0: 6573 7361 6765 626f 7828 7469 746c 653d  essagebox(title=
-00000a00: 2257 6172 6e69 6e67 204d 6573 7361 6765  "Warning Message
-00000a10: 2122 2c20 6d65 7373 6167 653d 2255 6e61  !", message="Una
-00000a20: 626c 6520 746f 2063 6f6e 6e65 6374 2122  ble to connect!"
-00000a30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000a40: 2020 2020 2069 636f 6e3d 2277 6172 6e69       icon="warni
-00000a50: 6e67 222c 206f 7074 696f 6e5f 313d 2243  ng", option_1="C
-00000a60: 616e 6365 6c22 2c20 6f70 7469 6f6e 5f32  ancel", option_2
-00000a70: 3d22 5265 7472 7922 290d 0a20 2020 200d  ="Retry")..    .
-00000a80: 0a20 2020 2069 6620 6d73 672e 6765 7428  .    if msg.get(
-00000a90: 293d 3d22 5265 7472 7922 3a0d 0a20 2020  )=="Retry":..   
-00000aa0: 2020 2020 2073 686f 775f 7761 726e 696e       show_warnin
-00000ab0: 6728 290d 0a20 2020 2020 2020 200d 0a64  g()..        ..d
-00000ac0: 6566 2061 736b 5f71 7565 7374 696f 6e28  ef ask_question(
-00000ad0: 293a 0d0a 2020 2020 2320 6765 7420 7965  ):..    # get ye
-00000ae0: 732f 6e6f 2061 6e73 7765 7273 0d0a 2020  s/no answers..  
-00000af0: 2020 6d73 6720 3d20 4354 6b4d 6573 7361    msg = CTkMessa
-00000b00: 6765 626f 7828 7469 746c 653d 2245 7869  gebox(title="Exi
-00000b10: 743f 222c 206d 6573 7361 6765 3d22 446f  t?", message="Do
-00000b20: 2079 6f75 2077 616e 7420 746f 2063 6c6f   you want to clo
-00000b30: 7365 2074 6865 2070 726f 6772 616d 3f22  se the program?"
-00000b40: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000b50: 2020 2020 2020 2020 2020 2069 636f 6e3d             icon=
-00000b60: 2271 7565 7374 696f 6e22 2c20 6f70 7469  "question", opti
-00000b70: 6f6e 5f31 3d22 4361 6e63 656c 222c 206f  on_1="Cancel", o
-00000b80: 7074 696f 6e5f 323d 224e 6f22 2c20 6f70  ption_2="No", op
-00000b90: 7469 6f6e 5f33 3d22 5965 7322 290d 0a20  tion_3="Yes").. 
-00000ba0: 2020 2072 6573 706f 6e73 6520 3d20 6d73     response = ms
-00000bb0: 672e 6765 7428 290d 0a20 2020 200d 0a20  g.get()..    .. 
-00000bc0: 2020 2069 6620 7265 7370 6f6e 7365 3d3d     if response==
-00000bd0: 2259 6573 223a 0d0a 2020 2020 2020 2020  "Yes":..        
-00000be0: 6170 702e 6465 7374 726f 7928 2920 2020  app.destroy()   
-00000bf0: 2020 2020 0d0a 2020 2020 656c 7365 3a0d      ..    else:.
-00000c00: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00000c10: 436c 6963 6b20 2759 6573 2720 746f 2065  Click 'Yes' to e
-00000c20: 7869 7421 2229 0d0a 2020 2020 2020 2020  xit!")..        
-00000c30: 2020 2020 2020 0d0a 6170 7020 3d20 6375        ..app = cu
-00000c40: 7374 6f6d 746b 696e 7465 722e 4354 6b28  stomtkinter.CTk(
-00000c50: 290d 0a61 7070 2e72 6f77 636f 6e66 6967  )..app.rowconfig
-00000c60: 7572 6528 2830 2c31 2c32 2c33 2c34 2c35  ure((0,1,2,3,4,5
-00000c70: 292c 2077 6569 6768 743d 3129 0d0a 6170  ), weight=1)..ap
-00000c80: 702e 636f 6c75 6d6e 636f 6e66 6967 7572  p.columnconfigur
-00000c90: 6528 302c 2077 6569 6768 743d 3129 0d0a  e(0, weight=1)..
-00000ca0: 6170 702e 6d69 6e73 697a 6528 3230 302c  app.minsize(200,
-00000cb0: 3235 3029 0d0a 0d0a 6375 7374 6f6d 746b  250)....customtk
-00000cc0: 696e 7465 722e 4354 6b4c 6162 656c 2861  inter.CTkLabel(a
-00000cd0: 7070 2c20 7465 7874 3d22 4354 6b20 4d65  pp, text="CTk Me
-00000ce0: 7373 6167 6562 6f78 2045 7861 6d70 6c65  ssagebox Example
-00000cf0: 7322 292e 6772 6964 2870 6164 783d 3230  s").grid(padx=20
-00000d00: 290d 0a63 7573 746f 6d74 6b69 6e74 6572  )..customtkinter
-00000d10: 2e43 546b 4275 7474 6f6e 2861 7070 2c20  .CTkButton(app, 
-00000d20: 7465 7874 3d22 4368 6563 6b20 4354 6b4d  text="Check CTkM
-00000d30: 6573 7361 6765 626f 7822 2c20 636f 6d6d  essagebox", comm
-00000d40: 616e 643d 7368 6f77 5f63 6865 636b 6d61  and=show_checkma
-00000d50: 726b 292e 6772 6964 2870 6164 783d 3230  rk).grid(padx=20
-00000d60: 2c20 7061 6479 3d31 302c 2073 7469 636b  , pady=10, stick
-00000d70: 793d 226e 6577 7322 290d 0a63 7573 746f  y="news")..custo
-00000d80: 6d74 6b69 6e74 6572 2e43 546b 4275 7474  mtkinter.CTkButt
-00000d90: 6f6e 2861 7070 2c20 7465 7874 3d22 5368  on(app, text="Sh
-00000da0: 6f77 2049 6e66 6f22 2c20 636f 6d6d 616e  ow Info", comman
-00000db0: 643d 7368 6f77 5f69 6e66 6f29 2e67 7269  d=show_info).gri
-00000dc0: 6428 7061 6478 3d32 302c 2070 6164 793d  d(padx=20, pady=
-00000dd0: 3130 2c20 7374 6963 6b79 3d22 6e65 7773  10, sticky="news
-00000de0: 2229 0d0a 6375 7374 6f6d 746b 696e 7465  ")..customtkinte
-00000df0: 722e 4354 6b42 7574 746f 6e28 6170 702c  r.CTkButton(app,
-00000e00: 2074 6578 743d 2253 686f 7720 4572 726f   text="Show Erro
-00000e10: 7222 2c20 636f 6d6d 616e 643d 7368 6f77  r", command=show
-00000e20: 5f65 7272 6f72 292e 6772 6964 2870 6164  _error).grid(pad
-00000e30: 783d 3230 2c20 7061 6479 3d31 302c 2073  x=20, pady=10, s
-00000e40: 7469 636b 793d 226e 6577 7322 290d 0a63  ticky="news")..c
-00000e50: 7573 746f 6d74 6b69 6e74 6572 2e43 546b  ustomtkinter.CTk
-00000e60: 4275 7474 6f6e 2861 7070 2c20 7465 7874  Button(app, text
-00000e70: 3d22 5368 6f77 2057 6172 6e69 6e67 222c  ="Show Warning",
-00000e80: 2063 6f6d 6d61 6e64 3d73 686f 775f 7761   command=show_wa
-00000e90: 726e 696e 6729 2e67 7269 6428 7061 6478  rning).grid(padx
-00000ea0: 3d32 302c 2070 6164 793d 3130 2c20 7374  =20, pady=10, st
-00000eb0: 6963 6b79 3d22 6e65 7773 2229 0d0a 6375  icky="news")..cu
-00000ec0: 7374 6f6d 746b 696e 7465 722e 4354 6b42  stomtkinter.CTkB
-00000ed0: 7574 746f 6e28 6170 702c 2074 6578 743d  utton(app, text=
-00000ee0: 2241 736b 2051 7565 7374 696f 6e22 2c20  "Ask Question", 
-00000ef0: 636f 6d6d 616e 643d 6173 6b5f 7175 6573  command=ask_ques
-00000f00: 7469 6f6e 292e 6772 6964 2870 6164 783d  tion).grid(padx=
-00000f10: 3230 2c20 7061 6479 3d28 3130 2c32 3029  20, pady=(10,20)
-00000f20: 2c20 7374 6963 6b79 3d22 6e65 7773 2229  , sticky="news")
-00000f30: 0d0a 0d0a 6170 702e 6d61 696e 6c6f 6f70  ....app.mainloop
-00000f40: 2829 0d0a 0d0a 6060 600d 0a0d 0a23 2320  ()....```....## 
-00000f50: 4f50 5449 4f4e 530d 0a20 207c 2050 6172  OPTIONS..  | Par
-00000f60: 616d 6574 6572 7320 207c 2044 6573 6372  ameters  | Descr
-00000f70: 6970 7469 6f6e 207c 0d0a 2020 7c20 2d2d  iption |..  | --
-00000f80: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
-00000f90: 2d2d 2d2d 207c 0d0a 2020 7c20 5f6d 6173  ---- |..  | _mas
-00000fa0: 7465 725f 207c 2073 6574 2070 6172 656e  ter_ | set paren
-00000fb0: 7420 7769 6e64 6f77 2028 6f70 7469 6f6e  t window (option
-00000fc0: 616c 292c 2074 6865 2062 6f78 2077 696c  al), the box wil
-00000fd0: 6c20 7370 6177 6e20 6174 2063 656e 7465  l spawn at cente
-00000fe0: 7220 6f66 2074 6865 2070 6172 656e 7420  r of the parent 
-00000ff0: 7769 6e64 6f77 207c 0d0a 2020 7c20 5f77  window |..  | _w
-00001000: 6964 7468 5f20 7c20 7769 6474 6820 6f66  idth_ | width of
-00001010: 2074 6865 2077 696e 646f 7720 696e 2070   the window in p
-00001020: 7820 286f 7074 696f 6e61 6c29 207c 0d0a  x (optional) |..
-00001030: 2020 7c20 5f68 6569 6768 745f 207c 2068    | _height_ | h
-00001040: 6569 6768 7420 6f66 2074 6865 2077 696e  eight of the win
-00001050: 646f 7720 696e 2070 7820 286f 7074 696f  dow in px (optio
-00001060: 6e61 6c29 207c 0d0a 2020 7c20 5f66 675f  nal) |..  | _fg_
-00001070: 636f 6c6f 725f 207c 2066 6f72 6772 6f75  color_ | forgrou
-00001080: 6e64 2063 6f6c 6f72 206f 6620 7468 6520  nd color of the 
-00001090: 6d65 7373 6167 6562 6f78 205b 6d69 6464  messagebox [midd
-000010a0: 6c65 2070 6f72 7469 6f6e 5d20 7c0d 0a20  le portion] |.. 
-000010b0: 207c 205f 6267 5f63 6f6c 6f72 5f20 207c   | _bg_color_  |
-000010c0: 2062 6163 6b67 726f 756e 6420 636f 6c6f   background colo
-000010d0: 7220 6f66 2074 6865 206d 6573 7361 6765  r of the message
-000010e0: 626f 7820 7c0d 0a20 207c 202a 2a5f 7469  box |..  | **_ti
-000010f0: 746c 655f 2a2a 207c 2074 6974 6c65 206f  tle_** | title o
-00001100: 6620 7468 6520 6d65 7373 6167 6562 6f78  f the messagebox
-00001110: 207c 0d0a 2020 7c20 2a2a 5f6d 6573 7361   |..  | **_messa
-00001120: 6765 5f2a 2a20 7c20 6d61 696e 206d 6573  ge_** | main mes
-00001130: 7361 6765 206f 6620 7468 6520 6d65 7373  sage of the mess
-00001140: 6167 6562 6f78 2077 6869 6368 2077 696c  agebox which wil
-00001150: 6c20 6265 2073 686f 776e 2061 7420 7468  l be shown at th
-00001160: 6520 6365 6e74 6572 207c 0d0a 2020 7c20  e center |..  | 
-00001170: 2a2a 5f6f 7074 696f 6e5f 315f 2a2a 207c  **_option_1_** |
-00001180: 2074 6865 2074 6578 7420 6f6e 2074 6865   the text on the
-00001190: 2066 6972 7374 2062 7574 746f 6e20 5b44   first button [D
-000011a0: 6566 6175 6c74 2069 7320 274f 4b27 5d20  efault is 'OK'] 
-000011b0: 7c0d 0a20 207c 202a 2a5f 6f70 7469 6f6e  |..  | **_option
-000011c0: 5f32 5f2a 2a20 7c20 7468 6520 7465 7874  _2_** | the text
-000011d0: 206f 6e20 7468 6520 7365 636f 6e64 2062   on the second b
-000011e0: 7574 746f 6e20 7c0d 0a20 207c 202a 2a5f  utton |..  | **_
-000011f0: 6f70 7469 6f6e 5f33 5f2a 2a20 7c20 7468  option_3_** | th
-00001200: 6520 7465 7874 206f 6e20 7468 6520 6c61  e text on the la
-00001210: 7374 2062 7574 746f 6e20 7c0d 0a20 207c  st button |..  |
-00001220: 205f 6f70 7469 6f6e 735f 207c 2064 6972   _options_ | dir
-00001230: 6563 746c 7920 7061 7373 2061 206c 6973  ectly pass a lis
-00001240: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
-00001250: 206f 7074 696f 6e73 2069 6e20 6f72 6465   options in orde
-00001260: 7220 7c0d 0a20 207c 205f 6275 7474 6f6e  r |..  | _button
-00001270: 5f63 6f6c 6f72 5f20 7c20 636f 6c6f 7220  _color_ | color 
-00001280: 6f66 2074 6865 2062 7574 746f 6e73 207c  of the buttons |
-00001290: 0d0a 2020 7c20 5f74 6578 745f 636f 6c6f  ..  | _text_colo
-000012a0: 725f 207c 2063 6f6c 6f72 206f 6620 7468  r_ | color of th
-000012b0: 6520 6d65 7373 6167 652d 7465 7874 207c  e message-text |
-000012c0: 0d0a 2020 7c20 5f74 6974 6c65 5f63 6f6c  ..  | _title_col
-000012d0: 6f72 5f20 7c20 636f 6c6f 7220 6f66 2074  or_ | color of t
-000012e0: 6865 2074 6974 6c65 2d74 6578 7420 7c0d  he title-text |.
-000012f0: 0a20 207c 205f 6275 7474 6f6e 5f74 6578  .  | _button_tex
-00001300: 745f 636f 6c6f 725f 207c 2063 6f6c 6f72  t_color_ | color
-00001310: 206f 6620 7468 6520 6275 7474 6f6e 2d74   of the button-t
-00001320: 6578 7420 7c0d 0a20 207c 205f 6275 7474  ext |..  | _butt
-00001330: 6f6e 5f68 6f76 6572 5f63 6f6c 6f72 5f20  on_hover_color_ 
-00001340: 7c20 686f 7665 7220 636f 6c6f 7220 6f66  | hover color of
-00001350: 2074 6865 2062 7574 746f 6e73 207c 0d0a   the buttons |..
-00001360: 2020 7c20 5f62 7574 746f 6e5f 7769 6474    | _button_widt
-00001370: 685f 207c 2077 6964 7468 206f 6620 7468  h_ | width of th
-00001380: 6520 6275 7474 6f6e 7320 696e 2070 7820  e buttons in px 
-00001390: 7c0d 0a20 207c 205f 6275 7474 6f6e 5f68  |..  | _button_h
-000013a0: 6569 6768 745f 207c 2068 6569 6768 7420  eight_ | height 
-000013b0: 6f66 2074 6865 2062 7574 746f 6e73 2069  of the buttons i
-000013c0: 6e20 7078 207c 0d0a 2020 7c20 5f62 6f72  n px |..  | _bor
-000013d0: 6465 725f 7769 6474 685f 207c 2077 6964  der_width_ | wid
-000013e0: 7468 206f 6620 7468 6520 626f 7264 6572  th of the border
-000013f0: 2061 726f 756e 6420 7468 6520 6d61 696e   around the main
-00001400: 2066 7261 6d65 205b 4465 6661 756c 7420   frame [Default 
-00001410: 6973 2031 5d20 7c0d 0a20 207c 205f 626f  is 1] |..  | _bo
-00001420: 7264 6572 5f63 6f6c 6f72 5f20 7c20 636f  rder_color_ | co
-00001430: 6c6f 7220 6f66 2074 6865 2066 7261 6d65  lor of the frame
-00001440: 2062 6f72 6465 7220 7c0d 0a20 207c 205f   border |..  | _
-00001450: 6361 6e63 656c 5f62 7574 746f 6e5f 207c  cancel_button_ |
-00001460: 2064 6566 696e 6520 7468 6520 6361 6e63   define the canc
-00001470: 656c 2062 7574 746f 6e20 7479 7065 3a20  el button type: 
-00001480: 2a2a 6369 7263 6c65 2c20 6372 6f73 7320  **circle, cross 
-00001490: 6f72 204e 6f6e 652a 2a20 7c0d 0a20 207c  or None** |..  |
-000014a0: 205f 6361 6e63 656c 5f62 7574 746f 6e5f   _cancel_button_
-000014b0: 636f 6c6f 725f 207c 2063 6f6c 6f72 206f  color_ | color o
-000014c0: 6620 7468 6520 2a2a 636c 6f73 652a 2a20  f the **close** 
-000014d0: 6275 7474 6f6e 2c20 2a2a 7365 7420 6974  button, **set it
-000014e0: 2074 6f20 2774 7261 6e73 7061 7265 6e74   to 'transparent
-000014f0: 2720 6966 2079 6f75 2077 616e 7420 746f  ' if you want to
-00001500: 2068 6964 6520 6974 2a2a 207c 0d0a 2020   hide it** |..  
-00001510: 7c20 2a2a 5f69 636f 6e5f 2a2a 207c 2069  | **_icon_** | i
-00001520: 636f 6e20 7468 6174 2077 696c 6c20 6265  con that will be
-00001530: 2073 686f 776e 2069 6e20 7468 6520 6d65   shown in the me
-00001540: 7373 6167 6562 6f78 205b 4465 6661 756c  ssagebox [Defaul
-00001550: 7420 6973 2074 6865 2027 696e 666f 2720  t is the 'info' 
-00001560: 6963 6f6e 5d20 7c0d 0a20 207c 205f 6963  icon] |..  | _ic
-00001570: 6f6e 5f73 697a 655f 207c 2064 6566 696e  on_size_ | defin
-00001580: 6520 7468 6520 7369 7a65 206f 6620 7468  e the size of th
-00001590: 6520 6963 6f6e 2069 6d61 6765 206d 616e  e icon image man
-000015a0: 7561 6c6c 7920 2874 7570 6c65 2920 7c0d  ually (tuple) |.
-000015b0: 0a20 207c 205f 636f 726e 6572 5f72 6164  .  | _corner_rad
-000015c0: 6975 735f 207c 2063 6f72 6e65 7220 726f  ius_ | corner ro
-000015d0: 756e 646e 6573 7320 6f66 2074 6865 206d  undness of the m
-000015e0: 6573 7361 6765 626f 7820 7769 6e64 6f77  essagebox window
-000015f0: 205b 2a2a 6e6f 7420 6170 706c 6963 6162   [**not applicab
-00001600: 6c65 2069 6e20 6c69 6e75 782a 2a5d 207c  le in linux**] |
-00001610: 0d0a 2020 7c20 5f66 6f6e 745f 207c 2066  ..  | _font_ | f
-00001620: 6f6e 7420 6f66 2074 6865 206d 6573 7361  ont of the messa
-00001630: 6765 626f 7820 7465 7874 2028 7475 706c  gebox text (tupl
-00001640: 6529 207c 0d0a 2020 7c20 5f68 6561 6465  e) |..  | _heade
-00001650: 725f 207c 2061 6464 2074 6865 206f 7269  r_ | add the ori
-00001660: 6769 6e61 6c20 6865 6164 6572 2062 6163  ginal header bac
-00001670: 6b20 6966 2079 6f75 2064 6f6e 2774 206c  k if you don't l
-00001680: 696b 6520 2a2a 6f76 6572 7269 6465 7265  ike **overridere
-00001690: 6469 7265 6374 2a2a 2028 626f 6f6c 2920  direct** (bool) 
-000016a0: 7c0d 0a20 207c 205f 746f 706d 6f73 745f  |..  | _topmost_
-000016b0: 207c 2064 6973 6162 6c65 2074 6865 2074   | disable the t
-000016c0: 6f70 6d6f 7374 2077 696e 646f 7720 6f75  opmost window ou
-000016d0: 7473 6964 6520 7468 6520 6170 7020 2862  tside the app (b
-000016e0: 6f6f 6c29 207c 0d0a 2020 7c20 2a2a 5f66  ool) |..  | **_f
-000016f0: 6164 655f 696e 5f64 7572 6174 696f 6e5f  ade_in_duration_
-00001700: 2a2a 207c 2065 6e61 626c 6520 6120 6661  ** | enable a fa
-00001710: 6465 2d69 6e20 616e 6420 6661 6465 2d6f  de-in and fade-o
-00001720: 7574 2061 6e69 6d61 7469 6f6e 2028 696e  ut animation (in
-00001730: 742c 2064 6566 6175 6c74 2069 7320 3029  t, default is 0)
-00001740: 2020 7c0d 0a20 200d 0a23 2323 2049 636f    |..  ..### Ico
-00001750: 6e73 0d0a 0d0a 2a2a 4465 6661 756c 7420  ns....**Default 
-00001760: 6963 6f6e 733a 2a2a 0d0a 0d0a 215b 6963  icons:**....![ic
-00001770: 6f6e 735d 2868 7474 7073 3a2f 2f75 7365  ons](https://use
-00001780: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-00001790: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f38  sercontent.com/8
-000017a0: 3932 3036 3430 312f 3232 3132 3538 3430  9206401/22125840
-000017b0: 332d 6161 6665 6135 3735 2d38 3536 652d  3-aafea575-856e-
-000017c0: 3466 3465 2d62 3361 662d 6639 3935 3738  4f4e-b3af-f99578
-000017d0: 3563 3938 3739 2e70 6e67 290d 0a0d 0a28  5c9879.png)....(
-000017e0: 2a54 6865 7365 2069 636f 6e73 2061 7265  *These icons are
-000017f0: 2063 7265 6174 6564 2075 7369 6e67 2050   created using P
-00001800: 6169 6e74 2e4e 4554 2c20 6672 6565 2074  aint.NET, free t
-00001810: 6f20 7573 6521 2a29 0d0a 0d0a 2a2a 466f  o use!*)....**Fo
-00001820: 7220 6375 7374 6f6d 2069 6d61 6765 732c  r custom images,
-00001830: 206a 7573 7420 7573 6520 6069 636f 6e3d   just use `icon=
-00001840: 2270 6174 685f 746f 5f74 6865 5f69 6d61  "path_to_the_ima
-00001850: 6765 2e70 6e67 2260 2a2a 0d0a 0d0a 2323  ge.png"`**....##
-00001860: 2054 6861 7427 7320 616c 6c2c 2068 6f70   That's all, hop
-00001870: 6520 6974 2077 696c 6c20 6865 6c70 2069  e it will help i
-00001880: 6e20 5549 2064 6576 656c 6f70 6d65 6e74  n UI development
-00001890: 210d 0a                                  !..
+000002b0: 4943 454e 5345 0d0a 0d0a 3c68 3120 616c  ICENSE....<h1 al
+000002c0: 6967 6e3d 2263 656e 7465 7222 3e43 546b  ign="center">CTk
+000002d0: 4d65 7373 6167 6562 6f78 3c2f 6831 3e0d  Messagebox</h1>.
+000002e0: 0a0d 0a3c 6833 2061 6c69 676e 3d22 6365  ...<h3 align="ce
+000002f0: 6e74 6572 223e 4120 6d6f 6465 726e 2061  nter">A modern a
+00000300: 6e64 2066 756c 6c79 2063 7573 746f 6d69  nd fully customi
+00000310: 7a61 626c 6520 6d65 7373 6167 6562 6f78  zable messagebox
+00000320: 2066 6f72 2043 7573 746f 6d54 6b69 6e74   for CustomTkint
+00000330: 6572 2c20 4120 6d75 7374 2d68 6176 6520  er, A must-have 
+00000340: 6578 7465 6e73 696f 6e20 7061 636b 213c  extension pack!<
+00000350: 2f68 333e 0d0a 0d0a 3c64 6976 2061 6c69  /h3>....<div ali
+00000360: 676e 3d22 6365 6e74 6572 223e 0d0a 2020  gn="center">..  
+00000370: 2020 0d0a 2020 3c61 2068 7265 663d 2268    ..  <a href="h
+00000380: 7474 7073 3a2f 2f63 7265 6174 6976 6563  ttps://creativec
+00000390: 6f6d 6d6f 6e73 2e6f 7267 2f70 7562 6c69  ommons.org/publi
+000003a0: 6364 6f6d 6169 6e2f 7a65 726f 2f31 2e30  cdomain/zero/1.0
+000003b0: 2f22 3e21 5b4c 6963 656e 7365 5d28 6874  /">![License](ht
+000003c0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000003d0: 732e 696f 2f62 6164 6765 2f4c 6963 656e  s.io/badge/Licen
+000003e0: 7365 2d43 4330 5f31 2e30 2d62 6c75 6529  se-CC0_1.0-blue)
+000003f0: 3c2f 613e 0d0a 2020 3c61 2068 7265 663d  </a>..  <a href=
+00000400: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000410: 636f 6d2f 416b 6173 6361 7065 2f43 546b  com/Akascape/CTk
+00000420: 4d65 7373 6167 6562 6f78 2f61 7263 6869  Messagebox/archi
+00000430: 7665 2f72 6566 732f 6865 6164 732f 6d61  ve/refs/heads/ma
+00000440: 696e 2e7a 6970 223e 215b 446f 776e 6c6f  in.zip">![Downlo
+00000450: 6164 5d28 6874 7470 733a 2f2f 696d 672e  ad](https://img.
+00000460: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000470: 2f53 6f75 7263 655f 436f 6465 2d44 6f77  /Source_Code-Dow
+00000480: 6e6c 6f61 642d 626c 7565 293c 2f61 3e0d  nload-blue)</a>.
+00000490: 0a20 205b 215b 5079 5049 5d28 6874 7470  .  [![PyPI](http
+000004a0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000004b0: 696f 2f70 7970 692f 762f 4354 6b4d 6573  io/pypi/v/CTkMes
+000004c0: 7361 6765 626f 783f 7374 796c 653d 666c  sagebox?style=fl
+000004d0: 6174 295d 2868 7474 7073 3a2f 2f70 7970  at)](https://pyp
+000004e0: 692e 6f72 672f 7072 6f6a 6563 742f 4354  i.org/project/CT
+000004f0: 6b4d 6573 7361 6765 626f 7829 0d0a 2020  kMessagebox)..  
+00000500: 5b21 5b44 6f77 6e6c 6f61 6473 5d28 6874  [![Downloads](ht
+00000510: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
+00000520: 792e 7465 6368 2f62 6164 6765 2f63 746b  y.tech/badge/ctk
+00000530: 6d65 7373 6167 6562 6f78 295d 2868 7474  messagebox)](htt
+00000540: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
+00000550: 726f 6a65 6374 2f63 746b 6d65 7373 6167  roject/ctkmessag
+00000560: 6562 6f78 290d 0a20 2021 5b50 6c61 7466  ebox)..  ![Platf
+00000570: 6f72 6d5d 2868 7474 7073 3a2f 2f69 6d67  orm](https://img
+00000580: 2e73 6869 656c 6473 2e69 6f2f 706f 7765  .shields.io/powe
+00000590: 7273 6865 6c6c 6761 6c6c 6572 792f 702f  rshellgallery/p/
+000005a0: 5065 7374 6572 3f63 6f6c 6f72 3d62 6c75  Pester?color=blu
+000005b0: 6529 0d0a 3c2f 6469 763e 0d0a 0d0a 0d0a  e)..</div>......
+000005c0: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+000005d0: 6572 223e 0d0a 0d0a 215b 3364 5d28 6874  er">....![3d](ht
+000005e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000005f0: 2f41 6b61 7363 6170 652f 4354 6b4d 6573  /Akascape/CTkMes
+00000600: 7361 6765 626f 782f 6173 7365 7473 2f38  sagebox/assets/8
+00000610: 3932 3036 3430 312f 6363 6535 3737 6663  9206401/cce577fc
+00000620: 2d36 3432 362d 3463 3039 2d39 3666 392d  -6426-4c09-96f9-
+00000630: 6564 6538 3863 6166 3737 3834 290d 0a0d  ede88caf7784)...
+00000640: 0a3c 2f64 6976 3e0d 0a0d 0a3c 6272 3e0d  .</div>....<br>.
+00000650: 0a0d 0a3c 6832 2061 6c69 676e 3d22 6365  ...<h2 align="ce
+00000660: 6e74 6572 223e 2046 6561 7475 7265 7320  nter"> Features 
+00000670: 3c2f 6832 3e0d 0a0d 0a2d 2043 7573 746f  </h2>....- Custo
+00000680: 6d69 7a65 2061 6c6c 2065 6c65 6d65 6e74  mize all element
+00000690: 7320 696e 7369 6465 2074 6865 206d 6573  s inside the mes
+000006a0: 7361 6765 626f 780d 0a2d 2041 6464 2063  sagebox..- Add c
+000006b0: 7573 746f 6d20 6963 6f6e 7320 6f72 2069  ustom icons or i
+000006c0: 6d61 6765 730d 0a2d 2041 6464 206d 756c  mages..- Add mul
+000006d0: 7469 706c 6520 6f70 7469 6f6e 7320 6163  tiple options ac
+000006e0: 636f 7264 696e 6720 746f 2079 6f75 7220  cording to your 
+000006f0: 7769 7368 0d0a 2d20 4e6f 2075 676c 7920  wish..- No ugly 
+00000700: 6c6f 6f6b 696e 6720 6865 6164 6572 206f  looking header o
+00000710: 7220 626f 7264 6572 730d 0a2d 2043 6f6d  r borders..- Com
+00000720: 6573 2077 6974 6820 2a2a 3520 6465 6661  es with **5 defa
+00000730: 756c 7420 6963 6f6e 732a 2a0d 0a2d 2053  ult icons**..- S
+00000740: 7061 776e 7320 6174 2063 656e 7465 7220  pawns at center 
+00000750: 6f66 2074 6865 2073 6372 6565 6e2f 6170  of the screen/ap
+00000760: 700d 0a2d 2044 7261 6767 6162 6c65 2077  p..- Draggable w
+00000770: 696e 646f 770d 0a2d 2046 6164 652d 696e  indow..- Fade-in
+00000780: 2f46 6164 652d 6f75 7420 7769 6e64 6f77  /Fade-out window
+00000790: 2065 6666 6563 740d 0a0d 0a3c 6272 3e0d   effect....<br>.
+000007a0: 0a0d 0a3c 6832 2061 6c69 676e 3d22 6365  ...<h2 align="ce
+000007b0: 6e74 6572 223e 2049 6e73 7461 6c6c 6174  nter"> Installat
+000007c0: 696f 6e20 3c2f 6832 3e0d 0a0d 0a3c 6469  ion </h2>....<di
+000007d0: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+000007e0: 3e0d 0a0d 0a60 6060 0d0a 7069 7020 696e  >....```..pip in
+000007f0: 7374 616c 6c20 4354 6b4d 6573 7361 6765  stall CTkMessage
+00000800: 626f 780d 0a60 6060 0d0a 0d0a 5b3c 696d  box..```....[<im
+00000810: 6720 616c 743d 2247 6974 4875 6220 7265  g alt="GitHub re
+00000820: 706f 2073 697a 6522 2073 7263 3d22 6874  po size" src="ht
+00000830: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000840: 732e 696f 2f67 6974 6875 622f 7265 706f  s.io/github/repo
+00000850: 2d73 697a 652f 416b 6173 6361 7065 2f43  -size/Akascape/C
+00000860: 546b 4d65 7373 6167 6562 6f78 3f26 636f  TkMessagebox?&co
+00000870: 6c6f 723d 6772 6565 6e26 6c61 6265 6c3d  lor=green&label=
+00000880: 536f 7572 6365 2532 3043 6f64 6526 6c6f  Source%20Code&lo
+00000890: 676f 3d50 7974 686f 6e26 6c6f 676f 436f  go=Python&logoCo
+000008a0: 6c6f 723d 7965 6c6c 6f77 2673 7479 6c65  lor=yellow&style
+000008b0: 3d66 6f72 2d74 6865 2d62 6164 6765 2220  =for-the-badge" 
+000008c0: 2077 6964 7468 3d22 3330 3022 3e5d 2868   width="300">](h
+000008d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000008e0: 6d2f 416b 6173 6361 7065 2f43 546b 4d65  m/Akascape/CTkMe
+000008f0: 7373 6167 6562 6f78 2f61 7263 6869 7665  ssagebox/archive
+00000900: 2f72 6566 732f 6865 6164 732f 6d61 696e  /refs/heads/main
+00000910: 2e7a 6970 290d 0a0d 0a0d 0a3c 2f64 6976  .zip)......</div
+00000920: 3e0d 0a0d 0a3c 6272 3e0d 0a0d 0a3c 6832  >....<br>....<h2
+00000930: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000940: 2048 6f77 2069 7420 6c6f 6f6b 733f 203c   How it looks? <
+00000950: 2f68 323e 0d0a 0d0a 3c64 6976 2061 6c69  /h2>....<div ali
+00000960: 676e 3d22 6365 6e74 6572 223e 0d0a 0d0a  gn="center">....
+00000970: 215b 5363 7265 656e 7368 6f74 5d28 6874  ![Screenshot](ht
+00000980: 7470 733a 2f2f 7573 6572 2d69 6d61 6765  tps://user-image
+00000990: 732e 6769 7468 7562 7573 6572 636f 6e74  s.githubusercont
+000009a0: 656e 742e 636f 6d2f 3839 3230 3634 3031  ent.com/89206401
+000009b0: 2f32 3231 3235 3835 3933 2d37 3530 3538  /221258593-75058
+000009c0: 3837 382d 6235 3938 2d34 3063 332d 3832  878-b598-40c3-82
+000009d0: 3861 2d31 6434 3461 3663 6566 6237 332e  8a-1d44a6cefb73.
+000009e0: 6a70 6729 0d0a 0d0a 3c2f 6469 763e 0d0a  jpg)....</div>..
+000009f0: 0d0a 3c62 723e 0d0a 0d0a 3c68 3220 616c  ..<br>....<h2 al
+00000a00: 6967 6e3d 2263 656e 7465 7222 3e20 4578  ign="center"> Ex
+00000a10: 616d 706c 6520 3c2f 6832 3e0d 0a0d 0a60  ample </h2>....`
+00000a20: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2043  ``python..from C
+00000a30: 546b 4d65 7373 6167 6562 6f78 2069 6d70  TkMessagebox imp
+00000a40: 6f72 7420 4354 6b4d 6573 7361 6765 626f  ort CTkMessagebo
+00000a50: 780d 0a69 6d70 6f72 7420 6375 7374 6f6d  x..import custom
+00000a60: 746b 696e 7465 720d 0a0d 0a64 6566 2073  tkinter....def s
+00000a70: 686f 775f 696e 666f 2829 3a0d 0a20 2020  how_info():..   
+00000a80: 2023 2044 6566 6175 6c74 206d 6573 7361   # Default messa
+00000a90: 6765 626f 7820 666f 7220 7368 6f77 696e  gebox for showin
+00000aa0: 6720 736f 6d65 2069 6e66 6f72 6d61 7469  g some informati
+00000ab0: 6f6e 0d0a 2020 2020 4354 6b4d 6573 7361  on..    CTkMessa
+00000ac0: 6765 626f 7828 7469 746c 653d 2249 6e66  gebox(title="Inf
+00000ad0: 6f22 2c20 6d65 7373 6167 653d 2254 6869  o", message="Thi
+00000ae0: 7320 6973 2061 2043 546b 4d65 7373 6167  s is a CTkMessag
+00000af0: 6562 6f78 2122 290d 0a0d 0a64 6566 2073  ebox!")....def s
+00000b00: 686f 775f 6368 6563 6b6d 6172 6b28 293a  how_checkmark():
+00000b10: 0d0a 2020 2020 2320 5368 6f77 2073 6f6d  ..    # Show som
+00000b20: 6520 706f 7369 7469 7665 206d 6573 7361  e positive messa
+00000b30: 6765 2077 6974 6820 7468 6520 6368 6563  ge with the chec
+00000b40: 6b6d 6172 6b20 6963 6f6e 0d0a 2020 2020  kmark icon..    
+00000b50: 4354 6b4d 6573 7361 6765 626f 7828 6d65  CTkMessagebox(me
+00000b60: 7373 6167 653d 2243 546b 4d65 7373 6167  ssage="CTkMessag
+00000b70: 6562 6f78 2069 7320 7375 6363 6573 7366  ebox is successf
+00000b80: 756c 6c79 2069 6e73 7461 6c6c 6564 2e22  ully installed."
+00000b90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000ba0: 2020 2020 2069 636f 6e3d 2263 6865 636b       icon="check
+00000bb0: 222c 206f 7074 696f 6e5f 313d 2254 6861  ", option_1="Tha
+00000bc0: 6e6b 7322 290d 0a20 2020 200d 0a64 6566  nks")..    ..def
+00000bd0: 2073 686f 775f 6572 726f 7228 293a 0d0a   show_error():..
+00000be0: 2020 2020 2320 5368 6f77 2073 6f6d 6520      # Show some 
+00000bf0: 6572 726f 7220 6d65 7373 6167 650d 0a20  error message.. 
+00000c00: 2020 2043 546b 4d65 7373 6167 6562 6f78     CTkMessagebox
+00000c10: 2874 6974 6c65 3d22 4572 726f 7222 2c20  (title="Error", 
+00000c20: 6d65 7373 6167 653d 2253 6f6d 6574 6869  message="Somethi
+00000c30: 6e67 2077 656e 7420 7772 6f6e 6721 2121  ng went wrong!!!
+00000c40: 222c 2069 636f 6e3d 2263 616e 6365 6c22  ", icon="cancel"
+00000c50: 290d 0a20 2020 200d 0a64 6566 2073 686f  )..    ..def sho
+00000c60: 775f 7761 726e 696e 6728 293a 0d0a 2020  w_warning():..  
+00000c70: 2020 2320 5368 6f77 2073 6f6d 6520 7265    # Show some re
+00000c80: 7472 792f 6361 6e63 656c 2077 6172 6e69  try/cancel warni
+00000c90: 6e67 730d 0a20 2020 206d 7367 203d 2043  ngs..    msg = C
+00000ca0: 546b 4d65 7373 6167 6562 6f78 2874 6974  TkMessagebox(tit
+00000cb0: 6c65 3d22 5761 726e 696e 6720 4d65 7373  le="Warning Mess
+00000cc0: 6167 6521 222c 206d 6573 7361 6765 3d22  age!", message="
+00000cd0: 556e 6162 6c65 2074 6f20 636f 6e6e 6563  Unable to connec
+00000ce0: 7421 222c 0d0a 2020 2020 2020 2020 2020  t!",..          
+00000cf0: 2020 2020 2020 2020 6963 6f6e 3d22 7761          icon="wa
+00000d00: 726e 696e 6722 2c20 6f70 7469 6f6e 5f31  rning", option_1
+00000d10: 3d22 4361 6e63 656c 222c 206f 7074 696f  ="Cancel", optio
+00000d20: 6e5f 323d 2252 6574 7279 2229 0d0a 2020  n_2="Retry")..  
+00000d30: 2020 0d0a 2020 2020 6966 206d 7367 2e67    ..    if msg.g
+00000d40: 6574 2829 3d3d 2252 6574 7279 223a 0d0a  et()=="Retry":..
+00000d50: 2020 2020 2020 2020 7368 6f77 5f77 6172          show_war
+00000d60: 6e69 6e67 2829 0d0a 2020 2020 2020 2020  ning()..        
+00000d70: 0d0a 6465 6620 6173 6b5f 7175 6573 7469  ..def ask_questi
+00000d80: 6f6e 2829 3a0d 0a20 2020 2023 2067 6574  on():..    # get
+00000d90: 2079 6573 2f6e 6f20 616e 7377 6572 730d   yes/no answers.
+00000da0: 0a20 2020 206d 7367 203d 2043 546b 4d65  .    msg = CTkMe
+00000db0: 7373 6167 6562 6f78 2874 6974 6c65 3d22  ssagebox(title="
+00000dc0: 4578 6974 3f22 2c20 6d65 7373 6167 653d  Exit?", message=
+00000dd0: 2244 6f20 796f 7520 7761 6e74 2074 6f20  "Do you want to 
+00000de0: 636c 6f73 6520 7468 6520 7072 6f67 7261  close the progra
+00000df0: 6d3f 222c 0d0a 2020 2020 2020 2020 2020  m?",..          
+00000e00: 2020 2020 2020 2020 2020 2020 2020 6963                ic
+00000e10: 6f6e 3d22 7175 6573 7469 6f6e 222c 206f  on="question", o
+00000e20: 7074 696f 6e5f 313d 2243 616e 6365 6c22  ption_1="Cancel"
+00000e30: 2c20 6f70 7469 6f6e 5f32 3d22 4e6f 222c  , option_2="No",
+00000e40: 206f 7074 696f 6e5f 333d 2259 6573 2229   option_3="Yes")
+00000e50: 0d0a 2020 2020 7265 7370 6f6e 7365 203d  ..    response =
+00000e60: 206d 7367 2e67 6574 2829 0d0a 2020 2020   msg.get()..    
+00000e70: 0d0a 2020 2020 6966 2072 6573 706f 6e73  ..    if respons
+00000e80: 653d 3d22 5965 7322 3a0d 0a20 2020 2020  e=="Yes":..     
+00000e90: 2020 2061 7070 2e64 6573 7472 6f79 2829     app.destroy()
+00000ea0: 2020 2020 2020 200d 0a20 2020 2065 6c73         ..    els
+00000eb0: 653a 0d0a 2020 2020 2020 2020 7072 696e  e:..        prin
+00000ec0: 7428 2243 6c69 636b 2027 5965 7327 2074  t("Click 'Yes' t
+00000ed0: 6f20 6578 6974 2122 290d 0a20 2020 2020  o exit!")..     
+00000ee0: 2020 2020 2020 2020 200d 0a61 7070 203d           ..app =
+00000ef0: 2063 7573 746f 6d74 6b69 6e74 6572 2e43   customtkinter.C
+00000f00: 546b 2829 0d0a 6170 702e 726f 7763 6f6e  Tk()..app.rowcon
+00000f10: 6669 6775 7265 2828 302c 312c 322c 332c  figure((0,1,2,3,
+00000f20: 342c 3529 2c20 7765 6967 6874 3d31 290d  4,5), weight=1).
+00000f30: 0a61 7070 2e63 6f6c 756d 6e63 6f6e 6669  .app.columnconfi
+00000f40: 6775 7265 2830 2c20 7765 6967 6874 3d31  gure(0, weight=1
+00000f50: 290d 0a61 7070 2e6d 696e 7369 7a65 2832  )..app.minsize(2
+00000f60: 3030 2c32 3530 290d 0a0d 0a63 7573 746f  00,250)....custo
+00000f70: 6d74 6b69 6e74 6572 2e43 546b 4c61 6265  mtkinter.CTkLabe
+00000f80: 6c28 6170 702c 2074 6578 743d 2243 546b  l(app, text="CTk
+00000f90: 204d 6573 7361 6765 626f 7820 4578 616d   Messagebox Exam
+00000fa0: 706c 6573 2229 2e67 7269 6428 7061 6478  ples").grid(padx
+00000fb0: 3d32 3029 0d0a 6375 7374 6f6d 746b 696e  =20)..customtkin
+00000fc0: 7465 722e 4354 6b42 7574 746f 6e28 6170  ter.CTkButton(ap
+00000fd0: 702c 2074 6578 743d 2243 6865 636b 2043  p, text="Check C
+00000fe0: 546b 4d65 7373 6167 6562 6f78 222c 2063  TkMessagebox", c
+00000ff0: 6f6d 6d61 6e64 3d73 686f 775f 6368 6563  ommand=show_chec
+00001000: 6b6d 6172 6b29 2e67 7269 6428 7061 6478  kmark).grid(padx
+00001010: 3d32 302c 2070 6164 793d 3130 2c20 7374  =20, pady=10, st
+00001020: 6963 6b79 3d22 6e65 7773 2229 0d0a 6375  icky="news")..cu
+00001030: 7374 6f6d 746b 696e 7465 722e 4354 6b42  stomtkinter.CTkB
+00001040: 7574 746f 6e28 6170 702c 2074 6578 743d  utton(app, text=
+00001050: 2253 686f 7720 496e 666f 222c 2063 6f6d  "Show Info", com
+00001060: 6d61 6e64 3d73 686f 775f 696e 666f 292e  mand=show_info).
+00001070: 6772 6964 2870 6164 783d 3230 2c20 7061  grid(padx=20, pa
+00001080: 6479 3d31 302c 2073 7469 636b 793d 226e  dy=10, sticky="n
+00001090: 6577 7322 290d 0a63 7573 746f 6d74 6b69  ews")..customtki
+000010a0: 6e74 6572 2e43 546b 4275 7474 6f6e 2861  nter.CTkButton(a
+000010b0: 7070 2c20 7465 7874 3d22 5368 6f77 2045  pp, text="Show E
+000010c0: 7272 6f72 222c 2063 6f6d 6d61 6e64 3d73  rror", command=s
+000010d0: 686f 775f 6572 726f 7229 2e67 7269 6428  how_error).grid(
+000010e0: 7061 6478 3d32 302c 2070 6164 793d 3130  padx=20, pady=10
+000010f0: 2c20 7374 6963 6b79 3d22 6e65 7773 2229  , sticky="news")
+00001100: 0d0a 6375 7374 6f6d 746b 696e 7465 722e  ..customtkinter.
+00001110: 4354 6b42 7574 746f 6e28 6170 702c 2074  CTkButton(app, t
+00001120: 6578 743d 2253 686f 7720 5761 726e 696e  ext="Show Warnin
+00001130: 6722 2c20 636f 6d6d 616e 643d 7368 6f77  g", command=show
+00001140: 5f77 6172 6e69 6e67 292e 6772 6964 2870  _warning).grid(p
+00001150: 6164 783d 3230 2c20 7061 6479 3d31 302c  adx=20, pady=10,
+00001160: 2073 7469 636b 793d 226e 6577 7322 290d   sticky="news").
+00001170: 0a63 7573 746f 6d74 6b69 6e74 6572 2e43  .customtkinter.C
+00001180: 546b 4275 7474 6f6e 2861 7070 2c20 7465  TkButton(app, te
+00001190: 7874 3d22 4173 6b20 5175 6573 7469 6f6e  xt="Ask Question
+000011a0: 222c 2063 6f6d 6d61 6e64 3d61 736b 5f71  ", command=ask_q
+000011b0: 7565 7374 696f 6e29 2e67 7269 6428 7061  uestion).grid(pa
+000011c0: 6478 3d32 302c 2070 6164 793d 2831 302c  dx=20, pady=(10,
+000011d0: 3230 292c 2073 7469 636b 793d 226e 6577  20), sticky="new
+000011e0: 7322 290d 0a0d 0a61 7070 2e6d 6169 6e6c  s")....app.mainl
+000011f0: 6f6f 7028 290d 0a0d 0a60 6060 0d0a 0d0a  oop()....```....
+00001200: 3c62 723e 0d0a 0d0a 3c68 3220 616c 6967  <br>....<h2 alig
+00001210: 6e3d 2263 656e 7465 7222 3e20 4f50 5449  n="center"> OPTI
+00001220: 4f4e 5320 3c2f 6832 3e0d 0a0d 0a3c 6469  ONS </h2>....<di
+00001230: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+00001240: 3e0d 0a0d 0a20 207c 2050 6172 616d 6574  >....  | Paramet
+00001250: 6572 7320 207c 2044 6573 6372 6970 7469  ers  | Descripti
+00001260: 6f6e 207c 0d0a 2020 7c20 2d2d 2d2d 2d2d  on |..  | ------
+00001270: 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d 2d2d  -- | -----------
+00001280: 207c 0d0a 2020 7c20 5f6d 6173 7465 725f   |..  | _master_
+00001290: 207c 2073 6574 2070 6172 656e 7420 7769   | set parent wi
+000012a0: 6e64 6f77 2028 6f70 7469 6f6e 616c 292c  ndow (optional),
+000012b0: 2074 6865 2062 6f78 2077 696c 6c20 7370   the box will sp
+000012c0: 6177 6e20 6174 2063 656e 7465 7220 6f66  awn at center of
+000012d0: 2074 6865 2070 6172 656e 7420 7769 6e64   the parent wind
+000012e0: 6f77 207c 0d0a 2020 7c20 5f77 6964 7468  ow |..  | _width
+000012f0: 5f20 7c20 7769 6474 6820 6f66 2074 6865  _ | width of the
+00001300: 2077 696e 646f 7720 696e 2070 7820 286f   window in px (o
+00001310: 7074 696f 6e61 6c29 207c 0d0a 2020 7c20  ptional) |..  | 
+00001320: 5f68 6569 6768 745f 207c 2068 6569 6768  _height_ | heigh
+00001330: 7420 6f66 2074 6865 2077 696e 646f 7720  t of the window 
+00001340: 696e 2070 7820 286f 7074 696f 6e61 6c29  in px (optional)
+00001350: 207c 0d0a 2020 7c20 5f66 675f 636f 6c6f   |..  | _fg_colo
+00001360: 725f 207c 2066 6f72 6772 6f75 6e64 2063  r_ | forground c
+00001370: 6f6c 6f72 206f 6620 7468 6520 6d65 7373  olor of the mess
+00001380: 6167 6562 6f78 205b 6d69 6464 6c65 2070  agebox [middle p
+00001390: 6f72 7469 6f6e 5d20 7c0d 0a20 207c 205f  ortion] |..  | _
+000013a0: 6267 5f63 6f6c 6f72 5f20 207c 2062 6163  bg_color_  | bac
+000013b0: 6b67 726f 756e 6420 636f 6c6f 7220 6f66  kground color of
+000013c0: 2074 6865 206d 6573 7361 6765 626f 7820   the messagebox 
+000013d0: 7c0d 0a20 207c 202a 2a5f 7469 746c 655f  |..  | **_title_
+000013e0: 2a2a 207c 2074 6974 6c65 206f 6620 7468  ** | title of th
+000013f0: 6520 6d65 7373 6167 6562 6f78 207c 0d0a  e messagebox |..
+00001400: 2020 7c20 2a2a 5f6d 6573 7361 6765 5f2a    | **_message_*
+00001410: 2a20 7c20 6d61 696e 206d 6573 7361 6765  * | main message
+00001420: 206f 6620 7468 6520 6d65 7373 6167 6562   of the messageb
+00001430: 6f78 2077 6869 6368 2077 696c 6c20 6265  ox which will be
+00001440: 2073 686f 776e 2061 7420 7468 6520 6365   shown at the ce
+00001450: 6e74 6572 207c 0d0a 2020 7c20 2a2a 5f6f  nter |..  | **_o
+00001460: 7074 696f 6e5f 315f 2a2a 207c 2074 6865  ption_1_** | the
+00001470: 2074 6578 7420 6f6e 2074 6865 2066 6972   text on the fir
+00001480: 7374 2062 7574 746f 6e20 5b44 6566 6175  st button [Defau
+00001490: 6c74 2069 7320 274f 4b27 5d20 7c0d 0a20  lt is 'OK'] |.. 
+000014a0: 207c 202a 2a5f 6f70 7469 6f6e 5f32 5f2a   | **_option_2_*
+000014b0: 2a20 7c20 7468 6520 7465 7874 206f 6e20  * | the text on 
+000014c0: 7468 6520 7365 636f 6e64 2062 7574 746f  the second butto
+000014d0: 6e20 7c0d 0a20 207c 202a 2a5f 6f70 7469  n |..  | **_opti
+000014e0: 6f6e 5f33 5f2a 2a20 7c20 7468 6520 7465  on_3_** | the te
+000014f0: 7874 206f 6e20 7468 6520 6c61 7374 2062  xt on the last b
+00001500: 7574 746f 6e20 7c0d 0a20 207c 205f 6f70  utton |..  | _op
+00001510: 7469 6f6e 735f 207c 2064 6972 6563 746c  tions_ | directl
+00001520: 7920 7061 7373 2061 206c 6973 7420 636f  y pass a list co
+00001530: 6e74 6169 6e69 6e67 2074 6865 206f 7074  ntaining the opt
+00001540: 696f 6e73 2069 6e20 6f72 6465 7220 7c0d  ions in order |.
+00001550: 0a20 207c 205f 6275 7474 6f6e 5f63 6f6c  .  | _button_col
+00001560: 6f72 5f20 7c20 636f 6c6f 7220 6f66 2074  or_ | color of t
+00001570: 6865 2062 7574 746f 6e73 207c 0d0a 2020  he buttons |..  
+00001580: 7c20 5f74 6578 745f 636f 6c6f 725f 207c  | _text_color_ |
+00001590: 2063 6f6c 6f72 206f 6620 7468 6520 6d65   color of the me
+000015a0: 7373 6167 652d 7465 7874 207c 0d0a 2020  ssage-text |..  
+000015b0: 7c20 5f74 6974 6c65 5f63 6f6c 6f72 5f20  | _title_color_ 
+000015c0: 7c20 636f 6c6f 7220 6f66 2074 6865 2074  | color of the t
+000015d0: 6974 6c65 2d74 6578 7420 7c0d 0a20 207c  itle-text |..  |
+000015e0: 205f 6275 7474 6f6e 5f74 6578 745f 636f   _button_text_co
+000015f0: 6c6f 725f 207c 2063 6f6c 6f72 206f 6620  lor_ | color of 
+00001600: 7468 6520 6275 7474 6f6e 2d74 6578 7420  the button-text 
+00001610: 7c0d 0a20 207c 205f 6275 7474 6f6e 5f68  |..  | _button_h
+00001620: 6f76 6572 5f63 6f6c 6f72 5f20 7c20 686f  over_color_ | ho
+00001630: 7665 7220 636f 6c6f 7220 6f66 2074 6865  ver color of the
+00001640: 2062 7574 746f 6e73 207c 0d0a 2020 7c20   buttons |..  | 
+00001650: 5f62 7574 746f 6e5f 7769 6474 685f 207c  _button_width_ |
+00001660: 2077 6964 7468 206f 6620 7468 6520 6275   width of the bu
+00001670: 7474 6f6e 7320 696e 2070 7820 7c0d 0a20  ttons in px |.. 
+00001680: 207c 205f 6275 7474 6f6e 5f68 6569 6768   | _button_heigh
+00001690: 745f 207c 2068 6569 6768 7420 6f66 2074  t_ | height of t
+000016a0: 6865 2062 7574 746f 6e73 2069 6e20 7078  he buttons in px
+000016b0: 207c 0d0a 2020 7c20 5f62 6f72 6465 725f   |..  | _border_
+000016c0: 7769 6474 685f 207c 2077 6964 7468 206f  width_ | width o
+000016d0: 6620 7468 6520 626f 7264 6572 2061 726f  f the border aro
+000016e0: 756e 6420 7468 6520 6d61 696e 2066 7261  und the main fra
+000016f0: 6d65 205b 4465 6661 756c 7420 6973 2031  me [Default is 1
+00001700: 5d20 7c0d 0a20 207c 205f 626f 7264 6572  ] |..  | _border
+00001710: 5f63 6f6c 6f72 5f20 7c20 636f 6c6f 7220  _color_ | color 
+00001720: 6f66 2074 6865 2066 7261 6d65 2062 6f72  of the frame bor
+00001730: 6465 7220 7c0d 0a20 207c 205f 6361 6e63  der |..  | _canc
+00001740: 656c 5f62 7574 746f 6e5f 207c 2064 6566  el_button_ | def
+00001750: 696e 6520 7468 6520 6361 6e63 656c 2062  ine the cancel b
+00001760: 7574 746f 6e20 7479 7065 3a20 2a2a 6369  utton type: **ci
+00001770: 7263 6c65 2c20 6372 6f73 7320 6f72 204e  rcle, cross or N
+00001780: 6f6e 652a 2a20 7c0d 0a20 207c 205f 6361  one** |..  | _ca
+00001790: 6e63 656c 5f62 7574 746f 6e5f 636f 6c6f  ncel_button_colo
+000017a0: 725f 207c 2063 6f6c 6f72 206f 6620 7468  r_ | color of th
+000017b0: 6520 2a2a 636c 6f73 652a 2a20 6275 7474  e **close** butt
+000017c0: 6f6e 2c20 2a2a 7365 7420 6974 2074 6f20  on, **set it to 
+000017d0: 2774 7261 6e73 7061 7265 6e74 2720 6966  'transparent' if
+000017e0: 2079 6f75 2077 616e 7420 746f 2068 6964   you want to hid
+000017f0: 6520 6974 2a2a 207c 0d0a 2020 7c20 2a2a  e it** |..  | **
+00001800: 5f69 636f 6e5f 2a2a 207c 2069 636f 6e20  _icon_** | icon 
+00001810: 7468 6174 2077 696c 6c20 6265 2073 686f  that will be sho
+00001820: 776e 2069 6e20 7468 6520 6d65 7373 6167  wn in the messag
+00001830: 6562 6f78 205b 4465 6661 756c 7420 6973  ebox [Default is
+00001840: 2074 6865 2027 696e 666f 2720 6963 6f6e   the 'info' icon
+00001850: 5d20 7c0d 0a20 207c 205f 6963 6f6e 5f73  ] |..  | _icon_s
+00001860: 697a 655f 207c 2064 6566 696e 6520 7468  ize_ | define th
+00001870: 6520 7369 7a65 206f 6620 7468 6520 6963  e size of the ic
+00001880: 6f6e 2069 6d61 6765 206d 616e 7561 6c6c  on image manuall
+00001890: 7920 2874 7570 6c65 2920 7c0d 0a20 207c  y (tuple) |..  |
+000018a0: 205f 636f 726e 6572 5f72 6164 6975 735f   _corner_radius_
+000018b0: 207c 2063 6f72 6e65 7220 726f 756e 646e   | corner roundn
+000018c0: 6573 7320 6f66 2074 6865 206d 6573 7361  ess of the messa
+000018d0: 6765 626f 7820 7769 6e64 6f77 205b 2a2a  gebox window [**
+000018e0: 6e6f 7420 6170 706c 6963 6162 6c65 2069  not applicable i
+000018f0: 6e20 6c69 6e75 782a 2a5d 207c 0d0a 2020  n linux**] |..  
+00001900: 7c20 5f66 6f6e 745f 207c 2066 6f6e 7420  | _font_ | font 
+00001910: 6f66 2074 6865 206d 6573 7361 6765 626f  of the messagebo
+00001920: 7820 7465 7874 2028 7475 706c 6529 207c  x text (tuple) |
+00001930: 0d0a 2020 7c20 5f68 6561 6465 725f 207c  ..  | _header_ |
+00001940: 2061 6464 2074 6865 206f 7269 6769 6e61   add the origina
+00001950: 6c20 6865 6164 6572 2062 6163 6b20 6966  l header back if
+00001960: 2079 6f75 2064 6f6e 2774 206c 696b 6520   you don't like 
+00001970: 2a2a 6f76 6572 7269 6465 7265 6469 7265  **overrideredire
+00001980: 6374 2a2a 2028 626f 6f6c 2920 7c0d 0a20  ct** (bool) |.. 
+00001990: 207c 205f 746f 706d 6f73 745f 207c 2064   | _topmost_ | d
+000019a0: 6973 6162 6c65 2074 6865 2074 6f70 6d6f  isable the topmo
+000019b0: 7374 2077 696e 646f 7720 6f75 7473 6964  st window outsid
+000019c0: 6520 7468 6520 6170 7020 2862 6f6f 6c29  e the app (bool)
+000019d0: 207c 0d0a 2020 7c20 2a2a 5f66 6164 655f   |..  | **_fade_
+000019e0: 696e 5f64 7572 6174 696f 6e5f 2a2a 207c  in_duration_** |
+000019f0: 2065 6e61 626c 6520 6120 6661 6465 2d69   enable a fade-i
+00001a00: 6e20 616e 6420 6661 6465 2d6f 7574 2061  n and fade-out a
+00001a10: 6e69 6d61 7469 6f6e 2028 696e 742c 2064  nimation (int, d
+00001a20: 6566 6175 6c74 2069 7320 3029 2020 7c0d  efault is 0)  |.
+00001a30: 0a0d 0a3c 2f64 6976 3e0d 0a0d 0a3c 6272  ...</div>....<br
+00001a40: 3e0d 0a0d 0a3c 6832 2061 6c69 676e 3d22  >....<h2 align="
+00001a50: 6365 6e74 6572 223e 2049 636f 6e73 203c  center"> Icons <
+00001a60: 2f68 323e 0d0a 0d0a 3c64 6976 2061 6c69  /h2>....<div ali
+00001a70: 676e 3d22 6365 6e74 6572 223e 0d0a 0d0a  gn="center">....
+00001a80: 2a2a 4465 6661 756c 7420 6963 6f6e 733a  **Default icons:
+00001a90: 2a2a 0d0a 0d0a 215b 6963 6f6e 735d 2868  **....![icons](h
+00001aa0: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
+00001ab0: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
+00001ac0: 7465 6e74 2e63 6f6d 2f38 3932 3036 3430  tent.com/8920640
+00001ad0: 312f 3232 3132 3538 3430 332d 6161 6665  1/221258403-aafe
+00001ae0: 6135 3735 2d38 3536 652d 3466 3465 2d62  a575-856e-4f4e-b
+00001af0: 3361 662d 6639 3935 3738 3563 3938 3739  3af-f995785c9879
+00001b00: 2e70 6e67 290d 0a0d 0a28 2a54 6865 7365  .png)....(*These
+00001b10: 2069 636f 6e73 2061 7265 2063 7265 6174   icons are creat
+00001b20: 6564 2075 7369 6e67 2050 6169 6e74 2e4e  ed using Paint.N
+00001b30: 4554 2c20 6672 6565 2074 6f20 7573 6521  ET, free to use!
+00001b40: 2a29 0d0a 0d0a 2a2a 466f 7220 6375 7374  *)....**For cust
+00001b50: 6f6d 2069 6d61 6765 732c 206a 7573 7420  om images, just 
+00001b60: 7573 6520 6069 636f 6e3d 2269 6d61 6765  use `icon="image
+00001b70: 5f70 6174 682e 706e 6722 602a 2a0d 0a0d  _path.png"`**...
+00001b80: 0a23 2320 5468 6174 2773 2061 6c6c 2c20  .## That's all, 
+00001b90: 686f 7065 2069 7420 7769 6c6c 2068 656c  hope it will hel
+00001ba0: 7020 696e 2055 4920 6465 7665 6c6f 706d  p in UI developm
+00001bb0: 656e 7421 0d0a 0d0a 3c2f 6469 763e 0d0a  ent!....</div>..
```

### Comparing `CTkMessagebox-2.0/setup.cfg` & `CTkMessagebox-2.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4d65 7373 6167 6562 6f78   = CTkMessagebox
-00000020: 0d0a 7665 7273 696f 6e20 3d20 322e 300d  ..version = 2.0.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 322e 310d  ..version = 2.1.
 00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000040: 206d 6f64 6572 6e20 6d65 7373 6167 6562   modern messageb
 00000050: 6f78 2066 6f72 2063 7573 746f 6d74 6b69  ox for customtki
 00000060: 6e74 6572 0d0a 6c6f 6e67 5f64 6573 6372  nter..long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
```

### Comparing `CTkMessagebox-2.0/setup.py` & `CTkMessagebox-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkMessagebox',
-    version = '2.0',
+    version = '2.1',
     description = "A modern messagebox for customtkinter",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkMessagebox",
```

