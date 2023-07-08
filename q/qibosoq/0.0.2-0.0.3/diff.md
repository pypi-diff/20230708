# Comparing `tmp/qibosoq-0.0.2.tar.gz` & `tmp/qibosoq-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibosoq-0.0.2.tar", max compression
+gzip compressed data, was "qibosoq-0.0.3.tar", max compression
```

## Comparing `qibosoq-0.0.2.tar` & `qibosoq-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-06-30 10:59:10.736272 qibosoq-0.0.2/LICENSE
--rw-r--r--   0        0        0     2363 2023-06-30 10:59:10.736272 qibosoq-0.0.2/README.md
--rw-r--r--   0        0        0     1547 2023-06-30 10:59:10.740272 qibosoq-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       94 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/__init__.py
--rw-r--r--   0        0        0      428 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/__main__.py
--rw-r--r--   0        0        0       22 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/components/__init__.py
--rw-r--r--   0        0        0     2176 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/components/base.py
--rw-r--r--   0        0        0     1388 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/components/pulses.py
--rw-r--r--   0        0        0     1021 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/configuration.py
--rw-r--r--   0        0        0     1063 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/log.py
--rw-r--r--   0        0        0       23 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/programs/__init__.py
--rw-r--r--   0        0        0    13726 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/programs/base.py
--rw-r--r--   0        0        0     2974 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/programs/flux.py
--rw-r--r--   0        0        0      917 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/programs/pulse_sequence.py
--rw-r--r--   0        0        0     5166 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/programs/sweepers.py
--rw-r--r--   0        0        0     4782 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/rfsoc_server.py
--rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 qibosoq-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-08 08:29:21.041516 qibosoq-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2577 2023-07-08 08:29:21.041516 qibosoq-0.0.3/README.md
+-rw-r--r--   0        0        0     1610 2023-07-08 08:29:21.045516 qibosoq-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       94 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/__init__.py
+-rw-r--r--   0        0        0      428 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/__main__.py
+-rw-r--r--   0        0        0     2086 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/client.py
+-rw-r--r--   0        0        0       22 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/components/__init__.py
+-rw-r--r--   0        0        0     2176 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/components/base.py
+-rw-r--r--   0        0        0     1670 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/components/pulses.py
+-rw-r--r--   0        0        0     1021 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/configuration.py
+-rw-r--r--   0        0        0     1063 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/log.py
+-rw-r--r--   0        0        0       23 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/programs/__init__.py
+-rw-r--r--   0        0        0    13923 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/programs/base.py
+-rw-r--r--   0        0        0     2964 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/programs/flux.py
+-rw-r--r--   0        0        0      917 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/programs/pulse_sequence.py
+-rw-r--r--   0        0        0     4910 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/programs/sweepers.py
+-rw-r--r--   0        0        0     4737 2023-07-08 08:29:21.045516 qibosoq-0.0.3/src/qibosoq/rfsoc_server.py
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 qibosoq-0.0.3/PKG-INFO
```

### Comparing `qibosoq-0.0.2/LICENSE` & `qibosoq-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qibosoq-0.0.2/README.md` & `qibosoq-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Qibosoq
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083286.svg)](https://doi.org/10.5281/zenodo.8083286)
+![Tests](https://github.com/qiboteam/qibosoq/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/qiboteam/qibosoq/branch/main/graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibosoq)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083285.svg)](https://doi.org/10.5281/zenodo.8083285)
 
 Repository for developing server side of RFSoC fpga boards
 Qibosoq is a server for integrating [Qick](https://github.com/openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab) ecosystem
 for executing arbitrary pulses sequences on QPUs.
 
-The complete documentation can be found at [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
+The complete documentation for can be found at [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
 
 ## Installation
 The package can be installed by source:
 
 ```sh
 git clone https://github.com/qiboteam/qibosoq.git
 cd qibosoq
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
-# Qibosoq [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083286.svg)]
-(https://doi.org/10.5281/zenodo.8083286) Repository for developing server side
-of RFSoC fpga boards Qibosoq is a server for integrating [Qick](https://
-github.com/openquantumhardware/qick) in the [Qibolab](https://github.com/
-qiboteam/qibolab) ecosystem for executing arbitrary pulses sequences on QPUs.
-The complete documentation can be found at [qibo.science/qibosoq/stable](https:
-//qibo.science/qibosoq/stable/) ## Installation The package can be installed by
+# Qibosoq ![Tests](https://github.com/qiboteam/qibosoq/workflows/Tests/
+badge.svg) [![codecov](https://codecov.io/gh/qiboteam/qibosoq/branch/main/
+graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibosoq) [!
+[DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083285.svg)](https://
+doi.org/10.5281/zenodo.8083285) Repository for developing server side of RFSoC
+fpga boards Qibosoq is a server for integrating [Qick](https://github.com/
+openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab)
+ecosystem for executing arbitrary pulses sequences on QPUs. The complete
+documentation for can be found at [qibo.science/qibosoq/stable](https://
+qibo.science/qibosoq/stable/) ## Installation The package can be installed by
 source: ```sh git clone https://github.com/qiboteam/qibosoq.git cd qibosoq pip
 install . ``` ### Developer instructions For development make sure to install
 the package using [`poetry`](https://python-poetry.org/) and to install the
 pre-commit hooks: ```sh git clone https://github.com/qiboteam/qibosoq.git cd
 qibosoq poetry install pre-commit install ``` ## Configuration parameters In
 `configuration.py` some default qibosoq parameters are hardcoded. They can be
 changed using environment variables ([see documentation](https://qibo.science/
```

### Comparing `qibosoq-0.0.2/pyproject.toml` & `qibosoq-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qibosoq"
-version = "0.0.2"
+version = "0.0.3"
 description = "QIBO Server On Qick (qibosoq) is the server component of qibolab to be run on RFSoC boards"
 authors = [
   "Rodolfo Carobene <rodolfo.carobene@gmail.com>",
   "Javier Serrano <javier.serrano@tii.ae>",
 ]
 license = "Apache License 2.0"
 readme = "README.md"
@@ -25,29 +25,31 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
+ipython = "^8.12.0"
 sphinx = "^6.1.3"
 furo = "^2023.3.27"
 recommonmark = "^0.7.1"
 sphinxcontrib-bibtex = "^2.5.0"
 sphinx-markdown-tables = "^0.0.17"
 nbsphinx = "^0.9.1"
-ipython = "^8.12.0"
 sphinx-copybutton = "^0.5.1"
+sphinx-last-updated-by-git = "^0.3.5"
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
 pytest = ">=7.2.2"
 pytest-cov = "^4.0.0"
+pytest-mock = ">=3.10.0"
 
 [tool.poetry.group.analysis]
 optional = true
 
 [tool.poetry.group.analysis.dependencies]
 pylint = ">=2.16.0"
```

### Comparing `qibosoq-0.0.2/src/qibosoq/components/base.py` & `qibosoq-0.0.3/src/qibosoq/components/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 class Parameter(str, Enum):
     """Available parameters for sweepers."""
 
     FREQUENCY = "freq"
     AMPLITUDE = "gain"
     RELATIVE_PHASE = "phase"
-    START = "t"
+    DELAY = "t"
     BIAS = "bias"
     DURATION = "duration"
 
     @overload
     @classmethod
     def variants(cls, parameters: str) -> "Parameter":
         """Convert a string to a Parameter."""
```

### Comparing `qibosoq-0.0.2/src/qibosoq/configuration.py` & `qibosoq-0.0.3/src/qibosoq/configuration.py`

 * *Files identical despite different names*

### Comparing `qibosoq-0.0.2/src/qibosoq/log.py` & `qibosoq-0.0.3/src/qibosoq/log.py`

 * *Files identical despite different names*

### Comparing `qibosoq-0.0.2/src/qibosoq/programs/base.py` & `qibosoq-0.0.3/src/qibosoq/programs/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Base program used by qibosoq to execute sequences and sweeps."""
 
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import asdict
-from typing import List, Tuple
+from typing import Dict, List, Tuple
 
 import numpy as np
 import numpy.typing as npt
 from qick import QickProgram, QickSoc
+from qick.qick_asm import QickRegister
 
 import qibosoq.configuration as qibosoq_cfg
 from qibosoq.components.base import Config, Qubit
-from qibosoq.components.pulses import Drag, Gaussian, Pulse, Rectangular
+from qibosoq.components.pulses import Arbitrary, Drag, Gaussian, Pulse, Rectangular
 
 logger = logging.getLogger(qibosoq_cfg.MAIN_LOGGER_NAME)
 
 
 class BaseProgram(ABC, QickProgram):
     """Abstract class for QickPrograms."""
 
@@ -38,25 +39,28 @@
 
         # general settings
         self.adc_trig_offset = qpcfg.adc_trig_offset
         self.reps = qpcfg.reps
 
         # mux settings
         self.is_mux = qibosoq_cfg.IS_MULTIPLEXED
-        self.readouts_per_experiment = None
+        self.readouts_per_experiment = len([pulse for pulse in self.sequence if pulse.type == "readout"])
 
         self.relax_delay = self.us2cycles(qpcfg.repetition_duration)
         self.syncdelay = self.us2cycles(0)
         self.wait_initialize = self.us2cycles(2.0)
 
         self.pulses_registered = False
-        self.registered_waveform = []
+        self.registered_waveforms = {}
+        for pulse in sequence:
+            if pulse.dac not in self.registered_waveforms:
+                self.registered_waveforms[pulse.dac] = []
 
         if self.is_mux:
-            self.multi_ro_pulses = self.create_mux_ro_dict()
+            self.multi_ro_pulses = self.group_mux_ro()
             self.readouts_per_experiment = len(self.multi_ro_pulses)
 
         # pylint: disable-next=too-many-function-args
         super().__init__(soc, asdict(qpcfg))
 
     def declare_nqz_zones(self, sequence: List[Pulse]):
         """Declare nqz zone (1-2) for a given PulseSequence.
@@ -99,149 +103,148 @@
         gen_ch = pulse.dac
         max_gain = int(self.soccfg["gens"][gen_ch]["maxv"])
 
         # assign gain parameter
         gain = int(pulse.amplitude * max_gain)
         phase = self.deg2reg(pulse.relative_phase, gen_ch=gen_ch)
 
+        # pulse freq converted with frequency matching
+        freq = self.soc.freq2reg(pulse.frequency, gen_ch=gen_ch, ro_ch=pulse.adc)
+
         # pulse length converted with DAC CLK
         us_length = pulse.duration
         soc_length = self.soc.us2cycles(us_length, gen_ch=gen_ch)
 
-        is_drag = isinstance(pulse, Drag)
-        is_gaus = isinstance(pulse, Gaussian)
-        is_rect = isinstance(pulse, Rectangular)
-
-        # pulse freq converted with frequency matching
-        freq = self.soc.freq2reg(pulse.frequency, gen_ch=gen_ch, ro_ch=pulse.adc)
+        if isinstance(pulse, Rectangular):
+            self.set_pulse_registers(ch=gen_ch, style="const", freq=freq, phase=phase, gain=gain, length=soc_length)
+            return
 
-        # if pulse is drag or gauss first define the i-q shape and then set reg
-        if is_drag or is_gaus:
-            name = pulse.name
+        if isinstance(pulse, Gaussian):
             sigma = (soc_length / pulse.rel_sigma) * np.sqrt(2)
-
-            if is_gaus:
-                name = f"{gen_ch}_gaus_{round(sigma, 2)}_{round(soc_length, 2)}"
-                if name not in self.registered_waveform:
-                    self.add_gauss(ch=gen_ch, name=name, sigma=sigma, length=soc_length)
-                    self.registered_waveform.append(name)
-
-            elif is_drag:
-                # delta will be divided for the same quantity, we are setting it = 1
-                delta = -self.soccfg["gens"][gen_ch]["samps_per_clk"] * self.soccfg["gens"][gen_ch]["f_fabric"] / 2
-                name = (
-                    f"{gen_ch}_drag_{round(sigma, 2)}_{round(soc_length, 2)}_{round(pulse.beta, 2)}_{round(delta, 2)}"
+            name = f"{gen_ch}_gaus_{round(sigma, 2)}_{round(soc_length, 2)}"
+            if name not in self.registered_waveforms[gen_ch]:
+                self.add_gauss(ch=gen_ch, name=name, sigma=sigma, length=soc_length)
+                self.registered_waveforms[gen_ch].append(name)
+        elif isinstance(pulse, Drag):
+            delta = -self.soccfg["gens"][gen_ch]["samps_per_clk"] * self.soccfg["gens"][gen_ch]["f_fabric"] / 2
+            sigma = (soc_length / pulse.rel_sigma) * np.sqrt(2)
+            name = f"{gen_ch}_drag_{round(sigma, 2)}_{round(soc_length, 2)}_{round(pulse.beta, 2)}_{round(delta, 2)}"
+            if name not in self.registered_waveforms[gen_ch]:
+                self.add_DRAG(
+                    ch=gen_ch,
+                    name=name,
+                    sigma=sigma,
+                    delta=delta,
+                    alpha=pulse.beta,
+                    length=soc_length,
                 )
+                self.registered_waveforms[gen_ch].append(name)
+        elif isinstance(pulse, Arbitrary):
+            name = pulse.name
+            if name not in self.registered_waveforms[gen_ch]:
+                self.add_pulse(gen_ch, name, pulse.i_values, pulse.q_values)
+                self.registered_waveforms[gen_ch].append(name)
+
+        self.set_pulse_registers(
+            ch=gen_ch,
+            style="arb",
+            freq=freq,
+            phase=phase,
+            gain=gain,
+            waveform=name,
+        )
 
-                if name not in self.registered_waveform:
-                    self.add_DRAG(
-                        ch=gen_ch,
-                        name=name,
-                        sigma=sigma,
-                        delta=delta,
-                        alpha=pulse.beta,
-                        length=soc_length,
-                    )
-                    self.registered_waveform.append(name)
-
-            self.set_pulse_registers(
-                ch=gen_ch,
-                style="arb",
-                freq=freq,
-                phase=phase,
-                gain=gain,
-                waveform=name,
-            )
+    def execute_drive_pulse(self, pulse: Pulse, last_pulse_registered: Dict):
+        """Register a drive pulse if needed, then trigger the respective DAC.
 
-        # if pulse is rectangular set directly register
-        elif is_rect:
-            self.set_pulse_registers(ch=gen_ch, style="const", freq=freq, phase=phase, gain=gain, length=soc_length)
+        A pulse gets register if:
+        - it didn't happen in `initialize` (`self.pulses_registered` is False)
+        - it is not identical to the last pulse registered
 
+        """
+        if not self.pulses_registered and (
+            pulse.dac not in last_pulse_registered or pulse != last_pulse_registered[pulse.dac]
+        ):
+            self.add_pulse_to_register(pulse)
+            last_pulse_registered[pulse.dac] = pulse
+        self.pulse(ch=pulse.dac, t=0)
+
+    def execute_readout_pulse(
+        self, pulse: Pulse, muxed_pulses_executed: List[Pulse], muxed_ro_executed_indexes: List[int]
+    ):
+        """Register a readout pulse and perform a measurement."""
+        adcs = []
+        if self.is_mux:
+            if pulse in muxed_pulses_executed:
+                return
+            idx_mux = next(idx for idx, mux_time in enumerate(self.multi_ro_pulses) if pulse in mux_time)
+            self.add_muxed_readout_to_register(self.multi_ro_pulses[idx_mux])
+            muxed_ro_executed_indexes.append(idx_mux)
+            for ro_pulse in self.multi_ro_pulses[idx_mux]:
+                adcs.append(ro_pulse.adc)
+                muxed_pulses_executed.append(ro_pulse)
         else:
-            raise NotImplementedError(f"Shape {pulse} not supported!")
+            if not self.pulses_registered:
+                self.add_pulse_to_register(pulse)
+            adcs = [pulse.adc]
+
+        self.measure(
+            pulse_ch=pulse.dac,
+            adcs=adcs,
+            adc_trig_offset=self.adc_trig_offset,
+            wait=False,
+            syncdelay=self.syncdelay,
+        )
 
-    def body(self, wait: bool = True):
+    def body(self):
         """Execute sequence of pulses.
 
         For each pulses calls the add_pulse_to_register function (if not already registered)
         before firing it. If the pulse is a readout, it does a measurement and does
         not wait for the end of it. At the end of the sequence wait for meas and clock.
         """
-        muxed_ro_executed_time = []
-        muxed_pulses_executed = []
-
+        # in the form of {dac_number_0: last_pulse_of_dac_0, ...}
         last_pulse_registered = {}
-        for idx in self.gen_chs:
-            last_pulse_registered[idx] = None
+        muxed_pulses_executed = []
+        muxed_ro_executed_indexes = []
 
         for pulse in self.sequence:
-            # time follows tproc CLK
-            time = self.soc.us2cycles(pulse.start)
-
-            adc_ch = pulse.adc
-            gen_ch = pulse.dac
+            # wait the needed wait time so that the start is timed correctly
+            if isinstance(pulse.start_delay, QickRegister):
+                self.sync(pulse.start_delay.page, pulse.start_delay.addr)
+            else:  # assume is number
+                delay_start = self.soc.us2cycles(pulse.start_delay)
+                if delay_start != 0:
+                    self.synci(delay_start)
 
             if pulse.type == "drive":
-                if not self.pulses_registered:
-                    # TODO
-                    if not pulse == last_pulse_registered[gen_ch]:
-                        self.add_pulse_to_register(pulse)
-                        last_pulse_registered[gen_ch] = pulse
-                self.pulse(ch=gen_ch, t=time)
+                self.execute_drive_pulse(pulse, last_pulse_registered)
             elif pulse.type == "readout":
-                if self.is_mux:
-                    if pulse not in muxed_pulses_executed:
-                        start = list(self.multi_ro_pulses)[len(muxed_ro_executed_time)]
-                        time = self.soc.us2cycles(start)
-                        self.add_muxed_readout_to_register(self.multi_ro_pulses[start])
-                        muxed_ro_executed_time.append(start)
-                        adcs = []
-                        for ro_pulse in self.multi_ro_pulses[start]:
-                            adcs.append(ro_pulse.adc)
-                            muxed_pulses_executed.append(ro_pulse)
-                    else:
-                        continue
-                else:
-                    if not self.pulses_registered:
-                        self.add_pulse_to_register(pulse)
-                    adcs = [adc_ch]
-
-                self.measure(
-                    pulse_ch=gen_ch,
-                    adcs=adcs,
-                    adc_trig_offset=time + self.adc_trig_offset,
-                    t=time,
-                    wait=False,
-                    syncdelay=self.syncdelay,
-                )
+                self.execute_readout_pulse(pulse, muxed_pulses_executed, muxed_ro_executed_indexes)
+
         self.wait_all()
-        if wait:
-            self.sync_all(self.relax_delay)
 
     # pylint: disable=unexpected-keyword-arg, arguments-renamed
     def acquire(
         self,
         soc: QickSoc,
-        readouts_per_experiment: int = 1,
         load_pulses: bool = True,
         progress: bool = False,
         debug: bool = False,
         average: bool = False,
     ) -> Tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
         """Call the super() acquire function.
 
         Args:
-            readouts_per_experiment (int): relevant for internal acquisition
             load_pulse, progress, debug (bool): internal Qick parameters
             progress (bool): if true shows a progress bar, slows down things
             debug (bool): if true prints the program actually executed
             average (bool): if true return averaged res, otherwise single shots
         """
-        if self.readouts_per_experiment is not None:
-            readouts_per_experiment = self.readouts_per_experiment
+        readouts_per_experiment = self.readouts_per_experiment
         # if there are no readouts, temporaray set 1 so that qick can execute properly
         reads_per_rep = 1 if readouts_per_experiment == 0 else readouts_per_experiment
 
         res = super().acquire(
             soc,
             readouts_per_experiment=reads_per_rep,
             load_pulses=load_pulses,
@@ -289,14 +292,15 @@
     def declare_gen_mux_ro(self):
         """Declare nqz zone for multiplexed readout."""
         adc_ch_added = []
 
         mux_freqs = []
         mux_gains = []
 
+        ro_ch = None
         for pulse in (pulse for pulse in self.sequence if pulse.type == "readout"):
             adc_ch = pulse.adc
             ro_ch = pulse.dac
 
             if adc_ch not in adc_ch_added:
                 adc_ch_added.append(adc_ch)
                 freq = pulse.frequency
@@ -324,34 +328,30 @@
         length = self.soc.us2cycles(pulse.duration, gen_ch=gen_ch)
 
         if pulse.shape != "rectangular":
             raise TypeError("Only rectangular pulses can be multiplexed")
 
         self.set_pulse_registers(ch=gen_ch, style="const", length=length, mask=mask)
 
-    def create_mux_ro_dict(self) -> dict:
-        """Create a dictionary containing grouped readout pulses.
+    def group_mux_ro(self) -> list:
+        """Create a list containing readout pulses grouped by start time.
 
-        Example of dictionary:
-        { 'start_time_0': [pulse1, pulse2],
-        'start_time_1': [pulse3]}
+        Example of list:
+        [[pulse1, pulse2], [pulse3]]
         """
-        mux_dict = {}
+        mux_list = []
+        len_last_readout = 0
         for pulse in (pulse for pulse in self.sequence if pulse.type == "readout"):
-            if round(pulse.start, 5) not in mux_dict:
-                if len(mux_dict) > 0:
-                    if (pulse.start - list(mux_dict)[-1]) < 2:  # TODO not 2, but pulses len
-                        mux_dict[round(pulse.start, 5)] = mux_dict[list(mux_dict)[-1]]
-                        del mux_dict[list(mux_dict)[-2]]
-                    else:
-                        mux_dict[round(pulse.start, 5)] = []
-                else:
-                    mux_dict[round(pulse.start, 5)] = []
-            mux_dict[round(pulse.start, 5)].append(pulse)
+            if pulse.start_delay <= len_last_readout and len(mux_list) > 0:
+                # add the pulse to the last multiplexed readout
+                mux_list[-1].append(pulse)
+            else:
+                # add a new multiplexed readout
+                mux_list.append([pulse])
+            len_last_readout = pulse.duration
 
-        self.readouts_per_experiment = len(mux_dict)
-        return mux_dict
+        return mux_list
 
     @abstractmethod
     def initialize(self):
         """Abstract initialization."""
         raise NotImplementedError
```

### Comparing `qibosoq-0.0.2/src/qibosoq/programs/flux.py` & `qibosoq-0.0.3/src/qibosoq/programs/flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,12 +75,12 @@
             if qubit.dac is not None:
                 flux_ch = qubit.dac
                 self.declare_gen(flux_ch, nqz=1)
 
     def body(self):
         """Body program with flux biases set."""
         self.set_bias("sweetspot")
-        super().body(wait=False)
+        super().body()
         # the next two lines are redunant for security reasons
         self.set_bias("zero")
         self.soc.reset_gens()
         self.sync_all(self.relax_delay)
```

### Comparing `qibosoq-0.0.2/src/qibosoq/programs/pulse_sequence.py` & `qibosoq-0.0.3/src/qibosoq/programs/pulse_sequence.py`

 * *Files identical despite different names*

### Comparing `qibosoq-0.0.2/src/qibosoq/programs/sweepers.py` & `qibosoq-0.0.3/src/qibosoq/programs/sweepers.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,24 +36,14 @@
         qubits: List[Qubit],
         sweepers: Tuple[Sweeper, ...],
     ):
         """Init function, sets sweepers parameters before calling super.__init__."""
         self.sweepers = reversed_sweepers(sweepers)
         super().__init__(soc, qpcfg, sequence, qubits)
 
-    @staticmethod
-    def sweepers_to_reversed_list(sweepers) -> List[Sweeper]:
-        """Ensure that sweepers is a list and reverse it.
-
-        This is because sweepers are handled by Qick in the opposite order.
-        """
-        if isinstance(sweepers, Sweeper):
-            return [sweepers]
-        return list(reversed(sweepers))
-
     def add_sweep_info(self, sweeper: Sweeper):
         """Register RfsocSweep objects.
 
         Args:
             sweeper (RfsocSweep): single qibolab sweeper object to register
         """
         starts = sweeper.starts
@@ -91,17 +81,18 @@
                 sweep_type = sweeper.parameters[idx].value
                 register = self.get_gen_reg(gen_ch, sweep_type)
 
                 if sweeper.parameters[idx] is Parameter.AMPLITUDE:
                     max_gain = int(self.soccfg["gens"][gen_ch]["maxv"])
                     starts = (sweeper.starts * max_gain).astype(int)
                     stops = (sweeper.stops * max_gain).astype(int)
-                elif sweeper.parameters[idx] is Parameter.START:
-                    # TODO tell qick of the mismatch (t != time)
-                    register.reg_type = "time"
+                elif sweeper.parameters[idx] is Parameter.DELAY:
+                    # define a new register for the delay
+                    register = self.new_gen_reg(gen_ch, reg_type="time", tproc_reg=True)
+                    pulse.start_delay = register
 
                 new_sweep = QickSweep(
                     self,
                     register,  # sweeper_register
                     starts[idx],  # start
                     stops[idx],  # stop
                     sweeper.expts,  # number of points
```

### Comparing `qibosoq-0.0.2/src/qibosoq/rfsoc_server.py` & `qibosoq-0.0.3/src/qibosoq/rfsoc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
             debug=False,
         )
         toti = [[results[0][0].tolist()]]
         totq = [[results[0][1].tolist()]]
     else:
         toti, totq = program.acquire(
             qick_soc,
-            data["readouts_per_experiment"],
             load_pulses=True,
             progress=False,
             debug=False,
             average=data["average"],
         )
         toti = toti.tolist()
         totq = totq.tolist()
```

### Comparing `qibosoq-0.0.2/PKG-INFO` & `qibosoq-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibosoq
-Version: 0.0.2
+Version: 0.0.3
 Summary: QIBO Server On Qick (qibosoq) is the server component of qibolab to be run on RFSoC boards
 Home-page: https://github.com/qiboteam/qibosoq/
 License: Apache-2.0
 Author: Rodolfo Carobene
 Author-email: rodolfo.carobene@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,21 +16,23 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: qick (==0.2.135)
 Project-URL: Repository, https://github.com/qiboteam/qibosoq/
 Description-Content-Type: text/markdown
 
 # Qibosoq
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083286.svg)](https://doi.org/10.5281/zenodo.8083286)
+![Tests](https://github.com/qiboteam/qibosoq/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/qiboteam/qibosoq/branch/main/graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibosoq)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083285.svg)](https://doi.org/10.5281/zenodo.8083285)
 
 Repository for developing server side of RFSoC fpga boards
 Qibosoq is a server for integrating [Qick](https://github.com/openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab) ecosystem
 for executing arbitrary pulses sequences on QPUs.
 
-The complete documentation can be found at [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
+The complete documentation for can be found at [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
 
 ## Installation
 The package can be installed by source:
 
 ```sh
 git clone https://github.com/qiboteam/qibosoq.git
 cd qibosoq
```

#### html2text {}

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 2.1 Name: qibosoq Version: 0.0.2 Summary: QIBO Server On Qick
+Metadata-Version: 2.1 Name: qibosoq Version: 0.0.3 Summary: QIBO Server On Qick
 (qibosoq) is the server component of qibolab to be run on RFSoC boards Home-
 page: https://github.com/qiboteam/qibosoq/ License: Apache-2.0 Author: Rodolfo
 Carobene Author-email: rodolfo.carobene@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Physics Requires-
 Dist: qick (==0.2.135) Project-URL: Repository, https://github.com/qiboteam/
-qibosoq/ Description-Content-Type: text/markdown # Qibosoq [![DOI](https://
-zenodo.org/badge/DOI/10.5281/zenodo.8083286.svg)](https://doi.org/10.5281/
-zenodo.8083286) Repository for developing server side of RFSoC fpga boards
-Qibosoq is a server for integrating [Qick](https://github.com/
-openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab)
-ecosystem for executing arbitrary pulses sequences on QPUs. The complete
-documentation can be found at [qibo.science/qibosoq/stable](https://
-qibo.science/qibosoq/stable/) ## Installation The package can be installed by
-source: ```sh git clone https://github.com/qiboteam/qibosoq.git cd qibosoq pip
-install . ``` ### Developer instructions For development make sure to install
-the package using [`poetry`](https://python-poetry.org/) and to install the
-pre-commit hooks: ```sh git clone https://github.com/qiboteam/qibosoq.git cd
-qibosoq poetry install pre-commit install ``` ## Configuration parameters In
-`configuration.py` some default qibosoq parameters are hardcoded. They can be
-changed using environment variables ([see documentation](https://qibo.science/
-qibosoq/stable/getting-started/usage.html)). * IP of the server * Port of the
-server * Paths of log files * Name of python loggers * Path of bitstream * Type
-of readout (multiplexed or not, depending on the loaded bitstream) ## Run the
-server The simplest way of executing the server is: ``` sudo -E python -
-m qibosoq ``` and the server can be closed with `Ctrl-C`.\ Note that with this
-command the script will close as soon as the terminal where it's running it's
-closed. To run the server in detached mode you can use: ``` nohup sudo -
-E python -m qibosoq & ``` And the server can be closed with `sudo kill ` (PID
-will be saved in log). ### TII boards With TII boards the server can also be
-executed using the alias `server-run-bkg`. Also, two additional command are
-added in `.bashrc`: `serverinfo` and `serverclose`. `serverinfo` will print the
-PID if the server is running, otherwise will print "No running server".
-`serverclose` will close the server, if it is running. All these commands
-require sudo privileges. ## Contributing Contributions, issues and feature
-requests are welcome! Feel free to check [GitHub_issues]
+qibosoq/ Description-Content-Type: text/markdown # Qibosoq ![Tests](https://
+github.com/qiboteam/qibosoq/workflows/Tests/badge.svg) [![codecov](https://
+codecov.io/gh/qiboteam/qibosoq/branch/main/graph/badge.svg?token=1EKZKVEVX0)]
+(https://codecov.io/gh/qiboteam/qibosoq) [![DOI](https://zenodo.org/badge/DOI/
+10.5281/zenodo.8083285.svg)](https://doi.org/10.5281/zenodo.8083285) Repository
+for developing server side of RFSoC fpga boards Qibosoq is a server for
+integrating [Qick](https://github.com/openquantumhardware/qick) in the
+[Qibolab](https://github.com/qiboteam/qibolab) ecosystem for executing
+arbitrary pulses sequences on QPUs. The complete documentation for can be found
+at [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/) ##
+Installation The package can be installed by source: ```sh git clone https://
+github.com/qiboteam/qibosoq.git cd qibosoq pip install . ``` ### Developer
+instructions For development make sure to install the package using [`poetry`]
+(https://python-poetry.org/) and to install the pre-commit hooks: ```sh git
+clone https://github.com/qiboteam/qibosoq.git cd qibosoq poetry install pre-
+commit install ``` ## Configuration parameters In `configuration.py` some
+default qibosoq parameters are hardcoded. They can be changed using environment
+variables ([see documentation](https://qibo.science/qibosoq/stable/getting-
+started/usage.html)). * IP of the server * Port of the server * Paths of log
+files * Name of python loggers * Path of bitstream * Type of readout
+(multiplexed or not, depending on the loaded bitstream) ## Run the server The
+simplest way of executing the server is: ``` sudo -E python -m qibosoq ``` and
+the server can be closed with `Ctrl-C`.\ Note that with this command the script
+will close as soon as the terminal where it's running it's closed. To run the
+server in detached mode you can use: ``` nohup sudo -E python -m qibosoq & ```
+And the server can be closed with `sudo kill ` (PID will be saved in log). ###
+TII boards With TII boards the server can also be executed using the alias
+`server-run-bkg`. Also, two additional command are added in `.bashrc`:
+`serverinfo` and `serverclose`. `serverinfo` will print the PID if the server
+is running, otherwise will print "No running server". `serverclose` will close
+the server, if it is running. All these commands require sudo privileges. ##
+Contributing Contributions, issues and feature requests are welcome! Feel free
+to check [GitHub_issues]
```

