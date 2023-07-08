# Comparing `tmp/sklearn2pmml-0.94.0.tar.gz` & `tmp/sklearn2pmml-0.94.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sklearn2pmml-0.94.0.tar", last modified: Mon Jun 19 19:22:25 2023, max compression
+gzip compressed data, was "dist/sklearn2pmml-0.94.1.tar", last modified: Sat Jul  8 06:47:06 2023, max compression
```

## Comparing `sklearn2pmml-0.94.0.tar` & `sklearn2pmml-0.94.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.0/setup.cfg
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.0/LICENSE.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/setup.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/PKG-INFO
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/h2o.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/ruleset/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/ruleset/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/pipeline/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/pipeline/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/tpot.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    11627 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/decoration/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/decoration/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/neural_network/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/neural_network/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/pycaret.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/util/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/util/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/xgboost.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_extraction/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_extraction/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_extraction/text/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_extraction/text/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/ensemble/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/ensemble/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/statsmodels.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_selection/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/feature_selection/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/postprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/postprocessing/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   202327 2023-06-11 10:10:38.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-python-1.1.15.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    33104 2023-06-11 15:37:09.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jcommander-1.72.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6331 2023-06-19 19:03:17.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.30.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-model-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   432826 2023-05-01 06:26:58.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/guava-21.0.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7974 2023-06-19 19:03:17.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.30.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/ubjson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    83162 2023-06-19 19:03:17.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.30.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6242 2023-06-19 19:03:17.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.30.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7310 2023-06-19 19:03:17.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.30.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-06-19 19:18:50.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/classpath.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-05-01 06:26:58.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    46831 2023-06-15 18:20:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-h2o-1.2.7.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5703 2023-06-19 19:18:51.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   468727 2023-06-19 19:03:16.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-1.7.30.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/serpent-1.40.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/pickle-1.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.94.0/sklearn2pmml/resources/gson-2.10.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-06-19 19:18:28.000000 sklearn2pmml-0.94.0/sklearn2pmml/metadata.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/h2o.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/xgboost.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/lightgbm.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/tree/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/tree/chaid.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/tree/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-06-19 19:22:25.000000 sklearn2pmml-0.94.0/sklearn2pmml/expression/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.0/sklearn2pmml/expression/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.1/setup.cfg
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.1/LICENSE.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/setup.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/PKG-INFO
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/h2o.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/ruleset/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/ruleset/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/pipeline/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/pipeline/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/tpot.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    11627 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/decoration/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/decoration/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/neural_network/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/neural_network/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/pycaret.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/util/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/util/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/xgboost.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_extraction/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_extraction/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_extraction/text/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_extraction/text/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/ensemble/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/ensemble/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/statsmodels.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_selection/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_selection/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/postprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/postprocessing/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6333 2023-07-08 06:03:24.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.31.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   202327 2023-06-11 10:10:38.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-python-1.1.15.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    33104 2023-06-11 15:37:09.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jcommander-1.72.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-model-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-converter-1.5.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/guava-21.0.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7976 2023-07-08 06:03:24.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.31.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-07-08 05:55:57.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-logger-3.42.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6242 2023-07-08 06:03:24.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.31.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   442644 2023-07-08 05:55:57.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-genmodel-3.42.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/ubjson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   472037 2023-07-08 06:03:23.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-1.7.31.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-07-08 06:28:35.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/classpath.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    46831 2023-06-15 18:20:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-h2o-1.2.7.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     5711 2023-07-08 06:24:13.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7311 2023-07-08 06:03:24.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.31.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/serpent-1.40.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    83825 2023-07-08 06:03:24.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.31.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pickle-1.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/gson-2.10.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-07-08 06:24:05.000000 sklearn2pmml-0.94.1/sklearn2pmml/metadata.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/h2o.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/xgboost.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/lightgbm.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/tree/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/tree/chaid.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/tree/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/expression/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/expression/__init__.py
```

### Comparing `sklearn2pmml-0.94.0/LICENSE.txt` & `sklearn2pmml-0.94.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/setup.py` & `sklearn2pmml-0.94.1/setup.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/PKG-INFO` & `sklearn2pmml-0.94.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sklearn2pmml
-Version: 0.94.0
+Version: 0.94.1
 Summary: Python library for converting Scikit-Learn pipelines to PMML
 Home-page: https://github.com/jpmml/sklearn2pmml
 Author: Villu Ruusmann
 Author-email: villu.ruusmann@gmail.com
 License: GNU Affero General Public License (AGPL) version 3.0
-Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.94.0.tar.gz
+Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.94.1.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/h2o.py` & `sklearn2pmml-0.94.1/sklearn2pmml/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/ruleset/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/pipeline/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/tpot.py` & `sklearn2pmml-0.94.1/sklearn2pmml/tpot.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/decoration/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/decoration/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/neural_network/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/neural_network/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/pycaret.py` & `sklearn2pmml-0.94.1/sklearn2pmml/pycaret.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/util/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/xgboost.py` & `sklearn2pmml-0.94.1/sklearn2pmml/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/feature_extraction/text/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/feature_extraction/text/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/ensemble/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/statsmodels.py` & `sklearn2pmml-0.94.1/sklearn2pmml/statsmodels.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/feature_selection/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/postprocessing/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-python-1.1.15.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-python-1.1.15.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/jcommander-1.72.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/jcommander-1.72.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.30.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.31.jar`

 * *Files 17% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 6331 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 h2o/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 h2o/estimators/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/preprocessing/h2o/
--rw-rw-r--  2.0 unx      679 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     5710 b- defN 23-Jun-19 22:03 h2o/estimators/H2OEstimator.class
--rw-rw-r--  2.0 unx     1694 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
--rw-rw-r--  2.0 unx     1305 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
--rw-rw-r--  2.0 unx      112 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
-15 files, 9630 bytes uncompressed, 4315 bytes compressed:  55.2%
+Zip file size: 6333 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 h2o/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 h2o/estimators/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/preprocessing/h2o/
+-rw-rw-r--  2.0 unx      679 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     5710 b- defN 23-Jul-08 09:03 h2o/estimators/H2OEstimator.class
+-rw-rw-r--  2.0 unx     1694 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/h2o/H2OFrameConstructor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-h2o/
+-rw-rw-r--  2.0 unx     1305 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml
+-rw-rw-r--  2.0 unx      112 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties
+15 files, 9630 bytes uncompressed, 4317 bytes compressed:  55.2%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.30</version>
+    <version>1.7.31</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-h2o</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn H2O.ai converter</name>
   <description>JPMML Scikit-Learn H2O.ai to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-h2o/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Mon Jun 19 22:03:17 EEST 2023
-version=1.7.30
+#Sat Jul 08 09:03:24 EEST 2023
+version=1.7.31
 groupId=org.jpmml
 artifactId=pmml-sklearn-h2o
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-model-1.6.4.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-model-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-genmodel-3.40.0.4.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-genmodel-3.42.0.1.jar`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,361 +1,368 @@
-Zip file size: 432826 bytes, number of entries: 359
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-28 12:08 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/
--rw-r--r--  2.0 unx     1699 b- defN 23-Apr-28 12:08 hex/ModelCategory.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/
--rw-r--r--  2.0 unx      731 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/ModelDescriptor.class
--rw-r--r--  2.0 unx     3832 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/ModelDescriptorBuilder$PojoModelDescriptor.class
--rw-r--r--  2.0 unx      262 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/ModelDescriptorBuilder$1.class
--rw-r--r--  2.0 unx     1415 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/ModelDescriptorBuilder.class
--rw-r--r--  2.0 unx     4531 b- defN 23-Apr-28 12:08 hex/genmodel/descriptor/ModelDescriptorBuilder$MojoModelDescriptor.class
--rw-r--r--  2.0 unx     1088 b- defN 23-Apr-28 12:08 hex/genmodel/ModelMojoReader$RawValue.class
--rw-r--r--  2.0 unx     5067 b- defN 23-Apr-28 12:08 hex/genmodel/MojoReaderBackendFactory.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/easy/
--rw-r--r--  2.0 unx     2069 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumLimitedEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     1698 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumEncoder.class
--rw-r--r--  2.0 unx     1570 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EigenEncoder.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/
--rw-r--r--  2.0 unx      549 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/AutoEncoderModelPrediction.class
--rw-r--r--  2.0 unx      365 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/AbstractPrediction.class
--rw-r--r--  2.0 unx     1159 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/AnomalyDetectionPrediction.class
--rw-r--r--  2.0 unx      476 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/OrdinalModelPrediction.class
--rw-r--r--  2.0 unx      394 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/CoxPHModelPrediction.class
--rw-r--r--  2.0 unx      455 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/ClusteringModelPrediction.class
--rw-r--r--  2.0 unx      683 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/SortedClassProbability.class
--rw-r--r--  2.0 unx      606 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/MultinomialModelPrediction.class
--rw-r--r--  2.0 unx      479 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/Word2VecPrediction.class
--rw-r--r--  2.0 unx      665 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/BinomialModelPrediction.class
--rw-r--r--  2.0 unx      445 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/DimReductionModelPrediction.class
--rw-r--r--  2.0 unx      561 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/RegressionModelPrediction.class
--rw-r--r--  2.0 unx      414 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/TargetEncoderPrediction.class
--rw-r--r--  2.0 unx      430 b- defN 23-Apr-28 12:08 hex/genmodel/easy/prediction/KLimeModelPrediction.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/
--rw-r--r--  2.0 unx      454 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/PredictUnknownTypeException.class
--rw-r--r--  2.0 unx      683 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/PredictException.class
--rw-r--r--  2.0 unx      457 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/PredictNumberFormatException.class
--rw-r--r--  2.0 unx      475 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/PredictWrongModelCategoryException.class
--rw-r--r--  2.0 unx      831 b- defN 23-Apr-28 12:08 hex/genmodel/easy/exception/PredictUnknownCategoricalLevelException.class
--rw-r--r--  2.0 unx     1302 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumEncoderColumnMapper.class
--rw-r--r--  2.0 unx     1309 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EigenEncoderColumnMapper.class
--rw-r--r--  2.0 unx    23998 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EasyPredictModelWrapper.class
--rw-r--r--  2.0 unx     5805 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EasyPredictModelWrapper$Config.class
--rw-r--r--  2.0 unx      621 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumLimitedEncoderColumnMapper.class
--rw-r--r--  2.0 unx      241 b- defN 23-Apr-28 12:08 hex/genmodel/easy/CategoricalEncoder.class
--rw-r--r--  2.0 unx     5444 b- defN 23-Apr-28 12:08 hex/genmodel/easy/RowToRawDataConverter.class
--rw-r--r--  2.0 unx      363 b- defN 23-Apr-28 12:08 hex/genmodel/easy/RowData.class
--rw-r--r--  2.0 unx      597 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EasyPredictModelWrapper$ErrorConsumer.class
--rw-r--r--  2.0 unx     1939 b- defN 23-Apr-28 12:08 hex/genmodel/easy/LabelEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     1591 b- defN 23-Apr-28 12:08 hex/genmodel/easy/BinaryColumnMapper.class
--rw-r--r--  2.0 unx      872 b- defN 23-Apr-28 12:08 hex/genmodel/easy/DomainMapConstructor.class
--rw-r--r--  2.0 unx     1941 b- defN 23-Apr-28 12:08 hex/genmodel/easy/BinaryDomainMapConstructor.class
--rw-r--r--  2.0 unx     1570 b- defN 23-Apr-28 12:08 hex/genmodel/easy/OneHotEncoderColumnMapper.class
--rw-r--r--  2.0 unx     1962 b- defN 23-Apr-28 12:08 hex/genmodel/easy/OneHotEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     2357 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumLimitedEncoder.class
--rw-r--r--  2.0 unx     2209 b- defN 23-Apr-28 12:08 hex/genmodel/easy/OneHotEncoder.class
--rw-r--r--  2.0 unx     2290 b- defN 23-Apr-28 12:08 hex/genmodel/easy/BinaryEncoder.class
--rw-r--r--  2.0 unx     1633 b- defN 23-Apr-28 12:08 hex/genmodel/easy/LabelEncoder.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/easy/error/
--rw-r--r--  2.0 unx      805 b- defN 23-Apr-28 12:08 hex/genmodel/easy/error/VoidErrorConsumer.class
--rw-r--r--  2.0 unx      702 b- defN 23-Apr-28 12:08 hex/genmodel/easy/error/CountingErrorConsumer$Config.class
--rw-r--r--  2.0 unx     5332 b- defN 23-Apr-28 12:08 hex/genmodel/easy/error/CountingErrorConsumer.class
--rw-r--r--  2.0 unx     1269 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EasyPredictModelWrapper$1.class
--rw-r--r--  2.0 unx     1876 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EnumEncoderDomainMapConstructor.class
--rw-r--r--  2.0 unx     2146 b- defN 23-Apr-28 12:08 hex/genmodel/easy/EigenEncoderDomainMapConstructor.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/tools/
--rw-r--r--  2.0 unx     1287 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PrintMojo$FloatCastingSerializer.class
--rw-r--r--  2.0 unx     1026 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PredictCsv$1.class
--rw-r--r--  2.0 unx     5410 b- defN 23-Apr-28 12:08 hex/genmodel/tools/MungeCsv.class
--rw-r--r--  2.0 unx     1010 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PrintMojo$PrintTreeOptions.class
--rw-r--r--  2.0 unx    20777 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PredictCsv.class
--rw-r--r--  2.0 unx    14133 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PrintMojo.class
--rw-r--r--  2.0 unx     1286 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PredictCsv$PredictCsvCollection.class
--rw-r--r--  2.0 unx     4591 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PredictCsv$PredictCsvBuilder.class
--rw-r--r--  2.0 unx      826 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PrintMojo$2.class
--rw-r--r--  2.0 unx      722 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PrintMojo$1.class
--rw-r--r--  2.0 unx     7956 b- defN 23-Apr-28 12:08 hex/genmodel/tools/BuildPipeline.class
--rw-r--r--  2.0 unx     1294 b- defN 23-Apr-28 12:08 hex/genmodel/tools/PredictCsv$PredictCsvCallable.class
--rw-r--r--  2.0 unx     1202 b- defN 23-Apr-28 12:08 hex/genmodel/tools/MojoPrinter$Format.class
--rw-r--r--  2.0 unx      388 b- defN 23-Apr-28 12:08 hex/genmodel/tools/MojoPrinter.class
--rw-r--r--  2.0 unx      895 b- defN 23-Apr-28 12:08 hex/genmodel/ConverterFactoryProvidingModel.class
--rw-r--r--  2.0 unx     1538 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$6.class
--rw-r--r--  2.0 unx     2779 b- defN 23-Apr-28 12:08 hex/genmodel/MultiModelMojoReader.class
--rw-r--r--  2.0 unx     1583 b- defN 23-Apr-28 12:08 hex/genmodel/GenMunger$Step.class
--rw-r--r--  2.0 unx     1277 b- defN 23-Apr-28 12:08 hex/genmodel/GenModel$1.class
--rw-r--r--  2.0 unx     1403 b- defN 23-Apr-28 12:08 hex/genmodel/TmpMojoReaderBackend.class
--rw-r--r--  2.0 unx      215 b- defN 23-Apr-28 12:08 hex/genmodel/IClusteringModel.class
--rw-r--r--  2.0 unx     2445 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding.class
--rw-r--r--  2.0 unx     6310 b- defN 23-Apr-28 12:08 hex/genmodel/MojoPipelineBuilder.class
--rw-r--r--  2.0 unx     2276 b- defN 23-Apr-28 12:08 hex/genmodel/InMemoryMojoReaderBackend.class
--rw-r--r--  2.0 unx     5604 b- defN 23-Apr-28 12:08 hex/genmodel/MojoPipelineWriter.class
--rw-r--r--  2.0 unx     1729 b- defN 23-Apr-28 12:08 hex/genmodel/FolderMojoReaderBackend.class
--rw-r--r--  2.0 unx     1489 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$1.class
--rw-r--r--  2.0 unx      225 b- defN 23-Apr-28 12:08 hex/genmodel/PredictContributionsFactory.class
--rw-r--r--  2.0 unx      334 b- defN 23-Apr-28 12:08 hex/genmodel/PredictContributions.class
--rw-r--r--  2.0 unx     4315 b- defN 23-Apr-28 12:08 hex/genmodel/MojoPipelineWriter$MojoPipelineDescriptor.class
--rw-r--r--  2.0 unx      234 b- defN 23-Apr-28 12:08 hex/genmodel/MultiModelMojoReader$1.class
--rw-r--r--  2.0 unx     9766 b- defN 23-Apr-28 12:08 hex/genmodel/AbstractMojoWriter.class
--rw-r--r--  2.0 unx     2771 b- defN 23-Apr-28 12:08 hex/genmodel/MojoModel.class
--rw-r--r--  2.0 unx      228 b- defN 23-Apr-28 12:08 hex/genmodel/MojoPipelineWriter$1.class
--rw-r--r--  2.0 unx      345 b- defN 23-Apr-28 12:08 hex/genmodel/MojoReaderBackend.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/utils/
--rw-r--r--  2.0 unx     1366 b- defN 23-Apr-28 12:08 hex/genmodel/utils/StringEscapeUtils.class
--rw-r--r--  2.0 unx      770 b- defN 23-Apr-28 12:08 hex/genmodel/utils/IOUtils.class
--rw-r--r--  2.0 unx     7386 b- defN 23-Apr-28 12:08 hex/genmodel/utils/ArrayUtils.class
--rw-r--r--  2.0 unx     3399 b- defN 23-Apr-28 12:08 hex/genmodel/utils/ParseUtils.class
--rw-r--r--  2.0 unx     1869 b- defN 23-Apr-28 12:08 hex/genmodel/utils/ByteBufferWrapper.class
--rw-r--r--  2.0 unx     1329 b- defN 23-Apr-28 12:08 hex/genmodel/utils/MathUtils.class
--rw-r--r--  2.0 unx      988 b- defN 23-Apr-28 12:08 hex/genmodel/utils/ArrayUtils$1.class
--rw-r--r--  2.0 unx     1361 b- defN 23-Apr-28 12:08 hex/genmodel/utils/LinkFunctionType.class
--rw-r--r--  2.0 unx     1862 b- defN 23-Apr-28 12:08 hex/genmodel/utils/DistributionFamily.class
--rw-r--r--  2.0 unx     3320 b- defN 23-Apr-28 12:08 hex/genmodel/utils/GenmodelBitSet.class
--rw-r--r--  2.0 unx     1206 b- defN 23-Apr-28 12:08 hex/genmodel/utils/ArrayUtils$2.class
--rw-r--r--  2.0 unx     1234 b- defN 23-Apr-28 12:08 hex/genmodel/MojoReaderBackendFactory$CachingStrategy.class
--rw-r--r--  2.0 unx     7590 b- defN 23-Apr-28 12:08 hex/genmodel/GenMunger.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/annotations/
--rw-r--r--  2.0 unx      521 b- defN 23-Apr-28 12:08 hex/genmodel/annotations/ModelPojo.class
--rw-r--r--  2.0 unx     1527 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$3.class
--rw-r--r--  2.0 unx      398 b- defN 23-Apr-28 12:08 hex/genmodel/IGenModel.class
--rw-r--r--  2.0 unx     1539 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$5.class
--rw-r--r--  2.0 unx     1268 b- defN 23-Apr-28 12:08 hex/genmodel/NestedMojoReaderBackend.class
--rw-r--r--  2.0 unx    14911 b- defN 23-Apr-28 12:08 hex/genmodel/ModelMojoReader.class
--rw-r--r--  2.0 unx     2041 b- defN 23-Apr-28 12:08 hex/genmodel/ZipfileMojoReaderBackend.class
--rw-r--r--  2.0 unx    18923 b- defN 23-Apr-28 12:08 hex/genmodel/GenModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/svm/
--rw-r--r--  2.0 unx     1887 b- defN 23-Apr-28 12:08 hex/genmodel/algos/svm/SvmMojoReader.class
--rw-r--r--  2.0 unx     1340 b- defN 23-Apr-28 12:08 hex/genmodel/algos/svm/SvmMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/klime/
--rw-r--r--  2.0 unx     2319 b- defN 23-Apr-28 12:08 hex/genmodel/algos/klime/KLimeMojoModel.class
--rw-r--r--  2.0 unx     2687 b- defN 23-Apr-28 12:08 hex/genmodel/algos/klime/KLimeMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/word2vec/
--rw-r--r--  2.0 unx     1490 b- defN 23-Apr-28 12:08 hex/genmodel/algos/word2vec/Word2VecMojoModel.class
--rw-r--r--  2.0 unx     3174 b- defN 23-Apr-28 12:08 hex/genmodel/algos/word2vec/Word2VecMojoReader.class
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-28 12:08 hex/genmodel/algos/word2vec/WordEmbeddingModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/
--rw-r--r--  2.0 unx      863 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/MojoRule.class
--rw-r--r--  2.0 unx     1620 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/MojoCondition.class
--rw-r--r--  2.0 unx     2502 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/RuleFitMojoModel.class
--rw-r--r--  2.0 unx     7385 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/RuleFitMojoReader.class
--rw-r--r--  2.0 unx     3386 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/MojoRuleEnsemble.class
--rw-r--r--  2.0 unx     1177 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/MojoCondition$Type.class
--rw-r--r--  2.0 unx     1286 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/RuleFitMojoModel$ModelType.class
--rw-r--r--  2.0 unx     1256 b- defN 23-Apr-28 12:08 hex/genmodel/algos/rulefit/MojoCondition$Operator.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/
--rw-r--r--  2.0 unx      263 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAPPredictor$Workspace.class
--rw-r--r--  2.0 unx     3299 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfoLightReader.class
--rw-r--r--  2.0 unx      880 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAP$PathElement.class
--rw-r--r--  2.0 unx     4714 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoReader.class
--rw-r--r--  2.0 unx      353 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeGraphConverter.class
--rw-r--r--  2.0 unx      657 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreTree0.class
--rw-r--r--  2.0 unx      202 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreTree.class
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAP$1.class
--rw-r--r--  2.0 unx      635 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreTree2.class
--rw-r--r--  2.0 unx     1101 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ConvertTreeOptions.class
--rw-r--r--  2.0 unx     8018 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeSubgraph.class
--rw-r--r--  2.0 unx     2998 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAPEnsemble.class
--rw-r--r--  2.0 unx     8370 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAP.class
--rw-r--r--  2.0 unx      253 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$1.class
--rw-r--r--  2.0 unx      535 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafNodeAssignments.class
--rw-r--r--  2.0 unx      438 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$DecisionPathTracker.class
--rw-r--r--  2.0 unx     2835 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions.class
--rw-r--r--  2.0 unx      657 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreTree1.class
--rw-r--r--  2.0 unx      712 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAPPredictor.class
--rw-r--r--  2.0 unx    16477 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeNode.class
--rw-r--r--  2.0 unx     1175 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/CalibrationMojoHelper.class
--rw-r--r--  2.0 unx     2634 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ContributionComposer.class
--rw-r--r--  2.0 unx      602 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreIsolationTree0.class
--rw-r--r--  2.0 unx     1395 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/NaSplitDir.class
--rw-r--r--  2.0 unx     3003 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafDecisionPathTracker.class
--rw-r--r--  2.0 unx      611 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeBackedMojoModel.class
--rw-r--r--  2.0 unx     3699 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeGraph.class
--rw-r--r--  2.0 unx    24842 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel.class
--rw-r--r--  2.0 unx     1518 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions$SharedTreeContributionsPredictor.class
--rw-r--r--  2.0 unx     1707 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/TreeSHAP$PathPointer.class
--rw-r--r--  2.0 unx      199 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ScoreIsolationTree.class
--rw-r--r--  2.0 unx     1445 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$StringDecisionPathTracker.class
--rw-r--r--  2.0 unx      399 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/CalibrationMojoHelper$MojoModelWithCalibration.class
--rw-r--r--  2.0 unx     3805 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/ContributionsPredictor.class
--rw-r--r--  2.0 unx     2632 b- defN 23-Apr-28 12:08 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfo.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/coxph/
--rw-r--r--  2.0 unx     3758 b- defN 23-Apr-28 12:08 hex/genmodel/algos/coxph/CoxPHMojoModel.class
--rw-r--r--  2.0 unx     1144 b- defN 23-Apr-28 12:08 hex/genmodel/algos/coxph/CoxPHMojoModel$Strata.class
--rw-r--r--  2.0 unx     3613 b- defN 23-Apr-28 12:08 hex/genmodel/algos/coxph/CoxPHMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/drf/
--rw-r--r--  2.0 unx     1633 b- defN 23-Apr-28 12:08 hex/genmodel/algos/drf/DrfMojoReader.class
--rw-r--r--  2.0 unx      230 b- defN 23-Apr-28 12:08 hex/genmodel/algos/drf/DrfMojoModel$1.class
--rw-r--r--  2.0 unx     3129 b- defN 23-Apr-28 12:08 hex/genmodel/algos/drf/DrfMojoModel$ContributionsPredictorDRF.class
--rw-r--r--  2.0 unx     2700 b- defN 23-Apr-28 12:08 hex/genmodel/algos/drf/DrfMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isoforextended/
--rw-r--r--  2.0 unx     4170 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoModel.class
--rw-r--r--  2.0 unx     2306 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pca/
--rw-r--r--  2.0 unx     2645 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pca/PCAMojoModel.class
--rw-r--r--  2.0 unx     2819 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pca/PCAMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/
--rw-r--r--  2.0 unx     4318 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel.class
--rw-r--r--  2.0 unx     2466 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMultinomialMojoModel.class
--rw-r--r--  2.0 unx     1747 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModelBase.class
--rw-r--r--  2.0 unx      848 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_inverseInv.class
--rw-r--r--  2.0 unx      851 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_identityInv.class
--rw-r--r--  2.0 unx      230 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$1.class
--rw-r--r--  2.0 unx     2647 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmOrdinalMojoModel.class
--rw-r--r--  2.0 unx      836 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_logInv.class
--rw-r--r--  2.0 unx      626 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_ologitInv.class
--rw-r--r--  2.0 unx      272 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$Function1.class
--rw-r--r--  2.0 unx      724 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_tweedieInv.class
--rw-r--r--  2.0 unx      842 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoModel$GLM_logitInv.class
--rw-r--r--  2.0 unx     3584 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glm/GlmMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/
--rw-r--r--  2.0 unx      677 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/ColumnsMapping.class
--rw-r--r--  2.0 unx     3493 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/EncodingMap.class
--rw-r--r--  2.0 unx     9375 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/TargetEncoderMojoReader.class
--rw-r--r--  2.0 unx     2436 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/EncodingMaps.class
--rw-r--r--  2.0 unx     1417 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/ColumnsToSingleMapping.class
--rw-r--r--  2.0 unx     8265 b- defN 23-Apr-28 12:08 hex/genmodel/algos/targetencoder/TargetEncoderMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isotonic/
--rw-r--r--  2.0 unx      888 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isotonic/IsotonicCalibrator.class
--rw-r--r--  2.0 unx      874 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isotonic/IsotonicRegressionMojoModel.class
--rw-r--r--  2.0 unx     1676 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isotonic/IsotonicRegressionMojoReader.class
--rw-r--r--  2.0 unx     1680 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isotonic/IsotonicRegressionUtils.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/
--rw-r--r--  2.0 unx      783 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierDropoutOut.class
--rw-r--r--  2.0 unx     5224 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/DeeplearningMojoReader.class
--rw-r--r--  2.0 unx     1081 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$SoftmaxOut.class
--rw-r--r--  2.0 unx      769 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutDropoutOut.class
--rw-r--r--  2.0 unx      709 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$LinearOut.class
--rw-r--r--  2.0 unx     1096 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$1.class
--rw-r--r--  2.0 unx     6719 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/NeuralNetwork.class
--rw-r--r--  2.0 unx      934 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierOut.class
--rw-r--r--  2.0 unx      323 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$ActivationFunctions.class
--rw-r--r--  2.0 unx     2132 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils.class
--rw-r--r--  2.0 unx      798 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierDropoutOut.class
--rw-r--r--  2.0 unx      663 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$StoreWeightsBias.class
--rw-r--r--  2.0 unx     6843 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/DeeplearningMojoModel.class
--rw-r--r--  2.0 unx      787 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$TanhDropoutOut.class
--rw-r--r--  2.0 unx      995 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierOut.class
--rw-r--r--  2.0 unx      922 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$TanhOut.class
--rw-r--r--  2.0 unx     1007 b- defN 23-Apr-28 12:08 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutOut.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/
--rw-r--r--  2.0 unx      196 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/SupportVectorScorer.class
--rw-r--r--  2.0 unx      422 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/KernelParameters.class
--rw-r--r--  2.0 unx     1388 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/ScorerFactory.class
--rw-r--r--  2.0 unx     1550 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/GaussianScorer.class
--rw-r--r--  2.0 unx      973 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/KernelType.class
--rw-r--r--  2.0 unx      699 b- defN 23-Apr-28 12:08 hex/genmodel/algos/psvm/ScorerFactory$1.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/ensemble/
--rw-r--r--  2.0 unx     3993 b- defN 23-Apr-28 12:08 hex/genmodel/algos/ensemble/StackedEnsembleMojoReader.class
--rw-r--r--  2.0 unx      974 b- defN 23-Apr-28 12:08 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel$StackedEnsembleMojoSubModel.class
--rw-r--r--  2.0 unx     2165 b- defN 23-Apr-28 12:08 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isofor/
--rw-r--r--  2.0 unx     1835 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isofor/IsolationForestMojoModel.class
--rw-r--r--  2.0 unx     2021 b- defN 23-Apr-28 12:08 hex/genmodel/algos/isofor/IsolationForestMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/
--rw-r--r--  2.0 unx     1572 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamMojoModel.class
--rw-r--r--  2.0 unx     2046 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/ISplines.class
--rw-r--r--  2.0 unx     2045 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/NBSplinesTypeII.class
--rw-r--r--  2.0 unx    10957 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamMojoReader.class
--rw-r--r--  2.0 unx     1717 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/NBSplinesTypeI$MSplineBasis.class
--rw-r--r--  2.0 unx      855 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/ISplines$ISplineBasis.class
--rw-r--r--  2.0 unx     1902 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/NBSplinesTypeII$BSplineBasis.class
--rw-r--r--  2.0 unx     3495 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/NBSplinesTypeI.class
--rw-r--r--  2.0 unx     2061 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamUtilsThinPlateRegression.class
--rw-r--r--  2.0 unx    11583 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamMojoModelBase.class
--rw-r--r--  2.0 unx     1347 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/MSplines.class
--rw-r--r--  2.0 unx     4489 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamUtilsISplines.class
--rw-r--r--  2.0 unx      896 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamMojoModelBase$1.class
--rw-r--r--  2.0 unx     2234 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamMojoMultinomialModel.class
--rw-r--r--  2.0 unx     1977 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamRowToRawDataConverter.class
--rw-r--r--  2.0 unx     2518 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gam/GamUtilsCubicRegression.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pipeline/
--rw-r--r--  2.0 unx     1732 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pipeline/MojoPipeline.class
--rw-r--r--  2.0 unx     6799 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pipeline/MojoPipelineReader.class
--rw-r--r--  2.0 unx      635 b- defN 23-Apr-28 12:08 hex/genmodel/algos/pipeline/MojoPipeline$PipelineSubModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/kmeans/
--rw-r--r--  2.0 unx     1339 b- defN 23-Apr-28 12:08 hex/genmodel/algos/kmeans/KMeansMojoModel.class
--rw-r--r--  2.0 unx     2248 b- defN 23-Apr-28 12:08 hex/genmodel/algos/kmeans/KMeansMojoReader.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gbm/
--rw-r--r--  2.0 unx     4006 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gbm/GbmMojoModel.class
--rw-r--r--  2.0 unx     2104 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gbm/GbmMojoReader.class
--rw-r--r--  2.0 unx      981 b- defN 23-Apr-28 12:08 hex/genmodel/algos/gbm/GbmMojoModel$1.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/
--rw-r--r--  2.0 unx     1345 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$3.class
--rw-r--r--  2.0 unx     4904 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmMojoReader.class
--rw-r--r--  2.0 unx     1567 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$5.class
--rw-r--r--  2.0 unx     2161 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$8.class
--rw-r--r--  2.0 unx     1232 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$2.class
--rw-r--r--  2.0 unx     1980 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$8.class
--rw-r--r--  2.0 unx      875 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$1.class
--rw-r--r--  2.0 unx     2578 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer.class
--rw-r--r--  2.0 unx     1219 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmInitialization.class
--rw-r--r--  2.0 unx     1075 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$2.class
--rw-r--r--  2.0 unx     2236 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$9.class
--rw-r--r--  2.0 unx     1512 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$6.class
--rw-r--r--  2.0 unx     1186 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$3.class
--rw-r--r--  2.0 unx     1290 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$4.class
--rw-r--r--  2.0 unx     1406 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$7.class
--rw-r--r--  2.0 unx     9537 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmMojoModel.class
--rw-r--r--  2.0 unx     1280 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$5.class
--rw-r--r--  2.0 unx      983 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$1.class
--rw-r--r--  2.0 unx     1510 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$7.class
--rw-r--r--  2.0 unx     1460 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmRegularizer$6.class
--rw-r--r--  2.0 unx     3178 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss.class
--rw-r--r--  2.0 unx     1499 b- defN 23-Apr-28 12:08 hex/genmodel/algos/glrm/GlrmLoss$4.class
--rw-r--r--  2.0 unx     1100 b- defN 23-Apr-28 12:08 hex/genmodel/ModelMojoReader$1.class
--rw-r--r--  2.0 unx      855 b- defN 23-Apr-28 12:08 hex/genmodel/MojoReaderBackendFactory$1.class
--rw-r--r--  2.0 unx     1934 b- defN 23-Apr-28 12:08 hex/genmodel/MultiModelMojoReader$NestedMojoReaderBackend.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/
--rw-r--r--  2.0 unx     1045 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/SharedTreeModelAttributes.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/
--rw-r--r--  2.0 unx      773 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinalGLM.class
--rw-r--r--  2.0 unx      420 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsSupervised.class
--rw-r--r--  2.0 unx      590 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsRegression.class
--rw-r--r--  2.0 unx      777 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsBinomialGLM.class
--rw-r--r--  2.0 unx      449 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsAnomaly.class
--rw-r--r--  2.0 unx      630 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetrics.class
--rw-r--r--  2.0 unx      748 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinal.class
--rw-r--r--  2.0 unx      860 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsBinomial.class
--rw-r--r--  2.0 unx      860 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomial.class
--rw-r--r--  2.0 unx      785 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionGLM.class
--rw-r--r--  2.0 unx      789 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomialGLM.class
--rw-r--r--  2.0 unx      517 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionCoxPH.class
--rw-r--r--  2.0 unx      993 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/DeepLearningModelAttributes.class
--rw-r--r--  2.0 unx     5653 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelAttributes.class
--rw-r--r--  2.0 unx     1267 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/VariableImportances$1.class
--rw-r--r--  2.0 unx      495 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/SerializedName.class
--rw-r--r--  2.0 unx     2602 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/VariableImportances.class
--rw-r--r--  2.0 unx     1676 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/Table$ColumnType.class
--rw-r--r--  2.0 unx     1155 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelAttributes$1.class
--rw-r--r--  2.0 unx     3376 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/Table.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/
--rw-r--r--  2.0 unx      874 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/ColumnSpecifier.class
--rw-r--r--  2.0 unx      249 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/VariableImportancesHolder.class
--rw-r--r--  2.0 unx      953 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/KeyValue.class
--rw-r--r--  2.0 unx     1892 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/ModelParameter.class
--rw-r--r--  2.0 unx     1319 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/ParameterKey$Type.class
--rw-r--r--  2.0 unx      880 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/FeatureContribution.class
--rw-r--r--  2.0 unx     1176 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/ParameterKey.class
--rw-r--r--  2.0 unx     1263 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/parameters/StringPair.class
--rw-r--r--  2.0 unx     1768 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelJsonReader$1.class
--rw-r--r--  2.0 unx     2522 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelJsonReader$TypeHint.class
--rw-r--r--  2.0 unx     1234 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelAttributesGLM.class
--rw-r--r--  2.0 unx    15710 b- defN 23-Apr-28 12:08 hex/genmodel/attributes/ModelJsonReader.class
--rw-r--r--  2.0 unx     1541 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$2.class
--rw-r--r--  2.0 unx     1551 b- defN 23-Apr-28 12:08 hex/genmodel/CategoricalEncoding$4.class
--rw-r--r--  2.0 unx     1127 b- defN 23-Apr-28 12:08 hex/genmodel/MojoPipelineBuilder$MappingSpec.class
--rw-r--r--  2.0 unx     5010 b- defN 23-Apr-28 12:08 hex/genmodel/ModelMojoFactory.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 water/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 water/util/
--rw-r--r--  2.0 unx    10148 b- defN 23-Apr-28 12:08 water/util/H2OPredictor.class
--rw-r--r--  2.0 unx      606 b- defN 23-Apr-28 12:08 water/util/H2OPredictor$1.class
--rw-r--r--  2.0 unx     2742 b- defN 23-Apr-28 12:08 water/util/JavaVersionUtils.class
--rw-r--r--  2.0 unx      971 b- defN 23-Apr-28 12:08 water/util/ModelUtils.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 water/genmodel/
--rw-r--r--  2.0 unx      873 b- defN 23-Apr-28 12:08 water/genmodel/AbstractBuildVersion$1.class
--rw-r--r--  2.0 unx     2965 b- defN 23-Apr-28 12:08 water/genmodel/AbstractBuildVersion.class
--rw-r--r--  2.0 unx      922 b- defN 23-Apr-28 12:08 water/genmodel/BuildVersion.class
--rw-r--r--  2.0 unx      921 b- defN 23-Apr-28 12:08 water/genmodel/IGeneratedModel.class
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 META-INF/services/
--rw-r--r--  2.0 unx       29 b- defN 23-Apr-28 12:08 META-INF/services/hex.genmodel.tools.MojoPrinter
-359 files, 759160 bytes uncompressed, 372212 bytes compressed:  51.0%
+Zip file size: 442644 bytes, number of entries: 366
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:49 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-20 17:49 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/
+-rw-r--r--  2.0 unx     1699 b- defN 23-Jun-20 17:48 hex/ModelCategory.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/descriptor/
+-rw-r--r--  2.0 unx      731 b- defN 23-Jun-20 17:48 hex/genmodel/descriptor/ModelDescriptor.class
+-rw-r--r--  2.0 unx     3832 b- defN 23-Jun-20 17:48 hex/genmodel/descriptor/ModelDescriptorBuilder$PojoModelDescriptor.class
+-rw-r--r--  2.0 unx      262 b- defN 23-Jun-20 17:48 hex/genmodel/descriptor/ModelDescriptorBuilder$1.class
+-rw-r--r--  2.0 unx     1415 b- defN 23-Jun-20 17:48 hex/genmodel/descriptor/ModelDescriptorBuilder.class
+-rw-r--r--  2.0 unx     4531 b- defN 23-Jun-20 17:48 hex/genmodel/descriptor/ModelDescriptorBuilder$MojoModelDescriptor.class
+-rw-r--r--  2.0 unx     1088 b- defN 23-Jun-20 17:48 hex/genmodel/ModelMojoReader$RawValue.class
+-rw-r--r--  2.0 unx     5067 b- defN 23-Jun-20 17:48 hex/genmodel/MojoReaderBackendFactory.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/easy/
+-rw-r--r--  2.0 unx     2069 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EnumLimitedEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     1698 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EnumEncoder.class
+-rw-r--r--  2.0 unx     1570 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EigenEncoder.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/
+-rw-r--r--  2.0 unx      549 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/AutoEncoderModelPrediction.class
+-rw-r--r--  2.0 unx      365 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/AbstractPrediction.class
+-rw-r--r--  2.0 unx     1159 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/AnomalyDetectionPrediction.class
+-rw-r--r--  2.0 unx      476 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/OrdinalModelPrediction.class
+-rw-r--r--  2.0 unx      394 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/CoxPHModelPrediction.class
+-rw-r--r--  2.0 unx      455 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/ClusteringModelPrediction.class
+-rw-r--r--  2.0 unx      683 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/SortedClassProbability.class
+-rw-r--r--  2.0 unx      606 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/MultinomialModelPrediction.class
+-rw-r--r--  2.0 unx      479 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/Word2VecPrediction.class
+-rw-r--r--  2.0 unx      665 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/BinomialModelPrediction.class
+-rw-r--r--  2.0 unx      445 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/DimReductionModelPrediction.class
+-rw-r--r--  2.0 unx      561 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/RegressionModelPrediction.class
+-rw-r--r--  2.0 unx      414 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/TargetEncoderPrediction.class
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-20 17:48 hex/genmodel/easy/prediction/KLimeModelPrediction.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/easy/exception/
+-rw-r--r--  2.0 unx      454 b- defN 23-Jun-20 17:48 hex/genmodel/easy/exception/PredictUnknownTypeException.class
+-rw-r--r--  2.0 unx      683 b- defN 23-Jun-20 17:48 hex/genmodel/easy/exception/PredictException.class
+-rw-r--r--  2.0 unx      457 b- defN 23-Jun-20 17:48 hex/genmodel/easy/exception/PredictNumberFormatException.class
+-rw-r--r--  2.0 unx      475 b- defN 23-Jun-20 17:48 hex/genmodel/easy/exception/PredictWrongModelCategoryException.class
+-rw-r--r--  2.0 unx      831 b- defN 23-Jun-20 17:48 hex/genmodel/easy/exception/PredictUnknownCategoricalLevelException.class
+-rw-r--r--  2.0 unx     1302 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EnumEncoderColumnMapper.class
+-rw-r--r--  2.0 unx     1309 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EigenEncoderColumnMapper.class
+-rw-r--r--  2.0 unx    23998 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EasyPredictModelWrapper.class
+-rw-r--r--  2.0 unx     5805 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EasyPredictModelWrapper$Config.class
+-rw-r--r--  2.0 unx      621 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EnumLimitedEncoderColumnMapper.class
+-rw-r--r--  2.0 unx      241 b- defN 23-Jun-20 17:48 hex/genmodel/easy/CategoricalEncoder.class
+-rw-r--r--  2.0 unx     5444 b- defN 23-Jun-20 17:48 hex/genmodel/easy/RowToRawDataConverter.class
+-rw-r--r--  2.0 unx      363 b- defN 23-Jun-20 17:48 hex/genmodel/easy/RowData.class
+-rw-r--r--  2.0 unx      597 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EasyPredictModelWrapper$ErrorConsumer.class
+-rw-r--r--  2.0 unx     1939 b- defN 23-Jun-20 17:48 hex/genmodel/easy/LabelEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     1591 b- defN 23-Jun-20 17:48 hex/genmodel/easy/BinaryColumnMapper.class
+-rw-r--r--  2.0 unx      872 b- defN 23-Jun-20 17:48 hex/genmodel/easy/DomainMapConstructor.class
+-rw-r--r--  2.0 unx     1941 b- defN 23-Jun-20 17:48 hex/genmodel/easy/BinaryDomainMapConstructor.class
+-rw-r--r--  2.0 unx     1570 b- defN 23-Jun-20 17:48 hex/genmodel/easy/OneHotEncoderColumnMapper.class
+-rw-r--r--  2.0 unx     1962 b- defN 23-Jun-20 17:48 hex/genmodel/easy/OneHotEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     2357 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EnumLimitedEncoder.class
+-rw-r--r--  2.0 unx     2209 b- defN 23-Jun-20 17:48 hex/genmodel/easy/OneHotEncoder.class
+-rw-r--r--  2.0 unx     2290 b- defN 23-Jun-20 17:48 hex/genmodel/easy/BinaryEncoder.class
+-rw-r--r--  2.0 unx     1633 b- defN 23-Jun-20 17:48 hex/genmodel/easy/LabelEncoder.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/easy/error/
+-rw-r--r--  2.0 unx      805 b- defN 23-Jun-20 17:48 hex/genmodel/easy/error/VoidErrorConsumer.class
+-rw-r--r--  2.0 unx      702 b- defN 23-Jun-20 17:48 hex/genmodel/easy/error/CountingErrorConsumer$Config.class
+-rw-r--r--  2.0 unx     5332 b- defN 23-Jun-20 17:48 hex/genmodel/easy/error/CountingErrorConsumer.class
+-rw-r--r--  2.0 unx     1269 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EasyPredictModelWrapper$1.class
+-rw-r--r--  2.0 unx     1876 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EnumEncoderDomainMapConstructor.class
+-rw-r--r--  2.0 unx     2146 b- defN 23-Jun-20 17:48 hex/genmodel/easy/EigenEncoderDomainMapConstructor.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/tools/
+-rw-r--r--  2.0 unx     1287 b- defN 23-Jun-20 17:48 hex/genmodel/tools/PrintMojo$FloatCastingSerializer.class
+-rw-r--r--  2.0 unx     1026 b- defN 23-Jun-20 17:48 hex/genmodel/tools/PredictCsv$1.class
+-rw-r--r--  2.0 unx     5410 b- defN 23-Jun-20 17:48 hex/genmodel/tools/MungeCsv.class
+-rw-r--r--  2.0 unx     1010 b- defN 23-Jun-20 17:48 hex/genmodel/tools/PrintMojo$PrintTreeOptions.class
+-rw-r--r--  2.0 unx    20777 b- defN 23-Jun-20 17:48 hex/genmodel/tools/PredictCsv.class
+-rw-r--r--  2.0 unx    14133 b- defN 23-Jun-20 17:48 hex/genmodel/tools/PrintMojo.class
+-rw-r--r--  2.0 unx     1286 b- defN 23-Jun-20 17:48 hex/genmodel/tools/PredictCsv$PredictCsvCollection.class
+-rw-r--r--  2.0 unx     4591 b- defN 23-Jun-20 17:48 hex/genmodel/tools/PredictCsv$PredictCsvBuilder.class
+-rw-r--r--  2.0 unx      826 b- defN 23-Jun-20 17:48 hex/genmodel/tools/PrintMojo$2.class
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-20 17:48 hex/genmodel/tools/PrintMojo$1.class
+-rw-r--r--  2.0 unx     7956 b- defN 23-Jun-20 17:48 hex/genmodel/tools/BuildPipeline.class
+-rw-r--r--  2.0 unx     1294 b- defN 23-Jun-20 17:48 hex/genmodel/tools/PredictCsv$PredictCsvCallable.class
+-rw-r--r--  2.0 unx     1202 b- defN 23-Jun-20 17:48 hex/genmodel/tools/MojoPrinter$Format.class
+-rw-r--r--  2.0 unx      388 b- defN 23-Jun-20 17:48 hex/genmodel/tools/MojoPrinter.class
+-rw-r--r--  2.0 unx      895 b- defN 23-Jun-20 17:48 hex/genmodel/ConverterFactoryProvidingModel.class
+-rw-r--r--  2.0 unx     1538 b- defN 23-Jun-20 17:48 hex/genmodel/CategoricalEncoding$6.class
+-rw-r--r--  2.0 unx     2779 b- defN 23-Jun-20 17:48 hex/genmodel/MultiModelMojoReader.class
+-rw-r--r--  2.0 unx     1583 b- defN 23-Jun-20 17:48 hex/genmodel/GenMunger$Step.class
+-rw-r--r--  2.0 unx     1277 b- defN 23-Jun-20 17:48 hex/genmodel/GenModel$1.class
+-rw-r--r--  2.0 unx     1403 b- defN 23-Jun-20 17:48 hex/genmodel/TmpMojoReaderBackend.class
+-rw-r--r--  2.0 unx      215 b- defN 23-Jun-20 17:48 hex/genmodel/IClusteringModel.class
+-rw-r--r--  2.0 unx     2445 b- defN 23-Jun-20 17:48 hex/genmodel/CategoricalEncoding.class
+-rw-r--r--  2.0 unx     6310 b- defN 23-Jun-20 17:48 hex/genmodel/MojoPipelineBuilder.class
+-rw-r--r--  2.0 unx     2276 b- defN 23-Jun-20 17:48 hex/genmodel/InMemoryMojoReaderBackend.class
+-rw-r--r--  2.0 unx     5604 b- defN 23-Jun-20 17:48 hex/genmodel/MojoPipelineWriter.class
+-rw-r--r--  2.0 unx     1729 b- defN 23-Jun-20 17:48 hex/genmodel/FolderMojoReaderBackend.class
+-rw-r--r--  2.0 unx     1489 b- defN 23-Jun-20 17:48 hex/genmodel/CategoricalEncoding$1.class
+-rw-r--r--  2.0 unx      225 b- defN 23-Jun-20 17:48 hex/genmodel/PredictContributionsFactory.class
+-rw-r--r--  2.0 unx      334 b- defN 23-Jun-20 17:48 hex/genmodel/PredictContributions.class
+-rw-r--r--  2.0 unx     4315 b- defN 23-Jun-20 17:48 hex/genmodel/MojoPipelineWriter$MojoPipelineDescriptor.class
+-rw-r--r--  2.0 unx      234 b- defN 23-Jun-20 17:48 hex/genmodel/MultiModelMojoReader$1.class
+-rw-r--r--  2.0 unx     9766 b- defN 23-Jun-20 17:48 hex/genmodel/AbstractMojoWriter.class
+-rw-r--r--  2.0 unx     2771 b- defN 23-Jun-20 17:48 hex/genmodel/MojoModel.class
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-20 17:48 hex/genmodel/MojoPipelineWriter$1.class
+-rw-r--r--  2.0 unx      345 b- defN 23-Jun-20 17:48 hex/genmodel/MojoReaderBackend.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/utils/
+-rw-r--r--  2.0 unx     1366 b- defN 23-Jun-20 17:48 hex/genmodel/utils/StringEscapeUtils.class
+-rw-r--r--  2.0 unx      770 b- defN 23-Jun-20 17:48 hex/genmodel/utils/IOUtils.class
+-rw-r--r--  2.0 unx     7386 b- defN 23-Jun-20 17:48 hex/genmodel/utils/ArrayUtils.class
+-rw-r--r--  2.0 unx     3399 b- defN 23-Jun-20 17:48 hex/genmodel/utils/ParseUtils.class
+-rw-r--r--  2.0 unx     1869 b- defN 23-Jun-20 17:48 hex/genmodel/utils/ByteBufferWrapper.class
+-rw-r--r--  2.0 unx     1329 b- defN 23-Jun-20 17:48 hex/genmodel/utils/MathUtils.class
+-rw-r--r--  2.0 unx      988 b- defN 23-Jun-20 17:48 hex/genmodel/utils/ArrayUtils$1.class
+-rw-r--r--  2.0 unx     1361 b- defN 23-Jun-20 17:48 hex/genmodel/utils/LinkFunctionType.class
+-rw-r--r--  2.0 unx     1862 b- defN 23-Jun-20 17:48 hex/genmodel/utils/DistributionFamily.class
+-rw-r--r--  2.0 unx     3320 b- defN 23-Jun-20 17:48 hex/genmodel/utils/GenmodelBitSet.class
+-rw-r--r--  2.0 unx     1206 b- defN 23-Jun-20 17:48 hex/genmodel/utils/ArrayUtils$2.class
+-rw-r--r--  2.0 unx     1234 b- defN 23-Jun-20 17:48 hex/genmodel/MojoReaderBackendFactory$CachingStrategy.class
+-rw-r--r--  2.0 unx     8569 b- defN 23-Jun-20 17:48 hex/genmodel/GenMunger.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/annotations/
+-rw-r--r--  2.0 unx      521 b- defN 23-Jun-20 17:48 hex/genmodel/annotations/ModelPojo.class
+-rw-r--r--  2.0 unx     1527 b- defN 23-Jun-20 17:48 hex/genmodel/CategoricalEncoding$3.class
+-rw-r--r--  2.0 unx      398 b- defN 23-Jun-20 17:48 hex/genmodel/IGenModel.class
+-rw-r--r--  2.0 unx     1539 b- defN 23-Jun-20 17:48 hex/genmodel/CategoricalEncoding$5.class
+-rw-r--r--  2.0 unx     1268 b- defN 23-Jun-20 17:48 hex/genmodel/NestedMojoReaderBackend.class
+-rw-r--r--  2.0 unx    15247 b- defN 23-Jun-20 17:48 hex/genmodel/ModelMojoReader.class
+-rw-r--r--  2.0 unx     2041 b- defN 23-Jun-20 17:48 hex/genmodel/ZipfileMojoReaderBackend.class
+-rw-r--r--  2.0 unx    18923 b- defN 23-Jun-20 17:48 hex/genmodel/GenModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/svm/
+-rw-r--r--  2.0 unx     1887 b- defN 23-Jun-20 17:48 hex/genmodel/algos/svm/SvmMojoReader.class
+-rw-r--r--  2.0 unx     1340 b- defN 23-Jun-20 17:48 hex/genmodel/algos/svm/SvmMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/klime/
+-rw-r--r--  2.0 unx     2319 b- defN 23-Jun-20 17:48 hex/genmodel/algos/klime/KLimeMojoModel.class
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jun-20 17:48 hex/genmodel/algos/klime/KLimeMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/word2vec/
+-rw-r--r--  2.0 unx     1490 b- defN 23-Jun-20 17:48 hex/genmodel/algos/word2vec/Word2VecMojoModel.class
+-rw-r--r--  2.0 unx     3174 b- defN 23-Jun-20 17:48 hex/genmodel/algos/word2vec/Word2VecMojoReader.class
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-20 17:48 hex/genmodel/algos/word2vec/WordEmbeddingModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/rulefit/
+-rw-r--r--  2.0 unx      863 b- defN 23-Jun-20 17:48 hex/genmodel/algos/rulefit/MojoRule.class
+-rw-r--r--  2.0 unx     1620 b- defN 23-Jun-20 17:48 hex/genmodel/algos/rulefit/MojoCondition.class
+-rw-r--r--  2.0 unx     2502 b- defN 23-Jun-20 17:48 hex/genmodel/algos/rulefit/RuleFitMojoModel.class
+-rw-r--r--  2.0 unx     7385 b- defN 23-Jun-20 17:48 hex/genmodel/algos/rulefit/RuleFitMojoReader.class
+-rw-r--r--  2.0 unx     3386 b- defN 23-Jun-20 17:48 hex/genmodel/algos/rulefit/MojoRuleEnsemble.class
+-rw-r--r--  2.0 unx     1177 b- defN 23-Jun-20 17:48 hex/genmodel/algos/rulefit/MojoCondition$Type.class
+-rw-r--r--  2.0 unx     1286 b- defN 23-Jun-20 17:48 hex/genmodel/algos/rulefit/RuleFitMojoModel$ModelType.class
+-rw-r--r--  2.0 unx     1256 b- defN 23-Jun-20 17:48 hex/genmodel/algos/rulefit/MojoCondition$Operator.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/TreeSHAPPredictor$Workspace.class
+-rw-r--r--  2.0 unx     3299 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfoLightReader.class
+-rw-r--r--  2.0 unx      880 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/TreeSHAP$PathElement.class
+-rw-r--r--  2.0 unx     4714 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoReader.class
+-rw-r--r--  2.0 unx      353 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeGraphConverter.class
+-rw-r--r--  2.0 unx      657 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/ScoreTree0.class
+-rw-r--r--  2.0 unx      202 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/ScoreTree.class
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/TreeSHAP$1.class
+-rw-r--r--  2.0 unx      635 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/ScoreTree2.class
+-rw-r--r--  2.0 unx     1101 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/ConvertTreeOptions.class
+-rw-r--r--  2.0 unx     8018 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeSubgraph.class
+-rw-r--r--  2.0 unx     2998 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/TreeSHAPEnsemble.class
+-rw-r--r--  2.0 unx     8370 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/TreeSHAP.class
+-rw-r--r--  2.0 unx      253 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoModel$1.class
+-rw-r--r--  2.0 unx      535 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafNodeAssignments.class
+-rw-r--r--  2.0 unx      438 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoModel$DecisionPathTracker.class
+-rw-r--r--  2.0 unx     2835 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions.class
+-rw-r--r--  2.0 unx      657 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/ScoreTree1.class
+-rw-r--r--  2.0 unx      712 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/TreeSHAPPredictor.class
+-rw-r--r--  2.0 unx    16477 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeNode.class
+-rw-r--r--  2.0 unx     1175 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/CalibrationMojoHelper.class
+-rw-r--r--  2.0 unx     2634 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/ContributionComposer.class
+-rw-r--r--  2.0 unx      602 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/ScoreIsolationTree0.class
+-rw-r--r--  2.0 unx     1395 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/NaSplitDir.class
+-rw-r--r--  2.0 unx     3003 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoModel$LeafDecisionPathTracker.class
+-rw-r--r--  2.0 unx      611 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/TreeBackedMojoModel.class
+-rw-r--r--  2.0 unx     3699 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeGraph.class
+-rw-r--r--  2.0 unx    24842 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoModel.class
+-rw-r--r--  2.0 unx     1518 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoModelWithContributions$SharedTreeContributionsPredictor.class
+-rw-r--r--  2.0 unx     1707 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/TreeSHAP$PathPointer.class
+-rw-r--r--  2.0 unx      199 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/ScoreIsolationTree.class
+-rw-r--r--  2.0 unx     1445 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoModel$StringDecisionPathTracker.class
+-rw-r--r--  2.0 unx      399 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/CalibrationMojoHelper$MojoModelWithCalibration.class
+-rw-r--r--  2.0 unx     3805 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/ContributionsPredictor.class
+-rw-r--r--  2.0 unx     2632 b- defN 23-Jun-20 17:48 hex/genmodel/algos/tree/SharedTreeMojoModel$AuxInfo.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/coxph/
+-rw-r--r--  2.0 unx     6398 b- defN 23-Jun-20 17:48 hex/genmodel/algos/coxph/CoxPHMojoModel.class
+-rw-r--r--  2.0 unx     1311 b- defN 23-Jun-20 17:48 hex/genmodel/algos/coxph/CoxPHMojoModel$InteractionTypes.class
+-rw-r--r--  2.0 unx     1144 b- defN 23-Jun-20 17:48 hex/genmodel/algos/coxph/CoxPHMojoModel$Strata.class
+-rw-r--r--  2.0 unx     5061 b- defN 23-Jun-20 17:48 hex/genmodel/algos/coxph/CoxPHMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/drf/
+-rw-r--r--  2.0 unx     1633 b- defN 23-Jun-20 17:48 hex/genmodel/algos/drf/DrfMojoReader.class
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-20 17:48 hex/genmodel/algos/drf/DrfMojoModel$1.class
+-rw-r--r--  2.0 unx     3129 b- defN 23-Jun-20 17:48 hex/genmodel/algos/drf/DrfMojoModel$ContributionsPredictorDRF.class
+-rw-r--r--  2.0 unx     2700 b- defN 23-Jun-20 17:48 hex/genmodel/algos/drf/DrfMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isoforextended/
+-rw-r--r--  2.0 unx     4170 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoModel.class
+-rw-r--r--  2.0 unx     2306 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isoforextended/ExtendedIsolationForestMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/pca/
+-rw-r--r--  2.0 unx     2645 b- defN 23-Jun-20 17:48 hex/genmodel/algos/pca/PCAMojoModel.class
+-rw-r--r--  2.0 unx     2819 b- defN 23-Jun-20 17:48 hex/genmodel/algos/pca/PCAMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/
+-rw-r--r--  2.0 unx     4318 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoModel.class
+-rw-r--r--  2.0 unx     2466 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMultinomialMojoModel.class
+-rw-r--r--  2.0 unx     1747 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoModelBase.class
+-rw-r--r--  2.0 unx      848 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoModel$GLM_inverseInv.class
+-rw-r--r--  2.0 unx      851 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoModel$GLM_identityInv.class
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoModel$1.class
+-rw-r--r--  2.0 unx     2647 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmOrdinalMojoModel.class
+-rw-r--r--  2.0 unx      836 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoModel$GLM_logInv.class
+-rw-r--r--  2.0 unx      626 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoModel$GLM_ologitInv.class
+-rw-r--r--  2.0 unx      272 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoModel$Function1.class
+-rw-r--r--  2.0 unx      724 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoModel$GLM_tweedieInv.class
+-rw-r--r--  2.0 unx      842 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoModel$GLM_logitInv.class
+-rw-r--r--  2.0 unx     3584 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glm/GlmMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/targetencoder/
+-rw-r--r--  2.0 unx      677 b- defN 23-Jun-20 17:48 hex/genmodel/algos/targetencoder/ColumnsMapping.class
+-rw-r--r--  2.0 unx     3493 b- defN 23-Jun-20 17:48 hex/genmodel/algos/targetencoder/EncodingMap.class
+-rw-r--r--  2.0 unx     9375 b- defN 23-Jun-20 17:48 hex/genmodel/algos/targetencoder/TargetEncoderMojoReader.class
+-rw-r--r--  2.0 unx     2436 b- defN 23-Jun-20 17:48 hex/genmodel/algos/targetencoder/EncodingMaps.class
+-rw-r--r--  2.0 unx     1417 b- defN 23-Jun-20 17:48 hex/genmodel/algos/targetencoder/ColumnsToSingleMapping.class
+-rw-r--r--  2.0 unx     8265 b- defN 23-Jun-20 17:48 hex/genmodel/algos/targetencoder/TargetEncoderMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isotonic/
+-rw-r--r--  2.0 unx      888 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isotonic/IsotonicCalibrator.class
+-rw-r--r--  2.0 unx      874 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isotonic/IsotonicRegressionMojoModel.class
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isotonic/IsotonicRegressionMojoReader.class
+-rw-r--r--  2.0 unx     1680 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isotonic/IsotonicRegressionUtils.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/
+-rw-r--r--  2.0 unx      783 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierDropoutOut.class
+-rw-r--r--  2.0 unx     5224 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/DeeplearningMojoReader.class
+-rw-r--r--  2.0 unx     1081 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$SoftmaxOut.class
+-rw-r--r--  2.0 unx      769 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutDropoutOut.class
+-rw-r--r--  2.0 unx      709 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$LinearOut.class
+-rw-r--r--  2.0 unx     1096 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$1.class
+-rw-r--r--  2.0 unx     6719 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/NeuralNetwork.class
+-rw-r--r--  2.0 unx      934 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$RectifierOut.class
+-rw-r--r--  2.0 unx      323 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$ActivationFunctions.class
+-rw-r--r--  2.0 unx     2132 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils.class
+-rw-r--r--  2.0 unx      798 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierDropoutOut.class
+-rw-r--r--  2.0 unx      663 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/DeeplearningMojoModel$StoreWeightsBias.class
+-rw-r--r--  2.0 unx     6843 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/DeeplearningMojoModel.class
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$TanhDropoutOut.class
+-rw-r--r--  2.0 unx      995 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$ExpRectifierOut.class
+-rw-r--r--  2.0 unx      922 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$TanhOut.class
+-rw-r--r--  2.0 unx     1007 b- defN 23-Jun-20 17:48 hex/genmodel/algos/deeplearning/ActivationUtils$MaxoutOut.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/psvm/
+-rw-r--r--  2.0 unx      196 b- defN 23-Jun-20 17:48 hex/genmodel/algos/psvm/SupportVectorScorer.class
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-20 17:48 hex/genmodel/algos/psvm/KernelParameters.class
+-rw-r--r--  2.0 unx     1388 b- defN 23-Jun-20 17:48 hex/genmodel/algos/psvm/ScorerFactory.class
+-rw-r--r--  2.0 unx     1550 b- defN 23-Jun-20 17:48 hex/genmodel/algos/psvm/GaussianScorer.class
+-rw-r--r--  2.0 unx      973 b- defN 23-Jun-20 17:48 hex/genmodel/algos/psvm/KernelType.class
+-rw-r--r--  2.0 unx      699 b- defN 23-Jun-20 17:48 hex/genmodel/algos/psvm/ScorerFactory$1.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/ensemble/
+-rw-r--r--  2.0 unx     3993 b- defN 23-Jun-20 17:48 hex/genmodel/algos/ensemble/StackedEnsembleMojoReader.class
+-rw-r--r--  2.0 unx      974 b- defN 23-Jun-20 17:48 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel$StackedEnsembleMojoSubModel.class
+-rw-r--r--  2.0 unx     2165 b- defN 23-Jun-20 17:48 hex/genmodel/algos/ensemble/StackedEnsembleMojoModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isofor/
+-rw-r--r--  2.0 unx     1835 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isofor/IsolationForestMojoModel.class
+-rw-r--r--  2.0 unx     2021 b- defN 23-Jun-20 17:48 hex/genmodel/algos/isofor/IsolationForestMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/
+-rw-r--r--  2.0 unx     1572 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/GamMojoModel.class
+-rw-r--r--  2.0 unx     2046 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/ISplines.class
+-rw-r--r--  2.0 unx     2045 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/NBSplinesTypeII.class
+-rw-r--r--  2.0 unx    10726 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/GamMojoReader.class
+-rw-r--r--  2.0 unx     1717 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/NBSplinesTypeI$MSplineBasis.class
+-rw-r--r--  2.0 unx      855 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/ISplines$ISplineBasis.class
+-rw-r--r--  2.0 unx     1902 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/NBSplinesTypeII$BSplineBasis.class
+-rw-r--r--  2.0 unx     3495 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/NBSplinesTypeI.class
+-rw-r--r--  2.0 unx     2061 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/GamUtilsThinPlateRegression.class
+-rw-r--r--  2.0 unx    11583 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/GamMojoModelBase.class
+-rw-r--r--  2.0 unx     1347 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/MSplines.class
+-rw-r--r--  2.0 unx     4489 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/GamUtilsISplines.class
+-rw-r--r--  2.0 unx      896 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/GamMojoModelBase$1.class
+-rw-r--r--  2.0 unx     2234 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/GamMojoMultinomialModel.class
+-rw-r--r--  2.0 unx     1977 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/GamRowToRawDataConverter.class
+-rw-r--r--  2.0 unx     2518 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gam/GamUtilsCubicRegression.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/pipeline/
+-rw-r--r--  2.0 unx     1732 b- defN 23-Jun-20 17:48 hex/genmodel/algos/pipeline/MojoPipeline.class
+-rw-r--r--  2.0 unx     6799 b- defN 23-Jun-20 17:48 hex/genmodel/algos/pipeline/MojoPipelineReader.class
+-rw-r--r--  2.0 unx      635 b- defN 23-Jun-20 17:48 hex/genmodel/algos/pipeline/MojoPipeline$PipelineSubModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/kmeans/
+-rw-r--r--  2.0 unx     1339 b- defN 23-Jun-20 17:48 hex/genmodel/algos/kmeans/KMeansMojoModel.class
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-20 17:48 hex/genmodel/algos/kmeans/KMeansMojoReader.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gbm/
+-rw-r--r--  2.0 unx     4006 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gbm/GbmMojoModel.class
+-rw-r--r--  2.0 unx     2104 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gbm/GbmMojoReader.class
+-rw-r--r--  2.0 unx      981 b- defN 23-Jun-20 17:48 hex/genmodel/algos/gbm/GbmMojoModel$1.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/
+-rw-r--r--  2.0 unx     1345 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmRegularizer$3.class
+-rw-r--r--  2.0 unx     4904 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmMojoReader.class
+-rw-r--r--  2.0 unx     1567 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmLoss$5.class
+-rw-r--r--  2.0 unx     2161 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmLoss$8.class
+-rw-r--r--  2.0 unx     1232 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmRegularizer$2.class
+-rw-r--r--  2.0 unx     1980 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmRegularizer$8.class
+-rw-r--r--  2.0 unx      875 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmRegularizer$1.class
+-rw-r--r--  2.0 unx     2578 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmRegularizer.class
+-rw-r--r--  2.0 unx     1219 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmInitialization.class
+-rw-r--r--  2.0 unx     1075 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmLoss$2.class
+-rw-r--r--  2.0 unx     2236 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmLoss$9.class
+-rw-r--r--  2.0 unx     1512 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmLoss$6.class
+-rw-r--r--  2.0 unx     1186 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmLoss$3.class
+-rw-r--r--  2.0 unx     1290 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmRegularizer$4.class
+-rw-r--r--  2.0 unx     1406 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmRegularizer$7.class
+-rw-r--r--  2.0 unx     9537 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmMojoModel.class
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmRegularizer$5.class
+-rw-r--r--  2.0 unx      983 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmLoss$1.class
+-rw-r--r--  2.0 unx     1510 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmLoss$7.class
+-rw-r--r--  2.0 unx     1460 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmRegularizer$6.class
+-rw-r--r--  2.0 unx     3178 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmLoss.class
+-rw-r--r--  2.0 unx     1499 b- defN 23-Jun-20 17:48 hex/genmodel/algos/glrm/GlrmLoss$4.class
+-rw-r--r--  2.0 unx     1100 b- defN 23-Jun-20 17:48 hex/genmodel/ModelMojoReader$1.class
+-rw-r--r--  2.0 unx      855 b- defN 23-Jun-20 17:48 hex/genmodel/MojoReaderBackendFactory$1.class
+-rw-r--r--  2.0 unx     1934 b- defN 23-Jun-20 17:48 hex/genmodel/MultiModelMojoReader$NestedMojoReaderBackend.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/
+-rw-r--r--  2.0 unx     1045 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/SharedTreeModelAttributes.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/
+-rw-r--r--  2.0 unx      798 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinalGLM.class
+-rw-r--r--  2.0 unx      420 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsSupervised.class
+-rw-r--r--  2.0 unx      590 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsRegression.class
+-rw-r--r--  2.0 unx      802 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsBinomialGLM.class
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsAnomaly.class
+-rw-r--r--  2.0 unx      630 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetrics.class
+-rw-r--r--  2.0 unx      748 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsOrdinal.class
+-rw-r--r--  2.0 unx      860 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsBinomial.class
+-rw-r--r--  2.0 unx      860 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomial.class
+-rw-r--r--  2.0 unx      810 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionGLM.class
+-rw-r--r--  2.0 unx      814 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsMultinomialGLM.class
+-rw-r--r--  2.0 unx      517 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/metrics/MojoModelMetricsRegressionCoxPH.class
+-rw-r--r--  2.0 unx      993 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/DeepLearningModelAttributes.class
+-rw-r--r--  2.0 unx     5653 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/ModelAttributes.class
+-rw-r--r--  2.0 unx     1267 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/VariableImportances$1.class
+-rw-r--r--  2.0 unx      495 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/SerializedName.class
+-rw-r--r--  2.0 unx     2602 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/VariableImportances.class
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/Table$ColumnType.class
+-rw-r--r--  2.0 unx     1155 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/ModelAttributes$1.class
+-rw-r--r--  2.0 unx     3376 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/Table.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/parameters/
+-rw-r--r--  2.0 unx      874 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/parameters/ColumnSpecifier.class
+-rw-r--r--  2.0 unx      249 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/parameters/VariableImportancesHolder.class
+-rw-r--r--  2.0 unx      953 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/parameters/KeyValue.class
+-rw-r--r--  2.0 unx     1892 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/parameters/ModelParameter.class
+-rw-r--r--  2.0 unx     1319 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/parameters/ParameterKey$Type.class
+-rw-r--r--  2.0 unx      880 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/parameters/FeatureContribution.class
+-rw-r--r--  2.0 unx     1176 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/parameters/ParameterKey.class
+-rw-r--r--  2.0 unx     1263 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/parameters/StringPair.class
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/ModelJsonReader$1.class
+-rw-r--r--  2.0 unx     2522 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/ModelJsonReader$TypeHint.class
+-rw-r--r--  2.0 unx     1234 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/ModelAttributesGLM.class
+-rw-r--r--  2.0 unx    15710 b- defN 23-Jun-20 17:48 hex/genmodel/attributes/ModelJsonReader.class
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-20 17:48 hex/genmodel/CategoricalEncoding$2.class
+-rw-r--r--  2.0 unx     1551 b- defN 23-Jun-20 17:48 hex/genmodel/CategoricalEncoding$4.class
+-rw-r--r--  2.0 unx     1127 b- defN 23-Jun-20 17:48 hex/genmodel/MojoPipelineBuilder$MappingSpec.class
+-rw-r--r--  2.0 unx     5010 b- defN 23-Jun-20 17:48 hex/genmodel/ModelMojoFactory.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 water/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 water/util/
+-rw-r--r--  2.0 unx     4898 b- defN 23-Jun-20 17:48 water/util/ParseTime.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 water/util/comparison/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 water/util/comparison/string/
+-rw-r--r--  2.0 unx     1910 b- defN 23-Jun-20 17:48 water/util/comparison/string/StringComparatorFactory.class
+-rw-r--r--  2.0 unx     1623 b- defN 23-Jun-20 17:48 water/util/comparison/string/LevenshteinDistanceComparator.class
+-rw-r--r--  2.0 unx     2076 b- defN 23-Jun-20 17:48 water/util/comparison/string/H2OJaroWinklerComparator.class
+-rw-r--r--  2.0 unx    10148 b- defN 23-Jun-20 17:48 water/util/H2OPredictor.class
+-rw-r--r--  2.0 unx      606 b- defN 23-Jun-20 17:48 water/util/H2OPredictor$1.class
+-rw-r--r--  2.0 unx     2742 b- defN 23-Jun-20 17:48 water/util/JavaVersionUtils.class
+-rw-r--r--  2.0 unx      971 b- defN 23-Jun-20 17:48 water/util/ModelUtils.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 water/genmodel/
+-rw-r--r--  2.0 unx      873 b- defN 23-Jun-20 17:48 water/genmodel/AbstractBuildVersion$1.class
+-rw-r--r--  2.0 unx     2965 b- defN 23-Jun-20 17:48 water/genmodel/AbstractBuildVersion.class
+-rw-r--r--  2.0 unx      921 b- defN 23-Jun-20 17:48 water/genmodel/BuildVersion.class
+-rw-r--r--  2.0 unx      921 b- defN 23-Jun-20 17:48 water/genmodel/IGeneratedModel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:49 META-INF/services/
+-rw-r--r--  2.0 unx       29 b- defN 23-Jun-20 17:49 META-INF/services/hex.genmodel.tools.MojoPrinter
+366 files, 776249 bytes uncompressed, 380858 bytes compressed:  50.9%
```

#### zipnote «TEMP»/diffoscope_ztes36tb_/tmpjncpm52v_.zip

```diff
@@ -537,14 +537,17 @@
 
 Filename: hex/genmodel/algos/coxph/
 Comment: 
 
 Filename: hex/genmodel/algos/coxph/CoxPHMojoModel.class
 Comment: 
 
+Filename: hex/genmodel/algos/coxph/CoxPHMojoModel$InteractionTypes.class
+Comment: 
+
 Filename: hex/genmodel/algos/coxph/CoxPHMojoModel$Strata.class
 Comment: 
 
 Filename: hex/genmodel/algos/coxph/CoxPHMojoReader.class
 Comment: 
 
 Filename: hex/genmodel/algos/drf/
@@ -1038,14 +1041,32 @@
 
 Filename: water/
 Comment: 
 
 Filename: water/util/
 Comment: 
 
+Filename: water/util/ParseTime.class
+Comment: 
+
+Filename: water/util/comparison/
+Comment: 
+
+Filename: water/util/comparison/string/
+Comment: 
+
+Filename: water/util/comparison/string/StringComparatorFactory.class
+Comment: 
+
+Filename: water/util/comparison/string/LevenshteinDistanceComparator.class
+Comment: 
+
+Filename: water/util/comparison/string/H2OJaroWinklerComparator.class
+Comment: 
+
 Filename: water/util/H2OPredictor.class
 Comment: 
 
 Filename: water/util/H2OPredictor$1.class
 Comment: 
 
 Filename: water/util/JavaVersionUtils.class
```

#### hex/genmodel/GenMunger.class

##### procyon -ec {}

```diff
@@ -85,65 +85,104 @@
         }
         return cnt;
     }
     
     public static double add(final double d, final HashMap<String, String[]> parameters) {
         final String[] leftArg = (String[])parameters.get("leftArg");
         final String[] riteArg = (String[])parameters.get("rightArg");
-        if (leftArg == null) {
+        if (riteArg != null) {
             return d + parseNum(riteArg[0]);
         }
         return parseNum(leftArg[0]) + d;
     }
     
     public static double minus(final double d, final HashMap<String, String[]> parameters) {
         final String[] leftArg = (String[])parameters.get("leftArg");
         final String[] riteArg = (String[])parameters.get("rightArg");
-        if (leftArg == null) {
+        if (riteArg != null) {
             return d - parseNum(riteArg[0]);
         }
         return parseNum(leftArg[0]) - d;
     }
     
     public static double multiply(final double d, final HashMap<String, String[]> parameters) {
         final String[] leftArg = (String[])parameters.get("leftArg");
         final String[] riteArg = (String[])parameters.get("rightArg");
-        if (leftArg == null) {
+        if (riteArg != null) {
             return d * parseNum(riteArg[0]);
         }
         return parseNum(leftArg[0]) * d;
     }
     
     public static double divide(final double d, final HashMap<String, String[]> parameters) {
         final String[] leftArg = (String[])parameters.get("leftArg");
-        final String[] riteArg = (String[])parameters.get("rightArg");
-        if (leftArg == null) {
-            return d / parseNum(riteArg[0]);
+        final String[] rightArg = (String[])parameters.get("rightArg");
+        if (rightArg != null) {
+            return d / parseNum(rightArg[0]);
         }
         return parseNum(leftArg[0]) / d;
     }
     
     public static double mod(final double d, final HashMap<String, String[]> parameters) {
         final String leftArg = ((String[])parameters.get("leftArg"))[0];
-        final String riteArg = ((String[])parameters.get("rightArg"))[0];
-        if (leftArg == null) {
-            return d % parseNum(riteArg);
+        final String rightArg = ((String[])parameters.get("rightArg"))[0];
+        if (rightArg != null) {
+            return d % parseNum(rightArg);
         }
         return parseNum(leftArg) % d;
     }
     
     public static double pow(final double d, final HashMap<String, String[]> parameters) {
         final String leftArg = ((String[])parameters.get("leftArg"))[0];
-        final String riteArg = ((String[])parameters.get("rightArg"))[0];
-        if (leftArg == null) {
-            return Math.pow(d, parseNum(riteArg));
+        final String rightArg = ((String[])parameters.get("rightArg"))[0];
+        if (rightArg != null) {
+            return Math.pow(d, parseNum(rightArg));
         }
         return Math.pow(parseNum(leftArg), d);
     }
     
+    private static double and(final double l, final double r) {
+        return (l == 0.0 || r == 0.0) ? 0.0 : ((Double.isNaN(l) || Double.isNaN(r)) ? Double.NaN : 1.0);
+    }
+    
+    public static double and(final double d, final HashMap<String, String[]> parameters) {
+        final String leftArg = ((String[])parameters.get("leftArg"))[0];
+        final String rightArg = ((String[])parameters.get("rightArg"))[0];
+        if (rightArg != null) {
+            return and(d, parseNum(rightArg));
+        }
+        return and(parseNum(leftArg), d);
+    }
+    
+    private static double or(final double l, final double r) {
+        return (l == 1.0 || r == 1.0) ? 1.0 : ((Double.isNaN(l) || Double.isNaN(r)) ? Double.NaN : 0.0);
+    }
+    
+    public static double or(final double d, final HashMap<String, String[]> parameters) {
+        final String leftArg = ((String[])parameters.get("leftArg"))[0];
+        final String rightArg = ((String[])parameters.get("rightArg"))[0];
+        if (rightArg != null) {
+            return or(d, parseNum(rightArg));
+        }
+        return or(parseNum(leftArg), d);
+    }
+    
+    private static double intDiv(final double l, final double r) {
+        return ((int)r == 0) ? Double.NaN : ((double)((int)l / (int)r));
+    }
+    
+    public static double intDiv(final double d, final HashMap<String, String[]> parameters) {
+        final String leftArg = ((String[])parameters.get("leftArg"))[0];
+        final String rightArg = ((String[])parameters.get("rightArg"))[0];
+        if (rightArg != null) {
+            return intDiv(d, parseNum(rightArg));
+        }
+        return intDiv(parseNum(leftArg), d);
+    }
+    
     public static String[] strsplit(final String s, final HashMap<String, String[]> parameters) {
         final String pattern = ((String[])parameters.get("split"))[0];
         return s.split(pattern);
     }
     
     public static double asnumeric(final String s, final HashMap<String, String[]> parameters) {
         return parseNum(s);
```

#### hex/genmodel/ModelMojoReader.class

##### procyon -ec {}

```diff
@@ -325,8 +325,17 @@
             }
         }
     }
     
     protected MojoReaderBackend getMojoReaderBackend() {
         return this._reader;
     }
+    
+    public String[] readStringArrays(final int aSize, final String title) throws IOException {
+        final String[] stringArrays = new String[aSize];
+        int counter = 0;
+        for (final String line : this.readtext(title)) {
+            stringArrays[counter++] = line;
+        }
+        return stringArrays;
+    }
 }
```

#### hex/genmodel/algos/coxph/CoxPHMojoModel.class

##### procyon -ec {}

```diff
@@ -1,63 +1,94 @@
 
 package hex.genmodel.algos.coxph;
 
+import java.util.Arrays;
+import java.util.List;
+import java.util.HashSet;
 import java.util.HashMap;
 import hex.genmodel.MojoModel;
 
 public class CoxPHMojoModel extends MojoModel
 {
     double[] _coef;
     HashMap<CoxPHMojoModel.Strata, Integer> _strata;
     int _strata_len;
     double[][] _x_mean_cat;
     double[][] _x_mean_num;
     int[] _cat_offsets;
     int _cats;
     double[] _lpBase;
     boolean _useAllFactorLevels;
+    int _nums;
     int[] _interactions_1;
     int[] _interactions_2;
     int[] _interaction_targets;
+    boolean[] _is_enum_1;
+    HashSet<Integer> _interaction_column_index;
+    HashMap<Integer, List<String>> _interaction_column_domains;
+    CoxPHMojoModel.InteractionTypes[] _interaction_types;
+    int[] _num_offsets;
     
     CoxPHMojoModel(final String[] columns, final String[][] domains, final String responseColumn) {
         super(columns, domains, responseColumn);
     }
     
     public double[] score0(final double[] row, final double[] predictions) {
         return this.score0(row, 0.0, predictions);
     }
     
     public double[] score0(final double[] row, final double offset, final double[] predictions) {
+        int[] enumOffset = null;
         if (this._interaction_targets != null) {
-            this.evaluateInteractions(row);
+            enumOffset = this.evaluateInteractions(row);
         }
-        predictions[0] = this.forCategories(row) + this.forOtherColumns(row) - this.forStrata(row) + offset;
+        predictions[0] = this.forCategories(row) + this.forOtherColumns(row, enumOffset) - this.forStrata(row) + offset;
         return predictions;
     }
     
-    private double forOtherColumns(final double[] row) {
+    private double forOtherColumns(final double[] row, final int[] enumOffset) {
         double result = 0.0;
-        for (int catOffsetDiff = this._cat_offsets[this._cats] - this._cats, i = this._cats; i + catOffsetDiff < this._coef.length; ++i) {
-            result += this._coef[catOffsetDiff + i] * this.featureValue(row, i);
+        final int coefLen = this._coef.length;
+        for (int i = 0; i < this._nums; ++i) {
+            if (enumOffset == null || enumOffset[i] < 0) {
+                if (this._num_offsets[i] >= coefLen) {
+                    break;
+                }
+                result += this._coef[this._num_offsets[i]] * this.featureValue(row, i + this._cats);
+            }
+            else {
+                if (enumOffset[i] >= coefLen) {
+                    break;
+                }
+                result += this._coef[enumOffset[i]] * this.featureValue(row, i + this._cats);
+            }
         }
         return result;
     }
     
     private double forStrata(final double[] row) {
         final int strata = this.strataForRow(row);
         return this._lpBase[strata];
     }
     
     private double forCategories(final double[] row) {
         double result = 0.0;
         if (!this._useAllFactorLevels) {
-            for (int category = 0; category < this._cat_offsets.length - 1; ++category) {
-                if (this.featureValue(row, category) != 0.0) {
-                    result += this.forOneCategory(row, category, 1);
+            for (int category = 0; category < this._cats; ++category) {
+                final double val = this.featureValue(row, category);
+                if (Double.isNaN(val)) {
+                    result = Double.NaN;
+                }
+                else if (val >= 0.0) {
+                    if (this._interaction_column_index.contains(Integer.valueOf(category))) {
+                        result += this.forOneCategory(row, category, 0);
+                    }
+                    else {
+                        result += this.forOneCategory(row, category, 1);
+                    }
                 }
             }
         }
         else {
             for (int category = 0; category < this._cat_offsets.length - 1; ++category) {
                 result += this.forOneCategory(row, category, 0);
             }
@@ -67,15 +98,15 @@
     
     double forOneCategory(final double[] row, final int category, final int lowestFactorValue) {
         final int value = (int)this.featureValue(row, category) - lowestFactorValue;
         if (value != this.featureValue(row, category) - lowestFactorValue) {
             throw new IllegalArgumentException("categorical value out of range");
         }
         final int x = value + this._cat_offsets[category];
-        if (x < this._cat_offsets[category + 1]) {
+        if (value >= 0 && x < this._cat_offsets[category + 1]) {
             return this._coef[x];
         }
         return 0.0;
     }
     
     double[] computeLpBase() {
         final int _numStart = (this._x_mean_cat.length >= 1) ? this._x_mean_cat[0].length : 0;
@@ -104,16 +135,51 @@
         if (0 == this._strata.size()) {
             return 0;
         }
         final CoxPHMojoModel.Strata o = new CoxPHMojoModel.Strata(row, this._strata_len);
         return Integer.valueOf(this._strata.get((Object)o));
     }
     
-    private void evaluateInteractions(final double[] row) {
-        for (int i = 0; i < this._interaction_targets.length; ++i) {
-            final int target = this._interaction_targets[i];
+    private int[] evaluateInteractions(final double[] row) {
+        final int[] enumOffset = new int[this._nums];
+        Arrays.fill(enumOffset, -1);
+        for (int interactionIndex = 0; interactionIndex < this._interaction_targets.length; ++interactionIndex) {
+            final int target = this._interaction_targets[interactionIndex];
             if (Double.isNaN(row[target])) {
-                row[target] = row[this._interactions_1[i]] * row[this._interactions_2[i]];
+                if (CoxPHMojoModel.InteractionTypes.ENUM_TO_ENUM.equals((Object)this._interaction_types[interactionIndex])) {
+                    row[target] = this.enumEnumInteractions(row, interactionIndex);
+                }
+                else if (CoxPHMojoModel.InteractionTypes.NUM_TO_NUM.equals((Object)this._interaction_types[interactionIndex])) {
+                    row[target] = row[this._interactions_1[interactionIndex]] * row[this._interactions_2[interactionIndex]];
+                }
+                else {
+                    this.enumNumInteractions(row, enumOffset, interactionIndex, target);
+                }
             }
         }
+        return enumOffset;
+    }
+    
+    private void enumNumInteractions(final double[] row, final int[] enumOffset, final int interactionIndex, final int rowIndex) {
+        final int enumPredIndex = this._is_enum_1[interactionIndex] ? this._interactions_1[interactionIndex] : this._interactions_2[interactionIndex];
+        final int numPredIndex = this._is_enum_1[interactionIndex] ? this._interactions_2[interactionIndex] : this._interactions_1[interactionIndex];
+        final int offset = this._num_offsets[rowIndex - this._cats];
+        final int catLevel = (int)row[enumPredIndex] - (this._useAllFactorLevels ? 0 : 1);
+        row[rowIndex] = ((catLevel < 0) ? 0.0 : row[numPredIndex]);
+        enumOffset[rowIndex - this._cats] = catLevel + offset;
+    }
+    
+    private int enumEnumInteractions(final double[] row, final int interactionIndex) {
+        final List<String> combinedDomains = (List<String>)this._interaction_column_domains.get(Integer.valueOf(this._interaction_targets[interactionIndex]));
+        final int predictor1Index = this._interactions_1[interactionIndex];
+        final int predictor2Index = this._interactions_2[interactionIndex];
+        final String[] predictor1Domains = this._domains[predictor1Index];
+        final String[] predictor2Domains = this._domains[predictor2Index];
+        final String predictor1Domain = predictor1Domains[(int)row[predictor1Index]];
+        final String predictor2Domain = predictor2Domains[(int)row[predictor2Index]];
+        final String combinedEnumDomains = predictor1Domain + "_" + predictor2Domain;
+        if (combinedDomains.contains(combinedEnumDomains)) {
+            return combinedDomains.indexOf(combinedEnumDomains);
+        }
+        return -1;
     }
 }
```

#### hex/genmodel/algos/coxph/CoxPHMojoReader.class

##### procyon -ec {}

```diff
@@ -1,13 +1,15 @@
 
 package hex.genmodel.algos.coxph;
 
 import hex.genmodel.MojoModel;
-import java.util.HashMap;
 import java.io.IOException;
+import java.util.Arrays;
+import java.util.HashMap;
+import java.util.HashSet;
 import hex.genmodel.ModelMojoReader;
 
 public class CoxPHMojoReader extends ModelMojoReader<CoxPHMojoModel>
 {
     public String getModelName() {
         return "CoxPH";
     }
@@ -18,17 +20,51 @@
         ((CoxPHMojoModel)this._model)._coef = (double[])this.readkv("coef");
         ((CoxPHMojoModel)this._model)._strata = this.readStrata();
         ((CoxPHMojoModel)this._model)._strata_len = this.readStrataLen();
         ((CoxPHMojoModel)this._model)._cat_offsets = (int[])this.readkv("cat_offsets");
         ((CoxPHMojoModel)this._model)._cats = (int)this.readkv("cats");
         ((CoxPHMojoModel)this._model)._useAllFactorLevels = (boolean)this.readkv("use_all_factor_levels");
         ((CoxPHMojoModel)this._model)._lpBase = ((CoxPHMojoModel)this._model).computeLpBase();
-        ((CoxPHMojoModel)this._model)._interactions_1 = (int[])this.readkv("interactions_1");
-        ((CoxPHMojoModel)this._model)._interactions_2 = (int[])this.readkv("interactions_2");
         ((CoxPHMojoModel)this._model)._interaction_targets = (int[])this.readkv("interaction_targets");
+        ((CoxPHMojoModel)this._model)._interaction_column_index = new HashSet();
+        ((CoxPHMojoModel)this._model)._interaction_column_domains = new HashMap();
+        ((CoxPHMojoModel)this._model)._nums = (int)this.readkv("num_numerical_columns");
+        ((CoxPHMojoModel)this._model)._num_offsets = (int[])this.readkv("num_offsets");
+        if (((CoxPHMojoModel)this._model)._interaction_targets != null) {
+            ((CoxPHMojoModel)this._model)._interactions_1 = (int[])this.readkv("interactions_1");
+            ((CoxPHMojoModel)this._model)._interactions_2 = (int[])this.readkv("interactions_2");
+            for (final int index : ((CoxPHMojoModel)this._model)._interaction_targets) {
+                ((CoxPHMojoModel)this._model)._interaction_column_index.add(Integer.valueOf(index));
+                if (((CoxPHMojoModel)this._model)._domains[index] != null) {
+                    ((CoxPHMojoModel)this._model)._interaction_column_domains.put(Integer.valueOf(index), Arrays.asList(((CoxPHMojoModel)this._model)._domains[index]));
+                }
+            }
+            this.createInteractionTypes();
+        }
+    }
+    
+    private void createInteractionTypes() {
+        final int numInteractions = ((CoxPHMojoModel)this._model)._interaction_targets.length;
+        ((CoxPHMojoModel)this._model)._interaction_types = new CoxPHMojoModel.InteractionTypes[numInteractions];
+        ((CoxPHMojoModel)this._model)._is_enum_1 = new boolean[numInteractions];
+        for (int index = 0; index < numInteractions; ++index) {
+            if (((CoxPHMojoModel)this._model)._domains[((CoxPHMojoModel)this._model)._interactions_1[index]] != null && ((CoxPHMojoModel)this._model)._domains[((CoxPHMojoModel)this._model)._interactions_2[index]] != null) {
+                ((CoxPHMojoModel)this._model)._interaction_types[index] = CoxPHMojoModel.InteractionTypes.ENUM_TO_ENUM;
+                ((CoxPHMojoModel)this._model)._is_enum_1[index] = true;
+            }
+            else if (((CoxPHMojoModel)this._model)._domains[((CoxPHMojoModel)this._model)._interactions_1[index]] == null && ((CoxPHMojoModel)this._model)._domains[((CoxPHMojoModel)this._model)._interactions_2[index]] == null) {
+                ((CoxPHMojoModel)this._model)._interaction_types[index] = CoxPHMojoModel.InteractionTypes.NUM_TO_NUM;
+            }
+            else {
+                ((CoxPHMojoModel)this._model)._interaction_types[index] = CoxPHMojoModel.InteractionTypes.ENUM_TO_NUM;
+                if (((CoxPHMojoModel)this._model)._domains[((CoxPHMojoModel)this._model)._interactions_1[index]] != null) {
+                    ((CoxPHMojoModel)this._model)._is_enum_1[index] = true;
+                }
+            }
+        }
     }
     
     private HashMap<CoxPHMojoModel.Strata, Integer> readStrata() {
         final int count = (int)this.readkv("strata_count");
         final HashMap<CoxPHMojoModel.Strata, Integer> result = new HashMap<CoxPHMojoModel.Strata, Integer>(count);
         for (int i = 0; i < count; ++i) {
             final double[] strata = (double[])this.readkv("strata_" + i);
```

#### hex/genmodel/algos/gam/GamMojoReader.class

##### procyon -ec {}

```diff
@@ -125,23 +125,14 @@
         if (((GamMojoModelBase)this._model)._numCSCol > 0) {
             final int[] numKnotsM2 = ArrayUtils.subtract(((GamMojoModelBase)this._model)._num_knots_sorted, 2);
             ((GamMojoModelBase)this._model)._binvD = this.read3DArray("_binvD", ((GamMojoModelBase)this._model)._numCSCol, numKnotsM2, ((GamMojoModelBase)this._model)._num_knots_sorted);
         }
         ((GamMojoModelBase)this._model).init();
     }
     
-    String[] readStringArrays(final int aSize, final String title) throws IOException {
-        final String[] stringArrays = new String[aSize];
-        int counter = 0;
-        for (final String line : this.readtext(title)) {
-            stringArrays[counter++] = line;
-        }
-        return stringArrays;
-    }
-    
     String[][] read2DStringArrays(final int[] arrayDim, final String title) throws IOException {
         final int firstDim = arrayDim.length;
         final String[][] stringArrays = new String[firstDim][];
         int indexDim1 = 0;
         int indexDim2 = 0;
         for (int index = 0; index < firstDim; ++index) {
             stringArrays[index] = new String[arrayDim[index]];
```

#### hex/genmodel/attributes/metrics/MojoModelMetricsOrdinalGLM.class

##### procyon -ec {}

```diff
@@ -10,8 +10,9 @@
     @SerializedName("residual_degrees_of_freedom")
     public long _residualDegreesOfFreedom;
     @SerializedName("residual_deviance")
     public double _resDev;
     @SerializedName("null_deviance")
     public double _nullDev;
     public double _AIC;
+    public double _loglikelihood;
 }
```

#### hex/genmodel/attributes/metrics/MojoModelMetricsBinomialGLM.class

##### procyon -ec {}

```diff
@@ -10,8 +10,9 @@
     @SerializedName("residual_degrees_of_freedom")
     public long _residualDegreesOfFreedom;
     @SerializedName("residual_deviance")
     public double _resDev;
     @SerializedName("null_deviance")
     public double _nullDev;
     public double _AIC;
+    public double _loglikelihood;
 }
```

#### hex/genmodel/attributes/metrics/MojoModelMetricsRegressionGLM.class

##### procyon -ec {}

```diff
@@ -10,8 +10,9 @@
     @SerializedName("residual_degrees_of_freedom")
     public long _residualDegreesOfFreedom;
     @SerializedName("residual_deviance")
     public double _resDev;
     @SerializedName("null_deviance")
     public double _nullDev;
     public double _AIC;
+    public double _loglikelihood;
 }
```

#### hex/genmodel/attributes/metrics/MojoModelMetricsMultinomialGLM.class

##### procyon -ec {}

```diff
@@ -10,8 +10,9 @@
     @SerializedName("residual_degrees_of_freedom")
     public long _residualDegreesOfFreedom;
     @SerializedName("residual_deviance")
     public double _resDev;
     @SerializedName("null_deviance")
     public double _nullDev;
     public double _AIC;
+    public double _loglikelihood;
 }
```

#### water/genmodel/BuildVersion.class

##### procyon -ec {}

```diff
@@ -1,29 +1,29 @@
 
 package water.genmodel;
 
 public class BuildVersion extends AbstractBuildVersion
 {
     public String branchName() {
-        return "rel-zz_kurka";
+        return "rel-3.42.0";
     }
     
     public String lastCommitHash() {
-        return "5ff8870f912c6110d7b6988f577c020de10496ec";
+        return "d87d47b38cd85369b3c3d04e521ea500d46fc1ce";
     }
     
     public String describe() {
-        return "jenkins-3.40.0.3-122-g5ff8870";
+        return "jenkins-master-6234-5-gd87d47b";
     }
     
     public String projectVersion() {
-        return "3.40.0.4";
+        return "3.42.0.1";
     }
     
     public String compiledOn() {
-        return "2023-04-28 12:08:23";
+        return "2023-06-20 17:48:24";
     }
     
     public String compiledBy() {
         return "jenkins";
     }
 }
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-converter-1.5.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/guava-21.0.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/guava-21.0.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.30.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.31.jar`

 * *Files 26% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7974 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 xgboost/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 xgboost/sklearn/
--rw-rw-r--  2.0 unx      364 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      168 b- defN 23-Jun-19 22:03 xgboost/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     2270 b- defN 23-Jun-19 22:03 xgboost/sklearn/XGBClassifier.class
--rw-rw-r--  2.0 unx     2210 b- defN 23-Jun-19 22:03 xgboost/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2246 b- defN 23-Jun-19 22:03 xgboost/sklearn/XGBRegressor.class
--rw-rw-r--  2.0 unx     4204 b- defN 23-Jun-19 22:03 xgboost/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
--rw-rw-r--  2.0 unx     1453 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
--rw-rw-r--  2.0 unx      116 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
-15 files, 13161 bytes uncompressed, 5918 bytes compressed:  55.0%
+Zip file size: 7976 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 xgboost/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 xgboost/sklearn/
+-rw-rw-r--  2.0 unx      364 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      168 b- defN 23-Jul-08 09:03 xgboost/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2270 b- defN 23-Jul-08 09:03 xgboost/sklearn/XGBClassifier.class
+-rw-rw-r--  2.0 unx     2210 b- defN 23-Jul-08 09:03 xgboost/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2246 b- defN 23-Jul-08 09:03 xgboost/sklearn/XGBRegressor.class
+-rw-rw-r--  2.0 unx     4204 b- defN 23-Jul-08 09:03 xgboost/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
+-rw-rw-r--  2.0 unx      116 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
+15 files, 13161 bytes uncompressed, 5920 bytes compressed:  55.0%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.30</version>
+    <version>1.7.31</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-xgboost</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn XGBoost converter</name>
   <description>JPMML Scikit-Learn XGBoost to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Mon Jun 19 22:03:17 EEST 2023
-version=1.7.30
+#Sat Jul 08 09:03:24 EEST 2023
+version=1.7.31
 groupId=org.jpmml
 artifactId=pmml-sklearn-xgboost
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/ubjson-0.1.8.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/ubjson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.30.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.31.jar`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,68 +1,65 @@
-Zip file size: 83162 bytes, number of entries: 66
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 mlxtend/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 mlxtend/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 pycaret/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 pycaret/preprocess/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 tpot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 tpot/builtins/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 optbinning/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 optbinning/scorecard/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 imblearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 category_encoders/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklego/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklego/meta/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklego/preprocessing/
--rw-rw-r--  2.0 unx      913 b- defN 23-Jun-19 22:03 mlxtend/preprocessing/DenseTransformer.class
--rw-rw-r--  2.0 unx     4244 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      898 b- defN 23-Jun-19 22:03 pycaret/preprocess/FixImbalancer.class
--rw-rw-r--  2.0 unx     2818 b- defN 23-Jun-19 22:03 pycaret/preprocess/RemoveMulticollinearity.class
--rw-rw-r--  2.0 unx      907 b- defN 23-Jun-19 22:03 pycaret/preprocess/CleanColumnNames.class
--rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-19 22:03 pycaret/preprocess/RareCategoryGrouping.class
--rw-rw-r--  2.0 unx     7434 b- defN 23-Jun-19 22:03 pycaret/preprocess/TransformerWrapper.class
--rw-rw-r--  2.0 unx     4951 b- defN 23-Jun-19 22:03 pycaret/preprocess/TransformerWrapperWithInverse.class
--rw-rw-r--  2.0 unx      720 b- defN 23-Jun-19 22:03 tpot/builtins/StackingEstimator$1.class
--rw-rw-r--  2.0 unx     4530 b- defN 23-Jun-19 22:03 tpot/builtins/StackingEstimator.class
--rw-rw-r--  2.0 unx     2433 b- defN 23-Jun-19 22:03 optbinning/BinnedFeature.class
--rw-rw-r--  2.0 unx     8333 b- defN 23-Jun-19 22:03 optbinning/scorecard/Scorecard.class
--rw-rw-r--  2.0 unx     2133 b- defN 23-Jun-19 22:03 optbinning/OptimalBinningUtil.class
--rw-rw-r--  2.0 unx     6372 b- defN 23-Jun-19 22:03 optbinning/BinningProcess.class
--rw-rw-r--  2.0 unx     2274 b- defN 23-Jun-19 22:03 optbinning/ContinuousOptimalBinning.class
--rw-rw-r--  2.0 unx     3917 b- defN 23-Jun-19 22:03 optbinning/MulticlassOptimalBinning.class
--rw-rw-r--  2.0 unx     1242 b- defN 23-Jun-19 22:03 optbinning/BinningProcess$1.class
--rw-rw-r--  2.0 unx    14050 b- defN 23-Jun-19 22:03 optbinning/OptimalBinning.class
--rw-rw-r--  2.0 unx      860 b- defN 23-Jun-19 22:03 imblearn/Sampler.class
--rw-rw-r--  2.0 unx     1916 b- defN 23-Jun-19 22:03 category_encoders/MapEncoder.class
--rw-rw-r--  2.0 unx     8449 b- defN 23-Jun-19 22:03 category_encoders/MapFeature.class
--rw-rw-r--  2.0 unx      527 b- defN 23-Jun-19 22:03 category_encoders/TargetEncoder.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Jun-19 22:03 category_encoders/CountEncoder$1.class
--rw-rw-r--  2.0 unx      515 b- defN 23-Jun-19 22:03 category_encoders/WOEEncoder.class
--rw-rw-r--  2.0 unx     8474 b- defN 23-Jun-19 22:03 category_encoders/MeanEncoder.class
--rw-rw-r--  2.0 unx     8520 b- defN 23-Jun-19 22:03 category_encoders/CountEncoder.class
--rw-rw-r--  2.0 unx    12815 b- defN 23-Jun-19 22:03 category_encoders/BaseNFeature.class
--rw-rw-r--  2.0 unx     1481 b- defN 23-Jun-19 22:03 category_encoders/OrdinalMapEncoder$1.class
--rw-rw-r--  2.0 unx     1445 b- defN 23-Jun-19 22:03 category_encoders/MeanEncoder$1.class
--rw-rw-r--  2.0 unx     2119 b- defN 23-Jun-19 22:03 category_encoders/OrdinalEncoder$Mapping.class
--rw-rw-r--  2.0 unx     1323 b- defN 23-Jun-19 22:03 category_encoders/LeaveOneOutEncoder$1.class
--rw-rw-r--  2.0 unx     7967 b- defN 23-Jun-19 22:03 category_encoders/OrdinalMapEncoder.class
--rw-rw-r--  2.0 unx     9241 b- defN 23-Jun-19 22:03 category_encoders/BaseNEncoder.class
--rw-rw-r--  2.0 unx     1334 b- defN 23-Jun-19 22:03 category_encoders/BinaryEncoder.class
--rw-rw-r--  2.0 unx     3547 b- defN 23-Jun-19 22:03 category_encoders/OneHotEncoder.class
--rw-rw-r--  2.0 unx     1325 b- defN 23-Jun-19 22:03 category_encoders/CatBoostEncoder.class
--rw-rw-r--  2.0 unx     2062 b- defN 23-Jun-19 22:03 category_encoders/CategoryEncoderUtil.class
--rw-rw-r--  2.0 unx     1564 b- defN 23-Jun-19 22:03 category_encoders/OrdinalEncoder$1.class
--rw-rw-r--  2.0 unx     1047 b- defN 23-Jun-19 22:03 category_encoders/LeaveOneOutEncoder.class
--rw-rw-r--  2.0 unx     4690 b- defN 23-Jun-19 22:03 category_encoders/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      742 b- defN 23-Jun-19 22:03 category_encoders/MeanEncoder$MeanFunction.class
--rw-rw-r--  2.0 unx     1378 b- defN 23-Jun-19 22:03 category_encoders/CatBoostEncoder$1.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Jun-19 22:03 category_encoders/CategoryEncoder.class
--rw-rw-r--  2.0 unx      725 b- defN 23-Jun-19 22:03 sklego/meta/EstimatorTransformer$1.class
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-19 22:03 sklego/meta/EstimatorTransformer.class
--rw-rw-r--  2.0 unx      920 b- defN 23-Jun-19 22:03 sklego/preprocessing/IdentityTransformer.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-extension/
--rw-rw-r--  2.0 unx     1226 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
--rw-rw-r--  2.0 unx      118 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
-66 files, 169531 bytes uncompressed, 73746 bytes compressed:  56.5%
+Zip file size: 83825 bytes, number of entries: 63
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 pycaret/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 pycaret/preprocess/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 tpot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 tpot/builtins/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 optbinning/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 optbinning/scorecard/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 imblearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 category_encoders/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklego/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklego/meta/
+-rw-rw-r--  2.0 unx     4312 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      412 b- defN 23-Jul-08 09:03 pycaret/preprocess/FixImbalancer.class
+-rw-rw-r--  2.0 unx     2818 b- defN 23-Jul-08 09:03 pycaret/preprocess/RemoveMulticollinearity.class
+-rw-rw-r--  2.0 unx      421 b- defN 23-Jul-08 09:03 pycaret/preprocess/CleanColumnNames.class
+-rw-rw-r--  2.0 unx     1332 b- defN 23-Jul-08 09:03 pycaret/preprocess/RemoveOutliers$1.class
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jul-08 09:03 pycaret/preprocess/RareCategoryGrouping.class
+-rw-rw-r--  2.0 unx     3125 b- defN 23-Jul-08 09:03 pycaret/preprocess/RemoveOutliers.class
+-rw-rw-r--  2.0 unx     7822 b- defN 23-Jul-08 09:03 pycaret/preprocess/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     4951 b- defN 23-Jul-08 09:03 pycaret/preprocess/TransformerWrapperWithInverse.class
+-rw-rw-r--  2.0 unx      720 b- defN 23-Jul-08 09:03 tpot/builtins/StackingEstimator$1.class
+-rw-rw-r--  2.0 unx     4530 b- defN 23-Jul-08 09:03 tpot/builtins/StackingEstimator.class
+-rw-rw-r--  2.0 unx     2433 b- defN 23-Jul-08 09:03 optbinning/BinnedFeature.class
+-rw-rw-r--  2.0 unx     8333 b- defN 23-Jul-08 09:03 optbinning/scorecard/Scorecard.class
+-rw-rw-r--  2.0 unx     2133 b- defN 23-Jul-08 09:03 optbinning/OptimalBinningUtil.class
+-rw-rw-r--  2.0 unx     6372 b- defN 23-Jul-08 09:03 optbinning/BinningProcess.class
+-rw-rw-r--  2.0 unx     2274 b- defN 23-Jul-08 09:03 optbinning/ContinuousOptimalBinning.class
+-rw-rw-r--  2.0 unx     3917 b- defN 23-Jul-08 09:03 optbinning/MulticlassOptimalBinning.class
+-rw-rw-r--  2.0 unx     1240 b- defN 23-Jul-08 09:03 optbinning/BinningProcess$1.class
+-rw-rw-r--  2.0 unx    14050 b- defN 23-Jul-08 09:03 optbinning/OptimalBinning.class
+-rw-rw-r--  2.0 unx      374 b- defN 23-Jul-08 09:03 imblearn/Sampler.class
+-rw-rw-r--  2.0 unx     1916 b- defN 23-Jul-08 09:03 category_encoders/MapEncoder.class
+-rw-rw-r--  2.0 unx     8449 b- defN 23-Jul-08 09:03 category_encoders/MapFeature.class
+-rw-rw-r--  2.0 unx      527 b- defN 23-Jul-08 09:03 category_encoders/TargetEncoder.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Jul-08 09:03 category_encoders/CountEncoder$1.class
+-rw-rw-r--  2.0 unx      515 b- defN 23-Jul-08 09:03 category_encoders/WOEEncoder.class
+-rw-rw-r--  2.0 unx     8474 b- defN 23-Jul-08 09:03 category_encoders/MeanEncoder.class
+-rw-rw-r--  2.0 unx     8520 b- defN 23-Jul-08 09:03 category_encoders/CountEncoder.class
+-rw-rw-r--  2.0 unx    12815 b- defN 23-Jul-08 09:03 category_encoders/BaseNFeature.class
+-rw-rw-r--  2.0 unx     1481 b- defN 23-Jul-08 09:03 category_encoders/OrdinalMapEncoder$1.class
+-rw-rw-r--  2.0 unx     1445 b- defN 23-Jul-08 09:03 category_encoders/MeanEncoder$1.class
+-rw-rw-r--  2.0 unx     2119 b- defN 23-Jul-08 09:03 category_encoders/OrdinalEncoder$Mapping.class
+-rw-rw-r--  2.0 unx     1323 b- defN 23-Jul-08 09:03 category_encoders/LeaveOneOutEncoder$1.class
+-rw-rw-r--  2.0 unx     8108 b- defN 23-Jul-08 09:03 category_encoders/OrdinalMapEncoder.class
+-rw-rw-r--  2.0 unx     9241 b- defN 23-Jul-08 09:03 category_encoders/BaseNEncoder.class
+-rw-rw-r--  2.0 unx     1334 b- defN 23-Jul-08 09:03 category_encoders/BinaryEncoder.class
+-rw-rw-r--  2.0 unx     3547 b- defN 23-Jul-08 09:03 category_encoders/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     1325 b- defN 23-Jul-08 09:03 category_encoders/CatBoostEncoder.class
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Jul-08 09:03 category_encoders/CategoryEncoderUtil.class
+-rw-rw-r--  2.0 unx     1564 b- defN 23-Jul-08 09:03 category_encoders/OrdinalEncoder$1.class
+-rw-rw-r--  2.0 unx     1047 b- defN 23-Jul-08 09:03 category_encoders/LeaveOneOutEncoder.class
+-rw-rw-r--  2.0 unx     4690 b- defN 23-Jul-08 09:03 category_encoders/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jul-08 09:03 category_encoders/MeanEncoder$MeanFunction.class
+-rw-rw-r--  2.0 unx     1378 b- defN 23-Jul-08 09:03 category_encoders/CatBoostEncoder$1.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Jul-08 09:03 category_encoders/CategoryEncoder.class
+-rw-rw-r--  2.0 unx      725 b- defN 23-Jul-08 09:03 sklego/meta/EstimatorTransformer$1.class
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jul-08 09:03 sklego/meta/EstimatorTransformer.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-extension/
+-rw-rw-r--  2.0 unx     1226 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
+-rw-rw-r--  2.0 unx      118 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
+63 files, 171292 bytes uncompressed, 74759 bytes compressed:  56.4%
```

#### zipnote «TEMP»/diffoscope_ztes36tb_/tmp45oho3gf_.zip

```diff
@@ -1,19 +1,13 @@
 Filename: META-INF/
 Comment: 
 
 Filename: META-INF/MANIFEST.MF
 Comment: 
 
-Filename: mlxtend/
-Comment: 
-
-Filename: mlxtend/preprocessing/
-Comment: 
-
 Filename: pycaret/
 Comment: 
 
 Filename: pycaret/preprocess/
 Comment: 
 
 Filename: tpot/
@@ -36,35 +30,35 @@
 
 Filename: sklego/
 Comment: 
 
 Filename: sklego/meta/
 Comment: 
 
-Filename: sklego/preprocessing/
-Comment: 
-
-Filename: mlxtend/preprocessing/DenseTransformer.class
-Comment: 
-
 Filename: META-INF/sklearn2pmml.properties
 Comment: 
 
 Filename: pycaret/preprocess/FixImbalancer.class
 Comment: 
 
 Filename: pycaret/preprocess/RemoveMulticollinearity.class
 Comment: 
 
 Filename: pycaret/preprocess/CleanColumnNames.class
 Comment: 
 
+Filename: pycaret/preprocess/RemoveOutliers$1.class
+Comment: 
+
 Filename: pycaret/preprocess/RareCategoryGrouping.class
 Comment: 
 
+Filename: pycaret/preprocess/RemoveOutliers.class
+Comment: 
+
 Filename: pycaret/preprocess/TransformerWrapper.class
 Comment: 
 
 Filename: pycaret/preprocess/TransformerWrapperWithInverse.class
 Comment: 
 
 Filename: tpot/builtins/StackingEstimator$1.class
@@ -174,17 +168,14 @@
 
 Filename: sklego/meta/EstimatorTransformer$1.class
 Comment: 
 
 Filename: sklego/meta/EstimatorTransformer.class
 Comment: 
 
-Filename: sklego/preprocessing/IdentityTransformer.class
-Comment: 
-
 Filename: META-INF/maven/
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/pmml-sklearn-extension/
```

#### META-INF/sklearn2pmml.properties

```diff
@@ -26,24 +26,25 @@
 imblearn.under_sampling._prototype_selection._edited_nearest_neighbours.RepeatedEditedNearestNeighbours = imblearn.Sampler
 imblearn.under_sampling._prototype_selection._instance_hardness_threshold.InstanceHardnessThreshold = imblearn.Sampler
 imblearn.under_sampling._prototype_selection._nearmiss.NearMiss = imblearn.Sampler
 imblearn.under_sampling._prototype_selection._neighbourhood_cleaning_rule.NeighbourhoodCleaningRule = imblearn.Sampler
 imblearn.under_sampling._prototype_selection._one_sided_selection.OneSidedSelection = imblearn.Sampler
 imblearn.under_sampling._prototype_selection._random_under_sampler.RandomUnderSampler = imblearn.Sampler
 imblearn.under_sampling._prototype_selection._tomek_links.TomekLinks = imblearn.Sampler
-mlxtend.preprocessing.dense_transformer.DenseTransformer = mlxtend.preprocessing.DenseTransformer
+mlxtend.preprocessing.dense_transformer.DenseTransformer = sklearn.IdentityTransformer
 optbinning.binning.binning.OptimalBinning = optbinning.OptimalBinning
 optbinning.binning.continuous_binning.ContinuousOptimalBinning = optbinning.ContinuousOptimalBinning
 optbinning.binning.binning_process.BinningProcess = optbinning.BinningProcess
 optbinning.binning.multiclass_binning.MulticlassOptimalBinning = optbinning.MulticlassOptimalBinning
 optbinning.scorecard.scorecard.Scorecard = optbinning.scorecard.Scorecard
 pycaret.internal.pipeline.Pipeline = sklearn.pipeline.Pipeline
 pycaret.internal.preprocess.transformers.CleanColumnNames = pycaret.preprocess.CleanColumnNames
 pycaret.internal.preprocess.transformers.FixImbalancer = pycaret.preprocess.FixImbalancer
 pycaret.internal.preprocess.transformers.RareCategoryGrouping = pycaret.preprocess.RareCategoryGrouping
 pycaret.internal.preprocess.transformers.RemoveMulticollinearity = pycaret.preprocess.RemoveMulticollinearity
+pycaret.internal.preprocess.transformers.RemoveOutliers = pycaret.preprocess.RemoveOutliers
 pycaret.internal.preprocess.transformers.TransformerWrapper = pycaret.preprocess.TransformerWrapper
 pycaret.internal.preprocess.transformers.TransformerWrapperWithInverse = pycaret.preprocess.TransformerWrapperWithInverse
 sklego.meta.estimator_transformer.EstimatorTransformer = sklego.meta.EstimatorTransformer
 sklego.pipeline.DebugPipeline = sklearn.pipeline.Pipeline
-sklego.preprocessing.identitytransformer.IdentityTransformer = sklego.preprocessing.IdentityTransformer
+sklego.preprocessing.identitytransformer.IdentityTransformer = sklearn.IdentityTransformer
 tpot.builtins.stacking_estimator.StackingEstimator = tpot.builtins.StackingEstimator
```

#### pycaret/preprocess/FixImbalancer.class

##### procyon -ec {}

```diff
@@ -1,18 +1,11 @@
 
 package pycaret.preprocess;
 
-import org.jpmml.sklearn.SkLearnEncoder;
-import org.jpmml.converter.Feature;
-import java.util.List;
-import sklearn.MultiTransformer;
+import sklearn.IdentityTransformer;
 
-public class FixImbalancer extends MultiTransformer
+public class FixImbalancer extends IdentityTransformer
 {
     public FixImbalancer(final String module, final String name) {
         super(module, name);
     }
-    
-    public List<Feature> encodeFeatures(final List<Feature> features, final SkLearnEncoder encoder) {
-        return features;
-    }
 }
```

#### pycaret/preprocess/CleanColumnNames.class

##### procyon -ec {}

```diff
@@ -1,18 +1,11 @@
 
 package pycaret.preprocess;
 
-import org.jpmml.sklearn.SkLearnEncoder;
-import org.jpmml.converter.Feature;
-import java.util.List;
-import sklearn.MultiTransformer;
+import sklearn.IdentityTransformer;
 
-public class CleanColumnNames extends MultiTransformer
+public class CleanColumnNames extends IdentityTransformer
 {
     public CleanColumnNames(final String module, final String name) {
         super(module, name);
     }
-    
-    public List<Feature> encodeFeatures(final List<Feature> features, final SkLearnEncoder encoder) {
-        return features;
-    }
 }
```

#### pycaret/preprocess/TransformerWrapper.class

##### procyon -ec {}

```diff
@@ -43,15 +43,19 @@
     public List<Feature> initializeFeatures(final SkLearnEncoder encoder) {
         return this.encodeFeatures(Collections.emptyList(), encoder);
     }
     
     public List<Feature> encodeFeatures(List<Feature> features, final SkLearnEncoder encoder) {
         final List<String> featureNamesIn = this.getFeatureNamesIn();
         final List<String> include = this.getInclude();
+        final Boolean trainOnly = this.getTrainOnly();
         final Transformer transformer = this.getTransformer();
+        if ((boolean)trainOnly) {
+            return features;
+        }
         if (features.isEmpty()) {
             features = InitializerUtil.selectFeatures((List)featureNamesIn, (List)features, encoder);
         }
         final List<Feature> includeFeatures = new ArrayList<Feature>();
         for (int i = 0; i < include.size(); ++i) {
             final String includeColumn = (String)include.get(i);
             Feature includeFeature;
@@ -123,14 +127,18 @@
         return this.getList("_exclude", (Class)String.class);
     }
     
     public List<String> getInclude() {
         return this.getList("_include", (Class)String.class);
     }
     
+    public Boolean getTrainOnly() {
+        return this.getOptionalBoolean("_train_only", Boolean.FALSE);
+    }
+    
     public Transformer getTransformer() {
         return (Transformer)this.get("transformer", (Class)Transformer.class);
     }
     
     private static List<List<Feature>> groupByField(final List<Feature> features) {
         final List<List<Feature>> result = new ArrayList<List<Feature>>();
         Field<?> prevField = null;
```

#### optbinning/BinningProcess$1.class

##### procyon -ec {}

```diff
@@ -2,10 +2,10 @@
 package optbinning;
 
 import org.jpmml.python.ClassDictUtil;
 import org.jpmml.python.CastFunction;
 
 class BinningProcess$1 extends CastFunction<OptimalBinning> {
     protected String formatMessage(final Object object) {
-        return "The binning object (" + ClassDictUtil.formatClass(object) + ") is not a supported";
+        return "The binning object (" + ClassDictUtil.formatClass(object) + ") is not supported";
     }
 }
```

#### imblearn/Sampler.class

##### procyon -ec {}

```diff
@@ -1,18 +1,11 @@
 
 package imblearn;
 
-import org.jpmml.sklearn.SkLearnEncoder;
-import org.jpmml.converter.Feature;
-import java.util.List;
-import sklearn.MultiTransformer;
+import sklearn.IdentityTransformer;
 
-public class Sampler extends MultiTransformer
+public class Sampler extends IdentityTransformer
 {
     public Sampler(final String module, final String name) {
         super(module, name);
     }
-    
-    public List<Feature> encodeFeatures(final List<Feature> features, final SkLearnEncoder encoder) {
-        return features;
-    }
 }
```

#### category_encoders/OrdinalMapEncoder$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 04ae45f1ff7100ff86056891900df691b699a98056aed10cd734c113eb3c5a92
+  SHA-256 checksum d83c3409263aafb39bf0c36122bbd7faea6591ded3d3f273e12199376cd7d363
   Compiled from "OrdinalMapEncoder.java"
 class category_encoders.OrdinalMapEncoder$1 extends category_encoders.MapFeature
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #7                          // category_encoders/OrdinalMapEncoder$1
   super_class: #8                         // category_encoders/MapFeature
@@ -79,15 +79,15 @@
          7: aload_3
          8: aload         4
         10: aload         5
         12: aload         6
         14: invokespecial #2                  // Method category_encoders/MapFeature."<init>":(Lorg/jpmml/converter/PMMLEncoder;Lorg/jpmml/converter/Feature;Ljava/util/Map;Ljava/lang/Object;Ljava/lang/Number;)V
         17: return
       LineNumberTable:
-        line 132: 0
+        line 136: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      18     0  this   Lcategory_encoders/OrdinalMapEncoder$1;
             0      18     1 this$0   Lcategory_encoders/OrdinalMapEncoder;
             0      18     2 encoder   Lorg/jpmml/converter/PMMLEncoder;
             0      18     3 feature   Lorg/jpmml/converter/Feature;
             0      18     4 mapping   Ljava/util/Map;
@@ -113,15 +113,15 @@
         16: iconst_0
         17: aload_0
         18: invokevirtual #5                  // Method getName:()Ljava/lang/String;
         21: aastore
         22: invokevirtual #6                  // Method category_encoders/OrdinalMapEncoder.createFieldName:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/String;
         25: areturn
       LineNumberTable:
-        line 136: 0
+        line 140: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      26     0  this   Lcategory_encoders/OrdinalMapEncoder$1;
 }
 SourceFile: "OrdinalMapEncoder.java"
 EnclosingMethod: #36.#37                // category_encoders.OrdinalMapEncoder.encodeFeatures
 InnerClasses:
```

#### category_encoders/OrdinalMapEncoder.class

##### procyon -ec {}

```diff
@@ -10,14 +10,15 @@
 import org.dmg.pmml.Field;
 import org.jpmml.converter.InvalidValueDecorator;
 import org.dmg.pmml.InvalidValueTreatmentMethod;
 import sklearn.preprocessing.EncoderUtil;
 import pandas.core.SeriesUtil;
 import org.jpmml.converter.ValueUtil;
 import pandas.core.Series;
+import numpy.core.ScalarUtil;
 import java.util.ArrayList;
 import org.jpmml.python.ClassDictUtil;
 import java.util.Collection;
 import org.jpmml.sklearn.SkLearnEncoder;
 import org.jpmml.converter.Feature;
 import java.util.List;
 
@@ -108,15 +109,15 @@
             }
         }
         final List<OrdinalEncoder.Mapping> ordinalMappings = ordinalEncoder.getMapping();
         ClassDictUtil.checkSize(new Collection[] { features, cols, ordinalMappings });
         final List<Feature> result = new ArrayList<Feature>();
         for (int i = 0; i < features.size(); ++i) {
             final Feature feature = (Feature)features.get(i);
-            final Object col = cols.get(i);
+            final Object col = ScalarUtil.decode((Object)cols.get(i));
             final OrdinalEncoder.Mapping ordinalMapping = (OrdinalEncoder.Mapping)ordinalMappings.get(i);
             final Map<?, Integer> ordinalCategoryMappings = ordinalMapping.getCategoryMapping();
             final String s3 = handleMissing;
             int n3 = -1;
             switch (s3.hashCode()) {
                 case 96784904: {
                     if (s3.equals("error")) {
@@ -129,14 +130,17 @@
             switch (n3) {
                 case 0: {
                     ordinalCategoryMappings.remove(CategoryEncoder.CATEGORY_NAN);
                     break;
                 }
             }
             final Series series = (Series)mapping.get(col);
+            if (series == null) {
+                throw new IllegalArgumentException(String.valueOf(col));
+            }
             final Map<Integer, Double> valueMappings = SeriesUtil.toMap(series, key -> ValueUtil.asInteger((Number)key), ValueUtil::asDouble);
             final Map<?, Double> categoryValues = mapEncodeValues(ordinalCategoryMappings, valueMappings);
             final List<Object> categories = new ArrayList<Object>(categoryValues.keySet());
             final Field<?> field = (Field<?>)encoder.toCategorical(feature.getName(), EncoderUtil.filterCategories((List)categories));
             Double defaultValue = null;
             final String s4 = handleUnknown;
             int n4 = -1;
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.30</version>
+    <version>1.7.31</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-extension</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn extensions converter</name>
   <description>JPMML Scikit-Learn extension packages to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Mon Jun 19 22:03:16 EEST 2023
-version=1.7.30
+#Sat Jul 08 09:03:24 EEST 2023
+version=1.7.31
 groupId=org.jpmml
 artifactId=pmml-sklearn-extension
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.30.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.31.jar`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 6242 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/statsmodels/
--rw-rw-r--  2.0 unx      152 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2083 b- defN 23-Jun-19 22:03 sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
--rw-rw-r--  2.0 unx     1515 b- defN 23-Jun-19 22:03 sklearn2pmml/statsmodels/StatsModelsClassifier.class
--rw-rw-r--  2.0 unx     1920 b- defN 23-Jun-19 22:03 sklearn2pmml/statsmodels/StatsModelsUtil.class
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-19 22:03 sklearn2pmml/statsmodels/StatsModelsRegressor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
--rw-rw-r--  2.0 unx     1331 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
--rw-rw-r--  2.0 unx      120 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/statsmodels/
+-rw-rw-r--  2.0 unx      152 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Jul-08 09:03 sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Jul-08 09:03 sklearn2pmml/statsmodels/StatsModelsClassifier.class
+-rw-rw-r--  2.0 unx     1920 b- defN 23-Jul-08 09:03 sklearn2pmml/statsmodels/StatsModelsUtil.class
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-08 09:03 sklearn2pmml/statsmodels/StatsModelsRegressor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
+-rw-rw-r--  2.0 unx     1331 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
+-rw-rw-r--  2.0 unx      120 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
 14 files, 8762 bytes uncompressed, 4120 bytes compressed:  53.0%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.30</version>
+    <version>1.7.31</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-statsmodels</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn StatsModels converter</name>
   <description>JPMML Scikit-Learn StatsModels to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Mon Jun 19 22:03:17 EEST 2023
-version=1.7.30
+#Sat Jul 08 09:03:24 EEST 2023
+version=1.7.31
 groupId=org.jpmml
 artifactId=pmml-sklearn-statsmodels
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.30.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.31.jar`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7310 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 lightgbm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 lightgbm/sklearn/
--rw-rw-r--  2.0 unx      177 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      170 b- defN 23-Jun-19 22:03 lightgbm/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     1953 b- defN 23-Jun-19 22:03 lightgbm/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2102 b- defN 23-Jun-19 22:03 lightgbm/sklearn/LGBMRegressor.class
--rw-rw-r--  2.0 unx     2126 b- defN 23-Jun-19 22:03 lightgbm/sklearn/LGBMClassifier.class
--rw-rw-r--  2.0 unx     3298 b- defN 23-Jun-19 22:03 lightgbm/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
--rw-rw-r--  2.0 unx     1319 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
--rw-rw-r--  2.0 unx      117 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
-15 files, 11392 bytes uncompressed, 5230 bytes compressed:  54.1%
+Zip file size: 7311 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 lightgbm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 lightgbm/sklearn/
+-rw-rw-r--  2.0 unx      177 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      170 b- defN 23-Jul-08 09:03 lightgbm/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     1953 b- defN 23-Jul-08 09:03 lightgbm/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2102 b- defN 23-Jul-08 09:03 lightgbm/sklearn/LGBMRegressor.class
+-rw-rw-r--  2.0 unx     2126 b- defN 23-Jul-08 09:03 lightgbm/sklearn/LGBMClassifier.class
+-rw-rw-r--  2.0 unx     3298 b- defN 23-Jul-08 09:03 lightgbm/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
+-rw-rw-r--  2.0 unx     1319 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
+-rw-rw-r--  2.0 unx      117 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
+15 files, 11392 bytes uncompressed, 5231 bytes compressed:  54.1%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.30</version>
+    <version>1.7.31</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-lightgbm</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn LightGBM converter</name>
   <description>JPMML Scikit-Learn LightGBM to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Mon Jun 19 22:03:17 EEST 2023
-version=1.7.30
+#Sat Jul 08 09:03:24 EEST 2023
+version=1.7.31
 groupId=org.jpmml
 artifactId=pmml-sklearn-lightgbm
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/classpath.txt` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/classpath.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 sklearn2pmml-1.0-SNAPSHOT.jar
 gson-2.10.jar
 guava-21.0.jar
-h2o-genmodel-3.40.0.4.jar
-h2o-logger-3.40.0.4.jar
+h2o-genmodel-3.42.0.1.jar
+h2o-logger-3.42.0.1.jar
 h2o-tree-api-0.3.17.jar
 istack-commons-runtime-4.0.1.jar
 jackson-annotations-2.13.3.jar
 jakarta.activation-2.0.1.jar
 jakarta.xml.bind-api-3.0.1.jar
 jaxb-core-3.0.2.jar
 jaxb-runtime-3.0.2.jar
@@ -14,20 +14,20 @@
 pickle-1.4.jar
 pmml-converter-1.5.4.jar
 pmml-h2o-1.2.7.jar
 pmml-lightgbm-1.4.5.jar
 pmml-model-1.6.4.jar
 pmml-model-metro-1.6.4.jar
 pmml-python-1.1.15.jar
-pmml-sklearn-1.7.30.jar
-pmml-sklearn-extension-1.7.30.jar
-pmml-sklearn-h2o-1.7.30.jar
-pmml-sklearn-lightgbm-1.7.30.jar
-pmml-sklearn-statsmodels-1.7.30.jar
-pmml-sklearn-xgboost-1.7.30.jar
+pmml-sklearn-1.7.31.jar
+pmml-sklearn-extension-1.7.31.jar
+pmml-sklearn-h2o-1.7.31.jar
+pmml-sklearn-lightgbm-1.7.31.jar
+pmml-sklearn-statsmodels-1.7.31.jar
+pmml-sklearn-xgboost-1.7.31.jar
 pmml-statsmodels-1.0.4.jar
 pmml-xgboost-1.7.3.jar
 serpent-1.40.jar
 slf4j-api-1.7.36.jar
 slf4j-jdk14-1.7.36.jar
 ubjson-0.1.8.jar
 ubjson-gson-0.1.8.jar
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/h2o-logger-3.40.0.4.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-logger-3.42.0.1.jar`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 4526 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-28 12:08 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 water/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Apr-28 12:08 water/logging/
--rw-r--r--  2.0 unx     1853 b- defN 23-Apr-28 12:08 water/logging/Slf4JLogger.class
--rw-r--r--  2.0 unx      379 b- defN 23-Apr-28 12:08 water/logging/Logger.class
--rw-r--r--  2.0 unx     2473 b- defN 23-Apr-28 12:08 water/logging/LoggerFactory.class
--rw-r--r--  2.0 unx     1686 b- defN 23-Apr-28 12:08 water/logging/ConsoleLogger.class
--rw-r--r--  2.0 unx     1114 b- defN 23-Apr-28 12:08 water/logging/LoggingLevel.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:49 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-20 17:49 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 water/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-20 17:48 water/logging/
+-rw-r--r--  2.0 unx     1853 b- defN 23-Jun-20 17:48 water/logging/Slf4JLogger.class
+-rw-r--r--  2.0 unx      379 b- defN 23-Jun-20 17:48 water/logging/Logger.class
+-rw-r--r--  2.0 unx     2473 b- defN 23-Jun-20 17:48 water/logging/LoggerFactory.class
+-rw-r--r--  2.0 unx     1686 b- defN 23-Jun-20 17:48 water/logging/ConsoleLogger.class
+-rw-r--r--  2.0 unx     1114 b- defN 23-Jun-20 17:48 water/logging/LoggingLevel.class
 9 files, 7530 bytes uncompressed, 3412 bytes compressed:  54.7%
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-h2o-1.2.7.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-h2o-1.2.7.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5703 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-Jun-19 22:18 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 com/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 com/sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 META-INF/maven/com.sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:18 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
--rw-rw-r--  2.0 unx     3741 b- defN 23-Jun-19 22:18 com/sklearn2pmml/Main.class
--rw-rw-r--  2.0 unx     1200 b- defN 23-Jun-19 22:18 com/sklearn2pmml/Main$1.class
--rw-rw-r--  2.0 unx     7844 b- defN 23-Jun-19 22:18 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
--rw-rw-r--  2.0 unx       70 b- defN 23-Jun-19 22:18 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
-11 files, 13013 bytes uncompressed, 4227 bytes compressed:  67.5%
+Zip file size: 5711 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-Jul-08 09:24 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 com/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 com/sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 META-INF/maven/com.sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
+-rw-rw-r--  2.0 unx     3741 b- defN 23-Jul-08 09:24 com/sklearn2pmml/Main.class
+-rw-rw-r--  2.0 unx     1200 b- defN 23-Jul-08 09:24 com/sklearn2pmml/Main$1.class
+-rw-rw-r--  2.0 unx     7844 b- defN 23-Jul-08 09:23 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
+-rw-rw-r--  2.0 unx       70 b- defN 23-Jul-08 09:24 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
+11 files, 13013 bytes uncompressed, 4235 bytes compressed:  67.5%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: SkLearn2PMML package
-Implementation-Version: 0.94.0
+Implementation-Version: 0.94.1
 Build-Jdk-Spec: 1.8
-Created-By: Maven JAR Plugin 3.2.2
+Created-By: Maven JAR Plugin 3.3.0
```

#### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

##### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

```diff
@@ -24,15 +24,15 @@
     <tag>HEAD</tag>
   </scm>
   <issueManagement>
     <system>GitHub</system>
     <url>https://github.com/jpmml/sklearn2pmml/issues</url>
   </issueManagement>
   <properties>
-    <jpmml-sklearn.version>1.7.30</jpmml-sklearn.version>
+    <jpmml-sklearn.version>1.7.31</jpmml-sklearn.version>
   </properties>
   <dependencies>
     <dependency>
       <groupId>org.jpmml</groupId>
       <artifactId>pmml-sklearn</artifactId>
       <version>${jpmml-sklearn.version}</version>
       <exclusions>
@@ -123,24 +123,24 @@
             </configuration>
           </execution>
         </executions>
       </plugin>
       <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-compiler-plugin</artifactId>
-        <version>3.10.1</version>
+        <version>3.11.0</version>
         <configuration>
           <source>1.8</source>
           <target>1.8</target>
         </configuration>
       </plugin>
       <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-dependency-plugin</artifactId>
-        <version>3.3.0</version>
+        <version>3.6.0</version>
         <executions>
           <execution>
             <id>copy-dependencies</id>
             <phase>generate-resources</phase>
             <goals>
               <goal>copy-dependencies</goal>
             </goals>
@@ -149,28 +149,28 @@
             </configuration>
           </execution>
         </executions>
       </plugin>
       <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-jar-plugin</artifactId>
-        <version>3.2.2</version>
+        <version>3.3.0</version>
         <configuration>
           <archive>
             <manifestEntries>
               <Implementation-Title>SkLearn2PMML package</Implementation-Title>
               <Implementation-Version>${sklearn2pmml.version}</Implementation-Version>
             </manifestEntries>
           </archive>
         </configuration>
       </plugin>
       <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-resources-plugin</artifactId>
-        <version>3.2.0</version>
+        <version>3.3.1</version>
         <executions>
           <execution>
             <phase>package</phase>
             <goals>
               <goal>copy-resources</goal>
             </goals>
             <configuration>
@@ -235,15 +235,15 @@
             </configuration>
           </execution>
         </executions>
       </plugin>
       <plugin>
         <groupId>org.codehaus.mojo</groupId>
         <artifactId>build-helper-maven-plugin</artifactId>
-        <version>3.3.0</version>
+        <version>3.4.0</version>
         <executions>
           <execution>
             <phase>initialize</phase>
             <goals>
               <goal>regex-property</goal>
             </goals>
             <configuration>
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pmml-sklearn-1.7.30.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-1.7.31.jar`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,405 +1,407 @@
-Zip file size: 468727 bytes, number of entries: 403
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/
--rw-r--r--  2.0 unx      159 b- defN 23-Jun-19 22:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn_pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 chaid/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 stop_words/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/calibration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/dummy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/svm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/impute/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/naive_bayes/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/linear_model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/linear_model/logistic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/linear_model/ridge/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/linear_model/glm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/compose/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/model_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/decomposition/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/neighbors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/multioutput/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/isotonic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/bagging/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/stacking/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/forest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/iforest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/voting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/ensemble/weight_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/loss/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/discriminant_analysis/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/tree/visitors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/cluster/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn/multiclass/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/ruleset/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/decoration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/util/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/postprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 sklearn2pmml/expression/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 org/jpmml/sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 org/jpmml/sklearn/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn/
--rw-rw-r--  2.0 unx    16829 b- defN 23-Jun-19 22:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2287 b- defN 23-Jun-19 22:03 sklearn_pandas/CategoricalImputer.class
--rw-rw-r--  2.0 unx      656 b- defN 23-Jun-19 22:03 sklearn_pandas/TransformerPipeline.class
--rw-rw-r--  2.0 unx     1154 b- defN 23-Jun-19 22:03 sklearn_pandas/DataFrameMapper$2.class
--rw-rw-r--  2.0 unx     6280 b- defN 23-Jun-19 22:03 sklearn_pandas/DataFrameMapper.class
--rw-rw-r--  2.0 unx     1126 b- defN 23-Jun-19 22:03 sklearn_pandas/DataFrameMapper$1.class
--rw-rw-r--  2.0 unx      609 b- defN 23-Jun-19 22:03 chaid/ContinuousColumn.class
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-19 22:03 chaid/Node.class
--rw-rw-r--  2.0 unx      467 b- defN 23-Jun-19 22:03 chaid/Column.class
--rw-rw-r--  2.0 unx     3283 b- defN 23-Jun-19 22:03 chaid/Split.class
--rw-rw-r--  2.0 unx      401 b- defN 23-Jun-19 22:03 chaid/InvalidSplitReason.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Jun-19 22:03 chaid/NominalColumn.class
--rw-rw-r--  2.0 unx     1912 b- defN 23-Jun-19 22:03 stop_words/english.txt
--rw-rw-r--  2.0 unx      147 b- defN 23-Jun-19 22:03 sklearn/HasHead.class
--rw-rw-r--  2.0 unx     1728 b- defN 23-Jun-19 22:03 sklearn/StepUtil.class
--rw-rw-r--  2.0 unx    12044 b- defN 23-Jun-19 22:03 sklearn/calibration/CalibratedClassifier.class
--rw-rw-r--  2.0 unx     2953 b- defN 23-Jun-19 22:03 sklearn/calibration/SigmoidCalibration.class
--rw-rw-r--  2.0 unx      683 b- defN 23-Jun-19 22:03 sklearn/calibration/CalibratedClassifier$1.class
--rw-rw-r--  2.0 unx     3672 b- defN 23-Jun-19 22:03 sklearn/calibration/CalibratedClassifierCV.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Jun-19 22:03 sklearn/pipeline/PipelineTransformer.class
--rw-rw-r--  2.0 unx     1671 b- defN 23-Jun-19 22:03 sklearn/pipeline/Pipeline$2.class
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-19 22:03 sklearn/pipeline/FeatureUnion.class
--rw-rw-r--  2.0 unx     5062 b- defN 23-Jun-19 22:03 sklearn/pipeline/Pipeline.class
--rw-rw-r--  2.0 unx     2003 b- defN 23-Jun-19 22:03 sklearn/pipeline/PipelineRegressor.class
--rw-rw-r--  2.0 unx     1773 b- defN 23-Jun-19 22:03 sklearn/pipeline/Pipeline$1.class
--rw-rw-r--  2.0 unx     1111 b- defN 23-Jun-19 22:03 sklearn/pipeline/PipelineUtil.class
--rw-rw-r--  2.0 unx     2298 b- defN 23-Jun-19 22:03 sklearn/pipeline/PipelineClassifier.class
--rw-rw-r--  2.0 unx     4913 b- defN 23-Jun-19 22:03 sklearn/dummy/DummyClassifier.class
--rw-rw-r--  2.0 unx     2055 b- defN 23-Jun-19 22:03 sklearn/dummy/DummyRegressor.class
--rw-rw-r--  2.0 unx      454 b- defN 23-Jun-19 22:03 sklearn/SkLearnFields.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-Jun-19 22:03 sklearn/SkLearnOutlierTransformation.class
--rw-rw-r--  2.0 unx      240 b- defN 23-Jun-19 22:03 sklearn/HasEstimator.class
--rw-rw-r--  2.0 unx     3456 b- defN 23-Jun-19 22:03 sklearn/OutlierDetectorUtil.class
--rw-rw-r--  2.0 unx     1258 b- defN 23-Jun-19 22:03 sklearn/HasMultiApplyField.class
--rw-rw-r--  2.0 unx      908 b- defN 23-Jun-19 22:03 sklearn/None.class
--rw-rw-r--  2.0 unx     2393 b- defN 23-Jun-19 22:03 sklearn/svm/SupportVectorMachineUtil.class
--rw-rw-r--  2.0 unx     1109 b- defN 23-Jun-19 22:03 sklearn/svm/LinearSVC.class
--rw-rw-r--  2.0 unx     5037 b- defN 23-Jun-19 22:03 sklearn/svm/LibSVMClassifier.class
--rw-rw-r--  2.0 unx      966 b- defN 23-Jun-19 22:03 sklearn/svm/SupportVectorMachineUtil$1.class
--rw-rw-r--  2.0 unx     1305 b- defN 23-Jun-19 22:03 sklearn/svm/OneClassSVM.class
--rw-rw-r--  2.0 unx     3594 b- defN 23-Jun-19 22:03 sklearn/svm/LibSVMRegressor.class
--rw-rw-r--  2.0 unx     4114 b- defN 23-Jun-19 22:03 sklearn/InitializerUtil$1.class
--rw-rw-r--  2.0 unx      735 b- defN 23-Jun-19 22:03 sklearn/Estimator$1.class
--rw-rw-r--  2.0 unx      342 b- defN 23-Jun-19 22:03 sklearn/HasOutlierField.class
--rw-rw-r--  2.0 unx      214 b- defN 23-Jun-19 22:03 sklearn/HasNumberOfFeatures.class
--rw-rw-r--  2.0 unx      660 b- defN 23-Jun-19 22:03 sklearn/MultiTransformer.class
--rw-rw-r--  2.0 unx     2110 b- defN 23-Jun-19 22:03 sklearn/neural_network/MLPRegressor.class
--rw-rw-r--  2.0 unx     2555 b- defN 23-Jun-19 22:03 sklearn/neural_network/MLPClassifier.class
--rw-rw-r--  2.0 unx      759 b- defN 23-Jun-19 22:03 sklearn/neural_network/MultilayerPerceptronUtil$1.class
--rw-rw-r--  2.0 unx    10661 b- defN 23-Jun-19 22:03 sklearn/neural_network/MultilayerPerceptronUtil.class
--rw-rw-r--  2.0 unx      853 b- defN 23-Jun-19 22:03 sklearn/Step.class
--rw-rw-r--  2.0 unx      168 b- defN 23-Jun-19 22:03 sklearn/HasDefaultValue.class
--rw-rw-r--  2.0 unx     2936 b- defN 23-Jun-19 22:03 sklearn/impute/MissingIndicator.class
--rw-rw-r--  2.0 unx     4027 b- defN 23-Jun-19 22:03 sklearn/impute/ImputerUtil.class
--rw-rw-r--  2.0 unx     5703 b- defN 23-Jun-19 22:03 sklearn/impute/SimpleImputer.class
--rw-rw-r--  2.0 unx     6948 b- defN 23-Jun-19 22:03 sklearn/naive_bayes/GaussianNB.class
--rw-rw-r--  2.0 unx     4434 b- defN 23-Jun-19 22:03 sklearn/linear_model/LinearRegressor.class
--rw-rw-r--  2.0 unx     5040 b- defN 23-Jun-19 22:03 sklearn/linear_model/LinearClassifier.class
--rw-rw-r--  2.0 unx     7648 b- defN 23-Jun-19 22:03 sklearn/linear_model/logistic/LogisticRegression.class
--rw-rw-r--  2.0 unx     1042 b- defN 23-Jun-19 22:03 sklearn/linear_model/ridge/RidgeClassifier.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Jun-19 22:03 sklearn/linear_model/glm/DistributionBoundary.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Jun-19 22:03 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/Hinge.class
--rw-rw-r--  2.0 unx     2480 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
--rw-rw-r--  2.0 unx      461 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/LossFunction.class
--rw-rw-r--  2.0 unx      452 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/Log.class
--rw-rw-r--  2.0 unx     1165 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
--rw-rw-r--  2.0 unx      482 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
--rw-rw-r--  2.0 unx      932 b- defN 23-Jun-19 22:03 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
--rw-rw-r--  2.0 unx     1720 b- defN 23-Jun-19 22:03 sklearn/compose/ColumnTransformer$1.class
--rw-rw-r--  2.0 unx     3239 b- defN 23-Jun-19 22:03 sklearn/compose/TransformedTargetRegressor.class
--rw-rw-r--  2.0 unx     3649 b- defN 23-Jun-19 22:03 sklearn/compose/ColumnTransformer.class
--rw-rw-r--  2.0 unx     1534 b- defN 23-Jun-19 22:03 sklearn/compose/TransformedTargetRegressor$1.class
--rw-rw-r--  2.0 unx     4089 b- defN 23-Jun-19 22:03 sklearn/Classifier.class
--rw-rw-r--  2.0 unx     1457 b- defN 23-Jun-19 22:03 sklearn/model_selection/EstimatorSearcher.class
--rw-rw-r--  2.0 unx     1685 b- defN 23-Jun-19 22:03 sklearn/Selector.class
--rw-rw-r--  2.0 unx      419 b- defN 23-Jun-19 22:03 sklearn/decomposition/IncrementalPCA.class
--rw-rw-r--  2.0 unx     3471 b- defN 23-Jun-19 22:03 sklearn/decomposition/TruncatedSVD.class
--rw-rw-r--  2.0 unx     4759 b- defN 23-Jun-19 22:03 sklearn/decomposition/PCA.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Jun-19 22:03 sklearn/decomposition/BasePCA.class
--rw-rw-r--  2.0 unx      336 b- defN 23-Jun-19 22:03 sklearn/HasPredictField.class
--rw-rw-r--  2.0 unx     3018 b- defN 23-Jun-19 22:03 sklearn/neighbors/NearestNeighbors.class
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-19 22:03 sklearn/neighbors/KNeighborsClassifier.class
--rw-rw-r--  2.0 unx     3794 b- defN 23-Jun-19 22:03 sklearn/neighbors/NearestCentroid.class
--rw-rw-r--  2.0 unx     2025 b- defN 23-Jun-19 22:03 sklearn/neighbors/BinaryTree.class
--rw-rw-r--  2.0 unx     1266 b- defN 23-Jun-19 22:03 sklearn/neighbors/KNeighborsUtil$1.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Jun-19 22:03 sklearn/neighbors/HasMetric.class
--rw-rw-r--  2.0 unx    10733 b- defN 23-Jun-19 22:03 sklearn/neighbors/KNeighborsUtil.class
--rw-rw-r--  2.0 unx     4387 b- defN 23-Jun-19 22:03 sklearn/neighbors/KNeighborsRegressor.class
--rw-rw-r--  2.0 unx     1032 b- defN 23-Jun-19 22:03 sklearn/neighbors/DistanceMetric.class
--rw-rw-r--  2.0 unx      351 b- defN 23-Jun-19 22:03 sklearn/neighbors/HasTrainingData.class
--rw-rw-r--  2.0 unx      176 b- defN 23-Jun-19 22:03 sklearn/neighbors/HasNumberOfNeighbors.class
--rw-rw-r--  2.0 unx     2654 b- defN 23-Jun-19 22:03 sklearn/multioutput/MultiOutputUtil.class
--rw-rw-r--  2.0 unx     3510 b- defN 23-Jun-19 22:03 sklearn/multioutput/ChainUtil.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Jun-19 22:03 sklearn/multioutput/RegressorChain.class
--rw-rw-r--  2.0 unx     1316 b- defN 23-Jun-19 22:03 sklearn/multioutput/MultiOutputClassifier.class
--rw-rw-r--  2.0 unx     1310 b- defN 23-Jun-19 22:03 sklearn/multioutput/MultiOutputRegressor.class
--rw-rw-r--  2.0 unx     1745 b- defN 23-Jun-19 22:03 sklearn/multioutput/ClassifierChain.class
--rw-rw-r--  2.0 unx     4450 b- defN 23-Jun-19 22:03 sklearn/isotonic/IsotonicRegression.class
--rw-rw-r--  2.0 unx      326 b- defN 23-Jun-19 22:03 sklearn/HasApplyField.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Jun-19 22:03 sklearn/HasEstimatorEnsemble.class
--rw-rw-r--  2.0 unx     1929 b- defN 23-Jun-19 22:03 sklearn/Transformer$1.class
--rw-rw-r--  2.0 unx      953 b- defN 23-Jun-19 22:03 sklearn/LabelEncoderClassifier.class
--rw-rw-r--  2.0 unx      937 b- defN 23-Jun-19 22:03 sklearn/PassThrough.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Jun-19 22:03 sklearn/HasPriorProbability.class
--rw-rw-r--  2.0 unx     5693 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/TfidfVectorizer.class
--rw-rw-r--  2.0 unx      809 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/TfidfVectorizer$1.class
--rw-rw-r--  2.0 unx      675 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/Tokenizer.class
--rw-rw-r--  2.0 unx    13329 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/CountVectorizer.class
--rw-rw-r--  2.0 unx     2129 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/CountVectorizer$1.class
--rw-rw-r--  2.0 unx     1433 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/text/TfidfTransformer.class
--rw-rw-r--  2.0 unx     4031 b- defN 23-Jun-19 22:03 sklearn/feature_extraction/DictVectorizer.class
--rw-rw-r--  2.0 unx      762 b- defN 23-Jun-19 22:03 sklearn/Clusterer.class
--rw-rw-r--  2.0 unx     1375 b- defN 23-Jun-19 22:03 sklearn/metrics/DistanceMetric.class
--rw-rw-r--  2.0 unx     1069 b- defN 23-Jun-19 22:03 sklearn/ensemble/EnsembleUtil.class
--rw-rw-r--  2.0 unx     2112 b- defN 23-Jun-19 22:03 sklearn/ensemble/bagging/BaggingRegressor.class
--rw-rw-r--  2.0 unx     3293 b- defN 23-Jun-19 22:03 sklearn/ensemble/bagging/BaggingUtil.class
--rw-rw-r--  2.0 unx     3031 b- defN 23-Jun-19 22:03 sklearn/ensemble/bagging/BaggingClassifier.class
--rw-rw-r--  2.0 unx     1409 b- defN 23-Jun-19 22:03 sklearn/ensemble/EnsembleRegressor.class
--rw-rw-r--  2.0 unx     3485 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingClassifier.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
--rw-rw-r--  2.0 unx     3109 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingRegressor.class
--rw-rw-r--  2.0 unx     3862 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingUtil.class
--rw-rw-r--  2.0 unx     2524 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingClassifier$1.class
--rw-rw-r--  2.0 unx     2254 b- defN 23-Jun-19 22:03 sklearn/ensemble/stacking/StackingRegressor$1.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
--rw-rw-r--  2.0 unx     2563 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
--rw-rw-r--  2.0 unx      858 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/LossFunction.class
--rw-rw-r--  2.0 unx     1588 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
--rw-rw-r--  2.0 unx     1317 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
--rw-rw-r--  2.0 unx     7948 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
--rw-rw-r--  2.0 unx      960 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/MeanEstimator.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
--rw-rw-r--  2.0 unx     1578 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
--rw-rw-r--  2.0 unx      811 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
--rw-rw-r--  2.0 unx     3003 b- defN 23-Jun-19 22:03 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
--rw-rw-r--  2.0 unx     1148 b- defN 23-Jun-19 22:03 sklearn/ensemble/EnsembleUtil$1.class
--rw-rw-r--  2.0 unx     3059 b- defN 23-Jun-19 22:03 sklearn/ensemble/forest/ForestUtil.class
--rw-rw-r--  2.0 unx     2311 b- defN 23-Jun-19 22:03 sklearn/ensemble/forest/ForestRegressor.class
--rw-rw-r--  2.0 unx     2770 b- defN 23-Jun-19 22:03 sklearn/ensemble/forest/ForestClassifier.class
--rw-rw-r--  2.0 unx     1752 b- defN 23-Jun-19 22:03 sklearn/ensemble/iforest/IsolationForest$3.class
--rw-rw-r--  2.0 unx     2206 b- defN 23-Jun-19 22:03 sklearn/ensemble/iforest/IsolationForest$1.class
--rw-rw-r--  2.0 unx     1716 b- defN 23-Jun-19 22:03 sklearn/ensemble/iforest/IsolationForest$2.class
--rw-rw-r--  2.0 unx     8265 b- defN 23-Jun-19 22:03 sklearn/ensemble/iforest/IsolationForest.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Jun-19 22:03 sklearn/ensemble/voting/VotingClassifier.class
--rw-rw-r--  2.0 unx     3716 b- defN 23-Jun-19 22:03 sklearn/ensemble/voting/VotingRegressor.class
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
--rw-rw-r--  2.0 unx     1247 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
--rw-rw-r--  2.0 unx     3041 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
--rw-rw-r--  2.0 unx     6152 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
--rw-rw-r--  2.0 unx      505 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
--rw-rw-r--  2.0 unx      490 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
--rw-rw-r--  2.0 unx     1572 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
--rw-rw-r--  2.0 unx     6377 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     8868 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
--rw-rw-r--  2.0 unx      441 b- defN 23-Jun-19 22:03 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-19 22:03 sklearn/ensemble/EnsembleClassifier.class
--rw-rw-r--  2.0 unx     3564 b- defN 23-Jun-19 22:03 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
--rw-rw-r--  2.0 unx     6043 b- defN 23-Jun-19 22:03 sklearn/Transformer.class
--rw-rw-r--  2.0 unx      859 b- defN 23-Jun-19 22:03 sklearn/Transformer$1$1.class
--rw-rw-r--  2.0 unx      981 b- defN 23-Jun-19 22:03 sklearn/Drop.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-19 22:03 sklearn/feature_selection/SelectKBest$Entry.class
--rw-rw-r--  2.0 unx     3486 b- defN 23-Jun-19 22:03 sklearn/feature_selection/SelectFromModel.class
--rw-rw-r--  2.0 unx     2922 b- defN 23-Jun-19 22:03 sklearn/feature_selection/SelectKBest.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Jun-19 22:03 sklearn/feature_selection/PySelector.class
--rw-rw-r--  2.0 unx      607 b- defN 23-Jun-19 22:03 sklearn/Transformer$2.class
--rw-rw-r--  2.0 unx     2216 b- defN 23-Jun-19 22:03 sklearn/SkLearnUtil.class
--rw-rw-r--  2.0 unx      412 b- defN 23-Jun-19 22:03 sklearn/loss/HalfMultinomialLoss.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Jun-19 22:03 sklearn/loss/CyLossFunction.class
--rw-rw-r--  2.0 unx      403 b- defN 23-Jun-19 22:03 sklearn/loss/HalfBinomialLoss.class
--rw-rw-r--  2.0 unx      387 b- defN 23-Jun-19 22:03 sklearn/loss/BaseLoss.class
--rw-rw-r--  2.0 unx      381 b- defN 23-Jun-19 22:03 sklearn/HasDecisionFunctionField.class
--rw-rw-r--  2.0 unx      338 b- defN 23-Jun-19 22:03 sklearn/SkLearnMethods.class
--rw-rw-r--  2.0 unx     5114 b- defN 23-Jun-19 22:03 sklearn/ScalarLabelUtil.class
--rw-rw-r--  2.0 unx     1515 b- defN 23-Jun-19 22:03 sklearn/OutlierDetectorUtil$1.class
--rw-rw-r--  2.0 unx      195 b- defN 23-Jun-19 22:03 sklearn/HasClasses.class
--rw-rw-r--  2.0 unx     4685 b- defN 23-Jun-19 22:03 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
--rw-rw-r--  2.0 unx      696 b- defN 23-Jun-19 22:03 sklearn/EstimatorUtil$1.class
--rw-rw-r--  2.0 unx     3311 b- defN 23-Jun-19 22:03 sklearn/Composite.class
--rw-rw-r--  2.0 unx     1194 b- defN 23-Jun-19 22:03 sklearn/preprocessing/KBinsDiscretizer$1.class
--rw-rw-r--  2.0 unx     4567 b- defN 23-Jun-19 22:03 sklearn/preprocessing/PowerTransformer.class
--rw-rw-r--  2.0 unx     2381 b- defN 23-Jun-19 22:03 sklearn/preprocessing/LabelEncoder.class
--rw-rw-r--  2.0 unx     4924 b- defN 23-Jun-19 22:03 sklearn/preprocessing/LabelBinarizer.class
--rw-rw-r--  2.0 unx      729 b- defN 23-Jun-19 22:03 sklearn/preprocessing/EncoderUtil$3.class
--rw-rw-r--  2.0 unx      389 b- defN 23-Jun-19 22:03 sklearn/preprocessing/Scaler.class
--rw-rw-r--  2.0 unx     3242 b- defN 23-Jun-19 22:03 sklearn/preprocessing/MaxAbsScaler.class
--rw-rw-r--  2.0 unx     2948 b- defN 23-Jun-19 22:03 sklearn/preprocessing/FunctionTransformer.class
--rw-rw-r--  2.0 unx     3291 b- defN 23-Jun-19 22:03 sklearn/preprocessing/BaseEncoder.class
--rw-rw-r--  2.0 unx     1270 b- defN 23-Jun-19 22:03 sklearn/preprocessing/EncoderUtil$1.class
--rw-rw-r--  2.0 unx     4549 b- defN 23-Jun-19 22:03 sklearn/preprocessing/StandardScaler.class
--rw-rw-r--  2.0 unx     6971 b- defN 23-Jun-19 22:03 sklearn/preprocessing/EncoderUtil.class
--rw-rw-r--  2.0 unx     6343 b- defN 23-Jun-19 22:03 sklearn/preprocessing/PolynomialFeatures.class
--rw-rw-r--  2.0 unx     8486 b- defN 23-Jun-19 22:03 sklearn/preprocessing/KBinsDiscretizer.class
--rw-rw-r--  2.0 unx     4671 b- defN 23-Jun-19 22:03 sklearn/preprocessing/OneHotEncoder.class
--rw-rw-r--  2.0 unx     2553 b- defN 23-Jun-19 22:03 sklearn/preprocessing/Binarizer.class
--rw-rw-r--  2.0 unx     1054 b- defN 23-Jun-19 22:03 sklearn/preprocessing/EncoderUtil$2.class
--rw-rw-r--  2.0 unx     3595 b- defN 23-Jun-19 22:03 sklearn/preprocessing/MinMaxScaler.class
--rw-rw-r--  2.0 unx     4467 b- defN 23-Jun-19 22:03 sklearn/preprocessing/RobustScaler.class
--rw-rw-r--  2.0 unx     3740 b- defN 23-Jun-19 22:03 sklearn/preprocessing/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      957 b- defN 23-Jun-19 22:03 sklearn/preprocessing/Imputer.class
--rw-rw-r--  2.0 unx     2033 b- defN 23-Jun-19 22:03 sklearn/preprocessing/PolynomialFeatures$1.class
--rw-rw-r--  2.0 unx     7408 b- defN 23-Jun-19 22:03 sklearn/preprocessing/MultiOneHotEncoder.class
--rw-rw-r--  2.0 unx     2153 b- defN 23-Jun-19 22:03 sklearn/tree/TreeClassifier.class
--rw-rw-r--  2.0 unx     3111 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$1.class
--rw-rw-r--  2.0 unx     2664 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$4.class
--rw-rw-r--  2.0 unx     4805 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelFlattener.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelCompactor$1.class
--rw-rw-r--  2.0 unx     5431 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelCompactor.class
--rw-rw-r--  2.0 unx     2988 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelPruner.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelFlattener$1.class
--rw-rw-r--  2.0 unx      730 b- defN 23-Jun-19 22:03 sklearn/tree/visitors/TreeModelPruner$1.class
--rw-rw-r--  2.0 unx     1489 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$8.class
--rw-rw-r--  2.0 unx      879 b- defN 23-Jun-19 22:03 sklearn/tree/RegressionCriterion.class
--rw-rw-r--  2.0 unx     1151 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$5.class
--rw-rw-r--  2.0 unx      978 b- defN 23-Jun-19 22:03 sklearn/tree/PresortBestSplitter.class
--rw-rw-r--  2.0 unx      955 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$6.class
--rw-rw-r--  2.0 unx     1764 b- defN 23-Jun-19 22:03 sklearn/tree/TreeRegressor.class
--rw-rw-r--  2.0 unx     1589 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$7.class
--rw-rw-r--  2.0 unx    20072 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$3.class
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-19 22:03 sklearn/tree/HasTreeOptions.class
--rw-rw-r--  2.0 unx     2257 b- defN 23-Jun-19 22:03 sklearn/tree/Tree.class
--rw-rw-r--  2.0 unx      754 b- defN 23-Jun-19 22:03 sklearn/tree/TreeUtil$2.class
--rw-rw-r--  2.0 unx      150 b- defN 23-Jun-19 22:03 sklearn/tree/HasTree.class
--rw-rw-r--  2.0 unx     1967 b- defN 23-Jun-19 22:03 sklearn/InitializerUtil.class
--rw-rw-r--  2.0 unx      570 b- defN 23-Jun-19 22:03 sklearn/Regressor.class
--rw-rw-r--  2.0 unx      211 b- defN 23-Jun-19 22:03 sklearn/HasNumberOfOutputs.class
--rw-rw-r--  2.0 unx      494 b- defN 23-Jun-19 22:03 sklearn/OutlierDetector.class
--rw-rw-r--  2.0 unx     2808 b- defN 23-Jun-19 22:03 sklearn/Calibrator.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Jun-19 22:03 sklearn/HasClassifierOptions.class
--rw-rw-r--  2.0 unx     7075 b- defN 23-Jun-19 22:03 sklearn/EstimatorUtil.class
--rw-rw-r--  2.0 unx      199 b- defN 23-Jun-19 22:03 sklearn/HasType.class
--rw-rw-r--  2.0 unx      678 b- defN 23-Jun-19 22:03 sklearn/cluster/MiniBatchKMeans.class
--rw-rw-r--  2.0 unx     5086 b- defN 23-Jun-19 22:03 sklearn/cluster/KMeans.class
--rw-rw-r--  2.0 unx    12903 b- defN 23-Jun-19 22:03 sklearn/Estimator.class
--rw-rw-r--  2.0 unx     1624 b- defN 23-Jun-19 22:03 sklearn/Initializer.class
--rw-rw-r--  2.0 unx     4598 b- defN 23-Jun-19 22:03 sklearn/multiclass/OneVsRestClassifier.class
--rw-rw-r--  2.0 unx     5157 b- defN 23-Jun-19 22:03 sklearn2pmml/ruleset/RuleSetClassifier.class
--rw-rw-r--  2.0 unx     1023 b- defN 23-Jun-19 22:03 sklearn2pmml/pipeline/PMMLPipeline$3.class
--rw-rw-r--  2.0 unx    26752 b- defN 23-Jun-19 22:03 sklearn2pmml/pipeline/PMMLPipeline.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Jun-19 22:03 sklearn2pmml/pipeline/PMMLPipeline$2.class
--rw-rw-r--  2.0 unx     1421 b- defN 23-Jun-19 22:03 sklearn2pmml/pipeline/PMMLPipeline$1.class
--rw-rw-r--  2.0 unx     1811 b- defN 23-Jun-19 22:03 sklearn2pmml/pipeline/Verification.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/MultiDomain.class
--rw-rw-r--  2.0 unx     1152 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/ContinuousDomainEraser.class
--rw-rw-r--  2.0 unx     1654 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Alias.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/TemporalDomain.class
--rw-rw-r--  2.0 unx      779 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/ContinuousDomain$1.class
--rw-rw-r--  2.0 unx    11878 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Domain.class
--rw-rw-r--  2.0 unx     1416 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/MultiAlias.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DiscreteDomain.class
--rw-rw-r--  2.0 unx     1952 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/CategoricalDomain.class
--rw-rw-r--  2.0 unx     1453 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DomainEraser.class
--rw-rw-r--  2.0 unx      613 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DateTimeDomain.class
--rw-rw-r--  2.0 unx     7764 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/ContinuousDomain.class
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DiscreteDomainEraser.class
--rw-rw-r--  2.0 unx     1590 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/TransformerWrapper.class
--rw-rw-r--  2.0 unx     1045 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Domain$2.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DateDomain.class
--rw-rw-r--  2.0 unx     3544 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/DomainUtil.class
--rw-rw-r--  2.0 unx     1033 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Domain$1.class
--rw-rw-r--  2.0 unx     1577 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/OrdinalDomain.class
--rw-rw-r--  2.0 unx      672 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Domain$4.class
--rw-rw-r--  2.0 unx      799 b- defN 23-Jun-19 22:03 sklearn2pmml/decoration/Domain$3.class
--rw-rw-r--  2.0 unx     7862 b- defN 23-Jun-19 22:03 sklearn2pmml/neural_network/MLPTransformer.class
--rw-rw-r--  2.0 unx      391 b- defN 23-Jun-19 22:03 sklearn2pmml/SkLearn2PMMLFields.class
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-19 22:03 sklearn2pmml/util/Evaluatable.class
--rw-rw-r--  2.0 unx     1196 b- defN 23-Jun-19 22:03 sklearn2pmml/util/Expression.class
--rw-rw-r--  2.0 unx     1189 b- defN 23-Jun-19 22:03 sklearn2pmml/util/Predicate.class
--rw-rw-r--  2.0 unx     1434 b- defN 23-Jun-19 22:03 sklearn2pmml/util/Reshaper.class
--rw-rw-r--  2.0 unx     3392 b- defN 23-Jun-19 22:03 sklearn2pmml/util/EvaluatableUtil.class
--rw-rw-r--  2.0 unx     1658 b- defN 23-Jun-19 22:03 sklearn2pmml/util/Slicer.class
--rw-rw-r--  2.0 unx     2418 b- defN 23-Jun-19 22:03 sklearn2pmml/feature_extraction/text/Splitter.class
--rw-rw-r--  2.0 unx     3184 b- defN 23-Jun-19 22:03 sklearn2pmml/feature_extraction/text/Matcher.class
--rw-rw-r--  2.0 unx     1262 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/SelectFirstRegressor.class
--rw-rw-r--  2.0 unx     2083 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/GBDTUtil$2.class
--rw-rw-r--  2.0 unx     1934 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/GBDTLMRegressor.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/GBDTUtil$1.class
--rw-rw-r--  2.0 unx     7398 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/EstimatorChain.class
--rw-rw-r--  2.0 unx     6582 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/GBDTUtil.class
--rw-rw-r--  2.0 unx     3995 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/Link.class
--rw-rw-r--  2.0 unx     4360 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/SelectFirstUtil.class
--rw-rw-r--  2.0 unx     4252 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/GBDTLRClassifier.class
--rw-rw-r--  2.0 unx     2608 b- defN 23-Jun-19 22:03 sklearn2pmml/ensemble/SelectFirstClassifier.class
--rw-rw-r--  2.0 unx     1438 b- defN 23-Jun-19 22:03 sklearn2pmml/EstimatorProxy$1.class
--rw-rw-r--  2.0 unx      946 b- defN 23-Jun-19 22:03 sklearn2pmml/feature_selection/SelectUnique.class
--rw-rw-r--  2.0 unx     6477 b- defN 23-Jun-19 22:03 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
--rw-rw-r--  2.0 unx      791 b- defN 23-Jun-19 22:03 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
--rw-rw-r--  2.0 unx     1197 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/PatternTransformer.class
--rw-rw-r--  2.0 unx     2908 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/ReplaceTransformer.class
--rw-rw-r--  2.0 unx     1844 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/WordCountTransformer.class
--rw-rw-r--  2.0 unx      597 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/DateTimeFormatter.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
--rw-rw-r--  2.0 unx     4621 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/DurationTransformer.class
--rw-rw-r--  2.0 unx      444 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
--rw-rw-r--  2.0 unx     2777 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/FilterLookupTransformer.class
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/Formatter.class
--rw-rw-r--  2.0 unx     3424 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/CastTransformer.class
--rw-rw-r--  2.0 unx     2758 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/MatchesTransformer.class
--rw-rw-r--  2.0 unx      589 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/NumberFormatter.class
--rw-rw-r--  2.0 unx     4149 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/MultiLookupTransformer.class
--rw-rw-r--  2.0 unx     3871 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/StringNormalizer.class
--rw-rw-r--  2.0 unx     7145 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/ExpressionTransformer.class
--rw-rw-r--  2.0 unx      635 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
--rw-rw-r--  2.0 unx     3604 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/DataFrameConstructor.class
--rw-rw-r--  2.0 unx     2847 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/ConcatTransformer.class
--rw-rw-r--  2.0 unx     5993 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/CutTransformer.class
--rw-rw-r--  2.0 unx     7025 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/BSplineTransformer.class
--rw-rw-r--  2.0 unx     6410 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/LookupTransformer.class
--rw-rw-r--  2.0 unx     3236 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/SubstringTransformer.class
--rw-rw-r--  2.0 unx     3181 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
--rw-rw-r--  2.0 unx     2132 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
--rw-rw-r--  2.0 unx     3328 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/Aggregator.class
--rw-rw-r--  2.0 unx      647 b- defN 23-Jun-19 22:03 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
--rw-rw-r--  2.0 unx     1728 b- defN 23-Jun-19 22:03 sklearn2pmml/tree/CHAIDRegressor.class
--rw-rw-r--  2.0 unx    10719 b- defN 23-Jun-19 22:03 sklearn2pmml/tree/CHAIDUtil.class
--rw-rw-r--  2.0 unx     2121 b- defN 23-Jun-19 22:03 sklearn2pmml/tree/CHAIDClassifier.class
--rw-rw-r--  2.0 unx     1417 b- defN 23-Jun-19 22:03 sklearn2pmml/tree/CHAIDUtil$1.class
--rw-rw-r--  2.0 unx     3864 b- defN 23-Jun-19 22:03 sklearn2pmml/EstimatorProxy.class
--rw-rw-r--  2.0 unx     1458 b- defN 23-Jun-19 22:03 sklearn2pmml/SelectorProxy.class
--rw-rw-r--  2.0 unx     2046 b- defN 23-Jun-19 22:03 sklearn2pmml/expression/ExpressionUtil.class
--rw-rw-r--  2.0 unx     3799 b- defN 23-Jun-19 22:03 sklearn2pmml/expression/ExpressionRegressor.class
--rw-rw-r--  2.0 unx      990 b- defN 23-Jun-19 22:03 sklearn2pmml/expression/ExpressionClassifier$1.class
--rw-rw-r--  2.0 unx     8687 b- defN 23-Jun-19 22:03 sklearn2pmml/expression/ExpressionClassifier.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Jun-19 22:03 sklearn2pmml/expression/ExpressionUtil$1.class
--rw-rw-r--  2.0 unx     1774 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     2764 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
--rw-rw-r--  2.0 unx     3549 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
--rw-rw-r--  2.0 unx    13608 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/SkLearnEncoder.class
--rw-rw-r--  2.0 unx      194 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/FieldNames.class
--rw-rw-r--  2.0 unx      171 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/HasSkLearnOptions.class
--rw-rw-r--  2.0 unx     1030 b- defN 23-Jun-19 22:03 org/jpmml/sklearn/SkLearnEncoder$1.class
--rw-rw-r--  2.0 unx     1822 b- defN 23-Jun-19 22:02 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
--rw-rw-r--  2.0 unx       57 b- defN 23-Jun-19 22:03 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
-403 files, 923637 bytes uncompressed, 406937 bytes compressed:  55.9%
+Zip file size: 472037 bytes, number of entries: 405
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
+-rw-r--r--  2.0 unx      159 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn_pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 chaid/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 stop_words/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/calibration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/dummy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/svm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/impute/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/naive_bayes/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/linear_model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/linear_model/logistic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/linear_model/ridge/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/linear_model/glm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/compose/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/model_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/decomposition/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/neighbors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/multioutput/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/isotonic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/bagging/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/stacking/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/forest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/iforest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/voting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/weight_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/loss/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/discriminant_analysis/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/tree/visitors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/cluster/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/multiclass/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/ruleset/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/decoration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/util/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/postprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/expression/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 org/jpmml/sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 org/jpmml/sklearn/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn/
+-rw-rw-r--  2.0 unx    16829 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2287 b- defN 23-Jul-08 09:03 sklearn_pandas/CategoricalImputer.class
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jul-08 09:03 sklearn_pandas/TransformerPipeline.class
+-rw-rw-r--  2.0 unx     1154 b- defN 23-Jul-08 09:03 sklearn_pandas/DataFrameMapper$2.class
+-rw-rw-r--  2.0 unx     6280 b- defN 23-Jul-08 09:03 sklearn_pandas/DataFrameMapper.class
+-rw-rw-r--  2.0 unx     1126 b- defN 23-Jul-08 09:03 sklearn_pandas/DataFrameMapper$1.class
+-rw-rw-r--  2.0 unx      609 b- defN 23-Jul-08 09:03 chaid/ContinuousColumn.class
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-08 09:03 chaid/Node.class
+-rw-rw-r--  2.0 unx      467 b- defN 23-Jul-08 09:03 chaid/Column.class
+-rw-rw-r--  2.0 unx     3283 b- defN 23-Jul-08 09:03 chaid/Split.class
+-rw-rw-r--  2.0 unx      401 b- defN 23-Jul-08 09:03 chaid/InvalidSplitReason.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Jul-08 09:03 chaid/NominalColumn.class
+-rw-rw-r--  2.0 unx     1912 b- defN 23-Jul-08 09:03 stop_words/english.txt
+-rw-rw-r--  2.0 unx      147 b- defN 23-Jul-08 09:03 sklearn/HasHead.class
+-rw-rw-r--  2.0 unx     1728 b- defN 23-Jul-08 09:03 sklearn/StepUtil.class
+-rw-rw-r--  2.0 unx    12048 b- defN 23-Jul-08 09:03 sklearn/calibration/CalibratedClassifier.class
+-rw-rw-r--  2.0 unx     2953 b- defN 23-Jul-08 09:03 sklearn/calibration/SigmoidCalibration.class
+-rw-rw-r--  2.0 unx      683 b- defN 23-Jul-08 09:03 sklearn/calibration/CalibratedClassifier$1.class
+-rw-rw-r--  2.0 unx     3672 b- defN 23-Jul-08 09:03 sklearn/calibration/CalibratedClassifierCV.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Jul-08 09:03 sklearn/pipeline/PipelineTransformer.class
+-rw-rw-r--  2.0 unx     1671 b- defN 23-Jul-08 09:03 sklearn/pipeline/Pipeline$2.class
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jul-08 09:03 sklearn/pipeline/FeatureUnion.class
+-rw-rw-r--  2.0 unx     5062 b- defN 23-Jul-08 09:03 sklearn/pipeline/Pipeline.class
+-rw-rw-r--  2.0 unx     2003 b- defN 23-Jul-08 09:03 sklearn/pipeline/PipelineRegressor.class
+-rw-rw-r--  2.0 unx     1716 b- defN 23-Jul-08 09:03 sklearn/pipeline/Pipeline$1.class
+-rw-rw-r--  2.0 unx     1111 b- defN 23-Jul-08 09:03 sklearn/pipeline/PipelineUtil.class
+-rw-rw-r--  2.0 unx     2298 b- defN 23-Jul-08 09:03 sklearn/pipeline/PipelineClassifier.class
+-rw-rw-r--  2.0 unx     4913 b- defN 23-Jul-08 09:03 sklearn/dummy/DummyClassifier.class
+-rw-rw-r--  2.0 unx     2055 b- defN 23-Jul-08 09:03 sklearn/dummy/DummyRegressor.class
+-rw-rw-r--  2.0 unx      454 b- defN 23-Jul-08 09:03 sklearn/SkLearnFields.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-Jul-08 09:03 sklearn/SkLearnOutlierTransformation.class
+-rw-rw-r--  2.0 unx      240 b- defN 23-Jul-08 09:03 sklearn/HasEstimator.class
+-rw-rw-r--  2.0 unx     3421 b- defN 23-Jul-08 09:03 sklearn/OutlierDetectorUtil.class
+-rw-rw-r--  2.0 unx     1236 b- defN 23-Jul-08 09:03 sklearn/HasMultiApplyField.class
+-rw-rw-r--  2.0 unx     2393 b- defN 23-Jul-08 09:03 sklearn/svm/SupportVectorMachineUtil.class
+-rw-rw-r--  2.0 unx     1109 b- defN 23-Jul-08 09:03 sklearn/svm/LinearSVC.class
+-rw-rw-r--  2.0 unx     5037 b- defN 23-Jul-08 09:03 sklearn/svm/LibSVMClassifier.class
+-rw-rw-r--  2.0 unx      966 b- defN 23-Jul-08 09:03 sklearn/svm/SupportVectorMachineUtil$1.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jul-08 09:03 sklearn/svm/OneClassSVM.class
+-rw-rw-r--  2.0 unx     3594 b- defN 23-Jul-08 09:03 sklearn/svm/LibSVMRegressor.class
+-rw-rw-r--  2.0 unx     4114 b- defN 23-Jul-08 09:03 sklearn/InitializerUtil$1.class
+-rw-rw-r--  2.0 unx      735 b- defN 23-Jul-08 09:03 sklearn/Estimator$1.class
+-rw-rw-r--  2.0 unx      342 b- defN 23-Jul-08 09:03 sklearn/HasOutlierField.class
+-rw-rw-r--  2.0 unx      214 b- defN 23-Jul-08 09:03 sklearn/HasNumberOfFeatures.class
+-rw-rw-r--  2.0 unx      660 b- defN 23-Jul-08 09:03 sklearn/MultiTransformer.class
+-rw-rw-r--  2.0 unx     2110 b- defN 23-Jul-08 09:03 sklearn/neural_network/MLPRegressor.class
+-rw-rw-r--  2.0 unx     2555 b- defN 23-Jul-08 09:03 sklearn/neural_network/MLPClassifier.class
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jul-08 09:03 sklearn/neural_network/MultilayerPerceptronUtil$1.class
+-rw-rw-r--  2.0 unx    10661 b- defN 23-Jul-08 09:03 sklearn/neural_network/MultilayerPerceptronUtil.class
+-rw-rw-r--  2.0 unx      853 b- defN 23-Jul-08 09:03 sklearn/Step.class
+-rw-rw-r--  2.0 unx      168 b- defN 23-Jul-08 09:03 sklearn/HasDefaultValue.class
+-rw-rw-r--  2.0 unx     2936 b- defN 23-Jul-08 09:03 sklearn/impute/MissingIndicator.class
+-rw-rw-r--  2.0 unx     4027 b- defN 23-Jul-08 09:03 sklearn/impute/ImputerUtil.class
+-rw-rw-r--  2.0 unx     5703 b- defN 23-Jul-08 09:03 sklearn/impute/SimpleImputer.class
+-rw-rw-r--  2.0 unx     6948 b- defN 23-Jul-08 09:03 sklearn/naive_bayes/GaussianNB.class
+-rw-rw-r--  2.0 unx     4434 b- defN 23-Jul-08 09:03 sklearn/linear_model/LinearRegressor.class
+-rw-rw-r--  2.0 unx     5040 b- defN 23-Jul-08 09:03 sklearn/linear_model/LinearClassifier.class
+-rw-rw-r--  2.0 unx     7648 b- defN 23-Jul-08 09:03 sklearn/linear_model/logistic/LogisticRegression.class
+-rw-rw-r--  2.0 unx     1042 b- defN 23-Jul-08 09:03 sklearn/linear_model/ridge/RidgeClassifier.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jul-08 09:03 sklearn/linear_model/glm/DistributionBoundary.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Jul-08 09:03 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/Hinge.class
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
+-rw-rw-r--  2.0 unx      461 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/LossFunction.class
+-rw-rw-r--  2.0 unx      452 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/Log.class
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
+-rw-rw-r--  2.0 unx      482 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
+-rw-rw-r--  2.0 unx      932 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
+-rw-rw-r--  2.0 unx     1720 b- defN 23-Jul-08 09:03 sklearn/compose/ColumnTransformer$1.class
+-rw-rw-r--  2.0 unx     3239 b- defN 23-Jul-08 09:03 sklearn/compose/TransformedTargetRegressor.class
+-rw-rw-r--  2.0 unx     3649 b- defN 23-Jul-08 09:03 sklearn/compose/ColumnTransformer.class
+-rw-rw-r--  2.0 unx     1534 b- defN 23-Jul-08 09:03 sklearn/compose/TransformedTargetRegressor$1.class
+-rw-rw-r--  2.0 unx      894 b- defN 23-Jul-08 09:03 sklearn/IdentityTransformer.class
+-rw-rw-r--  2.0 unx     4089 b- defN 23-Jul-08 09:03 sklearn/Classifier.class
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Jul-08 09:03 sklearn/model_selection/EstimatorSearcher.class
+-rw-rw-r--  2.0 unx     1685 b- defN 23-Jul-08 09:03 sklearn/Selector.class
+-rw-rw-r--  2.0 unx      419 b- defN 23-Jul-08 09:03 sklearn/decomposition/IncrementalPCA.class
+-rw-rw-r--  2.0 unx     3471 b- defN 23-Jul-08 09:03 sklearn/decomposition/TruncatedSVD.class
+-rw-rw-r--  2.0 unx     4759 b- defN 23-Jul-08 09:03 sklearn/decomposition/PCA.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jul-08 09:03 sklearn/decomposition/BasePCA.class
+-rw-rw-r--  2.0 unx      336 b- defN 23-Jul-08 09:03 sklearn/HasPredictField.class
+-rw-rw-r--  2.0 unx     3018 b- defN 23-Jul-08 09:03 sklearn/neighbors/NearestNeighbors.class
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jul-08 09:03 sklearn/neighbors/KNeighborsClassifier.class
+-rw-rw-r--  2.0 unx     3794 b- defN 23-Jul-08 09:03 sklearn/neighbors/NearestCentroid.class
+-rw-rw-r--  2.0 unx     2025 b- defN 23-Jul-08 09:03 sklearn/neighbors/BinaryTree.class
+-rw-rw-r--  2.0 unx     1266 b- defN 23-Jul-08 09:03 sklearn/neighbors/KNeighborsUtil$1.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Jul-08 09:03 sklearn/neighbors/HasMetric.class
+-rw-rw-r--  2.0 unx    10733 b- defN 23-Jul-08 09:03 sklearn/neighbors/KNeighborsUtil.class
+-rw-rw-r--  2.0 unx     4387 b- defN 23-Jul-08 09:03 sklearn/neighbors/KNeighborsRegressor.class
+-rw-rw-r--  2.0 unx     1032 b- defN 23-Jul-08 09:03 sklearn/neighbors/DistanceMetric.class
+-rw-rw-r--  2.0 unx      351 b- defN 23-Jul-08 09:03 sklearn/neighbors/HasTrainingData.class
+-rw-rw-r--  2.0 unx      176 b- defN 23-Jul-08 09:03 sklearn/neighbors/HasNumberOfNeighbors.class
+-rw-rw-r--  2.0 unx     2654 b- defN 23-Jul-08 09:03 sklearn/multioutput/MultiOutputUtil.class
+-rw-rw-r--  2.0 unx     3510 b- defN 23-Jul-08 09:03 sklearn/multioutput/ChainUtil.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Jul-08 09:03 sklearn/multioutput/RegressorChain.class
+-rw-rw-r--  2.0 unx     1316 b- defN 23-Jul-08 09:03 sklearn/multioutput/MultiOutputClassifier.class
+-rw-rw-r--  2.0 unx     1310 b- defN 23-Jul-08 09:03 sklearn/multioutput/MultiOutputRegressor.class
+-rw-rw-r--  2.0 unx     1745 b- defN 23-Jul-08 09:03 sklearn/multioutput/ClassifierChain.class
+-rw-rw-r--  2.0 unx     4450 b- defN 23-Jul-08 09:03 sklearn/isotonic/IsotonicRegression.class
+-rw-rw-r--  2.0 unx      326 b- defN 23-Jul-08 09:03 sklearn/HasApplyField.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Jul-08 09:03 sklearn/HasEstimatorEnsemble.class
+-rw-rw-r--  2.0 unx     1929 b- defN 23-Jul-08 09:03 sklearn/Transformer$1.class
+-rw-rw-r--  2.0 unx      953 b- defN 23-Jul-08 09:03 sklearn/LabelEncoderClassifier.class
+-rw-rw-r--  2.0 unx      451 b- defN 23-Jul-08 09:03 sklearn/PassThrough.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Jul-08 09:03 sklearn/HasPriorProbability.class
+-rw-rw-r--  2.0 unx     5693 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/TfidfVectorizer.class
+-rw-rw-r--  2.0 unx      809 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/TfidfVectorizer$1.class
+-rw-rw-r--  2.0 unx      675 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/Tokenizer.class
+-rw-rw-r--  2.0 unx    13329 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/CountVectorizer.class
+-rw-rw-r--  2.0 unx     2129 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/CountVectorizer$1.class
+-rw-rw-r--  2.0 unx     1433 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/TfidfTransformer.class
+-rw-rw-r--  2.0 unx     4031 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/DictVectorizer.class
+-rw-rw-r--  2.0 unx      762 b- defN 23-Jul-08 09:03 sklearn/Clusterer.class
+-rw-rw-r--  2.0 unx     1375 b- defN 23-Jul-08 09:03 sklearn/metrics/DistanceMetric.class
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Jul-08 09:03 sklearn/ensemble/EnsembleUtil.class
+-rw-rw-r--  2.0 unx     2112 b- defN 23-Jul-08 09:03 sklearn/ensemble/bagging/BaggingRegressor.class
+-rw-rw-r--  2.0 unx     3293 b- defN 23-Jul-08 09:03 sklearn/ensemble/bagging/BaggingUtil.class
+-rw-rw-r--  2.0 unx     3031 b- defN 23-Jul-08 09:03 sklearn/ensemble/bagging/BaggingClassifier.class
+-rw-rw-r--  2.0 unx     1409 b- defN 23-Jul-08 09:03 sklearn/ensemble/EnsembleRegressor.class
+-rw-rw-r--  2.0 unx     3485 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingClassifier.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
+-rw-rw-r--  2.0 unx     3109 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingRegressor.class
+-rw-rw-r--  2.0 unx     3862 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingUtil.class
+-rw-rw-r--  2.0 unx     2524 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingClassifier$1.class
+-rw-rw-r--  2.0 unx     2254 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingRegressor$1.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
+-rw-rw-r--  2.0 unx     2563 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx      858 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/LossFunction.class
+-rw-rw-r--  2.0 unx     1588 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
+-rw-rw-r--  2.0 unx     1317 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
+-rw-rw-r--  2.0 unx     7948 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
+-rw-rw-r--  2.0 unx      960 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/MeanEstimator.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
+-rw-rw-r--  2.0 unx     1578 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
+-rw-rw-r--  2.0 unx      811 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
+-rw-rw-r--  2.0 unx     3003 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
+-rw-rw-r--  2.0 unx     1148 b- defN 23-Jul-08 09:03 sklearn/ensemble/EnsembleUtil$1.class
+-rw-rw-r--  2.0 unx     3059 b- defN 23-Jul-08 09:03 sklearn/ensemble/forest/ForestUtil.class
+-rw-rw-r--  2.0 unx     2528 b- defN 23-Jul-08 09:03 sklearn/ensemble/forest/ForestRegressor.class
+-rw-rw-r--  2.0 unx     2987 b- defN 23-Jul-08 09:03 sklearn/ensemble/forest/ForestClassifier.class
+-rw-rw-r--  2.0 unx     1752 b- defN 23-Jul-08 09:03 sklearn/ensemble/iforest/IsolationForest$3.class
+-rw-rw-r--  2.0 unx     2206 b- defN 23-Jul-08 09:03 sklearn/ensemble/iforest/IsolationForest$1.class
+-rw-rw-r--  2.0 unx     1716 b- defN 23-Jul-08 09:03 sklearn/ensemble/iforest/IsolationForest$2.class
+-rw-rw-r--  2.0 unx     8225 b- defN 23-Jul-08 09:03 sklearn/ensemble/iforest/IsolationForest.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Jul-08 09:03 sklearn/ensemble/voting/VotingClassifier.class
+-rw-rw-r--  2.0 unx     3716 b- defN 23-Jul-08 09:03 sklearn/ensemble/voting/VotingRegressor.class
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx     1247 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
+-rw-rw-r--  2.0 unx     3041 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
+-rw-rw-r--  2.0 unx     6152 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
+-rw-rw-r--  2.0 unx      490 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
+-rw-rw-r--  2.0 unx     1572 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
+-rw-rw-r--  2.0 unx     6377 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     8868 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-08 09:03 sklearn/ensemble/EnsembleClassifier.class
+-rw-rw-r--  2.0 unx     3564 b- defN 23-Jul-08 09:03 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
+-rw-rw-r--  2.0 unx     6043 b- defN 23-Jul-08 09:03 sklearn/Transformer.class
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jul-08 09:03 sklearn/Transformer$1$1.class
+-rw-rw-r--  2.0 unx      981 b- defN 23-Jul-08 09:03 sklearn/Drop.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jul-08 09:03 sklearn/feature_selection/SelectKBest$Entry.class
+-rw-rw-r--  2.0 unx     3486 b- defN 23-Jul-08 09:03 sklearn/feature_selection/SelectFromModel.class
+-rw-rw-r--  2.0 unx     2922 b- defN 23-Jul-08 09:03 sklearn/feature_selection/SelectKBest.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Jul-08 09:03 sklearn/feature_selection/PySelector.class
+-rw-rw-r--  2.0 unx      607 b- defN 23-Jul-08 09:03 sklearn/Transformer$2.class
+-rw-rw-r--  2.0 unx     2216 b- defN 23-Jul-08 09:03 sklearn/SkLearnUtil.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-Jul-08 09:03 sklearn/loss/HalfMultinomialLoss.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Jul-08 09:03 sklearn/loss/CyLossFunction.class
+-rw-rw-r--  2.0 unx      403 b- defN 23-Jul-08 09:03 sklearn/loss/HalfBinomialLoss.class
+-rw-rw-r--  2.0 unx      387 b- defN 23-Jul-08 09:03 sklearn/loss/BaseLoss.class
+-rw-rw-r--  2.0 unx      381 b- defN 23-Jul-08 09:03 sklearn/HasDecisionFunctionField.class
+-rw-rw-r--  2.0 unx      338 b- defN 23-Jul-08 09:03 sklearn/SkLearnMethods.class
+-rw-rw-r--  2.0 unx     5114 b- defN 23-Jul-08 09:03 sklearn/ScalarLabelUtil.class
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Jul-08 09:03 sklearn/OutlierDetectorUtil$1.class
+-rw-rw-r--  2.0 unx      195 b- defN 23-Jul-08 09:03 sklearn/HasClasses.class
+-rw-rw-r--  2.0 unx     4685 b- defN 23-Jul-08 09:03 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
+-rw-rw-r--  2.0 unx      696 b- defN 23-Jul-08 09:03 sklearn/EstimatorUtil$1.class
+-rw-rw-r--  2.0 unx     3311 b- defN 23-Jul-08 09:03 sklearn/Composite.class
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Jul-08 09:03 sklearn/preprocessing/KBinsDiscretizer$1.class
+-rw-rw-r--  2.0 unx     4567 b- defN 23-Jul-08 09:03 sklearn/preprocessing/PowerTransformer.class
+-rw-rw-r--  2.0 unx     2381 b- defN 23-Jul-08 09:03 sklearn/preprocessing/LabelEncoder.class
+-rw-rw-r--  2.0 unx     4924 b- defN 23-Jul-08 09:03 sklearn/preprocessing/LabelBinarizer.class
+-rw-rw-r--  2.0 unx      729 b- defN 23-Jul-08 09:03 sklearn/preprocessing/EncoderUtil$3.class
+-rw-rw-r--  2.0 unx      389 b- defN 23-Jul-08 09:03 sklearn/preprocessing/Scaler.class
+-rw-rw-r--  2.0 unx     3242 b- defN 23-Jul-08 09:03 sklearn/preprocessing/MaxAbsScaler.class
+-rw-rw-r--  2.0 unx     2948 b- defN 23-Jul-08 09:03 sklearn/preprocessing/FunctionTransformer.class
+-rw-rw-r--  2.0 unx     3291 b- defN 23-Jul-08 09:03 sklearn/preprocessing/BaseEncoder.class
+-rw-rw-r--  2.0 unx     1270 b- defN 23-Jul-08 09:03 sklearn/preprocessing/EncoderUtil$1.class
+-rw-rw-r--  2.0 unx     4549 b- defN 23-Jul-08 09:03 sklearn/preprocessing/StandardScaler.class
+-rw-rw-r--  2.0 unx     6971 b- defN 23-Jul-08 09:03 sklearn/preprocessing/EncoderUtil.class
+-rw-rw-r--  2.0 unx     6343 b- defN 23-Jul-08 09:03 sklearn/preprocessing/PolynomialFeatures.class
+-rw-rw-r--  2.0 unx     8486 b- defN 23-Jul-08 09:03 sklearn/preprocessing/KBinsDiscretizer.class
+-rw-rw-r--  2.0 unx     4671 b- defN 23-Jul-08 09:03 sklearn/preprocessing/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     2553 b- defN 23-Jul-08 09:03 sklearn/preprocessing/Binarizer.class
+-rw-rw-r--  2.0 unx     1054 b- defN 23-Jul-08 09:03 sklearn/preprocessing/EncoderUtil$2.class
+-rw-rw-r--  2.0 unx     3595 b- defN 23-Jul-08 09:03 sklearn/preprocessing/MinMaxScaler.class
+-rw-rw-r--  2.0 unx     4467 b- defN 23-Jul-08 09:03 sklearn/preprocessing/RobustScaler.class
+-rw-rw-r--  2.0 unx     3740 b- defN 23-Jul-08 09:03 sklearn/preprocessing/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      957 b- defN 23-Jul-08 09:03 sklearn/preprocessing/Imputer.class
+-rw-rw-r--  2.0 unx     2033 b- defN 23-Jul-08 09:03 sklearn/preprocessing/PolynomialFeatures$1.class
+-rw-rw-r--  2.0 unx     7408 b- defN 23-Jul-08 09:03 sklearn/preprocessing/MultiOneHotEncoder.class
+-rw-rw-r--  2.0 unx     2153 b- defN 23-Jul-08 09:03 sklearn/tree/TreeClassifier.class
+-rw-rw-r--  2.0 unx     3111 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$1.class
+-rw-rw-r--  2.0 unx     2664 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$4.class
+-rw-rw-r--  2.0 unx     4805 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelFlattener.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelCompactor$1.class
+-rw-rw-r--  2.0 unx     5431 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelCompactor.class
+-rw-rw-r--  2.0 unx     2988 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelPruner.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelFlattener$1.class
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelPruner$1.class
+-rw-rw-r--  2.0 unx      879 b- defN 23-Jul-08 09:03 sklearn/tree/RegressionCriterion.class
+-rw-rw-r--  2.0 unx     1151 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$5.class
+-rw-rw-r--  2.0 unx      978 b- defN 23-Jul-08 09:03 sklearn/tree/PresortBestSplitter.class
+-rw-rw-r--  2.0 unx     1589 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$6.class
+-rw-rw-r--  2.0 unx     1764 b- defN 23-Jul-08 09:03 sklearn/tree/TreeRegressor.class
+-rw-rw-r--  2.0 unx     1489 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$7.class
+-rw-rw-r--  2.0 unx    19425 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$3.class
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jul-08 09:03 sklearn/tree/HasTreeOptions.class
+-rw-rw-r--  2.0 unx     2257 b- defN 23-Jul-08 09:03 sklearn/tree/Tree.class
+-rw-rw-r--  2.0 unx      754 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$2.class
+-rw-rw-r--  2.0 unx      150 b- defN 23-Jul-08 09:03 sklearn/tree/HasTree.class
+-rw-rw-r--  2.0 unx     1967 b- defN 23-Jul-08 09:03 sklearn/InitializerUtil.class
+-rw-rw-r--  2.0 unx      570 b- defN 23-Jul-08 09:03 sklearn/Regressor.class
+-rw-rw-r--  2.0 unx      211 b- defN 23-Jul-08 09:03 sklearn/HasNumberOfOutputs.class
+-rw-rw-r--  2.0 unx      534 b- defN 23-Jul-08 09:03 sklearn/OutlierDetector.class
+-rw-rw-r--  2.0 unx     2808 b- defN 23-Jul-08 09:03 sklearn/Calibrator.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Jul-08 09:03 sklearn/HasClassifierOptions.class
+-rw-rw-r--  2.0 unx     7080 b- defN 23-Jul-08 09:03 sklearn/EstimatorUtil.class
+-rw-rw-r--  2.0 unx      199 b- defN 23-Jul-08 09:03 sklearn/HasType.class
+-rw-rw-r--  2.0 unx      678 b- defN 23-Jul-08 09:03 sklearn/cluster/MiniBatchKMeans.class
+-rw-rw-r--  2.0 unx     5086 b- defN 23-Jul-08 09:03 sklearn/cluster/KMeans.class
+-rw-rw-r--  2.0 unx    14030 b- defN 23-Jul-08 09:03 sklearn/Estimator.class
+-rw-rw-r--  2.0 unx     1624 b- defN 23-Jul-08 09:03 sklearn/Initializer.class
+-rw-rw-r--  2.0 unx     4598 b- defN 23-Jul-08 09:03 sklearn/multiclass/OneVsRestClassifier.class
+-rw-rw-r--  2.0 unx     5157 b- defN 23-Jul-08 09:03 sklearn2pmml/ruleset/RuleSetClassifier.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/PMMLPipeline$3.class
+-rw-rw-r--  2.0 unx     1023 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/PMMLPipeline$4.class
+-rw-rw-r--  2.0 unx    27116 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/PMMLPipeline.class
+-rw-rw-r--  2.0 unx     1421 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/PMMLPipeline$2.class
+-rw-rw-r--  2.0 unx     1346 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/PMMLPipeline$1.class
+-rw-rw-r--  2.0 unx     1811 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/Verification.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/MultiDomain.class
+-rw-rw-r--  2.0 unx     1152 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/ContinuousDomainEraser.class
+-rw-rw-r--  2.0 unx     1654 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Alias.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/TemporalDomain.class
+-rw-rw-r--  2.0 unx      779 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/ContinuousDomain$1.class
+-rw-rw-r--  2.0 unx    11878 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Domain.class
+-rw-rw-r--  2.0 unx     1416 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/MultiAlias.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DiscreteDomain.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/CategoricalDomain.class
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DomainEraser.class
+-rw-rw-r--  2.0 unx      613 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DateTimeDomain.class
+-rw-rw-r--  2.0 unx     7764 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/ContinuousDomain.class
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DiscreteDomainEraser.class
+-rw-rw-r--  2.0 unx     1590 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     1045 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Domain$2.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DateDomain.class
+-rw-rw-r--  2.0 unx     3544 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DomainUtil.class
+-rw-rw-r--  2.0 unx     1033 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Domain$1.class
+-rw-rw-r--  2.0 unx     1577 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/OrdinalDomain.class
+-rw-rw-r--  2.0 unx      672 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Domain$4.class
+-rw-rw-r--  2.0 unx      799 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Domain$3.class
+-rw-rw-r--  2.0 unx     7862 b- defN 23-Jul-08 09:03 sklearn2pmml/neural_network/MLPTransformer.class
+-rw-rw-r--  2.0 unx      391 b- defN 23-Jul-08 09:03 sklearn2pmml/SkLearn2PMMLFields.class
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jul-08 09:03 sklearn2pmml/util/Evaluatable.class
+-rw-rw-r--  2.0 unx     1196 b- defN 23-Jul-08 09:03 sklearn2pmml/util/Expression.class
+-rw-rw-r--  2.0 unx     1189 b- defN 23-Jul-08 09:03 sklearn2pmml/util/Predicate.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jul-08 09:03 sklearn2pmml/util/Reshaper.class
+-rw-rw-r--  2.0 unx     3392 b- defN 23-Jul-08 09:03 sklearn2pmml/util/EvaluatableUtil.class
+-rw-rw-r--  2.0 unx     1658 b- defN 23-Jul-08 09:03 sklearn2pmml/util/Slicer.class
+-rw-rw-r--  2.0 unx     2418 b- defN 23-Jul-08 09:03 sklearn2pmml/feature_extraction/text/Splitter.class
+-rw-rw-r--  2.0 unx     3184 b- defN 23-Jul-08 09:03 sklearn2pmml/feature_extraction/text/Matcher.class
+-rw-rw-r--  2.0 unx     1262 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/SelectFirstRegressor.class
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/GBDTUtil$2.class
+-rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/GBDTLMRegressor.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/GBDTUtil$1.class
+-rw-rw-r--  2.0 unx     7398 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/EstimatorChain.class
+-rw-rw-r--  2.0 unx     6582 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/GBDTUtil.class
+-rw-rw-r--  2.0 unx     3995 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/Link.class
+-rw-rw-r--  2.0 unx     4360 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/SelectFirstUtil.class
+-rw-rw-r--  2.0 unx     4252 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/GBDTLRClassifier.class
+-rw-rw-r--  2.0 unx     2608 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/SelectFirstClassifier.class
+-rw-rw-r--  2.0 unx     1438 b- defN 23-Jul-08 09:03 sklearn2pmml/EstimatorProxy$1.class
+-rw-rw-r--  2.0 unx      946 b- defN 23-Jul-08 09:03 sklearn2pmml/feature_selection/SelectUnique.class
+-rw-rw-r--  2.0 unx     6477 b- defN 23-Jul-08 09:03 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
+-rw-rw-r--  2.0 unx      791 b- defN 23-Jul-08 09:03 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
+-rw-rw-r--  2.0 unx     1197 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/PatternTransformer.class
+-rw-rw-r--  2.0 unx     2908 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/ReplaceTransformer.class
+-rw-rw-r--  2.0 unx     1844 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/WordCountTransformer.class
+-rw-rw-r--  2.0 unx      597 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/DateTimeFormatter.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
+-rw-rw-r--  2.0 unx     4621 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/DurationTransformer.class
+-rw-rw-r--  2.0 unx      444 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
+-rw-rw-r--  2.0 unx     2777 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/FilterLookupTransformer.class
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/Formatter.class
+-rw-rw-r--  2.0 unx     3424 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/CastTransformer.class
+-rw-rw-r--  2.0 unx     2758 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/MatchesTransformer.class
+-rw-rw-r--  2.0 unx      589 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/NumberFormatter.class
+-rw-rw-r--  2.0 unx     4149 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/MultiLookupTransformer.class
+-rw-rw-r--  2.0 unx     3871 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/StringNormalizer.class
+-rw-rw-r--  2.0 unx     7145 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/ExpressionTransformer.class
+-rw-rw-r--  2.0 unx      635 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     3604 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/DataFrameConstructor.class
+-rw-rw-r--  2.0 unx     2847 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/ConcatTransformer.class
+-rw-rw-r--  2.0 unx     5993 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/CutTransformer.class
+-rw-rw-r--  2.0 unx     7025 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/BSplineTransformer.class
+-rw-rw-r--  2.0 unx     6410 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/LookupTransformer.class
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/SubstringTransformer.class
+-rw-rw-r--  2.0 unx     3181 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
+-rw-rw-r--  2.0 unx     2132 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
+-rw-rw-r--  2.0 unx     3328 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/Aggregator.class
+-rw-rw-r--  2.0 unx      647 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     1639 b- defN 23-Jul-08 09:03 sklearn2pmml/tree/CHAIDRegressor.class
+-rw-rw-r--  2.0 unx    10719 b- defN 23-Jul-08 09:03 sklearn2pmml/tree/CHAIDUtil.class
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-08 09:03 sklearn2pmml/tree/CHAIDClassifier.class
+-rw-rw-r--  2.0 unx     1417 b- defN 23-Jul-08 09:03 sklearn2pmml/tree/CHAIDUtil$1.class
+-rw-rw-r--  2.0 unx     3864 b- defN 23-Jul-08 09:03 sklearn2pmml/EstimatorProxy.class
+-rw-rw-r--  2.0 unx     1458 b- defN 23-Jul-08 09:03 sklearn2pmml/SelectorProxy.class
+-rw-rw-r--  2.0 unx     2046 b- defN 23-Jul-08 09:03 sklearn2pmml/expression/ExpressionUtil.class
+-rw-rw-r--  2.0 unx     3799 b- defN 23-Jul-08 09:03 sklearn2pmml/expression/ExpressionRegressor.class
+-rw-rw-r--  2.0 unx      990 b- defN 23-Jul-08 09:03 sklearn2pmml/expression/ExpressionClassifier$1.class
+-rw-rw-r--  2.0 unx     8687 b- defN 23-Jul-08 09:03 sklearn2pmml/expression/ExpressionClassifier.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jul-08 09:03 sklearn2pmml/expression/ExpressionUtil$1.class
+-rw-rw-r--  2.0 unx     1774 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     2764 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
+-rw-rw-r--  2.0 unx     3549 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
+-rw-rw-r--  2.0 unx    14546 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/SkLearnEncoder.class
+-rw-rw-r--  2.0 unx     1437 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/SkLearnEncoder$3.class
+-rw-rw-r--  2.0 unx     1344 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/SkLearnEncoder$2.class
+-rw-rw-r--  2.0 unx      194 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/FieldNames.class
+-rw-rw-r--  2.0 unx      171 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/HasSkLearnOptions.class
+-rw-rw-r--  2.0 unx     4094 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/SkLearnEncoder$1.class
+-rw-rw-r--  2.0 unx     1822 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
+-rw-rw-r--  2.0 unx       57 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
+405 files, 930740 bytes uncompressed, 409879 bytes compressed:  56.0%
```

#### zipnote «TEMP»/diffoscope_ztes36tb_/tmphnyy_ok1_.zip

```diff
@@ -291,17 +291,14 @@
 
 Filename: sklearn/OutlierDetectorUtil.class
 Comment: 
 
 Filename: sklearn/HasMultiApplyField.class
 Comment: 
 
-Filename: sklearn/None.class
-Comment: 
-
 Filename: sklearn/svm/SupportVectorMachineUtil.class
 Comment: 
 
 Filename: sklearn/svm/LinearSVC.class
 Comment: 
 
 Filename: sklearn/svm/LibSVMClassifier.class
@@ -408,14 +405,17 @@
 
 Filename: sklearn/compose/ColumnTransformer.class
 Comment: 
 
 Filename: sklearn/compose/TransformedTargetRegressor$1.class
 Comment: 
 
+Filename: sklearn/IdentityTransformer.class
+Comment: 
+
 Filename: sklearn/Classifier.class
 Comment: 
 
 Filename: sklearn/model_selection/EstimatorSearcher.class
 Comment: 
 
 Filename: sklearn/Selector.class
@@ -834,17 +834,14 @@
 
 Filename: sklearn/tree/visitors/TreeModelFlattener$1.class
 Comment: 
 
 Filename: sklearn/tree/visitors/TreeModelPruner$1.class
 Comment: 
 
-Filename: sklearn/tree/TreeUtil$8.class
-Comment: 
-
 Filename: sklearn/tree/RegressionCriterion.class
 Comment: 
 
 Filename: sklearn/tree/TreeUtil$5.class
 Comment: 
 
 Filename: sklearn/tree/PresortBestSplitter.class
@@ -918,14 +915,17 @@
 
 Filename: sklearn2pmml/ruleset/RuleSetClassifier.class
 Comment: 
 
 Filename: sklearn2pmml/pipeline/PMMLPipeline$3.class
 Comment: 
 
+Filename: sklearn2pmml/pipeline/PMMLPipeline$4.class
+Comment: 
+
 Filename: sklearn2pmml/pipeline/PMMLPipeline.class
 Comment: 
 
 Filename: sklearn2pmml/pipeline/PMMLPipeline$2.class
 Comment: 
 
 Filename: sklearn2pmml/pipeline/PMMLPipeline$1.class
@@ -1188,14 +1188,20 @@
 
 Filename: org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
 Comment: 
 
 Filename: org/jpmml/sklearn/SkLearnEncoder.class
 Comment: 
 
+Filename: org/jpmml/sklearn/SkLearnEncoder$3.class
+Comment: 
+
+Filename: org/jpmml/sklearn/SkLearnEncoder$2.class
+Comment: 
+
 Filename: org/jpmml/sklearn/FieldNames.class
 Comment: 
 
 Filename: org/jpmml/sklearn/HasSkLearnOptions.class
 Comment: 
 
 Filename: org/jpmml/sklearn/SkLearnEncoder$1.class
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-SkLearn library
-Implementation-Version: 1.7.30
+Implementation-Version: 1.7.31
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### sklearn/calibration/CalibratedClassifier.class

##### procyon -ec {}

```diff
@@ -188,22 +188,22 @@
     }
     
     public String getMethod() {
         return this.getString("method");
     }
     
     private String getDecisionFunctionField(Object value) {
-        final Object segmentId = this.getPMMLSegmentId();
+        final Object pmmlSegmentId = this.getPMMLSegmentId();
         if (value instanceof String) {
             final String name = (String)value;
             value = extractArguments("decisionFunction", name);
         }
         List<?> args;
-        if (segmentId != null) {
-            args = Arrays.asList(segmentId, value);
+        if (pmmlSegmentId != null) {
+            args = Arrays.asList(pmmlSegmentId, value);
         }
         else {
             args = Arrays.asList(value);
         }
         return FieldNameUtil.create("decisionFunction", (List)args);
     }
```

#### sklearn/pipeline/Pipeline$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum fe56c342c79d1dc5cd3a2a1e043234f5d5fa4e78b58985ed4040f81d87d9b7a2
+  SHA-256 checksum 56f9a79bda77f8bf022d7c361606ba0a1bd7339bd97071ca77a6e1ac4fb56516
   Compiled from "Pipeline.java"
 class sklearn.pipeline.Pipeline$2 extends org.jpmml.python.CastFunction<E>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #15                         // sklearn/pipeline/Pipeline$2
   super_class: #16                        // org/jpmml/python/CastFunction
@@ -100,15 +100,15 @@
          1: aload_1
          2: putfield      #1                  // Field this$0:Lsklearn/pipeline/Pipeline;
          5: aload_0
          6: aload_2
          7: invokespecial #2                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
         10: return
       LineNumberTable:
-        line 137: 0
+        line 132: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn/pipeline/Pipeline$2;
             0      11     1 this$0   Lsklearn/pipeline/Pipeline;
             0      11     2    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -127,17 +127,17 @@
         10: areturn
         11: aload_0
         12: aload_1
         13: invokespecial #5                  // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
         16: checkcast     #6                  // class sklearn/Estimator
         19: areturn
       LineNumberTable:
-        line 142: 0
-        line 143: 9
-        line 146: 11
+        line 137: 0
+        line 138: 9
+        line 141: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lsklearn/pipeline/Pipeline$2;
             0      20     1 object   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 11 /* same */
     Signature: #37                          // (Ljava/lang/Object;)TE;
@@ -156,15 +156,15 @@
         13: invokestatic  #11                 // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
         16: invokevirtual #10                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         19: ldc           #12                 // String ) is not a supported Estimator
         21: invokevirtual #10                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         24: invokevirtual #13                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         27: areturn
       LineNumberTable:
-        line 151: 0
+        line 146: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      28     0  this   Lsklearn/pipeline/Pipeline$2;
             0      28     1 object   Ljava/lang/Object;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
@@ -172,15 +172,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #14                 // Method apply:(Ljava/lang/Object;)Lsklearn/Estimator;
          5: areturn
       LineNumberTable:
-        line 137: 0
+        line 132: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/pipeline/Pipeline$2;
 }
 Signature: #41                          // Lorg/jpmml/python/CastFunction<TE;>;
 SourceFile: "Pipeline.java"
 EnclosingMethod: #45.#46                // sklearn.pipeline.Pipeline.getFinalEstimator
```

#### sklearn/pipeline/Pipeline.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum f5ade33c9705dea377880568e355be931193c5a12ed14f865735c76db631d956
+  SHA-256 checksum 296c7243a5baa858c8e6cdfb70720e8c07b7a4afea4b3123e237585db8c91b7e
   Compiled from "Pipeline.java"
 public class sklearn.pipeline.Pipeline extends sklearn.Composite implements org.jpmml.python.Castable,sklearn.HasHead
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #50                         // sklearn/pipeline/Pipeline
   super_class: #51                        // sklearn/Composite
@@ -221,16 +221,16 @@
       stack=3, locals=1, args_size=1
          0: aload_0
          1: ldc           #1                  // String sklearn.pipeline
          3: ldc           #2                  // String Pipeline
          5: invokespecial #3                  // Method "<init>":(Ljava/lang/String;Ljava/lang/String;)V
          8: return
       LineNumberTable:
-        line 41: 0
-        line 42: 8
+        line 40: 0
+        line 41: 8
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/pipeline/Pipeline;
 
   public sklearn.pipeline.Pipeline(java.lang.String, java.lang.String);
     descriptor: (Ljava/lang/String;Ljava/lang/String;)V
     flags: (0x0001) ACC_PUBLIC
@@ -238,16 +238,16 @@
       stack=3, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: aload_2
          3: invokespecial #4                  // Method sklearn/Composite."<init>":(Ljava/lang/String;Ljava/lang/String;)V
          6: return
       LineNumberTable:
-        line 45: 0
-        line 46: 6
+        line 44: 0
+        line 45: 6
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lsklearn/pipeline/Pipeline;
             0       7     1 module   Ljava/lang/String;
             0       7     2  name   Ljava/lang/String;
 
   public boolean hasTransformers();
@@ -273,20 +273,20 @@
         33: iconst_1
         34: goto          38
         37: iconst_0
         38: ireturn
         39: iconst_1
         40: ireturn
       LineNumberTable:
-        line 50: 0
-        line 52: 5
-        line 53: 14
-        line 56: 16
-        line 57: 26
-        line 61: 39
+        line 49: 0
+        line 51: 5
+        line 52: 14
+        line 55: 16
+        line 56: 26
+        line 60: 39
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      41     0  this   Lsklearn/pipeline/Pipeline;
             5      36     1 steps   Ljava/util/List;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             5      36     1 steps   Ljava/util/List<[Ljava/lang/Object;>;
@@ -335,23 +335,23 @@
         54: invokestatic  #15                 // Method org/jpmml/python/CastUtil.deepCastTo:(Ljava/lang/Object;Ljava/lang/Class;)Ljava/lang/Object;
         57: astore_3
         58: ldc           #14                 // class sklearn/Estimator
         60: aload_3
         61: invokevirtual #16                 // Method java/lang/Class.isInstance:(Ljava/lang/Object;)Z
         64: ireturn
       LineNumberTable:
-        line 67: 0
-        line 69: 5
-        line 70: 14
-        line 73: 16
-        line 75: 34
-        line 77: 40
-        line 78: 49
-        line 81: 51
-        line 83: 58
+        line 66: 0
+        line 68: 5
+        line 69: 14
+        line 72: 16
+        line 74: 34
+        line 76: 40
+        line 77: 49
+        line 80: 51
+        line 82: 58
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      65     0  this   Lsklearn/pipeline/Pipeline;
             5      60     1 steps   Ljava/util/List;
            34      31     2 finalStep   [Ljava/lang/Object;
            40      25     3 estimator   Ljava/lang/Object;
       LocalVariableTypeTable:
@@ -395,20 +395,20 @@
         41: invokespecial #21                 // Method sklearn/pipeline/Pipeline$1."<init>":(Lsklearn/pipeline/Pipeline;Ljava/lang/Class;)V
         44: astore_3
         45: aload_2
         46: aload_3
         47: invokestatic  #22                 // Method com/google/common/collect/Lists.transform:(Ljava/util/List;Lcom/google/common/base/Function;)Ljava/util/List;
         50: areturn
       LineNumberTable:
-        line 88: 0
-        line 90: 5
-        line 91: 12
-        line 94: 28
-        line 96: 34
-        line 118: 45
+        line 87: 0
+        line 89: 5
+        line 90: 12
+        line 93: 28
+        line 95: 34
+        line 113: 45
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      51     0  this   Lsklearn/pipeline/Pipeline;
             5      46     1 steps   Ljava/util/List;
            34      17     2 transformers   Ljava/util/List;
            45       6     3 castFunction   Lorg/jpmml/python/CastFunction;
       LocalVariableTypeTable:
@@ -428,15 +428,15 @@
     Code:
       stack=2, locals=1, args_size=1
          0: aload_0
          1: ldc           #14                 // class sklearn/Estimator
          3: invokevirtual #23                 // Method getFinalEstimator:(Ljava/lang/Class;)Lsklearn/Estimator;
          6: areturn
       LineNumberTable:
-        line 123: 0
+        line 118: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lsklearn/pipeline/Pipeline;
 
   public <E extends sklearn.Estimator> E getFinalEstimator(java.lang.Class<? extends E>);
     descriptor: (Ljava/lang/Class;)Lsklearn/Estimator;
     flags: (0x0001) ACC_PUBLIC
@@ -473,21 +473,21 @@
         58: astore        5
         60: aload         5
         62: aload         4
         64: invokevirtual #29                 // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
         67: checkcast     #14                 // class sklearn/Estimator
         70: areturn
       LineNumberTable:
-        line 127: 0
-        line 129: 5
-        line 130: 14
-        line 133: 24
-        line 135: 42
-        line 137: 49
-        line 155: 60
+        line 122: 0
+        line 124: 5
+        line 125: 14
+        line 128: 24
+        line 130: 42
+        line 132: 49
+        line 150: 60
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      71     0  this   Lsklearn/pipeline/Pipeline;
             0      71     1 clazz   Ljava/lang/Class;
             5      66     2 steps   Ljava/util/List;
            42      29     3 finalStep   [Ljava/lang/Object;
            49      22     4 estimator   Ljava/lang/Object;
@@ -535,23 +535,23 @@
         48: ifeq          56
         51: aload_0
         52: invokevirtual #36                 // Method toRegressor:()Lsklearn/Regressor;
         55: areturn
         56: aload_0
         57: areturn
       LineNumberTable:
-        line 161: 0
-        line 162: 9
-        line 165: 14
-        line 166: 23
-        line 169: 28
-        line 170: 37
-        line 173: 42
-        line 174: 51
-        line 177: 56
+        line 156: 0
+        line 157: 9
+        line 160: 14
+        line 161: 23
+        line 164: 28
+        line 165: 37
+        line 168: 42
+        line 169: 51
+        line 172: 56
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      58     0  this   Lsklearn/pipeline/Pipeline;
             0      58     1 clazz   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      58     1 clazz   Ljava/lang/Class<*>;
@@ -579,19 +579,19 @@
         15: invokevirtual #38                 // Method getFinalEstimator:()Lsklearn/Estimator;
         18: astore_2
         19: aload_1
         20: aload_2
         21: invokestatic  #39                 // Method sklearn/pipeline/PipelineUtil.getHead:(Ljava/util/List;Lsklearn/Estimator;)Lsklearn/Transformer;
         24: areturn
       LineNumberTable:
-        line 182: 0
-        line 183: 5
-        line 185: 7
-        line 186: 14
-        line 189: 19
+        line 177: 0
+        line 178: 5
+        line 180: 7
+        line 181: 14
+        line 184: 19
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      25     0  this   Lsklearn/pipeline/Pipeline;
             5      20     1 transformers   Ljava/util/List;
             7      18     2 estimator   Lsklearn/Estimator;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -621,19 +621,19 @@
         25: athrow
         26: new           #41                 // class sklearn/pipeline/PipelineTransformer
         29: dup
         30: aload_0
         31: invokespecial #42                 // Method sklearn/pipeline/PipelineTransformer."<init>":(Lsklearn/pipeline/Pipeline;)V
         34: areturn
       LineNumberTable:
-        line 194: 0
-        line 195: 7
-        line 197: 12
-        line 198: 16
-        line 202: 26
+        line 189: 0
+        line 190: 7
+        line 192: 12
+        line 193: 16
+        line 197: 26
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            12      14     1 estimator   Lsklearn/Estimator;
             0      35     0  this   Lsklearn/pipeline/Pipeline;
       StackMapTable: number_of_entries = 1
         frame_type = 26 /* same */
 
@@ -658,20 +658,20 @@
         25: invokevirtual #36                 // Method toRegressor:()Lsklearn/Regressor;
         28: areturn
         29: new           #24                 // class java/lang/IllegalArgumentException
         32: dup
         33: invokespecial #43                 // Method java/lang/IllegalArgumentException."<init>":()V
         36: athrow
       LineNumberTable:
-        line 206: 0
-        line 208: 5
-        line 209: 12
-        line 212: 17
-        line 213: 24
-        line 216: 29
+        line 201: 0
+        line 203: 5
+        line 204: 12
+        line 207: 17
+        line 208: 24
+        line 211: 29
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      37     0  this   Lsklearn/pipeline/Pipeline;
             5      32     1 estimator   Lsklearn/Estimator;
       StackMapTable: number_of_entries = 2
         frame_type = 252 /* append */
           offset_delta = 17
@@ -685,15 +685,15 @@
       stack=3, locals=1, args_size=1
          0: new           #44                 // class sklearn/pipeline/PipelineClassifier
          3: dup
          4: aload_0
          5: invokespecial #45                 // Method sklearn/pipeline/PipelineClassifier."<init>":(Lsklearn/pipeline/Pipeline;)V
          8: areturn
       LineNumberTable:
-        line 220: 0
+        line 215: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/pipeline/Pipeline;
 
   public sklearn.Regressor toRegressor();
     descriptor: ()Lsklearn/Regressor;
     flags: (0x0001) ACC_PUBLIC
@@ -701,30 +701,30 @@
       stack=3, locals=1, args_size=1
          0: new           #46                 // class sklearn/pipeline/PipelineRegressor
          3: dup
          4: aload_0
          5: invokespecial #47                 // Method sklearn/pipeline/PipelineRegressor."<init>":(Lsklearn/pipeline/Pipeline;)V
          8: areturn
       LineNumberTable:
-        line 224: 0
+        line 219: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/pipeline/Pipeline;
 
   public java.util.List<java.lang.Object[]> getSteps();
     descriptor: ()Ljava/util/List;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=1, args_size=1
          0: aload_0
          1: ldc           #48                 // String steps
          3: invokevirtual #49                 // Method getTupleList:(Ljava/lang/String;)Ljava/util/List;
          6: areturn
       LineNumberTable:
-        line 228: 0
+        line 223: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lsklearn/pipeline/Pipeline;
     Signature: #113                         // ()Ljava/util/List<[Ljava/lang/Object;>;
 }
 SourceFile: "Pipeline.java"
 InnerClasses:
```

#### sklearn/pipeline/Pipeline$1.class

##### procyon -ec {}

```diff
@@ -1,22 +1,18 @@
 
 package sklearn.pipeline;
 
 import org.jpmml.python.ClassDictUtil;
 import sklearn.PassThrough;
-import sklearn.None;
 import sklearn.Transformer;
 import org.jpmml.python.CastFunction;
 
 class Pipeline$1 extends CastFunction<Transformer> {
     public Transformer apply(final Object object) {
-        if (object == null) {
-            return (Transformer)None.INSTANCE;
-        }
-        if ("passthrough".equals(object)) {
+        if (object == null || "passthrough".equals(object)) {
             return (Transformer)PassThrough.INSTANCE;
         }
         return (Transformer)super.apply(object);
     }
     
     public String formatMessage(final Object object) {
         return "The transformer object (" + ClassDictUtil.formatClass(object) + ") is not a supported Transformer";
```

#### sklearn/OutlierDetectorUtil.class

##### procyon -ec {}

```diff
@@ -12,16 +12,16 @@
 import org.dmg.pmml.Output;
 
 public class OutlierDetectorUtil
 {
     private OutlierDetectorUtil() {
     }
     
-    public static <E extends Estimator & OutlierDetector & HasDecisionFunctionField> Output createPredictedOutput(final E estimator) {
-        final Output output = createPredictedOutput(estimator, ((E)estimator).getDecisionFunctionField(), new Transformation[0]);
+    public static <E extends Estimator & OutlierDetector> Output createPredictedOutput(final E estimator) {
+        final Output output = createPredictedOutput(estimator, ((HasDecisionFunctionField)estimator).getDecisionFunctionField(), new Transformation[0]);
         final List<OutputField> outputFields = output.getOutputFields();
         final OutputField decisionFunctionOutputField = (OutputField)outputFields.get(0);
         if (!decisionFunctionOutputField.isFinalResult()) {
             decisionFunctionOutputField.setFinalResult(Boolean.valueOf(true));
         }
         return output;
     }
```

#### sklearn/HasMultiApplyField.class

##### procyon -ec {}

```diff
@@ -1,24 +1,24 @@
 
 package sklearn;
 
 import org.jpmml.converter.FieldNameUtil;
 import java.util.ArrayList;
 import java.util.List;
 
-public interface HasMultiApplyField extends HasApplyField
+public interface HasMultiApplyField
 {
     int getNumberOfApplyFields();
     
-    default List<String> getApplyFields() {
+    default List<String> getMultiApplyFields() {
         final List<String> result = new ArrayList<String>();
         for (int i = 0, max = this.getNumberOfApplyFields(); i < max; ++i) {
-            final String name = this.getApplyField(Integer.valueOf(i + 1));
+            final String name = this.getMultiApplyField(Integer.valueOf(i + 1));
             result.add(name);
         }
         return result;
     }
     
-    default String getApplyField(final Object segmentId) {
-        return FieldNameUtil.create(this.getApplyField(), new Object[] { segmentId });
+    default String getMultiApplyField(final Object segmentId) {
+        return FieldNameUtil.create("apply", new Object[] { segmentId });
     }
 }
```

#### sklearn/svm/OneClassSVM.class

##### procyon -ec {}

```diff
@@ -3,17 +3,16 @@
 
 import org.dmg.pmml.Model;
 import sklearn.Estimator;
 import sklearn.OutlierDetectorUtil;
 import org.dmg.pmml.support_vector_machine.SupportVectorMachineModel;
 import org.jpmml.converter.Schema;
 import sklearn.OutlierDetector;
-import sklearn.HasDecisionFunctionField;
 
-public class OneClassSVM extends LibSVMRegressor implements HasDecisionFunctionField, OutlierDetector
+public class OneClassSVM extends LibSVMRegressor implements OutlierDetector
 {
     public OneClassSVM(final String module, final String name) {
         super(module, name);
     }
     
     public boolean isSupervised() {
         return false;
```

#### sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class

##### procyon -ec {}

```diff
@@ -6,18 +6,17 @@
 import sklearn.OutlierDetectorUtil;
 import java.util.List;
 import org.jpmml.converter.regression.RegressionModelUtil;
 import com.google.common.collect.Iterables;
 import org.dmg.pmml.regression.RegressionModel;
 import org.jpmml.converter.Schema;
 import sklearn.OutlierDetector;
-import sklearn.HasDecisionFunctionField;
 import sklearn.Regressor;
 
-public class SGDOneClassSVM extends Regressor implements HasDecisionFunctionField, OutlierDetector
+public class SGDOneClassSVM extends Regressor implements OutlierDetector
 {
     public SGDOneClassSVM(final String module, final String name) {
         super(module, name);
     }
     
     public boolean isSupervised() {
         return false;
```

#### sklearn/PassThrough.class

##### procyon -ec {}

```diff
@@ -1,23 +1,15 @@
 
 package sklearn;
 
-import org.jpmml.sklearn.SkLearnEncoder;
-import org.jpmml.converter.Feature;
-import java.util.List;
-
-public class PassThrough extends MultiTransformer
+public class PassThrough extends IdentityTransformer
 {
     public static final PassThrough INSTANCE;
     
     private PassThrough() {
         super((String)null, "_passthrough");
     }
     
-    public List<Feature> encodeFeatures(final List<Feature> features, final SkLearnEncoder encoder) {
-        return features;
-    }
-    
     static {
         INSTANCE = new PassThrough();
     }
 }
```

#### sklearn/ensemble/forest/ForestRegressor.class

##### procyon -ec {}

```diff
@@ -3,14 +3,15 @@
 
 import org.dmg.pmml.Model;
 import java.util.List;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.mining.Segmentation;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
+import org.jpmml.converter.FieldNameUtil;
 import sklearn.Estimator;
 import org.dmg.pmml.DataType;
 import sklearn.tree.HasTreeOptions;
 import sklearn.HasMultiApplyField;
 import sklearn.tree.TreeRegressor;
 import sklearn.HasEstimatorEnsemble;
 import sklearn.Regressor;
@@ -25,16 +26,16 @@
         return DataType.FLOAT;
     }
     
     public int getNumberOfApplyFields() {
         return ForestUtil.getNumberOfEstimators((Estimator)this);
     }
     
-    public String getApplyField() {
-        return "nodeId";
+    public String getMultiApplyField(final Object segmentId) {
+        return FieldNameUtil.create("nodeId", new Object[] { segmentId });
     }
     
     public MiningModel encodeModel(final Schema schema) {
         return ForestUtil.encodeBaseForest((Estimator)this, Segmentation.MultipleModelMethod.AVERAGE, MiningFunction.REGRESSION, schema);
     }
     
     public List<? extends TreeRegressor> getEstimators() {
```

#### sklearn/ensemble/forest/ForestClassifier.class

##### procyon -ec {}

```diff
@@ -4,14 +4,15 @@
 import java.util.List;
 import org.dmg.pmml.Model;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.mining.Segmentation;
 import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
+import org.jpmml.converter.FieldNameUtil;
 import sklearn.Estimator;
 import org.dmg.pmml.DataType;
 import sklearn.tree.HasTreeOptions;
 import sklearn.HasMultiApplyField;
 import sklearn.tree.TreeClassifier;
 import sklearn.HasEstimatorEnsemble;
 import sklearn.Classifier;
@@ -26,16 +27,16 @@
         return DataType.FLOAT;
     }
     
     public int getNumberOfApplyFields() {
         return ForestUtil.getNumberOfEstimators((Estimator)this);
     }
     
-    public String getApplyField() {
-        return "nodeId";
+    public String getMultiApplyField(final Object segmentId) {
+        return FieldNameUtil.create("nodeId", new Object[] { segmentId });
     }
     
     public MiningModel encodeModel(final Schema schema) {
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         final MiningModel miningModel = ForestUtil.encodeBaseForest((Estimator)this, Segmentation.MultipleModelMethod.AVERAGE, MiningFunction.CLASSIFICATION, schema);
         this.encodePredictProbaOutput((Model)miningModel, DataType.DOUBLE, categoricalLabel);
         return miningModel;
```

#### sklearn/ensemble/iforest/IsolationForest$3.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum f910951941a382c5b16ae325f86c2815de76d82e5b76c48688b6e6ddbc744961
+  SHA-256 checksum e869440e5af0d1a19749baaed37f5becc4c266e4acc4291b49f868b565981e32
   Compiled from "IsolationForest.java"
 class sklearn.ensemble.iforest.IsolationForest$3 extends org.jpmml.converter.transformations.AbstractTransformation
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #18                         // sklearn/ensemble/iforest/IsolationForest$3
   super_class: #19                        // org/jpmml/converter/transformations/AbstractTransformation
@@ -102,15 +102,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field this$0:Lsklearn/ensemble/iforest/IsolationForest;
          5: aload_0
          6: invokespecial #2                  // Method org/jpmml/converter/transformations/AbstractTransformation."<init>":()V
          9: return
       LineNumberTable:
-        line 163: 0
+        line 162: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lsklearn/ensemble/iforest/IsolationForest$3;
             0      10     1 this$0   Lsklearn/ensemble/iforest/IsolationForest;
 
   public java.lang.String getName(java.lang.String);
     descriptor: (Ljava/lang/String;)Ljava/lang/String;
@@ -118,29 +118,29 @@
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: getfield      #1                  // Field this$0:Lsklearn/ensemble/iforest/IsolationForest;
          4: invokevirtual #3                  // Method sklearn/ensemble/iforest/IsolationForest.getDecisionFunctionField:()Ljava/lang/String;
          7: areturn
       LineNumberTable:
-        line 167: 0
+        line 166: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lsklearn/ensemble/iforest/IsolationForest$3;
             0       8     1  name   Ljava/lang/String;
 
   public boolean isFinalResult();
     descriptor: ()Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: iconst_1
          1: ireturn
       LineNumberTable:
-        line 172: 0
+        line 171: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lsklearn/ensemble/iforest/IsolationForest$3;
 
   public org.dmg.pmml.Expression createExpression(org.dmg.pmml.FieldRef);
     descriptor: (Lorg/dmg/pmml/FieldRef;)Lorg/dmg/pmml/Expression;
     flags: (0x0001) ACC_PUBLIC
@@ -190,16 +190,16 @@
         72: invokestatic  #17                 // Method org/jpmml/converter/PMMLUtil.createApply:(Ljava/lang/String;[Lorg/dmg/pmml/Expression;)Lorg/dmg/pmml/Apply;
         75: aastore
         76: invokestatic  #17                 // Method org/jpmml/converter/PMMLUtil.createApply:(Ljava/lang/String;[Lorg/dmg/pmml/Expression;)Lorg/dmg/pmml/Apply;
         79: aastore
         80: invokestatic  #17                 // Method org/jpmml/converter/PMMLUtil.createApply:(Ljava/lang/String;[Lorg/dmg/pmml/Expression;)Lorg/dmg/pmml/Apply;
         83: areturn
       LineNumberTable:
-        line 177: 0
-        line 179: 8
+        line 176: 0
+        line 178: 8
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      84     0  this   Lsklearn/ensemble/iforest/IsolationForest$3;
             0      84     1 fieldRef   Lorg/dmg/pmml/FieldRef;
             8      76     2 offset   Ljava/lang/Number;
 }
 SourceFile: "IsolationForest.java"
```

#### sklearn/ensemble/iforest/IsolationForest$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum d7cf65bf37f9b925e92f6be5ffd259fd44a6e727a765f22b447bf5b1128fe489
+  SHA-256 checksum 51d1497e80b08663471601ea8a6d56a9fb3bbd09546883184af6edfafc989979
   Compiled from "IsolationForest.java"
 class sklearn.ensemble.iforest.IsolationForest$1 extends org.jpmml.model.visitors.AbstractVisitor
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #23                         // sklearn/ensemble/iforest/IsolationForest$1
   super_class: #24                        // org/jpmml/model/visitors/AbstractVisitor
@@ -175,16 +175,16 @@
         25: aload_0
         26: aload_0
         27: getfield      #2                  // Field val$tree:Lsklearn/tree/Tree;
         30: invokevirtual #6                  // Method sklearn/tree/Tree.getNodeSamples:()[I
         33: putfield      #7                  // Field nodeSamples:[I
         36: return
       LineNumberTable:
-        line 106: 0
-        line 108: 25
+        line 105: 0
+        line 107: 25
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      37     0  this   Lsklearn/ensemble/iforest/IsolationForest$1;
             0      37     1 this$0   Lsklearn/ensemble/iforest/IsolationForest;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.tree.Node);
     descriptor: (Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
@@ -246,26 +246,26 @@
        116: invokevirtual #21                 // Method org/dmg/pmml/tree/Node.setScore:(Ljava/lang/Object;)Lorg/dmg/pmml/tree/Node;
        119: pop
        120: aload_0
        121: aload_1
        122: invokespecial #22                 // Method org/jpmml/model/visitors/AbstractVisitor.visit:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
        125: areturn
       LineNumberTable:
-        line 114: 0
-        line 115: 7
-        line 117: 9
-        line 118: 15
-        line 120: 46
-        line 121: 54
-        line 124: 57
-        line 125: 61
-        line 127: 64
-        line 129: 82
-        line 131: 108
-        line 134: 120
+        line 113: 0
+        line 114: 7
+        line 116: 9
+        line 117: 15
+        line 119: 46
+        line 120: 54
+        line 123: 57
+        line 124: 61
+        line 126: 64
+        line 128: 82
+        line 130: 108
+        line 133: 120
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            46      15     6 parent   Lorg/dmg/pmml/PMMLObject;
             9     111     2 nodeDepth   D
            15     105     4 parents   Ljava/util/Deque;
            82      38     5 nodeSample   D
           108      12     7 averagePathLength   D
```

#### sklearn/ensemble/iforest/IsolationForest$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum f9b628588ece0aa30fea4df3177b1182efef9401b1f926367e7b73cf6da6555b
+  SHA-256 checksum b22708f10af1900733eb6de7a8a10379efee25dde8b4eb4a12840fa24b3e6c26
   Compiled from "IsolationForest.java"
 class sklearn.ensemble.iforest.IsolationForest$2 extends org.jpmml.converter.transformations.AbstractTransformation
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #15                         // sklearn/ensemble/iforest/IsolationForest$2
   super_class: #16                        // org/jpmml/converter/transformations/AbstractTransformation
@@ -117,29 +117,29 @@
         10: aload_0
         11: iload_3
         12: putfield      #3                  // Field val$nodeSampleCorrected:Z
         15: aload_0
         16: invokespecial #4                  // Method org/jpmml/converter/transformations/AbstractTransformation."<init>":()V
         19: return
       LineNumberTable:
-        line 145: 0
+        line 144: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lsklearn/ensemble/iforest/IsolationForest$2;
             0      20     1 this$0   Lsklearn/ensemble/iforest/IsolationForest;
 
   public java.lang.String getName(java.lang.String);
     descriptor: (Ljava/lang/String;)Ljava/lang/String;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=2, args_size=2
          0: ldc           #5                  // String normalizedAnomalyScore
          2: areturn
       LineNumberTable:
-        line 149: 0
+        line 148: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       3     0  this   Lsklearn/ensemble/iforest/IsolationForest$2;
             0       3     1  name   Ljava/lang/String;
 
   public org.dmg.pmml.Expression createExpression(org.dmg.pmml.FieldRef);
     descriptor: (Lorg/dmg/pmml/FieldRef;)Lorg/dmg/pmml/Expression;
@@ -174,17 +174,17 @@
         45: dload         4
         47: invokestatic  #12                 // Method java/lang/Double.valueOf:(D)Ljava/lang/Double;
         50: invokestatic  #13                 // Method org/jpmml/converter/PMMLUtil.createConstant:(Ljava/lang/Number;)Lorg/dmg/pmml/Constant;
         53: aastore
         54: invokestatic  #14                 // Method org/jpmml/converter/PMMLUtil.createApply:(Ljava/lang/String;[Lorg/dmg/pmml/Expression;)Lorg/dmg/pmml/Apply;
         57: areturn
       LineNumberTable:
-        line 154: 0
-        line 156: 9
-        line 158: 33
+        line 153: 0
+        line 155: 9
+        line 157: 33
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      58     0  this   Lsklearn/ensemble/iforest/IsolationForest$2;
             0      58     1 fieldRef   Lorg/dmg/pmml/FieldRef;
             9      49     2 maxSamples   D
            33      25     4 averagePathLength   D
       StackMapTable: number_of_entries = 2
```

#### sklearn/ensemble/iforest/IsolationForest.class

##### procyon -ec {}

```diff
@@ -27,18 +27,17 @@
 import org.jpmml.converter.ScoreDistributionManager;
 import org.jpmml.converter.PredicateManager;
 import sklearn.SkLearnUtil;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import sklearn.OutlierDetector;
 import sklearn.tree.HasTreeOptions;
-import sklearn.HasDecisionFunctionField;
 import sklearn.ensemble.EnsembleRegressor;
 
-public class IsolationForest extends EnsembleRegressor implements HasDecisionFunctionField, HasTreeOptions, OutlierDetector
+public class IsolationForest extends EnsembleRegressor implements HasTreeOptions, OutlierDetector
 {
     public IsolationForest(final String module, final String name) {
         super(module, name);
     }
     
     public boolean isSupervised() {
         return false;
```

#### sklearn/tree/TreeUtil$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 8be5aebcb04997f46dae0611df7ecd7cc6ed555a4c0a52f100b83e7bf3963273
+  SHA-256 checksum 2cf9b63373142a9ba06f612a67848657d6d5b22d82e076fbc2af8b86632a1225
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$1 extends org.jpmml.converter.visitors.AbstractExtender
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #27                         // sklearn/tree/TreeUtil$1
   super_class: #28                        // org/jpmml/converter/visitors/AbstractExtender
@@ -180,16 +180,16 @@
          6: aload_1
          7: invokespecial #2                  // Method org/jpmml/converter/visitors/AbstractExtender."<init>":(Ljava/lang/String;)V
         10: aload_0
         11: getstatic     #3                  // Field org/dmg/pmml/tree/SimplifyingNodeTransformer.INSTANCE:Lorg/dmg/pmml/tree/SimplifyingNodeTransformer;
         14: putfield      #4                  // Field nodeTransformer:Lorg/dmg/pmml/tree/NodeTransformer;
         17: return
       LineNumberTable:
-        line 133: 0
-        line 135: 10
+        line 131: 0
+        line 133: 10
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      18     0  this   Lsklearn/tree/TreeUtil$1;
             0      18     1    x0   Ljava/lang/String;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.tree.TreeModel);
     descriptor: (Lorg/dmg/pmml/tree/TreeModel;)Lorg/dmg/pmml/VisitorAction;
@@ -204,16 +204,16 @@
          9: invokevirtual #7                  // Method org/dmg/pmml/tree/TreeModel.setNode:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/tree/TreeModel;
         12: pop
         13: aload_0
         14: aload_1
         15: invokespecial #8                  // Method org/jpmml/converter/visitors/AbstractExtender.visit:(Lorg/dmg/pmml/tree/TreeModel;)Lorg/dmg/pmml/VisitorAction;
         18: areturn
       LineNumberTable:
-        line 140: 0
-        line 142: 13
+        line 138: 0
+        line 140: 13
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      19     0  this   Lsklearn/tree/TreeUtil$1;
             0      19     1 treeModel   Lorg/dmg/pmml/tree/TreeModel;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.tree.Node);
     descriptor: (Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
@@ -257,23 +257,23 @@
         74: invokestatic  #19                 // Method org/jpmml/converter/ValueUtil.asString:(Ljava/lang/Object;)Ljava/lang/String;
         77: invokevirtual #20                 // Method addExtension:(Lorg/dmg/pmml/PMMLObject;Ljava/lang/String;)V
         80: aload_0
         81: aload_1
         82: invokespecial #21                 // Method org/jpmml/converter/visitors/AbstractExtender.visit:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
         85: areturn
       LineNumberTable:
-        line 148: 0
-        line 149: 7
-        line 151: 12
-        line 152: 28
-        line 156: 50
-        line 157: 56
-        line 158: 60
-        line 160: 65
-        line 163: 80
+        line 146: 0
+        line 147: 7
+        line 149: 12
+        line 150: 28
+        line 154: 50
+        line 155: 56
+        line 156: 60
+        line 158: 65
+        line 161: 80
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            19      31     3 childIt   Ljava/util/ListIterator;
            12      38     2 children   Ljava/util/List;
             0      86     0  this   Lsklearn/tree/TreeUtil$1;
             0      86     1  node   Lorg/dmg/pmml/tree/Node;
            56      30     2 value   Ljava/lang/Object;
@@ -311,20 +311,20 @@
         20: getfield      #4                  // Field nodeTransformer:Lorg/dmg/pmml/tree/NodeTransformer;
         23: aload_1
         24: invokeinterface #22,  2           // InterfaceMethod org/dmg/pmml/tree/NodeTransformer.toComplexNode:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/tree/ComplexNode;
         29: areturn
         30: aload_1
         31: areturn
       LineNumberTable:
-        line 168: 0
-        line 169: 7
-        line 172: 9
-        line 173: 15
-        line 174: 19
-        line 177: 30
+        line 166: 0
+        line 167: 7
+        line 170: 9
+        line 171: 15
+        line 172: 19
+        line 175: 30
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      32     0  this   Lsklearn/tree/TreeUtil$1;
             0      32     1  node   Lorg/dmg/pmml/tree/Node;
            15      17     2 value   Ljava/lang/Object;
       StackMapTable: number_of_entries = 2
         frame_type = 9 /* same */
@@ -344,16 +344,16 @@
         10: astore_2
         11: aload_0
         12: getfield      #1                  // Field val$values:Ljava/util/Map;
         15: aload_2
         16: invokeinterface #26,  2           // InterfaceMethod java/util/Map.get:(Ljava/lang/Object;)Ljava/lang/Object;
         21: areturn
       LineNumberTable:
-        line 181: 0
-        line 183: 11
+        line 179: 0
+        line 181: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      22     0  this   Lsklearn/tree/TreeUtil$1;
             0      22     1  node   Lorg/dmg/pmml/tree/Node;
            11      11     2    id   Ljava/lang/Integer;
 }
 SourceFile: "TreeUtil.java"
```

#### sklearn/tree/TreeUtil$4.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum cd16e1b1849a751f6299f74a84e91d674062260cbfde1e1e3fe7e46a099e1799
+  SHA-256 checksum 1c1677eafe5eda9742c4956d51a196709ebb960ed8853471fd364a92e4e1ee70
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$4 extends java.lang.Object implements java.util.function.Function<T, org.dmg.pmml.tree.TreeModel>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #16                         // sklearn/tree/TreeUtil$4
   super_class: #17                        // java/lang/Object
@@ -146,15 +146,15 @@
         21: aload_0
         22: aload         5
         24: putfield      #5                  // Field val$scoreDistributionManager:Lorg/jpmml/converter/ScoreDistributionManager;
         27: aload_0
         28: invokespecial #6                  // Method java/lang/Object."<init>":()V
         31: return
       LineNumberTable:
-        line 251: 0
+        line 249: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      32     0  this   Lsklearn/tree/TreeUtil$4;
 
   public org.dmg.pmml.tree.TreeModel apply(T);
     descriptor: (Lsklearn/Estimator;)Lorg/dmg/pmml/tree/TreeModel;
     flags: (0x0001) ACC_PUBLIC
@@ -193,20 +193,20 @@
         61: aload_1
         62: aload_3
         63: aload         4
         65: invokevirtual #13                 // Method sklearn/Estimator.addFeatureImportances:(Lorg/dmg/pmml/Model;Lorg/jpmml/converter/Schema;)V
         68: aload_3
         69: areturn
       LineNumberTable:
-        line 255: 0
-        line 257: 19
-        line 260: 41
-        line 261: 48
-        line 263: 61
-        line 266: 68
+        line 253: 0
+        line 255: 19
+        line 258: 41
+        line 259: 48
+        line 261: 61
+        line 264: 68
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            61       7     4 featureImportanceSchema   Lorg/jpmml/converter/Schema;
             0      70     0  this   Lsklearn/tree/TreeUtil$4;
             0      70     1 estimator   Lsklearn/Estimator;
            19      51     2 treeModelSchema   Lorg/jpmml/converter/Schema;
            41      29     3 treeModel   Lorg/dmg/pmml/tree/TreeModel;
@@ -226,15 +226,15 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: checkcast     #14                 // class sklearn/Estimator
          5: invokevirtual #15                 // Method apply:(Lsklearn/Estimator;)Lorg/dmg/pmml/tree/TreeModel;
          8: areturn
       LineNumberTable:
-        line 251: 0
+        line 249: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lsklearn/tree/TreeUtil$4;
 }
 Signature: #53                          // Ljava/lang/Object;Ljava/util/function/Function<TT;Lorg/dmg/pmml/tree/TreeModel;>;
 SourceFile: "TreeUtil.java"
 EnclosingMethod: #57.#58                // sklearn.tree.TreeUtil.encodeTreeModelEnsemble
```

#### sklearn/tree/TreeUtil$5.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum df3560b0bb449738226a74dc63c33dc4b2ac8c225d9dbb269005159626286b47
+  SHA-256 checksum 78acc6ac457e809e7ee42ecacb401ecb810b9b1af4add6598e7b82b931f00ae6
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$5 extends java.util.AbstractList<java.lang.Number>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #5                          // sklearn/tree/TreeUtil$5
   super_class: #6                         // java/util/AbstractList
@@ -67,30 +67,30 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field val$leafValues:[D
          5: aload_0
          6: invokespecial #2                  // Method java/util/AbstractList."<init>":()V
          9: return
       LineNumberTable:
-        line 411: 0
+        line 409: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lsklearn/tree/TreeUtil$5;
 
   public int size();
     descriptor: ()I
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #1                  // Field val$leafValues:[D
          4: arraylength
          5: ireturn
       LineNumberTable:
-        line 415: 0
+        line 413: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/tree/TreeUtil$5;
 
   public java.lang.Number get(int);
     descriptor: (I)Ljava/lang/Number;
     flags: (0x0001) ACC_PUBLIC
@@ -101,16 +101,16 @@
          4: iload_1
          5: daload
          6: dstore_2
          7: dload_2
          8: invokestatic  #3                  // Method org/jpmml/converter/ValueUtil.narrow:(D)Ljava/lang/Number;
         11: areturn
       LineNumberTable:
-        line 420: 0
-        line 422: 7
+        line 418: 0
+        line 420: 7
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lsklearn/tree/TreeUtil$5;
             0      12     1 index   I
             7       5     2 leafValue   D
 
   public java.lang.Object get(int);
@@ -119,15 +119,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: iload_1
          2: invokevirtual #4                  // Method get:(I)Ljava/lang/Number;
          5: areturn
       LineNumberTable:
-        line 411: 0
+        line 409: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/tree/TreeUtil$5;
 }
 Signature: #27                          // Ljava/util/AbstractList<Ljava/lang/Number;>;
 SourceFile: "TreeUtil.java"
 EnclosingMethod: #31.#32                // sklearn.tree.TreeUtil.encodeNode
```

#### sklearn/tree/TreeUtil$6.class

##### procyon -ec {}

```diff
@@ -1,16 +1,25 @@
 
 package sklearn.tree;
 
-import org.dmg.pmml.VisitorAction;
-import org.dmg.pmml.tree.Node;
-import java.util.List;
-import org.jpmml.model.visitors.AbstractVisitor;
+import org.jpmml.converter.ContinuousFeature;
+import org.jpmml.converter.ThresholdFeature;
+import org.jpmml.converter.BinaryFeature;
+import org.dmg.pmml.DataType;
+import org.jpmml.converter.Feature;
+import java.util.function.Function;
 
-static final class TreeUtil$6 extends AbstractVisitor {
-    public VisitorAction visit(final Node node) {
-        if (!node.hasNodes()) {
-            this.val$result.add(node.getId());
+static final class TreeUtil$6 implements Function<Feature, Feature> {
+    @Override
+    public Feature apply(final Feature feature) {
+        if (feature instanceof BinaryFeature) {
+            final BinaryFeature binaryFeature = (BinaryFeature)feature;
+            return (Feature)binaryFeature;
         }
-        return super.visit(node);
+        if (feature instanceof ThresholdFeature && !this.val$numeric) {
+            final ThresholdFeature thresholdFeature = (ThresholdFeature)feature;
+            return (Feature)thresholdFeature;
+        }
+        final ContinuousFeature continuousFeature = feature.toContinuousFeature(this.val$dataType);
+        return (Feature)continuousFeature;
     }
 }
```

#### sklearn/tree/TreeUtil$7.class

##### procyon -ec {}

```diff
@@ -1,25 +1,24 @@
 
 package sklearn.tree;
 
 import org.jpmml.converter.ContinuousFeature;
 import org.jpmml.converter.ThresholdFeature;
 import org.jpmml.converter.BinaryFeature;
-import org.dmg.pmml.DataType;
 import org.jpmml.converter.Feature;
 import java.util.function.Function;
 
 static final class TreeUtil$7 implements Function<Feature, Feature> {
     @Override
     public Feature apply(final Feature feature) {
         if (feature instanceof BinaryFeature) {
             final BinaryFeature binaryFeature = (BinaryFeature)feature;
             return (Feature)binaryFeature;
         }
         if (feature instanceof ThresholdFeature && !this.val$numeric) {
             final ThresholdFeature thresholdFeature = (ThresholdFeature)feature;
             return (Feature)thresholdFeature;
         }
-        final ContinuousFeature continuousFeature = feature.toContinuousFeature(this.val$dataType);
+        final ContinuousFeature continuousFeature = TreeUtil.access$200(feature);
         return (Feature)continuousFeature;
     }
 }
```

#### sklearn/tree/TreeUtil.class

##### procyon -ec {}

```diff
@@ -1,17 +1,15 @@
 
 package sklearn.tree;
 
-import org.dmg.pmml.OutputField;
 import org.dmg.pmml.mining.Segmentation;
-import org.dmg.pmml.DataType;
 import org.jpmml.model.UnsupportedElementException;
 import org.dmg.pmml.mining.Segment;
-import sklearn.HasMultiApplyField;
 import org.dmg.pmml.mining.MiningModel;
+import org.dmg.pmml.DataType;
 import org.jpmml.converter.ContinuousFeature;
 import org.dmg.pmml.tree.LeafNode;
 import org.dmg.pmml.PMMLObject;
 import com.google.common.primitives.Doubles;
 import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.tree.BranchNode;
 import org.dmg.pmml.tree.ClassifierNode;
@@ -222,54 +220,45 @@
             final double value4 = values[index];
             result2 = (Node)new LeafNode((Object)Double.valueOf(value4), predicate).setId((Object)id);
         }
         return result2;
     }
     
     private static void encodeNodeId(final Estimator estimator, final Model model) {
-        if (model instanceof MiningModel) {
+        if (model instanceof TreeModel) {
+            final TreeModel treeModel = (TreeModel)model;
+            estimator.encodeApplyOutput((Model)treeModel, DataType.INTEGER);
+        }
+        else {
+            if (!(model instanceof MiningModel)) {
+                throw new IllegalArgumentException();
+            }
             final MiningModel miningModel = (MiningModel)model;
-            final HasMultiApplyField hasMultiApplyField = (HasMultiApplyField)estimator;
             final Segmentation segmentation = miningModel.requireSegmentation();
             final List<Segment> segments = segmentation.requireSegments();
+            final List<String> segmentIds = new ArrayList<String>();
             for (final Segment segment : segments) {
-                final TreeModel treeModel = (TreeModel)segment.requireModel((Class)TreeModel.class);
+                final TreeModel treeModel2 = (TreeModel)segment.requireModel((Class)TreeModel.class);
                 final String segmentId = segment.getId();
                 if (segmentId == null) {
                     throw new UnsupportedElementException((PMMLObject)segment);
                 }
-                final List<Integer> nodeIds = collectNodeIds(treeModel);
-                final OutputField applyField = estimator.encodeApplyOutput((Model)miningModel, DataType.INTEGER, (List)nodeIds);
-                applyField.setName(hasMultiApplyField.getApplyField((Object)segmentId)).setSegmentId(segmentId);
+                segmentIds.add(segmentId);
             }
+            estimator.encodeMultiApplyOutput((Model)miningModel, DataType.INTEGER, (List)segmentIds);
         }
-        else {
-            if (!(model instanceof TreeModel)) {
-                throw new IllegalArgumentException();
-            }
-            final TreeModel treeModel2 = (TreeModel)model;
-            final List<Integer> nodeIds2 = collectNodeIds(treeModel2);
-            estimator.encodeApplyOutput((Model)treeModel2, DataType.INTEGER, (List)nodeIds2);
-        }
-    }
-    
-    private static List<Integer> collectNodeIds(final TreeModel treeModel) {
-        final List<Integer> result = new ArrayList<Integer>();
-        final Visitor nodeIdCollector = (Visitor)new TreeUtil.TreeUtil$6((List)result);
-        nodeIdCollector.applyTo((Visitable)treeModel);
-        return result;
     }
     
     private static Schema toTreeModelSchema(final DataType dataType, final boolean numeric, final Schema schema) {
-        final Function<Feature, Feature> function = (Function<Feature, Feature>)new TreeUtil.TreeUtil$7(numeric, dataType);
+        final Function<Feature, Feature> function = (Function<Feature, Feature>)new TreeUtil.TreeUtil$6(numeric, dataType);
         return schema.toTransformedSchema((Function)function);
     }
     
     private static Schema toTreeModelFeatureImportanceSchema(final boolean numeric, final Schema schema) {
-        final Function<Feature, Feature> function = (Function<Feature, Feature>)new TreeUtil.TreeUtil$8(numeric);
+        final Function<Feature, Feature> function = (Function<Feature, Feature>)new TreeUtil.TreeUtil$7(numeric);
         return schema.toTransformedSchema((Function)function);
     }
     
     private static ContinuousFeature toContinuousFeature(final Feature feature) {
         return feature.toContinuousFeature(DataType.FLOAT).toContinuousFeature(DataType.DOUBLE);
     }
```

#### sklearn/tree/TreeUtil$3.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum dca8a72a335aaef426dcb04c7c019d964578eaac211e88ea6db9de4e8ac79921
+  SHA-256 checksum 4c9394cee0ff3293ec9fe5c88ba68128f9d1db18a6bb0c3f25acc7dcccaa3fb4
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$3 extends org.jpmml.model.visitors.AbstractVisitor
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #8                          // sklearn/tree/TreeUtil$3
   super_class: #9                         // org/jpmml/model/visitors/AbstractVisitor
@@ -69,15 +69,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method org/jpmml/model/visitors/AbstractVisitor."<init>":()V
          4: return
       LineNumberTable:
-        line 206: 0
+        line 204: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn/tree/TreeUtil$3;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.tree.Node);
     descriptor: (Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
     flags: (0x0001) ACC_PUBLIC
@@ -99,20 +99,20 @@
         25: aload_2
         26: invokeinterface #6,  1            // InterfaceMethod java/util/List.clear:()V
         31: aload_0
         32: aload_1
         33: invokespecial #7                  // Method org/jpmml/model/visitors/AbstractVisitor.visit:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
         36: areturn
       LineNumberTable:
-        line 211: 0
-        line 212: 7
-        line 214: 13
-        line 215: 20
-        line 217: 25
-        line 221: 31
+        line 209: 0
+        line 210: 7
+        line 212: 13
+        line 213: 20
+        line 215: 25
+        line 219: 31
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            25       6     2 scoreDistributions   Ljava/util/List;
             0      37     0  this   Lsklearn/tree/TreeUtil$3;
             0      37     1  node   Lorg/dmg/pmml/tree/Node;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
```

#### sklearn/tree/TreeUtil$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum aea5b8005680539aa288fe10864010d5a7b29fd4320d79a0c8abae8b311a0bd5
+  SHA-256 checksum 1daf1f80556fb8ce31741c60d996f8cdaa94c188ff8f571d39189496a21725ef
   Compiled from "TreeUtil.java"
 final class sklearn.tree.TreeUtil$2 extends org.jpmml.model.visitors.AbstractVisitor
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #4                          // sklearn/tree/TreeUtil$2
   super_class: #5                         // org/jpmml/model/visitors/AbstractVisitor
@@ -48,15 +48,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method org/jpmml/model/visitors/AbstractVisitor."<init>":()V
          4: return
       LineNumberTable:
-        line 192: 0
+        line 190: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn/tree/TreeUtil$2;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.tree.Node);
     descriptor: (Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
     flags: (0x0001) ACC_PUBLIC
@@ -67,16 +67,16 @@
          2: invokevirtual #2                  // Method org/dmg/pmml/tree/Node.setId:(Ljava/lang/Object;)Lorg/dmg/pmml/tree/Node;
          5: pop
          6: aload_0
          7: aload_1
          8: invokespecial #3                  // Method org/jpmml/model/visitors/AbstractVisitor.visit:(Lorg/dmg/pmml/tree/Node;)Lorg/dmg/pmml/VisitorAction;
         11: areturn
       LineNumberTable:
-        line 196: 0
-        line 198: 6
+        line 194: 0
+        line 196: 6
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lsklearn/tree/TreeUtil$2;
             0      12     1  node   Lorg/dmg/pmml/tree/Node;
 }
 SourceFile: "TreeUtil.java"
 EnclosingMethod: #21.#22                // sklearn.tree.TreeUtil.transform
```

#### sklearn/OutlierDetector.class

##### procyon -ec {}

```diff
@@ -1,11 +1,11 @@
 
 package sklearn;
 
-public interface OutlierDetector extends HasOutlierField
+public interface OutlierDetector extends HasDecisionFunctionField, HasOutlierField
 {
     public static final String FIELD_OUTLIER = "outlier";
     
     default Number getDecisionFunctionThreshold() {
         return Double.valueOf(0.0);
     }
 }
```

#### sklearn/EstimatorUtil.class

##### procyon -ec {}

```diff
@@ -70,22 +70,22 @@
                     break;
                 }
                 break;
             }
         }
         switch (n) {
             case 0: {
-                if (estimator instanceof HasMultiApplyField) {
-                    final HasMultiApplyField hasMultiApplyField = (HasMultiApplyField)estimator;
-                    return encoder.export(model, hasMultiApplyField.getApplyFields());
-                }
                 if (estimator instanceof HasApplyField) {
                     final HasApplyField hasApplyField = (HasApplyField)estimator;
                     return encoder.export(model, hasApplyField.getApplyField());
                 }
+                if (estimator instanceof HasMultiApplyField) {
+                    final HasMultiApplyField hasMultiApplyField = (HasMultiApplyField)estimator;
+                    return encoder.export(model, hasMultiApplyField.getMultiApplyFields());
+                }
                 throw new IllegalArgumentException();
             }
             case 1: {
                 if (estimator instanceof HasDecisionFunctionField) {
                     final HasDecisionFunctionField hasDecisionFunctionField = (HasDecisionFunctionField)estimator;
                     return encoder.export(model, hasDecisionFunctionField.getDecisionFunctionField());
                 }
```

#### sklearn/Estimator.class

##### procyon -ec {}

```diff
@@ -1,14 +1,14 @@
 
 package sklearn;
 
 import org.slf4j.LoggerFactory;
+import java.util.Iterator;
+import java.util.ArrayList;
 import org.dmg.pmml.Output;
-import org.dmg.pmml.Field;
-import org.jpmml.converter.PMMLUtil;
 import java.util.stream.Collector;
 import java.util.stream.Collectors;
 import org.jpmml.converter.ModelUtil;
 import org.jpmml.converter.FieldNameUtil;
 import org.dmg.pmml.OutputField;
 import org.jpmml.converter.CategoricalLabel;
 import numpy.core.NDArrayUtil;
@@ -260,24 +260,47 @@
                 name = FieldNameUtil.create(name, new Object[] { pmmlSegmentId });
             }
             return ModelUtil.createEntityIdField(name, dataType);
         }
         throw new IllegalArgumentException();
     }
     
-    public OutputField encodeApplyOutput(final Model model, final DataType dataType, final List<?> values) {
+    public OutputField encodeApplyOutput(final Model model, final DataType dataType) {
         final OutputField applyField = this.createApplyField(dataType);
-        if (values != null && !values.isEmpty()) {
-            PMMLUtil.addValues((Field)applyField, (List)values);
-        }
         final Output output = ModelUtil.ensureOutput(model);
         output.getOutputFields().add(applyField);
         return applyField;
     }
     
+    public OutputField createMultiApplyField(final DataType dataType, final String segmentId) {
+        final Object pmmlSegmentId = this.getPMMLSegmentId();
+        if (this instanceof HasMultiApplyField) {
+            final HasMultiApplyField hasMultiApplyField = (HasMultiApplyField)this;
+            String name = hasMultiApplyField.getMultiApplyField((Object)segmentId);
+            if (pmmlSegmentId != null) {
+                name = FieldNameUtil.create(name, new Object[] { pmmlSegmentId });
+            }
+            final OutputField result = ModelUtil.createEntityIdField(name, dataType);
+            result.setSegmentId(segmentId);
+            return result;
+        }
+        throw new IllegalArgumentException();
+    }
+    
+    public List<OutputField> encodeMultiApplyOutput(final Model model, final DataType dataType, final List<String> segmentIds) {
+        final List<OutputField> applyFields = new ArrayList<OutputField>();
+        for (final String segmentId : segmentIds) {
+            final OutputField applyField = this.createMultiApplyField(dataType, segmentId);
+            applyFields.add(applyField);
+        }
+        final Output output = ModelUtil.ensureOutput(model);
+        output.getOutputFields().addAll(applyFields);
+        return applyFields;
+    }
+    
     protected static String extractArguments(final String function, final String name) {
         if (name.startsWith(function + "(") && name.endsWith(")")) {
             return name.substring((function + "(").length(), name.length() - ")".length());
         }
         return name;
     }
```

#### sklearn2pmml/pipeline/PMMLPipeline$3.class

##### procyon -ec {}

```diff
@@ -1,6 +1,16 @@
 
 package sklearn2pmml.pipeline;
 
-import org.dmg.pmml.DataType;
-import org.dmg.pmml.MiningFunction;
+import org.jpmml.converter.ValueUtil;
+import sklearn2pmml.decoration.Domain;
+import com.google.common.base.Function;
 
+static final class PMMLPipeline$3 implements Function<Object, Object> {
+    public Object apply(final Object value) {
+        Domain.checkValue(value);
+        if (ValueUtil.isNaN(value)) {
+            return null;
+        }
+        return value;
+    }
+}
```

#### sklearn2pmml/pipeline/PMMLPipeline.class

##### procyon -ec {}

```diff
@@ -6,14 +6,15 @@
 import com.google.common.collect.Lists;
 import org.jpmml.converter.ContinuousLabel;
 import org.dmg.pmml.Field;
 import org.dmg.pmml.Visitable;
 import org.dmg.pmml.Visitor;
 import org.dmg.pmml.OpType;
 import org.jpmml.converter.TypeUtil;
+import org.jpmml.python.CastFunction;
 import org.dmg.pmml.MiningFunction;
 import org.jpmml.converter.MultiLabel;
 import sklearn.HasEstimatorEnsemble;
 import sklearn.EstimatorUtil;
 import numpy.core.NDArrayUtil;
 import org.dmg.pmml.DefineFunction;
 import org.dmg.pmml.ResultFeature;
@@ -222,15 +223,15 @@
                     final int[] targetValuesShape = verification.getTargetValuesShape();
                     ClassDictUtil.checkShapes(0, new int[][] { activeValuesShape, targetValuesShape });
                     ClassDictUtil.checkSize(new Collection[] { targetFields, scalarLabels2 });
                     for (int l = 0; l < targetFields.size(); ++l) {
                         final VerificationField verificationField3 = ModelUtil.createVerificationField((String)targetFields.get(l));
                         final ScalarLabel scalarLabel3 = (ScalarLabel)scalarLabels2.get(l);
                         final DataType dataType = scalarLabel3.getDataType();
-                        switch (PMMLPipeline.PMMLPipeline$3.$SwitchMap$org$dmg$pmml$DataType[dataType.ordinal()]) {
+                        switch (PMMLPipeline.PMMLPipeline$4.$SwitchMap$org$dmg$pmml$DataType[dataType.ordinal()]) {
                             case 1:
                             case 2: {
                                 verificationField3.setPrecision(precision).setZeroThreshold(zeroThreshold);
                                 break;
                             }
                         }
                         final Domain domain2 = encoder.getDomain(verificationField3.requireField());
@@ -400,24 +401,35 @@
         PMMLPipeline.logger.warn("Attribute '" + ClassDictUtil.formatMember((ClassDict)this, "target_fields") + "' is not set. Assuming {} as the name of target fields", (Object)targetFields);
         return targetFields;
     }
     
     private static Label initLabel(final Estimator estimator, final List<String> targetFields, final SkLearnEncoder encoder) {
         final List<Label> labels = new ArrayList<Label>();
         final MiningFunction miningFunction = estimator.getMiningFunction();
-        switch (PMMLPipeline.PMMLPipeline$3.$SwitchMap$org$dmg$pmml$MiningFunction[miningFunction.ordinal()]) {
+        switch (PMMLPipeline.PMMLPipeline$4.$SwitchMap$org$dmg$pmml$MiningFunction[miningFunction.ordinal()]) {
             case 1: {
                 final List<?> categories = EstimatorUtil.getClasses(estimator);
                 final Map<String, Map<String, ?>> classExtensions = (Map)estimator.getOption("class_extensions", (Object)null);
                 if (classExtensions != null) {
                     ClassDictUtil.checkSize(1, new Collection[] { targetFields });
                 }
                 for (int i = 0; i < targetFields.size(); ++i) {
                     final String targetField = (String)targetFields.get(i);
-                    labels.add((Label)initCategoricalLabel(targetField, (targetFields.size() > 1) ? ((List)categories.get(i)) : categories, classExtensions, encoder));
+                    List<?> targetCategories;
+                    if (targetFields.size() == 1) {
+                        targetCategories = categories;
+                    }
+                    else {
+                        if (targetFields.size() < 2) {
+                            throw new IllegalArgumentException();
+                        }
+                        final CastFunction<List<?>> castFunction = (CastFunction<List<?>>)new PMMLPipeline.PMMLPipeline$1((Class)List.class, targetField);
+                        targetCategories = (List)castFunction.apply((Object)categories.get(i));
+                    }
+                    labels.add((Label)initCategoricalLabel(targetField, targetCategories, classExtensions, encoder));
                 }
                 break;
             }
             case 2: {
                 for (int j = 0; j < targetFields.size(); ++j) {
                     final String targetField2 = (String)targetFields.get(j);
                     labels.add((Label)initContinuousLabel(targetField2, encoder));
@@ -452,15 +464,15 @@
         final DataField dataField = encoder.createDataField(targetField, OpType.CATEGORICAL, dataType, (List)categories);
         final List<Visitor> visitors = new ArrayList<Visitor>();
         if (classExtensions != null) {
             final Collection<? extends Map.Entry<String, Map<String, ?>>> entries = classExtensions.entrySet();
             for (final Map.Entry<String, Map<String, ?>> entry : entries) {
                 final String name = (String)entry.getKey();
                 final Map<String, ?> values = (Map<String, ?>)entry.getValue();
-                final Visitor valueExtender = (Visitor)new PMMLPipeline.PMMLPipeline$1(name, (Map)values);
+                final Visitor valueExtender = (Visitor)new PMMLPipeline.PMMLPipeline$2(name, (Map)values);
                 visitors.add(valueExtender);
             }
         }
         for (final Visitor visitor : visitors) {
             visitor.applyTo((Visitable)dataField);
         }
         return new CategoricalLabel((Field)dataField);
@@ -477,15 +489,15 @@
             final DataField dataField = encoder.createDataField(activeField, opType, dataType);
             result.add((Feature)new WildcardFeature((PMMLEncoder)encoder, dataField));
         }
         return result;
     }
     
     private static List<?> cleanValues(final Domain domain, final List<?> values) {
-        final Function<Object, Object> function = (Function<Object, Object>)new PMMLPipeline.PMMLPipeline$2();
+        final Function<Object, Object> function = (Function<Object, Object>)new PMMLPipeline.PMMLPipeline$3();
         return Lists.transform((List)values, (Function)function);
     }
     
     private static List<String> makeVariables(final String name, final int count, final boolean indexed) {
         if (count <= 0) {
             throw new IllegalArgumentException();
         }
```

#### sklearn2pmml/pipeline/PMMLPipeline$2.class

##### procyon -ec {}

```diff
@@ -1,16 +1,21 @@
 
 package sklearn2pmml.pipeline;
 
+import org.dmg.pmml.PMMLObject;
 import org.jpmml.converter.ValueUtil;
-import sklearn2pmml.decoration.Domain;
-import com.google.common.base.Function;
+import numpy.core.ScalarUtil;
+import org.dmg.pmml.VisitorAction;
+import org.dmg.pmml.Value;
+import java.util.Map;
+import org.jpmml.converter.visitors.AbstractExtender;
 
-static final class PMMLPipeline$2 implements Function<Object, Object> {
-    public Object apply(final Object value) {
-        Domain.checkValue(value);
-        if (ValueUtil.isNaN(value)) {
-            return null;
+static final class PMMLPipeline$2 extends AbstractExtender {
+    public VisitorAction visit(final Value pmmlValue) {
+        Object value = this.val$values.get(pmmlValue.requireValue());
+        if (value != null) {
+            value = ScalarUtil.decode(value);
+            this.addExtension((PMMLObject)pmmlValue, ValueUtil.asString(value));
         }
-        return value;
+        return super.visit(pmmlValue);
     }
 }
```

#### sklearn2pmml/pipeline/PMMLPipeline$1.class

##### procyon -ec {}

```diff
@@ -1,21 +1,12 @@
 
 package sklearn2pmml.pipeline;
 
-import org.dmg.pmml.PMMLObject;
-import org.jpmml.converter.ValueUtil;
-import numpy.core.ScalarUtil;
-import org.dmg.pmml.VisitorAction;
-import org.dmg.pmml.Value;
-import java.util.Map;
-import org.jpmml.converter.visitors.AbstractExtender;
+import org.jpmml.python.ClassDictUtil;
+import java.util.List;
+import org.jpmml.python.CastFunction;
 
-static final class PMMLPipeline$1 extends AbstractExtender {
-    public VisitorAction visit(final Value pmmlValue) {
-        Object value = this.val$values.get(pmmlValue.requireValue());
-        if (value != null) {
-            value = ScalarUtil.decode(value);
-            this.addExtension((PMMLObject)pmmlValue, ValueUtil.asString(value));
-        }
-        return super.visit(pmmlValue);
+static final class PMMLPipeline$1 extends CastFunction<List<?>> {
+    public String formatMessage(final Object object) {
+        return "The categories object of the '" + this.val$targetField + "' target field (" + ClassDictUtil.formatClass(object) + ") is not supported";
     }
 }
```

#### sklearn2pmml/util/Reshaper.class

##### procyon -ec {}

```diff
@@ -1,31 +1,24 @@
 
 package sklearn2pmml.util;
 
-import org.jpmml.sklearn.SkLearnEncoder;
-import org.jpmml.converter.Feature;
-import java.util.List;
 import org.jpmml.converter.ValueUtil;
-import sklearn.MultiTransformer;
+import sklearn.IdentityTransformer;
 
-public class Reshaper extends MultiTransformer
+public class Reshaper extends IdentityTransformer
 {
     public Reshaper(final String module, final String name) {
         super(module, name);
     }
     
     public int getNumberOfFeatures() {
         final Object[] newshape = this.getNewshape();
         if (newshape.length >= 2) {
             return ValueUtil.asInteger((Number)newshape[1]);
         }
         return super.getNumberOfFeatures();
     }
     
-    public List<Feature> encodeFeatures(final List<Feature> features, final SkLearnEncoder encoder) {
-        return features;
-    }
-    
     public Object[] getNewshape() {
         return this.getTuple("newshape");
     }
 }
```

#### sklearn2pmml/tree/CHAIDRegressor.class

##### procyon -ec {}

```diff
@@ -1,14 +1,12 @@
 
 package sklearn2pmml.tree;
 
 import treelib.Tree;
-import java.util.List;
 import org.dmg.pmml.Model;
-import java.util.Collections;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.tree.TreeModel;
 import org.jpmml.converter.Schema;
 import sklearn.HasApplyField;
 import sklearn.Regressor;
 
@@ -21,15 +19,15 @@
     public String getApplyField() {
         return "nodeId";
     }
     
     public TreeModel encodeModel(final Schema schema) {
         final Tree tree = this.getTree();
         final TreeModel treeModel = CHAIDUtil.encodeModel(MiningFunction.REGRESSION, tree, schema);
-        this.encodeApplyOutput((Model)treeModel, DataType.INTEGER, (List)Collections.emptyList());
+        this.encodeApplyOutput((Model)treeModel, DataType.INTEGER);
         return treeModel;
     }
     
     public Tree getTree() {
         return (Tree)this.get("treelib_tree_", (Class)Tree.class);
     }
 }
```

#### sklearn2pmml/tree/CHAIDClassifier.class

##### procyon -ec {}

```diff
@@ -1,13 +1,11 @@
 
 package sklearn2pmml.tree;
 
 import treelib.Tree;
-import java.util.List;
-import java.util.Collections;
 import org.dmg.pmml.Model;
 import org.dmg.pmml.DataType;
 import org.dmg.pmml.MiningFunction;
 import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.tree.TreeModel;
 import org.jpmml.converter.Schema;
 import sklearn.HasApplyField;
@@ -24,15 +22,15 @@
     }
     
     public TreeModel encodeModel(final Schema schema) {
         final Tree tree = this.getTree();
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         final TreeModel treeModel = CHAIDUtil.encodeModel(MiningFunction.CLASSIFICATION, tree, schema);
         this.encodePredictProbaOutput((Model)treeModel, DataType.DOUBLE, categoricalLabel);
-        this.encodeApplyOutput((Model)treeModel, DataType.INTEGER, (List)Collections.emptyList());
+        this.encodeApplyOutput((Model)treeModel, DataType.INTEGER);
         return treeModel;
     }
     
     public Tree getTree() {
         return (Tree)this.get("treelib_tree_", (Class)Tree.class);
     }
 }
```

#### org/jpmml/sklearn/SkLearnEncoder.class

##### procyon -ec {}

```diff
@@ -29,45 +29,59 @@
 import java.util.Collection;
 import org.jpmml.converter.ContinuousFeature;
 import org.dmg.pmml.Field;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.converter.CategoricalFeature;
 import org.dmg.pmml.OutputField;
 import java.util.ArrayList;
+import org.dmg.pmml.PMML;
 import java.util.Collections;
 import java.util.LinkedHashMap;
 import org.dmg.pmml.Model;
+import org.dmg.pmml.Predicate;
 import org.jpmml.converter.Feature;
 import java.util.List;
 import org.jpmml.converter.Label;
 import sklearn2pmml.decoration.Domain;
 import java.util.Map;
 import org.jpmml.python.PythonEncoder;
 
 public class SkLearnEncoder extends PythonEncoder
 {
     private Map<String, Domain> domains;
     private Label label;
     private List<? extends Feature> features;
+    private Predicate predicate;
     private Model model;
     
     public SkLearnEncoder() {
         this.domains = new LinkedHashMap<String, Domain>();
         this.label = null;
         this.features = Collections.emptyList();
+        this.predicate = null;
         this.model = null;
     }
     
     public void addTransformer(final Model transformer) {
         if (this.hasModel()) {
             throw new IllegalStateException("Model is already defined");
         }
         super.addTransformer(transformer);
     }
     
+    public PMML encodePMML() {
+        final PMML pmml = super.encodePMML();
+        final Predicate predicate = this.getPredicate();
+        if (predicate == null) {
+            return pmml;
+        }
+        final PMML result = (PMML)new SkLearnEncoder.SkLearnEncoder$1(this, pmml, predicate);
+        return result;
+    }
+    
     public List<Feature> export(final Model model, final String name) {
         return this.export(model, Collections.singletonList(name));
     }
     
     public List<Feature> export(final Model model, final List<String> names) {
         final Output output = model.getOutput();
         if (output == null) {
@@ -79,17 +93,21 @@
             DerivedOutputField derivedOutputField = null;
             final List<OutputField> nameOutputFields = selectOutputFields(name, outputFields);
             for (final OutputField nameOutputField : nameOutputFields) {
                 derivedOutputField = this.createDerivedField(model, nameOutputField, true);
             }
             final OpType opType = derivedOutputField.getOpType();
             Feature feature = null;
-            switch (SkLearnEncoder.SkLearnEncoder$1.$SwitchMap$org$dmg$pmml$OpType[opType.ordinal()]) {
+            switch (SkLearnEncoder.SkLearnEncoder$3.$SwitchMap$org$dmg$pmml$OpType[opType.ordinal()]) {
                 case 1: {
-                    feature = (Feature)new CategoricalFeature((PMMLEncoder)this, (Field)derivedOutputField);
+                    if (derivedOutputField.hasValues()) {
+                        feature = (Feature)new CategoricalFeature((PMMLEncoder)this, (Field)derivedOutputField);
+                        break;
+                    }
+                    feature = (Feature)new SkLearnEncoder.SkLearnEncoder$2(this, (PMMLEncoder)this, (Field)derivedOutputField);
                     break;
                 }
                 case 2: {
                     feature = (Feature)new ContinuousFeature((PMMLEncoder)this, (Field)derivedOutputField);
                     break;
                 }
                 default: {
@@ -173,15 +191,15 @@
         List<? extends Feature> features = this.getFeatures();
         if (label instanceof ScalarLabel) {
             final ScalarLabel scalarLabel = (ScalarLabel)label;
             final Feature labelFeature = ScalarLabelUtil.findLabelFeature(scalarLabel, (List)features);
             if (labelFeature != null) {
                 final DataField dataField = (DataField)labelFeature.getField();
                 final OpType opType = dataField.requireOpType();
-                switch (SkLearnEncoder.SkLearnEncoder$1.$SwitchMap$org$dmg$pmml$OpType[opType.ordinal()]) {
+                switch (SkLearnEncoder.SkLearnEncoder$3.$SwitchMap$org$dmg$pmml$OpType[opType.ordinal()]) {
                     case 2: {
                         label = (Label)new ContinuousLabel((Field)dataField);
                         break;
                     }
                     case 1: {
                         label = (Label)new CategoricalLabel((Field)dataField);
                         break;
@@ -225,14 +243,22 @@
         return this.features;
     }
     
     public void setFeatures(final List<? extends Feature> features) {
         this.features = Objects.requireNonNull(features);
     }
     
+    public Predicate getPredicate() {
+        return this.predicate;
+    }
+    
+    public void setPredicate(final Predicate predicate) {
+        this.predicate = predicate;
+    }
+    
     public boolean hasModel() {
         final Model model = this.getModel();
         return model != null;
     }
     
     public Model getModel() {
         return this.model;
@@ -240,15 +266,15 @@
     
     public void setModel(final Model model) {
         this.model = model;
     }
     
     public static boolean isPrediction(final OutputField outputField) {
         final ResultFeature resultFeature = outputField.getResultFeature();
-        switch (SkLearnEncoder.SkLearnEncoder$1.$SwitchMap$org$dmg$pmml$ResultFeature[resultFeature.ordinal()]) {
+        switch (SkLearnEncoder.SkLearnEncoder$3.$SwitchMap$org$dmg$pmml$ResultFeature[resultFeature.ordinal()]) {
             case 1:
             case 2:
             case 3: {
                 return true;
             }
             default: {
                 return false;
```

#### org/jpmml/sklearn/SkLearnEncoder$1.class

##### procyon -ec {}

```diff
@@ -1,6 +1,48 @@
 
 package org.jpmml.sklearn;
 
-import org.dmg.pmml.OpType;
-import org.dmg.pmml.ResultFeature;
+import java.util.List;
+import org.dmg.pmml.mining.Segmentation;
+import org.jpmml.model.UnsupportedAttributeException;
+import java.util.stream.Collector;
+import java.util.stream.Collectors;
+import java.util.function.Function;
+import org.dmg.pmml.MiningFunction;
+import java.util.Set;
+import org.dmg.pmml.mining.Segment;
+import org.dmg.pmml.mining.MiningModel;
+import org.dmg.pmml.Model;
+import org.dmg.pmml.PMMLObject;
+import org.jpmml.model.ReflectionUtil;
+import org.dmg.pmml.Predicate;
+import org.dmg.pmml.PMML;
 
+class SkLearnEncoder$1 extends PMML {
+    {
+        ReflectionUtil.copyState((PMMLObject)this.val$pmml, (PMMLObject)this);
+    }
+    
+    public PMML addModels(final Model... models) {
+        if (models.length != 1) {
+            throw new IllegalArgumentException();
+        }
+        final MiningModel miningModel = (MiningModel)models[0];
+        final Segmentation segmentation = miningModel.requireSegmentation();
+        final Segmentation.MultipleModelMethod multipleModelMethod = segmentation.requireMultipleModelMethod();
+        switch (SkLearnEncoder.SkLearnEncoder$3.$SwitchMap$org$dmg$pmml$mining$Segmentation$MultipleModelMethod[multipleModelMethod.ordinal()]) {
+            case 1: {
+                final List<Segment> segments = segmentation.requireSegments();
+                final Segment finalSegment = (Segment)segments.get(segments.size() - 1);
+                finalSegment.setPredicate(this.val$predicate);
+                final Set<MiningFunction> miningFunctions = (Set<MiningFunction>)segments.stream().map((Function<? super Object, ?>)SkLearnEncoder$1::lambda$addModels$0).collect((Collector<? super Object, ?, Set<MiningFunction>>)Collectors.toSet());
+                if (miningFunctions.size() > 1) {
+                    miningModel.setMiningFunction(MiningFunction.MIXED);
+                }
+                return super.addModels(models);
+            }
+            default: {
+                throw new UnsupportedAttributeException((PMMLObject)segmentation, (Enum)multipleModelMethod);
+            }
+        }
+    }
+}
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.30</version>
+    <version>1.7.31</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn converter</name>
   <description>JPMML Scikit-Learn to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-sklearn
 groupId=org.jpmml
-version=1.7.30
+version=1.7.31
```

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/serpent-1.40.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/serpent-1.40.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/pickle-1.4.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/pickle-1.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/resources/gson-2.10.jar` & `sklearn2pmml-0.94.1/sklearn2pmml/resources/gson-2.10.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/h2o.py` & `sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/xgboost.py` & `sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/preprocessing/lightgbm.py` & `sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/tree/chaid.py` & `sklearn2pmml-0.94.1/sklearn2pmml/tree/chaid.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.0/sklearn2pmml/expression/__init__.py` & `sklearn2pmml-0.94.1/sklearn2pmml/expression/__init__.py`

 * *Files identical despite different names*

