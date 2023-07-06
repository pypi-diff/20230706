# Comparing `tmp/stdatm-0.3.0.tar.gz` & `tmp/stdatm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdatm-0.3.0.tar", max compression
+gzip compressed data, was "stdatm-0.3.1.tar", max compression
```

## Comparing `stdatm-0.3.0.tar` & `stdatm-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-06 08:21:38.389067 stdatm-0.3.0/LICENSE
--rw-r--r--   0        0        0       50 2023-07-06 08:21:38.389067 stdatm-0.3.0/README.md
--rw-r--r--   0        0        0     2567 2023-07-06 08:21:57.981546 stdatm-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1183 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/__init__.py
--rw-r--r--   0        0        0    14500 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/atmosphere.py
--rw-r--r--   0        0        0     7111 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/atmosphere_partials.py
--rw-r--r--   0        0        0     6822 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/partials_state_parameters.py
--rw-r--r--   0        0        0     8954 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/speed_parameters.py
--rw-r--r--   0        0        0     4447 2023-07-06 08:21:38.389067 stdatm-0.3.0/src/stdatm/state_parameters.py
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 stdatm-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-06 09:57:56.922461 stdatm-0.3.1/LICENSE
+-rw-r--r--   0        0        0       50 2023-07-06 09:57:56.922461 stdatm-0.3.1/README.md
+-rw-r--r--   0        0        0     2567 2023-07-06 09:58:12.339043 stdatm-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1183 2023-07-06 09:57:56.922461 stdatm-0.3.1/src/stdatm/__init__.py
+-rw-r--r--   0        0        0    14556 2023-07-06 09:57:56.922461 stdatm-0.3.1/src/stdatm/atmosphere.py
+-rw-r--r--   0        0        0     7111 2023-07-06 09:57:56.922461 stdatm-0.3.1/src/stdatm/atmosphere_partials.py
+-rw-r--r--   0        0        0     6822 2023-07-06 09:57:56.922461 stdatm-0.3.1/src/stdatm/partials_state_parameters.py
+-rw-r--r--   0        0        0     8954 2023-07-06 09:57:56.922461 stdatm-0.3.1/src/stdatm/speed_parameters.py
+-rw-r--r--   0        0        0     4447 2023-07-06 09:57:56.922461 stdatm-0.3.1/src/stdatm/state_parameters.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 stdatm-0.3.1/PKG-INFO
```

### Comparing `stdatm-0.3.0/LICENSE` & `stdatm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stdatm-0.3.0/pyproject.toml` & `stdatm-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stdatm"
-version = "0.3.0"
+version = "0.3.1"
 description = "Numpy-oriented Standard Atmosphere model"
 readme = "README.md"
 authors = [
     "Christophe DAVID <christophe.david@onera.fr>",
 ]
 license = "GPL-3.0-only"
 classifiers = [
```

### Comparing `stdatm-0.3.0/src/stdatm/__init__.py` & `stdatm-0.3.1/src/stdatm/__init__.py`

 * *Files identical despite different names*

### Comparing `stdatm-0.3.0/src/stdatm/atmosphere.py` & `stdatm-0.3.1/src/stdatm/atmosphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from copy import deepcopy
-from numbers import Number
+from numbers import Real
 from typing import Sequence, Union
 
 import numpy as np
 from scipy.constants import foot
 from scipy.optimize import root
 
 from stdatm.speed_parameters import (
@@ -112,15 +112,15 @@
                                  it should be provided in meters.
         """
 
         self.delta_t = delta_t
 
         # For convenience, let's have altitude as numpy arrays and in meters in all cases
         unit_coeff = foot if altitude_in_feet else 1.0
-        if not isinstance(altitude, Number):
+        if not isinstance(altitude, Real):
             altitude = np.asarray(altitude)
         self._altitude = altitude * unit_coeff
 
         # Outputs
         self._temperature = None
         self._pressure = None
         self._density = None
@@ -149,15 +149,15 @@
     def delta_t(self) -> float:
         """Temperature increment applied to whole temperature profile."""
         return self._delta_t
 
     @delta_t.setter
     def delta_t(self, value: float):
         # Let's ensure it is not a one-element array that would crash lru_cache
-        if isinstance(value, Number):
+        if isinstance(value, Real):
             self._delta_t = value
         else:
             self._delta_t = np.asarray(value).item()
 
     @property
     def temperature(self) -> Union[float, np.ndarray]:
         """Temperature in K."""
@@ -312,14 +312,17 @@
         self._calibrated_airspeed = self._process_speed_value(value)
 
     def _process_speed_value(self, value):
         self._reset_speeds()
         return self._adapt_shape(value)
 
     def _adapt_shape(self, value):
+        if isinstance(value, Real):
+            return value
+
         if value is not None:
             value = np.asarray(value)
             if np.size(value) > 1:
                 try:
                     expected_shape = np.shape(value + self.get_altitude())
                 except ValueError as exc:
                     raise RuntimeError(
```

### Comparing `stdatm-0.3.0/src/stdatm/atmosphere_partials.py` & `stdatm-0.3.1/src/stdatm/atmosphere_partials.py`

 * *Files identical despite different names*

### Comparing `stdatm-0.3.0/src/stdatm/partials_state_parameters.py` & `stdatm-0.3.1/src/stdatm/partials_state_parameters.py`

 * *Files identical despite different names*

### Comparing `stdatm-0.3.0/src/stdatm/speed_parameters.py` & `stdatm-0.3.1/src/stdatm/speed_parameters.py`

 * *Files identical despite different names*

### Comparing `stdatm-0.3.0/src/stdatm/state_parameters.py` & `stdatm-0.3.1/src/stdatm/state_parameters.py`

 * *Files identical despite different names*

### Comparing `stdatm-0.3.0/PKG-INFO` & `stdatm-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdatm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Numpy-oriented Standard Atmosphere model
 License: GPL-3.0-only
 Author: Christophe DAVID
 Author-email: christophe.david@onera.fr
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

