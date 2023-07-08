# Comparing `tmp/fusionlab-0.1.3.tar.gz` & `tmp/fusionlab-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusionlab-0.1.3.tar", last modified: Fri Jul  7 01:26:44 2023, max compression
+gzip compressed data, was "fusionlab-0.1.4.tar", last modified: Sat Jul  8 09:26:21 2023, max compression
```

## Comparing `fusionlab-0.1.3.tar` & `fusionlab-0.1.4.tar`

### file list

```diff
@@ -1,102 +1,109 @@
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.654669 fusionlab-0.1.3/
--rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.3/LICENSE
--rw-r--r--   0 cyli       (502) staff       (20)     3762 2023-07-07 01:26:44.654502 fusionlab-0.1.3/PKG-INFO
--rw-r--r--   0 cyli       (502) staff       (20)     3299 2023-07-01 03:49:44.000000 fusionlab-0.1.3/README.md
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.632531 fusionlab-0.1.3/fusionlab/
--rw-r--r--   0 cyli       (502) staff       (20)      993 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)       63 2023-07-01 03:50:01.000000 fusionlab-0.1.3/fusionlab/__version__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.634401 fusionlab-0.1.3/fusionlab/classification/
--rw-r--r--   0 cyli       (502) staff       (20)      387 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/classification/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3353 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/classification/base.py
--rw-r--r--   0 cyli       (502) staff       (20)      711 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/classification/lstm.py
--rw-r--r--   0 cyli       (502) staff       (20)     1473 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/classification/vgg.py
--rw-r--r--   0 cyli       (502) staff       (20)       32 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/configs.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.635915 fusionlab-0.1.3/fusionlab/datasets/
--rw-r--r--   0 cyli       (502) staff       (20)      558 2023-07-01 03:49:44.000000 fusionlab-0.1.3/fusionlab/datasets/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/datasets/a12lead.py
--rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/datasets/cinc2017.py
--rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/datasets/csvread.py
--rw-r--r--   0 cyli       (502) staff       (20)    13273 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/datasets/ludb.py
--rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/datasets/muse.py
--rw-r--r--   0 cyli       (502) staff       (20)     4586 2023-07-01 03:49:44.000000 fusionlab-0.1.3/fusionlab/datasets/utils.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.636210 fusionlab-0.1.3/fusionlab/encoders/
--rw-r--r--   0 cyli       (502) staff       (20)      507 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/encoders/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.636732 fusionlab-0.1.3/fusionlab/encoders/alexnet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/encoders/alexnet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/encoders/alexnet/alexnet.py
--rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.3/fusionlab/encoders/alexnet/tfalexnet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.637405 fusionlab-0.1.3/fusionlab/encoders/inceptionv1/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/encoders/inceptionv1/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/encoders/inceptionv1/inceptionv1.py
--rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.3/fusionlab/encoders/inceptionv1/tfinceptionv1.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.645166 fusionlab-0.1.3/fusionlab/encoders/resnetv1/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/encoders/resnetv1/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4838 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/encoders/resnetv1/resnetv1.py
--rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.3/fusionlab/encoders/resnetv1/tfresnetv1.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.645887 fusionlab-0.1.3/fusionlab/encoders/vgg/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/encoders/vgg/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.3/fusionlab/encoders/vgg/tfvgg.py
--rw-r--r--   0 cyli       (502) staff       (20)     4753 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/encoders/vgg/vgg.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.647468 fusionlab-0.1.3/fusionlab/functional/
--rw-r--r--   0 cyli       (502) staff       (20)      347 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/functional/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/functional/dice.py
--rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/functional/iou.py
--rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/functional/tfdice.py
--rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/functional/tfiou.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.647766 fusionlab-0.1.3/fusionlab/layers/
--rw-r--r--   0 cyli       (502) staff       (20)      255 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/layers/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)    17810 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/layers/factories.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.648470 fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1045 2023-05-20 16:17:48.000000 fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/se.py
--rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/tfse.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.648729 fusionlab-0.1.3/fusionlab/losses/
--rw-r--r--   0 cyli       (502) staff       (20)      405 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/losses/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.649202 fusionlab-0.1.3/fusionlab/losses/diceloss/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.3/fusionlab/losses/diceloss/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.3/fusionlab/losses/diceloss/dice.py
--rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.3/fusionlab/losses/diceloss/tfdice.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.649776 fusionlab-0.1.3/fusionlab/losses/iouloss/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.3/fusionlab/losses/iouloss/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.3/fusionlab/losses/iouloss/iou.py
--rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.3/fusionlab/losses/iouloss/tfiou.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.650359 fusionlab-0.1.3/fusionlab/losses/tversky/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.3/fusionlab/losses/tversky/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.3/fusionlab/losses/tversky/tftversky.py
--rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.3/fusionlab/losses/tversky/tversky.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.650605 fusionlab-0.1.3/fusionlab/metrics/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.3/fusionlab/metrics/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.651009 fusionlab-0.1.3/fusionlab/segmentation/
--rw-r--r--   0 cyli       (502) staff       (20)      420 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/segmentation/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1770 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/segmentation/base.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.651443 fusionlab-0.1.3/fusionlab/segmentation/resunet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.3/fusionlab/segmentation/resunet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     5271 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/segmentation/resunet/resunet.py
--rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/segmentation/resunet/tfresunet.py
--rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/segmentation/tfbase.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.651877 fusionlab-0.1.3/fusionlab/segmentation/unet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.3/fusionlab/segmentation/unet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/segmentation/unet/tfunet.py
--rw-r--r--   0 cyli       (502) staff       (20)     5414 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/segmentation/unet/unet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.652361 fusionlab-0.1.3/fusionlab/segmentation/unet2plus/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.3/fusionlab/segmentation/unet2plus/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/segmentation/unet2plus/tfunet2plus.py
--rw-r--r--   0 cyli       (502) staff       (20)     5662 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/segmentation/unet2plus/unet2plus.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.653167 fusionlab-0.1.3/fusionlab/trainers/
--rw-r--r--   0 cyli       (502) staff       (20)      224 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/trainers/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/trainers/dcgan.py
--rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.3/fusionlab/trainers/test.py
--rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/trainers/trainer.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.654147 fusionlab-0.1.3/fusionlab/utils/
--rw-r--r--   0 cyli       (502) staff       (20)       93 2023-07-01 03:49:44.000000 fusionlab-0.1.3/fusionlab/utils/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      218 2022-12-31 04:40:09.000000 fusionlab-0.1.3/fusionlab/utils/basic.py
--rw-r--r--   0 cyli       (502) staff       (20)      406 2023-07-01 03:49:44.000000 fusionlab-0.1.3/fusionlab/utils/plots.py
--rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/utils/trace.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.633307 fusionlab-0.1.3/fusionlab.egg-info/
--rw-r--r--   0 cyli       (502) staff       (20)     3762 2023-07-07 01:26:44.000000 fusionlab-0.1.3/fusionlab.egg-info/PKG-INFO
--rw-r--r--   0 cyli       (502) staff       (20)     2526 2023-07-07 01:26:44.000000 fusionlab-0.1.3/fusionlab.egg-info/SOURCES.txt
--rw-r--r--   0 cyli       (502) staff       (20)        1 2023-07-07 01:26:44.000000 fusionlab-0.1.3/fusionlab.egg-info/dependency_links.txt
--rw-r--r--   0 cyli       (502) staff       (20)      191 2023-07-07 01:26:44.000000 fusionlab-0.1.3/fusionlab.egg-info/requires.txt
--rw-r--r--   0 cyli       (502) staff       (20)       10 2023-07-07 01:26:44.000000 fusionlab-0.1.3/fusionlab.egg-info/top_level.txt
--rw-r--r--   0 cyli       (502) staff       (20)       38 2023-07-07 01:26:44.654721 fusionlab-0.1.3/setup.cfg
--rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.3/setup.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.854576 fusionlab-0.1.4/
+-rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.4/LICENSE
+-rw-r--r--   0 cyli       (502) staff       (20)     3730 2023-07-08 09:26:21.854421 fusionlab-0.1.4/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     3267 2023-07-08 09:17:08.000000 fusionlab-0.1.4/README.md
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.838028 fusionlab-0.1.4/fusionlab/
+-rw-r--r--   0 cyli       (502) staff       (20)      993 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)       63 2023-07-08 09:19:32.000000 fusionlab-0.1.4/fusionlab/__version__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.840314 fusionlab-0.1.4/fusionlab/classification/
+-rw-r--r--   0 cyli       (502) staff       (20)      387 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/classification/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3353 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/classification/base.py
+-rw-r--r--   0 cyli       (502) staff       (20)      711 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/classification/lstm.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1473 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/classification/vgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)       32 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/configs.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.841619 fusionlab-0.1.4/fusionlab/datasets/
+-rw-r--r--   0 cyli       (502) staff       (20)      558 2023-07-01 03:49:44.000000 fusionlab-0.1.4/fusionlab/datasets/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/datasets/a12lead.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/datasets/cinc2017.py
+-rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/datasets/csvread.py
+-rw-r--r--   0 cyli       (502) staff       (20)    13273 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/datasets/ludb.py
+-rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/datasets/muse.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4586 2023-07-01 03:49:44.000000 fusionlab-0.1.4/fusionlab/datasets/utils.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.841885 fusionlab-0.1.4/fusionlab/encoders/
+-rw-r--r--   0 cyli       (502) staff       (20)      906 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/encoders/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.842345 fusionlab-0.1.4/fusionlab/encoders/alexnet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/encoders/alexnet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/encoders/alexnet/alexnet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.4/fusionlab/encoders/alexnet/tfalexnet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.842682 fusionlab-0.1.4/fusionlab/encoders/convnext/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/encoders/convnext/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     8194 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/encoders/convnext/convnext.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.843025 fusionlab-0.1.4/fusionlab/encoders/efficientnet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/encoders/efficientnet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)    12573 2023-07-08 09:19:15.000000 fusionlab-0.1.4/fusionlab/encoders/efficientnet/efficientnet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.843740 fusionlab-0.1.4/fusionlab/encoders/inceptionv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/encoders/inceptionv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/encoders/inceptionv1/inceptionv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.4/fusionlab/encoders/inceptionv1/tfinceptionv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.844359 fusionlab-0.1.4/fusionlab/encoders/resnetv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/encoders/resnetv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4838 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/encoders/resnetv1/resnetv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.4/fusionlab/encoders/resnetv1/tfresnetv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.845000 fusionlab-0.1.4/fusionlab/encoders/vgg/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/encoders/vgg/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.4/fusionlab/encoders/vgg/tfvgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4753 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/encoders/vgg/vgg.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.846444 fusionlab-0.1.4/fusionlab/functional/
+-rw-r--r--   0 cyli       (502) staff       (20)      347 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/functional/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/functional/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/functional/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/functional/tfdice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/functional/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.847036 fusionlab-0.1.4/fusionlab/layers/
+-rw-r--r--   0 cyli       (502) staff       (20)      289 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/layers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3604 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/layers/base.py
+-rw-r--r--   0 cyli       (502) staff       (20)    17832 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/layers/factories.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.847987 fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-07 10:44:19.000000 fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     2187 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/se.py
+-rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/tfse.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.848273 fusionlab-0.1.4/fusionlab/losses/
+-rw-r--r--   0 cyli       (502) staff       (20)      405 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/losses/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.848756 fusionlab-0.1.4/fusionlab/losses/diceloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.4/fusionlab/losses/diceloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.4/fusionlab/losses/diceloss/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.4/fusionlab/losses/diceloss/tfdice.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.849377 fusionlab-0.1.4/fusionlab/losses/iouloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.4/fusionlab/losses/iouloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.4/fusionlab/losses/iouloss/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.4/fusionlab/losses/iouloss/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.849972 fusionlab-0.1.4/fusionlab/losses/tversky/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.4/fusionlab/losses/tversky/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.4/fusionlab/losses/tversky/tftversky.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.4/fusionlab/losses/tversky/tversky.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.850205 fusionlab-0.1.4/fusionlab/metrics/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.4/fusionlab/metrics/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.851218 fusionlab-0.1.4/fusionlab/segmentation/
+-rw-r--r--   0 cyli       (502) staff       (20)      420 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/segmentation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1770 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/segmentation/base.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.851621 fusionlab-0.1.4/fusionlab/segmentation/resunet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.4/fusionlab/segmentation/resunet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5271 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/segmentation/resunet/resunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/segmentation/resunet/tfresunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/segmentation/tfbase.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.851994 fusionlab-0.1.4/fusionlab/segmentation/unet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.4/fusionlab/segmentation/unet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/segmentation/unet/tfunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5414 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/segmentation/unet/unet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.852353 fusionlab-0.1.4/fusionlab/segmentation/unet2plus/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.4/fusionlab/segmentation/unet2plus/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/segmentation/unet2plus/tfunet2plus.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5662 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/segmentation/unet2plus/unet2plus.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.853102 fusionlab-0.1.4/fusionlab/trainers/
+-rw-r--r--   0 cyli       (502) staff       (20)      224 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/trainers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/trainers/dcgan.py
+-rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.4/fusionlab/trainers/test.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/trainers/trainer.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.854111 fusionlab-0.1.4/fusionlab/utils/
+-rw-r--r--   0 cyli       (502) staff       (20)       93 2023-07-01 03:49:44.000000 fusionlab-0.1.4/fusionlab/utils/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      218 2022-12-31 04:40:09.000000 fusionlab-0.1.4/fusionlab/utils/basic.py
+-rw-r--r--   0 cyli       (502) staff       (20)      406 2023-07-01 03:49:44.000000 fusionlab-0.1.4/fusionlab/utils/plots.py
+-rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/utils/trace.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.839044 fusionlab-0.1.4/fusionlab.egg-info/
+-rw-r--r--   0 cyli       (502) staff       (20)     3730 2023-07-08 09:26:21.000000 fusionlab-0.1.4/fusionlab.egg-info/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     2723 2023-07-08 09:26:21.000000 fusionlab-0.1.4/fusionlab.egg-info/SOURCES.txt
+-rw-r--r--   0 cyli       (502) staff       (20)        1 2023-07-08 09:26:21.000000 fusionlab-0.1.4/fusionlab.egg-info/dependency_links.txt
+-rw-r--r--   0 cyli       (502) staff       (20)      191 2023-07-08 09:26:21.000000 fusionlab-0.1.4/fusionlab.egg-info/requires.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       10 2023-07-08 09:26:21.000000 fusionlab-0.1.4/fusionlab.egg-info/top_level.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       38 2023-07-08 09:26:21.854619 fusionlab-0.1.4/setup.cfg
+-rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.4/setup.py
```

### Comparing `fusionlab-0.1.3/LICENSE` & `fusionlab-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/PKG-INFO` & `fusionlab-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionlab
-Version: 0.1.3
+Version: 0.1.4
 Summary: Useful packages for DL
 Home-page: https://github.com/taipingeric/fusionlab
 Author: Chih-Yang Li
 Author-email: taipingeric@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -131,15 +131,15 @@
 
 * UNet
 * ResUNet
 * UNet2plus
 
 ## N Dimensional Model
 
-some model can be used in 1D, 2D, 3D
+some models can be used in 1D, 2D, 3D
 
 ```python
 import fusionlab as fl
 
 resnet1d = fl.encoders.ResNet50V1(cin=3, spatial_dims=1)
 resnet2d = fl.encoders.ResNet50V1(cin=3, spatial_dims=2)
 resnet3d = fl.encoders.ResNet50V1(cin=3, spatial_dims=3)
@@ -147,18 +147,12 @@
 unet1d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=1)
 unet2d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=2)
 unet3d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=3)
 ```
 
 ## News
 
-0.1.2
-
-* Add LUDB dataset
-
-0.0.52
-
-* Tversky Loss for Torch and TF
+[Release logs](./release_logs.md)
 
 ## Acknowledgements
 
 * [BloodAxe/pytorch-toolbelt](https://github.com/BloodAxe/pytorch-toolbelt)
```

### Comparing `fusionlab-0.1.3/README.md` & `fusionlab-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 * UNet
 * ResUNet
 * UNet2plus
 
 ## N Dimensional Model
 
-some model can be used in 1D, 2D, 3D
+some models can be used in 1D, 2D, 3D
 
 ```python
 import fusionlab as fl
 
 resnet1d = fl.encoders.ResNet50V1(cin=3, spatial_dims=1)
 resnet2d = fl.encoders.ResNet50V1(cin=3, spatial_dims=2)
 resnet3d = fl.encoders.ResNet50V1(cin=3, spatial_dims=3)
@@ -130,18 +130,12 @@
 unet1d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=1)
 unet2d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=2)
 unet3d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=3)
 ```
 
 ## News
 
-0.1.2
-
-* Add LUDB dataset
-
-0.0.52
-
-* Tversky Loss for Torch and TF
+[Release logs](./release_logs.md)
 
 ## Acknowledgements
 
 * [BloodAxe/pytorch-toolbelt](https://github.com/BloodAxe/pytorch-toolbelt)
```

### Comparing `fusionlab-0.1.3/fusionlab/__init__.py` & `fusionlab-0.1.4/fusionlab/__init__.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/classification/base.py` & `fusionlab-0.1.4/fusionlab/classification/base.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/classification/lstm.py` & `fusionlab-0.1.4/fusionlab/classification/lstm.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/classification/vgg.py` & `fusionlab-0.1.4/fusionlab/classification/vgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/datasets/__init__.py` & `fusionlab-0.1.4/fusionlab/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/datasets/a12lead.py` & `fusionlab-0.1.4/fusionlab/datasets/a12lead.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/datasets/cinc2017.py` & `fusionlab-0.1.4/fusionlab/datasets/cinc2017.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/datasets/ludb.py` & `fusionlab-0.1.4/fusionlab/datasets/ludb.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/datasets/muse.py` & `fusionlab-0.1.4/fusionlab/datasets/muse.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/datasets/utils.py` & `fusionlab-0.1.4/fusionlab/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/encoders/alexnet/alexnet.py` & `fusionlab-0.1.4/fusionlab/encoders/alexnet/alexnet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/encoders/alexnet/tfalexnet.py` & `fusionlab-0.1.4/fusionlab/encoders/alexnet/tfalexnet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/encoders/inceptionv1/inceptionv1.py` & `fusionlab-0.1.4/fusionlab/encoders/inceptionv1/inceptionv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/encoders/inceptionv1/tfinceptionv1.py` & `fusionlab-0.1.4/fusionlab/encoders/inceptionv1/tfinceptionv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/encoders/resnetv1/resnetv1.py` & `fusionlab-0.1.4/fusionlab/encoders/resnetv1/resnetv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/encoders/resnetv1/tfresnetv1.py` & `fusionlab-0.1.4/fusionlab/encoders/resnetv1/tfresnetv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/encoders/vgg/tfvgg.py` & `fusionlab-0.1.4/fusionlab/encoders/vgg/tfvgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/encoders/vgg/vgg.py` & `fusionlab-0.1.4/fusionlab/encoders/vgg/vgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/functional/tfdice.py` & `fusionlab-0.1.4/fusionlab/functional/tfdice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/functional/tfiou.py` & `fusionlab-0.1.4/fusionlab/functional/tfiou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/layers/factories.py` & `fusionlab-0.1.4/fusionlab/layers/factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,16 @@
         track_running_stats: a boolean value that when set to ``True``, this
             module tracks the running mean and variance, and when set to ``False``,
             this module does not track such statistics, and initializes statistics
             buffers :attr:`running_mean` and :attr:`running_var` as ``None``.
             When these buffers are ``None``, this module always uses batch statistics.
             in both training and eval modes. Default: ``True``
     """
-    def __new__(cls, spatial_dims, 
+    def __new__(cls, 
+                spatial_dims: int, 
                 num_features: int,
                 eps: float = 1e-5,
                 momentum: float = 0.1,
                 affine: bool = True,
                 track_running_stats: bool = True):
         if spatial_dims not in [1, 2, 3]:
             raise ValueError(f'`spatial_dims` must be 1, 2, or 3, got {spatial_dims}')
```

### Comparing `fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/tfse.py` & `fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/tfse.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/losses/diceloss/dice.py` & `fusionlab-0.1.4/fusionlab/losses/diceloss/dice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/losses/diceloss/tfdice.py` & `fusionlab-0.1.4/fusionlab/losses/diceloss/tfdice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/losses/iouloss/iou.py` & `fusionlab-0.1.4/fusionlab/losses/iouloss/iou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/losses/iouloss/tfiou.py` & `fusionlab-0.1.4/fusionlab/losses/iouloss/tfiou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/losses/tversky/tftversky.py` & `fusionlab-0.1.4/fusionlab/losses/tversky/tftversky.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/losses/tversky/tversky.py` & `fusionlab-0.1.4/fusionlab/losses/tversky/tversky.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/segmentation/base.py` & `fusionlab-0.1.4/fusionlab/segmentation/base.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/segmentation/resunet/resunet.py` & `fusionlab-0.1.4/fusionlab/segmentation/resunet/resunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/segmentation/resunet/tfresunet.py` & `fusionlab-0.1.4/fusionlab/segmentation/resunet/tfresunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/segmentation/tfbase.py` & `fusionlab-0.1.4/fusionlab/segmentation/tfbase.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/segmentation/unet/tfunet.py` & `fusionlab-0.1.4/fusionlab/segmentation/unet/tfunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/segmentation/unet/unet.py` & `fusionlab-0.1.4/fusionlab/segmentation/unet/unet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/segmentation/unet2plus/tfunet2plus.py` & `fusionlab-0.1.4/fusionlab/segmentation/unet2plus/tfunet2plus.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/segmentation/unet2plus/unet2plus.py` & `fusionlab-0.1.4/fusionlab/segmentation/unet2plus/unet2plus.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/trainers/dcgan.py` & `fusionlab-0.1.4/fusionlab/trainers/dcgan.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/trainers/trainer.py` & `fusionlab-0.1.4/fusionlab/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab/utils/trace.py` & `fusionlab-0.1.4/fusionlab/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.3/fusionlab.egg-info/PKG-INFO` & `fusionlab-0.1.4/fusionlab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionlab
-Version: 0.1.3
+Version: 0.1.4
 Summary: Useful packages for DL
 Home-page: https://github.com/taipingeric/fusionlab
 Author: Chih-Yang Li
 Author-email: taipingeric@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -131,15 +131,15 @@
 
 * UNet
 * ResUNet
 * UNet2plus
 
 ## N Dimensional Model
 
-some model can be used in 1D, 2D, 3D
+some models can be used in 1D, 2D, 3D
 
 ```python
 import fusionlab as fl
 
 resnet1d = fl.encoders.ResNet50V1(cin=3, spatial_dims=1)
 resnet2d = fl.encoders.ResNet50V1(cin=3, spatial_dims=2)
 resnet3d = fl.encoders.ResNet50V1(cin=3, spatial_dims=3)
@@ -147,18 +147,12 @@
 unet1d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=1)
 unet2d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=2)
 unet3d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=3)
 ```
 
 ## News
 
-0.1.2
-
-* Add LUDB dataset
-
-0.0.52
-
-* Tversky Loss for Torch and TF
+[Release logs](./release_logs.md)
 
 ## Acknowledgements
 
 * [BloodAxe/pytorch-toolbelt](https://github.com/BloodAxe/pytorch-toolbelt)
```

### Comparing `fusionlab-0.1.3/fusionlab.egg-info/SOURCES.txt` & `fusionlab-0.1.4/fusionlab.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 fusionlab/datasets/ludb.py
 fusionlab/datasets/muse.py
 fusionlab/datasets/utils.py
 fusionlab/encoders/__init__.py
 fusionlab/encoders/alexnet/__init__.py
 fusionlab/encoders/alexnet/alexnet.py
 fusionlab/encoders/alexnet/tfalexnet.py
+fusionlab/encoders/convnext/__init__.py
+fusionlab/encoders/convnext/convnext.py
+fusionlab/encoders/efficientnet/__init__.py
+fusionlab/encoders/efficientnet/efficientnet.py
 fusionlab/encoders/inceptionv1/__init__.py
 fusionlab/encoders/inceptionv1/inceptionv1.py
 fusionlab/encoders/inceptionv1/tfinceptionv1.py
 fusionlab/encoders/resnetv1/__init__.py
 fusionlab/encoders/resnetv1/resnetv1.py
 fusionlab/encoders/resnetv1/tfresnetv1.py
 fusionlab/encoders/vgg/__init__.py
@@ -35,14 +39,15 @@
 fusionlab/encoders/vgg/vgg.py
 fusionlab/functional/__init__.py
 fusionlab/functional/dice.py
 fusionlab/functional/iou.py
 fusionlab/functional/tfdice.py
 fusionlab/functional/tfiou.py
 fusionlab/layers/__init__.py
+fusionlab/layers/base.py
 fusionlab/layers/factories.py
 fusionlab/layers/squeeze_excitation/__init__.py
 fusionlab/layers/squeeze_excitation/se.py
 fusionlab/layers/squeeze_excitation/tfse.py
 fusionlab/losses/__init__.py
 fusionlab/losses/diceloss/__init__.py
 fusionlab/losses/diceloss/dice.py
```

### Comparing `fusionlab-0.1.3/setup.py` & `fusionlab-0.1.4/setup.py`

 * *Files identical despite different names*

