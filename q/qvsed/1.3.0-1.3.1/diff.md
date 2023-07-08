# Comparing `tmp/qvsed-1.3.0.tar.gz` & `tmp/qvsed-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.3.0.tar", last modified: Sat Jul  8 16:26:55 2023, max compression
+gzip compressed data, was "qvsed-1.3.1.tar", last modified: Sat Jul  8 17:31:10 2023, max compression
```

## Comparing `qvsed-1.3.0.tar` & `qvsed-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 16:26:55.305394 qvsed-1.3.0/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-07 19:12:44.000000 qvsed-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-08 16:26:55.303084 qvsed-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-07-08 16:26:32.000000 qvsed-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 16:26:55.289728 qvsed-1.3.0/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.3.0/qvsed/__init__.py
--rw-rw-rw-   0        0        0      597 2023-07-08 15:55:18.000000 qvsed-1.3.0/qvsed/config_default.py
--rw-rw-rw-   0        0        0    13654 2023-07-08 16:22:56.000000 qvsed-1.3.0/qvsed/qvsed.py
--rw-rw-rw-   0        0        0    20071 2023-07-08 15:47:30.000000 qvsed-1.3.0/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-08 16:26:55.303084 qvsed-1.3.0/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 16:26:55.000000 qvsed-1.3.0/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 16:26:55.305394 qvsed-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-08 16:25:32.000000 qvsed-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:31:10.385096 qvsed-1.3.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-07 19:12:44.000000 qvsed-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-08 17:31:10.385096 qvsed-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6068 2023-07-08 17:30:58.000000 qvsed-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 17:31:10.363725 qvsed-1.3.1/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.3.1/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      597 2023-07-08 15:55:18.000000 qvsed-1.3.1/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    13655 2023-07-08 17:28:21.000000 qvsed-1.3.1/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0    21365 2023-07-08 17:21:24.000000 qvsed-1.3.1/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-08 17:31:10.382077 qvsed-1.3.1/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-08 17:31:10.000000 qvsed-1.3.1/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 17:31:10.385096 qvsed-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-08 17:30:42.000000 qvsed-1.3.1/setup.py
```

### Comparing `qvsed-1.3.0/LICENSE.txt` & `qvsed-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.0/PKG-INFO` & `qvsed-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.0
+Version: 1.3.1
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.0/README.md` & `qvsed-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # QVSED - Qt-based Volatile Small Editor
 
-QVSED is a volatile text editor. "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded. Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata. You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
+QVSED is a volatile text editor.
+
+![QVSED screenshot, showing the help message](qvsed_screenie.png)
+
+"Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded. Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata. You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
 
 QVSED follows the philosophy of ultra-minimalism, with its heavy emphasis on just editing text and nothing more. QVSED's editing style is text-based, not file-based like basically every other editor out there. Text goes in, from a file, and then text later comes out, into another or perhaps the same file.
 
 QVSED can be used as a simple scratchpad or throwaway editor, as well as a general editing software application, since it won't prompt you if you do anything destructive, It stays out of your way on many occasions. Whether or not that's a good thing is up to you.
 
 QVSED is a PyQt5 rewrite of my older project, [ASMED (Another SMol EDitor)](https://github.com/That1M8Head/ASMED), which was written using Windows Forms, and was quite obviously only for Windows.
 
@@ -26,16 +30,14 @@
 
 ## Usage
 
 QVSED is broken up into three parts - the Action Deck, the Text Area and the Echo Area.
 
 The Action Deck contains editing commands, the Text Area is a text area, and the Echo Area is where messages will be printed.
 
-![QVSED screenshot, showing the help message](qsved_screenie.png)
-
 ## Action Deck
 
 The Action Deck, positioned on the left side of the QVSED window, containing commands to clear the Text Area, open or save a file, display this help text, toggle in and out of full screen mode or quit QVSED.
 
 The Action Deck is on the left rather than on the top like a traditional menu bar, so that the buttons can be bigger while still providing enough screen real estate for the Text Area.
 
 ### Key Prefixes
```

### Comparing `qvsed-1.3.0/qvsed/config_default.py` & `qvsed-1.3.1/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.0/qvsed/qvsed.py` & `qvsed-1.3.1/qvsed/qvsed.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 QScrollBar::add-page:vertical, QScrollBar::sub-page:vertical {{
     background: none;
 }}
         """
 
         # Apply the stylesheet to the app
         self.setStyleSheet(stylesheet)
-        
+
     def clear_text_area(self):
         """
         Clear the Text Area.
         """
         text_area = self.findChild(QPlainTextEdit, "textArea")
 
         if text_area.toPlainText() == "":
@@ -337,15 +337,15 @@
         text_area = self.findChild(QPlainTextEdit, "textArea")
 
         help_message = """QVSED - Qt-based Volatile Small Editor
 ========================================
 QVSED is a stateless, volatile text editor with a minimalist approach, focusing solely on text editing without file metadata or prompts for potentially destructive actions.
 
 This is the Text Area, where the actual editing takes place. Type anything you want into here, and edit as you please.
-Down there, below the Text Area is the Echo Area, where messages and errors will be displayed.
+Down there, at the bottom of the window, is the Echo Area, where messages and errors will be displayed.
 On the left of the QVSED window is the Action Deck, containing commands to clear the Text Area, open or save a file, display this help text, toggle in and out of full screen mode or quit QVSED.
 
 I hope you enjoy using QVSED! I enjoyed writing it, and it's a nice little venture into my first Qt project.
 
 - Arsalan Kazmi <sonicspeed848@gmail.com>, That1M8Head on GitHub"""
 
         self.echo_area_update("Help message shown in Text Area.")
```

### Comparing `qvsed-1.3.0/qvsed/qvsed.ui` & `qvsed-1.3.1/qvsed/qvsed.ui`

 * *Files 8% similar despite different names*

#### Comparing `qvsed-1.3.0/qvsed/qvsed.ui` & `qvsed-1.3.1/qvsed/qvsed.ui`

```diff
@@ -500,274 +500,290 @@
     background: none;
 }
 
 QScrollBar::add-page:vertical, QScrollBar::sub-page:vertical {
     background: none;
 }</string>
       </property>
-      <layout class="QHBoxLayout" name="horizontalLayout">
+      <layout class="QHBoxLayout" name="horizontalLayout_4">
         <property name="spacing">
-          <number>12</number>
+          <number>0</number>
         </property>
         <property name="leftMargin">
-          <number>8</number>
+          <number>0</number>
         </property>
         <property name="topMargin">
-          <number>8</number>
+          <number>0</number>
         </property>
         <property name="rightMargin">
-          <number>8</number>
+          <number>0</number>
         </property>
         <property name="bottomMargin">
-          <number>8</number>
+          <number>0</number>
         </property>
         <item>
-          <layout class="QVBoxLayout" name="actionDeck">
+          <layout class="QVBoxLayout" name="verticalLayout_3">
             <property name="spacing">
-              <number>4</number>
+              <number>8</number>
             </property>
-            <item>
-              <widget class="QPushButton" name="clearButton">
-                <property name="minimumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="maximumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="font">
-                  <font>
-                    <family>monospace</family>
-                    <pointsize>11</pointsize>
-                  </font>
-                </property>
-                <property name="styleSheet">
-                  <string notr="true"/>
-                </property>
-                <property name="text">
-                  <string>Clear Text &lt;C-n&gt;</string>
-                </property>
-                <property name="flat">
-                  <bool>false</bool>
-                </property>
-              </widget>
-            </item>
-            <item>
-              <widget class="QPushButton" name="saveButton">
-                <property name="minimumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="maximumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="font">
-                  <font>
-                    <family>monospace</family>
-                    <pointsize>11</pointsize>
-                  </font>
-                </property>
-                <property name="styleSheet">
-                  <string notr="true"/>
-                </property>
-                <property name="text">
-                  <string>Save File &lt;C-s&gt;</string>
-                </property>
-                <property name="flat">
-                  <bool>false</bool>
-                </property>
-              </widget>
-            </item>
-            <item>
-              <widget class="QPushButton" name="openButton">
-                <property name="minimumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="maximumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="font">
-                  <font>
-                    <family>monospace</family>
-                    <pointsize>11</pointsize>
-                  </font>
-                </property>
-                <property name="styleSheet">
-                  <string notr="true"/>
-                </property>
-                <property name="text">
-                  <string>Open File &lt;C-f&gt;</string>
-                </property>
-                <property name="flat">
-                  <bool>false</bool>
-                </property>
-              </widget>
-            </item>
-            <item>
-              <widget class="QPushButton" name="fullscreenButton">
-                <property name="minimumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="maximumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="font">
-                  <font>
-                    <family>monospace</family>
-                    <pointsize>11</pointsize>
-                  </font>
-                </property>
-                <property name="styleSheet">
-                  <string notr="true"/>
-                </property>
-                <property name="text">
-                  <string>Full Screen &lt;A-f&gt;</string>
-                </property>
-                <property name="flat">
-                  <bool>false</bool>
-                </property>
-              </widget>
-            </item>
-            <item>
-              <spacer name="verticalSpacer">
-                <property name="orientation">
-                  <enum>Qt::Vertical</enum>
-                </property>
-                <property name="sizeHint" stdset="0">
-                  <size>
-                    <width>20</width>
-                    <height>40</height>
-                  </size>
-                </property>
-              </spacer>
-            </item>
-            <item>
-              <widget class="QPushButton" name="helpButton">
-                <property name="minimumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="maximumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="font">
-                  <font>
-                    <family>monospace</family>
-                    <pointsize>11</pointsize>
-                  </font>
-                </property>
-                <property name="styleSheet">
-                  <string notr="true"/>
-                </property>
-                <property name="text">
-                  <string>Get Help &lt;C-h&gt;</string>
-                </property>
-                <property name="flat">
-                  <bool>false</bool>
-                </property>
-              </widget>
-            </item>
-            <item>
-              <widget class="QPushButton" name="quitButton">
-                <property name="minimumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="maximumSize">
-                  <size>
-                    <width>161</width>
-                    <height>51</height>
-                  </size>
-                </property>
-                <property name="font">
-                  <font>
-                    <family>monospace</family>
-                    <pointsize>11</pointsize>
-                  </font>
-                </property>
-                <property name="styleSheet">
-                  <string notr="true"/>
-                </property>
-                <property name="text">
-                  <string>Quit QVSED &lt;A-q&gt;</string>
-                </property>
-                <property name="flat">
-                  <bool>false</bool>
-                </property>
-              </widget>
-            </item>
-          </layout>
-        </item>
-        <item>
-          <layout class="QVBoxLayout" name="textAndEchoAreas">
-            <property name="spacing">
-              <number>4</number>
+            <property name="leftMargin">
+              <number>8</number>
+            </property>
+            <property name="topMargin">
+              <number>8</number>
+            </property>
+            <property name="rightMargin">
+              <number>8</number>
+            </property>
+            <property name="bottomMargin">
+              <number>8</number>
             </property>
             <item>
-              <widget class="QPlainTextEdit" name="textArea">
-                <property name="font">
-                  <font>
-                    <family>monospace</family>
-                    <pointsize>11</pointsize>
-                  </font>
-                </property>
-                <property name="styleSheet">
-                  <string notr="true">border: 2px;
+              <layout class="QHBoxLayout" name="horizontalLayout_3">
+                <item>
+                  <layout class="QVBoxLayout" name="verticalLayout_2">
+                    <item>
+                      <widget class="QPushButton" name="clearButton">
+                        <property name="minimumSize">
+                          <size>
+                            <width>175</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>161</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="font">
+                          <font>
+                            <family>monospace</family>
+                            <pointsize>11</pointsize>
+                          </font>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true"/>
+                        </property>
+                        <property name="text">
+                          <string>Clear Text &lt;C-n&gt;</string>
+                        </property>
+                        <property name="flat">
+                          <bool>false</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QPushButton" name="saveButton">
+                        <property name="minimumSize">
+                          <size>
+                            <width>175</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>161</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="font">
+                          <font>
+                            <family>monospace</family>
+                            <pointsize>11</pointsize>
+                          </font>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true"/>
+                        </property>
+                        <property name="text">
+                          <string>Save File &lt;C-s&gt;</string>
+                        </property>
+                        <property name="flat">
+                          <bool>false</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QPushButton" name="openButton">
+                        <property name="minimumSize">
+                          <size>
+                            <width>175</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>161</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="font">
+                          <font>
+                            <family>monospace</family>
+                            <pointsize>11</pointsize>
+                          </font>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true"/>
+                        </property>
+                        <property name="text">
+                          <string>Open File &lt;C-f&gt;</string>
+                        </property>
+                        <property name="flat">
+                          <bool>false</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QPushButton" name="fullscreenButton">
+                        <property name="minimumSize">
+                          <size>
+                            <width>175</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>161</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="font">
+                          <font>
+                            <family>monospace</family>
+                            <pointsize>11</pointsize>
+                          </font>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true"/>
+                        </property>
+                        <property name="text">
+                          <string>Full Screen &lt;A-f&gt;</string>
+                        </property>
+                        <property name="flat">
+                          <bool>false</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <spacer name="verticalSpacer">
+                        <property name="orientation">
+                          <enum>Qt::Vertical</enum>
+                        </property>
+                        <property name="sizeHint" stdset="0">
+                          <size>
+                            <width>20</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                      </spacer>
+                    </item>
+                    <item>
+                      <widget class="QPushButton" name="helpButton">
+                        <property name="minimumSize">
+                          <size>
+                            <width>175</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>161</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="font">
+                          <font>
+                            <family>monospace</family>
+                            <pointsize>11</pointsize>
+                          </font>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true"/>
+                        </property>
+                        <property name="text">
+                          <string>Get Help &lt;C-h&gt;</string>
+                        </property>
+                        <property name="flat">
+                          <bool>false</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QPushButton" name="quitButton">
+                        <property name="minimumSize">
+                          <size>
+                            <width>175</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="maximumSize">
+                          <size>
+                            <width>161</width>
+                            <height>40</height>
+                          </size>
+                        </property>
+                        <property name="font">
+                          <font>
+                            <family>monospace</family>
+                            <pointsize>11</pointsize>
+                          </font>
+                        </property>
+                        <property name="styleSheet">
+                          <string notr="true"/>
+                        </property>
+                        <property name="text">
+                          <string>Quit QVSED &lt;A-q&gt;</string>
+                        </property>
+                        <property name="flat">
+                          <bool>false</bool>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                </item>
+                <item>
+                  <widget class="QPlainTextEdit" name="textArea">
+                    <property name="font">
+                      <font>
+                        <family>monospace</family>
+                        <pointsize>11</pointsize>
+                      </font>
+                    </property>
+                    <property name="styleSheet">
+                      <string notr="true">border: 2px;
 background: #31353f;
 padding: 5px;
 
 QPlainTextEdit {
     background-color: #f2f2f2;
 }</string>
-                </property>
-              </widget>
+                    </property>
+                  </widget>
+                </item>
+              </layout>
             </item>
             <item>
               <widget class="QLineEdit" name="echoArea">
                 <property name="font">
                   <font>
                     <family>monospace</family>
                     <pointsize>11</pointsize>
                   </font>
                 </property>
                 <property name="styleSheet">
-                  <string notr="true">border: 2px; background: #31353f; padding: 2px 6px;</string>
+                  <string notr="true">border: 2px; background: #31353f; padding: 6px;</string>
                 </property>
                 <property name="text">
                   <string>Welcome to QVSED! This is the Echo Area.</string>
                 </property>
+                <property name="cursorPosition">
+                  <number>0</number>
+                </property>
                 <property name="readOnly">
                   <bool>true</bool>
                 </property>
               </widget>
             </item>
           </layout>
         </item>
```

### Comparing `qvsed-1.3.0/qvsed.egg-info/PKG-INFO` & `qvsed-1.3.1/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.0
+Version: 1.3.1
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.0/setup.py` & `qvsed-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.3.0',
+    version='1.3.1',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

