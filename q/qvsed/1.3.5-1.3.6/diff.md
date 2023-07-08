# Comparing `tmp/qvsed-1.3.5.tar.gz` & `tmp/qvsed-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.3.5.tar", last modified: Sat Jul  8 21:15:15 2023, max compression
+gzip compressed data, was "qvsed-1.3.6.tar", last modified: Sat Jul  8 21:35:11 2023, max compression
```

## Comparing `qvsed-1.3.5.tar` & `qvsed-1.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 21:15:15.680575 qvsed-1.3.5/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-08 21:15:15.679403 qvsed-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     6070 2023-07-08 17:32:53.000000 qvsed-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 21:15:15.669752 qvsed-1.3.5/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.3.5/qvsed/__init__.py
--rw-rw-rw-   0        0        0      383 2023-07-08 21:13:12.000000 qvsed-1.3.5/qvsed/config_default.py
--rw-rw-rw-   0        0        0    14233 2023-07-08 21:14:48.000000 qvsed-1.3.5/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     9193 2023-07-08 21:06:50.000000 qvsed-1.3.5/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-08 21:15:15.678395 qvsed-1.3.5/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 21:15:15.000000 qvsed-1.3.5/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 21:15:15.680575 qvsed-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-08 21:12:36.000000 qvsed-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 21:35:11.204442 qvsed-1.3.6/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-08 21:35:11.203445 qvsed-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6070 2023-07-08 17:32:53.000000 qvsed-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 21:35:11.188373 qvsed-1.3.6/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.3.6/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-07-08 21:13:12.000000 qvsed-1.3.6/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    14366 2023-07-08 21:34:38.000000 qvsed-1.3.6/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-08 21:34:43.000000 qvsed-1.3.6/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-08 21:35:11.202435 qvsed-1.3.6/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 21:35:11.000000 qvsed-1.3.6/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 21:35:11.204442 qvsed-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-08 21:35:03.000000 qvsed-1.3.6/setup.py
```

### Comparing `qvsed-1.3.5/LICENSE.txt` & `qvsed-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.5/PKG-INFO` & `qvsed-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.5
+Version: 1.3.6
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.5/README.md` & `qvsed-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.5/qvsed/qvsed.py` & `qvsed-1.3.6/qvsed/qvsed.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,31 +64,42 @@
             self.load_from_file(sys.argv[1])
 
     def apply_style_sheet(self, text_color, background_color, button_color, button_focus_color):
         """
         Generate and apply a style sheet based on the config.py file.
         """
 
+        print(text_color)
+
         stylesheet = f"""
+QMainWindow {{
+    color: {text_color};
+    background: {background_color};
+}}
+
 QPlainTextEdit, QLineEdit {{
+    color: {text_color};
     background: {button_focus_color};
     border: 2px solid {button_color};
 }}
 
 QPushButton {{
+    color: {text_color};
     border: 2px solid {button_focus_color};
     background: {button_color};
     padding: 2px;
 }}
 
 QPushButton:hover {{
+    color: {text_color};
     background: {button_focus_color};
 }}
 
 QPushButton:pressed {{
+    color: {text_color};
     background: {background_color};
 }}
 
 QScrollBar:vertical {{
     background-color: {button_focus_color};
     width: 16px;
     margin: 16px 0 16px 0;
@@ -106,19 +117,14 @@
 QScrollBar::add-line:vertical, QScrollBar::sub-line:vertical {{
     background: none;
 }}
 
 QScrollBar::add-page:vertical, QScrollBar::sub-page:vertical {{
     background: none;
 }}
-
-QMainWindow {{
-    color: {text_color};
-    background: {background_color};
-}}
         """
 
         # Apply the stylesheet to the app
         self.setStyleSheet(stylesheet)
 
     def check_if_file_parameter(self):
         """
```

### Comparing `qvsed-1.3.5/qvsed/qvsed.ui` & `qvsed-1.3.6/qvsed/qvsed.ui`

 * *Files 12% similar despite different names*

#### Comparing `qvsed-1.3.5/qvsed/qvsed.ui` & `qvsed-1.3.6/qvsed/qvsed.ui`

```diff
@@ -15,21 +15,15 @@
       <font>
         <family>monospace</family>
       </font>
     </property>
     <property name="windowTitle">
       <string>QVSED</string>
     </property>
-    <property name="styleSheet">
-      <string notr="true"/>
-    </property>
     <widget class="QWidget" name="centralwidget">
-      <property name="styleSheet">
-        <string notr="true"/>
-      </property>
       <layout class="QHBoxLayout" name="horizontalLayout_4">
         <property name="spacing">
           <number>0</number>
         </property>
         <property name="leftMargin">
           <number>0</number>
         </property>
@@ -79,17 +73,14 @@
                         </property>
                         <property name="font">
                           <font>
                             <family>monospace</family>
                             <pointsize>11</pointsize>
                           </font>
                         </property>
-                        <property name="styleSheet">
-                          <string notr="true"/>
-                        </property>
                         <property name="text">
                           <string>Clear Text &lt;C-n&gt;</string>
                         </property>
                         <property name="flat">
                           <bool>false</bool>
                         </property>
                       </widget>
@@ -106,21 +97,17 @@
                           <size>
                             <width>161</width>
                             <height>40</height>
                           </size>
                         </property>
                         <property name="font">
                           <font>
-                            <family>monospace</family>
                             <pointsize>11</pointsize>
                           </font>
                         </property>
-                        <property name="styleSheet">
-                          <string notr="true"/>
-                        </property>
                         <property name="text">
                           <string>Save File &lt;C-s&gt;</string>
                         </property>
                         <property name="flat">
                           <bool>false</bool>
                         </property>
                       </widget>
@@ -137,21 +124,17 @@
                           <size>
                             <width>161</width>
                             <height>40</height>
                           </size>
                         </property>
                         <property name="font">
                           <font>
-                            <family>monospace</family>
                             <pointsize>11</pointsize>
                           </font>
                         </property>
-                        <property name="styleSheet">
-                          <string notr="true"/>
-                        </property>
                         <property name="text">
                           <string>Open File &lt;C-f&gt;</string>
                         </property>
                         <property name="flat">
                           <bool>false</bool>
                         </property>
                       </widget>
@@ -168,21 +151,17 @@
                           <size>
                             <width>161</width>
                             <height>40</height>
                           </size>
                         </property>
                         <property name="font">
                           <font>
-                            <family>monospace</family>
                             <pointsize>11</pointsize>
                           </font>
                         </property>
-                        <property name="styleSheet">
-                          <string notr="true"/>
-                        </property>
                         <property name="text">
                           <string>Full Screen &lt;A-f&gt;</string>
                         </property>
                         <property name="flat">
                           <bool>false</bool>
                         </property>
                       </widget>
@@ -212,21 +191,17 @@
                           <size>
                             <width>161</width>
                             <height>40</height>
                           </size>
                         </property>
                         <property name="font">
                           <font>
-                            <family>monospace</family>
                             <pointsize>11</pointsize>
                           </font>
                         </property>
-                        <property name="styleSheet">
-                          <string notr="true"/>
-                        </property>
                         <property name="text">
                           <string>Get Help &lt;C-h&gt;</string>
                         </property>
                         <property name="flat">
                           <bool>false</bool>
                         </property>
                       </widget>
@@ -243,57 +218,45 @@
                           <size>
                             <width>161</width>
                             <height>40</height>
                           </size>
                         </property>
                         <property name="font">
                           <font>
-                            <family>monospace</family>
                             <pointsize>11</pointsize>
                           </font>
                         </property>
-                        <property name="styleSheet">
-                          <string notr="true"/>
-                        </property>
                         <property name="text">
                           <string>Quit QVSED &lt;A-q&gt;</string>
                         </property>
                         <property name="flat">
                           <bool>false</bool>
                         </property>
                       </widget>
                     </item>
                   </layout>
                 </item>
                 <item>
                   <widget class="QPlainTextEdit" name="textArea">
                     <property name="font">
                       <font>
-                        <family>monospace</family>
                         <pointsize>11</pointsize>
                       </font>
                     </property>
-                    <property name="styleSheet">
-                      <string notr="true"/>
-                    </property>
                   </widget>
                 </item>
               </layout>
             </item>
             <item>
               <widget class="QLineEdit" name="echoArea">
                 <property name="font">
                   <font>
-                    <family>monospace</family>
                     <pointsize>11</pointsize>
                   </font>
                 </property>
-                <property name="styleSheet">
-                  <string notr="true"/>
-                </property>
                 <property name="text">
                   <string>Welcome to QVSED!</string>
                 </property>
                 <property name="cursorPosition">
                   <number>0</number>
                 </property>
                 <property name="readOnly">
```

### Comparing `qvsed-1.3.5/qvsed.egg-info/PKG-INFO` & `qvsed-1.3.6/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.5
+Version: 1.3.6
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.5/setup.py` & `qvsed-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.3.5',
+    version='1.3.6',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

