# Comparing `tmp/medisynth-0.0.0.tar.gz` & `tmp/medisynth-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medisynth-0.0.0.tar", last modified: Sun Jul  2 11:05:45 2023, max compression
+gzip compressed data, was "medisynth-0.0.1.tar", last modified: Sat Jul  8 12:11:00 2023, max compression
```

## Comparing `medisynth-0.0.0.tar` & `medisynth-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-02 11:05:45.382506 medisynth-0.0.0/
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      584 2023-07-02 11:05:45.382506 medisynth-0.0.0/PKG-INFO
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     4617 2023-07-02 10:25:20.000000 medisynth-0.0.0/README.md
-drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-02 11:05:45.382506 medisynth-0.0.0/medisynth/
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       49 2023-07-02 10:25:20.000000 medisynth-0.0.0/medisynth/__init__.py
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     2920 2023-07-02 10:25:20.000000 medisynth-0.0.0/medisynth/medisynth.py
-drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-02 11:05:45.382506 medisynth-0.0.0/medisynth.egg-info/
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      584 2023-07-02 11:05:45.000000 medisynth-0.0.0/medisynth.egg-info/PKG-INFO
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      227 2023-07-02 11:05:45.000000 medisynth-0.0.0/medisynth.egg-info/SOURCES.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-02 11:05:45.000000 medisynth-0.0.0/medisynth.egg-info/dependency_links.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        6 2023-07-02 11:05:45.000000 medisynth-0.0.0/medisynth.egg-info/requires.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       10 2023-07-02 11:05:45.000000 medisynth-0.0.0/medisynth.egg-info/top_level.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       38 2023-07-02 11:05:45.382506 medisynth-0.0.0/setup.cfg
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      829 2023-07-02 10:25:20.000000 medisynth-0.0.0/setup.py
+drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-08 12:11:00.728814 medisynth-0.0.1/
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     5363 2023-07-08 12:11:00.728814 medisynth-0.0.1/PKG-INFO
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     4761 2023-07-08 10:06:20.000000 medisynth-0.0.1/README.md
+drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-08 12:11:00.728814 medisynth-0.0.1/medisynth.egg-info/
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     5363 2023-07-08 12:11:00.000000 medisynth-0.0.1/medisynth.egg-info/PKG-INFO
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      198 2023-07-08 12:11:00.000000 medisynth-0.0.1/medisynth.egg-info/SOURCES.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-08 12:11:00.000000 medisynth-0.0.1/medisynth.egg-info/dependency_links.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       35 2023-07-08 12:11:00.000000 medisynth-0.0.1/medisynth.egg-info/requires.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-08 12:11:00.000000 medisynth-0.0.1/medisynth.egg-info/top_level.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       99 2023-07-08 12:08:20.000000 medisynth-0.0.1/pyproject.toml
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      834 2023-07-08 12:11:00.728814 medisynth-0.0.1/setup.cfg
```

### Comparing `medisynth-0.0.0/README.md` & `medisynth-0.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # medisynth
+[![PyPI version](https://badge.fury.io/py/medisynth.svg)](https://badge.fury.io/py/medisynth)
 
 A library for ultrasound fetal brain imaging using techniques from diffusion models
 
+
+## Install
+
+```bash
+$ pip install medisynth
+```
+
 ## Slides
 Good practices in AI/ML for Ultrasound Fetal Brain Imaging Synthesis   
 Harvey Mannering, Sofia Miñano, and Miguel Xochicale      
 
 University College London     
 The deep learning and computer vision Journal Club       
 UCL Centre for Advance Research Computing
```

#### html2text {}

```diff
@@ -1,37 +1,39 @@
-# medisynth A library for ultrasound fetal brain imaging using techniques from
-diffusion models ## Slides Good practices in AI/ML for Ultrasound Fetal Brain
-Imaging Synthesis Harvey Mannering, Sofia MiÃ±ano, and Miguel Xochicale
-University College London The deep learning and computer vision Journal Club
-UCL Centre for Advance Research Computing 1st of June 2023, 15:00 GMT ###
-Abstract Medical image datasets for AI and ML methods must be diverse to
-generalise well unseen data (i.e. diagnoses, diseases, pathologies, scanners,
-demographics, etc). However there are few public ultrasound fetal imaging
-datasets due to insufficient amounts of clinical data, patient privacy, rare
-occurrence of abnormalities, and limited experts for data collection and
-validation. To address such challenges in Ultrasound Medical Imaging, Miguel
-will discuss two proposed generative adversarial networks (GAN)-based models:
-diffusion-super-resolution-GAN and transformer-based-GAN, to synthesise images
-of fetal Ultrasound brain image planes from one public dataset. Similarly,
-Miguel will present and discuss AI and ML workflow aligned to good ML practices
-by FDA, and methods for quality image assessment (e.g., visual Turing test and
-FID scores). Finally, a simple prototype in GitHub, google-colabs and
-guidelines to train it using Myriad cluster will be presented as well as
-applications for Medical Image Synthesis e.g., classification, augmentation,
-segmentation, registration and other downstream tasks, etc. will be discussed.
-The resources to reproduce the work of this talk are available at https://
-github.com/mxochicale/medisynth. ## Clone repository * Generate your SSH keys
-as suggested [here](https://docs.github.com/en/github/authenticating-to-github/
-generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) (or [here](https://
-github.com/mxochicale/tools/blob/main/github/SSH.md)) * Clone the repository by
-typing (or copying) the following line in a terminal at your selected path in
-your machine: ``` cd && mkdir -p $HOME/repositories/$USERNAME && cd $HOME/
-repositories/$USERNAME git clone git@github.com:mxochicale/medisynth.git ``` ##
-Contributors Thanks goes to all these people ([emoji key](https://
-allcontributors.org/docs/en/emoji-key)):
+# medisynth [![PyPI version](https://badge.fury.io/py/medisynth.svg)](https://
+badge.fury.io/py/medisynth) A library for ultrasound fetal brain imaging using
+techniques from diffusion models ## Install ```bash $ pip install medisynth ```
+## Slides Good practices in AI/ML for Ultrasound Fetal Brain Imaging Synthesis
+Harvey Mannering, Sofia MiÃ±ano, and Miguel Xochicale University College London
+The deep learning and computer vision Journal Club UCL Centre for Advance
+Research Computing 1st of June 2023, 15:00 GMT ### Abstract Medical image
+datasets for AI and ML methods must be diverse to generalise well unseen data
+(i.e. diagnoses, diseases, pathologies, scanners, demographics, etc). However
+there are few public ultrasound fetal imaging datasets due to insufficient
+amounts of clinical data, patient privacy, rare occurrence of abnormalities,
+and limited experts for data collection and validation. To address such
+challenges in Ultrasound Medical Imaging, Miguel will discuss two proposed
+generative adversarial networks (GAN)-based models: diffusion-super-resolution-
+GAN and transformer-based-GAN, to synthesise images of fetal Ultrasound brain
+image planes from one public dataset. Similarly, Miguel will present and
+discuss AI and ML workflow aligned to good ML practices by FDA, and methods for
+quality image assessment (e.g., visual Turing test and FID scores). Finally, a
+simple prototype in GitHub, google-colabs and guidelines to train it using
+Myriad cluster will be presented as well as applications for Medical Image
+Synthesis e.g., classification, augmentation, segmentation, registration and
+other downstream tasks, etc. will be discussed. The resources to reproduce the
+work of this talk are available at https://github.com/mxochicale/medisynth. ##
+Clone repository * Generate your SSH keys as suggested [here](https://
+docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-
+and-adding-it-to-the-ssh-agent) (or [here](https://github.com/mxochicale/tools/
+blob/main/github/SSH.md)) * Clone the repository by typing (or copying) the
+following line in a terminal at your selected path in your machine: ``` cd &&
+mkdir -p $HOME/repositories/$USERNAME && cd $HOME/repositories/$USERNAME git
+clone git@github.com:mxochicale/medisynth.git ``` ## Contributors Thanks goes
+to all these people ([emoji key](https://allcontributors.org/docs/en/emoji-
+key)):
 
                          Sofia_MiÃ±ano           Harvey_Mannering
  ADD_NAME_SURNAME                                                             Miguel_Xochicale
                          ð» ð¬_ð�      ð» ð¬_ð�       ð» ð_ð§
      ð¬_ð¤
    This work follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
```

