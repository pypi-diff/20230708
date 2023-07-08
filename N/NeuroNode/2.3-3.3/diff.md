# Comparing `tmp/NeuroNode-2.3.tar.gz` & `tmp/NeuroNode-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuroNode-2.3.tar", last modified: Sat Jul  8 08:18:08 2023, max compression
+gzip compressed data, was "NeuroNode-3.3.tar", last modified: Sat Jul  8 13:07:25 2023, max compression
```

## Comparing `NeuroNode-2.3.tar` & `NeuroNode-3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 08:18:08.594444 NeuroNode-2.3/
--rw-rw-rw-   0        0        0     1052 2023-02-05 10:37:40.000000 NeuroNode-2.3/LICENSE.text
--rw-rw-rw-   0        0        0      748 2023-07-08 08:18:08.593407 NeuroNode-2.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-05 07:37:25.000000 NeuroNode-2.3/README.md
--rw-rw-rw-   0        0        0      877 2023-07-08 07:11:02.000000 NeuroNode-2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 08:18:08.594444 NeuroNode-2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-08 08:18:08.507960 NeuroNode-2.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 08:18:08.579276 NeuroNode-2.3/src/NeuroNode.egg-info/
--rw-rw-rw-   0        0        0      748 2023-07-08 08:18:08.000000 NeuroNode-2.3/src/NeuroNode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-08 08:18:08.000000 NeuroNode-2.3/src/NeuroNode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 08:18:08.000000 NeuroNode-2.3/src/NeuroNode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-08 08:18:08.000000 NeuroNode-2.3/src/NeuroNode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 08:18:08.590342 NeuroNode-2.3/src/neuronode/
--rw-rw-rw-   0        0        0        0 2023-02-05 09:46:02.000000 NeuroNode-2.3/src/neuronode/Debug.py
--rw-rw-rw-   0        0        0     7242 2023-07-08 08:17:11.000000 NeuroNode-2.3/src/neuronode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:07:25.039305 NeuroNode-3.3/
+-rw-rw-rw-   0        0        0     1052 2023-02-05 10:37:40.000000 NeuroNode-3.3/LICENSE.text
+-rw-rw-rw-   0        0        0      748 2023-07-08 13:07:25.038001 NeuroNode-3.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-05 07:37:25.000000 NeuroNode-3.3/README.md
+-rw-rw-rw-   0        0        0      877 2023-07-08 12:47:53.000000 NeuroNode-3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:07:25.040308 NeuroNode-3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 13:07:24.960029 NeuroNode-3.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 13:07:25.030420 NeuroNode-3.3/src/NeuroNode.egg-info/
+-rw-rw-rw-   0        0        0      748 2023-07-08 13:07:24.000000 NeuroNode-3.3/src/NeuroNode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-08 13:07:24.000000 NeuroNode-3.3/src/NeuroNode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:07:24.000000 NeuroNode-3.3/src/NeuroNode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 13:07:24.000000 NeuroNode-3.3/src/NeuroNode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 13:07:25.034782 NeuroNode-3.3/src/neuronode/
+-rw-rw-rw-   0        0        0        0 2023-02-05 09:46:02.000000 NeuroNode-3.3/src/neuronode/Debug.py
+-rw-rw-rw-   0        0        0     7237 2023-07-08 13:06:29.000000 NeuroNode-3.3/src/neuronode/__init__.py
```

### Comparing `NeuroNode-2.3/LICENSE.text` & `NeuroNode-3.3/LICENSE.text`

 * *Files identical despite different names*

### Comparing `NeuroNode-2.3/PKG-INFO` & `NeuroNode-3.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroNode
-Version: 2.3
+Version: 3.3
 Summary: The Neuro Node is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences. Utilizing a vast neural network comprising more than 1 trillion parameters, the Neuro Node has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 Author-email: Jay Singh <jaysinghdulrasar@gmail.com>
 Project-URL: WebApp, https://neuro-node.web.app
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `NeuroNode-2.3/pyproject.toml` & `NeuroNode-3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NeuroNode"
-version = "2.3"
+version = "3.3"
 authors = [
   { name="Jay Singh", email="jaysinghdulrasar@gmail.com" },
 ]
 description = '''The Neuro Node is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences. Utilizing a vast neural network comprising more than 1 trillion parameters, the Neuro Node has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 WebSite : https://neuro-node.web.app'''
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `NeuroNode-2.3/src/NeuroNode.egg-info/PKG-INFO` & `NeuroNode-3.3/src/NeuroNode.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroNode
-Version: 2.3
+Version: 3.3
 Summary: The Neuro Node is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences. Utilizing a vast neural network comprising more than 1 trillion parameters, the Neuro Node has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 Author-email: Jay Singh <jaysinghdulrasar@gmail.com>
 Project-URL: WebApp, https://neuro-node.web.app
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `NeuroNode-2.3/src/neuronode/__init__.py` & `NeuroNode-3.3/src/neuronode/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,27 @@
     def DownloadData(self,urls):
         for i,url in enumerate(urls):
 
             r = requests.get(url, allow_redirects=True)
             open('Video'+str(i+1)+'.mp4', 'wb').write(r.content)
 
     def PrepareData(self):
-        if os.path.exists(self.directory + ".\\Scenes"):
-            shutil.rmtree(self.directory + ".\\Scenes")
-        os.mkdir(self.directory + ".\\Scenes")
+        if os.path.exists(self.directory + "/Scenes"):
+            shutil.rmtree(self.directory + "/Scenes")
+        os.mkdir(self.directory + "/Scenes")
 
         video_files = [f for f in os.listdir(self.directory) if f.endswith(".mp4") or f.endswith(".mkv") or f.endswith(".avi") or f.endswith(".mov")or f.endswith(".webm")]
 
         for video_file in video_files:
             video_path = os.path.join(self.directory, video_file)
             scene_list = detect(video_path, ContentDetector())
-            os.chdir(self.directory + "\\Scenes")
+            os.chdir(self.directory + "/Scenes")
             split_video_ffmpeg(video_path, scene_list, show_progress=True)
             # os.remove(video_path)
-        self.directory = self.directory + "\\Scenes"
+        self.directory = self.directory + "/Scenes"
 
         video_files = [f for f in os.listdir(self.directory) if f.endswith(".mp4") or f.endswith(".mkv") or f.endswith(".avi") or f.endswith(".mov")]
         Train_X = list()
         FirstFrames=list()
         i=1
         for video_file in video_files:
             FirstFrames.append(i)
@@ -63,15 +63,15 @@
 
 
 
 class Convection3D():
     def __init__(self):
         pass
 
-    def Generate(self,directory=os.getcwd()+ "\\Scenes"):
+    def Generate(self,directory=os.getcwd()+ "/Scenes"):
         model_type = "DPT_Large"
         midas = torch.hub.load("intel-isl/MiDas", model_type, force_reload=False)
         device = torch.device("cuba") if torch.cuda.is_available() else torch.device("cpu")
         midas.to(device)
         midas.eval()
         midas_transforms = torch.hub.load("intel-isl/MiDas", "transforms")
 
@@ -207,7 +207,9 @@
     log.upload("Conv3D.bin")
 
     # Generator = NextFrameGenerator()
     # Train_D = np.random.randint(0, 255, (241, 10000))
     # Train_D_Y = np.random.randint(0, 1, (240, 10000))
     # print("data loaded...")
     # NextFrameGenerator.Train(Train_D, Train_D_Y)
+
+
```
