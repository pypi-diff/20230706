# Comparing `tmp/calsim-0.0.5.tar.gz` & `tmp/calsim-0.0.6.tar.gz`

## Comparing `calsim-0.0.5.tar` & `calsim-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/__init__.py
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/control.py
--rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/controller.py
--rwxr-xr-x   0        0        0    13617 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/dynamics.py
--rwxr-xr-x   0        0        0     6073 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/environment.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/exceptions.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/manipulator.py
--rwxr-xr-x   0        0        0      483 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/run_simulation.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/sim_utils.py
--rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/state_estimation.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/tests.py
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/transforms.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/twist.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 calsim-0.0.5/tests/test_simulation_simple.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.5/LICENSE
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 calsim-0.0.5/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 calsim-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/__init__.py
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/control.py
+-rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/controller.py
+-rwxr-xr-x   0        0        0    15278 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/dynamics.py
+-rwxr-xr-x   0        0        0     6163 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/environment.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/exceptions.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/manipulator.py
+-rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/run_simulation.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/sim_utils.py
+-rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/state_estimation.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/tests.py
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/transforms.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/core/twist.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 calsim-0.0.6/src/CalSim/tests/test_double_pend.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 calsim-0.0.6/tests/test_double_pend.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 calsim-0.0.6/tests/test_simulation_simple.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.6/LICENSE
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 calsim-0.0.6/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 calsim-0.0.6/PKG-INFO
```

### Comparing `calsim-0.0.5/src/CalSim/core/control.py` & `calsim-0.0.6/src/CalSim/core/control.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.5/src/CalSim/core/controller.py` & `calsim-0.0.6/src/CalSim/core/controller.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.5/src/CalSim/core/dynamics.py` & `calsim-0.0.6/src/CalSim/core/dynamics.py`

 * *Files 4% similar despite different names*

```diff
@@ -241,14 +241,66 @@
                 t (float): current time in simulation
             """
             return np.array([[x[1, 0]], [u[0, 0]/m -k/m * x[0, 0] - b/m * x[1, 0] - g*np.sin(theta)]])
         
         #call the init function on the MSD ramp system
         super().__init__(x0, 2, 1, msd_ramp, N = N)
 
+class DoublePendulum(Dynamics):
+    """
+    Double pendulum dynamics
+    """
+    def __init__(self, x0, m = 0.5, I = 0.5, L = 1, g = 9.81, N = 1):
+        """
+        Inputs:
+            x0: initial condition [q1, q2, q1Dot, q2Dot]
+            m: mass of joints
+            I: inertia of joints
+            L: length of joints
+            g: gravitational acceleration
+        """
+        #store the system parameters
+        self.m = m
+        self.I = I
+        self.L = L
+        self.g = g
+
+        def double_pend(x, u, t):
+            """
+            Double pendulum dynamics
+            Includes a torque input at each joint.
+            """
+            #extract the states
+            q1, q2, q1Dot, q2Dot = x[0, 0], x[1, 0], x[2, 0], x[3, 0]
+
+            #compute the inertia matrix
+            M = np.array([[2*I + 1.5*m*L**2 + m*L**2*np.cos(q2), I+0.25*m*L**2+0.5*m*L**2*np.cos(q2)],
+                          [I+0.25*m*L**2+0.5*m*L**2*np.cos(q2), I+0.25*m*L**2]])
+            #compute C
+            C = np.array([[0, -m*L**2*q1Dot*np.sin(q2)-0.5*m*L**2*q2Dot*np.sin(q2)], [0.5*m*L**2*q1Dot*np.sin(q2), 0]])
+
+            #compute N
+            N = np.array([[0.5*m*g*L*(np.sin(q1+q2)+3*np.sin(q1)), 0.5*m*g*L*np.sin(q1+q2)]]).T
+
+            #compute qDDot
+            qDot = np.array([[q1Dot, q2Dot]]).T
+            qDDot = np.linalg.inv(M)@(u - C@qDot - N)
+
+            #return [qDot, qDDot]
+            return np.vstack((qDot, qDDot))
+        
+        #call the init function on the double pendulum system
+        super().__init__(x0, 4, 2, double_pend, N = N)
+
+
+class FlywheelPendulum(Dynamics):
+    """
+    Pendulum driven by a flywheel
+    """
+
 
 class TurtlebotSysDyn(Dynamics):
     """
     System of N Turtlebots
     """
     def __init__(self, x0, N = 1, rTurtlebot = 0.15):
         """
```

### Comparing `calsim-0.0.5/src/CalSim/core/environment.py` & `calsim-0.0.6/src/CalSim/core/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,28 +122,30 @@
             boolean: whether or not the time has exceeded the total simulation time
         """
         #check current time with respect to simulation time
         if self.t >= self.TOTAL_SIM_TIME:
             return True
         return False
     
-    def run(self, N = 1, run_vis = True):
+    def run(self, N = 1, run_vis = True, verbose = False):
         """
         Function to run the simulation N times
         Inputs:
             N (int): number of simulation examples to run
             run_vis (bool): run the visualization of the results
         Returns:
             self.xHist, self.uHist, self.tHist
         """
         #loop over an overall simulation N times
         for i in range(N):
             self.reset()
+            print("Running Simulation.")
             while not self._is_done():
-                print("Simulation Time Remaining: ", self.TOTAL_SIM_TIME - self.t)
+                if verbose:
+                    print("Simulation Time Remaining: ", self.TOTAL_SIM_TIME - self.t)
                 self.step() #step the environment while not done
             if run_vis:
                 self.visualize() #render the result
         #return the history arrays
         return self.xHist, self.uHist, self.tHist
             
     def visualize(self):
```

### Comparing `calsim-0.0.5/src/CalSim/core/manipulator.py` & `calsim-0.0.6/src/CalSim/core/manipulator.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.5/src/CalSim/core/sim_utils.py` & `calsim-0.0.6/src/CalSim/core/sim_utils.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.5/src/CalSim/core/state_estimation.py` & `calsim-0.0.6/src/CalSim/core/state_estimation.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.5/src/CalSim/core/transforms.py` & `calsim-0.0.6/src/CalSim/core/transforms.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.5/src/CalSim/core/twist.py` & `calsim-0.0.6/src/CalSim/core/twist.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.5/LICENSE` & `calsim-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `calsim-0.0.5/pyproject.toml` & `calsim-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CalSim"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Massimiliano de Sa", email="mz.desa@berkeley.edu" },
 ]
 description = "Simulator package for Berkeley robotics course."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calsim-0.0.5/PKG-INFO` & `calsim-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSim
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simulator package for Berkeley robotics course.
 Project-URL: Homepage, https://github.com/mzdesa/CalSim
 Project-URL: Bug Tracker, https://github.com/mzdesa/CalSim
 Author-email: Massimiliano de Sa <mz.desa@berkeley.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

