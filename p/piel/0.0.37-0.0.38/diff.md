# Comparing `tmp/piel-0.0.37.tar.gz` & `tmp/piel-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.37.tar", last modified: Thu Jul  6 07:06:39 2023, max compression
+gzip compressed data, was "piel-0.0.38.tar", last modified: Sat Jul  8 10:21:08 2023, max compression
```

## Comparing `piel-0.0.37.tar` & `piel-0.0.38.tar`

### file list

```diff
@@ -1,171 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-06 07:06:18.000000 piel-0.0.37/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 07:06:18.000000 piel-0.0.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-06 07:06:18.000000 piel-0.0.37/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-06 07:06:39.006881 piel-0.0.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-06 07:06:18.000000 piel-0.0.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-06 07:06:18.000000 piel-0.0.37/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-06 07:06:18.000000 piel-0.0.37/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 07:06:18.000000 piel-0.0.37/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.986880 piel-0.0.37/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.986880 piel-0.0.37/docs/examples/designs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.986880 piel-0.0.37/docs/examples/designs/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.986880 piel-0.0.37/docs/examples/designs/simple_design/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/examples/designs/simple_design/simple_design/tb/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-06 07:06:18.000000 piel-0.0.37/docs/examples/designs/simple_design/simple_design/tb/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/examples/designs/simple_design/simple_design/tb/default/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-06 07:06:18.000000 piel-0.0.37/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-06 07:06:18.000000 piel-0.0.37/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-06 07:06:18.000000 piel-0.0.37/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-06 07:06:18.000000 piel-0.0.37/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.986880 piel-0.0.37/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/about/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/about/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/about/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/codesign/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/codesign/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/components/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/components/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/environment/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/microservices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/microservices/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/dependencies/cocotb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/dependencies/gdsfactory.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/dependencies/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/dependencies/openlane.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/dependencies/sax.rst
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/microservices/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/integration/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/integration/sax_qutip.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/models/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/models/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 07:06:18.000000 piel-0.0.37/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 07:06:18.000000 piel-0.0.37/piel/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 07:06:18.000000 piel-0.0.37/piel/cocotb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-06 07:06:18.000000 piel-0.0.37/piel/cocotb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-06 07:06:18.000000 piel-0.0.37/piel/cocotb/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-06 07:06:18.000000 piel-0.0.37/piel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-06 07:06:18.000000 piel-0.0.37/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-06 07:06:18.000000 piel-0.0.37/piel/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-06 07:06:18.000000 piel-0.0.37/piel/file_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 07:06:18.000000 piel-0.0.37/piel/gdsfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-06 07:06:18.000000 piel-0.0.37/piel/gdsfactory/netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 07:06:18.000000 piel-0.0.37/piel/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-06 07:06:18.000000 piel-0.0.37/piel/integration/openlane_gdsfactory_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-06 07:06:18.000000 piel-0.0.37/piel/integration/sax_cocotb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-06 07:06:18.000000 piel-0.0.37/piel/integration/sax_qutip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/frequency/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/all.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/frequency/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/frequency/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/electro_optic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/electro_optic/ideal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/frequency/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/frequency/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/frequency/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/coupler_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/directional_coupler_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/directional_coupler_real.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/directional_coupler_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/grating_coupler.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/mmi1x2.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/mmi2x2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/straight_waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/electro_optic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/electro_optic/signal_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/photonic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/electrical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/electrical/cable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/electro_optic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/electronic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/electro_optic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/piel/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/piel/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/parse/run_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/parse/sta_rpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-06 07:06:18.000000 piel-0.0.37/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-06 07:06:18.000000 piel-0.0.37/piel/project_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/piel/sax/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 07:06:18.000000 piel-0.0.37/piel/sax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-06 07:06:18.000000 piel-0.0.37/piel/sax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-06 07:06:39.006881 piel-0.0.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-06 07:06:18.000000 piel-0.0.37/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-06 07:06:18.000000 piel-0.0.37/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/tests/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 07:06:18.000000 piel-0.0.37/tests/gdsfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-06 07:06:18.000000 piel-0.0.37/tests/gdsfactory/test_netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.990880 piel-0.0.37/tests/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.990880 piel-0.0.37/tests/models/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/tests/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-06 07:06:18.000000 piel-0.0.37/tests/models/logic/electro_optic/test_signal_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/tests/sax/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-06 07:06:18.000000 piel-0.0.37/tests/sax/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-06 07:06:18.000000 piel-0.0.37/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-08 10:20:52.000000 piel-0.0.38/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 10:20:52.000000 piel-0.0.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-08 10:20:52.000000 piel-0.0.38/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-08 10:21:08.286899 piel-0.0.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-08 10:20:52.000000 piel-0.0.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-08 10:20:52.000000 piel-0.0.38/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/config/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/file_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/file_conversion/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/file_system/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    40591 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/integration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/integration/openlane_gdsfactory_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/integration/sax_cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/integration/sax_cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/integration/sax_qutip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/integration/sax_qutip/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/frequency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/frequency/all/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/all/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/frequency/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/frequency/electro_optic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/frequency/electro_optic/ideal/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/electro_optic/ideal/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.266899 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/coupler_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/coupler_simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/grating_coupler/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/mmi1x2/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/mmi1x2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/mmi2x2/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/mmi2x2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/frequency/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/frequency/utils/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/logic/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/logic/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/logic/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/logic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/logic/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/logic/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/physical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/physical/electrical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/physical/electrical/cable/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/physical/electrical/cable/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/physical/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/physical/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/physical/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/physical/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/physical/electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/physical/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/physical/geometry/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/physical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/physical/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/physical/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/physical/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/physical/thermal/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/physical/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/physical/units/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/transient/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/transient/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/transient/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/transient/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/transient/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/transient/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/transient/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/models/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/project_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/project_structure/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/tools/cocotb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/tools/cocotb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/cocotb/core/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/tools/cocotb/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/cocotb/data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.270899 piel-0.0.38/docs/autoapi/piel/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/gdsfactory/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/gdsfactory/netlist/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28090 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)    18502 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/openlane/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/openlane/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/openlane/migrate/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/openlane/parse/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/openlane/parse/sta_rpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/openlane/parse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/openlane/parse/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/openlane/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/openlane/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/openlane/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/openlane/v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/openlane/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/openlane/v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/sax/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/tools/sax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/tools/sax/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/visual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/visual/auto_plot_multiple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/visual/auto_plot_multiple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/autoapi/piel/visual/data_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/visual/data_conversion/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-08 10:20:52.000000 piel-0.0.38/docs/autoapi/piel/visual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-08 10:20:52.000000 piel-0.0.38/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 10:20:52.000000 piel-0.0.38/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.262899 piel-0.0.38/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.262899 piel-0.0.38/docs/examples/designs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.262899 piel-0.0.38/docs/examples/designs/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.262899 piel-0.0.38/docs/examples/designs/simple_design/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/examples/designs/simple_design/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-08 10:20:52.000000 piel-0.0.38/docs/examples/designs/simple_design/simple_design/tb/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/examples/designs/simple_design/simple_design/tb/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-08 10:20:52.000000 piel-0.0.38/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-08 10:20:52.000000 piel-0.0.38/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-08 10:20:52.000000 piel-0.0.38/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-08 10:20:52.000000 piel-0.0.38/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.262899 piel-0.0.38/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/sections/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/about/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/about/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/sections/codesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/codesign/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/sections/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/environment/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/sections/microservices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/sections/microservices/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/microservices/dependencies/cocotb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/microservices/dependencies/gdsfactory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/microservices/dependencies/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/microservices/dependencies/openlane.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/microservices/dependencies/sax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/microservices/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/sections/microservices/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/microservices/integration/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/microservices/integration/sax_qutip.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/docs/sections/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-08 10:20:52.000000 piel-0.0.38/docs/sections/models/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.274899 piel-0.0.38/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-08 10:20:52.000000 piel-0.0.38/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-08 10:20:52.000000 piel-0.0.38/piel/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-08 10:20:52.000000 piel-0.0.38/piel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-08 10:20:52.000000 piel-0.0.38/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-08 10:20:52.000000 piel-0.0.38/piel/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-08 10:20:52.000000 piel-0.0.38/piel/file_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 10:20:52.000000 piel-0.0.38/piel/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-08 10:20:52.000000 piel-0.0.38/piel/integration/openlane_gdsfactory_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-08 10:20:52.000000 piel-0.0.38/piel/integration/sax_cocotb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-08 10:20:52.000000 piel-0.0.38/piel/integration/sax_qutip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/frequency/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/frequency/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/electro_optic/ideal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/frequency/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/photonic/coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/photonic/directional_coupler_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/photonic/directional_coupler_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/photonic/directional_coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/photonic/grating_coupler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/photonic/mmi1x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/photonic/mmi2x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/photonic/straight_waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/frequency/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/logic/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/logic/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/logic/electro_optic/signal_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/logic/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/logic/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/logic/photonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel/models/physical/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/physical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/physical/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/physical/electrical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/physical/electrical/cable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/physical/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/physical/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/physical/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/physical/electronic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/physical/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/physical/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/physical/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/physical/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/physical/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/transient/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/transient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/transient/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/transient/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/transient/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/transient/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/transient/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/piel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-08 10:20:52.000000 piel-0.0.38/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-08 10:20:52.000000 piel-0.0.38/piel/project_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/tools/cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/cocotb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/cocotb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/cocotb/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/gdsfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/gdsfactory/netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/tools/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/openlane/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/tools/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/openlane/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/openlane/parse/sta_rpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/openlane/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/openlane/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/openlane/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/openlane/v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/sax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-08 10:20:52.000000 piel-0.0.38/piel/tools/sax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/piel/visual/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-08 10:20:52.000000 piel-0.0.38/piel/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-08 10:20:52.000000 piel-0.0.38/piel/visual/auto_plot_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-08 10:20:52.000000 piel-0.0.38/piel/visual/data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.278899 piel-0.0.38/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-08 10:21:08.000000 piel-0.0.38/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-07-08 10:21:08.000000 piel-0.0.38/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 10:21:08.000000 piel-0.0.38/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 10:21:08.000000 piel-0.0.38/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 10:21:08.000000 piel-0.0.38/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-08 10:21:08.000000 piel-0.0.38/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-08 10:21:08.000000 piel-0.0.38/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-08 10:21:08.286899 piel-0.0.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-08 10:20:52.000000 piel-0.0.38/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 10:20:52.000000 piel-0.0.38/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.262899 piel-0.0.38/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.262899 piel-0.0.38/tests/models/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/tests/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-08 10:20:52.000000 piel-0.0.38/tests/models/logic/electro_optic/test_signal_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-08 10:20:52.000000 piel-0.0.38/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/tests/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/tests/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 10:20:52.000000 piel-0.0.38/tests/tools/gdsfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-08 10:20:52.000000 piel-0.0.38/tests/tools/gdsfactory/test_netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/tests/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:20:52.000000 piel-0.0.38/tests/tools/sax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-08 10:20:52.000000 piel-0.0.38/tests/tools/sax/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:21:08.282899 piel-0.0.38/tests/visual/
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-08 10:20:52.000000 piel-0.0.38/tests/visual/test_data_conversion.py
```

### Comparing `piel-0.0.37/CONTRIBUTING.rst` & `piel-0.0.38/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/LICENSE` & `piel-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/PKG-INFO` & `piel-0.0.38/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.37
+Version: 0.0.38
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -36,19 +36,27 @@
 * System interconnection modelling in multiple environments.
 * Individual and interposer design integration.
 * Multi-domain electronics and photonics component models.
 * Quantum models of physical circuitry
 
 `piel` aims to provide an integrated workflow to co-design photonics and electronics, classically and quantum. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
 
+## Examples
+
+Follow the many [examples in the documentation](https://piel.readthedocs.io/en/stable/examples.html).
+
 ## Microservices Toolset
 This package provides interconnection functions to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some existing microservice dependency integrations are:
 * [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 * [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
 * [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
 * [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 * [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in Python
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
+
+
+## Contribution
+If you feel dedicated enough to become a project maintainer, or just want to do a single contributor, let's do this together!
```

### Comparing `piel-0.0.37/README.md` & `piel-0.0.38/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,19 +14,27 @@
 * System interconnection modelling in multiple environments.
 * Individual and interposer design integration.
 * Multi-domain electronics and photonics component models.
 * Quantum models of physical circuitry
 
 `piel` aims to provide an integrated workflow to co-design photonics and electronics, classically and quantum. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
 
+## Examples
+
+Follow the many [examples in the documentation](https://piel.readthedocs.io/en/stable/examples.html).
+
 ## Microservices Toolset
 This package provides interconnection functions to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some existing microservice dependency integrations are:
 * [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 * [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
 * [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
 * [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 * [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in Python
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
+
+
+## Contribution
+If you feel dedicated enough to become a project maintainer, or just want to do a single contributor, let's do this together!
```

### Comparing `piel-0.0.37/docs/Makefile` & `piel-0.0.38/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/docs/conf.py` & `piel-0.0.38/docs/conf.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/docs/examples/designs/simple_design/simple_design/tb/default/Makefile` & `piel-0.0.38/docs/examples/designs/simple_design/simple_design/tb/default/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/docs/index.rst` & `piel-0.0.38/docs/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/docs/make.bat` & `piel-0.0.38/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/docs/sections/microservices/dependencies/cocotb.rst` & `piel-0.0.38/docs/sections/microservices/dependencies/cocotb.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/docs/sections/microservices/dependencies/openlane.rst` & `piel-0.0.38/docs/sections/microservices/dependencies/openlane.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/docs/sections/microservices/dependencies/sax.rst` & `piel-0.0.38/docs/sections/microservices/dependencies/sax.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/docs/sections/microservices/integration/sax_qutip.rst` & `piel-0.0.38/docs/sections/microservices/integration/sax_qutip.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/__init__.py` & `piel-0.0.38/piel/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Top-level package for piel."""
 import os
 import pathlib
 
 # Libraries
 from piel import components  # NOQA: F401
 from piel import models  # NOQA: F401
+from piel import visual  # NOQA: F401
 
 # Functions
-from .cocotb import *
+
 from .config import *
 from .defaults import *
 from .file_system import *
-from .gdsfactory import *
 from .integration import *
-from .openlane import *
 from .parametric import *
-from .sax import *
+from .tools import *
+
 
 os.environ["PIEL_PACKAGE_DIRECTORY"] = str(
     pathlib.Path(__file__).parent.parent.resolve()
 )
 
 __author__ = """Dario Quintero"""
 __email__ = "darioaquintero@gmail.com"
-__version__ = "0.0.37"
+__version__ = "0.0.38"
```

### Comparing `piel-0.0.37/piel/cocotb/core.py` & `piel-0.0.38/piel/tools/cocotb/core.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/cocotb/data.py` & `piel-0.0.38/piel/tools/cocotb/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This file contains a range of functions used to read, plot and analyse cocotb simulations in a data-flow standard as suggested
 """
 import functools
 import pandas as pd
-from ..config import piel_path_types
-from ..file_system import return_path, get_files_recursively_in_directory
+from piel.config import piel_path_types
+from piel.file_system import return_path, get_files_recursively_in_directory
 
 __all__ = [
     "get_simulation_output_files",
     "get_simulation_output_files_from_design",
     "read_simulation_data",
     "simple_plot_simulation_data",
 ]
```

### Comparing `piel-0.0.37/piel/config.py` & `piel-0.0.38/piel/config.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/defaults.py` & `piel-0.0.38/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/file_conversion.py` & `piel-0.0.38/piel/file_conversion.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/file_system.py` & `piel-0.0.38/piel/file_system.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/gdsfactory/netlist.py` & `piel-0.0.38/piel/tools/gdsfactory/netlist.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/integration/openlane_gdsfactory_core.py` & `piel-0.0.38/piel/integration/openlane_gdsfactory_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 It is worth noting that GDSFactory has already the following PDKs installed:
 * SKY130nm https://gdsfactory.github.io/skywater130/
 * GF180nm https://gdsfactory.github.io/gf180/
 """
 import gdsfactory as gf
 from ..config import piel_path_types
 from ..file_system import check_path_exists
-from ..openlane.migrate import get_design_from_openlane_migration
-from ..openlane.utils import find_design_run
+from piel.tools.openlane.migrate import get_design_from_openlane_migration
+from piel.tools.openlane import find_design_run
 
 
 def create_gdsfactory_component_from_openlane(
     design_name_v1: str | None = None,
     design_directory: piel_path_types | None = None,
     run_name: str | None = None,
     v1: bool = True,
```

### Comparing `piel-0.0.37/piel/integration/sax_qutip.py` & `piel-0.0.38/piel/integration/sax_qutip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import qutip  # NOQA : F401
 import sax
 from ..config import nso
-from ..sax.utils import sax_to_s_parameters_standard_matrix
+from piel.tools.sax.utils import sax_to_s_parameters_standard_matrix
 
 __all__ = ["sax_to_ideal_qutip_unitary", "standard_s_parameters_to_ideal_qutip_unitary"]
 
 
 def standard_s_parameters_to_ideal_qutip_unitary(
     s_parameters_standard_matrix: nso.ndarray,
 ):
```

### Comparing `piel-0.0.37/piel/models/frequency/all.py` & `piel-0.0.38/piel/models/frequency/all.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/models/frequency/defaults.py` & `piel-0.0.38/piel/models/frequency/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/models/frequency/photonic/directional_coupler_length.py` & `piel-0.0.38/piel/models/frequency/photonic/directional_coupler_length.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/models/frequency/photonic/directional_coupler_real.py` & `piel-0.0.38/piel/models/frequency/photonic/directional_coupler_real.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/models/frequency/photonic/grating_coupler.py` & `piel-0.0.38/piel/models/frequency/photonic/grating_coupler.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/models/frequency/photonic/straight_waveguide.py` & `piel-0.0.38/piel/models/frequency/photonic/straight_waveguide.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/models/logic/electro_optic/signal_mapping.py` & `piel-0.0.38/piel/models/logic/electro_optic/signal_mapping.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/openlane/migrate.py` & `piel-0.0.38/piel/tools/openlane/migrate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 These functions provide easy tools for easily migrating between OpenLane v1 and v2 based designs.
 """
 import pathlib
 from .v1 import get_design_directory_from_root_openlane_v1
-from ..file_system import return_path
+from piel.file_system import return_path
 
 
 def get_design_from_openlane_migration(
     v1: bool = True,
     design_name_v1: str | None = None,
     design_directory: str | pathlib.Path | None = None,
     root_directory_v1: str | pathlib.Path | None = None,
```

### Comparing `piel-0.0.37/piel/openlane/parse/sta_rpt.py` & `piel-0.0.38/piel/tools/openlane/parse/sta_rpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 import pathlib
-from ...file_system import return_path
+from piel.file_system import return_path
 from .utils import (
     contains_in_lines,
     read_file_lines,
     get_file_line_by_keyword,
     create_file_lines_dataframe,
 )
```

### Comparing `piel-0.0.37/piel/openlane/parse/utils.py` & `piel-0.0.38/piel/tools/openlane/parse/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 import pathlib
-from ...file_system import check_path_exists, return_path
+from piel.file_system import check_path_exists, return_path
 
 
 def contains_in_lines(
     file_lines_data: pd.DataFrame,
     keyword: str,
 ):
     """
```

### Comparing `piel-0.0.37/piel/openlane/utils.py` & `piel-0.0.38/piel/tools/openlane/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pathlib
-from ..config import piel_path_types
-from ..file_system import return_path
+from piel.config import piel_path_types
+from piel.file_system import return_path
 
 
 def find_design_run(
     design_directory: piel_path_types,
     run_name: str | None = None,
 ) -> pathlib.Path:
     """
```

### Comparing `piel-0.0.37/piel/openlane/v1.py` & `piel-0.0.38/piel/tools/openlane/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 These set of functions aim to provide functionality to automate interacting with OpenLanes v1 design into Python environment, whilst `OpenLanes2` is under development.
 """
 
 import os
 import pathlib
 import json
-from ..parametric import multi_parameter_sweep
-from ..file_system import (
+from piel.parametric import multi_parameter_sweep
+from piel.file_system import (
     copy_source_folder,
     permit_script_execution,
     read_json,
     return_path,
     run_script,
     write_script,
 )
```

### Comparing `piel-0.0.37/piel/openlane/v2.py` & `piel-0.0.38/piel/tools/openlane/v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import openlane
-from ..config import piel_path_types
-from ..file_system import return_path, read_json
+from piel.config import piel_path_types
+from piel.file_system import return_path, read_json
 from piel.defaults import test_spm_open_lane_configuration
 
 
 def run_openlane_flow(
     configuration: dict | None = test_spm_open_lane_configuration,
     design_directory: piel_path_types = "/foss/designs/spm",
 ) -> None:
```

### Comparing `piel-0.0.37/piel/parametric.py` & `piel-0.0.38/piel/parametric.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/project_structure.py` & `piel-0.0.38/piel/project_structure.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel/sax/utils.py` & `piel-0.0.38/piel/tools/sax/utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/piel.egg-info/PKG-INFO` & `piel-0.0.38/piel.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.37
+Version: 0.0.38
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -36,19 +36,27 @@
 * System interconnection modelling in multiple environments.
 * Individual and interposer design integration.
 * Multi-domain electronics and photonics component models.
 * Quantum models of physical circuitry
 
 `piel` aims to provide an integrated workflow to co-design photonics and electronics, classically and quantum. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
 
+## Examples
+
+Follow the many [examples in the documentation](https://piel.readthedocs.io/en/stable/examples.html).
+
 ## Microservices Toolset
 This package provides interconnection functions to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some existing microservice dependency integrations are:
 * [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 * [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
 * [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
 * [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 * [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in Python
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
+
+
+## Contribution
+If you feel dedicated enough to become a project maintainer, or just want to do a single contributor, let's do this together!
```

### Comparing `piel-0.0.37/setup.py` & `piel-0.0.38/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 requirements = [
     "bokeh",
     "jupyter_bokeh",
+    "jupytext",
     "Click>=7.0",
     "cocotb",
     "gdsfactory",
     "openlane",
     "pandas",
     "sax",
     "qutip",
@@ -65,10 +66,10 @@
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/daquintero/piel",
-    version="0.0.37",
+    version="0.0.38",
     zip_safe=False,
 )
```

### Comparing `piel-0.0.37/tests/gdsfactory/test_netlist.py` & `piel-0.0.38/tests/tools/gdsfactory/test_netlist.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/tests/models/logic/electro_optic/test_signal_mapping.py` & `piel-0.0.38/tests/models/logic/electro_optic/test_signal_mapping.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/tests/sax/test_utils.py` & `piel-0.0.38/tests/tools/sax/test_utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.37/tests/test_piel.py` & `piel-0.0.38/tests/test_piel.py`

 * *Files identical despite different names*

