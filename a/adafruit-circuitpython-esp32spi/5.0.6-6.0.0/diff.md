# Comparing `tmp/adafruit-circuitpython-esp32spi-5.0.6.tar.gz` & `tmp/adafruit-circuitpython-esp32spi-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-esp32spi-5.0.6.tar", last modified: Thu Jun 22 17:43:49 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-esp32spi-6.0.0.tar", last modified: Sat Jul  8 14:17:03 2023, max compression
```

## Comparing `adafruit-circuitpython-esp32spi-5.0.6.tar` & `adafruit-circuitpython-esp32spi-6.0.0.tar`

### file list

```diff
@@ -1,72 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.102824 adafruit-circuitpython-esp32spi-5.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.106824 adafruit-circuitpython-esp32spi-5.0.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.106824 adafruit-circuitpython-esp32spi-5.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.106824 adafruit-circuitpython-esp32spi-5.0.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.106824 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-22 17:43:49.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-22 17:43:49.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:43:49.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-22 17:43:49.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 17:43:49.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.110825 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/PWMOut.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38983 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_socket.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13094 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_wsgiserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6293 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/digitalio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.114825 adafruit-circuitpython-esp32spi-5.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.114825 adafruit-circuitpython-esp32spi-5.0.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.114825 adafruit-circuitpython-esp32spi-5.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_ipconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_localtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_simpletest_rp2040.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_tcp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_udp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_wpa2ent_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_wpa2ent_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/examples/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/gpio/esp32spi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/gpio/gpio.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/examples/server/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8400 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/server/esp32spi_wsgiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/examples/server/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/server/static/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3862 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/server/static/led_color_picker_example.js
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.957063 adafruit-circuitpython-esp32spi-6.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.949062 adafruit-circuitpython-esp32spi-6.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.949062 adafruit-circuitpython-esp32spi-6.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.949062 adafruit-circuitpython-esp32spi-6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.953063 adafruit-circuitpython-esp32spi-6.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-08 14:17:03.957063 adafruit-circuitpython-esp32spi-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.953063 adafruit-circuitpython-esp32spi-6.0.0/adafruit_circuitpython_esp32spi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-08 14:17:03.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-08 14:17:03.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:17:03.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-08 14:17:03.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_circuitpython_esp32spi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-08 14:17:03.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.953063 adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/PWMOut.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38979 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/adafruit_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/adafruit_esp32spi_socket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13094 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/adafruit_esp32spi_wsgiserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6293 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/digitalio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.953063 adafruit-circuitpython-esp32spi-6.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.953063 adafruit-circuitpython-esp32spi-6.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.957063 adafruit-circuitpython-esp32spi-6.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_ipconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_localtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_simpletest_rp2040.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_tcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_udp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_wpa2ent_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_wpa2ent_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.957063 adafruit-circuitpython-esp32spi-6.0.0/examples/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/gpio/esp32spi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/gpio/gpio.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:17:03.957063 adafruit-circuitpython-esp32spi-6.0.0/examples/server/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/examples/server/esp32spi_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-08 14:16:55.000000 adafruit-circuitpython-esp32spi-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-08 14:16:45.000000 adafruit-circuitpython-esp32spi-6.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:17:03.957063 adafruit-circuitpython-esp32spi-6.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-esp32spi-6.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/.gitignore` & `adafruit-circuitpython-esp32spi-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/.pre-commit-config.yaml` & `adafruit-circuitpython-esp32spi-6.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/.pylintrc` & `adafruit-circuitpython-esp32spi-6.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-esp32spi-6.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/LICENSE` & `adafruit-circuitpython-esp32spi-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-esp32spi-6.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/LICENSES/MIT.txt` & `adafruit-circuitpython-esp32spi-6.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-esp32spi-6.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/PKG-INFO` & `adafruit-circuitpython-esp32spi-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 5.0.6
+Version: 6.0.0
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/README.rst` & `adafruit-circuitpython-esp32spi-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO` & `adafruit-circuitpython-esp32spi-6.0.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 5.0.6
+Version: 6.0.0
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt` & `adafruit-circuitpython-esp32spi-6.0.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -48,10 +48,8 @@
 examples/esp32spi_simpletest_rp2040.py
 examples/esp32spi_tcp_client.py
 examples/esp32spi_udp_client.py
 examples/esp32spi_wpa2ent_aio_post.py
 examples/esp32spi_wpa2ent_simpletest.py
 examples/gpio/esp32spi_gpio.py
 examples/gpio/gpio.md
-examples/server/esp32spi_wsgiserver.py
-examples/server/static/index.html
-examples/server/static/led_color_picker_example.js
+examples/server/esp32spi_wsgiserver.py
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/PWMOut.py` & `adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/PWMOut.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi.py` & `adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/adafruit_esp32spi.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import struct
 import time
 from micropython import const
 from adafruit_bus_device.spi_device import SPIDevice
 from digitalio import Direction
 
-__version__ = "5.0.6"
+__version__ = "6.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI.git"
 
 _SET_NET_CMD = const(0x10)
 _SET_PASSPHRASE_CMD = const(0x11)
 _SET_IP_CONFIG = const(0x14)
 _SET_DNS_CONFIG = const(0x15)
 _SET_HOSTNAME = const(0x16)
@@ -789,15 +789,15 @@
         resp = self._send_command_get_response(_AVAIL_DATA_TCP_CMD, self._socknum_ll)
         reply = struct.unpack("<H", resp[0])[0]
         if self._debug:
             print("ESPSocket: %d bytes available" % reply)
         return reply
 
     def socket_read(self, socket_num, size):
-        """Read up to 'size' bytes from the socket number. Returns a bytearray"""
+        """Read up to 'size' bytes from the socket number. Returns a bytes"""
         if self._debug:
             print(
                 "Reading %d bytes from ESP socket with status %d"
                 % (size, self.socket_status(socket_num))
             )
         self._socknum_ll[0][0] = socket_num
         resp = self._send_command_get_response(
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_socket.py` & `adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/adafruit_esp32spi_socket.py`

 * *Files 24% similar despite different names*

```diff
@@ -84,88 +84,23 @@
         if self._type is SOCK_DGRAM:
             conntype = _the_interface.UDP_MODE
         else:
             conntype = _the_interface.TCP_MODE
         _the_interface.socket_write(self._socknum, data, conn_mode=conntype)
         gc.collect()
 
-    def write(self, data):
-        """Sends data to the socket.
-        NOTE: This method is deprecated and will be removed.
-        """
-        self.send(data)
-
-    def readline(self, eol=b"\r\n"):
-        """Attempt to return as many bytes as we can up to but not including
-        end-of-line character (default is '\\r\\n')"""
-
-        # print("Socket readline")
-        stamp = time.monotonic()
-        while eol not in self._buffer:
-            # there's no line already in there, read some more
-            avail = self.available()
-            if avail:
-                self._buffer += _the_interface.socket_read(self._socknum, avail)
-            elif self._timeout > 0 and time.monotonic() - stamp > self._timeout:
-                self.close()  # Make sure to close socket so that we don't exhaust sockets.
-                raise OSError("Didn't receive full response, failing out")
-        firstline, self._buffer = self._buffer.split(eol, 1)
-        gc.collect()
-        return firstline
-
-    def recv(self, bufsize=0):
+    def recv(self, bufsize: int) -> bytes:
         """Reads some bytes from the connected remote address. Will only return
         an empty string after the configured timeout.
 
         :param int bufsize: maximum number of bytes to receive
         """
-        # print("Socket read", bufsize)
-        if bufsize == 0:  # read as much as we can at the moment
-            while True:
-                avail = self.available()
-                if avail:
-                    self._buffer += _the_interface.socket_read(self._socknum, avail)
-                else:
-                    break
-            gc.collect()
-            ret = self._buffer
-            self._buffer = b""
-            gc.collect()
-            return ret
-        stamp = time.monotonic()
-
-        to_read = bufsize - len(self._buffer)
-        received = []
-        while to_read > 0:
-            # print("Bytes to read:", to_read)
-            avail = self.available()
-            if avail:
-                stamp = time.monotonic()
-                recv = _the_interface.socket_read(self._socknum, min(to_read, avail))
-                received.append(recv)
-                to_read -= len(recv)
-                gc.collect()
-            elif received:
-                # We've received some bytes but no more are available. So return
-                # what we have.
-                break
-            if self._timeout > 0 and time.monotonic() - stamp > self._timeout:
-                break
-        # print(received)
-        self._buffer += b"".join(received)
-
-        ret = None
-        if len(self._buffer) == bufsize:
-            ret = self._buffer
-            self._buffer = b""
-        else:
-            ret = self._buffer[:bufsize]
-            self._buffer = self._buffer[bufsize:]
-        gc.collect()
-        return ret
+        buf = bytearray(bufsize)
+        self.recv_into(buf, bufsize)
+        return bytes(buf)
 
     def recv_into(self, buffer, nbytes: int = 0):
         """Read bytes from the connected remote address into a given buffer.
 
         :param bytearray buffer: the buffer to read into
         :param int nbytes: maximum number of bytes to receive; if 0,
             receive as many bytes as possible before filling the
@@ -174,55 +109,50 @@
         if not 0 <= nbytes <= len(buffer):
             raise ValueError("nbytes must be 0 to len(buffer)")
 
         last_read_time = time.monotonic()
         num_to_read = len(buffer) if nbytes == 0 else nbytes
         num_read = 0
         while num_to_read > 0:
-            num_avail = self.available()
+            num_avail = self._available()
             if num_avail > 0:
                 last_read_time = time.monotonic()
                 bytes_read = _the_interface.socket_read(
                     self._socknum, min(num_to_read, num_avail)
                 )
                 buffer[num_read : num_read + len(bytes_read)] = bytes_read
                 num_read += len(bytes_read)
                 num_to_read -= num_read
             elif num_read > 0:
                 # We got a message, but there are no more bytes to read, so we can stop.
                 break
             # No bytes yet, or more bytes requested.
             if self._timeout > 0 and time.monotonic() - last_read_time > self._timeout:
-                break
+                raise timeout("timed out")
         return num_read
 
-    def read(self, size=0):
-        """Read up to 'size' bytes from the socket, this may be buffered internally!
-        If 'size' isnt specified, return everything in the buffer.
-        NOTE: This method is deprecated and will be removed.
-        """
-        return self.recv(size)
-
     def settimeout(self, value):
-        """Set the read timeout for sockets, if value is 0 it will block"""
+        """Set the read timeout for sockets.
+        If value is 0 socket reads will block until a message is available.
+        """
         self._timeout = value
 
-    def available(self):
+    def _available(self):
         """Returns how many bytes of data are available to be read (up to the MAX_PACKET length)"""
-        if self.socknum != NO_SOCKET_AVAIL:
+        if self._socknum != NO_SOCKET_AVAIL:
             return min(_the_interface.socket_available(self._socknum), MAX_PACKET)
         return 0
 
-    def connected(self):
+    def _connected(self):
         """Whether or not we are connected to the socket"""
-        if self.socknum == NO_SOCKET_AVAIL:
+        if self._socknum == NO_SOCKET_AVAIL:
             return False
-        if self.available():
+        if self._available():
             return True
-        status = _the_interface.socket_status(self.socknum)
+        status = _the_interface.socket_status(self._socknum)
         result = status not in (
             adafruit_esp32spi.SOCKET_LISTEN,
             adafruit_esp32spi.SOCKET_CLOSED,
             adafruit_esp32spi.SOCKET_FIN_WAIT_1,
             adafruit_esp32spi.SOCKET_FIN_WAIT_2,
             adafruit_esp32spi.SOCKET_TIME_WAIT,
             adafruit_esp32spi.SOCKET_SYN_SENT,
@@ -230,18 +160,21 @@
             adafruit_esp32spi.SOCKET_CLOSE_WAIT,
         )
         if not result:
             self.close()
             self._socknum = NO_SOCKET_AVAIL
         return result
 
-    @property
-    def socknum(self):
-        """The socket number"""
-        return self._socknum
-
     def close(self):
         """Close the socket, after reading whatever remains"""
         _the_interface.socket_close(self._socknum)
 
 
+class timeout(TimeoutError):
+    """TimeoutError class. An instance of this error will be raised by recv_into() if
+    the timeout has elapsed and we haven't received any data yet."""
+
+    def __init__(self, msg):
+        super().__init__(msg)
+
+
 # pylint: enable=unused-argument, redefined-builtin, invalid-name
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py` & `adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/digitalio.py` & `adafruit-circuitpython-esp32spi-6.0.0/adafruit_esp32spi/digitalio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/docs/_static/favicon.ico` & `adafruit-circuitpython-esp32spi-6.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/docs/api.rst` & `adafruit-circuitpython-esp32spi-6.0.0/docs/api.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,12 @@
 
 .. automodule:: adafruit_esp32spi.adafruit_esp32spi_socket
    :members:
 
 .. automodule:: adafruit_esp32spi.adafruit_esp32spi_wifimanager
    :members:
 
-.. automodule:: adafruit_esp32spi.adafruit_esp32spi_wsgiserver
-   :members:
-
 .. automodule:: adafruit_esp32spi.digitalio
    :members:
 
 .. automodule:: adafruit_esp32spi.PWMOut
    :members:
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/docs/conf.py` & `adafruit-circuitpython-esp32spi-6.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/docs/index.rst` & `adafruit-circuitpython-esp32spi-6.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_aio_post.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_cheerlights.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_ipconfig.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_ipconfig.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_localtime.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_localtime.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_simpletest.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_simpletest_rp2040.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_simpletest_rp2040.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_tcp_client.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_tcp_client.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_udp_client.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_udp_client.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_wpa2ent_aio_post.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_wpa2ent_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_wpa2ent_simpletest.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/esp32spi_wpa2ent_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/gpio/esp32spi_gpio.py` & `adafruit-circuitpython-esp32spi-6.0.0/examples/gpio/esp32spi_gpio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/examples/gpio/gpio.md` & `adafruit-circuitpython-esp32spi-6.0.0/examples/gpio/gpio.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.6/pyproject.toml` & `adafruit-circuitpython-esp32spi-6.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-esp32spi"
 description = "CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI"
-version = "5.0.6"
+version = "6.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI"}
 keywords = [
     "adafruit",
```

