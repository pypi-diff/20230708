# Comparing `tmp/slackker-1.0.1.tar.gz` & `tmp/slackker-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackker-1.0.1.tar", last modified: Tue Jan 31 18:03:22 2023, max compression
+gzip compressed data, was "slackker-1.1.0.tar", last modified: Sat Jul  8 11:50:23 2023, max compression
```

## Comparing `slackker-1.0.1.tar` & `slackker-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:03:22.185468 slackker-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-31 18:03:08.000000 slackker-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-01-31 18:03:22.185468 slackker-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-01-31 18:03:08.000000 slackker-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 18:03:22.185468 slackker-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-31 18:03:08.000000 slackker-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:03:22.181468 slackker-1.0.1/slackker/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-01-31 18:03:08.000000 slackker-1.0.1/slackker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-01-31 18:03:08.000000 slackker-1.0.1/slackker/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:03:22.185468 slackker-1.0.1/slackker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 18:03:08.000000 slackker-1.0.1/slackker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-01-31 18:03:08.000000 slackker-1.0.1/slackker/utils/ccolors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-01-31 18:03:08.000000 slackker-1.0.1/slackker/utils/checkker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-01-31 18:03:08.000000 slackker-1.0.1/slackker/utils/funckker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:03:22.185468 slackker-1.0.1/slackker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-01-31 18:03:22.000000 slackker-1.0.1/slackker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-01-31 18:03:22.000000 slackker-1.0.1/slackker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 18:03:22.000000 slackker-1.0.1/slackker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-31 18:03:22.000000 slackker-1.0.1/slackker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-31 18:03:22.000000 slackker-1.0.1/slackker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:50:23.428047 slackker-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 11:50:12.000000 slackker-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-07-08 11:50:23.428047 slackker-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-07-08 11:50:12.000000 slackker-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 11:50:23.428047 slackker-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-08 11:50:12.000000 slackker-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:50:23.424047 slackker-1.1.0/slackker/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-08 11:50:12.000000 slackker-1.1.0/slackker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:50:23.424047 slackker-1.1.0/slackker/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:50:12.000000 slackker-1.1.0/slackker/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-07-08 11:50:12.000000 slackker-1.1.0/slackker/callbacks/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:50:23.428047 slackker-1.1.0/slackker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:50:12.000000 slackker-1.1.0/slackker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-08 11:50:12.000000 slackker-1.1.0/slackker/utils/ccolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-08 11:50:12.000000 slackker-1.1.0/slackker/utils/checkker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-08 11:50:12.000000 slackker-1.1.0/slackker/utils/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:50:23.424047 slackker-1.1.0/slackker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-07-08 11:50:23.000000 slackker-1.1.0/slackker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-08 11:50:23.000000 slackker-1.1.0/slackker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:50:23.000000 slackker-1.1.0/slackker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 11:50:23.000000 slackker-1.1.0/slackker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 11:50:23.000000 slackker-1.1.0/slackker.egg-info/top_level.txt
```

### Comparing `slackker-1.0.1/LICENSE` & `slackker-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slackker-1.0.1/PKG-INFO` & `slackker-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,35 @@
-Metadata-Version: 2.1
-Name: slackker
-Version: 1.0.1
-Summary: Python package for reporting your Model training status in realtime on slack channel.
-Home-page: https://github.com/siddheshgunjal/slackker
-Author: Siddhesh Gunjal
-Author-email: siddhu19@live.com
-License: Apache-2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Introducing slackker! :fire:
 
 ![PyPI](https://img.shields.io/pypi/v/slackker?color=blue&label=pip) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/slackker?color=orange) ![PyPI - License](https://img.shields.io/pypi/l/slackker?color=gr)
 
 
-`slackker` is a python package for monitoring your Keras training status in real-time on slack channel. It can send you update for your ML model training progress and send final report with graphs when the training finishes. So now you don't have to sit in front of the machine all the time. You can quickly go and grab coffee :coffee: downstairs or run some errands and still keep tracking the progress while on the move.
+`slackker` is a python package for monitoring your Keras training status in real-time on Slack & Telegram. It can send you update for your ML model training progress and send final report with graphs when the training finishes. So now you don't have to sit in front of the machine all the time. You can quickly go and grab coffee :coffee: downstairs or run some errands and still keep tracking the progress while on the move without loosing your peace of mind.
 
 ## Table of contents :notebook:
 
 * [Requirements](#requirements-clipboard)
 * [Installation](#installation-arrow_down)
 * [Getting started with slackker callbacks](#getting-started-with-slackker-callbacks)
   * [Setup Slack to work with slackker](#setup-slack-to-work-with-slackker)
+  * [Setup Telegram to work with slackker](#setup-slack-to-work-with-slackker)
   * [Using slackker callbacks with keras callbacks](#using-slackker-callbacks-with-keras-callbacks-method)
-  * [Create slackker object](#create-slackker-object)
+  * [Create slackker object for Slack](#create-slackker-object-for-slack)
+  * [Create slackker object for Telegram](#create-slackker-object-for-telegram)
   * [Call slackker object into callbacks during model.fit()](#call-slackker-object-into-callbacks-during-model-fit)
   * [Final code](#final-code)
 * [Support](#support-sparkles)
 * [Citation](#citation-page_facing_up)
 * [Maintainer](#maintainer-sunglasses)
 
 
 ## Requirements :clipboard:
 
 * `slackker` utilises [slack_sdk][slack-sdk]`>=3.19.0` for communicating with slack API.
-* To use the `slackker.callbacks` method in keras.callbackss [keras][keras]`>=2.0.0` is required.
+* To use the `slackker.callbacks.keras` [keras][keras]`>=2.0.0` is required.
 
 
 ## Installation :arrow_down:
 * Install slackker from [PyPi][py-pi] is recommended. slackker is compatible with `Python >= 3.6` and runs on Linux, MacOS X and Windows. 
 * Installing slackker in your environment is easy. Just use below pip command:
 
 ```bash
@@ -56,47 +40,76 @@
 ### Setup Slack to work with slackker
 * First create an [slack app][slack-app] from scratch in your workspace.
 * we must give below mentioned permissions for `slackker` to be able to send status update and report to your channel:
   * `chat:write`
   * `chat:write.public`
   * `files:read`
   * `files:write`
-* Now install the app to your workspace and copy our apps **Bot & OAuth Token**. it should be in following format:
+* Now install the app to your workspace and copy our apps **Bot & OAuth Token**. It should be in following format:
 ```
  xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb
- ```
- * For detailed step by step guide visit this article: [How to setup slackker][setup-slack]
- * Now go to slack and add this slack app to the channel where you wish to receive al the update. Now we are ready to use `slackker` in your training flow!:smiling_imp:
+```
+* For detailed step by step guide, visit this article: [How to setup Slackker with Slack][setup-slack]
+* Now go to slack and add this slack app to the channel where you wish to receive al the update. Now we are ready to use `slackker` in your training flow!:smiling_imp:
+
+### Setup Telegram to work with slackker
+* Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots)
+* Type `/newbot` to create a new bot
+* Give your bot a name & a username
+* Copy your new Telegram bot’s token. It should be in following format:
+```
+1234567890:AAAAA_A111BBBBBCCC2DD3eEe44f5GGGgGG
+```
+* For detailed step by step guide, visit this article: [How to setup Slackker with Telegram][setup-telegram]
 
 ### Using slackker callbacks with keras callbacks method
 Import `slackker.callbacks` with following line:
 ```python
-from slackker.callbacks import SLKerasUpdate
+from slackker.callbacks.keras import slackUpdate, telegramUpdate
 ```
-### Create slackker object
-create slackker object with `SLKerasUpdate`
+### Create slackker object for Slack
+create slackker object with `slackUpdate`
 ```python
-slack_update = SLKerasUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb",
+slack_update = slackUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed",
     channel="A04AAB77ABC",
-    modelName='SampleModel',
+    modelName='Simple_NN',
     export='png',
     sendPlot=True,
     verbose=0)
 ```
-`SLKerasUpdate` takes following arguments:
+`slackUpdate` takes following arguments:
 * `token`: *(string)* Slack app token
 * `channel`: *(string)* Slack channel where you want to receive updates *(make sure you have added slack app to this same channel)*
 * `modelName`: *(string)* Name for your model. This same name will be used in future for title of the generated plots.
 * `export`: *(string)* default `"png"`: Format for plots to be exported. *(supported formats: eps, jpeg, jpg, pdf, pgf, png, ps, raw, rgba, svg, svgz, tif, tiff)*
 * `sendPlots`: *(Bool)* default `True`: If set to `True` it will export history of model, both training and validation, save it in the format given in `export` argument and send graphs to slack channel when training ends. If set to `False` it will not send exported graphs to slack channel. 
 * `verbose`: *(int)* default `0`: You can sent the verbose level up to 3.
   * `verbose = 0` No logging
   * `verbose = 1` Info logging
   * `verbose = 2` Debug/In-depth logging
 
+### Create slackker object for Telegram
+create slackker object with `telegramUpdate`
+```python
+telegram_update = telegramUpdate(token="1234567890:AAAAA_A111BBBBBCCC2DD3eEe44f5GGGgGG",
+    modelName='Simple_NN',
+    export='png',
+    sendPlot=True,
+    verbose=0)
+```
+`telegramUpdate` takes following arguments:
+* `token`: *(string)* Telegram bot token
+* `modelName`: *(string)* Name for your model. This same name will be used in future for title of the generated plots.
+* `export`: *(string)* default `"png"`: Format for plots to be exported. *(supported formats: eps, jpeg, jpg, pdf, pgf, png, ps, raw, rgba, svg, svgz, tif, tiff)*
+* `sendPlots`: *(Bool)* default `True`: If set to `True` it will export history of model, both training and validation, save it in the format given in `export` argument and send graphs to slack channel when training ends. If set to `False` it will not send exported graphs to slack channel. 
+* `verbose`: *(int)* default `0`: You can sent the verbose level up to 3.
+  * `verbose = 0` No logging
+  * `verbose = 1` Info logging
+  * `verbose = 2` Debug/In-depth logging
+
 ### Call slackker object into callbacks during model fit
 
 Now you can call slackker object into callbacks argument just like any other callbacks object.
 ```python
 history = model.fit(x_train, 
                     y_train,
                     epochs = 3,
@@ -105,28 +118,28 @@
                     validation_data=(x_val,y_val),
                     callbacks=[slack_update])
 ```
 
 ### Final code
 ```python
 # Import library for keras
-from slackker.callbacks import SLKerasUpdate
+from slackker.callbacks.keras import slackUpdate
 
 # Train-Test split for your keras model
 x_train, x_test, y_train, y_test = train_test_split(x, y, train_size=0.8)
 x_train, x_val, y_train, y_val = train_test_split(x_train, y_train, train_size=0.8)
 
 # Build keras model
 model = Sequential()
 model.add(Dense(8,activation='relu',input_shape = (IMG_WIDTH, IMG_HEIGHT, DEPTH)))
 model.add(Dense(3,activation='softmax'))
 model.compile(optimizer = 'rmsprop', loss='categorical_crossentropy', metrics=['accuracy'])
 
 # Create Slackker object
-slack_update = SLKerasUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb",
+slack_update = slackUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb",
     channel="A04AAB77ABC",
     modelName='SampleModel',
     export='png',
     sendPlot=True,
     verbose=0)
 
 # Call Slackker object in model.fit() callbacks
@@ -145,33 +158,35 @@
 * Use our [Github Issue Tracker][gh-issues] for reporting bugs or requesting features.
 Contribution are the best way to keep `slackker` amazing :muscle:
 * If you want to contribute please refer [Contributor's Guide][gh-contrib] for how to contribute in a helpful and collaborative way :innocent:
 
 #
 
 ## Citation :page_facing_up:
-Please cite slackker in your publications if this is useful for your research. Here is an example BibTeX entry:
+Please cite slackker in your publications if this is useful for your project/research. Here is an example BibTeX entry:
 ```BibTeX
 @misc{siddheshgunjal2023slackker,
   title={slackker},
   author={Siddhesh Gunjal},
   year={2023},
   howpublished={\url{https://github.com/siddheshgunjal/slackker}},
 }
 ```
 
 ## Maintainer :sunglasses:
 * Siddhesh Gunjal
-  * GitHub: [Siddhesh Gunjal](https://github.com/siddheshgunjal)
-  * LinkedIn: [LinkedIn](https://linkedin.com/in/siddheshgunjal)
+  * [Website][portfolio]
+  * [GitHub](https://github.com/siddheshgunjal)
+  * [LinkedIn](https://linkedin.com/in/siddheshgunjal)
 
 
 <!-- Markdown link -->
 [slack-sdk]: https://github.com/slackapi/python-slack-sdk
 [setup-slack]: https://medium.com/@siddheshgunjal82/how-to-setup-slackker-to-monitor-keras-model-training-status-on-slack-9f67265dfabd
+[setup-telegram]: https://medium.com/@siddheshgunjal82/how-to-setup-slackker-with-telegram-to-monitor-keras-model-training-21b1ff0c1020
 [matplot-lib]: https://github.com/matplotlib/matplotlib
 [keras]: https://github.com/keras-team/keras
 [py-pi]: https://pypi.org/
 [slack-app]: https://api.slack.com/apps
 [gh-issues]: https://github.com/siddheshgunjal/slackker/issues
 [gh-contrib]: https://github.com/siddheshgunjal/slackker/blob/main/CONTRIBUTING.md
-
+[portfolio]: https://siddheshgunjal.github.io/
```

### Comparing `slackker-1.0.1/README.md` & `slackker-1.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,59 @@
+Metadata-Version: 2.1
+Name: slackker
+Version: 1.1.0
+Summary: Python package for reporting your Model training status in realtime on slack & telegram.
+Home-page: https://github.com/siddheshgunjal/slackker
+Author: Siddhesh Gunjal
+Author-email: siddhu19@live.com
+License: Apache-2.0
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Introducing slackker! :fire:
 
 ![PyPI](https://img.shields.io/pypi/v/slackker?color=blue&label=pip) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/slackker?color=orange) ![PyPI - License](https://img.shields.io/pypi/l/slackker?color=gr)
 
 
-`slackker` is a python package for monitoring your Keras training status in real-time on slack channel. It can send you update for your ML model training progress and send final report with graphs when the training finishes. So now you don't have to sit in front of the machine all the time. You can quickly go and grab coffee :coffee: downstairs or run some errands and still keep tracking the progress while on the move.
+`slackker` is a python package for monitoring your Keras training status in real-time on Slack & Telegram. It can send you update for your ML model training progress and send final report with graphs when the training finishes. So now you don't have to sit in front of the machine all the time. You can quickly go and grab coffee :coffee: downstairs or run some errands and still keep tracking the progress while on the move without loosing your peace of mind.
 
 ## Table of contents :notebook:
 
 * [Requirements](#requirements-clipboard)
 * [Installation](#installation-arrow_down)
 * [Getting started with slackker callbacks](#getting-started-with-slackker-callbacks)
   * [Setup Slack to work with slackker](#setup-slack-to-work-with-slackker)
+  * [Setup Telegram to work with slackker](#setup-slack-to-work-with-slackker)
   * [Using slackker callbacks with keras callbacks](#using-slackker-callbacks-with-keras-callbacks-method)
-  * [Create slackker object](#create-slackker-object)
+  * [Create slackker object for Slack](#create-slackker-object-for-slack)
+  * [Create slackker object for Telegram](#create-slackker-object-for-telegram)
   * [Call slackker object into callbacks during model.fit()](#call-slackker-object-into-callbacks-during-model-fit)
   * [Final code](#final-code)
 * [Support](#support-sparkles)
 * [Citation](#citation-page_facing_up)
 * [Maintainer](#maintainer-sunglasses)
 
 
 ## Requirements :clipboard:
 
 * `slackker` utilises [slack_sdk][slack-sdk]`>=3.19.0` for communicating with slack API.
-* To use the `slackker.callbacks` method in keras.callbackss [keras][keras]`>=2.0.0` is required.
+* To use the `slackker.callbacks.keras` [keras][keras]`>=2.0.0` is required.
 
 
 ## Installation :arrow_down:
 * Install slackker from [PyPi][py-pi] is recommended. slackker is compatible with `Python >= 3.6` and runs on Linux, MacOS X and Windows. 
 * Installing slackker in your environment is easy. Just use below pip command:
 
 ```bash
@@ -38,47 +64,76 @@
 ### Setup Slack to work with slackker
 * First create an [slack app][slack-app] from scratch in your workspace.
 * we must give below mentioned permissions for `slackker` to be able to send status update and report to your channel:
   * `chat:write`
   * `chat:write.public`
   * `files:read`
   * `files:write`
-* Now install the app to your workspace and copy our apps **Bot & OAuth Token**. it should be in following format:
+* Now install the app to your workspace and copy our apps **Bot & OAuth Token**. It should be in following format:
 ```
  xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb
- ```
- * For detailed step by step guide visit this article: [How to setup slackker][setup-slack]
- * Now go to slack and add this slack app to the channel where you wish to receive al the update. Now we are ready to use `slackker` in your training flow!:smiling_imp:
+```
+* For detailed step by step guide, visit this article: [How to setup Slackker with Slack][setup-slack]
+* Now go to slack and add this slack app to the channel where you wish to receive al the update. Now we are ready to use `slackker` in your training flow!:smiling_imp:
+
+### Setup Telegram to work with slackker
+* Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots)
+* Type `/newbot` to create a new bot
+* Give your bot a name & a username
+* Copy your new Telegram bot’s token. It should be in following format:
+```
+1234567890:AAAAA_A111BBBBBCCC2DD3eEe44f5GGGgGG
+```
+* For detailed step by step guide, visit this article: [How to setup Slackker with Telegram][setup-telegram]
 
 ### Using slackker callbacks with keras callbacks method
 Import `slackker.callbacks` with following line:
 ```python
-from slackker.callbacks import SLKerasUpdate
+from slackker.callbacks.keras import slackUpdate, telegramUpdate
 ```
-### Create slackker object
-create slackker object with `SLKerasUpdate`
+### Create slackker object for Slack
+create slackker object with `slackUpdate`
 ```python
-slack_update = SLKerasUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb",
+slack_update = slackUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed",
     channel="A04AAB77ABC",
-    modelName='SampleModel',
+    modelName='Simple_NN',
     export='png',
     sendPlot=True,
     verbose=0)
 ```
-`SLKerasUpdate` takes following arguments:
+`slackUpdate` takes following arguments:
 * `token`: *(string)* Slack app token
 * `channel`: *(string)* Slack channel where you want to receive updates *(make sure you have added slack app to this same channel)*
 * `modelName`: *(string)* Name for your model. This same name will be used in future for title of the generated plots.
 * `export`: *(string)* default `"png"`: Format for plots to be exported. *(supported formats: eps, jpeg, jpg, pdf, pgf, png, ps, raw, rgba, svg, svgz, tif, tiff)*
 * `sendPlots`: *(Bool)* default `True`: If set to `True` it will export history of model, both training and validation, save it in the format given in `export` argument and send graphs to slack channel when training ends. If set to `False` it will not send exported graphs to slack channel. 
 * `verbose`: *(int)* default `0`: You can sent the verbose level up to 3.
   * `verbose = 0` No logging
   * `verbose = 1` Info logging
   * `verbose = 2` Debug/In-depth logging
 
+### Create slackker object for Telegram
+create slackker object with `telegramUpdate`
+```python
+telegram_update = telegramUpdate(token="1234567890:AAAAA_A111BBBBBCCC2DD3eEe44f5GGGgGG",
+    modelName='Simple_NN',
+    export='png',
+    sendPlot=True,
+    verbose=0)
+```
+`telegramUpdate` takes following arguments:
+* `token`: *(string)* Telegram bot token
+* `modelName`: *(string)* Name for your model. This same name will be used in future for title of the generated plots.
+* `export`: *(string)* default `"png"`: Format for plots to be exported. *(supported formats: eps, jpeg, jpg, pdf, pgf, png, ps, raw, rgba, svg, svgz, tif, tiff)*
+* `sendPlots`: *(Bool)* default `True`: If set to `True` it will export history of model, both training and validation, save it in the format given in `export` argument and send graphs to slack channel when training ends. If set to `False` it will not send exported graphs to slack channel. 
+* `verbose`: *(int)* default `0`: You can sent the verbose level up to 3.
+  * `verbose = 0` No logging
+  * `verbose = 1` Info logging
+  * `verbose = 2` Debug/In-depth logging
+
 ### Call slackker object into callbacks during model fit
 
 Now you can call slackker object into callbacks argument just like any other callbacks object.
 ```python
 history = model.fit(x_train, 
                     y_train,
                     epochs = 3,
@@ -87,28 +142,28 @@
                     validation_data=(x_val,y_val),
                     callbacks=[slack_update])
 ```
 
 ### Final code
 ```python
 # Import library for keras
-from slackker.callbacks import SLKerasUpdate
+from slackker.callbacks.keras import slackUpdate
 
 # Train-Test split for your keras model
 x_train, x_test, y_train, y_test = train_test_split(x, y, train_size=0.8)
 x_train, x_val, y_train, y_val = train_test_split(x_train, y_train, train_size=0.8)
 
 # Build keras model
 model = Sequential()
 model.add(Dense(8,activation='relu',input_shape = (IMG_WIDTH, IMG_HEIGHT, DEPTH)))
 model.add(Dense(3,activation='softmax'))
 model.compile(optimizer = 'rmsprop', loss='categorical_crossentropy', metrics=['accuracy'])
 
 # Create Slackker object
-slack_update = SLKerasUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb",
+slack_update = slackUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb",
     channel="A04AAB77ABC",
     modelName='SampleModel',
     export='png',
     sendPlot=True,
     verbose=0)
 
 # Call Slackker object in model.fit() callbacks
@@ -127,33 +182,35 @@
 * Use our [Github Issue Tracker][gh-issues] for reporting bugs or requesting features.
 Contribution are the best way to keep `slackker` amazing :muscle:
 * If you want to contribute please refer [Contributor's Guide][gh-contrib] for how to contribute in a helpful and collaborative way :innocent:
 
 #
 
 ## Citation :page_facing_up:
-Please cite slackker in your publications if this is useful for your research. Here is an example BibTeX entry:
+Please cite slackker in your publications if this is useful for your project/research. Here is an example BibTeX entry:
 ```BibTeX
 @misc{siddheshgunjal2023slackker,
   title={slackker},
   author={Siddhesh Gunjal},
   year={2023},
   howpublished={\url{https://github.com/siddheshgunjal/slackker}},
 }
 ```
 
 ## Maintainer :sunglasses:
 * Siddhesh Gunjal
-  * GitHub: [Siddhesh Gunjal](https://github.com/siddheshgunjal)
-  * LinkedIn: [LinkedIn](https://linkedin.com/in/siddheshgunjal)
+  * [Website][portfolio]
+  * [GitHub](https://github.com/siddheshgunjal)
+  * [LinkedIn](https://linkedin.com/in/siddheshgunjal)
 
 
 <!-- Markdown link -->
 [slack-sdk]: https://github.com/slackapi/python-slack-sdk
 [setup-slack]: https://medium.com/@siddheshgunjal82/how-to-setup-slackker-to-monitor-keras-model-training-status-on-slack-9f67265dfabd
+[setup-telegram]: https://medium.com/@siddheshgunjal82/how-to-setup-slackker-with-telegram-to-monitor-keras-model-training-21b1ff0c1020
 [matplot-lib]: https://github.com/matplotlib/matplotlib
 [keras]: https://github.com/keras-team/keras
 [py-pi]: https://pypi.org/
 [slack-app]: https://api.slack.com/apps
 [gh-issues]: https://github.com/siddheshgunjal/slackker/issues
 [gh-contrib]: https://github.com/siddheshgunjal/slackker/blob/main/CONTRIBUTING.md
-
+[portfolio]: https://siddheshgunjal.github.io/
```

### Comparing `slackker-1.0.1/setup.py` & `slackker-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,22 +20,28 @@
      install_requires=['slack_sdk>=3.19.0','numpy','matplotlib'],
      python_requires='>=3.5',
      name='slackker',
      version=new_version,
      license="Apache-2.0",
      author="Siddhesh Gunjal",
      author_email="siddhu19@live.com",
-     description="Python package for reporting your Model training status in realtime on slack channel.",
+     description="Python package for reporting your Model training status in realtime on slack & telegram.",
      long_description=read_file("README.md"),
      long_description_content_type="text/markdown",
      url="https://github.com/siddheshgunjal/slackker",
      packages=setuptools.find_packages(), # Searches throughout all dirs for files to include
      include_package_data=True, # Must be true to include files depicted in MANIFEST.in
      classifiers=[
-         "Programming Language :: Python :: 3",
+         "Programming Language :: Python :: 3.5",
+         "Programming Language :: Python :: 3.6",
+         "Programming Language :: Python :: 3.7",
+         "Programming Language :: Python :: 3.8",
+         "Programming Language :: Python :: 3.9",
+         "Programming Language :: Python :: 3.10",
+         "Programming Language :: Python :: 3.11",
          "License :: OSI Approved :: Apache Software License",
          "Operating System :: OS Independent",
          "Intended Audience :: Developers",
          "Intended Audience :: Information Technology",
          "Intended Audience :: Science/Research",
      ],
  )
```

### Comparing `slackker-1.0.1/slackker/utils/checkker.py` & `slackker-1.1.0/slackker/utils/checkker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,78 +1,94 @@
 import sys
 import time
+import requests
 import http.client as httplib
 from slack_sdk import WebClient
 from datetime import datetime, timezone
 from slackker.utils.ccolors import colors
 
 def _now():
     return datetime.utcnow().replace(tzinfo=timezone.utc)
 
 # Check whether server is still alive.
-def check_internet(url="www.slack.com", verbose=2):
+def check_internet(url, verbose=2):
     counter=1
     status=False
     sleepinsec=60
 
     while status is False:
         conn = httplib.HTTPConnection(url, timeout=5)
         try:
             conn.request("HEAD", "/")
             conn.close()
             status=True
             if verbose >= 2:
-                colors.prCyan(f"[slackker] {_now().strftime('%d-%m-%Y %H:%M')} Connection to slack Server successful!")
+                colors.prCyan(f"[slackker] {_now().strftime('%d-%m-%Y %H:%M')} Connection to '{url}' server successful!")
         except:
             status=False
-            colors.prYellow(f"[slackker] ERROR: {_now().strftime('%d-%m-%Y %H:%M')} Connection to Slack server failed. Trying again in 60 sec..[attempt {counter}]")
+            colors.prYellow(f"[slackker] ERROR: {_now().strftime('%d-%m-%Y %H:%M')} Connection to '{url}' server failed. Please check your internet. Trying again in 60 sec..[attempt {counter}]")
             time.sleep(sleepinsec)
             counter=counter+1
 
     if counter>1:
         if verbose>=2:
-        	colors.prCyan(f"[slackker] {_now().strftime('%d-%m-%Y %H:%M')} re-established connection to Slack server after {counter} attempts.")
+            colors.prCyan(f"[slackker] {_now().strftime('%d-%m-%Y %H:%M')} re-established connection to '{url}' server after {counter} attempts.")
 
     return status
 
 # Check whether server is still alive at the end of epoch if not skip the training. 
-def check_internet_epoch_end(url="www.slack.com"):
+def check_internet_epoch_end(url):
     counter=1
     status=False
     sleepinsec=10
 
     while status is False and counter <= 3:
         conn = httplib.HTTPConnection(url, timeout=5)
         try:
             conn.request("HEAD", "/")
             conn.close()
             status=True
         except:
             status=False
-            colors.prYellow(f"[slackker] ERROR: {_now().strftime('%d-%m-%Y %H:%M')} Connection to Slack server failed. Trying again in 10 sec..[attempt {counter}]")
+            colors.prYellow(f"[slackker] ERROR: {_now().strftime('%d-%m-%Y %H:%M')} Connection to '{url}' server failed. Trying again in 10 sec..[attempt {counter}]")
             time.sleep(sleepinsec)
             counter=counter+1
                 
     if counter <= 3 and counter > 1:
-        colors.prCyan(f"[slackker] {_now().strftime('%d-%m-%Y %H:%M')} re-established connection to Slack server after {counter} attempts.")
+        colors.prCyan(f"[slackker] {_now().strftime('%d-%m-%Y %H:%M')} re-established connection to '{url}' server after {counter} attempts.")
     elif counter > 3:
-        colors.prCyan(f'[slackker] Skipping report update to slack due to connection failure. {counter} attempts made before skipping')
+        colors.prCyan(f'[slackker] Skipping report update due to connection failure. {counter} attempts made before skipping')
 
     return status, counter
 
 
 def slack_connect(token, verbose=2):
+    status = False
 
-	status = False
+    try:
+        client = WebClient(token=token)
+        api_response = client.api_test()
+        status = True
+        if verbose >= 2:
+            colors.prCyan(f"[slackker] Connection to slack API successful! {api_response}")
+    except Exception as e:
+        status = False
+        colors.prRed(f"[slackker] ERROR: Invalid slack API token: {e}")
 
-	try:
-		client = WebClient(token=token)
-		api_response = client.api_test()
-		status = True
-		if verbose >= 2:
-			colors.prCyan(f"[slackker] Connection to slack API successful! {api_response}")
-
-	except Exception as e:
-		status = False
-		colors.prRed(f"[slackker] ERROR: Invalid slack API token: {e}")
+    return status
+
+def get_telegram_chat_id(token, verbose=2):
+    chat_id = False
+    url = f"https://api.telegram.org/bot{token}/getUpdates"
+
+    try:
+        firstMsg = requests.get(url).json()
+        chat_id = str(firstMsg["result"][0]["message"]["chat"]["id"])
+        if verbose >= 2:
+            colors.prCyan(f"[slackker] Connection to telegram API successful!")
+            colors.prCyan(f"[slackker] Found chat with 'chat_id'={chat_id}")
+    except Exception as e:
+        chat_id = False
+        colors.prRed(f"[slackker] ERROR: Could not connect to Telegram API: {e}")
+        colors.prYellow(f"[slackker] SUGGESTION: Please send 'Hello' once to your bot to make it discoverable to slackker")
 
-	return status
+    return chat_id
```

### Comparing `slackker-1.0.1/slackker.egg-info/PKG-INFO` & `slackker-1.1.0/slackker.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 Metadata-Version: 2.1
 Name: slackker
-Version: 1.0.1
-Summary: Python package for reporting your Model training status in realtime on slack channel.
+Version: 1.1.0
+Summary: Python package for reporting your Model training status in realtime on slack & telegram.
 Home-page: https://github.com/siddheshgunjal/slackker
 Author: Siddhesh Gunjal
 Author-email: siddhu19@live.com
 License: Apache-2.0
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Introducing slackker! :fire:
 
 ![PyPI](https://img.shields.io/pypi/v/slackker?color=blue&label=pip) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/slackker?color=orange) ![PyPI - License](https://img.shields.io/pypi/l/slackker?color=gr)
 
 
-`slackker` is a python package for monitoring your Keras training status in real-time on slack channel. It can send you update for your ML model training progress and send final report with graphs when the training finishes. So now you don't have to sit in front of the machine all the time. You can quickly go and grab coffee :coffee: downstairs or run some errands and still keep tracking the progress while on the move.
+`slackker` is a python package for monitoring your Keras training status in real-time on Slack & Telegram. It can send you update for your ML model training progress and send final report with graphs when the training finishes. So now you don't have to sit in front of the machine all the time. You can quickly go and grab coffee :coffee: downstairs or run some errands and still keep tracking the progress while on the move without loosing your peace of mind.
 
 ## Table of contents :notebook:
 
 * [Requirements](#requirements-clipboard)
 * [Installation](#installation-arrow_down)
 * [Getting started with slackker callbacks](#getting-started-with-slackker-callbacks)
   * [Setup Slack to work with slackker](#setup-slack-to-work-with-slackker)
+  * [Setup Telegram to work with slackker](#setup-slack-to-work-with-slackker)
   * [Using slackker callbacks with keras callbacks](#using-slackker-callbacks-with-keras-callbacks-method)
-  * [Create slackker object](#create-slackker-object)
+  * [Create slackker object for Slack](#create-slackker-object-for-slack)
+  * [Create slackker object for Telegram](#create-slackker-object-for-telegram)
   * [Call slackker object into callbacks during model.fit()](#call-slackker-object-into-callbacks-during-model-fit)
   * [Final code](#final-code)
 * [Support](#support-sparkles)
 * [Citation](#citation-page_facing_up)
 * [Maintainer](#maintainer-sunglasses)
 
 
 ## Requirements :clipboard:
 
 * `slackker` utilises [slack_sdk][slack-sdk]`>=3.19.0` for communicating with slack API.
-* To use the `slackker.callbacks` method in keras.callbackss [keras][keras]`>=2.0.0` is required.
+* To use the `slackker.callbacks.keras` [keras][keras]`>=2.0.0` is required.
 
 
 ## Installation :arrow_down:
 * Install slackker from [PyPi][py-pi] is recommended. slackker is compatible with `Python >= 3.6` and runs on Linux, MacOS X and Windows. 
 * Installing slackker in your environment is easy. Just use below pip command:
 
 ```bash
@@ -56,47 +64,76 @@
 ### Setup Slack to work with slackker
 * First create an [slack app][slack-app] from scratch in your workspace.
 * we must give below mentioned permissions for `slackker` to be able to send status update and report to your channel:
   * `chat:write`
   * `chat:write.public`
   * `files:read`
   * `files:write`
-* Now install the app to your workspace and copy our apps **Bot & OAuth Token**. it should be in following format:
+* Now install the app to your workspace and copy our apps **Bot & OAuth Token**. It should be in following format:
 ```
  xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb
- ```
- * For detailed step by step guide visit this article: [How to setup slackker][setup-slack]
- * Now go to slack and add this slack app to the channel where you wish to receive al the update. Now we are ready to use `slackker` in your training flow!:smiling_imp:
+```
+* For detailed step by step guide, visit this article: [How to setup Slackker with Slack][setup-slack]
+* Now go to slack and add this slack app to the channel where you wish to receive al the update. Now we are ready to use `slackker` in your training flow!:smiling_imp:
+
+### Setup Telegram to work with slackker
+* Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots)
+* Type `/newbot` to create a new bot
+* Give your bot a name & a username
+* Copy your new Telegram bot’s token. It should be in following format:
+```
+1234567890:AAAAA_A111BBBBBCCC2DD3eEe44f5GGGgGG
+```
+* For detailed step by step guide, visit this article: [How to setup Slackker with Telegram][setup-telegram]
 
 ### Using slackker callbacks with keras callbacks method
 Import `slackker.callbacks` with following line:
 ```python
-from slackker.callbacks import SLKerasUpdate
+from slackker.callbacks.keras import slackUpdate, telegramUpdate
 ```
-### Create slackker object
-create slackker object with `SLKerasUpdate`
+### Create slackker object for Slack
+create slackker object with `slackUpdate`
 ```python
-slack_update = SLKerasUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb",
+slack_update = slackUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed",
     channel="A04AAB77ABC",
-    modelName='SampleModel',
+    modelName='Simple_NN',
     export='png',
     sendPlot=True,
     verbose=0)
 ```
-`SLKerasUpdate` takes following arguments:
+`slackUpdate` takes following arguments:
 * `token`: *(string)* Slack app token
 * `channel`: *(string)* Slack channel where you want to receive updates *(make sure you have added slack app to this same channel)*
 * `modelName`: *(string)* Name for your model. This same name will be used in future for title of the generated plots.
 * `export`: *(string)* default `"png"`: Format for plots to be exported. *(supported formats: eps, jpeg, jpg, pdf, pgf, png, ps, raw, rgba, svg, svgz, tif, tiff)*
 * `sendPlots`: *(Bool)* default `True`: If set to `True` it will export history of model, both training and validation, save it in the format given in `export` argument and send graphs to slack channel when training ends. If set to `False` it will not send exported graphs to slack channel. 
 * `verbose`: *(int)* default `0`: You can sent the verbose level up to 3.
   * `verbose = 0` No logging
   * `verbose = 1` Info logging
   * `verbose = 2` Debug/In-depth logging
 
+### Create slackker object for Telegram
+create slackker object with `telegramUpdate`
+```python
+telegram_update = telegramUpdate(token="1234567890:AAAAA_A111BBBBBCCC2DD3eEe44f5GGGgGG",
+    modelName='Simple_NN',
+    export='png',
+    sendPlot=True,
+    verbose=0)
+```
+`telegramUpdate` takes following arguments:
+* `token`: *(string)* Telegram bot token
+* `modelName`: *(string)* Name for your model. This same name will be used in future for title of the generated plots.
+* `export`: *(string)* default `"png"`: Format for plots to be exported. *(supported formats: eps, jpeg, jpg, pdf, pgf, png, ps, raw, rgba, svg, svgz, tif, tiff)*
+* `sendPlots`: *(Bool)* default `True`: If set to `True` it will export history of model, both training and validation, save it in the format given in `export` argument and send graphs to slack channel when training ends. If set to `False` it will not send exported graphs to slack channel. 
+* `verbose`: *(int)* default `0`: You can sent the verbose level up to 3.
+  * `verbose = 0` No logging
+  * `verbose = 1` Info logging
+  * `verbose = 2` Debug/In-depth logging
+
 ### Call slackker object into callbacks during model fit
 
 Now you can call slackker object into callbacks argument just like any other callbacks object.
 ```python
 history = model.fit(x_train, 
                     y_train,
                     epochs = 3,
@@ -105,28 +142,28 @@
                     validation_data=(x_val,y_val),
                     callbacks=[slack_update])
 ```
 
 ### Final code
 ```python
 # Import library for keras
-from slackker.callbacks import SLKerasUpdate
+from slackker.callbacks.keras import slackUpdate
 
 # Train-Test split for your keras model
 x_train, x_test, y_train, y_test = train_test_split(x, y, train_size=0.8)
 x_train, x_val, y_train, y_val = train_test_split(x_train, y_train, train_size=0.8)
 
 # Build keras model
 model = Sequential()
 model.add(Dense(8,activation='relu',input_shape = (IMG_WIDTH, IMG_HEIGHT, DEPTH)))
 model.add(Dense(3,activation='softmax'))
 model.compile(optimizer = 'rmsprop', loss='categorical_crossentropy', metrics=['accuracy'])
 
 # Create Slackker object
-slack_update = SLKerasUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb",
+slack_update = slackUpdate(token="xoxb-123234234235-123234234235-adedce74748c3844747aed48499bb",
     channel="A04AAB77ABC",
     modelName='SampleModel',
     export='png',
     sendPlot=True,
     verbose=0)
 
 # Call Slackker object in model.fit() callbacks
@@ -145,33 +182,35 @@
 * Use our [Github Issue Tracker][gh-issues] for reporting bugs or requesting features.
 Contribution are the best way to keep `slackker` amazing :muscle:
 * If you want to contribute please refer [Contributor's Guide][gh-contrib] for how to contribute in a helpful and collaborative way :innocent:
 
 #
 
 ## Citation :page_facing_up:
-Please cite slackker in your publications if this is useful for your research. Here is an example BibTeX entry:
+Please cite slackker in your publications if this is useful for your project/research. Here is an example BibTeX entry:
 ```BibTeX
 @misc{siddheshgunjal2023slackker,
   title={slackker},
   author={Siddhesh Gunjal},
   year={2023},
   howpublished={\url{https://github.com/siddheshgunjal/slackker}},
 }
 ```
 
 ## Maintainer :sunglasses:
 * Siddhesh Gunjal
-  * GitHub: [Siddhesh Gunjal](https://github.com/siddheshgunjal)
-  * LinkedIn: [LinkedIn](https://linkedin.com/in/siddheshgunjal)
+  * [Website][portfolio]
+  * [GitHub](https://github.com/siddheshgunjal)
+  * [LinkedIn](https://linkedin.com/in/siddheshgunjal)
 
 
 <!-- Markdown link -->
 [slack-sdk]: https://github.com/slackapi/python-slack-sdk
 [setup-slack]: https://medium.com/@siddheshgunjal82/how-to-setup-slackker-to-monitor-keras-model-training-status-on-slack-9f67265dfabd
+[setup-telegram]: https://medium.com/@siddheshgunjal82/how-to-setup-slackker-with-telegram-to-monitor-keras-model-training-21b1ff0c1020
 [matplot-lib]: https://github.com/matplotlib/matplotlib
 [keras]: https://github.com/keras-team/keras
 [py-pi]: https://pypi.org/
 [slack-app]: https://api.slack.com/apps
 [gh-issues]: https://github.com/siddheshgunjal/slackker/issues
 [gh-contrib]: https://github.com/siddheshgunjal/slackker/blob/main/CONTRIBUTING.md
-
+[portfolio]: https://siddheshgunjal.github.io/
```

