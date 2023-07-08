# Comparing `tmp/succulent-0.2.3.tar.gz` & `tmp/succulent-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "succulent-0.2.3.tar", max compression
+gzip compressed data, was "succulent-0.2.4.tar", max compression
```

## Comparing `succulent-0.2.3.tar` & `succulent-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1094 2023-04-18 11:02:21.268343 succulent-0.2.3/LICENSE
--rw-r--r--   0        0        0      693 2023-06-09 08:05:28.302397 succulent-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7409 2023-06-09 07:49:54.909125 succulent-0.2.3/README.md
--rw-r--r--   0        0        0      113 2023-06-09 08:05:33.530717 succulent-0.2.3/succulent/__init__.py
--rw-r--r--   0        0        0     1716 2023-06-08 12:14:03.927866 succulent-0.2.3/succulent/api.py
--rw-r--r--   0        0        0      362 2023-05-24 09:55:47.296058 succulent-0.2.3/succulent/configuration.py
--rw-r--r--   0        0        0     4664 2023-06-09 07:59:43.240467 succulent-0.2.3/succulent/processing.py
--rw-r--r--   0        0        0     8099 1970-01-01 00:00:00.000000 succulent-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-08 09:11:45.421628 succulent-0.2.4/LICENSE
+-rw-r--r--   0        0        0     9336 2023-07-08 09:11:45.421628 succulent-0.2.4/README.md
+-rw-r--r--   0        0        0      704 2023-07-08 09:11:45.422628 succulent-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-08 09:11:45.422628 succulent-0.2.4/succulent/__init__.py
+-rw-r--r--   0        0        0     1669 2023-07-08 09:11:45.422628 succulent-0.2.4/succulent/api.py
+-rw-r--r--   0        0        0      349 2023-07-08 09:11:45.422628 succulent-0.2.4/succulent/configuration.py
+-rw-r--r--   0        0        0     4553 2023-07-08 09:11:45.422628 succulent-0.2.4/succulent/processing.py
+-rw-r--r--   0        0        0    10211 2023-07-08 09:11:51.856852 succulent-0.2.4/setup.py
+-rw-r--r--   0        0        0    10142 2023-07-08 09:11:51.857119 succulent-0.2.4/PKG-INFO
```

### Comparing `succulent-0.2.3/LICENSE` & `succulent-0.2.4/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Iztok Fister Jr.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Iztok Fister Jr.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `succulent-0.2.3/README.md` & `succulent-0.2.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,138 +1,163 @@
----
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
-
-<p align="center">
-  <img alt="logo" width="300" src=".github/images/logo.png">
-</p>
-
-
-# succulent - Collect POST requests easily
-
----
-![PyPI Version](https://img.shields.io/pypi/v/succulent.svg)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/succulent.svg)
-[![Downloads](https://pepy.tech/badge/succulent)](https://pepy.tech/project/succulent)
-![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/succulent?style=flat-square)
-[![GitHub license](https://img.shields.io/github/license/firefly-cpp/succulent.svg)](https://github.com/firefly-cpp/succulent/blob/master/LICENSE)
-![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/succulent.svg)
-[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Average time to resolve an issue")
-[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Percentage of issues still open")
-
-## About
-
-Sending sensor measurements, data, or GPS positions from embedded devices, microcontrollers, and [smartwatches](https://github.com/firefly-cpp/AST-Monitor) to the central server is sometimes complicated and tricky. Setting up the primary data collection scripts can be time-consuming (selecting a protocol, framework, API, testing it, etc.). Usually, scripts are written for a specific task; thus, they are not easily adaptive to other tasks. succulent is a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. The inspiration for the framework comes from the practical data collection challenges in [smart agriculture](https://github.com/firefly-cpp/smart-agriculture-datasets/tree/main/plant-monitoring-esp32). The main idea of the framework was to speed up the process of configuring different collected parameters and providing several useful functions for data transformations. The framework allows users to configure the whole endpoint for data collection in several minutes and thus not spend time on server-side scripts.
-
-## Detailed insights
-The current version includes (but is not limited to) the following functions:
-
-- Request URL generation for data collection
-- Data collection from POST requests
-- Storing data in different formats (CSV, JSON, SQLite, images)
-- Defining boundaries for collected data (min, max)
-
-## Installation
-
-### pip
-
-Install succulent with pip:
-
-```sh
-pip install succulent
-```
-### Alpine Linux
-
-To install succulent on Alpine Linux, please use:
-
-```sh
-$ apk add py3-succulent
-```
-
-## Container
-
-[Basic container for succulent](https://github.com/firefly-cpp/succulent-container)
-
-### Configuration
-Follow the instructions in the [configuration](##configuration) section to define the configuration file.
-
-### Installation
-Build the container using Docker:
-```bash
-docker build -t succulent-container .
-```
-
-Alternatively, you can use ``docker-compose``:
-```bash
-docker compose build
-```
-
-### Usage
-Run the container using Docker:
-```bash
-docker run -p 8080:8080 succulent-container
-```
-
-Alternatively, you can use ``docker-compose``:
-```bash
-docker compose up
-```
-
-## Usage
-
-### Example
-
-```python
-from succulent.api import SucculentAPI
-api = SucculentAPI(host='0.0.0.0', port=8080, config='configuration.yml', format='csv')
-api.start()
-```
-
-## Configuration
-In the root directory, create a file named `configuration.yml` and define the following:
-```yml
-data:
-  - name: # Measure name
-    min: # Minimum value (optional)
-    max: # Maximum value (optional)
-```
-
-To collect images, create a file named ``configuration.yml`` in the root directory and define the following:
-```yml
-data:
-  - key: # Key in POST request
-```
-
-## License
-
-This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.
-
-## Disclaimer
-
-This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
-
-## Contributors ✨
-
-Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<table>
-  <tbody>
-    <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lahovniktadej"><img src="https://avatars.githubusercontent.com/u/57890734?v=4?s=100" width="100px;" alt="Tadej Lahovnik"/><br /><sub><b>Tadej Lahovnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Alahovniktadej" title="Bug reports">🐛</a> <a href="#ideas-lahovniktadej" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/AyanDas348"><img src="https://avatars.githubusercontent.com/u/53610626?v=4?s=100" width="100px;" alt="Ayan Das"/><br /><sub><b>Ayan Das</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=firefly-cpp" title="Code">💻</a> <a href="#ideas-firefly-cpp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑‍🏫</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Acarlosal1015" title="Bug reports">🐛</a> <a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rhododendrom"><img src="https://avatars.githubusercontent.com/u/3198785?v=4?s=100" width="100px;" alt="rhododendrom"/><br /><sub><b>rhododendrom</b></sub></a><br /><a href="#design-rhododendrom" title="Design">🎨</a></td>
-    </tr>
-  </tbody>
-</table>
-
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-
-<!-- ALL-CONTRIBUTORS-LIST:END -->
-
-This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+---
+<p align="center">
+  <img alt="logo" width="300" src=".github/images/logo.png">
+</p>
+
+
+# succulent - Collect POST requests easily
+
+---
+![PyPI Version](https://img.shields.io/pypi/v/succulent.svg)
+[![Documentation Status](https://readthedocs.org/projects/succulent/badge/?version=latest)](https://succulent.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/succulent.svg)
+[![Downloads](https://pepy.tech/badge/succulent)](https://pepy.tech/project/succulent)
+![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/succulent?style=flat-square)
+[![GitHub license](https://img.shields.io/github/license/firefly-cpp/succulent.svg)](https://github.com/firefly-cpp/succulent/blob/master/LICENSE)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/succulent.svg)
+[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Average time to resolve an issue")
+[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Percentage of issues still open")
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+[![AUR package](https://img.shields.io/aur/version/python-succulent?color=blue&label=Arch%20Linux&logo=arch-linux)](https://aur.archlinux.org/packages/python-succulent)
+[![Fedora package](https://img.shields.io/fedora/v/python3-succulent?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-succulent)
+
+* **Documentation:** [https://succulent.readthedocs.io/en/latest/](https://succulent.readthedocs.io/en/latest/)
+* **Tested OS:** Windows, Ubuntu, Fedora, Alpine, Arch, macOS. **However, that does not mean it does not work on others**
+
+## About :information_source:
+
+Do you ever find it challenging and tricky to send sensor measurements :straight_ruler:, data :bar_chart:, or GPS positions from embedded devices :iphone:, microcontrollers, and [smartwatches](https://github.com/firefly-cpp/AST-Monitor) to a central server? :satellite: Setting up the primary data collection scripts can be a time-consuming :hourglass_flowing_sand: process, involving selecting a protocol, framework, API, and testing them out. Moreover, these scripts are often tailored for specific tasks, making them difficult to adapt to different scenarios.
+
+But fear not! Introducing succulent 🌵, a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. This framework draws inspiration from real-world data collection challenges in [smart agriculture](https://github.com/firefly-cpp/smart-agriculture-datasets/tree/main/plant-monitoring-esp32) :brain::herb:, specifically plant monitoring using ESP32 devices. The main goal behind succulent is to streamline the process of configuring various data parameters and provide a range of useful functions for data transformations. By leveraging succulent, you can set up your entire data collection endpoint within minutes, freeing you from the hassle of dealing with server-side scripts.:rocket::wrench:
+
+## Detailed Insights :mag:
+
+The current version of succulent comes packed with exciting features, including, but not limited to:
+
+- **Hassle-free generation of request URLs** for seamless data collection 🌐
+- **Effortless data retrieval** from POST requests 📥
+- **Versatile data storage options**, such as CSV, JSON, SQLite, and even images 🗂️📊🖼️
+- **Customizable boundaries for collected data**, allowing you to set minimum and maximum thresholds ⚙️
+
+With succulent, the process of collecting, managing, and preprocessing data becomes a breeze, empowering you to focus on what truly matters—gaining valuable insights from your embedded devices, microcontrollers, and smartwatches :watch:. So why waste precious time?:hourglass_flowing_sand: Dive into the world of succulent and unlock the true potential of your data! 💪:chart_with_upwards_trend:
+
+## Installation
+
+### pip
+
+Install succulent with pip:
+
+```sh
+pip install succulent
+```
+### Alpine Linux
+
+To install succulent on Alpine Linux, please use:
+
+```sh
+$ apk add py3-succulent
+```
+
+### Arch Linux
+
+To install succulent on Arch Linux, please use an [AUR helper](https://wiki.archlinux.org/title/AUR_helpers):
+
+```sh
+$ yay -Syyu python-succulent
+```
+
+### Fedora Linux
+
+To install succulent on Fedora, use:
+
+```sh
+$ dnf install python3-succulent
+```
+
+## Container
+
+[Basic container for succulent](https://github.com/firefly-cpp/succulent-container)
+
+### Configuration
+Follow the instructions in the [configuration](##configuration) section to define the configuration file.
+
+### Installation
+Build the container using Docker:
+```bash
+docker build -t succulent-container .
+```
+
+Alternatively, you can use ``docker-compose``:
+```bash
+docker compose build
+```
+
+### Usage
+Run the container using Docker:
+```bash
+docker run -p 8080:8080 succulent-container
+```
+
+Alternatively, you can use ``docker-compose``:
+```bash
+docker compose up
+```
+
+## Usage
+
+### Example
+
+```python
+from succulent.api import SucculentAPI
+api = SucculentAPI(host='0.0.0.0', port=8080, config='configuration.yml', format='csv')
+api.start()
+```
+
+## Configuration
+In the root directory, create a file named `configuration.yml` and define the following:
+```yml
+data:
+  - name: # Measure name
+    min: # Minimum value (optional)
+    max: # Maximum value (optional)
+```
+
+To collect images, create a file named ``configuration.yml`` in the root directory and define the following:
+```yml
+data:
+  - key: # Key in POST request
+```
+
+## License
+
+This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.
+
+## Disclaimer
+
+This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lahovniktadej"><img src="https://avatars.githubusercontent.com/u/57890734?v=4?s=100" width="100px;" alt="Tadej Lahovnik"/><br /><sub><b>Tadej Lahovnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Alahovniktadej" title="Bug reports">🐛</a> <a href="#ideas-lahovniktadej" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/AyanDas348"><img src="https://avatars.githubusercontent.com/u/53610626?v=4?s=100" width="100px;" alt="Ayan Das"/><br /><sub><b>Ayan Das</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=firefly-cpp" title="Code">💻</a> <a href="#ideas-firefly-cpp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑‍🏫</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Acarlosal1015" title="Bug reports">🐛</a> <a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rhododendrom"><img src="https://avatars.githubusercontent.com/u/3198785?v=4?s=100" width="100px;" alt="rhododendrom"/><br /><sub><b>rhododendrom</b></sub></a><br /><a href="#design-rhododendrom" title="Design">🎨</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/zala-lahovnik"><img src="https://avatars.githubusercontent.com/u/105444201?v=4?s=100" width="100px;" alt="Zala Lahovnik"/><br /><sub><b>Zala Lahovnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=zala-lahovnik" title="Documentation">📖</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

### Comparing `succulent-0.2.3/succulent/api.py` & `succulent-0.2.4/succulent/api.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from flask import Flask, jsonify, request
-from succulent.configuration import Configuration
-from succulent.processing import Processing
-from datetime import datetime
-
-class SucculentAPI:
-    def __init__(self, host, port, config, format='csv'):
-        self.host = host
-        self.port = port
-        self.format = format
-
-        # Configuration file
-        conf = Configuration(config)
-        self.config = conf.load_config()
-
-        # Initialise processing
-        self.processing = Processing(config=self.config, format=self.format)
-
-        # Initialise Flask
-        self.app = Flask(__name__)
-        self.app.add_url_rule('/measure', 'url', self.url, methods=['GET'])
-        self.app.add_url_rule('/measure', 'measure', self.measure, methods=['POST'])
-
-    def url(self):
-        # Generate URL
-        parameters = self.processing.parameters()
-
-        # Send response
-        return jsonify({'url': f'{self.host}:{self.port}/measure?{parameters}'}), 200
-
-    def measure(self):
-        try:
-            # Process request
-            self.processing.process(request)
-            
-            # Collect and store timestamp
-            timestamp = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            # You can store the timestamp in a database, file, or any other desired storage mechanism.
-            # Example: database.insert_timestamp(timestamp)
-        except ValueError as err:
-            # Invalid file type
-            return jsonify({'message': str(err)}), 400
-
-        # Send response
-        return jsonify({'message': 'Data stored', 'timestamp': timestamp}), 200
-
-    def start(self):
+from flask import Flask, jsonify, request
+from succulent.configuration import Configuration
+from succulent.processing import Processing
+from datetime import datetime
+
+class SucculentAPI:
+    def __init__(self, host, port, config, format='csv'):
+        self.host = host
+        self.port = port
+        self.format = format
+
+        # Configuration file
+        conf = Configuration(config)
+        self.config = conf.load_config()
+
+        # Initialise processing
+        self.processing = Processing(config=self.config, format=self.format)
+
+        # Initialise Flask
+        self.app = Flask(__name__)
+        self.app.add_url_rule('/measure', 'url', self.url, methods=['GET'])
+        self.app.add_url_rule('/measure', 'measure', self.measure, methods=['POST'])
+
+    def url(self):
+        # Generate URL
+        parameters = self.processing.parameters()
+
+        # Send response
+        return jsonify({'url': f'{self.host}:{self.port}/measure?{parameters}'}), 200
+
+    def measure(self):
+        try:
+            # Process request
+            self.processing.process(request)
+            
+            # Collect and store timestamp
+            timestamp = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+            # You can store the timestamp in a database, file, or any other desired storage mechanism.
+            # Example: database.insert_timestamp(timestamp)
+        except ValueError as err:
+            # Invalid file type
+            return jsonify({'message': str(err)}), 400
+
+        # Send response
+        return jsonify({'message': 'Data stored', 'timestamp': timestamp}), 200
+
+    def start(self):
         self.app.run(host=self.host, port=self.port)
```

### Comparing `succulent-0.2.3/succulent/processing.py` & `succulent-0.2.4/succulent/processing.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import os
-import sqlite3
-import inspect
-import pandas as pd
-from datetime import datetime
-
-class Processing:
-    def __init__(self, format, config, unittest=False):
-        # Validate format
-        if format not in ['csv', 'json', 'sqlite', 'image']:
-            raise ValueError(f'Invalid format: {format}')
-        
-        # Initialise attributes
-        index = 1 if unittest else 2
-        self.directory = os.path.join(os.path.dirname(os.path.abspath(inspect.stack()[index].filename)), 'data')
-        self.format = format
-
-        if format in ['csv', 'json', 'sqlite']:
-            self.columns = [configuration['name'] for configuration in config['data']]
-            self.boundaries = [{ 
-                configuration['name']: {
-                    key: configuration[key]
-                    for key in ['min', 'max']
-                    if key in configuration
-                }
-            } for configuration in config['data'] if configuration.get('min') is not None or configuration.get('max') is not None]
-            self.df = None  # Initialize df attribute
-
-        if format == 'image':
-            self.key = config['data'][0]['key']
-    
-    def parameters(self):
-        if self.format != 'image':
-            parameters = [f'{column}=' for column in self.columns]
-            parameters = '&'.join(parameters)
-        return parameters if self.format != 'image' else ''
-    
-    def boundary(self, value, boundary, column):
-        if 'min' in boundary and float(value) < float(boundary['min']):
-            raise ValueError(f'{column} ({value}) is lower than the specified minimum ({boundary["min"]}).')
-        if 'max' in boundary and float(value) > float(boundary['max']):
-            raise ValueError(f'{column} ({value}) is greater than the specified maximum ({boundary["max"]}).')
-        return value
-        
-    def process(self, req):
-        # Directory preparation
-        if not os.path.exists(self.directory):
-            os.makedirs(self.directory)
-
-        if self.format in ['csv', 'json', 'sqlite']:
-            # Define paths
-            path = os.path.join(
-                self.directory, f'data.{self.format}'
-            )
-
-            # Load existing data
-            if os.path.exists(path):
-                if self.format == 'csv':
-                    self.df = pd.read_csv(path, sep=',')
-                elif self.format == 'json':
-                    self.df = pd.read_json(path, orient='records')
-                elif self.format == 'sqlite':
-                    conn = sqlite3.connect(path)
-                    self.df = pd.read_sql_query('SELECT * FROM data', conn)
-                    conn.close()
-                else:
-                    raise ValueError(f'Invalid file type: {self.format}')
-            # Initialise new data
-            else:
-                self.df = pd.DataFrame(columns=self.columns)
-
-            # Parse data from request
-            data = {}
-            for column in self.columns:
-                # Request type
-                if req.is_json:
-                    value = req.json[column] if column in req.json else None
-                else:
-                    value = req.args.get(column, default=None)
-
-                # Boundary check
-                if column in [list(boundaries.keys())[0] for boundaries in self.boundaries]:
-                    index = [list(boundaries.keys())[0] for boundaries in self.boundaries].index(column)
-                    data[column] = self.boundary(value, self.boundaries[index][column], column)
-                else:
-                    data[column] = value
-
-            # Convert data to Series
-            data = pd.Series(data, index=self.columns)
-
-            # Merge data
-            self.df = pd.concat([self.df, data.to_frame().T], ignore_index=True)
-
-            # Store data to device
-            if self.format == 'csv':
-                self.df.to_csv(path, sep=',', index=False)
-            elif self.format == 'json':
-                self.df.to_json(path, orient='records', indent=4)
-            elif self.format == 'sqlite':
-                conn = sqlite3.connect(path)
-                self.df.to_sql('data', conn, if_exists='replace', index=False)
-                conn.close()
-        
-        if self.format == 'image':
-            # Retrieve image from request
-            file = req.files[self.key]
-
-            # Timestamp
-            timestamp = datetime.now().strftime('%Y-%m-%d_%H%M%S')
-
-            # Store image to device
+import os
+import sqlite3
+import inspect
+import pandas as pd
+from datetime import datetime
+
+class Processing:
+    def __init__(self, format, config, unittest=False):
+        # Validate format
+        if format not in ['csv', 'json', 'sqlite', 'image']:
+            raise ValueError(f'Invalid format: {format}')
+        
+        # Initialise attributes
+        index = 1 if unittest else 2
+        self.directory = os.path.join(os.path.dirname(os.path.abspath(inspect.stack()[index].filename)), 'data')
+        self.format = format
+
+        if format in ['csv', 'json', 'sqlite']:
+            self.columns = [configuration['name'] for configuration in config['data']]
+            self.boundaries = [{ 
+                configuration['name']: {
+                    key: configuration[key]
+                    for key in ['min', 'max']
+                    if key in configuration
+                }
+            } for configuration in config['data'] if configuration.get('min') is not None or configuration.get('max') is not None]
+            self.df = None  # Initialize df attribute
+
+        if format == 'image':
+            self.key = config['data'][0]['key']
+    
+    def parameters(self):
+        if self.format != 'image':
+            parameters = [f'{column}=' for column in self.columns]
+            parameters = '&'.join(parameters)
+        return parameters if self.format != 'image' else ''
+    
+    def boundary(self, value, boundary, column):
+        if 'min' in boundary and float(value) < float(boundary['min']):
+            raise ValueError(f'{column} ({value}) is lower than the specified minimum ({boundary["min"]}).')
+        if 'max' in boundary and float(value) > float(boundary['max']):
+            raise ValueError(f'{column} ({value}) is greater than the specified maximum ({boundary["max"]}).')
+        return value
+        
+    def process(self, req):
+        # Directory preparation
+        if not os.path.exists(self.directory):
+            os.makedirs(self.directory)
+
+        if self.format in ['csv', 'json', 'sqlite']:
+            # Define paths
+            path = os.path.join(
+                self.directory, f'data.{self.format}'
+            )
+
+            # Load existing data
+            if os.path.exists(path):
+                if self.format == 'csv':
+                    self.df = pd.read_csv(path, sep=',')
+                elif self.format == 'json':
+                    self.df = pd.read_json(path, orient='records')
+                elif self.format == 'sqlite':
+                    conn = sqlite3.connect(path)
+                    self.df = pd.read_sql_query('SELECT * FROM data', conn)
+                    conn.close()
+                else:
+                    raise ValueError(f'Invalid file type: {self.format}')
+            # Initialise new data
+            else:
+                self.df = pd.DataFrame(columns=self.columns)
+
+            # Parse data from request
+            data = {}
+            for column in self.columns:
+                # Request type
+                if req.is_json:
+                    value = req.json[column] if column in req.json else None
+                else:
+                    value = req.args.get(column, default=None)
+
+                # Boundary check
+                if column in [list(boundaries.keys())[0] for boundaries in self.boundaries]:
+                    index = [list(boundaries.keys())[0] for boundaries in self.boundaries].index(column)
+                    data[column] = self.boundary(value, self.boundaries[index][column], column)
+                else:
+                    data[column] = value
+
+            # Convert data to Series
+            data = pd.Series(data, index=self.columns)
+
+            # Merge data
+            self.df = pd.concat([self.df, data.to_frame().T], ignore_index=True)
+
+            # Store data to device
+            if self.format == 'csv':
+                self.df.to_csv(path, sep=',', index=False)
+            elif self.format == 'json':
+                self.df.to_json(path, orient='records', indent=4)
+            elif self.format == 'sqlite':
+                conn = sqlite3.connect(path)
+                self.df.to_sql('data', conn, if_exists='replace', index=False)
+                conn.close()
+        
+        if self.format == 'image':
+            # Retrieve image from request
+            file = req.files[self.key]
+
+            # Timestamp
+            timestamp = datetime.now().strftime('%Y-%m-%d_%H%M%S')
+
+            # Store image to device
             file.save(os.path.join(self.directory, f'{timestamp}_{file.filename}'))
```

### Comparing `succulent-0.2.3/PKG-INFO` & `succulent-0.2.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 Metadata-Version: 2.1
 Name: succulent
-Version: 0.2.3
+Version: 0.2.4
 Summary: Collect POST requests easily
 Home-page: https://github.com/firefly-cpp/succulent
 License: MIT
-Keywords: data collection,data science,sensor measurements
+Keywords: data collection,data science,sensor measurements,smart agriculture,smartwatch
 Author: Iztok Fister Jr.
 Author-email: iztok@iztok-jr-fister.eu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/firefly-cpp/succulent
 Description-Content-Type: text/markdown
 
 ---
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
-
 <p align="center">
   <img alt="logo" width="300" src=".github/images/logo.png">
 </p>
 
 
 # succulent - Collect POST requests easily
 
 ---
 ![PyPI Version](https://img.shields.io/pypi/v/succulent.svg)
+[![Documentation Status](https://readthedocs.org/projects/succulent/badge/?version=latest)](https://succulent.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/succulent.svg)
 [![Downloads](https://pepy.tech/badge/succulent)](https://pepy.tech/project/succulent)
 ![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/succulent?style=flat-square)
 [![GitHub license](https://img.shields.io/github/license/firefly-cpp/succulent.svg)](https://github.com/firefly-cpp/succulent/blob/master/LICENSE)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/succulent.svg)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Average time to resolve an issue")
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Percentage of issues still open")
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+[![AUR package](https://img.shields.io/aur/version/python-succulent?color=blue&label=Arch%20Linux&logo=arch-linux)](https://aur.archlinux.org/packages/python-succulent)
+[![Fedora package](https://img.shields.io/fedora/v/python3-succulent?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-succulent)
 
-## About
+* **Documentation:** [https://succulent.readthedocs.io/en/latest/](https://succulent.readthedocs.io/en/latest/)
+* **Tested OS:** Windows, Ubuntu, Fedora, Alpine, Arch, macOS. **However, that does not mean it does not work on others**
 
-Sending sensor measurements, data, or GPS positions from embedded devices, microcontrollers, and [smartwatches](https://github.com/firefly-cpp/AST-Monitor) to the central server is sometimes complicated and tricky. Setting up the primary data collection scripts can be time-consuming (selecting a protocol, framework, API, testing it, etc.). Usually, scripts are written for a specific task; thus, they are not easily adaptive to other tasks. succulent is a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. The inspiration for the framework comes from the practical data collection challenges in [smart agriculture](https://github.com/firefly-cpp/smart-agriculture-datasets/tree/main/plant-monitoring-esp32). The main idea of the framework was to speed up the process of configuring different collected parameters and providing several useful functions for data transformations. The framework allows users to configure the whole endpoint for data collection in several minutes and thus not spend time on server-side scripts.
+## About :information_source:
 
-## Detailed insights
-The current version includes (but is not limited to) the following functions:
+Do you ever find it challenging and tricky to send sensor measurements :straight_ruler:, data :bar_chart:, or GPS positions from embedded devices :iphone:, microcontrollers, and [smartwatches](https://github.com/firefly-cpp/AST-Monitor) to a central server? :satellite: Setting up the primary data collection scripts can be a time-consuming :hourglass_flowing_sand: process, involving selecting a protocol, framework, API, and testing them out. Moreover, these scripts are often tailored for specific tasks, making them difficult to adapt to different scenarios.
 
-- Request URL generation for data collection
-- Data collection from POST requests
-- Storing data in different formats (CSV, JSON, SQLite, images)
-- Defining boundaries for collected data (min, max)
+But fear not! Introducing succulent 🌵, a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. This framework draws inspiration from real-world data collection challenges in [smart agriculture](https://github.com/firefly-cpp/smart-agriculture-datasets/tree/main/plant-monitoring-esp32) :brain::herb:, specifically plant monitoring using ESP32 devices. The main goal behind succulent is to streamline the process of configuring various data parameters and provide a range of useful functions for data transformations. By leveraging succulent, you can set up your entire data collection endpoint within minutes, freeing you from the hassle of dealing with server-side scripts.:rocket::wrench:
+
+## Detailed Insights :mag:
+
+The current version of succulent comes packed with exciting features, including, but not limited to:
+
+- **Hassle-free generation of request URLs** for seamless data collection 🌐
+- **Effortless data retrieval** from POST requests 📥
+- **Versatile data storage options**, such as CSV, JSON, SQLite, and even images 🗂️📊🖼️
+- **Customizable boundaries for collected data**, allowing you to set minimum and maximum thresholds ⚙️
+
+With succulent, the process of collecting, managing, and preprocessing data becomes a breeze, empowering you to focus on what truly matters—gaining valuable insights from your embedded devices, microcontrollers, and smartwatches :watch:. So why waste precious time?:hourglass_flowing_sand: Dive into the world of succulent and unlock the true potential of your data! 💪:chart_with_upwards_trend:
 
 ## Installation
 
 ### pip
 
 Install succulent with pip:
 
@@ -67,14 +74,30 @@
 
 To install succulent on Alpine Linux, please use:
 
 ```sh
 $ apk add py3-succulent
 ```
 
+### Arch Linux
+
+To install succulent on Arch Linux, please use an [AUR helper](https://wiki.archlinux.org/title/AUR_helpers):
+
+```sh
+$ yay -Syyu python-succulent
+```
+
+### Fedora Linux
+
+To install succulent on Fedora, use:
+
+```sh
+$ dnf install python3-succulent
+```
+
 ## Container
 
 [Basic container for succulent](https://github.com/firefly-cpp/succulent-container)
 
 ### Configuration
 Follow the instructions in the [configuration](##configuration) section to define the configuration file.
 
@@ -144,14 +167,15 @@
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lahovniktadej"><img src="https://avatars.githubusercontent.com/u/57890734?v=4?s=100" width="100px;" alt="Tadej Lahovnik"/><br /><sub><b>Tadej Lahovnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Alahovniktadej" title="Bug reports">🐛</a> <a href="#ideas-lahovniktadej" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/AyanDas348"><img src="https://avatars.githubusercontent.com/u/53610626?v=4?s=100" width="100px;" alt="Ayan Das"/><br /><sub><b>Ayan Das</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=firefly-cpp" title="Code">💻</a> <a href="#ideas-firefly-cpp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑‍🏫</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Acarlosal1015" title="Bug reports">🐛</a> <a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/rhododendrom"><img src="https://avatars.githubusercontent.com/u/3198785?v=4?s=100" width="100px;" alt="rhododendrom"/><br /><sub><b>rhododendrom</b></sub></a><br /><a href="#design-rhododendrom" title="Design">🎨</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/zala-lahovnik"><img src="https://avatars.githubusercontent.com/u/105444201?v=4?s=100" width="100px;" alt="Zala Lahovnik"/><br /><sub><b>Zala Lahovnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=zala-lahovnik" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

