# Comparing `tmp/calsim-0.0.6.tar.gz` & `tmp/calsim-0.0.7.tar.gz`

## Comparing `calsim-0.0.6.tar` & `calsim-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/__init__.py
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/control.py
--rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/controller.py
--rwxr-xr-x   0        0        0    15278 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/dynamics.py
--rwxr-xr-x   0        0        0     6163 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/environment.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/exceptions.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/manipulator.py
--rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/run_simulation.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/sim_utils.py
--rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/state_estimation.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/tests.py
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/transforms.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/twist.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/tests/test_double_pend.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 calsim-0.0.6/tests/test_double_pend.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 calsim-0.0.6/tests/test_simulation_simple.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.6/LICENSE
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 calsim-0.0.6/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 calsim-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/__init__.py
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/control.py
+-rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/controller.py
+-rwxr-xr-x   0        0        0    17318 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/dynamics.py
+-rwxr-xr-x   0        0        0     6118 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/environment.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/exceptions.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/manipulator.py
+-rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/run_simulation.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/sim_utils.py
+-rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/state_estimation.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/tests.py
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/transforms.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/twist.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/tests/test_double_pend.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 calsim-0.0.7/tests/test_double_pend.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 calsim-0.0.7/tests/test_simulation_simple.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.7/LICENSE
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 calsim-0.0.7/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 calsim-0.0.7/PKG-INFO
```

### Comparing `calsim-0.0.6/src/CalSim/core/control.py` & `calsim-0.0.7/src/CalSim/core/control.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.6/src/CalSim/core/controller.py` & `calsim-0.0.7/src/CalSim/core/controller.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.6/src/CalSim/core/dynamics.py` & `calsim-0.0.7/src/CalSim/core/dynamics.py`

 * *Files 13% similar despite different names*

```diff
@@ -293,14 +293,64 @@
 
 
 class FlywheelPendulum(Dynamics):
     """
     Pendulum driven by a flywheel
     """
 
+class MarsProbe(Dynamics):
+    """
+    Dynamics of a particle falling through the atmosphere of mars.
+    """
+    def __init__(self, x0, m = 572.743, Cd = 1.46, A = 5.5155, ftMax = 9806.65, N = 1):
+        """
+        Init function for mars probe.
+        
+        Mission Phases and Probe Parameters:
+        - https://ntrs.nasa.gov/api/citations/20080034645/downloads/20080034645.pdf
+        - Enter atmosphere at 5600 m/s
+        - Chute deployment occurs at Mach 1.65, 12.9 km above surface
+        - Touchdown occurs at 0.7 m/s
+        
+        Inputs:
+            x0 (2x1 NumPy Array): position vector of the system
+            m (float): mass of the probe
+            Cd (float): drag coefficient of probe 
+                NOTE: Cd for a parachute ~0.5 -> add this to Cd for just probe. Chute area ~200m^2.
+                      https://downloads.spj.sciencemag.org/space/2022/9805457.pdf
+            A (float): surface area for drag calculation
+            ftMax (float): maximum thrust force of probe
+            N (int): number of probes to simulate
+        """
+        #properties of probe
+        self.m = m
+        self.Cd = Cd
+        self.ftMax = ftMax
+
+        #properties of Mars
+        self.rho = 0.02 #density of atmosphere (kg/m^3)
+        self.M = 6.41693 * 10**23 #mass of Mars (kg)
+        self.R = 3390 * 10**3 #radius of Mars (m)
+        self.G = 6.6743 * 10**(-11) #universal gravitational constant
+
+        def probe_dyn(x, u, t):
+            """
+            Mars probe dynamics.
+            Inputs:
+                x (2x1 NumPy Array): [y, yDot] for y distance to the center of mars
+                u (1x1 NumPy Array): thrust force of the probe
+                t (float): time
+            """
+            y = x[0, 0]
+            yDot = x[1, 0]
+            yDDot = -self.G * self.M / (y**2) + 0.5*self.rho*self.Cd*yDot**2/self.m + u[0, 0]/m
+            return np.array([[yDot, yDDot]]).T
+        
+        #call the init function on the probe pendulum system
+        super().__init__(x0, 2, 1, probe_dyn, N = N)
 
 class TurtlebotSysDyn(Dynamics):
     """
     System of N Turtlebots
     """
     def __init__(self, x0, N = 1, rTurtlebot = 0.15):
         """
```

### Comparing `calsim-0.0.6/src/CalSim/core/environment.py` & `calsim-0.0.7/src/CalSim/core/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,19 +39,20 @@
         self.ptCloud = None #point cloud state as read by vision
         
         #Define simulation parameters
         self.SIM_FREQ = 1000 #integration frequency in Hz
         self.CONTROL_FREQ = 50 #control frequency in Hz
         self.SIMS_PER_STEP = self.SIM_FREQ//self.CONTROL_FREQ
         self.TOTAL_SIM_TIME = T #total simulation time in s
+        self.TOTAL_ITER = self.TOTAL_SIM_TIME*self.CONTROL_FREQ + 1 #total number of iterations
         
         #Define history arrays
-        self.xHist = np.zeros((self.dynamics.sysStateDimn, self.TOTAL_SIM_TIME*self.CONTROL_FREQ))
-        self.uHist = np.zeros((self.dynamics.sysInputDimn, self.TOTAL_SIM_TIME*self.CONTROL_FREQ))
-        self.tHist = np.zeros((1, self.TOTAL_SIM_TIME*self.CONTROL_FREQ))
+        self.xHist = np.zeros((self.dynamics.sysStateDimn, self.TOTAL_ITER))
+        self.uHist = np.zeros((self.dynamics.sysInputDimn, self.TOTAL_ITER))
+        self.tHist = np.zeros((1, self.TOTAL_ITER))
         
     def reset(self):
         """
         Reset the gym environment to its inital state.
         """
         #Reset gym environment parameters
         self.iter = 0 #number of iterations
@@ -59,35 +60,35 @@
         self.done = False
         
         #Reset system state
         self.x = self.x0 #retrieves initial condiiton
         self.xObsv = None #reset observer state
         
         #Define history arrays
-        self.xHist = np.zeros((self.dynamics.sysStateDimn, self.TOTAL_SIM_TIME*self.CONTROL_FREQ + 1))
-        self.uHist = np.zeros((self.dynamics.sysInputDimn, self.TOTAL_SIM_TIME*self.CONTROL_FREQ + 1))
-        self.tHist = np.zeros((1, self.TOTAL_SIM_TIME*self.CONTROL_FREQ + 1))
+        self.xHist = np.zeros((self.dynamics.sysStateDimn, self.TOTAL_ITER))
+        self.uHist = np.zeros((self.dynamics.sysInputDimn, self.TOTAL_ITER))
+        self.tHist = np.zeros((1, self.TOTAL_ITER))
 
     def step(self):
         """
         Step the sim environment by one integration
         """
         #retrieve current state information
         self._get_observation() #updates the observer
         
         #solve for the control input using the observed state
         self.controller.eval_input(self.t)
+
+        #update the deterministic system data, iterations, and history array
+        self._update_data()
         
-        #Zero order hold over the controller frequency
+        #Zero order hold over the controller frequency and step dynamics
         for i in range(self.SIMS_PER_STEP):
             self.dynamics.integrate(self.controller.get_input(), self.t, 1/self.SIM_FREQ) #integrate dynamics
             self.t += 1/self.SIM_FREQ #increment the time
-            
-        #update the deterministic system data, iterations, and history array
-        self._update_data()        
     
     def _update_data(self):
         """
         Update history arrays and deterministic state data
         """
         #append the input, time, and state to their history queues
         self.xHist[:, self.iter] = self.x.reshape((self.dynamics.sysStateDimn, ))
@@ -117,16 +118,16 @@
     
     def _is_done(self):
         """
         Check if the simulation is complete
         Returns:
             boolean: whether or not the time has exceeded the total simulation time
         """
-        #check current time with respect to simulation time
-        if self.t >= self.TOTAL_SIM_TIME:
+        #check if we have exceeded the total number of iterations
+        if self.iter >= self.TOTAL_ITER:
             return True
         return False
     
     def run(self, N = 1, run_vis = True, verbose = False):
         """
         Function to run the simulation N times
         Inputs:
```

### Comparing `calsim-0.0.6/src/CalSim/core/manipulator.py` & `calsim-0.0.7/src/CalSim/core/manipulator.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.6/src/CalSim/core/sim_utils.py` & `calsim-0.0.7/src/CalSim/core/sim_utils.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.6/src/CalSim/core/state_estimation.py` & `calsim-0.0.7/src/CalSim/core/state_estimation.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.6/src/CalSim/core/transforms.py` & `calsim-0.0.7/src/CalSim/core/transforms.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.6/src/CalSim/core/twist.py` & `calsim-0.0.7/src/CalSim/core/twist.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.6/src/CalSim/tests/test_double_pend.py` & `calsim-0.0.7/src/CalSim/tests/test_double_pend.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,8 @@
 q1DotHist = xHist[2, :].tolist()
 q2DotHist = xHist[3, :].tolist()
 tHist = tHist[0, :].tolist()
 
 #plot q1 against q2
 plt.plot(q1Hist, q2Hist)
 plt.plot(q1DotHist, q2DotHist)
-
-plt.show()
+plt.show()
```

### Comparing `calsim-0.0.6/LICENSE` & `calsim-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `calsim-0.0.6/pyproject.toml` & `calsim-0.0.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CalSim"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Massimiliano de Sa", email="mz.desa@berkeley.edu" },
 ]
 description = "Simulator package for Berkeley robotics course."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calsim-0.0.6/PKG-INFO` & `calsim-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSim
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simulator package for Berkeley robotics course.
 Project-URL: Homepage, https://github.com/mzdesa/CalSim
 Project-URL: Bug Tracker, https://github.com/mzdesa/CalSim
 Author-email: Massimiliano de Sa <mz.desa@berkeley.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

