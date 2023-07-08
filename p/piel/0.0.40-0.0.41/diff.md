# Comparing `tmp/piel-0.0.40.tar.gz` & `tmp/piel-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.40.tar", last modified: Sat Jul  8 11:47:12 2023, max compression
+gzip compressed data, was "piel-0.0.41.tar", last modified: Sat Jul  8 15:26:00 2023, max compression
```

## Comparing `piel-0.0.40.tar` & `piel-0.0.41.tar`

### file list

```diff
@@ -1,333 +1,338 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.344609 piel-0.0.40/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-08 11:46:54.000000 piel-0.0.40/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 11:46:54.000000 piel-0.0.40/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-08 11:46:54.000000 piel-0.0.40/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-08 11:47:12.344609 piel-0.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-08 11:46:54.000000 piel-0.0.40/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.308608 piel-0.0.40/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-08 11:46:54.000000 piel-0.0.40/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.308608 piel-0.0.40/docs/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.308608 piel-0.0.40/docs/autoapi/piel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.308608 piel-0.0.40/docs/autoapi/piel/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/cli/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.308608 piel-0.0.40/docs/autoapi/piel/components/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/components/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.308608 piel-0.0.40/docs/autoapi/piel/config/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/config/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.308608 piel-0.0.40/docs/autoapi/piel/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.308608 piel-0.0.40/docs/autoapi/piel/file_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/file_conversion/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/file_system/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    40708 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/integration/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/integration/openlane_gdsfactory_core/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/integration/sax_cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/integration/sax_cocotb/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/integration/sax_qutip/
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/integration/sax_qutip/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/all/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/all/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/electro_optic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/electro_optic/ideal/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/electro_optic/ideal/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/coupler_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/coupler_simple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/grating_coupler/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/mmi1x2/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/mmi1x2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/mmi2x2/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/mmi2x2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.312609 piel-0.0.40/docs/autoapi/piel/models/frequency/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/frequency/utils/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/logic/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/logic/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/logic/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/logic/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/logic/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/logic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/logic/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/logic/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/logic/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/logic/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/physical/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/physical/electrical/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/physical/electrical/cable/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/physical/electrical/cable/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/physical/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/physical/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/physical/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/physical/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/physical/electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/physical/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/physical/geometry/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/physical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/physical/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/physical/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/physical/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/physical/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/physical/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/physical/thermal/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/physical/units/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/physical/units/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/transient/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/transient/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/transient/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/transient/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/transient/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/transient/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/transient/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/transient/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/transient/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/transient/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/transient/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/transient/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/models/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/parametric/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/parametric/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/project_structure/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/project_structure/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/tools/cocotb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/tools/cocotb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/cocotb/core/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.316609 piel-0.0.40/docs/autoapi/piel/tools/cocotb/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/cocotb/data/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/cocotb/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/gdsfactory/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/gdsfactory/netlist/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28090 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)    18502 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/openlane/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/openlane/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/openlane/migrate/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/openlane/parse/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/openlane/parse/sta_rpt/
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/openlane/parse/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/openlane/parse/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/openlane/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/openlane/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/openlane/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/openlane/v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/openlane/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/openlane/v2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/sax/
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/sax/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/tools/sax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/tools/sax/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/visual/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/visual/auto_plot_multiple/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/visual/auto_plot_multiple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/autoapi/piel/visual/data_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/visual/data_conversion/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-08 11:46:54.000000 piel-0.0.40/docs/autoapi/piel/visual/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-08 11:46:54.000000 piel-0.0.40/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 11:46:54.000000 piel-0.0.40/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.300608 piel-0.0.40/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.300608 piel-0.0.40/docs/examples/designs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.300608 piel-0.0.40/docs/examples/designs/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.300608 piel-0.0.40/docs/examples/designs/simple_design/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/examples/designs/simple_design/simple_design/tb/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-08 11:46:54.000000 piel-0.0.40/docs/examples/designs/simple_design/simple_design/tb/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.320609 piel-0.0.40/docs/examples/designs/simple_design/simple_design/tb/default/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-08 11:46:54.000000 piel-0.0.40/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-08 11:46:54.000000 piel-0.0.40/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-08 11:46:54.000000 piel-0.0.40/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-08 11:46:54.000000 piel-0.0.40/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.300608 piel-0.0.40/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.324609 piel-0.0.40/docs/sections/about/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/about/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/about/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.324609 piel-0.0.40/docs/sections/codesign/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/codesign/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.324609 piel-0.0.40/docs/sections/components/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/components/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.324609 piel-0.0.40/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/environment/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.324609 piel-0.0.40/docs/sections/microservices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.324609 piel-0.0.40/docs/sections/microservices/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/microservices/dependencies/cocotb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/microservices/dependencies/gdsfactory.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/microservices/dependencies/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/microservices/dependencies/openlane.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/microservices/dependencies/sax.rst
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/microservices/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.324609 piel-0.0.40/docs/sections/microservices/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/microservices/integration/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/microservices/integration/sax_qutip.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.324609 piel-0.0.40/docs/sections/models/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-08 11:46:54.000000 piel-0.0.40/docs/sections/models/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.328609 piel-0.0.40/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-08 11:46:54.000000 piel-0.0.40/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-08 11:46:54.000000 piel-0.0.40/piel/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.328609 piel-0.0.40/piel/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-08 11:46:54.000000 piel-0.0.40/piel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-08 11:46:54.000000 piel-0.0.40/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-08 11:46:54.000000 piel-0.0.40/piel/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-08 11:46:54.000000 piel-0.0.40/piel/file_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.328609 piel-0.0.40/piel/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 11:46:54.000000 piel-0.0.40/piel/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-08 11:46:54.000000 piel-0.0.40/piel/integration/openlane_gdsfactory_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-08 11:46:54.000000 piel-0.0.40/piel/integration/sax_cocotb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-08 11:46:54.000000 piel-0.0.40/piel/integration/sax_qutip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.328609 piel-0.0.40/piel/models/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.332609 piel-0.0.40/piel/models/frequency/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/all.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.332609 piel-0.0.40/piel/models/frequency/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.332609 piel-0.0.40/piel/models/frequency/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/electro_optic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/electro_optic/ideal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.332609 piel-0.0.40/piel/models/frequency/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.332609 piel-0.0.40/piel/models/frequency/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.332609 piel-0.0.40/piel/models/frequency/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/photonic/coupler_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/photonic/directional_coupler_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/photonic/directional_coupler_real.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/photonic/directional_coupler_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/photonic/grating_coupler.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/photonic/mmi1x2.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/photonic/mmi2x2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/photonic/straight_waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/frequency/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.332609 piel-0.0.40/piel/models/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/logic/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/logic/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/logic/electro_optic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/logic/electro_optic/signal_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/logic/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/logic/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/logic/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/logic/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/logic/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/logic/photonic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/physical/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/physical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/physical/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/physical/electrical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/physical/electrical/cable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/physical/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/physical/electro_optic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/physical/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/physical/electronic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/physical/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/physical/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/physical/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/physical/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/physical/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/physical/thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/physical/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/transient/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/transient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/transient/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/transient/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.336609 piel-0.0.40/piel/models/transient/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/transient/electro_optic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.340609 piel-0.0.40/piel/models/transient/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/transient/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.340609 piel-0.0.40/piel/models/transient/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/transient/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.340609 piel-0.0.40/piel/models/transient/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/transient/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/piel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-08 11:46:54.000000 piel-0.0.40/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-08 11:46:54.000000 piel-0.0.40/piel/project_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.340609 piel-0.0.40/piel/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.340609 piel-0.0.40/piel/tools/cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/cocotb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/cocotb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/cocotb/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.340609 piel-0.0.40/piel/tools/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/gdsfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/gdsfactory/netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.340609 piel-0.0.40/piel/tools/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/openlane/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.340609 piel-0.0.40/piel/tools/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/openlane/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/openlane/parse/sta_rpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/openlane/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/openlane/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/openlane/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/openlane/v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.340609 piel-0.0.40/piel/tools/sax/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/sax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-08 11:46:54.000000 piel-0.0.40/piel/tools/sax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.344609 piel-0.0.40/piel/visual/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-08 11:46:54.000000 piel-0.0.40/piel/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-08 11:46:54.000000 piel-0.0.40/piel/visual/auto_plot_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-08 11:46:54.000000 piel-0.0.40/piel/visual/data_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.328609 piel-0.0.40/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-08 11:47:12.000000 piel-0.0.40/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-07-08 11:47:12.000000 piel-0.0.40/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:47:12.000000 piel-0.0.40/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 11:47:12.000000 piel-0.0.40/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:47:12.000000 piel-0.0.40/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-08 11:47:12.000000 piel-0.0.40/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-08 11:47:12.000000 piel-0.0.40/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-08 11:47:12.344609 piel-0.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-08 11:46:54.000000 piel-0.0.40/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.344609 piel-0.0.40/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 11:46:54.000000 piel-0.0.40/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.308608 piel-0.0.40/tests/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.308608 piel-0.0.40/tests/models/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.344609 piel-0.0.40/tests/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-08 11:46:54.000000 piel-0.0.40/tests/models/logic/electro_optic/test_signal_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-08 11:46:54.000000 piel-0.0.40/tests/test_piel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.344609 piel-0.0.40/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/tests/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.344609 piel-0.0.40/tests/tools/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 11:46:54.000000 piel-0.0.40/tests/tools/gdsfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-08 11:46:54.000000 piel-0.0.40/tests/tools/gdsfactory/test_netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.344609 piel-0.0.40/tests/tools/sax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:54.000000 piel-0.0.40/tests/tools/sax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-08 11:46:54.000000 piel-0.0.40/tests/tools/sax/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:47:12.344609 piel-0.0.40/tests/visual/
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-08 11:46:54.000000 piel-0.0.40/tests/visual/test_data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-08 15:25:43.000000 piel-0.0.41/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 15:25:43.000000 piel-0.0.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-08 15:25:43.000000 piel-0.0.41/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-08 15:26:00.151372 piel-0.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-08 15:25:43.000000 piel-0.0.41/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-08 15:25:43.000000 piel-0.0.41/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/config/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/file_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/file_conversion/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/file_system/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    39344 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/integration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/integration/openlane_gdsfactory_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/integration/sax_cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/integration/sax_cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/integration/sax_qutip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/integration/sax_qutip/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/models/frequency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/models/frequency/all/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/all/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/models/frequency/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/electro_optic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/electro_optic/ideal/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/electro_optic/ideal/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/coupler_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/coupler_simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/grating_coupler/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/mmi1x2/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/mmi1x2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/mmi2x2/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/mmi2x2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/utils/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/electrical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/electrical/cable/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/electrical/cable/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/electro_optic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/electro_optic/basic_heater/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/electro_optic/basic_heater/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/geometry/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/thermal/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/physical/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/units/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/project_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/project_structure/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/cocotb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/cocotb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/cocotb/core/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/cocotb/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/cocotb/data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/netlist/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26766 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/migrate/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/sta_rpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/sax/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/sax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/sax/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/visual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/visual/auto_plot_multiple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/visual/auto_plot_multiple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/visual/data_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/visual/data_conversion/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/visual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-08 15:25:43.000000 piel-0.0.41/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 15:25:43.000000 piel-0.0.41/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.119372 piel-0.0.41/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.119372 piel-0.0.41/docs/examples/designs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.119372 piel-0.0.41/docs/examples/designs/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.119372 piel-0.0.41/docs/examples/designs/simple_design/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/examples/designs/simple_design/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-08 15:25:43.000000 piel-0.0.41/docs/examples/designs/simple_design/simple_design/tb/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/examples/designs/simple_design/simple_design/tb/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-08 15:25:43.000000 piel-0.0.41/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-08 15:25:43.000000 piel-0.0.41/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-08 15:25:43.000000 piel-0.0.41/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-08 15:25:43.000000 piel-0.0.41/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.123372 piel-0.0.41/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/about/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/about/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/codesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/codesign/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/environment/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/microservices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/microservices/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/cocotb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/gdsfactory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/openlane.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/principle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/pyspice.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/sax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/microservices/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/integration/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/integration/sax_qutip.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/models/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-08 15:25:43.000000 piel-0.0.41/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-08 15:25:43.000000 piel-0.0.41/piel/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-08 15:25:43.000000 piel-0.0.41/piel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-08 15:25:43.000000 piel-0.0.41/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-08 15:25:43.000000 piel-0.0.41/piel/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-08 15:25:43.000000 piel-0.0.41/piel/file_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 15:25:43.000000 piel-0.0.41/piel/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-08 15:25:43.000000 piel-0.0.41/piel/integration/openlane_gdsfactory_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-08 15:25:43.000000 piel-0.0.41/piel/integration/sax_cocotb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-08 15:25:43.000000 piel-0.0.41/piel/integration/sax_qutip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/electro_optic/ideal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/directional_coupler_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/directional_coupler_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/directional_coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/grating_coupler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/mmi1x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/mmi2x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/straight_waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/electro_optic/signal_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/photonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/electrical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/electrical/cable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/electro_optic/basic_heater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/electronic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-08 15:25:43.000000 piel-0.0.41/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-08 15:25:43.000000 piel-0.0.41/piel/project_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/cocotb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/cocotb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/cocotb/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/gdsfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/gdsfactory/netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/parse/sta_rpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/sax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/sax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/piel/visual/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-08 15:25:43.000000 piel-0.0.41/piel/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-08 15:25:43.000000 piel-0.0.41/piel/visual/auto_plot_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-08 15:25:43.000000 piel-0.0.41/piel/visual/data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:25:59.000000 piel-0.0.41/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-08 15:26:00.151372 piel-0.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-08 15:25:43.000000 piel-0.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 15:25:43.000000 piel-0.0.41/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.123372 piel-0.0.41/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.123372 piel-0.0.41/tests/models/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-08 15:25:43.000000 piel-0.0.41/tests/models/logic/electro_optic/test_signal_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-08 15:25:43.000000 piel-0.0.41/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/tests/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 15:25:43.000000 piel-0.0.41/tests/tools/gdsfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-08 15:25:43.000000 piel-0.0.41/tests/tools/gdsfactory/test_netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/tests/tools/sax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-08 15:25:43.000000 piel-0.0.41/tests/tools/sax/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/visual/
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-08 15:25:43.000000 piel-0.0.41/tests/visual/test_data_conversion.py
```

### Comparing `piel-0.0.40/CONTRIBUTING.rst` & `piel-0.0.41/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/LICENSE` & `piel-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/PKG-INFO` & `piel-0.0.41/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.40
+Version: 0.0.41
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -47,14 +47,15 @@
 ## Microservices Toolset
 This package provides interconnection functions to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some existing microservice dependency integrations are:
 * [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 * [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
 * [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
+* [pyspice](https://github.com/PySpice-org/PySpice) - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
 * [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 * [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in Python
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
```

### Comparing `piel-0.0.40/README.md` & `piel-0.0.41/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 ## Microservices Toolset
 This package provides interconnection functions to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some existing microservice dependency integrations are:
 * [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 * [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
 * [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
+* [pyspice](https://github.com/PySpice-org/PySpice) - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
 * [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 * [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in Python
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
```

### Comparing `piel-0.0.40/docs/Makefile` & `piel-0.0.41/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/config/index.rst` & `piel-0.0.41/docs/autoapi/piel/config/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/file_conversion/index.rst` & `piel-0.0.41/docs/autoapi/piel/file_conversion/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/file_system/index.rst` & `piel-0.0.41/docs/autoapi/piel/file_system/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/index.rst` & `piel-0.0.41/docs/autoapi/piel/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -69,49 +69,45 @@
    piel.configure_cocotb_simulation
    piel.run_cocotb_simulation
    piel.get_simulation_output_files_from_design
    piel.read_simulation_data
    piel.simple_plot_simulation_data
    piel.get_input_ports_index
    piel.get_matched_ports_tuple_index
-   piel.get_design_directory_from_root_openlane_v1
-   piel.return_path
    piel.get_design_from_openlane_migration
    piel.find_design_run
    piel.check_config_json_exists_openlane_v1
    piel.check_design_exists_openlane_v1
    piel.configure_and_run_design_openlane_v1
    piel.configure_parametric_designs_openlane_v1
    piel.configure_flow_script_openlane_v1
    piel.create_parametric_designs_openlane_v1
+   piel.get_design_directory_from_root_openlane_v1
    piel.get_latest_version_root_openlane_v1
    piel.read_configuration_openlane_v1
    piel.write_configuration_openlane_v1
-   piel.get_files_recursively_in_directory
-   piel.filter_timing_sta_files
-   piel.filter_power_sta_files
    piel.get_all_timing_sta_files
    piel.get_all_power_sta_files
-   piel.contains_in_lines
-   piel.read_file_lines
-   piel.get_file_line_by_keyword
-   piel.create_file_lines_dataframe
+   piel.filter_timing_sta_files
+   piel.filter_power_sta_files
    piel.calculate_max_frame_amount
-   piel.calculate_propagation_delay_from_timing_data
    piel.calculate_propagation_delay_from_file
+   piel.calculate_propagation_delay_from_timing_data
    piel.configure_timing_data_rows
    piel.configure_frame_id
    piel.filter_timing_data_by_net_name_and_type
    piel.get_frame_meta_data
    piel.get_frame_lines_data
    piel.get_frame_timing_data
    piel.get_all_timing_data_from_file
    piel.read_sta_rpt_fwf_file
-   piel.check_path_exists
-   piel.read_file
+   piel.contains_in_lines
+   piel.create_file_lines_dataframe
+   piel.get_file_line_by_keyword
+   piel.read_file_lines
    piel.run_openlane_flow
    piel.get_sdense_ports_index
    piel.sax_to_s_parameters_standard_matrix
 
 
 
 Attributes
@@ -353,16 +349,15 @@
    For example, a ``qutip`` representation of an s-gate gate would be:
 
    ..code-block:: python
 
        import numpy as np
        import qutip
        # S-Gate
-       s_gate_matrix = np.array([[1.,   0],
-                                [0., 1.j]])
+       s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
    In mathematical notation, this S-gate would be written as:
 
    ..math::
 
        S = \begin{bmatrix}
@@ -392,16 +387,15 @@
 
    ..code-block:: python
 
        import numpy as np
        import qutip
 
        # S-Gate
-       s_gate_matrix = np.array([[1.,   0],
-                                [0., 1.j]])
+       s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
    In mathematical notation, this S-gate would be written as:
 
    ..math::
 
        S = \begin{bmatrix}
@@ -624,53 +618,27 @@
    :type prefix: str, optional
 
    :returns: The ordered input ports index tuple.
              matched_ports_name_tuple_order(tuple): The ordered input ports name tuple.
    :rtype: matches_ports_index_tuple_order(tuple)
 
 
-.. py:function:: get_design_directory_from_root_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> pathlib.Path
-
-   Gets the design directory from the root directory.
-
-   :param design_name: Name of the design.
-   :type design_name: str
-   :param root_directory: Design directory.
-   :type root_directory: str | pathlib.Path
-
-   :returns: Design directory.
-   :rtype: design_directory(pathlib.Path)
-
-
-.. py:function:: return_path(input_path: piel.config.piel_path_types) -> pathlib.Path
-
-   Returns a pathlib.Path to be able to perform operations accordingly internally.
-
-   This allows us to maintain compatibility between POSIX and Windows systems.
-
-   :param input_path: Input path.
-   :type input_path: str
-
-   :returns: Pathlib path.
-   :rtype: pathlib.Path
-
-
 .. py:function:: get_design_from_openlane_migration(v1: bool = True, design_name_v1: str | None = None, design_directory: str | pathlib.Path | None = None, root_directory_v1: str | pathlib.Path | None = None) -> (str, pathlib.Path)
 
    This function provides the integration mechanism for easily migrating the interconnection with other toolsets from an OpenLane v1 design to an OpenLane v2 design.
 
    This function checks if the inputs are to be treated as v1 inputs. If so, and a `design_name` is provided then it will set the `design_directory` to the corresponding `design_name` directory in the corresponding `root_directory_v1 / designs`. If no `root_directory` is provided then it returns `$OPENLANE_ROOT/"<latest>"/. If a `design_directory` is provided then this will always take precedence even with a `v1` flag.
 
    :param v1: If True, it will migrate from v1 to v2.
    :type v1: bool
    :param design_name_v1: Design name of the v1 design that can be found within `$OPENLANE_ROOT/"<latest>"/designs`.
    :type design_name_v1: str
    :param design_directory: Design directory PATH. Optional path for v2-based designs.
    :type design_directory: str
-   :param root_directory_v1: Root directory of OpenLane v1. If set to None it will return `$OPENLANE_ROOT/"<latest>"
+   :param root_directory_v1: Root directory of OpenLane v1. If set to None it will return `$OPENLANE_ROOT/"<latest>"`
    :type root_directory_v1: str
 
    :returns: None
 
 
 .. py:function:: find_design_run(design_directory: piel.config.piel_path_types, run_name: str | None = None) -> pathlib.Path
 
@@ -760,14 +728,27 @@
    :type parameter_sweep_dictionary: dict
    :param target_directory: Optional target directory.
    :type target_directory: str | pathlib.Path | None
 
    :returns: None
 
 
+.. py:function:: get_design_directory_from_root_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> pathlib.Path
+
+   Gets the design directory from the root directory.
+
+   :param design_name: Name of the design.
+   :type design_name: str
+   :param root_directory: Design directory.
+   :type root_directory: str | pathlib.Path
+
+   :returns: Design directory.
+   :rtype: design_directory(pathlib.Path)
+
+
 .. py:function:: get_latest_version_root_openlane_v1() -> pathlib.Path
 
    Gets the latest version root of OpenLane v1.
 
 
 .. py:function:: read_configuration_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> dict
 
@@ -790,49 +771,14 @@
    :type configuration: dict
    :param design_directory: Design directory PATH.
    :type design_directory: str
 
    :returns: None
 
 
-.. py:function:: get_files_recursively_in_directory(path: piel.config.piel_path_types, extension: str = '*')
-
-   Returns a list of files in a directory.
-
-   :param path: Input path.
-   :type path: piel_path_types
-   :param extension: File extension.
-   :type extension: str
-
-   :returns: List of files.
-   :rtype: file_list(list)
-
-
-.. py:function:: filter_timing_sta_files(file_list)
-
-   Filter the timing sta files from the list of files
-
-   :param file_list: List containing the file paths
-   :type file_list: list
-
-   :returns: List containing the timing sta files
-   :rtype: timing_sta_files (list)
-
-
-.. py:function:: filter_power_sta_files(file_list)
-
-   Filter the power sta files from the list of files
-
-   :param file_list: List containing the file paths
-   :type file_list: list
-
-   :returns: List containing the power sta files
-   :rtype: power_sta_files (list)
-
-
 .. py:function:: get_all_timing_sta_files(run_directory)
 
    This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
 
    :param run_directory: The run directory to perform the analysis on. Defaults to None.
    :type run_directory: str, optional
 
@@ -847,73 +793,56 @@
    :param run_directory: The run directory to perform the analysis on. Defaults to None.
    :type run_directory: str, optional
 
    :returns: List of all the .rpt files in the run directory.
    :rtype: power_sta_files_list (list)
 
 
-.. py:function:: contains_in_lines(file_lines_data: pandas.DataFrame, keyword: str)
+.. py:function:: filter_timing_sta_files(file_list)
 
-   Check if the keyword is contained in the file lines
+   Filter the timing sta files from the list of files
 
-   :param file_lines_data: Dataframe containing the file lines
-   :type file_lines_data: pd.DataFrame
-   :param keyword: Keyword to search for
-   :type keyword: str
+   :param file_list: List containing the file paths
+   :type file_list: list
 
-   :returns: Dataframe containing the file lines
-   :rtype: file_lines_data (pd.DataFrame)
+   :returns: List containing the timing sta files
+   :rtype: timing_sta_files (list)
 
 
-.. py:function:: read_file_lines(file_path: str | pathlib.Path)
+.. py:function:: filter_power_sta_files(file_list)
 
-   Extract lines from the file
+   Filter the power sta files from the list of files
 
-   :param file_path: Path to the file
-   :type file_path: str | pathlib.Path
+   :param file_list: List containing the file paths
+   :type file_list: list
 
-   :returns: list containing the file lines
-   :rtype: file_lines_raw (list)
+   :returns: List containing the power sta files
+   :rtype: power_sta_files (list)
 
 
-.. py:function:: get_file_line_by_keyword(file_lines_data: pandas.DataFrame, keyword: str, regex: str)
+.. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
-   Extract the data from the file lines using the given keyword and regex
+   Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
-   :param keyword: Keyword to search for
-   :type keyword: str
-   :param regex: Regex to extract the data
-   :type regex: str
-
-   :returns: Dataframe containing the extracted values
-   :rtype: extracted_values (pd.DataFrame)
-
-
-.. py:function:: create_file_lines_dataframe(file_lines_raw)
-
-   Create a DataFrame from the raw lines of a file
 
-   :param file_lines_raw: list containing the file lines
-   :type file_lines_raw: list
-
-   :returns: Dataframe containing the file lines
-   :rtype: file_lines_data (pd.DataFrame)
+   :returns: Maximum number of frames in the file
+   :rtype: maximum_frame_amount (int)
 
 
-.. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
+.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
 
-   Calculate the maximum frame amount based on the frame IDs in the DataFrame
+   Calculate the propagation delay for each frame in the file
 
-   :param file_lines_data: Dataframe containing the file lines
-   :type file_lines_data: pd.DataFrame
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
-   :returns: Maximum number of frames in the file
-   :rtype: maximum_frame_amount (int)
+   :returns: Dictionary containing the propagation delay
+   :rtype: propagation_delay (dict)
 
 
 .. py:function:: calculate_propagation_delay_from_timing_data(net_name_in: str, net_name_out: str, timing_data: pandas.DataFrame)
 
    Calculate the propagation delay between two nets
 
    :param net_name_in: Name of the input net
@@ -923,25 +852,14 @@
    :param timing_data: Dataframe containing the timing data
    :type timing_data: pd.DataFrame
 
    :returns: Dataframe containing the propagation delay
    :rtype: propagation_delay_dataframe (pd.DataFrame)
 
 
-.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
-
-   Calculate the propagation delay for each frame in the file
-
-   :param file_path: Path to the file
-   :type file_path: str | pathlib.Path
-
-   :returns: Dictionary containing the propagation delay
-   :rtype: propagation_delay (dict)
-
-
 .. py:function:: configure_timing_data_rows(file_lines_data: pandas.DataFrame)
 
    Identify the timing data lines for each frame and creates a metadata dictionary for frames.
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
 
@@ -1037,34 +955,62 @@
    :param frame_id: Frame ID to be read
    :type frame_id: int
 
    :returns: DataFrame containing the file data
    :rtype: file_data (pd.DataFrame)
 
 
-.. py:function:: check_path_exists(path: piel.config.piel_path_types, raise_errors: bool = False) -> bool
+.. py:function:: contains_in_lines(file_lines_data: pandas.DataFrame, keyword: str)
 
-   Checks if a directory exists.
+   Check if the keyword is contained in the file lines
 
-   :param path: Input path.
-   :type path: piel_path_types
+   :param file_lines_data: Dataframe containing the file lines
+   :type file_lines_data: pd.DataFrame
+   :param keyword: Keyword to search for
+   :type keyword: str
+
+   :returns: Dataframe containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
 
-   :returns: True if directory exists.
-   :rtype: directory_exists(bool)
 
+.. py:function:: create_file_lines_dataframe(file_lines_raw)
 
-.. py:function:: read_file(file_path: str | pathlib.Path)
+   Create a DataFrame from the raw lines of a file
 
-   Read the file from the given path
+   :param file_lines_raw: list containing the file lines
+   :type file_lines_raw: list
+
+   :returns: Dataframe containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
+
+
+.. py:function:: get_file_line_by_keyword(file_lines_data: pandas.DataFrame, keyword: str, regex: str)
+
+   Extract the data from the file lines using the given keyword and regex
+
+   :param file_lines_data: Dataframe containing the file lines
+   :type file_lines_data: pd.DataFrame
+   :param keyword: Keyword to search for
+   :type keyword: str
+   :param regex: Regex to extract the data
+   :type regex: str
+
+   :returns: Dataframe containing the extracted values
+   :rtype: extracted_values (pd.DataFrame)
+
+
+.. py:function:: read_file_lines(file_path: str | pathlib.Path)
+
+   Extract lines from the file
 
    :param file_path: Path to the file
    :type file_path: str | pathlib.Path
 
-   :returns: the opened file
-   :rtype: file
+   :returns: list containing the file lines
+   :rtype: file_lines_raw (list)
 
 
 .. py:function:: run_openlane_flow(configuration: dict | None = test_spm_open_lane_configuration, design_directory: piel.config.piel_path_types = '/foss/designs/spm') -> None
 
    Runs the OpenLane flow.
 
    :param configuration: OpenLane configuration dictionary. If none is present it will default to the config.json file on the design_directory.
@@ -1216,8 +1162,8 @@
 
 .. py:data:: __email__
    :value: 'darioaquintero@gmail.com'
 
 
 
 .. py:data:: __version__
-   :value: '0.0.39'
+   :value: '0.0.40'
```

### Comparing `piel-0.0.40/docs/autoapi/piel/integration/index.rst` & `piel-0.0.41/docs/autoapi/piel/integration/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,15 @@
    For example, a ``qutip`` representation of an s-gate gate would be:
 
    ..code-block:: python
 
        import numpy as np
        import qutip
        # S-Gate
-       s_gate_matrix = np.array([[1.,   0],
-                                [0., 1.j]])
+       s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
    In mathematical notation, this S-gate would be written as:
 
    ..math::
 
        S = \begin{bmatrix}
@@ -103,16 +102,15 @@
 
    ..code-block:: python
 
        import numpy as np
        import qutip
 
        # S-Gate
-       s_gate_matrix = np.array([[1.,   0],
-                                [0., 1.j]])
+       s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
    In mathematical notation, this S-gate would be written as:
 
    ..math::
 
        S = \begin{bmatrix}
```

### Comparing `piel-0.0.40/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst` & `piel-0.0.41/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/integration/sax_qutip/index.rst` & `piel-0.0.41/docs/autoapi/piel/integration/sax_qutip/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 
    ..code-block:: python
 
        import numpy as np
        import qutip
 
        # S-Gate
-       s_gate_matrix = np.array([[1.,   0],
-                                [0., 1.j]])
+       s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
    In mathematical notation, this S-gate would be written as:
 
    ..math::
 
        S = \begin{bmatrix}
@@ -72,16 +71,15 @@
    For example, a ``qutip`` representation of an s-gate gate would be:
 
    ..code-block:: python
 
        import numpy as np
        import qutip
        # S-Gate
-       s_gate_matrix = np.array([[1.,   0],
-                                [0., 1.j]])
+       s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
    In mathematical notation, this S-gate would be written as:
 
    ..math::
 
        S = \begin{bmatrix}
```

### Comparing `piel-0.0.40/docs/autoapi/piel/models/frequency/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/frequency/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -50,21 +50,27 @@
    :param custom_models: Custom models dictionary.
    :type custom_models: dict
 
    :returns: Composed models dictionary.
    :rtype: dict
 
 
-.. py:function:: get_all_models() -> dict
+.. py:function:: get_all_models(custom_library: dict | None = None) -> dict
 
    Returns the default models dictionary.
 
+   :param custom_library: Custom defaults dictionary.
+   :type custom_library: dict
+
    :returns: Default models dictionary.
    :rtype: dict
 
 
-.. py:function:: get_default_models() -> dict
+.. py:function:: get_default_models(custom_defaults: dict | None = None) -> dict
 
    Returns the default models dictionary.
 
+   :param custom_defaults: Custom defaults dictionary.
+   :type custom_defaults: dict
+
    :returns: Default models dictionary.
    :rtype: dict
```

### Comparing `piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst`

 * *Files 23% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.models.frequency.photonic.grating_coupler.grating_coupler
+   piel.models.frequency.photonic.grating_coupler.grating_coupler_simple
 
 
 
-.. py:function:: grating_coupler(R=0.0, R_in=0.0, Tmax=1.0, bandwidth=6e-08, wl0=1.55e-06)
+.. py:function:: grating_coupler_simple(R=0.0, R_in=0.0, Tmax=1.0, bandwidth=6e-08, wl0=1.55e-06)
```

### Comparing `piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -28,50 +28,33 @@
 ~~~~~~~~~
 
 .. autoapisummary::
 
    piel.models.frequency.photonic.coupler
    piel.models.frequency.photonic.directional_coupler_with_length
    piel.models.frequency.photonic.directional_coupler
-   piel.models.frequency.photonic.grating_coupler
+   piel.models.frequency.photonic.grating_coupler_simple
    piel.models.frequency.photonic.mmi1x2_50_50
    piel.models.frequency.photonic.mmi2x2_50_50
    piel.models.frequency.photonic.ideal_active_waveguide
    piel.models.frequency.photonic.waveguide
    piel.models.frequency.photonic.simple_straight
 
 
 
-Attributes
-~~~~~~~~~~
-
-.. autoapisummary::
-
-   piel.models.frequency.photonic.nso
-   piel.models.frequency.photonic.nso
-
-
 .. py:function:: coupler(coupling=0.5)
 
 
-.. py:data:: nso
-
-
-
 .. py:function:: directional_coupler_with_length(length=1e-05, coupling=0.5, loss=0, neff=2.34, wl0=1.55e-06, ng=3.4, phase=0)
 
 
 .. py:function:: directional_coupler(coupling=0.5)
 
 
-.. py:data:: nso
-
-
-
-.. py:function:: grating_coupler(R=0.0, R_in=0.0, Tmax=1.0, bandwidth=6e-08, wl0=1.55e-06)
+.. py:function:: grating_coupler_simple(R=0.0, R_in=0.0, Tmax=1.0, bandwidth=6e-08, wl0=1.55e-06)
 
 
 .. py:function:: mmi1x2_50_50()
 
 
 .. py:function:: mmi2x2_50_50()
```

### Comparing `piel-0.0.40/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/models/frequency/utils/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/frequency/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/models/logic/electro_optic/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 
    In this function we implement different methods of mapping electronic signals to phase.
 
    One particular implementation of phase mapping would be:
 
    .. list-table:: Example Basic Phase Mapping
       :header-rows: 1
+
       * - Bit
         - Phase
       * - b0
-        - :math:`\phi_0    o 0`
+        - :math:`\phi_0 \to 0`
       * - b1
-        - :math:`\phi_1    o \pi`
+        - :math:`\phi_1 \to \pi`
 
    We can define the two corresponding angles that this would be.
 
    A more complex implementation of phase mapping can be similar to a DAC mapping: a bitstring within a converter bit-size can map directly to a particular phase space within a particular mapping.
```

### Comparing `piel-0.0.40/docs/autoapi/piel/models/physical/geometry/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/physical/geometry/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/models/physical/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/physical/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -38,26 +38,14 @@
 .. autoapisummary::
 
    piel.models.physical.calculate_cross_sectional_area_m2
    piel.models.physical.convert_awg_to_m2
 
 
 
-Attributes
-~~~~~~~~~~
-
-.. autoapisummary::
-
-   piel.models.physical.nso
-
-
-.. py:data:: nso
-
-
-
 .. py:function:: calculate_cross_sectional_area_m2(diameter_m: float) -> float
 
    Calculates the cross sectional area of a circle in meters squared.
 
    :param diameter_m: Diameter of the circle in meters.
    :type diameter_m: float
```

### Comparing `piel-0.0.40/docs/autoapi/piel/models/physical/units/index.rst` & `piel-0.0.41/docs/autoapi/piel/models/physical/units/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/parametric/index.rst` & `piel-0.0.41/docs/autoapi/piel/parametric/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/project_structure/index.rst` & `piel-0.0.41/docs/autoapi/piel/project_structure/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/cocotb/core/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/cocotb/core/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/cocotb/data/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/cocotb/data/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/cocotb/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/cocotb/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/gdsfactory/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,49 +29,45 @@
    piel.tools.configure_cocotb_simulation
    piel.tools.run_cocotb_simulation
    piel.tools.get_simulation_output_files_from_design
    piel.tools.read_simulation_data
    piel.tools.simple_plot_simulation_data
    piel.tools.get_input_ports_index
    piel.tools.get_matched_ports_tuple_index
-   piel.tools.get_design_directory_from_root_openlane_v1
-   piel.tools.return_path
    piel.tools.get_design_from_openlane_migration
    piel.tools.find_design_run
    piel.tools.check_config_json_exists_openlane_v1
    piel.tools.check_design_exists_openlane_v1
    piel.tools.configure_and_run_design_openlane_v1
    piel.tools.configure_parametric_designs_openlane_v1
    piel.tools.configure_flow_script_openlane_v1
    piel.tools.create_parametric_designs_openlane_v1
+   piel.tools.get_design_directory_from_root_openlane_v1
    piel.tools.get_latest_version_root_openlane_v1
    piel.tools.read_configuration_openlane_v1
    piel.tools.write_configuration_openlane_v1
-   piel.tools.get_files_recursively_in_directory
-   piel.tools.filter_timing_sta_files
-   piel.tools.filter_power_sta_files
    piel.tools.get_all_timing_sta_files
    piel.tools.get_all_power_sta_files
-   piel.tools.contains_in_lines
-   piel.tools.read_file_lines
-   piel.tools.get_file_line_by_keyword
-   piel.tools.create_file_lines_dataframe
+   piel.tools.filter_timing_sta_files
+   piel.tools.filter_power_sta_files
    piel.tools.calculate_max_frame_amount
-   piel.tools.calculate_propagation_delay_from_timing_data
    piel.tools.calculate_propagation_delay_from_file
+   piel.tools.calculate_propagation_delay_from_timing_data
    piel.tools.configure_timing_data_rows
    piel.tools.configure_frame_id
    piel.tools.filter_timing_data_by_net_name_and_type
    piel.tools.get_frame_meta_data
    piel.tools.get_frame_lines_data
    piel.tools.get_frame_timing_data
    piel.tools.get_all_timing_data_from_file
    piel.tools.read_sta_rpt_fwf_file
-   piel.tools.check_path_exists
-   piel.tools.read_file
+   piel.tools.contains_in_lines
+   piel.tools.create_file_lines_dataframe
+   piel.tools.get_file_line_by_keyword
+   piel.tools.read_file_lines
    piel.tools.run_openlane_flow
    piel.tools.get_sdense_ports_index
    piel.tools.sax_to_s_parameters_standard_matrix
 
 
 
 Attributes
@@ -244,53 +240,27 @@
    :type prefix: str, optional
 
    :returns: The ordered input ports index tuple.
              matched_ports_name_tuple_order(tuple): The ordered input ports name tuple.
    :rtype: matches_ports_index_tuple_order(tuple)
 
 
-.. py:function:: get_design_directory_from_root_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> pathlib.Path
-
-   Gets the design directory from the root directory.
-
-   :param design_name: Name of the design.
-   :type design_name: str
-   :param root_directory: Design directory.
-   :type root_directory: str | pathlib.Path
-
-   :returns: Design directory.
-   :rtype: design_directory(pathlib.Path)
-
-
-.. py:function:: return_path(input_path: piel.config.piel_path_types) -> pathlib.Path
-
-   Returns a pathlib.Path to be able to perform operations accordingly internally.
-
-   This allows us to maintain compatibility between POSIX and Windows systems.
-
-   :param input_path: Input path.
-   :type input_path: str
-
-   :returns: Pathlib path.
-   :rtype: pathlib.Path
-
-
 .. py:function:: get_design_from_openlane_migration(v1: bool = True, design_name_v1: str | None = None, design_directory: str | pathlib.Path | None = None, root_directory_v1: str | pathlib.Path | None = None) -> (str, pathlib.Path)
 
    This function provides the integration mechanism for easily migrating the interconnection with other toolsets from an OpenLane v1 design to an OpenLane v2 design.
 
    This function checks if the inputs are to be treated as v1 inputs. If so, and a `design_name` is provided then it will set the `design_directory` to the corresponding `design_name` directory in the corresponding `root_directory_v1 / designs`. If no `root_directory` is provided then it returns `$OPENLANE_ROOT/"<latest>"/. If a `design_directory` is provided then this will always take precedence even with a `v1` flag.
 
    :param v1: If True, it will migrate from v1 to v2.
    :type v1: bool
    :param design_name_v1: Design name of the v1 design that can be found within `$OPENLANE_ROOT/"<latest>"/designs`.
    :type design_name_v1: str
    :param design_directory: Design directory PATH. Optional path for v2-based designs.
    :type design_directory: str
-   :param root_directory_v1: Root directory of OpenLane v1. If set to None it will return `$OPENLANE_ROOT/"<latest>"
+   :param root_directory_v1: Root directory of OpenLane v1. If set to None it will return `$OPENLANE_ROOT/"<latest>"`
    :type root_directory_v1: str
 
    :returns: None
 
 
 .. py:function:: find_design_run(design_directory: piel.config.piel_path_types, run_name: str | None = None) -> pathlib.Path
 
@@ -380,14 +350,27 @@
    :type parameter_sweep_dictionary: dict
    :param target_directory: Optional target directory.
    :type target_directory: str | pathlib.Path | None
 
    :returns: None
 
 
+.. py:function:: get_design_directory_from_root_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> pathlib.Path
+
+   Gets the design directory from the root directory.
+
+   :param design_name: Name of the design.
+   :type design_name: str
+   :param root_directory: Design directory.
+   :type root_directory: str | pathlib.Path
+
+   :returns: Design directory.
+   :rtype: design_directory(pathlib.Path)
+
+
 .. py:function:: get_latest_version_root_openlane_v1() -> pathlib.Path
 
    Gets the latest version root of OpenLane v1.
 
 
 .. py:function:: read_configuration_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> dict
 
@@ -410,49 +393,14 @@
    :type configuration: dict
    :param design_directory: Design directory PATH.
    :type design_directory: str
 
    :returns: None
 
 
-.. py:function:: get_files_recursively_in_directory(path: piel.config.piel_path_types, extension: str = '*')
-
-   Returns a list of files in a directory.
-
-   :param path: Input path.
-   :type path: piel_path_types
-   :param extension: File extension.
-   :type extension: str
-
-   :returns: List of files.
-   :rtype: file_list(list)
-
-
-.. py:function:: filter_timing_sta_files(file_list)
-
-   Filter the timing sta files from the list of files
-
-   :param file_list: List containing the file paths
-   :type file_list: list
-
-   :returns: List containing the timing sta files
-   :rtype: timing_sta_files (list)
-
-
-.. py:function:: filter_power_sta_files(file_list)
-
-   Filter the power sta files from the list of files
-
-   :param file_list: List containing the file paths
-   :type file_list: list
-
-   :returns: List containing the power sta files
-   :rtype: power_sta_files (list)
-
-
 .. py:function:: get_all_timing_sta_files(run_directory)
 
    This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
 
    :param run_directory: The run directory to perform the analysis on. Defaults to None.
    :type run_directory: str, optional
 
@@ -467,73 +415,56 @@
    :param run_directory: The run directory to perform the analysis on. Defaults to None.
    :type run_directory: str, optional
 
    :returns: List of all the .rpt files in the run directory.
    :rtype: power_sta_files_list (list)
 
 
-.. py:function:: contains_in_lines(file_lines_data: pandas.DataFrame, keyword: str)
+.. py:function:: filter_timing_sta_files(file_list)
 
-   Check if the keyword is contained in the file lines
+   Filter the timing sta files from the list of files
 
-   :param file_lines_data: Dataframe containing the file lines
-   :type file_lines_data: pd.DataFrame
-   :param keyword: Keyword to search for
-   :type keyword: str
+   :param file_list: List containing the file paths
+   :type file_list: list
 
-   :returns: Dataframe containing the file lines
-   :rtype: file_lines_data (pd.DataFrame)
+   :returns: List containing the timing sta files
+   :rtype: timing_sta_files (list)
 
 
-.. py:function:: read_file_lines(file_path: str | pathlib.Path)
+.. py:function:: filter_power_sta_files(file_list)
 
-   Extract lines from the file
+   Filter the power sta files from the list of files
 
-   :param file_path: Path to the file
-   :type file_path: str | pathlib.Path
+   :param file_list: List containing the file paths
+   :type file_list: list
 
-   :returns: list containing the file lines
-   :rtype: file_lines_raw (list)
+   :returns: List containing the power sta files
+   :rtype: power_sta_files (list)
 
 
-.. py:function:: get_file_line_by_keyword(file_lines_data: pandas.DataFrame, keyword: str, regex: str)
+.. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
-   Extract the data from the file lines using the given keyword and regex
+   Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
-   :param keyword: Keyword to search for
-   :type keyword: str
-   :param regex: Regex to extract the data
-   :type regex: str
-
-   :returns: Dataframe containing the extracted values
-   :rtype: extracted_values (pd.DataFrame)
-
-
-.. py:function:: create_file_lines_dataframe(file_lines_raw)
-
-   Create a DataFrame from the raw lines of a file
-
-   :param file_lines_raw: list containing the file lines
-   :type file_lines_raw: list
 
-   :returns: Dataframe containing the file lines
-   :rtype: file_lines_data (pd.DataFrame)
+   :returns: Maximum number of frames in the file
+   :rtype: maximum_frame_amount (int)
 
 
-.. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
+.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
 
-   Calculate the maximum frame amount based on the frame IDs in the DataFrame
+   Calculate the propagation delay for each frame in the file
 
-   :param file_lines_data: Dataframe containing the file lines
-   :type file_lines_data: pd.DataFrame
+   :param file_path: Path to the file
+   :type file_path: str | pathlib.Path
 
-   :returns: Maximum number of frames in the file
-   :rtype: maximum_frame_amount (int)
+   :returns: Dictionary containing the propagation delay
+   :rtype: propagation_delay (dict)
 
 
 .. py:function:: calculate_propagation_delay_from_timing_data(net_name_in: str, net_name_out: str, timing_data: pandas.DataFrame)
 
    Calculate the propagation delay between two nets
 
    :param net_name_in: Name of the input net
@@ -543,25 +474,14 @@
    :param timing_data: Dataframe containing the timing data
    :type timing_data: pd.DataFrame
 
    :returns: Dataframe containing the propagation delay
    :rtype: propagation_delay_dataframe (pd.DataFrame)
 
 
-.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
-
-   Calculate the propagation delay for each frame in the file
-
-   :param file_path: Path to the file
-   :type file_path: str | pathlib.Path
-
-   :returns: Dictionary containing the propagation delay
-   :rtype: propagation_delay (dict)
-
-
 .. py:function:: configure_timing_data_rows(file_lines_data: pandas.DataFrame)
 
    Identify the timing data lines for each frame and creates a metadata dictionary for frames.
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
 
@@ -657,34 +577,62 @@
    :param frame_id: Frame ID to be read
    :type frame_id: int
 
    :returns: DataFrame containing the file data
    :rtype: file_data (pd.DataFrame)
 
 
-.. py:function:: check_path_exists(path: piel.config.piel_path_types, raise_errors: bool = False) -> bool
+.. py:function:: contains_in_lines(file_lines_data: pandas.DataFrame, keyword: str)
+
+   Check if the keyword is contained in the file lines
+
+   :param file_lines_data: Dataframe containing the file lines
+   :type file_lines_data: pd.DataFrame
+   :param keyword: Keyword to search for
+   :type keyword: str
+
+   :returns: Dataframe containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
+
+
+.. py:function:: create_file_lines_dataframe(file_lines_raw)
+
+   Create a DataFrame from the raw lines of a file
+
+   :param file_lines_raw: list containing the file lines
+   :type file_lines_raw: list
 
-   Checks if a directory exists.
+   :returns: Dataframe containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
 
-   :param path: Input path.
-   :type path: piel_path_types
 
-   :returns: True if directory exists.
-   :rtype: directory_exists(bool)
+.. py:function:: get_file_line_by_keyword(file_lines_data: pandas.DataFrame, keyword: str, regex: str)
 
+   Extract the data from the file lines using the given keyword and regex
 
-.. py:function:: read_file(file_path: str | pathlib.Path)
+   :param file_lines_data: Dataframe containing the file lines
+   :type file_lines_data: pd.DataFrame
+   :param keyword: Keyword to search for
+   :type keyword: str
+   :param regex: Regex to extract the data
+   :type regex: str
+
+   :returns: Dataframe containing the extracted values
+   :rtype: extracted_values (pd.DataFrame)
 
-   Read the file from the given path
+
+.. py:function:: read_file_lines(file_path: str | pathlib.Path)
+
+   Extract lines from the file
 
    :param file_path: Path to the file
    :type file_path: str | pathlib.Path
 
-   :returns: the opened file
-   :rtype: file
+   :returns: list containing the file lines
+   :rtype: file_lines_raw (list)
 
 
 .. py:function:: run_openlane_flow(configuration: dict | None = test_spm_open_lane_configuration, design_directory: piel.config.piel_path_types = '/foss/designs/spm') -> None
 
    Runs the OpenLane flow.
 
    :param configuration: OpenLane configuration dictionary. If none is present it will default to the config.json file on the design_directory.
```

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/openlane/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/openlane/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -30,94 +30,62 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.tools.openlane.get_design_directory_from_root_openlane_v1
-   piel.tools.openlane.return_path
    piel.tools.openlane.get_design_from_openlane_migration
    piel.tools.openlane.find_design_run
    piel.tools.openlane.check_config_json_exists_openlane_v1
    piel.tools.openlane.check_design_exists_openlane_v1
    piel.tools.openlane.configure_and_run_design_openlane_v1
    piel.tools.openlane.configure_parametric_designs_openlane_v1
    piel.tools.openlane.configure_flow_script_openlane_v1
    piel.tools.openlane.create_parametric_designs_openlane_v1
    piel.tools.openlane.get_design_directory_from_root_openlane_v1
    piel.tools.openlane.get_latest_version_root_openlane_v1
    piel.tools.openlane.read_configuration_openlane_v1
    piel.tools.openlane.write_configuration_openlane_v1
-   piel.tools.openlane.return_path
-   piel.tools.openlane.get_files_recursively_in_directory
-   piel.tools.openlane.filter_timing_sta_files
-   piel.tools.openlane.filter_power_sta_files
    piel.tools.openlane.get_all_timing_sta_files
    piel.tools.openlane.get_all_power_sta_files
-   piel.tools.openlane.contains_in_lines
-   piel.tools.openlane.read_file_lines
-   piel.tools.openlane.get_file_line_by_keyword
-   piel.tools.openlane.create_file_lines_dataframe
+   piel.tools.openlane.filter_timing_sta_files
+   piel.tools.openlane.filter_power_sta_files
    piel.tools.openlane.calculate_max_frame_amount
-   piel.tools.openlane.calculate_propagation_delay_from_timing_data
    piel.tools.openlane.calculate_propagation_delay_from_file
+   piel.tools.openlane.calculate_propagation_delay_from_timing_data
    piel.tools.openlane.configure_timing_data_rows
    piel.tools.openlane.configure_frame_id
    piel.tools.openlane.filter_timing_data_by_net_name_and_type
    piel.tools.openlane.get_frame_meta_data
    piel.tools.openlane.get_frame_lines_data
    piel.tools.openlane.get_frame_timing_data
    piel.tools.openlane.get_all_timing_data_from_file
    piel.tools.openlane.read_sta_rpt_fwf_file
-   piel.tools.openlane.check_path_exists
-   piel.tools.openlane.read_file
+   piel.tools.openlane.contains_in_lines
+   piel.tools.openlane.create_file_lines_dataframe
+   piel.tools.openlane.get_file_line_by_keyword
+   piel.tools.openlane.read_file_lines
    piel.tools.openlane.run_openlane_flow
 
 
 
-.. py:function:: get_design_directory_from_root_openlane_v1(design_name: str, root_directory: str | pathlib.Path | None = None) -> pathlib.Path
-
-   Gets the design directory from the root directory.
-
-   :param design_name: Name of the design.
-   :type design_name: str
-   :param root_directory: Design directory.
-   :type root_directory: str | pathlib.Path
-
-   :returns: Design directory.
-   :rtype: design_directory(pathlib.Path)
-
-
-.. py:function:: return_path(input_path: piel.config.piel_path_types) -> pathlib.Path
-
-   Returns a pathlib.Path to be able to perform operations accordingly internally.
-
-   This allows us to maintain compatibility between POSIX and Windows systems.
-
-   :param input_path: Input path.
-   :type input_path: str
-
-   :returns: Pathlib path.
-   :rtype: pathlib.Path
-
-
 .. py:function:: get_design_from_openlane_migration(v1: bool = True, design_name_v1: str | None = None, design_directory: str | pathlib.Path | None = None, root_directory_v1: str | pathlib.Path | None = None) -> (str, pathlib.Path)
 
    This function provides the integration mechanism for easily migrating the interconnection with other toolsets from an OpenLane v1 design to an OpenLane v2 design.
 
    This function checks if the inputs are to be treated as v1 inputs. If so, and a `design_name` is provided then it will set the `design_directory` to the corresponding `design_name` directory in the corresponding `root_directory_v1 / designs`. If no `root_directory` is provided then it returns `$OPENLANE_ROOT/"<latest>"/. If a `design_directory` is provided then this will always take precedence even with a `v1` flag.
 
    :param v1: If True, it will migrate from v1 to v2.
    :type v1: bool
    :param design_name_v1: Design name of the v1 design that can be found within `$OPENLANE_ROOT/"<latest>"/designs`.
    :type design_name_v1: str
    :param design_directory: Design directory PATH. Optional path for v2-based designs.
    :type design_directory: str
-   :param root_directory_v1: Root directory of OpenLane v1. If set to None it will return `$OPENLANE_ROOT/"<latest>"
+   :param root_directory_v1: Root directory of OpenLane v1. If set to None it will return `$OPENLANE_ROOT/"<latest>"`
    :type root_directory_v1: str
 
    :returns: None
 
 
 .. py:function:: find_design_run(design_directory: piel.config.piel_path_types, run_name: str | None = None) -> pathlib.Path
 
@@ -250,38 +218,34 @@
    :type configuration: dict
    :param design_directory: Design directory PATH.
    :type design_directory: str
 
    :returns: None
 
 
-.. py:function:: return_path(input_path: piel.config.piel_path_types) -> pathlib.Path
-
-   Returns a pathlib.Path to be able to perform operations accordingly internally.
+.. py:function:: get_all_timing_sta_files(run_directory)
 
-   This allows us to maintain compatibility between POSIX and Windows systems.
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
 
-   :param input_path: Input path.
-   :type input_path: str
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
 
-   :returns: Pathlib path.
-   :rtype: pathlib.Path
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: timing_sta_files_list (list)
 
 
-.. py:function:: get_files_recursively_in_directory(path: piel.config.piel_path_types, extension: str = '*')
+.. py:function:: get_all_power_sta_files(run_directory)
 
-   Returns a list of files in a directory.
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
 
-   :param path: Input path.
-   :type path: piel_path_types
-   :param extension: File extension.
-   :type extension: str
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
 
-   :returns: List of files.
-   :rtype: file_list(list)
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: power_sta_files_list (list)
 
 
 .. py:function:: filter_timing_sta_files(file_list)
 
    Filter the timing sta files from the list of files
 
    :param file_list: List containing the file paths
@@ -298,95 +262,34 @@
    :param file_list: List containing the file paths
    :type file_list: list
 
    :returns: List containing the power sta files
    :rtype: power_sta_files (list)
 
 
-.. py:function:: get_all_timing_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: timing_sta_files_list (list)
-
-
-.. py:function:: get_all_power_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: power_sta_files_list (list)
-
-
-.. py:function:: contains_in_lines(file_lines_data: pandas.DataFrame, keyword: str)
+.. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
-   Check if the keyword is contained in the file lines
+   Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
-   :param keyword: Keyword to search for
-   :type keyword: str
 
-   :returns: Dataframe containing the file lines
-   :rtype: file_lines_data (pd.DataFrame)
+   :returns: Maximum number of frames in the file
+   :rtype: maximum_frame_amount (int)
 
 
-.. py:function:: read_file_lines(file_path: str | pathlib.Path)
+.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
 
-   Extract lines from the file
+   Calculate the propagation delay for each frame in the file
 
    :param file_path: Path to the file
    :type file_path: str | pathlib.Path
 
-   :returns: list containing the file lines
-   :rtype: file_lines_raw (list)
-
-
-.. py:function:: get_file_line_by_keyword(file_lines_data: pandas.DataFrame, keyword: str, regex: str)
-
-   Extract the data from the file lines using the given keyword and regex
-
-   :param file_lines_data: Dataframe containing the file lines
-   :type file_lines_data: pd.DataFrame
-   :param keyword: Keyword to search for
-   :type keyword: str
-   :param regex: Regex to extract the data
-   :type regex: str
-
-   :returns: Dataframe containing the extracted values
-   :rtype: extracted_values (pd.DataFrame)
-
-
-.. py:function:: create_file_lines_dataframe(file_lines_raw)
-
-   Create a DataFrame from the raw lines of a file
-
-   :param file_lines_raw: list containing the file lines
-   :type file_lines_raw: list
-
-   :returns: Dataframe containing the file lines
-   :rtype: file_lines_data (pd.DataFrame)
-
-
-.. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
-
-   Calculate the maximum frame amount based on the frame IDs in the DataFrame
-
-   :param file_lines_data: Dataframe containing the file lines
-   :type file_lines_data: pd.DataFrame
-
-   :returns: Maximum number of frames in the file
-   :rtype: maximum_frame_amount (int)
+   :returns: Dictionary containing the propagation delay
+   :rtype: propagation_delay (dict)
 
 
 .. py:function:: calculate_propagation_delay_from_timing_data(net_name_in: str, net_name_out: str, timing_data: pandas.DataFrame)
 
    Calculate the propagation delay between two nets
 
    :param net_name_in: Name of the input net
@@ -396,25 +299,14 @@
    :param timing_data: Dataframe containing the timing data
    :type timing_data: pd.DataFrame
 
    :returns: Dataframe containing the propagation delay
    :rtype: propagation_delay_dataframe (pd.DataFrame)
 
 
-.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
-
-   Calculate the propagation delay for each frame in the file
-
-   :param file_path: Path to the file
-   :type file_path: str | pathlib.Path
-
-   :returns: Dictionary containing the propagation delay
-   :rtype: propagation_delay (dict)
-
-
 .. py:function:: configure_timing_data_rows(file_lines_data: pandas.DataFrame)
 
    Identify the timing data lines for each frame and creates a metadata dictionary for frames.
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
 
@@ -510,34 +402,62 @@
    :param frame_id: Frame ID to be read
    :type frame_id: int
 
    :returns: DataFrame containing the file data
    :rtype: file_data (pd.DataFrame)
 
 
-.. py:function:: check_path_exists(path: piel.config.piel_path_types, raise_errors: bool = False) -> bool
+.. py:function:: contains_in_lines(file_lines_data: pandas.DataFrame, keyword: str)
+
+   Check if the keyword is contained in the file lines
+
+   :param file_lines_data: Dataframe containing the file lines
+   :type file_lines_data: pd.DataFrame
+   :param keyword: Keyword to search for
+   :type keyword: str
+
+   :returns: Dataframe containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
 
-   Checks if a directory exists.
 
-   :param path: Input path.
-   :type path: piel_path_types
+.. py:function:: create_file_lines_dataframe(file_lines_raw)
 
-   :returns: True if directory exists.
-   :rtype: directory_exists(bool)
+   Create a DataFrame from the raw lines of a file
 
+   :param file_lines_raw: list containing the file lines
+   :type file_lines_raw: list
 
-.. py:function:: read_file(file_path: str | pathlib.Path)
+   :returns: Dataframe containing the file lines
+   :rtype: file_lines_data (pd.DataFrame)
 
-   Read the file from the given path
+
+.. py:function:: get_file_line_by_keyword(file_lines_data: pandas.DataFrame, keyword: str, regex: str)
+
+   Extract the data from the file lines using the given keyword and regex
+
+   :param file_lines_data: Dataframe containing the file lines
+   :type file_lines_data: pd.DataFrame
+   :param keyword: Keyword to search for
+   :type keyword: str
+   :param regex: Regex to extract the data
+   :type regex: str
+
+   :returns: Dataframe containing the extracted values
+   :rtype: extracted_values (pd.DataFrame)
+
+
+.. py:function:: read_file_lines(file_path: str | pathlib.Path)
+
+   Extract lines from the file
 
    :param file_path: Path to the file
    :type file_path: str | pathlib.Path
 
-   :returns: the opened file
-   :rtype: file
+   :returns: list containing the file lines
+   :rtype: file_lines_raw (list)
 
 
 .. py:function:: run_openlane_flow(configuration: dict | None = test_spm_open_lane_configuration, design_directory: piel.config.piel_path_types = '/foss/designs/spm') -> None
 
    Runs the OpenLane flow.
 
    :param configuration: OpenLane configuration dictionary. If none is present it will default to the config.json file on the design_directory.
```

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/openlane/migrate/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/openlane/migrate/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -30,11 +30,11 @@
 
    :param v1: If True, it will migrate from v1 to v2.
    :type v1: bool
    :param design_name_v1: Design name of the v1 design that can be found within `$OPENLANE_ROOT/"<latest>"/designs`.
    :type design_name_v1: str
    :param design_directory: Design directory PATH. Optional path for v2-based designs.
    :type design_directory: str
-   :param root_directory_v1: Root directory of OpenLane v1. If set to None it will return `$OPENLANE_ROOT/"<latest>"
+   :param root_directory_v1: Root directory of OpenLane v1. If set to None it will return `$OPENLANE_ROOT/"<latest>"`
    :type root_directory_v1: str
 
    :returns: None
```

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/openlane/parse/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -27,70 +27,56 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.tools.openlane.parse.return_path
-   piel.tools.openlane.parse.get_files_recursively_in_directory
-   piel.tools.openlane.parse.filter_timing_sta_files
-   piel.tools.openlane.parse.filter_power_sta_files
    piel.tools.openlane.parse.get_all_timing_sta_files
    piel.tools.openlane.parse.get_all_power_sta_files
-   piel.tools.openlane.parse.return_path
-   piel.tools.openlane.parse.contains_in_lines
-   piel.tools.openlane.parse.read_file_lines
-   piel.tools.openlane.parse.get_file_line_by_keyword
-   piel.tools.openlane.parse.create_file_lines_dataframe
+   piel.tools.openlane.parse.filter_timing_sta_files
+   piel.tools.openlane.parse.filter_power_sta_files
    piel.tools.openlane.parse.calculate_max_frame_amount
-   piel.tools.openlane.parse.calculate_propagation_delay_from_timing_data
    piel.tools.openlane.parse.calculate_propagation_delay_from_file
+   piel.tools.openlane.parse.calculate_propagation_delay_from_timing_data
    piel.tools.openlane.parse.configure_timing_data_rows
    piel.tools.openlane.parse.configure_frame_id
    piel.tools.openlane.parse.filter_timing_data_by_net_name_and_type
    piel.tools.openlane.parse.get_frame_meta_data
    piel.tools.openlane.parse.get_frame_lines_data
    piel.tools.openlane.parse.get_frame_timing_data
    piel.tools.openlane.parse.get_all_timing_data_from_file
    piel.tools.openlane.parse.read_sta_rpt_fwf_file
-   piel.tools.openlane.parse.check_path_exists
-   piel.tools.openlane.parse.return_path
    piel.tools.openlane.parse.contains_in_lines
    piel.tools.openlane.parse.create_file_lines_dataframe
    piel.tools.openlane.parse.get_file_line_by_keyword
    piel.tools.openlane.parse.read_file_lines
-   piel.tools.openlane.parse.read_file
-
 
 
-.. py:function:: return_path(input_path: piel.config.piel_path_types) -> pathlib.Path
 
-   Returns a pathlib.Path to be able to perform operations accordingly internally.
+.. py:function:: get_all_timing_sta_files(run_directory)
 
-   This allows us to maintain compatibility between POSIX and Windows systems.
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
 
-   :param input_path: Input path.
-   :type input_path: str
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
 
-   :returns: Pathlib path.
-   :rtype: pathlib.Path
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: timing_sta_files_list (list)
 
 
-.. py:function:: get_files_recursively_in_directory(path: piel.config.piel_path_types, extension: str = '*')
+.. py:function:: get_all_power_sta_files(run_directory)
 
-   Returns a list of files in a directory.
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
 
-   :param path: Input path.
-   :type path: piel_path_types
-   :param extension: File extension.
-   :type extension: str
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
 
-   :returns: List of files.
-   :rtype: file_list(list)
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: power_sta_files_list (list)
 
 
 .. py:function:: filter_timing_sta_files(file_list)
 
    Filter the timing sta files from the list of files
 
    :param file_list: List containing the file paths
@@ -107,108 +93,34 @@
    :param file_list: List containing the file paths
    :type file_list: list
 
    :returns: List containing the power sta files
    :rtype: power_sta_files (list)
 
 
-.. py:function:: get_all_timing_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: timing_sta_files_list (list)
-
-
-.. py:function:: get_all_power_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: power_sta_files_list (list)
-
-
-.. py:function:: return_path(input_path: piel.config.piel_path_types) -> pathlib.Path
-
-   Returns a pathlib.Path to be able to perform operations accordingly internally.
-
-   This allows us to maintain compatibility between POSIX and Windows systems.
-
-   :param input_path: Input path.
-   :type input_path: str
-
-   :returns: Pathlib path.
-   :rtype: pathlib.Path
-
-
-.. py:function:: contains_in_lines(file_lines_data: pandas.DataFrame, keyword: str)
+.. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
-   Check if the keyword is contained in the file lines
+   Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
-   :param keyword: Keyword to search for
-   :type keyword: str
 
-   :returns: Dataframe containing the file lines
-   :rtype: file_lines_data (pd.DataFrame)
+   :returns: Maximum number of frames in the file
+   :rtype: maximum_frame_amount (int)
 
 
-.. py:function:: read_file_lines(file_path: str | pathlib.Path)
+.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
 
-   Extract lines from the file
+   Calculate the propagation delay for each frame in the file
 
    :param file_path: Path to the file
    :type file_path: str | pathlib.Path
 
-   :returns: list containing the file lines
-   :rtype: file_lines_raw (list)
-
-
-.. py:function:: get_file_line_by_keyword(file_lines_data: pandas.DataFrame, keyword: str, regex: str)
-
-   Extract the data from the file lines using the given keyword and regex
-
-   :param file_lines_data: Dataframe containing the file lines
-   :type file_lines_data: pd.DataFrame
-   :param keyword: Keyword to search for
-   :type keyword: str
-   :param regex: Regex to extract the data
-   :type regex: str
-
-   :returns: Dataframe containing the extracted values
-   :rtype: extracted_values (pd.DataFrame)
-
-
-.. py:function:: create_file_lines_dataframe(file_lines_raw)
-
-   Create a DataFrame from the raw lines of a file
-
-   :param file_lines_raw: list containing the file lines
-   :type file_lines_raw: list
-
-   :returns: Dataframe containing the file lines
-   :rtype: file_lines_data (pd.DataFrame)
-
-
-.. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
-
-   Calculate the maximum frame amount based on the frame IDs in the DataFrame
-
-   :param file_lines_data: Dataframe containing the file lines
-   :type file_lines_data: pd.DataFrame
-
-   :returns: Maximum number of frames in the file
-   :rtype: maximum_frame_amount (int)
+   :returns: Dictionary containing the propagation delay
+   :rtype: propagation_delay (dict)
 
 
 .. py:function:: calculate_propagation_delay_from_timing_data(net_name_in: str, net_name_out: str, timing_data: pandas.DataFrame)
 
    Calculate the propagation delay between two nets
 
    :param net_name_in: Name of the input net
@@ -218,25 +130,14 @@
    :param timing_data: Dataframe containing the timing data
    :type timing_data: pd.DataFrame
 
    :returns: Dataframe containing the propagation delay
    :rtype: propagation_delay_dataframe (pd.DataFrame)
 
 
-.. py:function:: calculate_propagation_delay_from_file(file_path: str | pathlib.Path)
-
-   Calculate the propagation delay for each frame in the file
-
-   :param file_path: Path to the file
-   :type file_path: str | pathlib.Path
-
-   :returns: Dictionary containing the propagation delay
-   :rtype: propagation_delay (dict)
-
-
 .. py:function:: configure_timing_data_rows(file_lines_data: pandas.DataFrame)
 
    Identify the timing data lines for each frame and creates a metadata dictionary for frames.
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
 
@@ -332,38 +233,14 @@
    :param frame_id: Frame ID to be read
    :type frame_id: int
 
    :returns: DataFrame containing the file data
    :rtype: file_data (pd.DataFrame)
 
 
-.. py:function:: check_path_exists(path: piel.config.piel_path_types, raise_errors: bool = False) -> bool
-
-   Checks if a directory exists.
-
-   :param path: Input path.
-   :type path: piel_path_types
-
-   :returns: True if directory exists.
-   :rtype: directory_exists(bool)
-
-
-.. py:function:: return_path(input_path: piel.config.piel_path_types) -> pathlib.Path
-
-   Returns a pathlib.Path to be able to perform operations accordingly internally.
-
-   This allows us to maintain compatibility between POSIX and Windows systems.
-
-   :param input_path: Input path.
-   :type input_path: str
-
-   :returns: Pathlib path.
-   :rtype: pathlib.Path
-
-
 .. py:function:: contains_in_lines(file_lines_data: pandas.DataFrame, keyword: str)
 
    Check if the keyword is contained in the file lines
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
    :param keyword: Keyword to search for
@@ -404,18 +281,7 @@
    Extract lines from the file
 
    :param file_path: Path to the file
    :type file_path: str | pathlib.Path
 
    :returns: list containing the file lines
    :rtype: file_lines_raw (list)
-
-
-.. py:function:: read_file(file_path: str | pathlib.Path)
-
-   Read the file from the given path
-
-   :param file_path: Path to the file
-   :type file_path: str | pathlib.Path
-
-   :returns: the opened file
-   :rtype: file
```

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/openlane/parse/utils/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/utils/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 .. autoapisummary::
 
    piel.tools.openlane.parse.utils.contains_in_lines
    piel.tools.openlane.parse.utils.create_file_lines_dataframe
    piel.tools.openlane.parse.utils.get_file_line_by_keyword
    piel.tools.openlane.parse.utils.read_file_lines
-   piel.tools.openlane.parse.utils.read_file
 
 
 
 .. py:function:: contains_in_lines(file_lines_data: pandas.DataFrame, keyword: str)
 
    Check if the keyword is contained in the file lines
 
@@ -65,18 +64,7 @@
    Extract lines from the file
 
    :param file_path: Path to the file
    :type file_path: str | pathlib.Path
 
    :returns: list containing the file lines
    :rtype: file_lines_raw (list)
-
-
-.. py:function:: read_file(file_path: str | pathlib.Path)
-
-   Read the file from the given path
-
-   :param file_path: Path to the file
-   :type file_path: str | pathlib.Path
-
-   :returns: the opened file
-   :rtype: file
```

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/openlane/utils/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/openlane/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/openlane/v1/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/openlane/v1/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/openlane/v2/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/openlane/v2/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/sax/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/sax/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/tools/sax/utils/index.rst` & `piel-0.0.41/docs/autoapi/piel/tools/sax/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/visual/auto_plot_multiple/index.rst` & `piel-0.0.41/docs/autoapi/piel/visual/auto_plot_multiple/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/visual/data_conversion/index.rst` & `piel-0.0.41/docs/autoapi/piel/visual/data_conversion/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/autoapi/piel/visual/index.rst` & `piel-0.0.41/docs/autoapi/piel/visual/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/conf.py` & `piel-0.0.41/docs/conf.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/examples/designs/simple_design/simple_design/tb/default/Makefile` & `piel-0.0.41/docs/examples/designs/simple_design/simple_design/tb/default/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/index.rst` & `piel-0.0.41/docs/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/make.bat` & `piel-0.0.41/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/docs/sections/microservices/dependencies/cocotb.rst` & `piel-0.0.41/docs/sections/microservices/dependencies/cocotb.rst`

 * *Files 0% similar despite different names*

```diff
@@ -55,13 +55,13 @@
 00000360: 672f 656e 2f73 7461 626c 652f 7369 6d75  g/en/stable/simu
 00000370: 6c61 746f 725f 7375 7070 6f72 742e 6874  lator_support.ht
 00000380: 6d6c 3e60 5f5f 0a2d 2020 6047 4844 4c20  ml>`__.-  `GHDL 
 00000390: 3c68 7474 7073 3a2f 2f64 6f63 732e 636f  <https://docs.co
 000003a0: 636f 7462 2e6f 7267 2f65 6e2f 7374 6162  cotb.org/en/stab
 000003b0: 6c65 2f73 696d 756c 6174 6f72 5f73 7570  le/simulator_sup
 000003c0: 706f 7274 2e68 746d 6c3e 605f 5f0a 0a2e  port.html>`__...
-000003d0: 2e20 746f 6374 7265 653a 3a0a 2020 2020  . toctree::.    
-000003e0: 636f 636f 7462 5f75 7365 6675 6c5f 636f  cocotb_useful_co
-000003f0: 6d6d 616e 6473 0a20 2020 202e 2e2f 2e2e  mmands.    ../..
-00000400: 2f2e 2e2f 6175 746f 6170 692f 7069 656c  /../autoapi/piel
-00000410: 2f74 6f6f 6c73 2f63 6f63 6f74 622f 696e  /tools/cocotb/in
-00000420: 6465 782e 7273 740a                      dex.rst.
+000003d0: 2e20 746f 6374 7265 653a 3a0a 0a20 2020  . toctree::..   
+000003e0: 2063 6f63 6f74 625f 7573 6566 756c 5f63   cocotb_useful_c
+000003f0: 6f6d 6d61 6e64 730a 2020 2020 2e2e 2f2e  ommands.    ../.
+00000400: 2e2f 2e2e 2f61 7574 6f61 7069 2f70 6965  ./../autoapi/pie
+00000410: 6c2f 746f 6f6c 732f 636f 636f 7462 2f69  l/tools/cocotb/i
+00000420: 6e64 6578 2e72 7374 0a                   ndex.rst.
```

### Comparing `piel-0.0.40/docs/sections/microservices/dependencies/openlane.rst` & `piel-0.0.41/docs/sections/microservices/dependencies/openlane.rst`

 * *Files 16% similar despite different names*

```diff
@@ -39,11 +39,11 @@
 00000260: 6e61 6269 6c69 7479 2065 7863 6570 7420  nability except 
 00000270: 7768 656e 0a65 7870 6c69 6369 746c 7920  when.explicitly 
 00000280: 6675 6e63 7469 6f6e 7320 6361 6e20 6265  functions can be
 00000290: 2073 6861 7265 642e 2054 6869 7320 6973   shared. This is
 000002a0: 2069 6e20 7468 6520 6361 7365 206f 6620   in the case of 
 000002b0: 696e 7465 726e 616c 0a66 756e 6374 696f  internal.functio
 000002c0: 6e61 6c69 7479 2e0a 0a2e 2e20 746f 6374  nality..... toct
-000002d0: 7265 653a 3a0a 2020 2020 2e2e 2f2e 2e2f  ree::.    ../../
-000002e0: 2e2e 2f61 7574 6f61 7069 2f70 6965 6c2f  ../autoapi/piel/
-000002f0: 746f 6f6c 732f 6f70 656e 6c61 6e65 2f69  tools/openlane/i
-00000300: 6e64 6578 2e72 7374 0a                   ndex.rst.
+000002d0: 7265 653a 3a0a 0a20 2020 202e 2e2f 2e2e  ree::..    ../..
+000002e0: 2f2e 2e2f 6175 746f 6170 692f 7069 656c  /../autoapi/piel
+000002f0: 2f74 6f6f 6c73 2f6f 7065 6e6c 616e 652f  /tools/openlane/
+00000300: 696e 6465 782e 7273 740a                 index.rst.
```

### Comparing `piel-0.0.40/docs/sections/microservices/dependencies/sax.rst` & `piel-0.0.41/docs/sections/microservices/dependencies/sax.rst`

 * *Files 0% similar despite different names*

```diff
@@ -179,10 +179,10 @@
 00000b20: 6e61 7269 6573 2073 686f 756c 6420 636f  naries should co
 00000b30: 7272 6573 706f 6e64 2074 6f20 7468 6520  rrespond to the 
 00000b40: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
 00000b50: 7320 6f66 2065 6163 6820 696e 6469 7669  s of each indivi
 00000b60: 6475 616c 2073 7562 636f 6d70 6f6e 656e  dual subcomponen
 00000b70: 742e 0a0a 0a0a 0a41 5049 0a2d 2d2d 2d2d  t......API.-----
 00000b80: 2d0a 0a2e 2e20 746f 6374 7265 653a 3a0a  -.... toctree::.
-00000b90: 2020 2020 2e2e 2f2e 2e2f 2e2e 2f61 7574      ../../../aut
-00000ba0: 6f61 7069 2f70 6965 6c2f 746f 6f6c 732f  oapi/piel/tools/
-00000bb0: 7361 782f 696e 6465 782e 7273 740a       sax/index.rst.
+00000b90: 0a20 2020 202e 2e2f 2e2e 2f2e 2e2f 6175  .    ../../../au
+00000ba0: 746f 6170 692f 7069 656c 2f74 6f6f 6c73  toapi/piel/tools
+00000bb0: 2f73 6178 2f69 6e64 6578 2e72 7374 0a    /sax/index.rst.
```

### Comparing `piel-0.0.40/docs/sections/microservices/integration/sax_qutip.rst` & `piel-0.0.41/docs/sections/microservices/integration/sax_qutip.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/piel/__init__.py` & `piel-0.0.41/piel/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import pathlib
 
 # Libraries
 from piel import components  # NOQA: F401
 from piel import models  # NOQA: F401
 from piel import visual  # NOQA: F401
-from piel import tools  # NOQA: F401
 
 # Functions
 
 from .config import *
 from .defaults import *
 from .file_system import *
 from .integration import *
@@ -20,8 +19,8 @@
 
 os.environ["PIEL_PACKAGE_DIRECTORY"] = str(
     pathlib.Path(__file__).parent.parent.resolve()
 )
 
 __author__ = """Dario Quintero"""
 __email__ = "darioaquintero@gmail.com"
-__version__ = "0.0.40"
+__version__ = "0.0.41"
```

### Comparing `piel-0.0.40/piel/config.py` & `piel-0.0.41/piel/config.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 The numerical solver is normally delegated for as `numpy` but there are cases where a much faster solver is desired, and where different functioanlity is required. For example, `sax` uses `JAX` for its numerical solver. In this case, we will create a global numerical solver that we can use throughout the project, and that can be extended and solved accordingly for the particular project requirements.
 """
 import pathlib
 import sys
 import types
 
+__all__ = [
+    "numerical_solver",
+    "nso",
+    "piel_path_types",
+]
+
 
 if "jax" in sys.modules:
     import jax.numpy as jnp
 
     numerical_solver = jnp
 elif "numpy" in sys.modules:
     import numpy
@@ -19,13 +25,7 @@
 else:
     import numpy
 
     numerical_solver = numpy
 
 nso = numerical_solver
 piel_path_types = str | pathlib.Path | types.ModuleType
-
-__all__ = [
-    "numerical_solver",
-    "nso",
-    "piel_path_types",
-]
```

### Comparing `piel-0.0.40/piel/defaults.py` & `piel-0.0.41/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/piel/file_conversion.py` & `piel-0.0.41/piel/file_conversion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import pandas as pd
 from pyDigitalWaveTools.vcd.parser import VcdParser
 from .file_system import return_path
 from .config import piel_path_types
 
+__all__ = [
+    "read_csv_to_pandas",
+    "read_vcd_to_json",
+]
+
 
 def read_csv_to_pandas(file_path: piel_path_types):
     """
     This function returns a Pandas dataframe that contains all the simulation data outputted from the simulation run.
     """
     file_path = return_path(file_path)
     simulation_data = pd.read_csv(file_path)
```

### Comparing `piel-0.0.40/piel/file_system.py` & `piel-0.0.41/piel/file_system.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,32 @@
 import stat
 import subprocess
 import types
 from typing import Literal
 from .config import piel_path_types
 
 
+__all__ = [
+    "check_path_exists",
+    "check_example_design",
+    "copy_source_folder",
+    "create_new_directory",
+    "delete_path",
+    "delete_path_list_in_directory",
+    "get_files_recursively_in_directory",
+    "permit_directory_all",
+    "permit_script_execution",
+    "setup_example_design",
+    "read_json",
+    "return_path",
+    "run_script",
+    "write_script",
+]
+
+
 def check_path_exists(
     path: piel_path_types,
     raise_errors: bool = False,
 ) -> bool:
     """
     Checks if a directory exists.
 
@@ -387,25 +405,7 @@
                     + ". Your Python executable might not have the required permissions. Restructure your project directory so Python does not have to change permissions."
                 )
             )
 
     file = open(str(directory_path / script_name), "w")
     file.write(script)
     file.close()
-
-
-__all__ = [
-    "check_path_exists",
-    "check_example_design",
-    "copy_source_folder",
-    "create_new_directory",
-    "delete_path",
-    "delete_path_list_in_directory",
-    "get_files_recursively_in_directory",
-    "permit_directory_all",
-    "permit_script_execution",
-    "setup_example_design",
-    "read_json",
-    "return_path",
-    "run_script",
-    "write_script",
-]
```

### Comparing `piel-0.0.40/piel/integration/openlane_gdsfactory_core.py` & `piel-0.0.41/piel/integration/openlane_gdsfactory_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 """
 import gdsfactory as gf
 from ..config import piel_path_types
 from ..file_system import check_path_exists
 from piel.tools.openlane.migrate import get_design_from_openlane_migration
 from piel.tools.openlane import find_design_run
 
+__all__ = ["create_gdsfactory_component_from_openlane"]
+
 
 def create_gdsfactory_component_from_openlane(
     design_name_v1: str | None = None,
     design_directory: piel_path_types | None = None,
     run_name: str | None = None,
     v1: bool = True,
 ) -> gf.Component:
@@ -42,10 +44,7 @@
         / "final"
         / "gds"
         / (design_name + ".gds")
     )
     check_path_exists(final_gds_run, raise_errors=True)
     component = gf.import_gds(final_gds_run, name=design_name)
     return component
-
-
-__all__ = ["create_gdsfactory_component_from_openlane"]
```

### Comparing `piel-0.0.40/piel/integration/sax_qutip.py` & `piel-0.0.41/piel/integration/sax_qutip.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 
     ..code-block:: python
 
         import numpy as np
         import qutip
 
         # S-Gate
-        s_gate_matrix = np.array([[1.,   0],
-                                 [0., 1.j]])
+        s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
         s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
     In mathematical notation, this S-gate would be written as:
 
     ..math::
 
         S = \\begin{bmatrix}
@@ -67,16 +66,15 @@
     For example, a ``qutip`` representation of an s-gate gate would be:
 
     ..code-block:: python
 
         import numpy as np
         import qutip
         # S-Gate
-        s_gate_matrix = np.array([[1.,   0],
-                                 [0., 1.j]])
+        s_gate_matrix = np.array([[1.,   0], [0., 1.j]])
         s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
     In mathematical notation, this S-gate would be written as:
 
     ..math::
 
         S = \\begin{bmatrix}
```

### Comparing `piel-0.0.40/piel/models/frequency/photonic/directional_coupler_length.py` & `piel-0.0.41/piel/models/frequency/photonic/directional_coupler_length.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Translated from https://github.com/flaport/sax or https://github.com/flaport/photontorch/tree/master
 """
 import sax
 from ....config import nso
 
+__all__ = ["directional_coupler_with_length"]
+
 
 def directional_coupler_with_length(
     length=1e-5, coupling=0.5, loss=0, neff=2.34, wl0=1.55e-6, ng=3.40, phase=0
 ):
     kappa = coupling**0.5
     tau = (1 - coupling) ** 0.5
     loss = 10 ** (-loss * length / 20)  # factor 20 bc amplitudes, not intensities.
```

### Comparing `piel-0.0.40/piel/models/frequency/photonic/directional_coupler_real.py` & `piel-0.0.41/piel/models/frequency/photonic/directional_coupler_real.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/piel/models/frequency/photonic/grating_coupler.py` & `piel-0.0.41/piel/models/frequency/photonic/grating_coupler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Translated from https://github.com/flaport/sax or https://github.com/flaport/photontorch/tree/master
 """
 from ....config import nso
 
+__all__ = ["grating_coupler_simple"]
 
-def grating_coupler(R=0.0, R_in=0.0, Tmax=1.0, bandwidth=0.06e-6, wl0=1.55e-6):
+
+def grating_coupler_simple(R=0.0, R_in=0.0, Tmax=1.0, bandwidth=0.06e-6, wl0=1.55e-6):
     # Constants
     fwhm2sigma = 1.0 / (2 * nso.sqrt(2 * nso.log(2)))
 
     # Compute sigma
     sigma = fwhm2sigma * bandwidth
 
     # Assume the wavelength of the environment matches the center wavelength of the grating coupler
```

### Comparing `piel-0.0.40/piel/models/frequency/photonic/straight_waveguide.py` & `piel-0.0.41/piel/models/frequency/photonic/straight_waveguide.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/piel/models/logic/electro_optic/signal_mapping.py` & `piel-0.0.41/piel/models/logic/electro_optic/signal_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 In this function we implement different methods of mapping electronic signals to phase.
 
 One particular implementation of phase mapping would be:
 
 .. list-table:: Example Basic Phase Mapping
    :header-rows: 1
+
    * - Bit
      - Phase
    * - b0
-     - :math:`\phi_0 \to 0`
+     - :math:`\\phi_0 \\to 0`
    * - b1
-     - :math:`\phi_1 \to \pi`
+     - :math:`\\phi_1 \\to \\pi`
 
 We can define the two corresponding angles that this would be.
 
 A more complex implementation of phase mapping can be similar to a DAC mapping: a bitstring within a converter bit-size can map directly to a particular phase space within a particular mapping.
 """
 import numpy as np
 import pandas as pd
```

### Comparing `piel-0.0.40/piel/parametric.py` & `piel-0.0.41/piel/parametric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import itertools
 
+__all__ = [
+    "single_parameter_sweep",
+    "multi_parameter_sweep",
+]
+
 
 def single_parameter_sweep(
     base_design_configuration: dict,
     parameter_name: str,
     parameter_sweep_values: list,
 ):
     """
@@ -74,13 +79,7 @@
         parameter_index = 0
         for parameter in parameter_combination:
             design[parameter_names_sweep_list[parameter_index]] = parameter
             parameter_index += 1
         parameter_sweep_design_dictionary_array.extend([design])
 
     return parameter_sweep_design_dictionary_array
-
-
-__all__ = [
-    "single_parameter_sweep",
-    "multi_parameter_sweep",
-]
```

### Comparing `piel-0.0.40/piel/project_structure.py` & `piel-0.0.41/piel/project_structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """
 This file allows us to automate several aspects of creating a fully compatible project structure.
 """
 from .config import piel_path_types
 from .file_system import return_path, write_script, read_json, check_path_exists
 
+__all__ = [
+    "read_configuration",
+    "create_setup_py_from_config_json",
+]
+
 
 def read_configuration(design_directory: piel_path_types) -> dict:
     """
     This function reads the configuration file found in the design directory.
 
     Args:
         design_directory(piel_path_types): Design directory PATH.
```

### Comparing `piel-0.0.40/piel/tools/cocotb/core.py` & `piel-0.0.41/piel/tools/cocotb/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 """
 import functools
 import pathlib
 import subprocess
 from typing import Literal
 from piel.file_system import return_path, write_script, delete_path_list_in_directory
 
+__all__ = [
+    "check_cocotb_testbench_exists",
+    "configure_cocotb_simulation",
+    "delete_simulation_output_files",
+    "run_cocotb_simulation",
+]
+
 
 def check_cocotb_testbench_exists(
     design_directory: str | pathlib.Path,
 ) -> bool:
     """
     Checks if a cocotb testbench exists in the design directory.
 
@@ -163,15 +170,7 @@
     write_script(
         directory_path=test_directory,
         script=script,
         script_name="run_cocotb_simulation.sh",
     )
     run = subprocess.run(script, capture_output=True, shell=True, check=True)
     return run
-
-
-__all__ = [
-    "check_cocotb_testbench_exists",
-    "configure_cocotb_simulation",
-    "delete_simulation_output_files",
-    "run_cocotb_simulation",
-]
```

### Comparing `piel-0.0.40/piel/tools/cocotb/data.py` & `piel-0.0.41/piel/tools/cocotb/data.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/piel/tools/gdsfactory/netlist.py` & `piel-0.0.41/piel/tools/gdsfactory/netlist.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/piel/tools/openlane/migrate.py` & `piel-0.0.41/piel/tools/openlane/migrate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """
 These functions provide easy tools for easily migrating between OpenLane v1 and v2 based designs.
 """
 import pathlib
 from .v1 import get_design_directory_from_root_openlane_v1
 from piel.file_system import return_path
 
+__all__ = [
+    "get_design_from_openlane_migration",
+]
+
 
 def get_design_from_openlane_migration(
     v1: bool = True,
     design_name_v1: str | None = None,
     design_directory: str | pathlib.Path | None = None,
     root_directory_v1: str | pathlib.Path | None = None,
 ) -> (str, pathlib.Path):
@@ -17,15 +21,15 @@
 
     This function checks if the inputs are to be treated as v1 inputs. If so, and a `design_name` is provided then it will set the `design_directory` to the corresponding `design_name` directory in the corresponding `root_directory_v1 / designs`. If no `root_directory` is provided then it returns `$OPENLANE_ROOT/"<latest>"/. If a `design_directory` is provided then this will always take precedence even with a `v1` flag.
 
     Args:
         v1(bool): If True, it will migrate from v1 to v2.
         design_name_v1(str): Design name of the v1 design that can be found within `$OPENLANE_ROOT/"<latest>"/designs`.
         design_directory(str): Design directory PATH. Optional path for v2-based designs.
-        root_directory_v1(str): Root directory of OpenLane v1. If set to None it will return `$OPENLANE_ROOT/"<latest>"
+        root_directory_v1(str): Root directory of OpenLane v1. If set to None it will return `$OPENLANE_ROOT/"<latest>"`
 
     Returns:
         None
     """
     if design_directory is not None:
         design_directory = return_path(design_directory)
         design_name = design_directory.name
```

### Comparing `piel-0.0.40/piel/tools/openlane/parse/sta_rpt.py` & `piel-0.0.41/piel/tools/openlane/parse/sta_rpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,28 @@
 from .utils import (
     contains_in_lines,
     read_file_lines,
     get_file_line_by_keyword,
     create_file_lines_dataframe,
 )
 
+__all__ = [
+    "calculate_max_frame_amount",
+    "calculate_propagation_delay_from_file",
+    "calculate_propagation_delay_from_timing_data",
+    "configure_timing_data_rows",
+    "configure_frame_id",
+    "filter_timing_data_by_net_name_and_type",
+    "get_frame_meta_data",
+    "get_frame_lines_data",
+    "get_frame_timing_data",
+    "get_all_timing_data_from_file",
+    "read_sta_rpt_fwf_file",
+]
+
 
 def calculate_max_frame_amount(
     file_lines_data: pd.DataFrame,
 ):
     """
     Calculate the maximum frame amount based on the frame IDs in the DataFrame
```

### Comparing `piel-0.0.40/piel/tools/openlane/parse/utils.py` & `piel-0.0.41/piel/tools/openlane/parse/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import pandas as pd
 import pathlib
 from piel.file_system import check_path_exists, return_path
 
+__all__ = [
+    "contains_in_lines",
+    "create_file_lines_dataframe",
+    "get_file_line_by_keyword",
+    "read_file_lines",
+]
+
 
 def contains_in_lines(
     file_lines_data: pd.DataFrame,
     keyword: str,
 ):
     """
     Check if the keyword is contained in the file lines
```

### Comparing `piel-0.0.40/piel/tools/openlane/utils.py` & `piel-0.0.41/piel/tools/openlane/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import pathlib
 from piel.config import piel_path_types
 from piel.file_system import return_path
 
+__all__ = [
+    "find_design_run",
+]
+
 
 def find_design_run(
     design_directory: piel_path_types,
     run_name: str | None = None,
 ) -> pathlib.Path:
     """
     For a given `design_directory`, the `openlane` output can be found in the `runs` subdirectory.
@@ -36,12 +40,7 @@
             run_path = latest_run
         else:
             # If there are no runs
             raise ValueError(
                 "No OpenLane design runs were found in: " + str(runs_design_directory)
             )
     return run_path
-
-
-__all__ = [
-    "find_design_run",
-]
```

### Comparing `piel-0.0.40/piel/tools/openlane/v1.py` & `piel-0.0.41/piel/tools/openlane/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,27 @@
     permit_script_execution,
     read_json,
     return_path,
     run_script,
     write_script,
 )
 
+__all__ = [
+    "check_config_json_exists_openlane_v1",
+    "check_design_exists_openlane_v1",
+    "configure_and_run_design_openlane_v1",
+    "configure_parametric_designs_openlane_v1",
+    "configure_flow_script_openlane_v1",
+    "create_parametric_designs_openlane_v1",
+    "get_design_directory_from_root_openlane_v1",
+    "get_latest_version_root_openlane_v1",
+    "read_configuration_openlane_v1",
+    "write_configuration_openlane_v1",
+]
+
 
 def check_config_json_exists_openlane_v1(
     design_name: str,
     root_directory: str | pathlib.Path | None = None,
 ) -> bool:
     """
     Checks if a design has a `config.json` file.
@@ -310,21 +323,7 @@
         design_directory(str): Design directory PATH.
 
     Returns:
         None
     """
     with open(str((design_directory / "config.json").resolve()), "w") as write_file:
         json.dump(configuration, write_file, indent=4)
-
-
-__all__ = [
-    "check_config_json_exists_openlane_v1",
-    "check_design_exists_openlane_v1",
-    "configure_and_run_design_openlane_v1",
-    "configure_parametric_designs_openlane_v1",
-    "configure_flow_script_openlane_v1",
-    "create_parametric_designs_openlane_v1",
-    "get_design_directory_from_root_openlane_v1",
-    "get_latest_version_root_openlane_v1",
-    "read_configuration_openlane_v1",
-    "write_configuration_openlane_v1",
-]
```

### Comparing `piel-0.0.40/piel/tools/openlane/v2.py` & `piel-0.0.41/piel/tools/openlane/v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import openlane
 from piel.config import piel_path_types
 from piel.file_system import return_path, read_json
 from piel.defaults import test_spm_open_lane_configuration
 
+__all__ = ["run_openlane_flow"]
+
 
 def run_openlane_flow(
     configuration: dict | None = test_spm_open_lane_configuration,
     design_directory: piel_path_types = "/foss/designs/spm",
 ) -> None:
     """
     Runs the OpenLane flow.
@@ -28,10 +30,7 @@
 
     flow = Classic(
         config=configuration,
         design_dir=str(design_directory.resolve()),
     )
 
     flow.start()
-
-
-__all__ = ["run_openlane_flow"]
```

### Comparing `piel-0.0.40/piel/tools/sax/utils.py` & `piel-0.0.41/piel/tools/sax/utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/piel/visual/auto_plot_multiple.py` & `piel-0.0.41/piel/visual/auto_plot_multiple.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/piel/visual/data_conversion.py` & `piel-0.0.41/piel/visual/data_conversion.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/piel.egg-info/PKG-INFO` & `piel-0.0.41/piel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.40
+Version: 0.0.41
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -47,14 +47,15 @@
 ## Microservices Toolset
 This package provides interconnection functions to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
 
 Some existing microservice dependency integrations are:
 * [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
 * [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
 * [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
+* [pyspice](https://github.com/PySpice-org/PySpice) - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
 * [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
 * [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in Python
 
 ## Environment Requirements
 * Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
```

### Comparing `piel-0.0.40/piel.egg-info/SOURCES.txt` & `piel-0.0.41/piel.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 docs/autoapi/piel/models/logic/electronic/index.rst
 docs/autoapi/piel/models/logic/opto_electronic/index.rst
 docs/autoapi/piel/models/logic/photonic/index.rst
 docs/autoapi/piel/models/physical/index.rst
 docs/autoapi/piel/models/physical/electrical/index.rst
 docs/autoapi/piel/models/physical/electrical/cable/index.rst
 docs/autoapi/piel/models/physical/electro_optic/index.rst
+docs/autoapi/piel/models/physical/electro_optic/basic_heater/index.rst
 docs/autoapi/piel/models/physical/electronic/index.rst
 docs/autoapi/piel/models/physical/geometry/index.rst
 docs/autoapi/piel/models/physical/opto_electronic/index.rst
 docs/autoapi/piel/models/physical/photonic/index.rst
 docs/autoapi/piel/models/physical/thermal/index.rst
 docs/autoapi/piel/models/physical/units/index.rst
 docs/autoapi/piel/models/transient/index.rst
@@ -94,14 +95,16 @@
 docs/sections/components/index.rst
 docs/sections/environment/index.rst
 docs/sections/microservices/index.rst
 docs/sections/microservices/dependencies/cocotb.rst
 docs/sections/microservices/dependencies/gdsfactory.rst
 docs/sections/microservices/dependencies/index.rst
 docs/sections/microservices/dependencies/openlane.rst
+docs/sections/microservices/dependencies/principle.rst
+docs/sections/microservices/dependencies/pyspice.rst
 docs/sections/microservices/dependencies/sax.rst
 docs/sections/microservices/integration/index.rst
 docs/sections/microservices/integration/sax_qutip.rst
 docs/sections/models/index.rst
 piel/__init__.py
 piel/cli.py
 piel/config.py
@@ -152,14 +155,15 @@
 piel/models/physical/__init__.py
 piel/models/physical/geometry.py
 piel/models/physical/thermal.py
 piel/models/physical/units.py
 piel/models/physical/electrical/__init__.py
 piel/models/physical/electrical/cable.py
 piel/models/physical/electro_optic/__init__.py
+piel/models/physical/electro_optic/basic_heater.py
 piel/models/physical/electronic/__init__.py
 piel/models/physical/opto_electronic/__init__.py
 piel/models/physical/photonic/__init__.py
 piel/models/transient/__init__.py
 piel/models/transient/electrical/__init__.py
 piel/models/transient/electro_optic/__init__.py
 piel/models/transient/electronic/__init__.py
```

### Comparing `piel-0.0.40/setup.py` & `piel-0.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "jupyter_bokeh",
     "jupytext",
     "Click>=7.0",
     "cocotb",
     "gdsfactory",
     "openlane",
     "pandas",
+    "pyspice",
     "sax",
     "qutip",
 ]
 
 test_requirements = [
     "pytest>=3",
 ]
@@ -66,10 +67,10 @@
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/daquintero/piel",
-    version="0.0.40",
+    version="0.0.41",
     zip_safe=False,
 )
```

### Comparing `piel-0.0.40/tests/models/logic/electro_optic/test_signal_mapping.py` & `piel-0.0.41/tests/models/logic/electro_optic/test_signal_mapping.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/tests/test_piel.py` & `piel-0.0.41/tests/test_piel.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/tests/tools/gdsfactory/test_netlist.py` & `piel-0.0.41/tests/tools/gdsfactory/test_netlist.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/tests/tools/sax/test_utils.py` & `piel-0.0.41/tests/tools/sax/test_utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.40/tests/visual/test_data_conversion.py` & `piel-0.0.41/tests/visual/test_data_conversion.py`

 * *Files identical despite different names*

