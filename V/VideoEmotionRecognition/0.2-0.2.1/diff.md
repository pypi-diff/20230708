# Comparing `tmp/VideoEmotionRecognition-0.2.tar.gz` & `tmp/VideoEmotionRecognition-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VideoEmotionRecognition-0.2.tar", last modified: Sun Jul  2 18:43:28 2023, max compression
+gzip compressed data, was "VideoEmotionRecognition-0.2.1.tar", last modified: Sat Jul  8 16:56:45 2023, max compression
```

## Comparing `VideoEmotionRecognition-0.2.tar` & `VideoEmotionRecognition-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-02 18:43:28.011366 VideoEmotionRecognition-0.2/
--rw-r--r--   0 art       (1000) art       (1000)     1081 2023-06-26 12:27:40.000000 VideoEmotionRecognition-0.2/LICENSE
--rw-r--r--   0 art       (1000) art       (1000)     1752 2023-07-02 18:43:28.011366 VideoEmotionRecognition-0.2/PKG-INFO
--rw-r--r--   0 art       (1000) art       (1000)     1077 2023-06-25 22:04:56.000000 VideoEmotionRecognition-0.2/README.md
--rw-r--r--   0 art       (1000) art       (1000)      747 2023-07-02 18:43:03.000000 VideoEmotionRecognition-0.2/pyproject.toml
--rw-r--r--   0 art       (1000) art       (1000)       38 2023-07-02 18:43:28.011366 VideoEmotionRecognition-0.2/setup.cfg
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-02 18:43:28.011366 VideoEmotionRecognition-0.2/src/
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-02 18:43:28.011366 VideoEmotionRecognition-0.2/src/VideoEmotionRecognition/
--rw-r--r--   0 art       (1000) art       (1000)        0 2023-07-02 18:32:19.000000 VideoEmotionRecognition-0.2/src/VideoEmotionRecognition/__init__.py
--rw-r--r--   0 art       (1000) art       (1000)     6075 2023-07-02 17:44:16.000000 VideoEmotionRecognition-0.2/src/VideoEmotionRecognition/viemr.py
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-02 18:43:28.011366 VideoEmotionRecognition-0.2/src/VideoEmotionRecognition.egg-info/
--rw-r--r--   0 art       (1000) art       (1000)     1752 2023-07-02 18:43:28.000000 VideoEmotionRecognition-0.2/src/VideoEmotionRecognition.egg-info/PKG-INFO
--rw-r--r--   0 art       (1000) art       (1000)      313 2023-07-02 18:43:28.000000 VideoEmotionRecognition-0.2/src/VideoEmotionRecognition.egg-info/SOURCES.txt
--rw-r--r--   0 art       (1000) art       (1000)        1 2023-07-02 18:43:28.000000 VideoEmotionRecognition-0.2/src/VideoEmotionRecognition.egg-info/dependency_links.txt
--rw-r--r--   0 art       (1000) art       (1000)       24 2023-07-02 18:43:28.000000 VideoEmotionRecognition-0.2/src/VideoEmotionRecognition.egg-info/top_level.txt
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/
+-rw-r--r--   0 art       (1000) art       (1000)     1081 2023-06-26 12:27:40.000000 VideoEmotionRecognition-0.2.1/LICENSE
+-rw-r--r--   0 art       (1000) art       (1000)     1754 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/PKG-INFO
+-rw-r--r--   0 art       (1000) art       (1000)     1077 2023-06-25 22:04:56.000000 VideoEmotionRecognition-0.2.1/README.md
+-rw-r--r--   0 art       (1000) art       (1000)      749 2023-07-08 16:56:21.000000 VideoEmotionRecognition-0.2.1/pyproject.toml
+-rw-r--r--   0 art       (1000) art       (1000)       38 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/setup.cfg
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/src/
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition/
+-rw-r--r--   0 art       (1000) art       (1000)       42 2023-07-08 13:23:30.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition/__init__.py
+-rw-r--r--   0 art       (1000) art       (1000)     7989 2023-07-08 16:53:34.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition/viemr.py
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/
+-rw-r--r--   0 art       (1000) art       (1000)     1754 2023-07-08 16:56:45.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/PKG-INFO
+-rw-r--r--   0 art       (1000) art       (1000)      313 2023-07-08 16:56:45.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/SOURCES.txt
+-rw-r--r--   0 art       (1000) art       (1000)        1 2023-07-08 16:56:45.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/dependency_links.txt
+-rw-r--r--   0 art       (1000) art       (1000)       24 2023-07-08 16:56:45.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/top_level.txt
```

### Comparing `VideoEmotionRecognition-0.2/LICENSE` & `VideoEmotionRecognition-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `VideoEmotionRecognition-0.2/PKG-INFO` & `VideoEmotionRecognition-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VideoEmotionRecognition
-Version: 0.2
+Version: 0.2.1
 Summary: This package receives an mp4 file classfying it according to its emotions and generating a heat map
 Author-email: Artur Lima <vligmart@gmail.com>
 Project-URL: Homepage, https://github.com/Deflyer/Multimodal-Emotion-Recognition-from-Videos
 Project-URL: Example, https://colab.research.google.com/drive/1UqzA6bDgtZWGji652a0UjT7ZtDh3Xyi5?authuser=1#scrollTo=CKL-Mm9D18BB
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `VideoEmotionRecognition-0.2/README.md` & `VideoEmotionRecognition-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `VideoEmotionRecognition-0.2/pyproject.toml` & `VideoEmotionRecognition-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "VideoEmotionRecognition"
-version = "0.2"
+version = "0.2.1"
 authors = [
   { name="Artur Lima", email="vligmart@gmail.com" },
 ]
 description = "This package receives an mp4 file classfying it according to its emotions and generating a heat map"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `VideoEmotionRecognition-0.2/src/VideoEmotionRecognition/viemr.py` & `VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition/viemr.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,32 +4,55 @@
 import gdown
 import matplotlib.pyplot as plt
 import whisperx
 import gc
 import transformers
 import webvtt
 import os
+import logging
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, pipeline
 from transformers import RobertaTokenizerFast, TFRobertaForSequenceClassification
 
 class VideoEmotionRecognition:
     def __init__(self, mp4):
-        
+
+        logging.basicConfig(filename="newfile.log",
+        format='%(asctime)s %(message)s',filemode='w')
+        self.logger = logging.getLogger()
+        self.logger.setLevel(logging.INFO)
+
+        self.logger.info("Initializing the class")
+
         self.dataframe = -1
         self.mp4 = mp4
 
+        self.logger.info("Loading the arousal_valence map")
+
         url1 = 'https://drive.google.com/uc?id=1yJBHU8Zl4MuoQfJqkPgVDwJfYRJDPUAH'
         output = 'emotions_coord.xlsx'
         gdown.download(url1, output, quiet=False)
         self.emotions_coord = pd.read_excel(output)
 
-    def transcript(self, method = "whisperx"):
+        self.logger.info("Successfully initialized")
+
+
+    def transcript(self, method = "whisperx", min_time = 1):
+        self.logger.info("Running the whisperx transcription")
         bashCommand = "whisperx --compute_type float32 --output_format vtt " + self.mp4
         os.system(bashCommand)
+        self.logger.info("Successfully transcripted")
+
+        self.logger.info("Generating the Dataframe from the vtt")
         self.set_vtt(self.mp4.replace("mp4", "vtt"))
+
+        self.dataframe = self.dataframe[self.dataframe.apply(lambda x: time_diff(x[1], x[0]), axis=1) > min_time]
+        self.dataframe.reset_index(inplace = True)
+
+        self.logger.info("Successfully generated the dataframe")
+
     #Funcao utilizada para gerar uma coluna de strings no Dataframe contendo cada frase traduzida para o inglês
     def __Traduz(self, frase):
         traducao = self.pten_pipeline(frase)
         traducao = list(traducao[0].values())
         return traducao[0]
 
     #Função para extrair do dicionario retornado pelo goemotions a emoção mais provável e sua probabilidade
@@ -43,40 +66,52 @@
             if dict["score"] > max:
               max = dict["score"]
               emocao = dict["label"]
 
         return emocao, max
 
     def emotion_recognition(self, modality = "transcript", method = "RoBERTa-Go-Emotion"):
-        tokenizer = AutoTokenizer.from_pretrained("unicamp-dl/translation-pt-en-t5")
-
-        model = AutoModelForSeq2SeqLM.from_pretrained("unicamp-dl/translation-pt-en-t5")
+        try:
+            self.dataframe.size
+            self.logger.info("Loading the translator")
+            tokenizer = AutoTokenizer.from_pretrained("unicamp-dl/translation-pt-en-t5")
+
+            model = AutoModelForSeq2SeqLM.from_pretrained("unicamp-dl/translation-pt-en-t5")
+
+            self.pten_pipeline = pipeline('text2text-generation', model=model, tokenizer=tokenizer)
+
+            self.logger.info("Successfully loaded, now applyng")
+            self.dataframe['Translation'] = list(self.dataframe[2].apply(self.__Traduz))
+
+            self.logger.info("Loading the classifier")
+            tokenizer = RobertaTokenizerFast.from_pretrained("bhadresh-savani/bert-base-go-emotion")
+            model = TFRobertaForSequenceClassification.from_pretrained("bhadresh-savani/bert-base-go-emotion",from_pt=True)
+
+            self.emotion = pipeline('sentiment-analysis',
+                                model="bhadresh-savani/bert-base-go-emotion",
+                                return_all_scores=True)
+
+            self.logger.info("Successfully loaded, now applying")
+            resp = list(self.dataframe['Translation'].apply(self.__Emocao_provavel))
+            temp = pd.DataFrame.from_records(resp, columns=['label', 'prob'])
+
+            self.dataframe = pd.concat([self.dataframe, temp], axis=1)
+            self.logger.info("Dataframe emotions classified")
+        except AttributeError:
+          raise ValueError("There is no transcription")
 
-        self.pten_pipeline = pipeline('text2text-generation', model=model, tokenizer=tokenizer)
-
-        self.dataframe['Translation'] = list(self.dataframe[2].apply(self.__Traduz))
-
-        tokenizer = RobertaTokenizerFast.from_pretrained("bhadresh-savani/bert-base-go-emotion")
-        model = TFRobertaForSequenceClassification.from_pretrained("bhadresh-savani/bert-base-go-emotion",from_pt=True)
-
-        self.emotion = pipeline('sentiment-analysis',
-                            model="bhadresh-savani/bert-base-go-emotion",
-                            return_all_scores=True)
-
-        resp = list(self.dataframe['Translation'].apply(self.__Emocao_provavel))
-        temp = pd.DataFrame.from_records(resp, columns=['label', 'prob'])
-
-        self.dataframe = pd.concat([self.dataframe, temp], axis=1)
     def set_vtt(self, arquivo):
+        self.logger.info("Loading dataframe via vtt")
         L = []
 
         for caption in webvtt.read(arquivo):
             L.append([caption.start,caption.end,str(caption.text)])
 
         self.dataframe = pd.DataFrame(L)
+        self.logger.info("Successfully loaded")
 
     def get_labels(self, modality = "transcript"):
         return self.dataframe
 
     def __generate_coord(self,label):
         index = self.emotions_coord.loc[self.emotions_coord['Emotion'] == label].index[0]
         x = self.emotions_coord.iloc[index]['X']
@@ -85,15 +120,16 @@
 
     def __kde_quartic(self,d,h):
         dn=d/h
         P=(15/16)*(1-dn**2)**2
         return P
 
     def get_heatmap(self, modality = "transcript"):
-
+        
+        self.logger.info("Adding the arousal valence coordinates")
         resp = list(self.dataframe['label'].apply(self.__generate_coord))
         temp = pd.DataFrame.from_records(resp, columns=['x', 'y'])
 
         self.dataframe = pd.concat([self.dataframe, temp], axis=1)
         self.dataframe = self.dataframe[self.dataframe.label!='neutral']
         self.dataframe = self.dataframe.reset_index(drop=True)
 
@@ -117,14 +153,15 @@
         y_grid=np.arange(y_min-h,y_max+h,grid_size)
         x_mesh,y_mesh=np.meshgrid(x_grid,y_grid)
 
         #Determinando ponto central do grid
         xc=x_mesh+(grid_size/2)
         yc=y_mesh+(grid_size/2)
 
+        self.logger.info("Generating the intensity list for heatmap")
         intensity_list=[]
         for j in range(len(xc)):
             intensity_row=[]
             for k in range(len(xc[0])):
                 kde_value_list=[]
                 for i in range(len(x)):
                     #Calculando distância
@@ -134,15 +171,16 @@
                     else:
                         p=0
                     kde_value_list.append(p)
                 #Soma os valores de intensidade
                 p_total=sum(kde_value_list)
                 intensity_row.append(p_total)
             intensity_list.append(intensity_row)
-
+            
+        self.logger.info("Generating the plot")
         #Saída do Heatmap
         plt.figure(figsize=(7,7))
 
         intensity=np.array(intensity_list)
         plt.pcolormesh(x_mesh,y_mesh,intensity,cmap='YlOrRd') #https://matplotlib.org/stable/tutorials/colors/colormaps.html
 
 
@@ -163,7 +201,16 @@
         ax.add_patch(plt.Circle((0, 0), 1, color='black', fill=False))
         plt.axvline(x = 0, color = 'black', label = 'Arousal')
         plt.axhline(y = 0, color = 'black', label = 'Valence')
 
         #plt.colorbar()
         plt.plot(x,y,'x',color='white')
 
+def time_diff(fim, init):
+
+    str_fim = fim.split(":")
+    str_init = init.split(":")
+
+    time_fim = 3600*int(str_fim[0]) + 60*int(str_fim[1]) + float(str_fim[2])
+    time_init = 3600*int(str_init[0]) + 60*int(str_init[1]) + float(str_init[2])
+
+    return time_fim - time_init
```

### Comparing `VideoEmotionRecognition-0.2/src/VideoEmotionRecognition.egg-info/PKG-INFO` & `VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VideoEmotionRecognition
-Version: 0.2
+Version: 0.2.1
 Summary: This package receives an mp4 file classfying it according to its emotions and generating a heat map
 Author-email: Artur Lima <vligmart@gmail.com>
 Project-URL: Homepage, https://github.com/Deflyer/Multimodal-Emotion-Recognition-from-Videos
 Project-URL: Example, https://colab.research.google.com/drive/1UqzA6bDgtZWGji652a0UjT7ZtDh3Xyi5?authuser=1#scrollTo=CKL-Mm9D18BB
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

