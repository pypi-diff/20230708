# Comparing `tmp/adafruit-circuitpython-minimqtt-7.3.2.tar.gz` & `tmp/adafruit-circuitpython-minimqtt-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-minimqtt-7.3.2.tar", last modified: Mon Mar  6 16:22:23 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-minimqtt-7.4.0.tar", last modified: Sat Jul  8 14:23:05 2023, max compression
```

## Comparing `adafruit-circuitpython-minimqtt-7.3.2.tar` & `adafruit-circuitpython-minimqtt-7.4.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.839520 adafruit-circuitpython-minimqtt-7.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.823520 adafruit-circuitpython-minimqtt-7.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.827520 adafruit-circuitpython-minimqtt-7.3.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.831519 adafruit-circuitpython-minimqtt-7.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.831519 adafruit-circuitpython-minimqtt-7.3.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/LICENSES/EPL-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-03-06 16:22:23.839520 adafruit-circuitpython-minimqtt-7.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.831519 adafruit-circuitpython-minimqtt-7.3.2/adafruit_circuitpython_minimqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-03-06 16:22:23.000000 adafruit-circuitpython-minimqtt-7.3.2/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-06 16:22:23.000000 adafruit-circuitpython-minimqtt-7.3.2/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 16:22:23.000000 adafruit-circuitpython-minimqtt-7.3.2/adafruit_circuitpython_minimqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-06 16:22:23.000000 adafruit-circuitpython-minimqtt-7.3.2/adafruit_circuitpython_minimqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-06 16:22:23.000000 adafruit-circuitpython-minimqtt-7.3.2/adafruit_circuitpython_minimqtt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.831519 adafruit-circuitpython-minimqtt-7.3.2/adafruit_minimqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/adafruit_minimqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46003 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/adafruit_minimqtt/adafruit_minimqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/adafruit_minimqtt/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.835520 adafruit-circuitpython-minimqtt-7.3.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.835520 adafruit-circuitpython-minimqtt-7.3.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.835520 adafruit-circuitpython-minimqtt-7.3.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.835520 adafruit-circuitpython-minimqtt-7.3.2/examples/cellular/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3033 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/cellular/minimqtt_adafruitio_cellular.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/cellular/minimqtt_simpletest_cellular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.835520 adafruit-circuitpython-minimqtt-7.3.2/examples/cpython/
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/cpython/minimqtt_adafruitio_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/cpython/minimqtt_simpletest_cpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.835520 adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_adafruitio_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_certificate_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_simpletest_esp32spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.835520 adafruit-circuitpython-minimqtt-7.3.2/examples/ethernet/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2607 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/ethernet/minimqtt_adafruitio_eth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/ethernet/minimqtt_simpletest_eth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/minimqtt_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.835520 adafruit-circuitpython-minimqtt-7.3.2/examples/native_networking/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/native_networking/minimqtt_adafruitio_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 16:22:23.839520 adafruit-circuitpython-minimqtt-7.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:22:23.839520 adafruit-circuitpython-minimqtt-7.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/tests/backoff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-03-06 16:22:14.000000 adafruit-circuitpython-minimqtt-7.3.2/tests/test_port_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-06 16:21:59.000000 adafruit-circuitpython-minimqtt-7.3.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.232154 adafruit-circuitpython-minimqtt-7.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.236154 adafruit-circuitpython-minimqtt-7.4.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.236154 adafruit-circuitpython-minimqtt-7.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.236154 adafruit-circuitpython-minimqtt-7.4.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/LICENSES/EPL-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.240154 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-08 14:23:05.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-08 14:23:05.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:23:05.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 14:23:05.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-08 14:23:05.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.240154 adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45757 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/adafruit_minimqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.240154 adafruit-circuitpython-minimqtt-7.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.244154 adafruit-circuitpython-minimqtt-7.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.244154 adafruit-circuitpython-minimqtt-7.4.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.244154 adafruit-circuitpython-minimqtt-7.4.0/examples/cellular/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/cellular/minimqtt_adafruitio_cellular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/cellular/minimqtt_simpletest_cellular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.244154 adafruit-circuitpython-minimqtt-7.4.0/examples/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/cpython/minimqtt_adafruitio_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/cpython/minimqtt_simpletest_cpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_adafruitio_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_certificate_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_simpletest_esp32spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/examples/ethernet/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2608 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/ethernet/minimqtt_adafruitio_eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/ethernet/minimqtt_simpletest_eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/minimqtt_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_adafruitio_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:23:05.248154 adafruit-circuitpython-minimqtt-7.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/tests/backoff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-08 14:22:56.000000 adafruit-circuitpython-minimqtt-7.4.0/tests/test_port_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-08 14:22:47.000000 adafruit-circuitpython-minimqtt-7.4.0/tox.ini
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-minimqtt-7.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/.gitignore` & `adafruit-circuitpython-minimqtt-7.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/.pre-commit-config.yaml` & `adafruit-circuitpython-minimqtt-7.4.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/.pylintrc` & `adafruit-circuitpython-minimqtt-7.4.0/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -392,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-minimqtt-7.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/LICENSE` & `adafruit-circuitpython-minimqtt-7.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-minimqtt-7.4.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/LICENSES/EPL-1.0.txt` & `adafruit-circuitpython-minimqtt-7.4.0/LICENSES/EPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/LICENSES/MIT.txt` & `adafruit-circuitpython-minimqtt-7.4.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-minimqtt-7.4.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/PKG-INFO` & `adafruit-circuitpython-minimqtt-7.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-minimqtt
-Version: 7.3.2
+Version: 7.4.0
 Summary: MQTT client library for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT
 Keywords: adafruit,blinka,circuitpython,micropython,minimqtt,mqtt,,client,,socket
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/README.rst` & `adafruit-circuitpython-minimqtt-7.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO` & `adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-minimqtt
-Version: 7.3.2
+Version: 7.4.0
 Summary: MQTT client library for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT
 Keywords: adafruit,blinka,circuitpython,micropython,minimqtt,mqtt,,client,,socket
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt` & `adafruit-circuitpython-minimqtt-7.4.0/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/adafruit_minimqtt/adafruit_minimqtt.py` & `adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/adafruit_minimqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 except ImportError:
     pass
 
 from micropython import const
 
 from .matcher import MQTTMatcher
 
-__version__ = "7.3.2"
+__version__ = "7.4.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT.git"
 
 # Client-specific variables
 MQTT_MSG_MAX_SZ = const(268435455)
 MQTT_MSG_SZ_LIM = const(10000000)
 MQTT_TOPIC_LENGTH_LIMIT = const(65535)
 MQTT_TCP_PORT = const(1883)
@@ -187,15 +187,14 @@
         socket_pool=None,
         ssl_context=None,
         use_binary_mode: bool = False,
         socket_timeout: int = 1,
         connect_retries: int = 5,
         user_data=None,
     ) -> None:
-
         self._socket_pool = socket_pool
         self._ssl_context = ssl_context
         self._sock = None
         self._backwards_compatible_sock = False
         self._use_binary_mode = use_binary_mode
 
         if recv_timeout <= socket_timeout:
@@ -977,19 +976,18 @@
                 feed = subscribed_topics.pop()
                 self.subscribe(feed)
 
         return ret
 
     def loop(self, timeout: float = 0) -> Optional[list[int]]:
         # pylint: disable = too-many-return-statements
-        """Non-blocking message loop. Use this method to
-        check incoming subscription messages.
-        Returns response codes of any messages received.
+        """Non-blocking message loop. Use this method to check for incoming messages.
+        Returns list of response codes of any messages received or None.
 
-        :param float timeout: Socket timeout, in seconds.
+        :param float timeout: return after this timeout, in seconds.
 
         """
 
         self.logger.debug(f"waiting for messages for {timeout} seconds")
         if self._timestamp == 0:
             self._timestamp = time.monotonic()
         current_time = time.monotonic()
@@ -999,31 +997,27 @@
             self.logger.debug(
                 "KeepAlive period elapsed - requesting a PINGRESP from the server..."
             )
             rcs = self.ping()
             return rcs
 
         stamp = time.monotonic()
-        self._sock.settimeout(timeout)
         rcs = []
 
         while True:
-            rc = self._wait_for_msg(timeout)
-            if rc is None:
-                break
-            if time.monotonic() - stamp > self._recv_timeout:
-                self.logger.debug(
-                    f"Loop timed out, message queue not empty after {self._recv_timeout}s"
-                )
+            rc = self._wait_for_msg()
+            if rc is not None:
+                rcs.append(rc)
+            if time.monotonic() - stamp > timeout:
+                self.logger.debug(f"Loop timed out after {timeout} seconds")
                 break
-            rcs.append(rc)
 
         return rcs if rcs else None
 
-    def _wait_for_msg(self, timeout: float = 0.1) -> Optional[int]:
+    def _wait_for_msg(self) -> Optional[int]:
         # pylint: disable = too-many-return-statements
 
         """Reads and processes network events.
         Return the packet type or None if there is nothing to be received.
         """
         # CPython socket module contains a timeout attribute
         if hasattr(self._socket_pool, "timeout"):
@@ -1036,16 +1030,14 @@
                 res = self._sock_exact_recv(1)
             except OSError as error:
                 if error.errno in (errno.ETIMEDOUT, errno.EAGAIN):
                     # raised by a socket timeout if 0 bytes were present
                     return None
                 raise MMQTTException from error
 
-        # Block while we parse the rest of the response
-        self._sock.settimeout(timeout)
         if res in [None, b"", b"\x00"]:
             # If we get here, it means that there is nothing to be received
             return None
         if res[0] & MQTT_PKT_TYPE_MASK == MQTT_PINGRESP:
             self.logger.debug("Got PINGRESP")
             sz = self._sock_exact_recv(1)[0]
             if sz != 0x00:
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/adafruit_minimqtt/matcher.py` & `adafruit-circuitpython-minimqtt-7.4.0/adafruit_minimqtt/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,19 +66,18 @@
             parent, node = None, self._root
             for k in key.split("/"):
                 parent, node = node, node.children[k]
                 lst.append((parent, k, node))
             node.content = None
         except KeyError:
             raise KeyError(key) from None
-        else:  # cleanup
-            for parent, k, node in reversed(lst):
-                if node.children or node.content is not None:
-                    break
-                del parent.children[k]
+        for parent, k, node in reversed(lst):
+            if node.children or node.content is not None:
+                break
+            del parent.children[k]
 
     def iter_match(self, topic: str):
         """Return an iterator on all values associated with filters
         that match the :topic"""
         lst = topic.split("/")
         normal = not topic.startswith("$")
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/docs/_static/favicon.ico` & `adafruit-circuitpython-minimqtt-7.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/docs/conf.py` & `adafruit-circuitpython-minimqtt-7.4.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/docs/index.rst` & `adafruit-circuitpython-minimqtt-7.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/cellular/minimqtt_adafruitio_cellular.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/cellular/minimqtt_adafruitio_cellular.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 photocell_feed = secrets["aio_username"] + "/feeds/photocell"
 
 # Setup a feed named 'onoff' for subscribing to changes
 onoff_feed = secrets["aio_username"] + "/feeds/onoff"
 
 ### Code ###
 
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connected(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
     print("Connected to Adafruit IO! Listening for topic changes on %s" % onoff_feed)
     # Subscribe to all changes on the onoff_feed.
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/cellular/minimqtt_simpletest_cellular.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/cellular/minimqtt_simpletest_cellular.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 # Adafruit IO-style Topic
 # Use this topic if you'd like to connect to io.adafruit.com
 # mqtt_topic = 'aio_user/feeds/temperature'
 
 ### Code ###
 
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connect(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
     print("Connected to MQTT Broker!")
     print("Flags: {0}\n RC: {1}".format(flags, rc))
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/cpython/minimqtt_adafruitio_cpython.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/cpython/minimqtt_adafruitio_cpython.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 photocell_feed = secrets["aio_username"] + "/feeds/photocell"
 
 # Setup a feed named 'onoff' for subscribing to changes
 onoff_feed = secrets["aio_username"] + "/feeds/onoff"
 
 ### Code ###
 
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connected(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
     print("Connected to Adafruit IO! Listening for topic changes on %s" % onoff_feed)
     # Subscribe to all changes on the onoff_feed.
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/cpython/minimqtt_simpletest_cpython.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/cpython/minimqtt_simpletest_cpython.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # Use this topic if you'd like to connect to a standard MQTT broker
 mqtt_topic = "test/topic"
 
 # Adafruit IO-style Topic
 # Use this topic if you'd like to connect to io.adafruit.com
 # mqtt_topic = secrets["aio_username"] + "/feeds/temperature"
 
+
 ### Code ###
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connect(mqtt_client, userdata, flags, rc):
     # This function will be called when the mqtt_client is connected
     # successfully to the broker.
     print("Connected to MQTT Broker!")
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_adafruitio_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,73 +44,83 @@
 # from adafruit_esp32spi import PWMOut
 # RED_LED = PWMOut.PWMOut(esp, 26)
 # GREEN_LED = PWMOut.PWMOut(esp, 27)
 # BLUE_LED = PWMOut.PWMOut(esp, 25)
 # status_light = adafruit_rgbled.RGBLED(RED_LED, BLUE_LED, GREEN_LED)
 wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
-### Feeds ###
-
-# Setup a feed named 'photocell' for publishing to a feed
-photocell_feed = secrets["aio_username"] + "/feeds/photocell"
-
-# Setup a feed named 'onoff' for subscribing to changes
-onoff_feed = secrets["aio_username"] + "/feeds/onoff"
-
 ### Code ###
 
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connected(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
-    print("Connected to Adafruit IO! Listening for topic changes on %s" % onoff_feed)
-    # Subscribe to all changes on the onoff_feed.
-    client.subscribe(onoff_feed)
+    print("Connected to MQTT Broker!")
 
 
 def disconnected(client, userdata, rc):
     # This method is called when the client is disconnected
-    print("Disconnected from Adafruit IO!")
+    print("Disconnected from MQTT Broker!")
+
+
+def subscribe(client, userdata, topic, granted_qos):
+    # This method is called when the client subscribes to a new feed.
+    print("Subscribed to {0} with QOS level {1}".format(topic, granted_qos))
+
+
+def unsubscribe(client, userdata, topic, pid):
+    # This method is called when the client unsubscribes from a feed.
+    print("Unsubscribed from {0} with PID {1}".format(topic, pid))
 
 
-def message(client, topic, message):
-    # This method is called when a topic the client is subscribed to
-    # has a new message.
+def on_battery_msg(client, topic, message):
+    # Method called when device/batteryLife has a new value
+    print("Battery level: {}v".format(message))
+
+    # client.remove_topic_callback(secrets["aio_username"] + "/feeds/device.batterylevel")
+
+
+def on_message(client, topic, message):
+    # Method callled when a client's subscribed feed has a new value.
     print("New message on topic {0}: {1}".format(topic, message))
 
 
 # Connect to WiFi
 print("Connecting to WiFi...")
 wifi.connect()
 print("Connected!")
 
-# Initialize MQTT interface with the esp interface
 MQTT.set_socket(socket, esp)
 
 # Set up a MiniMQTT Client
-mqtt_client = MQTT.MQTT(
-    broker="io.adafruit.com",
-    username=secrets["aio_username"],
-    password=secrets["aio_key"],
-)
+client = MQTT.MQTT(broker=secrets["broker"], port=secrets["broker_port"])
 
 # Setup the callback methods above
-mqtt_client.on_connect = connected
-mqtt_client.on_disconnect = disconnected
-mqtt_client.on_message = message
+client.on_connect = connected
+client.on_disconnect = disconnected
+client.on_subscribe = subscribe
+client.on_unsubscribe = unsubscribe
+client.on_message = on_message
+client.add_topic_callback(
+    secrets["aio_username"] + "/feeds/device.batterylevel", on_battery_msg
+)
 
 # Connect the client to the MQTT broker.
-print("Connecting to Adafruit IO...")
-mqtt_client.connect()
+print("Connecting to MQTT broker...")
+client.connect()
 
-photocell_val = 0
-while True:
-    # Poll the message queue
-    mqtt_client.loop()
+# Subscribe to all notifications on the device group
+client.subscribe(secrets["aio_username"] + "/groups/device", 1)
 
-    # Send a new message
-    print("Sending photocell value: %d..." % photocell_val)
-    mqtt_client.publish(photocell_feed, photocell_val)
-    print("Sent!")
-    photocell_val += 1
-    time.sleep(5)
+# Start a blocking message loop...
+# NOTE: NO code below this loop will execute
+while True:
+    try:
+        client.loop()
+    except (ValueError, RuntimeError) as e:
+        print("Failed to get data, retrying\n", e)
+        wifi.reset()
+        client.reconnect()
+        continue
+    time.sleep(1)
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_certificate_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_certificate_esp32spi.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 
 # Adafruit IO-style Topic
 # Use this topic if you'd like to connect to io.adafruit.com
 # mqtt_topic = 'aio_user/feeds/temperature'
 
 ### Code ###
 
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connect(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
     print("Connected to MQTT Broker!")
     print("Flags: {0}\n RC: {1}".format(flags, rc))
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_simpletest_esp32spi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,115 +1,127 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
-
-import time
 import board
 import busio
 from digitalio import DigitalInOut
-import neopixel
 from adafruit_esp32spi import adafruit_esp32spi
-from adafruit_esp32spi import adafruit_esp32spi_wifimanager
 import adafruit_esp32spi.adafruit_esp32spi_socket as socket
-
 import adafruit_minimqtt.adafruit_minimqtt as MQTT
 
-### WiFi ###
-
-# Get wifi details and more from a secrets.py file
+# Add a secrets.py to your filesystem that has a dictionary called secrets with "ssid" and
+# "password" keys with your WiFi credentials. DO NOT share that file or commit it into Git or other
+# source control.
+# pylint: disable=no-name-in-module,wrong-import-order
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
+# Set your Adafruit IO Username and Key in secrets.py
+# (visit io.adafruit.com if you need to create an account,
+# or if you need your Adafruit IO key.)
+aio_username = secrets["aio_username"]
+aio_key = secrets["aio_key"]
+
 # If you are using a board with pre-defined ESP32 Pins:
 esp32_cs = DigitalInOut(board.ESP_CS)
 esp32_ready = DigitalInOut(board.ESP_BUSY)
 esp32_reset = DigitalInOut(board.ESP_RESET)
 
 # If you have an externally connected ESP32:
 # esp32_cs = DigitalInOut(board.D9)
 # esp32_ready = DigitalInOut(board.D10)
 # esp32_reset = DigitalInOut(board.D5)
 
 spi = busio.SPI(board.SCK, board.MOSI, board.MISO)
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
-"""Use below for Most Boards"""
-status_light = neopixel.NeoPixel(
-    board.NEOPIXEL, 1, brightness=0.2
-)  # Uncomment for Most Boards
-"""Uncomment below for ItsyBitsy M4"""
-# status_light = dotstar.DotStar(board.APA102_SCK, board.APA102_MOSI, 1, brightness=0.2)
-# Uncomment below for an externally defined RGB LED
-# import adafruit_rgbled
-# from adafruit_esp32spi import PWMOut
-# RED_LED = PWMOut.PWMOut(esp, 26)
-# GREEN_LED = PWMOut.PWMOut(esp, 27)
-# BLUE_LED = PWMOut.PWMOut(esp, 25)
-# status_light = adafruit_rgbled.RGBLED(RED_LED, BLUE_LED, GREEN_LED)
-wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
-### Adafruit IO Setup ###
+print("Connecting to AP...")
+while not esp.is_connected:
+    try:
+        esp.connect_AP(secrets["ssid"], secrets["password"])
+    except RuntimeError as e:
+        print("could not connect to AP, retrying: ", e)
+        continue
+print("Connected to", str(esp.ssid, "utf-8"), "\tRSSI:", esp.rssi)
 
-# Setup a feed named `testfeed` for publishing.
-default_topic = secrets["user"] + "/feeds/testfeed"
+### Topic Setup ###
+
+# MQTT Topic
+# Use this topic if you'd like to connect to a standard MQTT broker
+mqtt_topic = "test/topic"
+
+# Adafruit IO-style Topic
+# Use this topic if you'd like to connect to io.adafruit.com
+# mqtt_topic = secrets["aio_username"] + '/feeds/temperature'
 
 ### Code ###
 
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
-def connected(client, userdata, flags, rc):
-    # This function will be called when the client is connected
+def connect(mqtt_client, userdata, flags, rc):
+    # This function will be called when the mqtt_client is connected
     # successfully to the broker.
-    print("Connected to MQTT broker! Listening for topic changes on %s" % default_topic)
-    # Subscribe to all changes on the default_topic feed.
-    client.subscribe(default_topic)
+    print("Connected to MQTT Broker!")
+    print("Flags: {0}\n RC: {1}".format(flags, rc))
 
 
-def disconnected(client, userdata, rc):
-    # This method is called when the client is disconnected
+def disconnect(mqtt_client, userdata, rc):
+    # This method is called when the mqtt_client disconnects
+    # from the broker.
     print("Disconnected from MQTT Broker!")
 
 
+def subscribe(mqtt_client, userdata, topic, granted_qos):
+    # This method is called when the mqtt_client subscribes to a new feed.
+    print("Subscribed to {0} with QOS level {1}".format(topic, granted_qos))
+
+
+def unsubscribe(mqtt_client, userdata, topic, pid):
+    # This method is called when the mqtt_client unsubscribes from a feed.
+    print("Unsubscribed from {0} with PID {1}".format(topic, pid))
+
+
+def publish(mqtt_client, userdata, topic, pid):
+    # This method is called when the mqtt_client publishes data to a feed.
+    print("Published to {0} with PID {1}".format(topic, pid))
+
+
 def message(client, topic, message):
-    """Method callled when a client's subscribed feed has a new
-    value.
-    :param str topic: The topic of the feed with a new value.
-    :param str message: The new value
-    """
     print("New message on topic {0}: {1}".format(topic, message))
 
 
-# Connect to WiFi
-print("Connecting to WiFi...")
-wifi.connect()
-print("Connected!")
-
-# Initialize MQTT interface with the esp interface
+socket.set_interface(esp)
 MQTT.set_socket(socket, esp)
 
 # Set up a MiniMQTT Client
 mqtt_client = MQTT.MQTT(
-    broker=secrets["broker"], username=secrets["user"], password=secrets["pass"]
+    broker=secrets["broker"],
+    port=secrets["port"],
+    username=secrets["username"],
+    password=secrets["password"],
 )
 
-# Setup the callback methods above
-mqtt_client.on_connect = connected
-mqtt_client.on_disconnect = disconnected
+# Connect callback handlers to mqtt_client
+mqtt_client.on_connect = connect
+mqtt_client.on_disconnect = disconnect
+mqtt_client.on_subscribe = subscribe
+mqtt_client.on_unsubscribe = unsubscribe
+mqtt_client.on_publish = publish
 mqtt_client.on_message = message
 
-# Connect the client to the MQTT broker.
-print("Connecting to MQTT broker...")
+print("Attempting to connect to %s" % mqtt_client.broker)
 mqtt_client.connect()
 
-# Start a blocking message loop...
-# NOTE: NO code below this loop will execute
-# NOTE: Network reconnection is handled within this loop
-while True:
-    try:
-        mqtt_client.loop()
-    except (ValueError, RuntimeError) as e:
-        print("Failed to get data, retrying\n", e)
-        wifi.reset()
-        mqtt_client.reconnect()
-        continue
-    time.sleep(1)
+print("Subscribing to %s" % mqtt_topic)
+mqtt_client.subscribe(mqtt_topic)
+
+print("Publishing to %s" % mqtt_topic)
+mqtt_client.publish(mqtt_topic, "Hello Broker!")
+
+print("Unsubscribing from %s" % mqtt_topic)
+mqtt_client.unsubscribe(mqtt_topic)
+
+print("Disconnecting from %s" % mqtt_client.broker)
+mqtt_client.disconnect()
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
+import os
 import time
 import board
 import busio
 from digitalio import DigitalInOut
 import neopixel
 from adafruit_esp32spi import adafruit_esp32spi
-from adafruit_esp32spi import adafruit_esp32spi_wifimanager
 import adafruit_esp32spi.adafruit_esp32spi_socket as socket
 
 import adafruit_minimqtt.adafruit_minimqtt as MQTT
 
-### WiFi ###
+# Add settings.toml to your filesystem CIRCUITPY_WIFI_SSID and CIRCUITPY_WIFI_PASSWORD keys
+# with your WiFi credentials. Add your Adafruit IO username and key as well.
+# DO NOT share that file or commit it into Git or other source control.
 
-# Get wifi details and more from a secrets.py file
-try:
-    from secrets import secrets
-except ImportError:
-    print("WiFi secrets are kept in secrets.py, please add them there!")
-    raise
+aio_username = os.getenv("aio_username")
+aio_key = os.getenv("aio_key")
 
 # If you are using a board with pre-defined ESP32 Pins:
 esp32_cs = DigitalInOut(board.ESP_CS)
 esp32_ready = DigitalInOut(board.ESP_BUSY)
 esp32_reset = DigitalInOut(board.ESP_RESET)
 
 # If you have an externally connected ESP32:
@@ -42,84 +40,70 @@
 # Uncomment below for an externally defined RGB LED
 # import adafruit_rgbled
 # from adafruit_esp32spi import PWMOut
 # RED_LED = PWMOut.PWMOut(esp, 26)
 # GREEN_LED = PWMOut.PWMOut(esp, 27)
 # BLUE_LED = PWMOut.PWMOut(esp, 25)
 # status_light = adafruit_rgbled.RGBLED(RED_LED, BLUE_LED, GREEN_LED)
-wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
-### Code ###
+### Adafruit IO Setup ###
+
+# Setup a feed named `testfeed` for publishing.
+default_topic = aio_username + "/feeds/testfeed"
 
+
+### Code ###
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connected(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
-    print("Connected to MQTT Broker!")
+    print(f"Connected to MQTT broker! Listening for topic changes on {default_topic}")
+    # Subscribe to all changes on the default_topic feed.
+    client.subscribe(default_topic)
 
 
 def disconnected(client, userdata, rc):
     # This method is called when the client is disconnected
     print("Disconnected from MQTT Broker!")
 
 
-def subscribe(client, userdata, topic, granted_qos):
-    # This method is called when the client subscribes to a new feed.
-    print("Subscribed to {0} with QOS level {1}".format(topic, granted_qos))
-
-
-def unsubscribe(client, userdata, topic, pid):
-    # This method is called when the client unsubscribes from a feed.
-    print("Unsubscribed from {0} with PID {1}".format(topic, pid))
-
-
-def on_battery_msg(client, topic, message):
-    # Method called when device/batteryLife has a new value
-    print("Battery level: {}v".format(message))
-
-    # client.remove_topic_callback(secrets["aio_username"] + "/feeds/device.batterylevel")
-
-
-def on_message(client, topic, message):
-    # Method callled when a client's subscribed feed has a new value.
-    print("New message on topic {0}: {1}".format(topic, message))
+def message(client, topic, message):
+    """Method callled when a client's subscribed feed has a new
+    value.
+    :param str topic: The topic of the feed with a new value.
+    :param str message: The new value
+    """
+    print(f"New message on topic {topic}: {message}")
 
 
 # Connect to WiFi
 print("Connecting to WiFi...")
-wifi.connect()
+esp.connect_AP(os.getenv("CIRCUITPY_WIFI_SSID"), os.getenv("CIRCUITPY_WIFI_PASSWORD"))
 print("Connected!")
 
+# Initialize MQTT interface with the esp interface
 MQTT.set_socket(socket, esp)
 
 # Set up a MiniMQTT Client
-client = MQTT.MQTT(broker=secrets["broker"], port=secrets["broker_port"])
+mqtt_client = MQTT.MQTT(
+    broker="io.adafruit.com", username=aio_username, password=aio_key
+)
 
 # Setup the callback methods above
-client.on_connect = connected
-client.on_disconnect = disconnected
-client.on_subscribe = subscribe
-client.on_unsubscribe = unsubscribe
-client.on_message = on_message
-client.add_topic_callback(
-    secrets["aio_username"] + "/feeds/device.batterylevel", on_battery_msg
-)
+mqtt_client.on_connect = connected
+mqtt_client.on_disconnect = disconnected
+mqtt_client.on_message = message
 
 # Connect the client to the MQTT broker.
-print("Connecting to MQTT broker...")
-client.connect()
-
-# Subscribe to all notifications on the device group
-client.subscribe(secrets["aio_username"] + "/groups/device", 1)
+mqtt_client.connect()
 
-# Start a blocking message loop...
-# NOTE: NO code below this loop will execute
+photocell_val = 0
 while True:
-    try:
-        client.loop()
-    except (ValueError, RuntimeError) as e:
-        print("Failed to get data, retrying\n", e)
-        wifi.reset()
-        client.reconnect()
-        continue
-    time.sleep(1)
+    # Poll the message queue
+    mqtt_client.loop()
+
+    # Send a new message
+    print(f"Sending photocell value: {photocell_val}")
+    mqtt_client.publish(default_topic, photocell_val)
+    photocell_val += 1
+    time.sleep(3)
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,39 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 import time
-import board
-import busio
-from digitalio import DigitalInOut
-import neopixel
-from adafruit_esp32spi import adafruit_esp32spi
-from adafruit_esp32spi import adafruit_esp32spi_wifimanager
 import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_pyportal
 
 import adafruit_minimqtt.adafruit_minimqtt as MQTT
 
+pyportal = adafruit_pyportal.PyPortal()
+
 ### WiFi ###
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
-# If you are using a board with pre-defined ESP32 Pins:
-esp32_cs = DigitalInOut(board.ESP_CS)
-esp32_ready = DigitalInOut(board.ESP_BUSY)
-esp32_reset = DigitalInOut(board.ESP_RESET)
-
-# If you have an externally connected ESP32:
-# esp32_cs = DigitalInOut(board.D9)
-# esp32_ready = DigitalInOut(board.D10)
-# esp32_reset = DigitalInOut(board.D5)
-
-spi = busio.SPI(board.SCK, board.MOSI, board.MISO)
-esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
-"""Use below for Most Boards"""
-status_light = neopixel.NeoPixel(
-    board.NEOPIXEL, 1, brightness=0.2
-)  # Uncomment for Most Boards
-"""Uncomment below for ItsyBitsy M4"""
-# status_light = dotstar.DotStar(board.APA102_SCK, board.APA102_MOSI, 1, brightness=0.2)
-# Uncomment below for an externally defined RGB LED
-# import adafruit_rgbled
-# from adafruit_esp32spi import PWMOut
-# RED_LED = PWMOut.PWMOut(esp, 26)
-# GREEN_LED = PWMOut.PWMOut(esp, 27)
-# BLUE_LED = PWMOut.PWMOut(esp, 25)
-# status_light = adafruit_rgbled.RGBLED(RED_LED, BLUE_LED, GREEN_LED)
-wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
-
-### Adafruit IO Setup ###
+# ------------- MQTT Topic Setup ------------- #
+mqtt_topic = "test/topic"
 
-# Setup a feed named `testfeed` for publishing.
-default_topic = secrets["user"] + "/feeds/testfeed"
 
 ### Code ###
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connected(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
-    print("Connected to MQTT broker! Listening for topic changes on %s" % default_topic)
-    # Subscribe to all changes on the default_topic feed.
-    client.subscribe(default_topic)
+    print("Subscribing to %s" % (mqtt_topic))
+    client.subscribe(mqtt_topic)
 
 
 def disconnected(client, userdata, rc):
     # This method is called when the client is disconnected
     print("Disconnected from MQTT Broker!")
 
 
@@ -76,23 +44,27 @@
     :param str message: The new value
     """
     print("New message on topic {0}: {1}".format(topic, message))
 
 
 # Connect to WiFi
 print("Connecting to WiFi...")
-wifi.connect()
+pyportal.network.connect()
 print("Connected!")
 
 # Initialize MQTT interface with the esp interface
-MQTT.set_socket(socket, esp)
+# pylint: disable=protected-access
+MQTT.set_socket(socket, pyportal.network._wifi.esp)
 
 # Set up a MiniMQTT Client
 mqtt_client = MQTT.MQTT(
-    broker=secrets["broker"], username=secrets["user"], password=secrets["pass"]
+    broker=secrets["broker"],
+    username=secrets["user"],
+    password=secrets["pass"],
+    is_ssl=False,
 )
 
 # Setup the callback methods above
 mqtt_client.on_connect = connected
 mqtt_client.on_disconnect = disconnected
 mqtt_client.on_message = message
 
@@ -102,10 +74,10 @@
 photocell_val = 0
 while True:
     # Poll the message queue
     mqtt_client.loop()
 
     # Send a new message
     print("Sending photocell value: %d" % photocell_val)
-    mqtt_client.publish(default_topic, photocell_val)
+    mqtt_client.publish(mqtt_topic, photocell_val)
     photocell_val += 1
-    time.sleep(0.5)
+    time.sleep(1)
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/ethernet/minimqtt_simpletest_eth.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,99 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
-import time
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
-import adafruit_pyportal
+import board
+import busio
+from digitalio import DigitalInOut
+from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
+import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
 
 import adafruit_minimqtt.adafruit_minimqtt as MQTT
 
-pyportal = adafruit_pyportal.PyPortal()
-
-### WiFi ###
-
-# Get wifi details and more from a secrets.py file
+# Get MQTT details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
-    print("WiFi secrets are kept in secrets.py, please add them there!")
+    print("MQTT secrets are kept in secrets.py, please add them there!")
     raise
 
-# ------------- MQTT Topic Setup ------------- #
+cs = DigitalInOut(board.D10)
+spi_bus = busio.SPI(board.SCK, MOSI=board.MOSI, MISO=board.MISO)
+
+# Initialize ethernet interface with DHCP
+eth = WIZNET5K(spi_bus, cs)
+### Topic Setup ###
+
+# MQTT Topic
+# Use this topic if you'd like to connect to a standard MQTT broker
 mqtt_topic = "test/topic"
 
+# Adafruit IO-style Topic
+# Use this topic if you'd like to connect to io.adafruit.com
+# mqtt_topic = 'aio_user/feeds/temperature'
+
 ### Code ###
+
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
-def connected(client, userdata, flags, rc):
+def connect(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
-    print("Subscribing to %s" % (mqtt_topic))
-    client.subscribe(mqtt_topic)
+    print("Connected to MQTT Broker!")
+    print("Flags: {0}\n RC: {1}".format(flags, rc))
 
 
-def disconnected(client, userdata, rc):
-    # This method is called when the client is disconnected
+def disconnect(client, userdata, rc):
+    # This method is called when the client disconnects
+    # from the broker.
     print("Disconnected from MQTT Broker!")
 
 
-def message(client, topic, message):
-    """Method callled when a client's subscribed feed has a new
-    value.
-    :param str topic: The topic of the feed with a new value.
-    :param str message: The new value
-    """
-    print("New message on topic {0}: {1}".format(topic, message))
-
-
-# Connect to WiFi
-print("Connecting to WiFi...")
-pyportal.network.connect()
-print("Connected!")
-
-# Initialize MQTT interface with the esp interface
-# pylint: disable=protected-access
-MQTT.set_socket(socket, pyportal.network._wifi.esp)
+def subscribe(client, userdata, topic, granted_qos):
+    # This method is called when the client subscribes to a new feed.
+    print("Subscribed to {0} with QOS level {1}".format(topic, granted_qos))
+
+
+def unsubscribe(client, userdata, topic, pid):
+    # This method is called when the client unsubscribes from a feed.
+    print("Unsubscribed from {0} with PID {1}".format(topic, pid))
+
+
+def publish(client, userdata, topic, pid):
+    # This method is called when the client publishes data to a feed.
+    print("Published to {0} with PID {1}".format(topic, pid))
+
+
+# Initialize MQTT interface with the ethernet interface
+MQTT.set_socket(socket, eth)
 
 # Set up a MiniMQTT Client
-mqtt_client = MQTT.MQTT(
+# NOTE: We'll need to connect insecurely for ethernet configurations.
+client = MQTT.MQTT(
     broker=secrets["broker"],
     username=secrets["user"],
     password=secrets["pass"],
     is_ssl=False,
 )
 
-# Setup the callback methods above
-mqtt_client.on_connect = connected
-mqtt_client.on_disconnect = disconnected
-mqtt_client.on_message = message
-
-# Connect the client to the MQTT broker.
-mqtt_client.connect()
-
-photocell_val = 0
-while True:
-    # Poll the message queue
-    mqtt_client.loop()
-
-    # Send a new message
-    print("Sending photocell value: %d" % photocell_val)
-    mqtt_client.publish(mqtt_topic, photocell_val)
-    photocell_val += 1
-    time.sleep(1)
+# Connect callback handlers to client
+client.on_connect = connect
+client.on_disconnect = disconnect
+client.on_subscribe = subscribe
+client.on_unsubscribe = unsubscribe
+client.on_publish = publish
+
+print("Attempting to connect to %s" % client.broker)
+client.connect()
+
+print("Subscribing to %s" % mqtt_topic)
+client.subscribe(mqtt_topic)
+
+print("Publishing to %s" % mqtt_topic)
+client.publish(mqtt_topic, "Hello Broker!")
+
+print("Unsubscribing from %s" % mqtt_topic)
+client.unsubscribe(mqtt_topic)
+
+print("Disconnecting from %s" % client.broker)
+client.disconnect()
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/esp32spi/minimqtt_simpletest_esp32spi.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/minimqtt_simpletest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
+
+import os
 import board
 import busio
 from digitalio import DigitalInOut
 from adafruit_esp32spi import adafruit_esp32spi
 import adafruit_esp32spi.adafruit_esp32spi_socket as socket
 import adafruit_minimqtt.adafruit_minimqtt as MQTT
 
-# Add a secrets.py to your filesystem that has a dictionary called secrets with "ssid" and
-# "password" keys with your WiFi credentials. DO NOT share that file or commit it into Git or other
-# source control.
-# pylint: disable=no-name-in-module,wrong-import-order
-try:
-    from secrets import secrets
-except ImportError:
-    print("WiFi secrets are kept in secrets.py, please add them there!")
-    raise
-
-# Set your Adafruit IO Username and Key in secrets.py
-# (visit io.adafruit.com if you need to create an account,
-# or if you need your Adafruit IO key.)
-aio_username = secrets["aio_username"]
-aio_key = secrets["aio_key"]
+# Add settings.toml to your filesystem CIRCUITPY_WIFI_SSID and CIRCUITPY_WIFI_PASSWORD keys
+# with your WiFi credentials. Add your Adafruit IO username and key as well.
+# DO NOT share that file or commit it into Git or other source control.
+
+aio_username = os.getenv("aio_username")
+aio_key = os.getenv("aio_key")
 
 # If you are using a board with pre-defined ESP32 Pins:
 esp32_cs = DigitalInOut(board.ESP_CS)
 esp32_ready = DigitalInOut(board.ESP_BUSY)
 esp32_reset = DigitalInOut(board.ESP_RESET)
 
 # If you have an externally connected ESP32:
@@ -35,32 +28,36 @@
 
 spi = busio.SPI(board.SCK, board.MOSI, board.MISO)
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
 
 print("Connecting to AP...")
 while not esp.is_connected:
     try:
-        esp.connect_AP(secrets["ssid"], secrets["password"])
+        esp.connect_AP(
+            os.getenv("CIRCUITPY_WIFI_SSID"), os.getenv("CIRCUITPY_WIFI_PASSWORD")
+        )
     except RuntimeError as e:
         print("could not connect to AP, retrying: ", e)
         continue
 print("Connected to", str(esp.ssid, "utf-8"), "\tRSSI:", esp.rssi)
 
 ### Topic Setup ###
 
 # MQTT Topic
 # Use this topic if you'd like to connect to a standard MQTT broker
-mqtt_topic = "test/topic"
+# mqtt_topic = "test/topic"
 
 # Adafruit IO-style Topic
 # Use this topic if you'd like to connect to io.adafruit.com
-# mqtt_topic = secrets["aio_username"] + '/feeds/temperature'
+mqtt_topic = aio_username + "/feeds/temperature"
+
 
 ### Code ###
 
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connect(mqtt_client, userdata, flags, rc):
     # This function will be called when the mqtt_client is connected
     # successfully to the broker.
     print("Connected to MQTT Broker!")
     print("Flags: {0}\n RC: {1}".format(flags, rc))
@@ -92,18 +89,17 @@
 
 
 socket.set_interface(esp)
 MQTT.set_socket(socket, esp)
 
 # Set up a MiniMQTT Client
 mqtt_client = MQTT.MQTT(
-    broker=secrets["broker"],
-    port=secrets["port"],
-    username=secrets["username"],
-    password=secrets["password"],
+    broker="io.adafruit.com",
+    username=aio_username,
+    password=aio_key,
 )
 
 # Connect callback handlers to mqtt_client
 mqtt_client.on_connect = connect
 mqtt_client.on_disconnect = disconnect
 mqtt_client.on_subscribe = subscribe
 mqtt_client.on_unsubscribe = unsubscribe
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/ethernet/minimqtt_adafruitio_eth.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/ethernet/minimqtt_adafruitio_eth.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 photocell_feed = secrets["aio_username"] + "/feeds/photocell"
 
 # Setup a feed named 'onoff' for subscribing to changes
 onoff_feed = secrets["aio_username"] + "/feeds/onoff"
 
 ### Code ###
 
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connected(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
     print("Connected to Adafruit IO! Listening for topic changes on %s" % onoff_feed)
     # Subscribe to all changes on the onoff_feed.
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/native_networking/minimqtt_adafruitio_native_networking.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_adafruitio_native_networking.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,85 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
+import os
 import time
 import ssl
 import socketpool
 import wifi
 import adafruit_minimqtt.adafruit_minimqtt as MQTT
 
-# Add a secrets.py to your filesystem that has a dictionary called secrets with "ssid" and
-# "password" keys with your WiFi credentials. DO NOT share that file or commit it into Git or other
+# Add settings.toml to your filesystem CIRCUITPY_WIFI_SSID and CIRCUITPY_WIFI_PASSWORD keys
+# with your WiFi credentials. DO NOT share that file or commit it into Git or other
 # source control.
-# pylint: disable=no-name-in-module,wrong-import-order
-try:
-    from secrets import secrets
-except ImportError:
-    print("WiFi secrets are kept in secrets.py, please add them there!")
-    raise
 
-# Set your Adafruit IO Username and Key in secrets.py
+# Set your Adafruit IO Username, Key and Port in settings.toml
 # (visit io.adafruit.com if you need to create an account,
 # or if you need your Adafruit IO key.)
-aio_username = secrets["aio_username"]
-aio_key = secrets["aio_key"]
+aio_username = os.getenv("aio_username")
+aio_key = os.getenv("aio_key")
 
-print("Connecting to %s" % secrets["ssid"])
-wifi.radio.connect(secrets["ssid"], secrets["password"])
-print("Connected to %s!" % secrets["ssid"])
+print(f"Connecting to {os.getenv('CIRCUITPY_WIFI_SSID')}")
+wifi.radio.connect(
+    os.getenv("CIRCUITPY_WIFI_SSID"), os.getenv("CIRCUITPY_WIFI_PASSWORD")
+)
+print(f"Connected to {os.getenv('CIRCUITPY_WIFI_SSID')}!")
 ### Feeds ###
 
 # Setup a feed named 'photocell' for publishing to a feed
-photocell_feed = secrets["aio_username"] + "/feeds/photocell"
+photocell_feed = aio_username + "/feeds/photocell"
 
 # Setup a feed named 'onoff' for subscribing to changes
-onoff_feed = secrets["aio_username"] + "/feeds/onoff"
+onoff_feed = aio_username + "/feeds/onoff"
 
 ### Code ###
 
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connected(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
-    print("Connected to Adafruit IO! Listening for topic changes on %s" % onoff_feed)
+    print(f"Connected to Adafruit IO! Listening for topic changes on {onoff_feed}")
     # Subscribe to all changes on the onoff_feed.
     client.subscribe(onoff_feed)
 
 
 def disconnected(client, userdata, rc):
     # This method is called when the client is disconnected
     print("Disconnected from Adafruit IO!")
 
 
 def message(client, topic, message):
     # This method is called when a topic the client is subscribed to
     # has a new message.
-    print("New message on topic {0}: {1}".format(topic, message))
+    print(f"New message on topic {topic}: {message}")
 
 
 # Create a socket pool
 pool = socketpool.SocketPool(wifi.radio)
+ssl_context = ssl.create_default_context()
+
+# If you need to use certificate/key pair authentication (e.g. X.509), you can load them in the
+# ssl context by uncommenting the lines below and adding the following keys to the "secrets"
+# dictionary in your secrets.py file:
+# "device_cert_path" - Path to the Device Certificate
+# "device_key_path" - Path to the RSA Private Key
+# ssl_context.load_cert_chain(
+#     certfile=secrets["device_cert_path"], keyfile=secrets["device_key_path"]
+# )
 
 # Set up a MiniMQTT Client
 mqtt_client = MQTT.MQTT(
     broker="io.adafruit.com",
-    port=secrets["port"],
-    username=secrets["aio_username"],
-    password=secrets["aio_key"],
+    port=1883,
+    username=aio_username,
+    password=aio_key,
     socket_pool=pool,
-    ssl_context=ssl.create_default_context(),
+    ssl_context=ssl_context,
 )
 
 # Setup the callback methods above
 mqtt_client.on_connect = connected
 mqtt_client.on_disconnect = disconnected
 mqtt_client.on_message = message
 
@@ -81,12 +89,12 @@
 
 photocell_val = 0
 while True:
     # Poll the message queue
     mqtt_client.loop()
 
     # Send a new message
-    print("Sending photocell value: %d..." % photocell_val)
+    print(f"Sending photocell value: {photocell_val}...")
     mqtt_client.publish(photocell_feed, photocell_val)
     print("Sent!")
     photocell_val += 1
     time.sleep(5)
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
+import os
 import time
 import ssl
 import socketpool
 import wifi
 import adafruit_minimqtt.adafruit_minimqtt as MQTT
 
-# Add a secrets.py to your filesystem that has a dictionary called secrets with "ssid" and
-# "password" keys with your WiFi credentials. DO NOT share that file or commit it into Git or other
+# Add settings.toml to your filesystem CIRCUITPY_WIFI_SSID and CIRCUITPY_WIFI_PASSWORD keys
+# with your WiFi credentials. DO NOT share that file or commit it into Git or other
 # source control.
-# pylint: disable=no-name-in-module,wrong-import-order
-try:
-    from secrets import secrets
-except ImportError:
-    print("WiFi secrets are kept in secrets.py, please add them there!")
-    raise
 
-# Set your Adafruit IO Username and Key in secrets.py
+# Set your Adafruit IO Username, Key and Port in settings.toml
 # (visit io.adafruit.com if you need to create an account,
 # or if you need your Adafruit IO key.)
-aio_username = secrets["aio_username"]
-aio_key = secrets["aio_key"]
+aio_username = os.getenv("aio_username")
+aio_key = os.getenv("aio_key")
 
-print("Connecting to %s" % secrets["ssid"])
-wifi.radio.connect(secrets["ssid"], secrets["password"])
-print("Connected to %s!" % secrets["ssid"])
+print("Connecting to %s" % os.getenv("CIRCUITPY_WIFI_SSID"))
+wifi.radio.connect(
+    os.getenv("CIRCUITPY_WIFI_SSID"), os.getenv("CIRCUITPY_WIFI_PASSWORD")
+)
+print("Connected to %s!" % os.getenv("CIRCUITPY_WIFI_SSID"))
 
 ### Adafruit IO Setup ###
 
 # Setup a feed named `testfeed` for publishing.
-default_topic = secrets["aio_username"] + "/feeds/testfeed"
+default_topic = aio_username + "/feeds/testfeed"
+
 
 ### Code ###
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connected(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
-    print("Connected to MQTT broker! Listening for topic changes on %s" % default_topic)
+    print(f"Connected to MQTT broker! Listening for topic changes on {default_topic}")
     # Subscribe to all changes on the default_topic feed.
     client.subscribe(default_topic)
 
 
 def disconnected(client, userdata, rc):
     # This method is called when the client is disconnected
     print("Disconnected from MQTT Broker!")
@@ -50,28 +48,38 @@
 
 def message(client, topic, message):
     """Method callled when a client's subscribed feed has a new
     value.
     :param str topic: The topic of the feed with a new value.
     :param str message: The new value
     """
-    print("New message on topic {0}: {1}".format(topic, message))
+    print(f"New message on topic {topic}: {message}")
 
 
 # Create a socket pool
 pool = socketpool.SocketPool(wifi.radio)
+ssl_context = ssl.create_default_context()
+
+# If you need to use certificate/key pair authentication (e.g. X.509), you can load them in the
+# ssl context by uncommenting the lines below and adding the following keys to the "secrets"
+# dictionary in your secrets.py file:
+# "device_cert_path" - Path to the Device Certificate
+# "device_key_path" - Path to the RSA Private Key
+# ssl_context.load_cert_chain(
+#     certfile=secrets["device_cert_path"], keyfile=secrets["device_key_path"]
+# )
 
 # Set up a MiniMQTT Client
 mqtt_client = MQTT.MQTT(
-    broker=secrets["broker"],
-    port=secrets["port"],
-    username=secrets["aio_username"],
-    password=secrets["aio_key"],
+    broker="io.adafruit.com",
+    port=1883,
+    username=aio_username,
+    password=aio_key,
     socket_pool=pool,
-    ssl_context=ssl.create_default_context(),
+    ssl_context=ssl_context,
 )
 
 # Setup the callback methods above
 mqtt_client.on_connect = connected
 mqtt_client.on_disconnect = disconnected
 mqtt_client.on_message = message
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py` & `adafruit-circuitpython-minimqtt-7.4.0/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
+import os
 import time
 import ssl
 import socketpool
 import wifi
 import adafruit_minimqtt.adafruit_minimqtt as MQTT
 
-# Add a secrets.py to your filesystem that has a dictionary called secrets with "ssid" and
-# "password" keys with your WiFi credentials. DO NOT share that file or commit it into Git or other
+# Add settings.toml to your filesystem CIRCUITPY_WIFI_SSID and CIRCUITPY_WIFI_PASSWORD keys
+# with your WiFi credentials. DO NOT share that file or commit it into Git or other
 # source control.
-# pylint: disable=no-name-in-module,wrong-import-order
-try:
-    from secrets import secrets
-except ImportError:
-    print("WiFi secrets are kept in secrets.py, please add them there!")
-    raise
 
-# Set your Adafruit IO Username and Key in secrets.py
+# Set your Adafruit IO Username, Key and Port in settings.toml
 # (visit io.adafruit.com if you need to create an account,
 # or if you need your Adafruit IO key.)
-aio_username = secrets["aio_username"]
-aio_key = secrets["aio_key"]
+aio_username = os.getenv("aio_username")
+aio_key = os.getenv("aio_key")
 
-print("Connecting to %s" % secrets["ssid"])
-wifi.radio.connect(secrets["ssid"], secrets["password"])
-print("Connected to %s!" % secrets["ssid"])
+print("Connecting to %s" % os.getenv("CIRCUITPY_WIFI_SSID"))
+wifi.radio.connect(
+    os.getenv("CIRCUITPY_WIFI_SSID"), os.getenv("CIRCUITPY_WIFI_PASSWORD")
+)
+print("Connected to %s!" % os.getenv("CIRCUITPY_WIFI_SSID"))
 
 ### Code ###
 
+
 # Define callback methods which are called when events occur
 # pylint: disable=unused-argument, redefined-outer-name
 def connected(client, userdata, flags, rc):
     # This function will be called when the client is connected
     # successfully to the broker.
     print("Connected to MQTT Broker!")
 
@@ -52,51 +50,59 @@
     print("Unsubscribed from {0} with PID {1}".format(topic, pid))
 
 
 def on_battery_msg(client, topic, message):
     # Method called when device/batteryLife has a new value
     print("Battery level: {}v".format(message))
 
-    # client.remove_topic_callback(secrets["aio_username"] + "/feeds/device.batterylevel")
+    # client.remove_topic_callback(aio_username + "/feeds/device.batterylevel")
 
 
 def on_message(client, topic, message):
     # Method callled when a client's subscribed feed has a new value.
     print("New message on topic {0}: {1}".format(topic, message))
 
 
 # Create a socket pool
 pool = socketpool.SocketPool(wifi.radio)
+ssl_context = ssl.create_default_context()
+
+# If you need to use certificate/key pair authentication (e.g. X.509), you can load them in the
+# ssl context by uncommenting the lines below and adding the following keys to the "secrets"
+# dictionary in your secrets.py file:
+# "device_cert_path" - Path to the Device Certificate
+# "device_key_path" - Path to the RSA Private Key
+# ssl_context.load_cert_chain(
+#     certfile=secrets["device_cert_path"], keyfile=secrets["device_key_path"]
+# )
 
 # Set up a MiniMQTT Client
 client = MQTT.MQTT(
-    broker=secrets["broker"],
-    port=secrets["port"],
-    username=secrets["aio_username"],
-    password=secrets["aio_key"],
+    broker="io.adafruit.com",
+    port=1883,
+    username=aio_username,
+    password=aio_key,
     socket_pool=pool,
-    ssl_context=ssl.create_default_context(),
+    ssl_context=ssl_context,
 )
 
 # Setup the callback methods above
 client.on_connect = connected
 client.on_disconnect = disconnected
 client.on_subscribe = subscribe
 client.on_unsubscribe = unsubscribe
 client.on_message = on_message
-client.add_topic_callback(
-    secrets["aio_username"] + "/feeds/device.batterylevel", on_battery_msg
-)
+client.add_topic_callback(aio_username + "/feeds/device.batterylevel", on_battery_msg)
 
 # Connect the client to the MQTT broker.
 print("Connecting to MQTT broker...")
 client.connect()
 
 # Subscribe to all notifications on the device group
-client.subscribe(secrets["aio_username"] + "/groups/device", 1)
+client.subscribe(aio_username + "/groups/device", 1)
 
 # Start a blocking message loop...
 # NOTE: NO code below this loop will execute
 while True:
     try:
         client.loop()
     except (ValueError, RuntimeError) as e:
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/pyproject.toml` & `adafruit-circuitpython-minimqtt-7.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-minimqtt"
 description = "MQTT client library for CircuitPython"
-version = "7.3.2"
+version = "7.4.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/tests/backoff_test.py` & `adafruit-circuitpython-minimqtt-7.4.0/tests/backoff_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-minimqtt-7.3.2/tests/test_port_ssl.py` & `adafruit-circuitpython-minimqtt-7.4.0/tests/test_port_ssl.py`

 * *Files identical despite different names*

