# Comparing `tmp/adafruit-circuitpython-requests-1.9.9.tar.gz` & `tmp/adafruit-circuitpython-requests-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-requests-1.9.9.tar", last modified: Thu Apr  8 17:55:08 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-requests-2.0.0.tar", last modified: Sat Jul  8 14:20:32 2023, max compression
```

## Comparing `adafruit-circuitpython-requests-1.9.9.tar` & `adafruit-circuitpython-requests-2.0.0.tar`

### file list

```diff
@@ -1,62 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.177097 adafruit-circuitpython-requests-1.9.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.181098 adafruit-circuitpython-requests-1.9.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.github/workflows/release.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)      189 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (121)    16223 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.pylintrc
--rwxr-xr-x   0 runner    (1001) docker     (121)      162 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)     6147 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (121)     1098 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.181098 adafruit-circuitpython-requests-1.9.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     2205 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.181098 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2021-04-08 17:55:07.000000 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-04-08 17:55:08.000000 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-08 17:55:07.000000 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-04-08 17:55:07.000000 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-04-08 17:55:07.000000 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    23369 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/adafruit_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.181098 adafruit-circuitpython-requests-1.9.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/docs/_static/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4414 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/_static/favicon.ico.license
--rwxr-xr-x   0 runner    (1001) docker     (121)      267 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     5437 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      190 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/examples.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (121)      901 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2183 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_advanced.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2028 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_cellular.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_cpython.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_ethernet.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      515 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_github_cpython.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1853 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_https_circuitpython.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1348 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_https_cpython.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2986 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2506 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_cellular.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1307 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_cpython.py
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_ethernet.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      119 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1977 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3921 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/chunk_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/header_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/legacy_mocket.py
--rw-r--r--   0 runner    (1001) docker     (121)     6638 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/legacy_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/parse_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/post_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3282 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6858 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/reuse_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.508599 adafruit-circuitpython-requests-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.500599 adafruit-circuitpython-requests-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.500599 adafruit-circuitpython-requests-2.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.500599 adafruit-circuitpython-requests-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.github/workflows/release_pypi.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6147 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.504599 adafruit-circuitpython-requests-2.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-08 14:20:32.508599 adafruit-circuitpython-requests-2.0.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2524 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.504599 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-08 14:20:32.000000 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-08 14:20:32.000000 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:20:32.000000 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 14:20:32.000000 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-08 14:20:32.000000 adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29095 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/adafruit_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.504599 adafruit-circuitpython-requests-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.504599 adafruit-circuitpython-requests-2.0.0/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4414 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/_static/favicon.ico.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5677 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      190 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/examples.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)      973 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.508599 adafruit-circuitpython-requests-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_adafruit_discord_active_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_advanced.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_cellular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_mastodon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_openskynetwork_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_openskynetwork_private_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_openskynetwork_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_api_youtube.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_github_cpython.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1853 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_https_circuitpython.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_https_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_multiple_cookies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2986 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2506 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_cellular.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:20:32.508599 adafruit-circuitpython-requests-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:20:32.508599 adafruit-circuitpython-requests-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/chunk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/chunked_redirect_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/header_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/parse_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/post_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-08 14:20:24.000000 adafruit-circuitpython-requests-2.0.0/tests/reuse_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-08 14:20:16.000000 adafruit-circuitpython-requests-2.0.0/tox.ini
```

### Comparing `adafruit-circuitpython-requests-1.9.9/.pre-commit-config.yaml` & `adafruit-circuitpython-requests-2.0.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 23.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v1.1.2
+    hooks:
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.4.0
+    hooks:
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
+    rev: v2.17.4
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
-    hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
-    rev: pylint-2.7.1
-    hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
+        args:
+          - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
--   repo: local
-    hooks:
-    -   id: pylint_examples
-        name: pylint (examples code)
+      - id: pylint
+        name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name $example; done)']
-        language: system
--   repo: local
-    hooks:
-    -   id: pylint_tests
-        name: pylint (tests code)
+        types: [python]
+        files: "^examples/"
+        args:
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
+        name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "tests" ]] || for example in $(find . -path "./tests/*.py"); do pylint --disable=missing-docstring,invalid-name $example; done)']
-        language: system
+        types: [python]
+        files: "^tests/"
+        args:
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-requests-1.9.9/.pylintrc` & `adafruit-circuitpython-requests-2.0.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-requests-1.9.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-requests-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/LICENSE` & `adafruit-circuitpython-requests-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-requests-2.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/LICENSES/MIT.txt` & `adafruit-circuitpython-requests-2.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-requests-2.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/PKG-INFO` & `adafruit-circuitpython-requests-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,92 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 1.9.9
+Version: 2.0.0
 Summary: A requests-like library for web interfacing
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Requests
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Description: Introduction
-        ============
-        
-        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-requests/badge/?version=latest
-            :target: https://circuitpython.readthedocs.io/projects/requests/en/latest/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/discord/327254708534116352.svg
-            :target: https://adafru.it/discord
-            :alt: Discord
-        
-        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_Requests/workflows/Build%20CI/badge.svg
-            :target: https://github.com/adafruit/Adafruit_CircuitPython_Requests/actions/
-            :alt: Build Status
-        
-        A requests-like library for HTTP commands.
-        
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading
-        `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
-        
-        Installing from PyPI
-        =====================
-        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-        PyPI <https://pypi.org/project/adafruit-circuitpython-requests/>`_. To install for current user:
-        
-        .. code-block:: shell
-        
-            pip3 install adafruit-circuitpython-requests
-        
-        To install system-wide (this may be required in some cases):
-        
-        .. code-block:: shell
-        
-            sudo pip3 install adafruit-circuitpython-requests
-        
-        To install in a virtual environment in your current project:
-        
-        .. code-block:: shell
-        
-            mkdir project-name && cd project-name
-            python3 -m venv .env
-            source .env/bin/activate
-            pip3 install adafruit-circuitpython-requests
-        
-        Usage Example
-        =============
-        
-        Usage examples are within the `examples` subfolder of this library.
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_Requests/blob/master/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Documentation
-        =============
-        
-        For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-        
-Keywords: adafruit blinka circuitpython micropython requests requests,networking
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
+Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
+License-File: LICENSE
+
+Introduction
+============
+
+.. image:: https://readthedocs.org/projects/adafruit-circuitpython-requests/badge/?version=latest
+    :target: https://docs.circuitpython.org/projects/requests/en/latest/
+    :alt: Documentation Status
+
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
+    :target: https://adafru.it/discord
+    :alt: Discord
+
+.. image:: https://github.com/adafruit/Adafruit_CircuitPython_Requests/workflows/Build%20CI/badge.svg
+    :target: https://github.com/adafruit/Adafruit_CircuitPython_Requests/actions/
+    :alt: Build Status
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
+A requests-like library for HTTP commands.
+
+
+Dependencies
+=============
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading
+`the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
+
+Installing from PyPI
+=====================
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+PyPI <https://pypi.org/project/adafruit-circuitpython-requests/>`_. To install for current user:
+
+.. code-block:: shell
+
+    pip3 install adafruit-circuitpython-requests
+
+To install system-wide (this may be required in some cases):
+
+.. code-block:: shell
+
+    sudo pip3 install adafruit-circuitpython-requests
+
+To install in a virtual environment in your current project:
+
+.. code-block:: shell
+
+    mkdir project-name && cd project-name
+    python3 -m venv .venv
+    source .venv/bin/activate
+    pip3 install adafruit-circuitpython-requests
+
+Usage Example
+=============
+
+Usage examples are within the `examples` subfolder of this library.
+
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/requests/en/latest/>`_.
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
+Contributing
+============
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/adafruit/Adafruit_CircuitPython_Requests/blob/main/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-requests-1.9.9/README.rst` & `adafruit-circuitpython-requests-2.0.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-requests/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/requests/en/latest/
+    :target: https://docs.circuitpython.org/projects/requests/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_Requests/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_Requests/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 A requests-like library for HTTP commands.
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -42,27 +46,29 @@
     sudo pip3 install adafruit-circuitpython-requests
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-requests
 
 Usage Example
 =============
 
 Usage examples are within the `examples` subfolder of this library.
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/requests/en/latest/>`_.
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/adafruit/Adafruit_CircuitPython_Requests/blob/master/CODE_OF_CONDUCT.md>`_
+<https://github.com/adafruit/Adafruit_CircuitPython_Requests/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/PKG-INFO` & `adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,92 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 1.9.9
+Version: 2.0.0
 Summary: A requests-like library for web interfacing
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Requests
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Description: Introduction
-        ============
-        
-        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-requests/badge/?version=latest
-            :target: https://circuitpython.readthedocs.io/projects/requests/en/latest/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/discord/327254708534116352.svg
-            :target: https://adafru.it/discord
-            :alt: Discord
-        
-        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_Requests/workflows/Build%20CI/badge.svg
-            :target: https://github.com/adafruit/Adafruit_CircuitPython_Requests/actions/
-            :alt: Build Status
-        
-        A requests-like library for HTTP commands.
-        
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading
-        `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
-        
-        Installing from PyPI
-        =====================
-        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-        PyPI <https://pypi.org/project/adafruit-circuitpython-requests/>`_. To install for current user:
-        
-        .. code-block:: shell
-        
-            pip3 install adafruit-circuitpython-requests
-        
-        To install system-wide (this may be required in some cases):
-        
-        .. code-block:: shell
-        
-            sudo pip3 install adafruit-circuitpython-requests
-        
-        To install in a virtual environment in your current project:
-        
-        .. code-block:: shell
-        
-            mkdir project-name && cd project-name
-            python3 -m venv .env
-            source .env/bin/activate
-            pip3 install adafruit-circuitpython-requests
-        
-        Usage Example
-        =============
-        
-        Usage examples are within the `examples` subfolder of this library.
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_Requests/blob/master/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Documentation
-        =============
-        
-        For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-        
-Keywords: adafruit blinka circuitpython micropython requests requests,networking
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
+Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
+License-File: LICENSE
+
+Introduction
+============
+
+.. image:: https://readthedocs.org/projects/adafruit-circuitpython-requests/badge/?version=latest
+    :target: https://docs.circuitpython.org/projects/requests/en/latest/
+    :alt: Documentation Status
+
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
+    :target: https://adafru.it/discord
+    :alt: Discord
+
+.. image:: https://github.com/adafruit/Adafruit_CircuitPython_Requests/workflows/Build%20CI/badge.svg
+    :target: https://github.com/adafruit/Adafruit_CircuitPython_Requests/actions/
+    :alt: Build Status
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
+A requests-like library for HTTP commands.
+
+
+Dependencies
+=============
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading
+`the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
+
+Installing from PyPI
+=====================
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+PyPI <https://pypi.org/project/adafruit-circuitpython-requests/>`_. To install for current user:
+
+.. code-block:: shell
+
+    pip3 install adafruit-circuitpython-requests
+
+To install system-wide (this may be required in some cases):
+
+.. code-block:: shell
+
+    sudo pip3 install adafruit-circuitpython-requests
+
+To install in a virtual environment in your current project:
+
+.. code-block:: shell
+
+    mkdir project-name && cd project-name
+    python3 -m venv .venv
+    source .venv/bin/activate
+    pip3 install adafruit-circuitpython-requests
+
+Usage Example
+=============
+
+Usage examples are within the `examples` subfolder of this library.
+
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/requests/en/latest/>`_.
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
+Contributing
+============
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/adafruit/Adafruit_CircuitPython_Requests/blob/main/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/SOURCES.txt` & `adafruit-circuitpython-requests-2.0.0/adafruit_circuitpython_requests.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
-.readthedocs.yml
+.readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_requests.py
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
+tox.ini
+.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
-.github/workflows/release.yml
+.github/workflows/failure-help-text.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_requests.egg-info/PKG-INFO
 adafruit_circuitpython_requests.egg-info/SOURCES.txt
 adafruit_circuitpython_requests.egg-info/dependency_links.txt
 adafruit_circuitpython_requests.egg-info/requires.txt
@@ -22,30 +27,42 @@
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
+docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/requests_adafruit_discord_active_online.py
 examples/requests_advanced.py
 examples/requests_advanced_cellular.py
 examples/requests_advanced_cpython.py
 examples/requests_advanced_ethernet.py
+examples/requests_api_discord.py
+examples/requests_api_github.py
+examples/requests_api_mastodon.py
+examples/requests_api_openskynetwork_private.py
+examples/requests_api_openskynetwork_private_area.py
+examples/requests_api_openskynetwork_public.py
+examples/requests_api_steam.py
+examples/requests_api_twitch.py
+examples/requests_api_twitter.py
+examples/requests_api_youtube.py
 examples/requests_github_cpython.py
 examples/requests_https_circuitpython.py
 examples/requests_https_cpython.py
+examples/requests_multiple_cookies.py
 examples/requests_simpletest.py
 examples/requests_simpletest_cellular.py
 examples/requests_simpletest_cpython.py
 examples/requests_simpletest_ethernet.py
 tests/chunk_test.py
+tests/chunked_redirect_test.py
 tests/concurrent_test.py
 tests/header_test.py
-tests/legacy_mocket.py
-tests/legacy_test.py
 tests/mocket.py
 tests/parse_test.py
 tests/post_test.py
 tests/protocol_test.py
 tests/reuse_test.py
```

### Comparing `adafruit-circuitpython-requests-1.9.9/docs/_static/favicon.ico` & `adafruit-circuitpython-requests-2.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/docs/conf.py` & `adafruit-circuitpython-requests-2.0.0/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,52 +2,61 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
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
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 # autodoc_mock_imports = ["digitalio", "busio"]
 
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.4", None),
-    "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
+    "python": ("https://docs.python.org/3", None),
+    "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit Requests Library"
-copyright = "2019 ladyada"
+creation_year = "2019"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " ladyada"
 author = "ladyada"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -56,15 +65,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-requests-1.9.9/docs/index.rst` & `adafruit-circuitpython-requests-2.0.0/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 
 .. toctree::
     :caption: Related Products
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_Requests/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_Requests/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-requests-1.9.9/examples/requests_advanced.py` & `adafruit-circuitpython-requests-2.0.0/examples/requests_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_cellular.py` & `adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_cpython.py` & `adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_ethernet.py` & `adafruit-circuitpython-requests-2.0.0/examples/requests_advanced_ethernet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/examples/requests_github_cpython.py` & `adafruit-circuitpython-requests-2.0.0/examples/requests_github_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/examples/requests_https_circuitpython.py` & `adafruit-circuitpython-requests-2.0.0/examples/requests_https_circuitpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/examples/requests_https_cpython.py` & `adafruit-circuitpython-requests-2.0.0/examples/requests_https_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest.py` & `adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_cellular.py` & `adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_ethernet.py` & `adafruit-circuitpython-requests-2.0.0/examples/requests_simpletest_ethernet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/tests/chunk_test.py` & `adafruit-circuitpython-requests-2.0.0/tests/chunk_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/tests/concurrent_test.py` & `adafruit-circuitpython-requests-2.0.0/tests/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/tests/header_test.py` & `adafruit-circuitpython-requests-2.0.0/tests/header_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/tests/legacy_mocket.py` & `adafruit-circuitpython-requests-2.0.0/tests/mocket.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,73 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
-""" Mock for Legacy Socket """
+""" Mock Socket """
 
 from unittest import mock
 
-SOCK_STREAM = 0
 
-set_interface = mock.Mock()
-interface = mock.MagicMock()
-getaddrinfo = mock.Mock()
-socket = mock.Mock()
+class MocketPool:  # pylint: disable=too-few-public-methods
+    """Mock SocketPool"""
+
+    SOCK_STREAM = 0
+
+    def __init__(self):
+        self.getaddrinfo = mock.Mock()
+        self.socket = mock.Mock()
 
 
 class Mocket:  # pylint: disable=too-few-public-methods
-    """  Mock Socket """
+    """Mock Socket"""
 
     def __init__(self, response):
         self.settimeout = mock.Mock()
         self.close = mock.Mock()
         self.connect = mock.Mock()
         self.send = mock.Mock(side_effect=self._send)
         self.readline = mock.Mock(side_effect=self._readline)
         self.recv = mock.Mock(side_effect=self._recv)
-        self.fail_next_send = False
+        self.recv_into = mock.Mock(side_effect=self._recv_into)
         self._response = response
         self._position = 0
+        self.fail_next_send = False
 
-    def _send(self, data):  # pylint: disable=unused-argument
+    def _send(self, data):
         if self.fail_next_send:
             self.fail_next_send = False
-            raise RuntimeError("Send failed")
+            return 0
+        return len(data)
 
     def _readline(self):
         i = self._response.find(b"\r\n", self._position)
         response = self._response[self._position : i + 2]
         self._position = i + 2
         return response
 
     def _recv(self, count):
         end = self._position + count
         response = self._response[self._position : end]
         self._position = end
-        print(response)
         return response
+
+    def _recv_into(self, buf, nbytes=0):
+        assert isinstance(nbytes, int) and nbytes >= 0
+        read = nbytes if nbytes > 0 else len(buf)
+        remaining = len(self._response) - self._position
+        read = min(read, remaining)
+        end = self._position + read
+        buf[:read] = self._response[self._position : end]
+        self._position = end
+        return read
+
+
+class SSLContext:  # pylint: disable=too-few-public-methods
+    """Mock SSL Context"""
+
+    def __init__(self):
+        self.wrap_socket = mock.Mock(side_effect=self._wrap_socket)
+
+    def _wrap_socket(
+        self, sock, server_hostname=None
+    ):  # pylint: disable=no-self-use,unused-argument
+        return sock
```

### Comparing `adafruit-circuitpython-requests-1.9.9/tests/legacy_test.py` & `adafruit-circuitpython-requests-2.0.0/tests/reuse_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,208 +1,239 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
-""" Legacy Tests """
+""" Reuse Tests """
 
 from unittest import mock
-import json
-import legacy_mocket as mocket
+import mocket
+import pytest
 import adafruit_requests
 
 IP = "1.2.3.4"
-HOST = "httpbin.org"
-RESPONSE = {"Date": "July 25, 2019"}
-ENCODED = json.dumps(RESPONSE).encode("utf-8")
-HEADERS = "HTTP/1.0 200 OK\r\nContent-Length: {}\r\n\r\n".format(len(ENCODED)).encode(
-    "utf-8"
-)
+HOST = "wifitest.adafruit.com"
+HOST2 = "wifitest2.adafruit.com"
+PATH = "/testwifi/index.html"
+TEXT = b"This is a test of Adafruit WiFi!\r\nIf you can read this, its working :)"
+RESPONSE = b"HTTP/1.0 200 OK\r\nContent-Length: 70\r\n\r\n" + TEXT
 
 
-def test_get_json():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
-    sock = mocket.Mocket(HEADERS + ENCODED)
-    mocket.socket.return_value = sock
+def test_get_twice():
+    pool = mocket.MocketPool()
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE + RESPONSE)
+    pool.socket.return_value = sock
+    ssl = mocket.SSLContext()
 
-    adafruit_requests.set_socket(mocket, mocket.interface)
-    response = adafruit_requests.get("http://" + HOST + "/get")
+    requests_session = adafruit_requests.Session(pool, ssl)
+    response = requests_session.get("https://" + HOST + PATH)
 
-    sock.connect.assert_called_once_with((IP, 80))
-    assert response.json() == RESPONSE
-    response.close()
-
-
-def test_tls_mode():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
-    sock = mocket.Mocket(HEADERS + ENCODED)
-    mocket.socket.return_value = sock
-
-    adafruit_requests.set_socket(mocket, mocket.interface)
-    response = adafruit_requests.get("https://" + HOST + "/get")
-
-    sock.connect.assert_called_once_with((HOST, 443), mocket.interface.TLS_MODE)
-    assert response.json() == RESPONSE
-    response.close()
+    sock.send.assert_has_calls(
+        [
+            mock.call(b"GET"),
+            mock.call(b" /"),
+            mock.call(b"testwifi/index.html"),
+            mock.call(b" HTTP/1.1\r\n"),
+        ]
+    )
+    sock.send.assert_has_calls(
+        [
+            mock.call(b"Host: "),
+            mock.call(b"wifitest.adafruit.com"),
+        ]
+    )
+    assert response.text == str(TEXT, "utf-8")
 
+    response = requests_session.get("https://" + HOST + PATH + "2")
 
-def test_post_string():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
-    sock = mocket.Mocket(HEADERS + ENCODED)
-    mocket.socket.return_value = sock
+    sock.send.assert_has_calls(
+        [
+            mock.call(b"GET"),
+            mock.call(b" /"),
+            mock.call(b"testwifi/index.html2"),
+            mock.call(b" HTTP/1.1\r\n"),
+        ]
+    )
+    sock.send.assert_has_calls(
+        [
+            mock.call(b"Host: "),
+            mock.call(b"wifitest.adafruit.com"),
+        ]
+    )
 
-    adafruit_requests.set_socket(mocket, mocket.interface)
-    data = "31F"
-    response = adafruit_requests.post("http://" + HOST + "/post", data=data)
-    sock.connect.assert_called_once_with((IP, 80))
-    sock.send.assert_called_with(b"31F")
-    response.close()
+    assert response.text == str(TEXT, "utf-8")
+    sock.connect.assert_called_once_with((HOST, 443))
+    pool.socket.assert_called_once()
 
 
-def test_second_tls_send_fails():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
-    sock = mocket.Mocket(HEADERS + ENCODED)
-    sock2 = mocket.Mocket(HEADERS + ENCODED)
-    mocket.socket.call_count = 0  # Reset call count
-    mocket.socket.side_effect = [sock, sock2]
+def test_get_twice_after_second():
+    pool = mocket.MocketPool()
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE + RESPONSE)
+    pool.socket.return_value = sock
+    ssl = mocket.SSLContext()
 
-    adafruit_requests.set_socket(mocket, mocket.interface)
-    response = adafruit_requests.get("https://" + HOST + "/testwifi/index.html")
+    requests_session = adafruit_requests.Session(pool, ssl)
+    response = requests_session.get("https://" + HOST + PATH)
 
     sock.send.assert_has_calls(
         [
+            mock.call(b"GET"),
+            mock.call(b" /"),
             mock.call(b"testwifi/index.html"),
+            mock.call(b" HTTP/1.1\r\n"),
         ]
     )
-
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
-            mock.call(HOST.encode("utf-8")),
-            mock.call(b"\r\n"),
+            mock.call(b"wifitest.adafruit.com"),
         ]
     )
-    assert response.text == str(ENCODED, "utf-8")
 
-    sock.fail_next_send = True
-    adafruit_requests.get("https://" + HOST + "/get2")
+    requests_session.get("https://" + HOST + PATH + "2")
 
-    sock.connect.assert_called_once_with((HOST, 443), mocket.interface.TLS_MODE)
-    sock2.connect.assert_called_once_with((HOST, 443), mocket.interface.TLS_MODE)
-    # Make sure that the socket is closed after send fails.
-    sock.close.assert_called_once()
-    assert sock2.close.call_count == 0
-    assert mocket.socket.call_count == 2
+    sock.send.assert_has_calls(
+        [
+            mock.call(b"GET"),
+            mock.call(b" /"),
+            mock.call(b"testwifi/index.html2"),
+            mock.call(b" HTTP/1.1\r\n"),
+        ]
+    )
+    sock.send.assert_has_calls(
+        [
+            mock.call(b"Host: "),
+            mock.call(b"wifitest.adafruit.com"),
+        ]
+    )
+    sock.connect.assert_called_once_with((HOST, 443))
+    pool.socket.assert_called_once()
 
+    with pytest.raises(RuntimeError):
+        response.text == str(TEXT, "utf-8")  # pylint: disable=expression-not-assigned
 
-def test_second_send_fails():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
-    sock = mocket.Mocket(HEADERS + ENCODED)
-    sock2 = mocket.Mocket(HEADERS + ENCODED)
-    mocket.socket.call_count = 0  # Reset call count
-    mocket.socket.side_effect = [sock, sock2]
 
-    adafruit_requests.set_socket(mocket, mocket.interface)
-    response = adafruit_requests.get("http://" + HOST + "/testwifi/index.html")
+def test_connect_out_of_memory():
+    pool = mocket.MocketPool()
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE)
+    sock2 = mocket.Mocket(RESPONSE)
+    sock3 = mocket.Mocket(RESPONSE)
+    pool.socket.side_effect = [sock, sock2, sock3]
+    sock2.connect.side_effect = MemoryError()
+    ssl = mocket.SSLContext()
+
+    requests_session = adafruit_requests.Session(pool, ssl)
+    response = requests_session.get("https://" + HOST + PATH)
 
     sock.send.assert_has_calls(
         [
+            mock.call(b"GET"),
+            mock.call(b" /"),
             mock.call(b"testwifi/index.html"),
+            mock.call(b" HTTP/1.1\r\n"),
         ]
     )
-
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
-            mock.call(HOST.encode("utf-8")),
-            mock.call(b"\r\n"),
+            mock.call(b"wifitest.adafruit.com"),
         ]
     )
-    assert response.text == str(ENCODED, "utf-8")
+    assert response.text == str(TEXT, "utf-8")
 
-    sock.fail_next_send = True
-    adafruit_requests.get("http://" + HOST + "/get2")
+    response = requests_session.get("https://" + HOST2 + PATH)
+    sock3.send.assert_has_calls(
+        [
+            mock.call(b"GET"),
+            mock.call(b" /"),
+            mock.call(b"testwifi/index.html"),
+            mock.call(b" HTTP/1.1\r\n"),
+        ]
+    )
+    sock3.send.assert_has_calls(
+        [
+            mock.call(b"Host: "),
+            mock.call(b"wifitest2.adafruit.com"),
+        ]
+    )
 
-    sock.connect.assert_called_once_with((IP, 80))
-    sock2.connect.assert_called_once_with((IP, 80))
-    # Make sure that the socket is closed after send fails.
+    assert response.text == str(TEXT, "utf-8")
     sock.close.assert_called_once()
-    assert sock2.close.call_count == 0
-    assert mocket.socket.call_count == 2
+    sock.connect.assert_called_once_with((HOST, 443))
+    sock3.connect.assert_called_once_with((HOST2, 443))
 
 
-def test_first_read_fails():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
-    sock = mocket.Mocket(b"")
-    sock2 = mocket.Mocket(HEADERS + ENCODED)
-    mocket.socket.call_count = 0  # Reset call count
-    mocket.socket.side_effect = [sock, sock2]
+def test_second_send_fails():
+    pool = mocket.MocketPool()
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE)
+    sock2 = mocket.Mocket(RESPONSE)
+    pool.socket.side_effect = [sock, sock2]
+
+    ssl = mocket.SSLContext()
 
-    adafruit_requests.set_socket(mocket, mocket.interface)
-    adafruit_requests.get("http://" + HOST + "/testwifi/index.html")
+    requests_session = adafruit_requests.Session(pool, ssl)
+    response = requests_session.get("https://" + HOST + PATH)
 
     sock.send.assert_has_calls(
         [
             mock.call(b"testwifi/index.html"),
         ]
     )
 
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
-            mock.call(HOST.encode("utf-8")),
+            mock.call(b"wifitest.adafruit.com"),
             mock.call(b"\r\n"),
         ]
     )
+    assert response.text == str(TEXT, "utf-8")
 
-    sock2.send.assert_has_calls(
-        [
-            mock.call(b"Host: "),
-            mock.call(HOST.encode("utf-8")),
-            mock.call(b"\r\n"),
-        ]
-    )
+    sock.fail_next_send = True
+    requests_session.get("https://" + HOST + PATH + "2")
 
-    sock.connect.assert_called_once_with((IP, 80))
-    sock2.connect.assert_called_once_with((IP, 80))
-    # Make sure that the socket is closed after the first receive fails.
+    sock.connect.assert_called_once_with((HOST, 443))
+    sock2.connect.assert_called_once_with((HOST, 443))
+    # Make sure that the socket is closed after send fails.
     sock.close.assert_called_once()
-    assert mocket.socket.call_count == 2
+    assert sock2.close.call_count == 0
+    assert pool.socket.call_count == 2
 
 
-def test_second_tls_connect_fails():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
-    sock = mocket.Mocket(HEADERS + ENCODED)
-    sock2 = mocket.Mocket(HEADERS + ENCODED)
-    sock3 = mocket.Mocket(HEADERS + ENCODED)
-    mocket.socket.call_count = 0  # Reset call count
-    mocket.socket.side_effect = [sock, sock2, sock3]
-    sock2.connect.side_effect = RuntimeError("error connecting")
+def test_second_send_lies_recv_fails():  # pylint: disable=invalid-name
+    pool = mocket.MocketPool()
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE)
+    sock2 = mocket.Mocket(RESPONSE)
+    pool.socket.side_effect = [sock, sock2]
 
-    adafruit_requests.set_socket(mocket, mocket.interface)
-    response = adafruit_requests.get("https://" + HOST + "/testwifi/index.html")
+    ssl = mocket.SSLContext()
+
+    requests_session = adafruit_requests.Session(pool, ssl)
+    response = requests_session.get("https://" + HOST + PATH)
 
     sock.send.assert_has_calls(
         [
             mock.call(b"testwifi/index.html"),
         ]
     )
 
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
-            mock.call(HOST.encode("utf-8")),
+            mock.call(b"wifitest.adafruit.com"),
             mock.call(b"\r\n"),
         ]
     )
-    assert response.text == str(ENCODED, "utf-8")
+    assert response.text == str(TEXT, "utf-8")
 
-    host2 = "test.adafruit.com"
-    response = adafruit_requests.get("https://" + host2 + "/get2")
+    requests_session.get("https://" + HOST + PATH + "2")
 
-    sock.connect.assert_called_once_with((HOST, 443), mocket.interface.TLS_MODE)
-    sock2.connect.assert_called_once_with((host2, 443), mocket.interface.TLS_MODE)
-    sock3.connect.assert_called_once_with((host2, 443), mocket.interface.TLS_MODE)
+    sock.connect.assert_called_once_with((HOST, 443))
+    sock2.connect.assert_called_once_with((HOST, 443))
     # Make sure that the socket is closed after send fails.
     sock.close.assert_called_once()
-    sock2.close.assert_called_once()
-    assert sock3.close.call_count == 0
-    assert mocket.socket.call_count == 3
+    assert sock2.close.call_count == 0
+    assert pool.socket.call_count == 2
```

### Comparing `adafruit-circuitpython-requests-1.9.9/tests/parse_test.py` & `adafruit-circuitpython-requests-2.0.0/tests/parse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/tests/post_test.py` & `adafruit-circuitpython-requests-2.0.0/tests/post_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.9/tests/protocol_test.py` & `adafruit-circuitpython-requests-2.0.0/tests/protocol_test.py`

 * *Files identical despite different names*

