# Comparing `tmp/vessim-0.0.3.tar.gz` & `tmp/vessim-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vessim-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vessim-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vessim-0.0.3.tar` & `vessim-0.1.0.tar`

### file list

```diff
@@ -1,51 +1,56 @@
--rw-r--r--   0        0        0     1078 2023-06-16 14:57:30.270261 vessim-0.0.3/.github/workflows/vessim-ci.yml
--rw-r--r--   0        0        0     1142 2023-06-09 14:00:54.375018 vessim-0.0.3/.gitignore
--rw-r--r--   0        0        0     1089 2023-06-09 14:00:54.375226 vessim-0.0.3/LICENSE
--rw-r--r--   0        0        0     1602 2023-06-16 15:08:04.614316 vessim-0.0.3/README.md
--rw-r--r--   0        0        0     4778 2023-06-16 14:56:58.586950 vessim-0.0.3/examples/scenario_1.py
--rw-r--r--   0        0        0     4730 2023-06-16 14:53:48.527891 vessim-0.0.3/examples/sil/carbon-aware_control_unit/carbon_aware_control_unit.py
--rw-r--r--   0        0        0      931 2023-06-16 14:34:31.939597 vessim-0.0.3/examples/sil/carbon-aware_control_unit/main.py
--rw-r--r--   0        0        0     2097 2023-06-16 14:34:31.939747 vessim-0.0.3/examples/sil/example_node/README.md
--rw-r--r--   0        0        0     2262 2023-06-16 14:53:48.528050 vessim-0.0.3/examples/sil/example_node/node_api_server.py
--rw-r--r--   0        0        0      173 2023-06-16 14:34:31.940065 vessim-0.0.3/examples/sil/example_node/rpi/config/config.txt
--rw-r--r--   0        0        0      159 2023-06-16 14:34:31.940212 vessim-0.0.3/examples/sil/example_node/rpi/config/rc.local
--rw-r--r--   0        0        0     1405 2023-06-16 14:34:31.940332 vessim-0.0.3/examples/sil/example_node/rpi/init.sh
--rw-r--r--   0        0        0     2119 2023-06-16 14:34:31.940488 vessim-0.0.3/examples/sil/example_node/rpi/lib/pi_controller.py
--rw-r--r--   0        0        0       47 2023-06-16 14:34:31.940579 vessim-0.0.3/examples/sil/example_node/rpi/requirements.txt
--rw-r--r--   0        0        0     1294 2023-06-16 14:53:48.528254 vessim-0.0.3/examples/sil/example_node/rpi/rpi_api_server.py
--rw-r--r--   0        0        0      638 2023-06-16 14:34:31.940829 vessim-0.0.3/examples/sil/example_node/virtual_node/linear_power_model.py
--rw-r--r--   0        0        0       23 2023-06-16 14:34:31.940934 vessim-0.0.3/examples/sil/example_node/virtual_node/requirements.txt
--rw-r--r--   0        0        0     3550 2023-06-16 14:53:48.528453 vessim-0.0.3/examples/sil/example_node/virtual_node/v_node_api_server.py
--rw-r--r--   0        0        0      897 2023-06-16 14:34:31.941210 vessim-0.0.3/examples/sil/tf_gcp_node/.gitignore
--rw-r--r--   0        0        0     2253 2023-06-16 14:34:31.941318 vessim-0.0.3/examples/sil/tf_gcp_node/README.md
--rw-r--r--   0        0        0     3194 2023-06-16 14:34:31.941444 vessim-0.0.3/examples/sil/tf_gcp_node/main.tf
--rw-r--r--   0        0        0      249 2023-06-16 14:34:31.941592 vessim-0.0.3/examples/sil/tf_gcp_node/outputs.tf
--rwxr-xr-x   0        0        0      262 2023-06-16 14:34:31.941737 vessim-0.0.3/examples/sil/tf_gcp_node/ssh_scripts/tfreceive
--rwxr-xr-x   0        0        0      248 2023-06-16 14:34:31.941842 vessim-0.0.3/examples/sil/tf_gcp_node/ssh_scripts/tfsend
--rwxr-xr-x   0        0        0      225 2023-06-16 14:34:31.941938 vessim-0.0.3/examples/sil/tf_gcp_node/ssh_scripts/tfssh
--rw-r--r--   0        0        0      667 2023-06-16 14:34:31.942037 vessim-0.0.3/examples/sil/tf_gcp_node/variables.tf
--rw-r--r--   0        0        0    58362 2023-06-16 14:34:31.942294 vessim-0.0.3/experimental/custom.json
--rw-r--r--   0        0        0   427169 2023-06-16 15:07:31.717850 vessim-0.0.3/experimental/evaluation.ipynb
--rw-r--r--   0        0        0     1379 2023-06-09 14:00:54.382555 vessim-0.0.3/experimental/pp_scenario.py
--rw-r--r--   0        0        0     2826 2023-06-16 15:09:38.958920 vessim-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      415 2023-06-09 14:00:54.384250 vessim-0.0.3/requirements.txt
--rw-r--r--   0        0        0     1442 2023-06-16 14:34:31.943217 vessim-0.0.3/tests/test_carbon_api.py
--rw-r--r--   0        0        0     1915 2023-06-16 14:34:31.943608 vessim-0.0.3/tests/test_storage.py
--rw-r--r--   0        0        0       83 2023-06-16 15:12:35.504704 vessim-0.0.3/vessim/__init__.py
--rw-r--r--   0        0        0      188 2023-06-16 14:34:31.943833 vessim-0.0.3/vessim/core/__init__.py
--rw-r--r--   0        0        0     2918 2023-06-16 14:34:31.944203 vessim-0.0.3/vessim/core/simulator.py
--rw-r--r--   0        0        0     4030 2023-06-16 14:34:31.944716 vessim-0.0.3/vessim/core/storage.py
--rw-r--r--   0        0        0      515 2023-06-16 14:34:31.944870 vessim-0.0.3/vessim/cosim/__init__.py
--rw-r--r--   0        0        0     5162 2023-06-16 14:34:31.945160 vessim-0.0.3/vessim/cosim/_util.py
--rw-r--r--   0        0        0     1625 2023-06-16 14:34:31.945661 vessim-0.0.3/vessim/cosim/carbon_api.py
--rw-r--r--   0        0        0     1706 2023-06-16 14:34:31.945796 vessim-0.0.3/vessim/cosim/computing_system.py
--rw-r--r--   0        0        0     9541 2023-06-16 14:56:58.587227 vessim-0.0.3/vessim/cosim/energy_system_interface.py
--rw-r--r--   0        0        0     1469 2023-06-16 14:34:31.946070 vessim-0.0.3/vessim/cosim/generator.py
--rw-r--r--   0        0        0     1425 2023-06-16 14:34:31.946197 vessim-0.0.3/vessim/cosim/microgrid.py
--rw-r--r--   0        0        0     2036 2023-06-16 14:34:31.946331 vessim-0.0.3/vessim/cosim/monitor.py
--rw-r--r--   0        0        0      131 2023-06-16 14:34:31.946456 vessim-0.0.3/vessim/sil/__init__.py
--rw-r--r--   0        0        0     2105 2023-06-16 14:53:48.533390 vessim-0.0.3/vessim/sil/http_client.py
--rw-r--r--   0        0        0      930 2023-06-16 14:34:31.946911 vessim-0.0.3/vessim/sil/node.py
--rw-r--r--   0        0        0     2325 2023-06-16 14:34:31.947017 vessim-0.0.3/vessim/sil/power_meter.py
--rw-r--r--   0        0        0     4522 2023-06-16 14:34:31.947351 vessim-0.0.3/vessim/sil/redis_docker.py
--rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 vessim-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1296 2023-07-03 15:22:36.274826 vessim-0.1.0/.github/workflows/vessim-ci.yml
+-rw-r--r--   0        0        0     1154 2023-06-29 06:30:43.698698 vessim-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1089 2023-06-09 14:00:54.375226 vessim-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2738 2023-07-08 10:42:54.147664 vessim-0.1.0/README.md
+-rw-r--r--   0        0        0      626 2023-07-03 15:22:36.275084 vessim-0.1.0/examples/_data.py
+-rw-r--r--   0        0        0     2767 2023-07-03 15:22:36.275318 vessim-0.1.0/examples/cosim_example.py
+-rw-r--r--   0        0        0     3167 2023-07-03 15:22:36.275468 vessim-0.1.0/examples/cosim_sil_example.py
+-rw-r--r--   0        0        0  1428270 2023-07-03 15:22:36.280887 vessim-0.1.0/examples/data/carbon_intensity.csv
+-rw-r--r--   0        0        0  1128276 2023-07-03 15:22:36.284210 vessim-0.1.0/examples/data/weather_berlin_2021-06.csv
+-rw-r--r--   0        0        0     5183 2023-07-03 15:22:32.793112 vessim-0.1.0/examples/sil/carbon-aware_control_unit/carbon_aware_control_unit.py
+-rw-r--r--   0        0        0     1450 2023-07-03 15:22:32.793478 vessim-0.1.0/examples/sil/carbon-aware_control_unit/main.py
+-rw-r--r--   0        0        0     2097 2023-06-16 14:34:31.939747 vessim-0.1.0/examples/sil/example_node/README.md
+-rw-r--r--   0        0        0     2262 2023-06-16 14:53:48.528050 vessim-0.1.0/examples/sil/example_node/node_api_server.py
+-rw-r--r--   0        0        0      173 2023-06-16 14:34:31.940065 vessim-0.1.0/examples/sil/example_node/rpi/config/config.txt
+-rw-r--r--   0        0        0      159 2023-06-16 14:34:31.940212 vessim-0.1.0/examples/sil/example_node/rpi/config/rc.local
+-rw-r--r--   0        0        0     1405 2023-06-16 14:34:31.940332 vessim-0.1.0/examples/sil/example_node/rpi/init.sh
+-rw-r--r--   0        0        0     2149 2023-06-29 06:30:43.700176 vessim-0.1.0/examples/sil/example_node/rpi/lib/pi_controller.py
+-rw-r--r--   0        0        0       47 2023-06-16 14:34:31.940579 vessim-0.1.0/examples/sil/example_node/rpi/requirements.txt
+-rw-r--r--   0        0        0     1290 2023-06-29 06:30:43.700595 vessim-0.1.0/examples/sil/example_node/rpi/rpi_api_server.py
+-rw-r--r--   0        0        0      638 2023-06-16 14:34:31.940829 vessim-0.1.0/examples/sil/example_node/virtual_node/linear_power_model.py
+-rw-r--r--   0        0        0       23 2023-06-16 14:34:31.940934 vessim-0.1.0/examples/sil/example_node/virtual_node/requirements.txt
+-rw-r--r--   0        0        0     3597 2023-06-29 06:30:43.700765 vessim-0.1.0/examples/sil/example_node/virtual_node/v_node_api_server.py
+-rw-r--r--   0        0        0      902 2023-06-29 06:30:43.701019 vessim-0.1.0/examples/sil/tf_gcp_node/.gitignore
+-rw-r--r--   0        0        0     2253 2023-06-16 14:34:31.941318 vessim-0.1.0/examples/sil/tf_gcp_node/README.md
+-rw-r--r--   0        0        0     2920 2023-06-29 06:30:43.701374 vessim-0.1.0/examples/sil/tf_gcp_node/main.tf
+-rw-r--r--   0        0        0      249 2023-06-16 14:34:31.941592 vessim-0.1.0/examples/sil/tf_gcp_node/outputs.tf
+-rwxr-xr-x   0        0        0      262 2023-06-16 14:34:31.941737 vessim-0.1.0/examples/sil/tf_gcp_node/ssh_scripts/tfreceive
+-rwxr-xr-x   0        0        0      248 2023-06-16 14:34:31.941842 vessim-0.1.0/examples/sil/tf_gcp_node/ssh_scripts/tfsend
+-rwxr-xr-x   0        0        0      225 2023-06-16 14:34:31.941938 vessim-0.1.0/examples/sil/tf_gcp_node/ssh_scripts/tfssh
+-rw-r--r--   0        0        0      667 2023-06-16 14:34:31.942037 vessim-0.1.0/examples/sil/tf_gcp_node/variables.tf
+-rw-r--r--   0        0        0   175373 2023-06-29 06:30:43.703104 vessim-0.1.0/experimental/baseline_experiment.ipynb
+-rw-r--r--   0        0        0    58362 2023-06-16 14:34:31.942294 vessim-0.1.0/experimental/custom.json
+-rw-r--r--   0        0        0     1394 2023-06-29 06:30:43.707622 vessim-0.1.0/experimental/pp_scenario.py
+-rw-r--r--   0        0        0     3259 2023-07-08 10:16:04.568903 vessim-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1442 2023-06-16 14:34:31.943217 vessim-0.1.0/tests/test_carbon_api.py
+-rw-r--r--   0        0        0     1915 2023-06-16 14:34:31.943608 vessim-0.1.0/tests/test_storage.py
+-rw-r--r--   0        0        0       83 2023-07-08 10:06:28.572911 vessim-0.1.0/vessim/__init__.py
+-rw-r--r--   0        0        0      188 2023-06-16 14:34:31.943833 vessim-0.1.0/vessim/core/__init__.py
+-rw-r--r--   0        0        0     1381 2023-07-03 10:58:34.957722 vessim-0.1.0/vessim/core/microgrid.py
+-rw-r--r--   0        0        0     2691 2023-07-08 10:04:28.186893 vessim-0.1.0/vessim/core/simulator.py
+-rw-r--r--   0        0        0     4159 2023-07-03 15:22:36.284479 vessim-0.1.0/vessim/core/storage.py
+-rw-r--r--   0        0        0      487 2023-07-03 10:58:34.958296 vessim-0.1.0/vessim/cosim/__init__.py
+-rw-r--r--   0        0        0     4609 2023-07-03 10:58:34.958809 vessim-0.1.0/vessim/cosim/_util.py
+-rw-r--r--   0        0        0     1650 2023-07-03 10:58:34.959274 vessim-0.1.0/vessim/cosim/carbon_api.py
+-rw-r--r--   0        0        0     1978 2023-07-03 10:35:01.124497 vessim-0.1.0/vessim/cosim/computing_system.py
+-rw-r--r--   0        0        0     1432 2023-07-03 10:58:34.959447 vessim-0.1.0/vessim/cosim/generator.py
+-rw-r--r--   0        0        0      975 2023-07-03 10:58:34.959738 vessim-0.1.0/vessim/cosim/microgrid.py
+-rw-r--r--   0        0        0     2356 2023-07-03 10:58:34.960060 vessim-0.1.0/vessim/cosim/monitor.py
+-rw-r--r--   0        0        0     6102 2023-07-03 15:22:36.284784 vessim-0.1.0/vessim/cosim/sil_interface.py
+-rw-r--r--   0        0        0      131 2023-06-16 14:34:31.946456 vessim-0.1.0/vessim/sil/__init__.py
+-rw-r--r--   0        0        0     6134 2023-07-03 09:39:51.812632 vessim-0.1.0/vessim/sil/api_server.py
+-rw-r--r--   0        0        0     2193 2023-07-03 09:39:51.812770 vessim-0.1.0/vessim/sil/http_client.py
+-rw-r--r--   0        0        0      930 2023-06-16 14:34:31.946911 vessim-0.1.0/vessim/sil/node.py
+-rw-r--r--   0        0        0     2333 2023-07-03 10:35:01.125242 vessim-0.1.0/vessim/sil/power_meter.py
+-rw-r--r--   0        0        0     1009 2023-07-03 09:32:31.700809 vessim-0.1.0/vessim/sil/stoppable_thread.py
+-rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 vessim-0.1.0/PKG-INFO
```

### Comparing `vessim-0.0.3/.github/workflows/vessim-ci.yml` & `vessim-0.1.0/.github/workflows/vessim-ci.yml`

 * *Files 15% similar despite different names*

```diff
@@ -5,37 +5,43 @@
 on: 
   push:
 
 jobs:
   linting-and-testing:
     # specifies the os that the job will run on 
     runs-on: ubuntu-latest
-
+    strategy:
+      matrix:
+        python-version: [3.8, 3.11]
     steps:
     # downloads the repository code to the runner's file system for workflow access
     - uses: actions/checkout@v2
     - uses: chartboost/ruff-action@v1
        
-    # sets up python environment with specified version 
-    - name: Set up Python
+    # sets up python environment with specified versions 
+    - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
-        python-version: '3.11'
+        python-version: ${{ matrix.python-version }}   
     
     # get rid of DeprecationWarning related to Jupyter paths when running pytest
     - name: Set JUPYTER_PLATFORM_DIRS environment variable
       env:
         JUPYTER_PLATFORM_DIRS: 1
       run: |
         echo "JUPYTER_PLATFORM_DIRS=${JUPYTER_PLATFORM_DIRS}" >> $GITHUB_ENV   
 
     # installs dependencies from requirements.txt
     - name: Install dependencies
       run: pip install -r requirements.txt
+    
+    # run type checker on Python files
+    - name: Run type checker
+      run: mypy vessim
 
     # run ruff on Python files
     - name: Run linter
       run: ruff .
-    
+        
     # run tests
     - name: Run tests
       run: python -m pytest
```

### Comparing `vessim-0.0.3/.gitignore` & `vessim-0.1.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .idea
 .vscode
 .texpadtmp
 .DS_Store
 .ipynb_checkpoints
 .ruff_cache
+.mypy_cache
 .pytest_cache
 __pycache__
 
 .eggs
 vessim.egg-info
 
 venv
```

### Comparing `vessim-0.0.3/LICENSE` & `vessim-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/README.md` & `vessim-0.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,94 @@
 # Vessim
 
 [![PyPI version](https://img.shields.io/pypi/v/vessim.svg?color=52c72b)](https://pypi.org/project/vessim/)
 ![Build](https://github.com/dos-group/vessim/actions/workflows/vessim-ci.yml/badge.svg)
 [![License](https://img.shields.io/pypi/l/vessim.svg)](https://pypi.org/project/vessim/)
 [![Supported versions](https://img.shields.io/pypi/pyversions/vessim.svg)](https://pypi.org/project/vessim/)
 
-Vessim is a versatile co-simulation testbed for carbon-aware applications and systems.
+Vessim is a versatile **co-simulation testbed for carbon-aware applications and systems**.
 It lets users connect domain-specific simulators for energy system components like renewable power generation, 
 energy storage, and power flow analysis with real software and hardware.
 
 Vessim is in alpha stage and under active development.
-Functionality and documentation will improve in the next weeks an months.
+Functionality and documentation will improve in the next weeks and months.
 
 
 ## ⚙️ Installation
 
-You can install the [latest release](https://pypi.org/project/vessim/) of Vessim via [pip](https://pip.pypa.io/en/stable/quickstart/):
+If you are using Vessim for the first time, we recommend to clone and install this repository, so you have all
+code and examples at hand:
+
+```
+$ pip install -e .
+```
+
+Alternatively, you can also install our [latest release](https://pypi.org/project/vessim/) 
+via [pip](https://pip.pypa.io/en/stable/quickstart/):
 
 ```
 $ pip install vessim
 ```
 
 
 ## 🚀 Getting started
 
-Vessim uses [Mosaik](https://mosaik.offis.de/) for co-simulation.
-To run the example scenario, clone the repository (including all examples) and set up your environment via:
+To execute our exemplary co-simulation scenario, run:
 
 ```
-$ pip install -e .
+$ python examples/cosim_example.py
 ```
 
-To execute the fully simulated example scenario, run:
+
+### Software-in-the-Loop Simulation
+
+Software-in-the-Loop (SiL) allows Vessim to interact with real computing systems.
+There is not yet good documentation on how to set up a full SiL scenario, but you can play with the existing
+functionality by installing 
+
 ```
-$ python examples/scenario_1.py
+pip install vessim[sil]
 ```
 
+and running:
+
+```
+$ python examples/cosim_sil_example.py
+```
 
-# Development
 
-Install the requirements in a virtual environment:
+### Vessim Base Components
+
+We are still working on examples for the base modules such as `CarbonApi` or `Generator` which can be used directly
+without the use of Mosaik to support simple experiments that do not require the entire co-simulation engine to run.
+
+Documentation and API are in progress.
+
+
+## 🏗️ Development
+
+Install Vessim with the `dev` option in a virtual environment:
 
 ```
-python3 -m venv venv              # create venv
-. venv/bin/activate               # activate venv
-pip3 install -r requirements.txt  # install dependencies
+python -m venv venv                # create venv
+. venv/bin/activate                # activate venv
+pip install ".[sil,dev,analysis]"  # install dependencies
 ```
 
-Install & start docker `systemctl start docker`
+
+## 📖 Publications
+
+If you use Vessim in your research, please cite our vision paper:
+
+- Philipp Wiesner, Ilja Behnke and Odej Kao. "[A Testbed for Carbon-Aware Applications and Systems](https://arxiv.org/pdf/2306.09774.pdf)" arXiv:2302.08681 [cs.DC]. 2023.
+
+Bibtex:
+```
+@misc{vessim2023,
+    title={A Testbed for Carbon-Aware Applications and Systems}, 
+    author={Wiesner, Philipp and Behnke, Ilja and Kao, Odej},
+    year={2023},
+    eprint={2306.09774},
+    archivePrefix={arXiv},
+    primaryClass={cs.DC}
+}
+```
```

### Comparing `vessim-0.0.3/examples/sil/carbon-aware_control_unit/carbon_aware_control_unit.py` & `vessim-0.1.0/examples/sil/carbon-aware_control_unit/carbon_aware_control_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import time
 from vessim.sil.http_client import HTTPClient
-import simpy
-from typing import Dict
+from vessim.sil.stoppable_thread import StoppableThread
+from threading import Thread
+from typing import Dict, Optional
 
 
 class RemoteBattery:
     """Initializes a battery instance that holds info of the remote battery.
 
     Args:
         soc: The initial state of the battery's state of charge in %.
@@ -37,84 +39,88 @@
             manages, with node IDs as keys and node objects as values.
 
     Attributes:
         power_modes: The list of available power modes for the nodes.
         nodes: A dictionary representing the nodes that the Control
             Unit manages, with node IDs as keys and node objects as values.
         client: The HTTPClient object used to communicate with the server.
-        env: The SimPy environment used to simulate the Control Unit's behavior.
     """
 
     def __init__(self, server_address: str, nodes: dict) -> None:
-        self.power_modes = ['power-saving', 'normal', 'high performance']
+        self.power_modes = ["power-saving", "normal", "high performance"]
         self.nodes = nodes
-
         self.client = HTTPClient(server_address)
 
-        self.env = simpy.Environment()
-        self.env.process(self.scenario())
-
-
-    def run_scenario(self, until: int):
-        self.env.run(until=until)
-
+        self.battery = RemoteBattery()
+        self.ci = 0.0
+        self.solar = 0.0
+
+    def run_scenario(self, until: int, rt_factor: float, update_interval: Optional[float]):
+        if update_interval is None:
+            update_interval = rt_factor
+        update_thread = StoppableThread(self._update_getter, update_interval)
+        update_thread.start()
+
+        for current_time in range(until):
+            self.scenario_step(current_time)
+            time.sleep(rt_factor)
+
+        update_thread.stop()
+        update_thread.join()
+
+    def _update_getter(self) -> None:
+        self.battery.soc = self.client.get("/api/battery-soc")["battery_soc"]
+        self.solar = self.client.get("/api/solar")["solar"]
+        self.ci = self.client.get("/api/ci")["ci"]
 
-    def scenario(self):
+    def scenario_step(self, current_time) -> None:
         """A Carbon-Aware Scenario.
 
-        A SimPy process that runs the main control loop for the Carbon-Aware
-        Control Unit. This process updates the Control Unit's values, sets the
-        battery's minimum state of charge (SOC) based on the current time, and
-        adjusts the power modes of the nodes based on the current carbon
-        intensity and battery SOC.
+        Scenario step for the Carbon-Aware Control Unit. This process updates
+        the Control Unit's values, sets the battery's minimum state of charge
+        (SOC) based on the current time, and adjusts the power modes of the
+        nodes based on the current carbon intensity and battery SOC.
 
-        Yields:
-            A SimPy timeout event that delays the process by one unit of time.
+        Args:
+            current_time: Current simulation time.
         """
-        battery = RemoteBattery(soc=self.client.get('/battery-soc')['battery_soc'])
-        solar = self.client.get('/solar')['solar']
-        ci = self.client.get('/ci')['ci']
         nodes_power_mode = {}
 
         # Set the minimum SOC of the battery based on the current time
-        if self.env.now < 60*36:
-            battery.min_soc = 0.3
+        if current_time < 60*36:
+            self.battery.min_soc = 0.3
         else:
-            battery.min_soc = 0.6
+            self.battery.min_soc = 0.6
 
         # Adjust the power modes of the nodes based on the current carbon intensity and battery SOC
-        if ci <= 200 or battery.soc > 0.8:
-            nodes_power_mode[self.nodes['aws']] = 'high performance'
-            nodes_power_mode[self.nodes['raspi']] = 'high performance'
-        elif ci >= 250 and battery.soc < battery.min_soc:
-            nodes_power_mode[self.nodes['aws']] = 'power-saving'
-            nodes_power_mode[self.nodes['raspi']] = 'power-saving'
+        if self.ci <= 200 or self.battery.soc > 0.8:
+            nodes_power_mode[self.nodes["aws"]] = "high performance"
+            nodes_power_mode[self.nodes["raspi"]] = "high performance"
+        elif self.ci >= 250 and self.battery.soc < self.battery.min_soc:
+            nodes_power_mode[self.nodes["aws"]] = "power-saving"
+            nodes_power_mode[self.nodes["raspi"]] = "power-saving"
         else:
-            nodes_power_mode[self.nodes['aws']] = 'normal'
-            nodes_power_mode[self.nodes['raspi']] = 'normal'
-
-        # Delay the process by one unit of time
-        self.send_battery(battery)
-        self.send_nodes_power_mode(nodes_power_mode)
+            nodes_power_mode[self.nodes["aws"]] = "normal"
+            nodes_power_mode[self.nodes["raspi"]] = "normal"
 
-        yield self.env.timeout(1)
+        # Send and forget
+        Thread(target=self.send_battery, args=(self.battery,)).start()
+        Thread(target=self.send_nodes_power_mode, args=(nodes_power_mode,)).start()
 
-
-    def send_battery(self, battery: Battery) -> None:
+    def send_battery(self, battery: RemoteBattery) -> None:
         """Sends battery data to the VES API.
 
         Args:
             battery: An object containing the battery data to be sent.
         """
-        self.client.put('/ves/battery', {'min_soc': battery.min_soc, 'grid_charge': battery.grid_charge})
-
+        self.client.put("/ves/battery", {"min_soc": battery.min_soc, "grid_charge": battery.grid_charge})
 
     def send_nodes_power_mode(self, nodes_power_mode: Dict[int, str]) -> None:
         """Sends power mode data for nodes to the VES API.
 
         Args:
             nodes_power_mode: A dictionary containing node IDs as keys and
                 their respective power modes as values.
 
         """
         for node_id, power_mode in nodes_power_mode.items():
-            self.client.put(f'/ves/nodes/{node_id}', {'power_mode': power_mode})
+            self.client.put(f"/ves/nodes/{node_id}", {"power_mode": power_mode})
```

### Comparing `vessim-0.0.3/examples/sil/carbon-aware_control_unit/main.py` & `vessim-0.1.0/examples/sil/carbon-aware_control_unit/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import argparse
 import json
 from carbon_aware_control_unit import CarbonAwareControlUnit
 
 
 def argparser() -> argparse.ArgumentParser:
-    # TODO add description=''
+    # TODO add description=""
     parser = argparse.ArgumentParser()
 
-    parser.add_argument('--server_address',
-                        help='address of the API server',
-                        default='http://127.0.0.1:8000')
-
-    parser.add_argument('--nodes',
-                        metavar='JSON e.g. {"aws": 0, "raspi": 1}',
-                        help='names and ids of nodes',
+    parser.add_argument("--nodes",
+                        metavar="JSON e.g. {'aws': 0, 'raspi': 1}",
+                        help="names and ids of nodes",
                         required=True)
 
-    parser.add_argument('--until',
-                        help='duration of the scenario',
-                        default='100')
+    parser.add_argument("--until",
+                        help="duration of the scenario",
+                        required=True)
 
-    return parser
+    parser.add_argument("--server_address",
+                        help="address of the API server",
+                        default="http://127.0.0.1:8000")
+
+    parser.add_argument("--rt_factor",
+                        help="real time factor of the simulation e.g \
+                             rt_factor=1/60 means the cacu run 60x faster as wall \
+                             clock time",
+                        default=1/60)
+
+    parser.add_argument("--update_interval",
+                        help="update interval of the getter methods. defaults \
+                             to rt_factor",
+                        defaul=None)
 
+    return parser
 
-if __name__ == '__main__':
 
+if __name__ == "__main__":
     parser = argparser()
     args = parser.parse_args()
     nodes = json.loads(args.nodes)
 
     cacu = CarbonAwareControlUnit(args.server_address, nodes)
-    cacu.run_scenario(args.until)
+    cacu.run_scenario(args.until, args.rt_factor, args.update_interval)
```

### Comparing `vessim-0.0.3/examples/sil/example_node/README.md` & `vessim-0.1.0/examples/sil/example_node/README.md`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/examples/sil/example_node/node_api_server.py` & `vessim-0.1.0/examples/sil/example_node/node_api_server.py`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/examples/sil/example_node/rpi/init.sh` & `vessim-0.1.0/examples/sil/example_node/rpi/init.sh`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/examples/sil/example_node/rpi/lib/pi_controller.py` & `vessim-0.1.0/examples/sil/example_node/rpi/lib/pi_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from cpufreq import cpuFreq
-from ina219 import INA219
+from cpufreq import cpuFreq # type: ignore
+from ina219 import INA219 # type: ignore
 import psutil
 
 
 class PiController:
     """This class represents a controller for the Raspberry Pi system.
 
     For providing information and control about power and CPU usage of
```

### Comparing `vessim-0.0.3/examples/sil/example_node/rpi/rpi_api_server.py` & `vessim-0.1.0/examples/sil/example_node/rpi/rpi_api_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 sys.path.append("../")
 from node_api_server import FastApiServer
-from lib.pi_controller import PiController
+from pi_controller import PiController
 
 class RpiNodeApiServer(FastApiServer):
     """A Raspberry Pi node API server, extending the base FastApiServer class.
 
     Args:
         host: The host on which to run the FastAPI application.
         port: The port on which to run the FastAPI application.
```

### Comparing `vessim-0.0.3/examples/sil/example_node/virtual_node/linear_power_model.py` & `vessim-0.1.0/examples/sil/example_node/virtual_node/linear_power_model.py`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/examples/sil/example_node/virtual_node/v_node_api_server.py` & `vessim-0.1.0/examples/sil/example_node/virtual_node/v_node_api_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from typing import Union
 sys.path.append("../")
 from linear_power_model import LinearPowerModel
 from node_api_server import FastApiServer
 import subprocess
 import multiprocessing
 import psutil
 import re
@@ -40,15 +41,15 @@
 
     def get_power(self) -> float:
         """Get the power usage of the virtual node.
 
         Returns:
             The current power usage.
         """
-        return self.power_model(psutil.cpu_percent(1))
+        return self.power_model(psutil.cpu_percent(1)) / 1000
 
     def _restart_sysbench(self, run_forever: bool = False) -> None:
         """Kill the existing sysbench instance and start a new one.
 
         Args:
             run_forever: Whether the sysbench should run indefinitely (1 year).
                 Defaults to False.
@@ -66,15 +67,15 @@
                          else list(self.power_config.keys())[0])
             command.append(f"--rate={self.power_config[power_mode]}")
         if run_forever:
             # 1 year
             command.append("--time=31622400")
 
         # Start the new sysbench process
-        self.sysbench = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+        self.sysbench = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True) # type: ignore
 
     def _run_benchmark(self) -> None:
         """Run a sysbench benchmark.
 
         Obtain the cpu metric "events/s" in high performance mode to scale the
         target rate of the other power modes and achieve approximately linear
         CPU utilisation and save in `self.power_config`.
```

### Comparing `vessim-0.0.3/examples/sil/tf_gcp_node/.gitignore` & `vessim-0.1.0/examples/sil/tf_gcp_node/.gitignore`

 * *Files 22% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 terraform.rc
 
 # Ignore sensitive files
 *.pem
 *.key
 *.pub
 /keys
+.ssh
 
 # Ignore crash log files
 crash.log
 
 # Ignore provider-specific files
 # Replace "PROVIDER_NAME" with the actual provider name, e.g., "aws", "azure", etc.
 # Uncomment the relevant line if you're using a specific provider.
```

### Comparing `vessim-0.0.3/examples/sil/tf_gcp_node/README.md` & `vessim-0.1.0/examples/sil/tf_gcp_node/README.md`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/examples/sil/tf_gcp_node/main.tf` & `vessim-0.1.0/examples/sil/tf_gcp_node/main.tf`

 * *Files 22% similar despite different names*

```diff
@@ -24,38 +24,25 @@
       nat_ip = google_compute_address.external.address
     }
   }
 
   metadata_startup_script = <<SCRIPT
     #!/bin/bash
 
-    server_dir=/home/${local.user}/api_server
-    mkdir -p $server_dir
-    chown -R ${local.user}:${local.user} $server_dir
-
-    until [ -d $server_dir/virtual_node ]; do
-      sleep 1
-    done
-
     apt-get update
-    apt-get install python3-pip sysbench -y
-    cd $server_dir/virtual_node
+    apt-get install python3-pip git sysbench -y
+    cd /opt
+    git clone --depth 1 https://github.com/dos-group/vessim.git
+    cp -r vessim/examples/sil/example_node vessim_node_api_server
+    rm -rf vessim
+    cd vessim_node_api_server/virtual_node
     pip3 install -r requirements.txt
     python3 v_node_api_server.py
-SCRIPT
 
-  provisioner "file" {
-    source      = "../example_node/"
-    destination = "api_server"
-    connection {
-      host = google_compute_address.external.address
-      user = local.user
-      private_key = local_file.ssh_private_key_pem.content
-    }
-  }
+SCRIPT
 }
 
 ### network
 
 resource "google_compute_network" "vpc_network" {
   name = "node-vpc"
 }
```

#### html2text {}

```diff
@@ -2,25 +2,22 @@
 ### node resource "google_compute_instance" "node" { name = "node" machine_type
 = var.machine_type tags = ["allow-ssh", "allow-http", "allow-icmp"] metadata =
 { ssh-keys = "${local.user}:${tls_private_key.ssh.public_key_openssh}" }
 boot_disk { initialize_params { image = "ubuntu-2204-jammy-v20221206" } }
 network_interface { network = google_compute_network.vpc_network.name
 access_config { nat_ip = google_compute_address.external.address } }
 metadata_startup_script = <
-!/bin/bash server_dir=/home/${local.user}/api_server mkdir -p $server_dir chown
--R ${local.user}:${local.user} $server_dir until [ -d $server_dir/virtual_node
-]; do sleep 1 done apt-get update apt-get install python3-pip sysbench -y cd
-$server_dir/virtual_node pip3 install -r requirements.txt python3
-v_node_api_server.py SCRIPT provisioner "file" { source = "../example_node/
-" destination = "api_server" connection { host =
-google_compute_address.external.address user = local.user private_key =
-local_file.ssh_private_key_pem.content } } } ### network resource
-"google_compute_network" "vpc_network" { name = "node-vpc" } resource
-"google_compute_address" "external" { name = "node-external" } resource
-"google_compute_firewall" "allow_ssh" { name = "allow-ssh" network =
+!/bin/bash apt-get update apt-get install python3-pip git sysbench -y cd /opt
+git clone --depth 1 https://github.com/dos-group/vessim.git cp -r vessim/
+examples/sil/example_node vessim_node_api_server rm -rf vessim cd
+vessim_node_api_server/virtual_node pip3 install -r requirements.txt python3
+v_node_api_server.py SCRIPT } ### network resource "google_compute_network"
+"vpc_network" { name = "node-vpc" } resource "google_compute_address"
+"external" { name = "node-external" } resource "google_compute_firewall"
+"allow_ssh" { name = "allow-ssh" network =
 google_compute_network.vpc_network.name target_tags = ["allow-ssh"]
 source_ranges = ["0.0.0.0/0"] allow { protocol = "tcp" ports = ["22"] } }
 resource "google_compute_firewall" "allow_http" { name = "allow-http" network =
 google_compute_network.vpc_network.name target_tags = ["allow-http"]
 source_ranges = ["0.0.0.0/0"] allow { protocol = "tcp" ports = ["80", "8000"] }
 } resource "google_compute_firewall" "allow_icmp" { name = "allow-icmp" network
 = google_compute_network.vpc_network.name allow { protocol = "icmp" }
```

### Comparing `vessim-0.0.3/examples/sil/tf_gcp_node/variables.tf` & `vessim-0.1.0/examples/sil/tf_gcp_node/variables.tf`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/experimental/custom.json` & `vessim-0.1.0/experimental/custom.json`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/experimental/pp_scenario.py` & `vessim-0.1.0/experimental/pp_scenario.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pandapower as pp
+import pandapower as pp # type: ignore
 
 # create empty net
 import pandas as pd
 
 net = pp.create_empty_network(f_hz=50.0)
 
 # create buses
```

### Comparing `vessim-0.0.3/pyproject.toml` & `vessim-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,65 @@
 [project]
 name = "vessim"
 dynamic = ["version", "description"]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["simulation", "energy system", "testbed", "carbon-aware"]
 authors = [{name = "Philipp Wiesner", email = "wiesner@tu-berlin.de"}]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Topic :: Scientific/Engineering",
   "Topic :: Software Development :: Testing",
   "Topic :: Education",
   "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
-dependencies = [ # Optional
+dependencies = [
   "pandas",
   "mosaik",
   "mosaik-api",
+  "loguru",  # TODO shall we remove this?
+]
+
+[project.optional-dependencies]
+sil = [
+  "requests",
+  "fastapi",
+  "docker",
+  "uvicorn",
+]
+dev = [
+  # testing
+  "pytest",
+  # typechecking
+  "mypy",
+  "types-psutil",
+  "pandas-stubs",
+  "types-requests",
+  # linting
+  "black",
+  "ruff",
+  # build
+  "flit",
+]
+analysis = [
+  "jupyterlab",
+  "matplotlib",
+  "seaborn==0.12.2",
 ]
 
-# [project.optional-dependencies] # Optional
-# dev = ["check-manifest"]
-# test = ["coverage"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/dos-group/vessim"
 "Source" = "https://github.com/dos-group/vessim"
 "Bug Reports" = "https://github.com/dos-group/vessim/issues"
 
 # The following would provide a command line executable called `sample`
@@ -44,45 +70,51 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.sdist]
 exclude = ["data"]
 
+[tool.flit.module]
+name = "vessim"
 
 [tool.black]
 line-length = 90  # Set the maximum characters per line
-target-version = ['py311']  # Set python version that black should format the code for
+target-version = ['py38']   # Set python versions that black should format the code for
 include = '\.py$'  # Format only python files
 
-
 [tool.ruff]
-# Enable Ruff to check for docstring-related (D), pycodestyle-related (E, W), and Pyflakes-related (F) issues
-select = ["D", "E", "F", "W"]
+# Enable Ruff to check for issues (https://beta.ruff.rs/docs/rules)
+select = [
+  "E", "W",  # pycodestyle (error and warning)
+  "D",  # docstrings
+  "F",  # Pyflakes
+  "N",  # variable naming
+  #  "B",  # flake8-bugbear
+]
 
 # For now the following rules are disabled:
 #   D100: Missing docstring in public module
 #   D101: Missing docstring in public class
 #   D102: Missing docstring in public method
 #   D103: Missing docstring in public function
 #   D107: Missing docstring in __init__
-#   F401: Imported but unused
-ignore = ["D100", "D101", "D102", "D103", "D107", "F401"]
+ignore = ["D100", "D101", "D102", "D103", "D107"]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["D", "E", "W"]
 unfixable = ["F"]
 
 line-length = 90  # Set the maximum characters per line (similar to black)
-target-version = "py311"  # Set python version for linting (similar to black)
+target-version = "py38"  # Set python version for linting (similar to black)
 include = ["*.py"]  # Only enable linting for python files (similar to black)
 
 # Exclude specific directories and all defaults
 extend-exclude = ["example_node", "simulator/power_meter.py", "carbon-aware_control_unit"]
 
 # Configure Ruff to enforce Google-style docstrings when checking documentation
 [tool.ruff.pydocstyle]
 convention = "google"
 
-
+# Configure mypy to ignore missing imports
 [mypy]
 ignore_missing_imports = true
```

### Comparing `vessim-0.0.3/tests/test_carbon_api.py` & `vessim-0.1.0/tests/test_carbon_api.py`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/tests/test_storage.py` & `vessim-0.1.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/vessim/core/simulator.py` & `vessim-0.1.0/vessim/core/simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from abc import ABC
-from typing import Union
 from datetime import datetime
-from typing import List, Optional
+from typing import Union, List, Optional
 
 import pandas as pd
 
-
 Time = Union[int, float, str, datetime]
 
 
 class TraceSimulator(ABC):
 
     def __init__(self, data: Union[pd.Series, pd.DataFrame]):
         self.data = data
 
     def next_update(self, dt: Time):
+        """Returns the next time of when the trace will change.
+
+        This method is being called in the time-based simulation model for Mosaik.
+        """
         current_index = self.data.index.asof(dt)
         next_iloc = self.data.index.get_loc(current_index) + 1
         return self.data.index[next_iloc]
 
 
 class CarbonApi(TraceSimulator):
     def __init__(self, data: pd.DataFrame, unit: str = "g_per_kWh"):
@@ -58,25 +60,15 @@
             raise ValueError(f"Cannot retrieve carbon intensity at zone '{zone}'.")
         try:
             return zone_carbon_intensity.loc[self.data.index.asof(dt)]
         except KeyError:
             raise ValueError(f"Cannot retrieve carbon intensity at {dt} in zone "
                              f"'{zone}'.")
 
-    def next_update(self, dt: Time):
-        """Returns the next time of when the carbon intensity will change.
-
-        This method is being called in the time-based simulation model for Mosaik.
-        """
-        current_index = self.data.index.asof(dt)
-        next_iloc = self.data.index.get_loc(current_index) + 1
-        return self.data.iloc[next_iloc].name
-
 
 class Generator(TraceSimulator):
 
     def power_at(self, dt: Time):
         try:
             return self.data.loc[self.data.index.asof(dt)]
         except KeyError:
             raise ValueError(f"Cannot retrieve power at {dt}.")
-
```

### Comparing `vessim-0.0.3/vessim/core/storage.py` & `vessim-0.1.0/vessim/core/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
         Returns:
             The power delta, in case not all requested power could be discharged from or
             charged into the battery. This can happen either if the batter is full/empty
             or if the C-rate was exceeded.
             If 0, all power was successfully (dis)charged.
         """
 
+    @abstractmethod
+    def soc(self) -> float:
+        """Returns the current State of Charge (SoC)."""
+
 
 class SimpleBattery(Storage):
     """(Way too) simple battery.
 
     Args:
         capacity: Battery capacity in Ws
         charge_level: Initial charge level in Ws
@@ -41,27 +45,27 @@
         assert 0 <= charge_level <= self.capacity
         self.charge_level = charge_level
         assert 0 <= min_soc <= self.soc()
         self.min_soc = min_soc
         self.c_rate = c_rate
 
     def update(self, power: float, duration: int) -> float:
-        max_charge_p_delta, p_delta = 0, 0
+        max_charge_p_delta, p_delta = 0.0, 0.0
 
         if self.c_rate is not None:
             max_rate = self.c_rate * self.capacity / 3600
             if power >= max_rate:
-                logger.info(f"Trying to charge storage '{__class__.__name__}' with "
+                logger.info(f"Trying to charge storage '{self.__class__.__name__}' with "
                             f"{power} W but only {max_rate} W are supported.")
                 max_charge_p_delta = power - max_rate
                 power = max_rate
 
             if power <= -max_rate:
-                logger.info(f"Trying to discharge storage '{__class__.__name__}' with "
-                            f"{power} W but only {max_rate} W are supported.")
+                logger.info(f"Trying to discharge storage '{self.__class__.__name__}' "
+                            f"with {power} W but only {max_rate} W are supported.")
                 max_charge_p_delta = power + max_rate
                 power = -self.c_rate
 
         charge_energy = power * duration
         new_charge_level = self.charge_level + power * duration
 
         abs_min_soc = self.min_soc * self.capacity
@@ -72,15 +76,15 @@
             p_delta = (new_charge_level - self.capacity) / duration
             self.charge_level = self.capacity
         else:
             self.charge_level += charge_energy
 
         return p_delta + max_charge_p_delta
 
-    def soc(self):
+    def soc(self) -> float:
         return self.charge_level / self.capacity
 
 
 class StoragePolicy(ABC):
 
     @abstractmethod
     def apply(self, storage: Storage, p_delta: float, time_since_last_step: int) -> float:
```

### Comparing `vessim-0.0.3/vessim/cosim/_util.py` & `vessim-0.1.0/vessim/cosim/_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
 from typing import Type, Dict, Any, Union
 
-import mosaik_api
+import mosaik_api  # type: ignore
 import pandas as pd
 
 
 class VessimModel:
 
     @abstractmethod
     def step(self, time: int, inputs: dict) -> None:
@@ -41,17 +41,17 @@
             meta: A dictionary that describes the simulator's metadata.
             model_class: The class of the model to be simulated. Model requires
                 step() method with no args (must only utilize object
                 attributes). Alternatively, the step() method of this class
                 must be overwritten and implemented individually.
         """
         super().__init__(meta)
-        self.eid_prefix = list(self.meta["models"])[0] + "_"  # type: ignore
+        self.eid_prefix = list(self.meta["models"])[0] + "_"
         self.model_class = model_class
-        self.entities: Dict[int, VessimModel] = {}
+        self.entities: Dict[str, VessimModel] = {}
         self.time = 0
 
     def init(self, sid, time_resolution, eid_prefix=None):
         """Initialize Simulator and set `step_size` and `eid_prefix`."""
         if float(time_resolution) != 1.0:
             raise ValueError(
                 f"{self.__class__.__name__} only supports time_resolution=1., "
@@ -72,67 +72,53 @@
             self.entities[eid] = entity
             entities.append({"eid": eid, "type": model})
         return entities
 
     def step(self, time, inputs, max_advance):
         """Set all `inputs` attr values to the `entity` attrs, then step the `entity`."""
         self.time = time
-        input_mapping = {eid: _convert_inputs(attrs) for eid, attrs in inputs.items()}
         for eid, entity in self.entities.items():
-            entity.step(time, input_mapping.get(eid, {}))
+            entity.step(time, inputs.get(eid, {}))
         return self.next_step(time)
 
     @abstractmethod
     def next_step(self, time):
         """Return time of next simulation step (None for event-based)."""
 
     def get_data(self, outputs):
         """Return all requested data as attr from the `model_instance`."""
         data = {}
-        model_name = list(self.meta["models"])[0]  # type: ignore
+        model_name = list(self.meta["models"])[0]
         for eid, attrs in outputs.items():
             model = self.entities[eid]
             data["time"] = self.time
             data[eid] = {}
             for attr in attrs:
-                if attr not in self.meta["models"][model_name]["attrs"]:  # type: ignore
+                if attr not in self.meta["models"][model_name]["attrs"]:
                     raise ValueError(f"Unknown output attribute: {attr}")
                 if hasattr(model, attr):
                     data[eid][attr] = getattr(model, attr)
         return data
 
 
-def _convert_inputs(
-    attrs: dict[str, dict[str, Any]]
-) -> dict[str, Union[Any, list[Any]]]:
-    """Converts Mosaik step inputs into a simpler format suitable for Vessim.
-
-    If there is a single input, only the input is being returned.
-    If there are multiple inputs, they are returned as a list.
-
-    Examples:
-        >>> _convert_inputs({'p': {'ComputingSystem-0.ComputingSystem_0': -50})
-        -50
-
-        >>> _convert_inputs({'p': {'ComputingSystem-0.ComputingSystem_0': -50,
-        >>>                        'Generator-0.Generator_0': 12})
-        [-50, 12]
-    """
-    result = {}
-    for key, val_dict in attrs.items():
-        values = list(val_dict.values())
-        if len(values) == 1:
-            result[key] = values[0]
-        else:
-            result[key] = values
-    return result
-
-
 class Clock:
     def __init__(self, sim_start: Union[str, datetime]):
         self.sim_start = pd.to_datetime(sim_start)
 
     def to_datetime(self, simtime: int) -> datetime:
         return self.sim_start + timedelta(seconds=simtime)
 
     def to_simtime(self, dt: datetime) -> int:
-        return (dt - self.sim_start).seconds
+        return int((dt - self.sim_start).total_seconds())
+
+
+def simplify_inputs(attrs: Dict[str, Dict[str, Any]]) -> Dict[str, Any]:
+    """Removes Mosaik source entity from input dict.
+
+    Examples:
+        >>> simplify_inputs({'p': {'ComputingSystem-0.ComputingSystem_0': -50}})
+        {'p': -50}
+    """
+    result = {}
+    for key, val_dict in attrs.items():
+        result[key] = list(val_dict.values())[0]
+    return result
```

### Comparing `vessim-0.0.3/vessim/cosim/carbon_api.py` & `vessim-0.1.0/vessim/cosim/carbon_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 
     def __init__(self):
         super().__init__(self.META, _CarbonApiModel)
         self.clock = None
         self.sim_start = None
         self.carbon_api = None
 
-    def init(self, sid, time_resolution, sim_start: datetime, carbon_api: CarbonApi,
-             eid_prefix=None):
+    def init(self, sid, time_resolution, sim_start: datetime, # type: ignore
+            carbon_api: CarbonApi, eid_prefix=None):
         super().init(sid, time_resolution, eid_prefix=eid_prefix)
         self.clock = Clock(sim_start)
         self.carbon_api = carbon_api
         return self.meta
 
-    def create(self, num, model, zone: str):
-        return super().create(num, model, zone=zone, clock=self.clock,
+    def create(self, num, model, *args, **kwargs):
+        return super().create(num, model, *args, **kwargs, clock=self.clock,
                               carbon_api=self.carbon_api)
 
     def next_step(self, time: int) -> int:
         dt = self.clock.to_datetime(time)
         next_dt = self.carbon_api.next_update(dt)
         return self.clock.to_simtime(next_dt)
 
 
 class _CarbonApiModel(VessimModel):
     def __init__(self, carbon_api: CarbonApi, clock: Clock, zone: str):
         self.api = carbon_api
         self.clock = clock
         self.zone = zone
-        self.carbon_intensity = None
+        self.carbon_intensity = 0.0
 
     def step(self, time: int, inputs: dict) -> None:
         dt = self.clock.to_datetime(time)
         self.carbon_intensity = self.api.carbon_intensity_at(dt, self.zone)
```

### Comparing `vessim-0.0.3/vessim/cosim/computing_system.py` & `vessim-0.1.0/vessim/cosim/computing_system.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,21 @@
         self.step_size = None
         super().__init__(self.META, _ComputingSystemModel)
 
     def init(self, sid, time_resolution, step_size, eid_prefix=None):
         self.step_size = step_size
         return super().init(sid, time_resolution, eid_prefix=eid_prefix)
 
+    def finalize(self) -> None:
+        """Stops power meters' threads."""
+        super().finalize()
+        for model_instance in self.entities.values():
+            for power_meter in model_instance.power_meters: # type: ignore
+                power_meter.finalize()
+
     def next_step(self, time):
         return time + self.step_size
 
 
 class _ComputingSystemModel(VessimModel):
     """Model of the computing system.
 
@@ -49,8 +56,8 @@
 
     def step(self, time: int, inputs: dict) -> None:
         """Updates the power consumption of the system.
 
         The power consumption is calculated as the product of the PUE and the
         sum of the node power of all power meters.
         """
-        self.p = self.pue * sum(pm.measure() for pm in self.power_meters)
+        self.p = -self.pue * sum(pm.measure() for pm in self.power_meters)
```

### Comparing `vessim-0.0.3/vessim/cosim/monitor.py` & `vessim-0.1.0/vessim/cosim/monitor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 from collections import defaultdict
 from datetime import datetime
 from typing import Dict, Callable, Any
 
-import mosaik_api
 import pandas as pd
 from loguru import logger
 
-from vessim.cosim._util import Clock
+from vessim.cosim._util import Clock, VessimSimulator, VessimModel, simplify_inputs
 
 
-class MonitorSim(mosaik_api.Simulator):  # TODO Make time based
-    """Simple data collector for printing data at the end of simulation.
-
-    Attributes:
-        eid: Identifier of Simulator Instance
-        data: Dictionary for holding the necessary simulation data
-    """
+class MonitorSim(VessimSimulator):
 
     META = {
-        "type": "event-based",
+        "type": "time-based",
         "models": {
             "Monitor": {
                 "public": True,
                 "any_inputs": True,
-                "params": ["fn", "sim_start"],
+                "params": ["out_path", "fn"],
                 "attrs": [],
             },
         },
     }
 
-    def __init__(self):
-        super().__init__(self.META)
-        self.eid = None
-        self.data = defaultdict(dict)
-        self.fn = None
-        self._clock = None
+    def __init__(self) -> None:
+        """Simple data collector for printing data at the end of simulation."""
+        self.step_size = None
+        self.clock = None
+        super().__init__(self.META, _MonitorModel)
+
+    def init(self, sid, time_resolution, sim_start: datetime,  # type: ignore
+             step_size: int, eid_prefix=None):
+        self.step_size = step_size  # type: ignore
+        self.clock = Clock(sim_start)  # type: ignore
+        return super().init(sid, time_resolution, eid_prefix=eid_prefix)
 
-    def init(self, sid, time_resolution):
-        return self.meta
+    def create(self, num, model, *args, **kwargs):  # type: ignore
+        return super().create(num, model, *args, **kwargs, clock=self.clock)
 
-    def create(self, num, model, fn: Callable[[], Dict[str, Any]], sim_start: datetime):
-        self.fn = fn
-        self._clock = Clock(sim_start)
-        if num > 1 or self.eid is not None:
-            raise RuntimeError("Can only create one instance of Monitor.")
+    def finalize(self):
+        """Collected data is printed to file at simulation end."""
+        for model in self.entities.values():
+            model: _MonitorModel
+            model.finalize()
+
+    def next_step(self, time):
+        return time + self.step_size
 
-        self.eid = "Monitor"
-        return [{"eid": self.eid, "type": model}]
 
-    def step(self, time, inputs, max_advance):
+class _MonitorModel(VessimModel):
+    def __init__(self, out_path: str, fn: Callable[[], Dict[str, Any]], clock: Clock):
+        self.out_path = out_path
+        self.fn = fn
+        self._clock = clock
+        self.data: Dict = defaultdict(dict)
+
+    def step(self, time: int, inputs: Dict) -> None:
+        inputs = simplify_inputs(inputs)
         dt = self._clock.to_datetime(time)
-        data = inputs.get(self.eid, {})
         logger.info(f"# --- {str(dt):>5} ---")
-        for attr, values in data.items():
-            for src, value in values.items():
-                logger.info(f"{attr}: {value}")
-                self.data[attr][dt] = value
+        for attr, value in inputs.items():
+            logger.info(f"{attr}: {value}")
+            self.data[attr][dt] = value
         if self.fn is not None:
             for attr, value in self.fn().items():
                 logger.info(f"{attr}: {value}")
                 self.data[attr][dt] = value
-        return None
 
     def finalize(self):
         """Collected data is printed to file at simulation end."""
-        pd.DataFrame(self.data).to_csv("data.csv")
+        pd.DataFrame(self.data).to_csv(self.out_path)
```

### Comparing `vessim-0.0.3/vessim/sil/http_client.py` & `vessim-0.1.0/vessim/sil/http_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,17 @@
             HTTPClientError if the data could not be retrieved from route
 
         Returns:
             A dictionary containing the response.
         """
         response = requests.get(self.server_address + route)
         if response.status_code == 200:
-            return response.json() # assuming the response data is in JSON format
+            data = response.json() # assuming the response data is in JSON format
+            print(f'Data received at {route}: {data}')
+            return data
 
         raise HTTPClientError(
             response.status_code,
             f'Failed to retrieve data from {route}'
         )
 
     def put(self, route: str, data: Dict[str, Any]) -> None:
@@ -55,13 +57,14 @@
         headers = {'Content-type': 'application/json'}
         response = requests.put(
             self.server_address + route,
             data=json.dumps(data),
             headers=headers
         )
         if response.status_code == 200:
-            print(f'Data successfully updated at {route}')
+            print(f'Data successfully updated at {route}: {data}')
         else:
             raise HTTPClientError(
                 response.status_code,
                 f'Failed to update data at {route}'
             )
+
```

### Comparing `vessim-0.0.3/vessim/sil/node.py` & `vessim-0.1.0/vessim/sil/node.py`

 * *Files identical despite different names*

### Comparing `vessim-0.0.3/vessim/sil/power_meter.py` & `vessim-0.1.0/vessim/sil/power_meter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import threading
-import time
 from abc import ABC, abstractmethod
 from typing import Optional
 
 from vessim.sil.http_client import HTTPClient
+from vessim.sil.stoppable_thread import StoppableThread
 
 
 class PowerMeter(ABC):
     """Abstract base class for power meters.
 
     Args:
         name: The name of the power meter.
@@ -21,14 +20,18 @@
         """Abstract method to measure and return the current node power demand.
 
         Returns:
             float: The current power demand of the node.
         """
         pass
 
+    @abstractmethod
+    def finalize(self) -> None:
+        pass
+
 
 class HttpPowerMeter(PowerMeter):
     """Power meter for an external node that implements the vessim node API.
 
     This class represents a power meter for an external node. It creates a thread
     that updates the power demand from the node API at a given interval.
 
@@ -37,44 +40,45 @@
         server_address: The IP address of the node API.
         port: The IP port of the node API.
         name: The name of the power meter.
     """
 
     def __init__(
         self,
-        interval: int,
+        interval: float,
         server_address: str,
         port: int = 8000,
         name: Optional[str] = None
     ) -> None:
         super().__init__(name)
         self.http_client = HTTPClient(f"{server_address}:{port}")
-        self.power = 0
-        self.update_thread = threading.Thread(target=self._update_power, args=(interval,))
-        self.update_thread.daemon = True
+        self.power = 0.0
+        self.update_thread = StoppableThread(self._update_power, interval)
         self.update_thread.start()
 
-    def _update_power(self, interval: int) -> None:
+    def _update_power(self) -> None:
         """Gets the power demand every `interval` seconds from the API server."""
-        while True:
-            self.power = float(self.http_client.get("/power"))
-            time.sleep(interval)
+        self.power = float(self.http_client.get("/power")["power"])
 
     def measure(self) -> float:
         """Returns the current power demand of the node."""
         return self.power
 
-    def __del__(self) -> None:
-        """Terminates the power demand update thread when the instance is deleted."""
-        if self.update_thread.is_alive():
-            self.update_thread.join()
+    def finalize(self) -> None:
+        """Terminates the power update thread when the instance is finalized."""
+        self.update_thread.stop()
+        self.update_thread.join()
 
 
 class MockPowerMeter(PowerMeter):
 
     def __init__(self, p: float, name: Optional[str] = None):
         super().__init__(name)
-        assert p <= 0
+        assert p >= 0
         self.p = p
 
     def measure(self) -> float:
         return self.p
+
+    def finalize(self) -> None:
+        pass
+
```

