# Comparing `tmp/localstack-2.1.1.dev20230621080533.tar.gz` & `tmp/localstack-2.1.1.dev20230708135750.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-2.1.1.dev20230621080533.tar", last modified: Wed Jun 21 08:09:17 2023, max compression
+gzip compressed data, was "localstack-2.1.1.dev20230708135750.tar", last modified: Sat Jul  8 14:01:04 2023, max compression
```

## Comparing `localstack-2.1.1.dev20230621080533.tar` & `localstack-2.1.1.dev20230708135750.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-21 08:09:17.408929 localstack-2.1.1.dev20230621080533/
--rw-rw-r--   0 runner    (1000) runner    (1001)    11394 2023-06-21 08:09:17.408929 localstack-2.1.1.dev20230621080533/PKG-INFO
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-21 08:09:17.408929 localstack-2.1.1.dev20230621080533/localstack.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)    11394 2023-06-21 08:09:17.000000 localstack-2.1.1.dev20230621080533/localstack.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-06-21 08:09:17.000000 localstack-2.1.1.dev20230621080533/localstack.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-06-21 08:09:17.000000 localstack-2.1.1.dev20230621080533/localstack.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)      223 2023-06-21 08:09:17.000000 localstack-2.1.1.dev20230621080533/localstack.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-06-21 08:09:17.000000 localstack-2.1.1.dev20230621080533/localstack.egg-info/top_level.txt
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-06-21 08:09:17.408929 localstack-2.1.1.dev20230621080533/localstack_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-06-21 08:09:16.000000 localstack-2.1.1.dev20230621080533/localstack_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-06-21 08:09:17.408929 localstack-2.1.1.dev20230621080533/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-06-21 08:05:16.000000 localstack-2.1.1.dev20230621080533/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-07-08 14:01:04.072934 localstack-2.1.1.dev20230708135750/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    12371 2023-07-08 14:01:04.072934 localstack-2.1.1.dev20230708135750/PKG-INFO
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-07-08 14:01:04.072934 localstack-2.1.1.dev20230708135750/localstack.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    12371 2023-07-08 14:01:04.000000 localstack-2.1.1.dev20230708135750/localstack.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-07-08 14:01:04.000000 localstack-2.1.1.dev20230708135750/localstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-07-08 14:01:04.000000 localstack-2.1.1.dev20230708135750/localstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)      223 2023-07-08 14:01:04.000000 localstack-2.1.1.dev20230708135750/localstack.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-07-08 14:01:04.000000 localstack-2.1.1.dev20230708135750/localstack.egg-info/top_level.txt
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-07-08 14:01:04.072934 localstack-2.1.1.dev20230708135750/localstack_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-07-08 14:01:03.000000 localstack-2.1.1.dev20230708135750/localstack_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-07-08 14:01:04.072934 localstack-2.1.1.dev20230708135750/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-07-08 13:57:36.000000 localstack-2.1.1.dev20230708135750/setup.py
```

### Comparing `localstack-2.1.1.dev20230621080533/PKG-INFO` & `localstack-2.1.1.dev20230708135750/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.1.1.dev20230621080533
+Version: 2.1.1.dev20230708135750
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -60,30 +60,44 @@
 
 [LocalStack](https://localstack.cloud) is a cloud service emulator that runs in a single container on your laptop or in your CI environment. With LocalStack, you can run your AWS applications or Lambdas entirely on your local machine without connecting to a remote cloud provider! Whether you are testing complex CDK applications or Terraform configurations, or just beginning to learn about AWS services, LocalStack helps speed up and simplify your testing and development workflow.
 
 LocalStack supports a growing number of AWS services, like AWS Lambda, S3, Dynamodb, Kinesis, SQS, SNS, and many more! The [Pro version of LocalStack](https://localstack.cloud/pricing) supports additional APIs and advanced features. You can find a comprehensive list of supported APIs on our [☑️ Feature Coverage](https://docs.localstack.cloud/user-guide/aws/feature-coverage/) page.
 
 LocalStack also provides additional features to make your life as a cloud developer easier! Check out LocalStack's [Cloud Developer Tools](https://docs.localstack.cloud/user-guide/tools/) for more information.
 
-## Requirements
+## Installation
+The quickest way get started with LocalStack is by using the LocalStack CLI.
+It allows you to start and manage the LocalStack Docker container from your command line.
+Please make sure that you have a working [`docker` environment](https://docs.docker.com/get-docker/) on your machine before moving on.
 
-* `python` (Python 3.7 up to 3.11 supported)
-* `pip` (Python package manager)
-* `Docker`
+### Brew (MacOS or Linux with Homebrew)
+Install the LocalStack CLI by using our [official LocalStack Brew Tap](https://github.com/localstack/homebrew-tap):
+```
+$ brew install localstack/tap/localstack-cli
+```
 
-## Installing
+### Binary download (MacOS, Linux, Windows)
+If you do not have Brew on your machine, you can directly download the pre-built LocalStack CLI binary for your system:
+- Download the latest release for your platform on [localstack/localstack-cli](https://github.com/localstack/localstack-cli/releases/latest).
+- Extract the archive to a folder in your `PATH` variable:
+  - MacOS / Linux: ```sudo tar xvzf ~/Downloads/localstack-cli-*-darwin-*-onefile.tar.gz -C /usr/local/bin```
+
+### Python package (MacOS, Linux, Windows)
+LocalStack is built with Python.
+You can directly install the LocalStack CLI in your Python environment using `pip`.
 
-The easiest way to install LocalStack is via `pip`:
+#### Prerequisites
 
+* `python` (Python 3.7 up to 3.11 supported)
+
+#### Installation
 ```
-pip install localstack
+python3 -m pip install localstack
 ```
 
-This installs the `localstack-cli` which is used to run the Docker image that hosts the LocalStack runtime.
-
 > **Important**: Do not use `sudo` or run as `root` user. LocalStack must be installed and started entirely under a local non-root user. If you have problems with permissions in macOS High Sierra, install with `pip install --user localstack`
 
 ## Example
 
 Start LocalStack inside a Docker container by running:
 
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.1.1.dev20230621080533
+Metadata-Version: 2.1 Name: localstack Version: 2.1.1.dev20230708135750
 Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
 github.com/localstack/localstack Author: LocalStack Contributors Author-email:
 info@localstack.cloud License: Apache License 2.0 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Testing Classifier: Topic :: System :: Emulators Description-
 Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
@@ -27,29 +27,42 @@
 number of AWS services, like AWS Lambda, S3, Dynamodb, Kinesis, SQS, SNS, and
 many more! The [Pro version of LocalStack](https://localstack.cloud/pricing)
 supports additional APIs and advanced features. You can find a comprehensive
 list of supported APIs on our [âï¸ Feature Coverage](https://
 docs.localstack.cloud/user-guide/aws/feature-coverage/) page. LocalStack also
 provides additional features to make your life as a cloud developer easier!
 Check out LocalStack's [Cloud Developer Tools](https://docs.localstack.cloud/
-user-guide/tools/) for more information. ## Requirements * `python` (Python 3.7
-up to 3.11 supported) * `pip` (Python package manager) * `Docker` ## Installing
-The easiest way to install LocalStack is via `pip`: ``` pip install localstack
-``` This installs the `localstack-cli` which is used to run the Docker image
-that hosts the LocalStack runtime. > **Important**: Do not use `sudo` or run as
-`root` user. LocalStack must be installed and started entirely under a local
-non-root user. If you have problems with permissions in macOS High Sierra,
-install with `pip install --user localstack` ## Example Start LocalStack inside
-a Docker container by running: ``` % localstack start -d __ _______ __ __ / /
-____ _________ _/ / ___// /_____ ______/ /__ / / / __ \/ ___/ __ `/ /\__ \/ __/
-__ `/ ___/ //_/ / /___/ /_/ / /__/ /_/ / /___/ / /_/ /_/ / /__/ ,< /_____/
-\____/\___/\__,_/_//____/\__/\__,_/\___/_/|_| ð» LocalStack CLI 2.0.0 [20:22:
-20] starting LocalStack in Docker mode ð³ [20:22:21] detaching ``` You can
-query the status of respective services on LocalStack by running: ``` %
-localstack status services
+user-guide/tools/) for more information. ## Installation The quickest way get
+started with LocalStack is by using the LocalStack CLI. It allows you to start
+and manage the LocalStack Docker container from your command line. Please make
+sure that you have a working [`docker` environment](https://docs.docker.com/
+get-docker/) on your machine before moving on. ### Brew (MacOS or Linux with
+Homebrew) Install the LocalStack CLI by using our [official LocalStack Brew
+Tap](https://github.com/localstack/homebrew-tap): ``` $ brew install
+localstack/tap/localstack-cli ``` ### Binary download (MacOS, Linux, Windows)
+If you do not have Brew on your machine, you can directly download the pre-
+built LocalStack CLI binary for your system: - Download the latest release for
+your platform on [localstack/localstack-cli](https://github.com/localstack/
+localstack-cli/releases/latest). - Extract the archive to a folder in your
+`PATH` variable: - MacOS / Linux: ```sudo tar xvzf ~/Downloads/localstack-cli-
+*-darwin-*-onefile.tar.gz -C /usr/local/bin``` ### Python package (MacOS,
+Linux, Windows) LocalStack is built with Python. You can directly install the
+LocalStack CLI in your Python environment using `pip`. #### Prerequisites *
+`python` (Python 3.7 up to 3.11 supported) #### Installation ``` python3 -m pip
+install localstack ``` > **Important**: Do not use `sudo` or run as `root`
+user. LocalStack must be installed and started entirely under a local non-root
+user. If you have problems with permissions in macOS High Sierra, install with
+`pip install --user localstack` ## Example Start LocalStack inside a Docker
+container by running: ``` % localstack start -d __ _______ __ __ / / ____
+_________ _/ / ___// /_____ ______/ /__ / / / __ \/ ___/ __ `/ /\__ \/ __/ __
+`/ ___/ //_/ / /___/ /_/ / /__/ /_/ / /___/ / /_/ /_/ / /__/ ,< /_____/\____/
+\___/\__,_/_//____/\__/\__,_/\___/_/|_| ð» LocalStack CLI 2.0.0 [20:22:20]
+starting LocalStack in Docker mode ð³ [20:22:21] detaching ``` You can query
+the status of respective services on LocalStack by running: ``` % localstack
+status services
 ââââââââââââââââââââââââââââ³ââââââââââââââ
 â Service â Status â
 â¡âââââââââââââââââââââââââââââââââââââââââ©
 â acm â â available â â apigateway â â available â â
 cloudformation â â available â â cloudwatch â â available â â
 config â â available â â dynamodb â â available â ... ``` To use
 SQS, a fully managed distributed message queuing service, on LocalStack, run:
```

### Comparing `localstack-2.1.1.dev20230621080533/localstack.egg-info/PKG-INFO` & `localstack-2.1.1.dev20230708135750/localstack.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.1.1.dev20230621080533
+Version: 2.1.1.dev20230708135750
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -60,30 +60,44 @@
 
 [LocalStack](https://localstack.cloud) is a cloud service emulator that runs in a single container on your laptop or in your CI environment. With LocalStack, you can run your AWS applications or Lambdas entirely on your local machine without connecting to a remote cloud provider! Whether you are testing complex CDK applications or Terraform configurations, or just beginning to learn about AWS services, LocalStack helps speed up and simplify your testing and development workflow.
 
 LocalStack supports a growing number of AWS services, like AWS Lambda, S3, Dynamodb, Kinesis, SQS, SNS, and many more! The [Pro version of LocalStack](https://localstack.cloud/pricing) supports additional APIs and advanced features. You can find a comprehensive list of supported APIs on our [☑️ Feature Coverage](https://docs.localstack.cloud/user-guide/aws/feature-coverage/) page.
 
 LocalStack also provides additional features to make your life as a cloud developer easier! Check out LocalStack's [Cloud Developer Tools](https://docs.localstack.cloud/user-guide/tools/) for more information.
 
-## Requirements
+## Installation
+The quickest way get started with LocalStack is by using the LocalStack CLI.
+It allows you to start and manage the LocalStack Docker container from your command line.
+Please make sure that you have a working [`docker` environment](https://docs.docker.com/get-docker/) on your machine before moving on.
 
-* `python` (Python 3.7 up to 3.11 supported)
-* `pip` (Python package manager)
-* `Docker`
+### Brew (MacOS or Linux with Homebrew)
+Install the LocalStack CLI by using our [official LocalStack Brew Tap](https://github.com/localstack/homebrew-tap):
+```
+$ brew install localstack/tap/localstack-cli
+```
 
-## Installing
+### Binary download (MacOS, Linux, Windows)
+If you do not have Brew on your machine, you can directly download the pre-built LocalStack CLI binary for your system:
+- Download the latest release for your platform on [localstack/localstack-cli](https://github.com/localstack/localstack-cli/releases/latest).
+- Extract the archive to a folder in your `PATH` variable:
+  - MacOS / Linux: ```sudo tar xvzf ~/Downloads/localstack-cli-*-darwin-*-onefile.tar.gz -C /usr/local/bin```
+
+### Python package (MacOS, Linux, Windows)
+LocalStack is built with Python.
+You can directly install the LocalStack CLI in your Python environment using `pip`.
 
-The easiest way to install LocalStack is via `pip`:
+#### Prerequisites
 
+* `python` (Python 3.7 up to 3.11 supported)
+
+#### Installation
 ```
-pip install localstack
+python3 -m pip install localstack
 ```
 
-This installs the `localstack-cli` which is used to run the Docker image that hosts the LocalStack runtime.
-
 > **Important**: Do not use `sudo` or run as `root` user. LocalStack must be installed and started entirely under a local non-root user. If you have problems with permissions in macOS High Sierra, install with `pip install --user localstack`
 
 ## Example
 
 Start LocalStack inside a Docker container by running:
 
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.1.1.dev20230621080533
+Metadata-Version: 2.1 Name: localstack Version: 2.1.1.dev20230708135750
 Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
 github.com/localstack/localstack Author: LocalStack Contributors Author-email:
 info@localstack.cloud License: Apache License 2.0 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Testing Classifier: Topic :: System :: Emulators Description-
 Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
@@ -27,29 +27,42 @@
 number of AWS services, like AWS Lambda, S3, Dynamodb, Kinesis, SQS, SNS, and
 many more! The [Pro version of LocalStack](https://localstack.cloud/pricing)
 supports additional APIs and advanced features. You can find a comprehensive
 list of supported APIs on our [âï¸ Feature Coverage](https://
 docs.localstack.cloud/user-guide/aws/feature-coverage/) page. LocalStack also
 provides additional features to make your life as a cloud developer easier!
 Check out LocalStack's [Cloud Developer Tools](https://docs.localstack.cloud/
-user-guide/tools/) for more information. ## Requirements * `python` (Python 3.7
-up to 3.11 supported) * `pip` (Python package manager) * `Docker` ## Installing
-The easiest way to install LocalStack is via `pip`: ``` pip install localstack
-``` This installs the `localstack-cli` which is used to run the Docker image
-that hosts the LocalStack runtime. > **Important**: Do not use `sudo` or run as
-`root` user. LocalStack must be installed and started entirely under a local
-non-root user. If you have problems with permissions in macOS High Sierra,
-install with `pip install --user localstack` ## Example Start LocalStack inside
-a Docker container by running: ``` % localstack start -d __ _______ __ __ / /
-____ _________ _/ / ___// /_____ ______/ /__ / / / __ \/ ___/ __ `/ /\__ \/ __/
-__ `/ ___/ //_/ / /___/ /_/ / /__/ /_/ / /___/ / /_/ /_/ / /__/ ,< /_____/
-\____/\___/\__,_/_//____/\__/\__,_/\___/_/|_| ð» LocalStack CLI 2.0.0 [20:22:
-20] starting LocalStack in Docker mode ð³ [20:22:21] detaching ``` You can
-query the status of respective services on LocalStack by running: ``` %
-localstack status services
+user-guide/tools/) for more information. ## Installation The quickest way get
+started with LocalStack is by using the LocalStack CLI. It allows you to start
+and manage the LocalStack Docker container from your command line. Please make
+sure that you have a working [`docker` environment](https://docs.docker.com/
+get-docker/) on your machine before moving on. ### Brew (MacOS or Linux with
+Homebrew) Install the LocalStack CLI by using our [official LocalStack Brew
+Tap](https://github.com/localstack/homebrew-tap): ``` $ brew install
+localstack/tap/localstack-cli ``` ### Binary download (MacOS, Linux, Windows)
+If you do not have Brew on your machine, you can directly download the pre-
+built LocalStack CLI binary for your system: - Download the latest release for
+your platform on [localstack/localstack-cli](https://github.com/localstack/
+localstack-cli/releases/latest). - Extract the archive to a folder in your
+`PATH` variable: - MacOS / Linux: ```sudo tar xvzf ~/Downloads/localstack-cli-
+*-darwin-*-onefile.tar.gz -C /usr/local/bin``` ### Python package (MacOS,
+Linux, Windows) LocalStack is built with Python. You can directly install the
+LocalStack CLI in your Python environment using `pip`. #### Prerequisites *
+`python` (Python 3.7 up to 3.11 supported) #### Installation ``` python3 -m pip
+install localstack ``` > **Important**: Do not use `sudo` or run as `root`
+user. LocalStack must be installed and started entirely under a local non-root
+user. If you have problems with permissions in macOS High Sierra, install with
+`pip install --user localstack` ## Example Start LocalStack inside a Docker
+container by running: ``` % localstack start -d __ _______ __ __ / / ____
+_________ _/ / ___// /_____ ______/ /__ / / / __ \/ ___/ __ `/ /\__ \/ __/ __
+`/ ___/ //_/ / /___/ /_/ / /__/ /_/ / /___/ / /_/ /_/ / /__/ ,< /_____/\____/
+\___/\__,_/_//____/\__/\__,_/\___/_/|_| ð» LocalStack CLI 2.0.0 [20:22:20]
+starting LocalStack in Docker mode ð³ [20:22:21] detaching ``` You can query
+the status of respective services on LocalStack by running: ``` % localstack
+status services
 ââââââââââââââââââââââââââââ³ââââââââââââââ
 â Service â Status â
 â¡âââââââââââââââââââââââââââââââââââââââââ©
 â acm â â available â â apigateway â â available â â
 cloudformation â â available â â cloudwatch â â available â â
 config â â available â â dynamodb â â available â ... ``` To use
 SQS, a fully managed distributed message queuing service, on LocalStack, run:
```

### Comparing `localstack-2.1.1.dev20230621080533/setup.py` & `localstack-2.1.1.dev20230708135750/setup.py`

 * *Files identical despite different names*

