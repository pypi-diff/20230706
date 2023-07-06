# Comparing `tmp/multiSyncPy-0.1.0.tar.gz` & `tmp/multiSyncPy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiSyncPy-0.1.0.tar", last modified: Wed Aug  3 15:43:28 2022, max compression
+gzip compressed data, was "multiSyncPy-0.1.1.tar", last modified: Thu Jul  6 08:55:24 2023, max compression
```

## Comparing `multiSyncPy-0.1.0.tar` & `multiSyncPy-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-08-03 15:43:28.374742 multiSyncPy-0.1.0/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     7652 2022-08-03 13:08:23.000000 multiSyncPy-0.1.0/LICENSE.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     2338 2022-08-03 15:43:28.374742 multiSyncPy-0.1.0/PKG-INFO
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     1830 2022-08-03 15:31:22.000000 multiSyncPy-0.1.0/README.md
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-08-03 15:43:28.370742 multiSyncPy-0.1.0/multiSyncPy/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      709 2022-08-03 15:35:13.000000 multiSyncPy-0.1.0/multiSyncPy/__init__.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     3198 2022-01-07 11:17:02.000000 multiSyncPy-0.1.0/multiSyncPy/data_generation.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)    23855 2022-08-03 15:40:34.000000 multiSyncPy-0.1.0/multiSyncPy/synchrony_metrics.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)    22175 2022-08-03 14:23:47.000000 multiSyncPy-0.1.0/multiSyncPy/visualisations.py
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-08-03 15:43:28.374742 multiSyncPy-0.1.0/multiSyncPy.egg-info/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     2338 2022-08-03 15:43:28.000000 multiSyncPy-0.1.0/multiSyncPy.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      322 2022-08-03 15:43:28.000000 multiSyncPy-0.1.0/multiSyncPy.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)        1 2022-08-03 15:43:28.000000 multiSyncPy-0.1.0/multiSyncPy.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)       39 2022-08-03 15:43:28.000000 multiSyncPy-0.1.0/multiSyncPy.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)       12 2022-08-03 15:43:28.000000 multiSyncPy-0.1.0/multiSyncPy.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)       38 2022-08-03 15:43:28.374742 multiSyncPy-0.1.0/setup.cfg
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      943 2022-08-03 14:27:35.000000 multiSyncPy-0.1.0/setup.py
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2023-07-06 08:55:24.082361 multiSyncPy-0.1.1/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     7652 2023-07-06 08:48:02.000000 multiSyncPy-0.1.1/LICENSE.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     2466 2023-07-06 08:55:24.082361 multiSyncPy-0.1.1/PKG-INFO
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     1958 2023-07-06 08:51:42.000000 multiSyncPy-0.1.1/README.md
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2023-07-06 08:55:24.082361 multiSyncPy-0.1.1/multiSyncPy/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      709 2023-07-06 08:48:02.000000 multiSyncPy-0.1.1/multiSyncPy/__init__.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     3196 2023-07-06 08:48:02.000000 multiSyncPy-0.1.1/multiSyncPy/data_generation.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)    23451 2023-07-06 08:48:02.000000 multiSyncPy-0.1.1/multiSyncPy/synchrony_metrics.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)    23361 2023-07-06 08:48:02.000000 multiSyncPy-0.1.1/multiSyncPy/visualisations.py
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2023-07-06 08:55:24.082361 multiSyncPy-0.1.1/multiSyncPy.egg-info/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     2466 2023-07-06 08:55:23.000000 multiSyncPy-0.1.1/multiSyncPy.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      322 2023-07-06 08:55:23.000000 multiSyncPy-0.1.1/multiSyncPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)        1 2023-07-06 08:55:23.000000 multiSyncPy-0.1.1/multiSyncPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)       44 2023-07-06 08:55:23.000000 multiSyncPy-0.1.1/multiSyncPy.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)       12 2023-07-06 08:55:23.000000 multiSyncPy-0.1.1/multiSyncPy.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)       38 2023-07-06 08:55:24.082361 multiSyncPy-0.1.1/setup.cfg
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      949 2023-07-06 08:54:34.000000 multiSyncPy-0.1.1/setup.py
```

### Comparing `multiSyncPy-0.1.0/LICENSE.txt` & `multiSyncPy-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multiSyncPy-0.1.0/PKG-INFO` & `multiSyncPy-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: multiSyncPy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functions to quantify multivariate synchrony
 Home-page: https://github.com/cslab-hub/multiSyncPy
 Author: Dan Hudson
 Author-email: daniel.dominic.hudson@uni-osnabrueck.de
 License: GNU LGPL
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-**Important announcement** - *There is an issue with the calculation of determinism in version 0.0.3 and below; update to version 0.0.4 or above to receive the fix (pip install --upgrade multiSyncPy). Thanks to @mrrezaie for spotting the issue. Please inform anyone you know who might be using multiSyncPy.*
+**Important announcement** - *There is a new version of multiSyncPy (0.1.0) that includes a new multivariate synchronization measures as well as some visualiation functions.*
 
 # multiSyncPy
 
-multiSyncPy is a Python package for quantifying multivariate synchrony. Our package supports the burgeoning field of research into synchrony, making accessible a set of methods for studying group-level rather than dyadic constructs of synchrony and/or coordination. We offer a range of metrics for estimating mulivariate synchrony based on a collection of those used in recent literature.
+multiSyncPy is a Python package for quantifying multivariate synchrony. Our package supports the burgeoning field of research into synchrony, making accessible a set of methods for studying group-level rather than dyadic constructs of synchrony and/or coordination. We offer a range of metrics for estimating multivariate synchrony based on a collection of those used in recent literature.
 
 The main methods of this package are functions to calculate:
 
  * symbolic entropy, 
  * multidimensional recurrence quantification, 
  * coherence (and a related 'sum-normalized CSD' metric),
  * the cluster-phase 'Rho' metric
- * the synchronization coefficient metric, and 
- * a statistical test based on the Kuramoto order parameter
+ * the synchronization coefficient metric,
+ * a statistical test based on the Kuramoto order parameter, and
+ * driver-empath model with synchrony index
 
 We also include functions for two surrogation techniques to compare the observed coordination dynamics with chance levels.
 
+Additionally, we include a set of functions to visualize the time-varying coordination metrics as well as the individual or pair-wise contributions to the multivariate measure (depending on the particular method).
+
 multiSyncPy is freely available under the LGPL license. The source code is maintained at <https://github.com/cslab-hub/multiSyncPy>, which also includes examples of usage of the package. Documentation can be accessed through `help()` or accessed at <https://cslab-hub.github.io/multiSyncPy/>. 
 
-Further details of the package and case studies of its use on real-world data are described in our paper 
+Further details of the package and case studies of its use on real-world data are described in our paper. 
 
 Hudson, D., Wiltshire, T.J. & Atzmueller, M. multiSyncPy: A Python package for assessing multivariate coordination dynamics. *Behav Res* (2022). <https://doi.org/10.3758/s13428-022-01855-y>. 
 
 Please cite this paper if you use multiSyncPy in your research.
```

### Comparing `multiSyncPy-0.1.0/README.md` & `multiSyncPy-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-**Important announcement** - *There is an issue with the calculation of determinism in version 0.0.3 and below; update to version 0.0.4 or above to receive the fix (pip install --upgrade multiSyncPy). Thanks to @mrrezaie for spotting the issue. Please inform anyone you know who might be using multiSyncPy.*
+**Important announcement** - *There is a new version of multiSyncPy (0.1.0) that includes a new multivariate synchronization measures as well as some visualiation functions.*
 
 # multiSyncPy
 
-multiSyncPy is a Python package for quantifying multivariate synchrony. Our package supports the burgeoning field of research into synchrony, making accessible a set of methods for studying group-level rather than dyadic constructs of synchrony and/or coordination. We offer a range of metrics for estimating mulivariate synchrony based on a collection of those used in recent literature.
+multiSyncPy is a Python package for quantifying multivariate synchrony. Our package supports the burgeoning field of research into synchrony, making accessible a set of methods for studying group-level rather than dyadic constructs of synchrony and/or coordination. We offer a range of metrics for estimating multivariate synchrony based on a collection of those used in recent literature.
 
 The main methods of this package are functions to calculate:
 
  * symbolic entropy, 
  * multidimensional recurrence quantification, 
  * coherence (and a related 'sum-normalized CSD' metric),
  * the cluster-phase 'Rho' metric
- * the synchronization coefficient metric, and 
- * a statistical test based on the Kuramoto order parameter
+ * the synchronization coefficient metric,
+ * a statistical test based on the Kuramoto order parameter, and
+ * driver-empath model with synchrony index
 
 We also include functions for two surrogation techniques to compare the observed coordination dynamics with chance levels.
 
+Additionally, we include a set of functions to visualize the time-varying coordination metrics as well as the individual or pair-wise contributions to the multivariate measure (depending on the particular method).
+
 multiSyncPy is freely available under the LGPL license. The source code is maintained at <https://github.com/cslab-hub/multiSyncPy>, which also includes examples of usage of the package. Documentation can be accessed through `help()` or accessed at <https://cslab-hub.github.io/multiSyncPy/>. 
 
-Further details of the package and case studies of its use on real-world data are described in our paper 
+Further details of the package and case studies of its use on real-world data are described in our paper. 
 
 Hudson, D., Wiltshire, T.J. & Atzmueller, M. multiSyncPy: A Python package for assessing multivariate coordination dynamics. *Behav Res* (2022). <https://doi.org/10.3758/s13428-022-01855-y>. 
 
 Please cite this paper if you use multiSyncPy in your research.
```

### Comparing `multiSyncPy-0.1.0/multiSyncPy/__init__.py` & `multiSyncPy-0.1.1/multiSyncPy/__init__.py`

 * *Files identical despite different names*

### Comparing `multiSyncPy-0.1.0/multiSyncPy/data_generation.py` & `multiSyncPy-0.1.1/multiSyncPy/data_generation.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,93 +4,100 @@
 
  * autoregressive_data - Produces a time series using a stochastic autoregressive function of order two.
  * kuramoto_data - Produces a time series using a Kuramoto model. 
 """
 
 import numpy as np
 
+
 def autoregressive_data(length, phi_1, phi_2, epsilon, c=0):
     """Generates synthetic data using an autoregressive function where each time point depends on the previous two.
-    
+
     Parameters
     ----------
     length: int
         The number of time steps to generate.
     phi_1: float
         The weighting of the value two time steps ago.
     phi_2: float
         The weighting of the value one time steps ago.
     epsilon: float
         The standard deviation of Gaussian noise added at each time step.
     c: float
         An optional bias term.
-    
+
     Returns
     -------
     autoregressive_data: array
         An array containing autoregressive synthetic data.
     """
-    
+
     x_1 = c + np.random.normal(0) * phi_1 * phi_2
     x_2 = c + np.random.normal(0) * phi_1 * phi_2
-    
+
     outputs = []
-    
-    for i in range(length + 100): ## 100 extra points just to make sure that the autoregressive process has settled down
-        
+
+    for i in range(
+        length + 100
+    ):  ## 100 extra points just to make sure that the autoregressive process has settled down
         x_new = c + (phi_1 * x_1) + (phi_2 * x_2) + np.random.normal(0, epsilon)
-        
+
         outputs.append(x_new)
-        
+
         x_1 = x_2
         x_2 = x_new
-        
+
     return np.array(outputs[-length:])
 
 
 def kuramoto_data(phases, omegas, K, alpha, d_t, length):
     """Generates synthetic data from a Kuramoto model of coupled oscillators.
-    
+
     Parameters
     ----------
     phases: array
-        An array of initial phases in radians for each oscillator. 
+        An array of initial phases in radians for each oscillator.
     omegas: array
-        The natural frequencies of each oscillator. Must be the same length as phases. 
+        The natural frequencies of each oscillator. Must be the same length as phases.
     K: float
-        The coupling strength between oscillators in the model. 
+        The coupling strength between oscillators in the model.
     alpha: float
-        A parameter to control the amount of Gaussian noise added at each time step. 
+        A parameter to control the amount of Gaussian noise added at each time step.
     d_t: float
         The change in time that each time step represents.
     length: int
         The number of time points desired in the synthetic data.
-    
+
     Returns
     -------
     kuramoto_data: array
-        An array containing synthetic data generated from the Kuramoto model. 
+        An array containing synthetic data generated from the Kuramoto model.
     """
-    
-    def update_phases(phases, omegas, K, alpha, d_t):
 
+    def update_phases(phases, omegas, K, alpha, d_t):
         psi = np.mean(phases)
 
         r = np.linalg.norm([np.cos(phases), np.sin(phases)])
 
-        return phases + d_t * (omegas + K * r * np.sin(psi - phases)) + alpha * np.random.normal(0, np.sqrt(d_t), phases.shape)
-    
+        return (
+            phases
+            + d_t * (omegas + K * r * np.sin(psi - phases))
+            + alpha * np.random.normal(0, np.sqrt(d_t), phases.shape)
+        )
+
     phases_sequence = []
 
     for i in range(length):
-
         phases_sequence.append(phases)
         phases = update_phases(phases, omegas, K, alpha, d_t)
-        
+
     return np.sin(np.array(phases_sequence)).T
 
 
-def linear_nonstationary_transition(begin_frequency, end_frequency, sampling_rate, duration):
-    
-    transition_frequencies = np.linspace(begin_frequency, end_frequency, duration * sampling_rate)
+def linear_nonstationary_transition(
+    begin_frequency, end_frequency, sampling_rate, duration
+):
+    transition_frequencies = np.linspace(
+        begin_frequency, end_frequency, duration * sampling_rate
+    )
 
-    return np.exp(np.cumsum(transition_frequencies)/sampling_rate * np.pi * 2j).real
+    return np.exp(np.cumsum(transition_frequencies) / sampling_rate * np.pi * 2j).real
```

### Comparing `multiSyncPy-0.1.0/multiSyncPy/synchrony_metrics.py` & `multiSyncPy-0.1.1/multiSyncPy/synchrony_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,164 +24,166 @@
 import scipy.spatial
 import scipy.signal
 import scipy.stats
 import copy
 from sklearn.linear_model import LinearRegression
 
 
-def recurrence_matrix(data, radius, normalise=True, embedding_dimension=None, embedding_delay=None):
-    """Creates a recurrence matrix from a multivariate time series. The Euclidean distance, combined with the radius parameter, is used to determine which points are close enough to count as 'recurrent'. 
-    
+def recurrence_matrix(
+    data, radius, normalise=True, embedding_dimension=None, embedding_delay=None
+):
+    """Creates a recurrence matrix from a multivariate time series. The Euclidean distance, combined with the radius parameter, is used to determine which points are close enough to count as 'recurrent'.
+
     Parameters
     ----------
     data: ndarray
         An array containing the multivariate time series with shape (number_signals, duration).
     radius: float
         The Euclidean distance below which two points will count as recurrent.
     normalise: bool
         Whether to apply normalisation. Normalisation is applied on each variable separately, transforming the data to have mean 0 and variance 1, which is intended to help balance the relative importance of each variable when calculating Euclidean distances.
     embedding_dimension: int
-        The number of copies of the multivariate time series to use. If provided, embedding_delay must also be used. 
+        The number of copies of the multivariate time series to use. If provided, embedding_delay must also be used.
     embedding_delay: int
-        If using embedding_dimension, this is the delay in number of time steps that is applied to each new copy of the multivariate time series. 
-    
+        If using embedding_dimension, this is the delay in number of time steps that is applied to each new copy of the multivariate time series.
+
     Returns
     -------
     recurrence_matrix: ndarray
-        A square matrix with shape (duration, duration). Cells have value True when two time points are recurrent, and False otherwise. 
+        A square matrix with shape (duration, duration). Cells have value True when two time points are recurrent, and False otherwise.
     """
-    
+
     if normalise:
-        
-        data = (data - data.mean(axis=1).reshape(-1,1)) / data.std(axis=1).reshape(-1,1)
-    
+        data = (data - data.mean(axis=1).reshape(-1, 1)) / data.std(axis=1).reshape(
+            -1, 1
+        )
+
     if embedding_dimension and embedding_delay:
-        
         copies = []
-        
-        copy_length = data.shape[1] - (embedding_delay * (embedding_dimension-1))
-        
+
+        copy_length = data.shape[1] - (embedding_delay * (embedding_dimension - 1))
+
         for i in range(embedding_dimension):
-            
-            copies.append(data[:, i*embedding_delay:copy_length+i*embedding_delay])
-    
+            copies.append(
+                data[:, i * embedding_delay : copy_length + i * embedding_delay]
+            )
+
         data = np.concatenate(copies)
-    
+
     distance_matrix = scipy.spatial.distance_matrix(data.T, data.T)
-    
+
     return distance_matrix < radius
 
 
 def get_diagonal_lengths(recurrence_matrix):
-    """Returns the lengths of sequences where the successive cells have a value of 1, and how many times sequences of each length were observed, looking along the diagonals of a recurrence matrix. Considers only the upper triangle of the recurrence matrix, not including the line of identity. 
-    
+    """Returns the lengths of sequences where the successive cells have a value of 1, and how many times sequences of each length were observed, looking along the diagonals of a recurrence matrix. Considers only the upper triangle of the recurrence matrix, not including the line of identity.
+
     Parameters
     ----------
     recurrence_matrix: ndarray
         Matrix indicating which time points are recurrent with other time points. Truthy values are used to indicate a recurrence.
-    
+
     Returns
     -------
     full_diagonal_length_counts: dict
-        A dict where the keys are the length of a sequence and the values are the number of times a sequence of that length was observed. 
+        A dict where the keys are the length of a sequence and the values are the number of times a sequence of that length was observed.
     """
-    
+
     full_diagonal_length_counts = {}
-    
+
     def get_lengths(x):
-        
         diagonal_length_counts = {}
         current_length = 0
-        
+
         for cell in x:
-            
             if cell:
-                
-                current_length += 1 
-                
+                current_length += 1
+
             else:
-                
                 if current_length > 0:
-                    
-                    diagonal_length_counts[current_length] = diagonal_length_counts.get(current_length, 0) + 1
-                
+                    diagonal_length_counts[current_length] = (
+                        diagonal_length_counts.get(current_length, 0) + 1
+                    )
+
                 current_length = 0
-                
+
         if current_length > 0:
-                    
-            diagonal_length_counts[current_length] = diagonal_length_counts.get(current_length, 0) + 1
-                
+            diagonal_length_counts[current_length] = (
+                diagonal_length_counts.get(current_length, 0) + 1
+            )
+
         return diagonal_length_counts
-    
-    for diagonal in range(1,recurrence_matrix.shape[0]):
-        
+
+    for diagonal in range(1, recurrence_matrix.shape[0]):
         temp_length_counts = get_lengths(np.diag(recurrence_matrix, diagonal))
-        
+
         for length, count in temp_length_counts.items():
-            
-            full_diagonal_length_counts[length] = full_diagonal_length_counts.get(length,0) + count
-            
+            full_diagonal_length_counts[length] = (
+                full_diagonal_length_counts.get(length, 0) + count
+            )
+
     return full_diagonal_length_counts
 
 
 def rqa_metrics(recurrence_matrix, min_length=2):
-    """Returns the proportion of recurrence, proportion of determinism, mean diagonal length, and max diagonal length, for the input recurrence matrix. 
-    
+    """Returns the proportion of recurrence, proportion of determinism, mean diagonal length, and max diagonal length, for the input recurrence matrix.
+
     Parameters
     ----------
     recurrence_matrix: ndarray
         Matrix indicating which time points are recurrent with other time points. Truthy values are used to indicate a recurrence.
-    
+
     Returns
     -------
     rec: float
-        A value between 0 and 1 representing the proportion of recurrence observed in the recurrence matrix. Multiply by 100 to get the %REC. 
+        A value between 0 and 1 representing the proportion of recurrence observed in the recurrence matrix. Multiply by 100 to get the %REC.
     det: float
-        A value between 0 and 1 representing the proportion of determinism observed in the recurrence matrix. Multiply by 100 to get the %det. 
+        A value between 0 and 1 representing the proportion of determinism observed in the recurrence matrix. Multiply by 100 to get the %det.
     mean_length: float
-        The mean length of diagonal sequences in the recurrence matrix. 
+        The mean length of diagonal sequences in the recurrence matrix.
     max_length: int
-        The maximum length of diagonal sequences in the recurrence matrix. 
+        The maximum length of diagonal sequences in the recurrence matrix.
     """
-    
+
     diagonal_length_counts = get_diagonal_lengths(recurrence_matrix)
-    
+
     rec = 0
     det = 0
     mean_length = 0
     max_length = 0
-    
+
     if diagonal_length_counts.keys():
-    
         for length, count in diagonal_length_counts.items():
-
             rec += length * count
 
             if length >= min_length:
-
                 det += length * count
 
             mean_length = rec
-            
-        det = det / rec ##Divide by the number of recurrent points (before rec becomes a fraction)
-        rec = rec / (recurrence_matrix.shape[0]*(recurrence_matrix.shape[1]-1)/2) ##The number of off-diagonal cells in the upper triangle 
+
+        det = (
+            det / rec
+        )  ##Divide by the number of recurrent points (before rec becomes a fraction)
+        rec = rec / (
+            recurrence_matrix.shape[0] * (recurrence_matrix.shape[1] - 1) / 2
+        )  ##The number of off-diagonal cells in the upper triangle
         mean_length = mean_length / sum(diagonal_length_counts.values())
         max_length = max(diagonal_length_counts.keys())
-    
+
     return rec, det, mean_length, max_length
 
 
 def rho(phases):
-    """Returns the quantity defined by Richardson et al. as 'rho' in "Measuring group synchrony: a cluster-phase method foranalyzing multivariate movement time-series:, doi: 10.3389/fphys.2012.00405. 
-    
+    """Returns the quantity defined by Richardson et al. as 'rho' in "Measuring group synchrony: a cluster-phase method foranalyzing multivariate movement time-series:, doi: 10.3389/fphys.2012.00405.
+
     Parameters
     ----------
     phases: ndarray
         The phase time series (in radians) of the signals with the shape (number_signals, duration).
-    
+
     Returns
     -------
     rho_group_i: ndarray
         The quantity rho, computed for each signal at each time step.
     rho_group: ndarray
         The quantity rho averaged over time.
     """
@@ -191,446 +193,452 @@
     q = np.arctan2(q_dash.imag, q_dash.real)
     # Individual level
     phi = phases - q
     phi_bar_dash = np.exp(phi * 1j).mean(axis=1)
     phi_bar = np.arctan2(phi_bar_dash.imag, phi_bar_dash.real)
     rho = np.abs(phi_bar_dash)
     # Group level
-    rho_group_i = np.abs(np.exp((phi - phi_bar[:,None]) * 1j).mean(axis=0))
+    rho_group_i = np.abs(np.exp((phi - phi_bar[:, None]) * 1j).mean(axis=0))
     rho_group = rho_group_i.mean()
-    
+
     return rho_group_i, rho_group
 
 
 def coherence_team(data, nperseg=None):
     """Returns the quantity defined by Reinero, Dikker, and Bavel as 'coherence' in "Inter-brain synchrony in teams predicts collective performance", doi: 10.1093/scan/nsaa135, with the quantity being averaged across the team.
-    
+
     Parameters
     ----------
     data: ndarray
         An array containing the time series of measurements with shape (number_signals, duration).
     nperseg: int
-        The number of time steps used to form a 'sample' of the signal when computing coherence, see scipy.signal.coherence documentation for more details. Optional, and will default to the lesser of (data duration / 4) and 256. 
-    
+        The number of time steps used to form a 'sample' of the signal when computing coherence, see scipy.signal.coherence documentation for more details. Optional, and will default to the lesser of (data duration / 4) and 256.
+
     Returns
     -------
     coherence: float
-        The quantity coherence. 
+        The quantity coherence.
     """
-    
+
     ## Set nperseg to a reasonable default value for shorter input lengths
     if nperseg is None:
-        if (data.shape[1] // 256) < 4:  ## Default value is 256 
+        if (data.shape[1] // 256) < 4:  ## Default value is 256
             nperseg = data.shape[1] // 4
-    
+
     coherence_scores = []
-    
+
     for i, x in enumerate(data):
-        
         for j, y in enumerate(data):
-            
             if i < j:
-                
-                coherence_scores.append(scipy.signal.coherence(x, y, nperseg=nperseg)[1].mean()) ## Actually we should just use the scipy coherence function
-                
+                coherence_scores.append(
+                    scipy.signal.coherence(x, y, nperseg=nperseg)[1].mean()
+                )
+
     return np.mean(coherence_scores)
 
 
 def sum_normalized_csd(data):
     """Returns a quantity, based on the cross-spectral density (CSD), similar to that of coherence_team() but which is less impacted by Gaussian noise.
-    
+
     Parameters
     ----------
     data: ndarray
         An array containing the time series of measurements with shape (number_signals, duration).
-    
+
     Returns
     -------
     aggregated_csd: float
         The sum-normalized CSD quantity.
     """
-    
+
     ## Set nperseg to a reasonable value for shorter input lengths
-    if data.shape[1] // 256 < 4: ## Default value is 256
-    
+    if data.shape[1] // 256 < 4:  ## Default value is 256
         nperseg = data.shape[1] // 4
-    
+
     else:
-    
-        nperseg = None ## Let scipy set it to default value
-    
+        nperseg = None  ## Let scipy set it to default value
+
     csd_scores = []
-    
+
     for i, x in enumerate(data):
-    
         for j, y in enumerate(data):
-        
             if i < j:
-            
                 csd_scores.append(
-                    (np.abs(scipy.signal.csd(x, y, nperseg=nperseg)[1]) ** 2).sum() / (scipy.signal.csd(x, x, nperseg=nperseg)[1] * scipy.signal.csd(y, y, nperseg=nperseg)[1]).sum()
+                    (np.abs(scipy.signal.csd(x, y, nperseg=nperseg)[1]) ** 2).sum()
+                    / (
+                        scipy.signal.csd(x, x, nperseg=nperseg)[1]
+                        * scipy.signal.csd(y, y, nperseg=nperseg)[1]
+                    ).sum()
                 )
-    
+
     return np.mean(csd_scores)
 
 
 def convert_to_terciles(data):
-    """Maps the input time series to numbers representing 'low', 'medium' and 'high' values. The thresholds for deciding 'low', 'medium' and 'high' are terciles. 
-    
+    """Maps the input time series to numbers representing 'low', 'medium' and 'high' values. The thresholds for deciding 'low', 'medium' and 'high' are terciles.
+
     Parameters
     ----------
     data: array
-        An array containing the time series of measurements for a single signal. 
-    
+        An array containing the time series of measurements for a single signal.
+
     Returns
     -------
     data_terciles: array
         An array where 0 represents a 'low' value, 1 represents a 'medium' value and 2 represents a 'high' value
     """
-    
-    terciles = np.quantile(data.reshape(-1),[1/3,2/3])
-    
+
+    terciles = np.quantile(data.reshape(-1), [1 / 3, 2 / 3])
+
     data_terciles = data.copy()
     data_terciles[:] = 2
-    data_terciles[data<terciles[1]] = 1
-    data_terciles[data<terciles[0]] = 0
-    
+    data_terciles[data < terciles[1]] = 1
+    data_terciles[data < terciles[0]] = 0
+
     return data_terciles
 
 
 def symbolic_entropy(data):
-    """Computes entropy after mapping the signals to numbers representing 'low', 'medium' and 'high' values, and then concatenating these numbers (across the signals) to create a 'pattern' at each time step. The thresholds for deciding 'low', 'medium' and 'high' are terciles. 
-    
+    """Computes entropy after mapping the signals to numbers representing 'low', 'medium' and 'high' values, and then concatenating these numbers (across the signals) to create a 'pattern' at each time step. The thresholds for deciding 'low', 'medium' and 'high' are terciles.
+
     Parameters
     ----------
     data: ndarray
-        An array containing the time series of measurements, with the shape (number_signals, duration). 
-    
+        An array containing the time series of measurements, with the shape (number_signals, duration).
+
     Returns
     -------
     pattern_entropy: float
-        The Shannon entropy of symbols found by mapping the input signals to 'low', 'medium' and 'high' and concatenating across signals. 
+        The Shannon entropy of symbols found by mapping the input signals to 'low', 'medium' and 'high' and concatenating across signals.
     """
-    
+
     data_terciles = np.apply_along_axis(convert_to_terciles, 1, data)
-    data_patterns = np.apply_along_axis(lambda x: "".join([str(int(y)) for y in x]), 0, data_terciles)
-    
-    pattern_probabilities = np.unique(data_patterns, return_counts=True)[1]/data_patterns.shape[0]
-    
+    data_patterns = np.apply_along_axis(
+        lambda x: "".join([str(int(y)) for y in x]), 0, data_terciles
+    )
+
+    pattern_probabilities = (
+        np.unique(data_patterns, return_counts=True)[1] / data_patterns.shape[0]
+    )
+
     return -np.sum(pattern_probabilities * np.log(pattern_probabilities))
 
 
 def kuramoto_weak_null(phases):
-    """Estimates the significance of the Kuramoto order parameter for a sample of multi-signal recordings, according to the 'weak null' test described by Frank and Richardson in "On a test statistic for the Kuramoto order parameter of synchronization: An illustration for group synchronization during rocking chairs", doi: 10.1016/j.physd.2010.07.015. 
-    
+    """Estimates the significance of the Kuramoto order parameter for a sample of multi-signal recordings, according to the 'weak null' test described by Frank and Richardson in "On a test statistic for the Kuramoto order parameter of synchronization: An illustration for group synchronization during rocking chairs", doi: 10.1016/j.physd.2010.07.015.
+
     Parameters
     ----------
     phases: list
-        A list containing the phase time series (in radians) for each member of the sample, with each phase time series being an array with the shape (number_signals, duration). Each multivariate time series in the sample can be a different duration, although different numbers of signals are not permissible. 
-    
+        A list containing the phase time series (in radians) for each member of the sample, with each phase time series being an array with the shape (number_signals, duration). Each multivariate time series in the sample can be a different duration, although different numbers of signals are not permissible.
+
     Returns
     -------
     p-value: float
         The p-value of the observed Kuramoto order parameter.
     t-statistic: float
         The t-statistic.
     df: float
         The degrees of freedom.
     """
-    
-    ## Check that the number of signals is the same in each time series 
-    assert len(np.unique(list(map(lambda x: x.shape[0], phases)))) == 1, "The number of signals in each time series must be consistent across the whole sample."
-    
+
+    ## Check that the number of signals is the same in each time series
+    assert (
+        len(np.unique(list(map(lambda x: x.shape[0], phases)))) == 1
+    ), "The number of signals in each time series must be consistent across the whole sample."
+
     def y_bar(phases):
-    
         kuramoto_r = np.abs(np.exp(phases * 1j).mean(axis=0))
-        
+
         y = kuramoto_r**2
-        
+
         return y.mean(axis=-1)
-    
+
     y_bars = np.fromiter(map(y_bar, phases), dtype=np.float)
-    
-    M = y_bars.mean() 
-    
-    mu = 1/phases[0].shape[0]
-    
+
+    M = y_bars.mean()
+
+    mu = 1 / phases[0].shape[0]
+
     s = y_bars.std()
-    
-    R_root = len(phases)**0.5
-    
+
+    R_root = len(phases) ** 0.5
+
     t_statistic = (M - mu) / (s / R_root)
-    
+
     df = len(phases) - 1
-    
-    return scipy.stats.t.sf(t_statistic, df=df), t_statistic, df ## This is a one-sided t-test
+
+    return (
+        scipy.stats.t.sf(t_statistic, df=df),
+        t_statistic,
+        df,
+    )  ## This is a one-sided t-test
 
 
 def metric_fixed_parameters(function, parameters):
-    """Returns a copy of a function to compute a metric, but with all parameters fixed except the data input. For use with apply_windowed. 
-    
+    """Returns a copy of a function to compute a metric, but with all parameters fixed except the data input. For use with apply_windowed.
+
     Parameters
     ----------
     function: function
         A function to compute a synchrony metric.
     parameters: dict
         A dictionary containing the parameters and their values for the function, except the main data input parameter.
-    
+
     Returns
     -------
     new_function: function
         A copy of the function to compute a synchrony metric, with all parameters fixed except the data input.
     """
-    
+
     parameters = copy.deepcopy(parameters)
-    
+
     def new_function(data):
-        
         return function(data, **parameters)
-    
+
     return new_function
 
 
 def apply_windowed(data, function, window_length, step=None):
-    """Applies a function in a windowed fashion to a time series with shape (number_signals, duration). 
-    
+    """Applies a function in a windowed fashion to a time series with shape (number_signals, duration).
+
     Parameters
     ----------
     data: ndarray
         An array containing the time series of measurements, with the shape (number_signals, duration).
     function: function
-        The function to apply within each window. 
+        The function to apply within each window.
     window_length: int
         The number of time steps to be included in a window.
     step: int
-        The number of time steps by which to move forward in order to obtain the next window. 
-    
+        The number of time steps by which to move forward in order to obtain the next window.
+
     Returns
     -------
     windowed_results: ndarray
-        A numpy array containing the results of the function when it is applied to each window. 
+        A numpy array containing the results of the function when it is applied to each window.
     """
-    
+
     if step is None:
-    
         step = window_length
-    
+
     def windowed_view(data, window_length, step):
-    
         dim_0 = 1 + (data.shape[1] - window_length) // step
         dim_1 = data.shape[0]
         dim_2 = window_length
-        
+
         if step is None:
             step = dim_2
-        
+
         stride_0, stride_1 = data.strides
-        
-        return np.lib.stride_tricks.as_strided(data, shape=(dim_0,dim_1,dim_2), strides=(stride_1 * step, stride_0, stride_1))
-    
+
+        return np.lib.stride_tricks.as_strided(
+            data,
+            shape=(dim_0, dim_1, dim_2),
+            strides=(stride_1 * step, stride_0, stride_1),
+        )
+
     return np.array(list(map(function, windowed_view(data, window_length, step))))
 
 
 def shuffle_recordings(data):
-    """Creates surrogate data by shuffling variables between time series in a sample of multivariate recordings. This assumes that all recordings in the sample are the same length. 
-    
+    """Creates surrogate data by shuffling variables between time series in a sample of multivariate recordings. This assumes that all recordings in the sample are the same length.
+
     Parameters
     ----------
     data: ndarray
-        An array containing a sample of recordings with shape (number_recordings, number_signals, duration). 
-    
+        An array containing a sample of recordings with shape (number_recordings, number_signals, duration).
+
     Returns
     -------
     surrogate_data: ndarray
         An array containing a sample of recordings where the variables have been shuffled between recordings, with shape (number_recordings, number_signals, duration).
     """
-    
+
     surrogate_shape = data.shape
-    
+
     surrogate_data = data.copy()
-    
-    surrogate_data = surrogate_data.reshape(surrogate_shape[0] * surrogate_shape[1],-1)
-    
+
+    surrogate_data = surrogate_data.reshape(surrogate_shape[0] * surrogate_shape[1], -1)
+
     np.random.shuffle(surrogate_data)
-    
-    return surrogate_data.reshape(surrogate_shape[0],surrogate_shape[1],-1)
+
+    return surrogate_data.reshape(surrogate_shape[0], surrogate_shape[1], -1)
 
 
 def shuffle_time_windows(data, window_length):
-    """Creates surrogate data by shuffling windows of data within each variable in a multivariate time series. 
-    
+    """Creates surrogate data by shuffling windows of data within each variable in a multivariate time series.
+
     Parameters
     ----------
     data: ndarray
         An array containing a multivariate recording with shape (number_signals, duration).
     window_length: int
-        The number of time steps to use as the window length. 
-    
+        The number of time steps to use as the window length.
+
     Returns
     -------
     surrogate_data: ndarray
         An array containing a multivariate recording where windows of time have been shuffled independently for each variable, with shape (number_signals, duration).
     """
-    
+
     def shuffle_individual(data):
-    
         surrogate_shape = data.shape
 
         surrogate_data = data.copy()
 
         surrogate_data = surrogate_data.reshape(-1, window_length)
 
         np.random.shuffle(surrogate_data)
 
         return surrogate_data.reshape(surrogate_shape[0])
-    
-    return np.apply_along_axis(shuffle_individual, -1, data)
 
+    return np.apply_along_axis(shuffle_individual, -1, data)
 
 
-def get_sync_coef( series_1, series_2, lag_length = 10):
+def get_sync_coef(series_1, series_2, lag_length=10):
     """
-    Finds the synchronisation coefficient for a pair of univariate time series. 
+    Finds the synchronisation coefficient for a pair of univariate time series.
 
     Parameters
     -----------
     series_1, series_2: ndarrays shape ( 1, duration )
-        The data to analyse. 
-    lag_length: int 
-        Default value is 10. See recommendations at page 23 ( for GSR use 1, 5, 6 or 20 ) of the paper "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" by Stephen J. Guastello and Anthony F. Peressini. 
+        The data to analyse.
+    lag_length: int
+        Default value is 10. See recommendations at page 23 ( for GSR use 1, 5, 6 or 20 ) of the paper "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" by Stephen J. Guastello and Anthony F. Peressini.
 
     Returns
     ---------
     sync_coef: float
         How much of series_1 is predicted by series_2 ( as described in "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" )
     """
 
-    # get Beta_2 from formula (6) 
+    # get Beta_2 from formula (6)
 
-    X_s1_s2_merged = np.r_[ '1, 2, 0', series_1, series_2 ][ :len(series_1) - lag_length ]
-    y_s1_dependent = series_1[ lag_length: ]
+    X_s1_s2_merged = np.r_["1, 2, 0", series_1, series_2][: len(series_1) - lag_length]
+    y_s1_dependent = series_1[lag_length:]
 
     lin_regr = LinearRegression()
     lin_regr.fit(X_s1_s2_merged, y_s1_dependent)
 
-    Beta_2  = lin_regr.coef_[1]
+    Beta_2 = lin_regr.coef_[1]
 
     return Beta_2
 
 
-def get_matrix_sync_coef( series, lag_length ):
+def get_matrix_sync_coef(series, lag_length):
     """
-    Finds all pairwise synchronisation coefficients for a multivariate time series. 
+    Finds all pairwise synchronisation coefficients for a multivariate time series.
 
     Parameters
     -----------
     series: ndarray
         A multivariate time series to analyse, with the shape (number_signals, duration).
     lag_length: int
-        The lag length to use. For more details of this parameter, see the paper "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" by Stephen J. Guastello and Anthony F. Peressini. 
-    
+        The lag length to use. For more details of this parameter, see the paper "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" by Stephen J. Guastello and Anthony F. Peressini.
+
     Returns
     --------
     m: ndarray
         A matrix of synchrony coefficients with shape ( number variables in multivariate input, number variables in multivariate input )
     """
 
     m = []
 
-    for i in range( len(series)) :
+    for i in range(len(series)):
         row = []
         for j in range(len(series)):
-            row.append(get_sync_coef(series[j], series[i], lag_length) ) 
+            row.append(get_sync_coef(series[j], series[i], lag_length))
         m.append(row)
-    
+
     return m
 
 
-def get_driver_scores( series, lag_length = 10 ):
+def get_driver_scores(series, lag_length=10):
     """
-    Finds the 'driver' scores for all the variables in a multivariate time series. 
+    Finds the 'driver' scores for all the variables in a multivariate time series.
 
     Parameters
     -----------
     series: ndarray
         A multivariate time series to analyse, with the shape (number_signals, duration).
     lag_length: int
-        The lag length to use. The default value is 10. For more details of this parameter, see the paper "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" by Stephen J. Guastello and Anthony F. Peressini. 
-    
+        The lag length to use. The default value is 10. For more details of this parameter, see the paper "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" by Stephen J. Guastello and Anthony F. Peressini.
+
     Returns
     -------
     driver_scores: array
-        An array containing the driver scores of participants. 
+        An array containing the driver scores of participants.
     """
 
-    m = get_matrix_sync_coef( series, lag_length )
+    m = get_matrix_sync_coef(series, lag_length)
 
-    driver_scores = np.sum( np.square(m), 1)
+    driver_scores = np.sum(np.square(m), 1)
 
     return driver_scores
 
 
-def get_empath_scores( series, lag_length = 10 ):
+def get_empath_scores(series, lag_length=10):
     """
-    Finds the 'empath' scores for all the variables in a multivariate time series. 
+    Finds the 'empath' scores for all the variables in a multivariate time series.
 
     Parameters
     -----------
     series: ndarray
         A multivariate time series to analyse, with the shape (number_signals, duration).
     lag_length: int
-        The lag length to use. The default value is 10. For more details of this parameter, see the paper "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" by Stephen J. Guastello and Anthony F. Peressini. 
-    
+        The lag length to use. The default value is 10. For more details of this parameter, see the paper "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" by Stephen J. Guastello and Anthony F. Peressini.
+
     Returns
     -------
     empath_scores: array
-        An array containing the empath scores of participants. 
+        An array containing the empath scores of participants.
     """
 
-    m = get_matrix_sync_coef( series, lag_length )
+    m = get_matrix_sync_coef(series, lag_length)
 
-    empath_scores = np.sum( np.square(m), 0)
+    empath_scores = np.sum(np.square(m), 0)
 
     return empath_scores
 
 
-def get_sync_index( series, lag_length = 10 ):
+def get_sync_index(series, lag_length=10):
     """
-    Finds the synchronisation index for a multivariate time series. 
+    Finds the synchronisation index for a multivariate time series.
 
     Parameters
     -----------
     series: ndarray
         A multivariate time series to analyse, with the shape (number_signals, duration).
     lag_length: int
-        The lag length to use. The default value is 10. For more details of this parameter, see the paper "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" by Stephen J. Guastello and Anthony F. Peressini. 
-    
+        The lag length to use. The default value is 10. For more details of this parameter, see the paper "Development of a Synchronization Coefficient for Biosocial Interactions in Groups and Teams" by Stephen J. Guastello and Anthony F. Peressini.
+
     Returns
     --------
     sync_index: float
         The Synchrony Index computed using the driver and empath scores.
     """
 
     # calculate Synchrony Index
 
     m = get_matrix_sync_coef(series, lag_length)
     empath_scores = get_empath_scores(series, lag_length)
 
     # identify the empath
-    empath_index = np.where( empath_scores == np.amax(empath_scores) )
+    empath_index = np.where(empath_scores == np.amax(empath_scores))
 
     # remove row of empath, create V, remove column of empath
-    M = np.array( m )
+    M = np.array(m)
 
     M = np.delete(M, empath_index, 0)  # delete row of empath
-    V = M[ :, empath_index]
+    V = M[:, empath_index]
     V = np.squeeze(V)
 
     M = np.delete(M, empath_index, 1)  # delete column of empath
 
     # take inverse of M and calculate vector of weights = Q
 
     M_inverse = np.linalg.inv(M)
-    Q = np.around( M_inverse.dot(V), 4 )
-    S = np.around(V.dot( Q ), 4 )
-    
+    Q = np.around(M_inverse.dot(V), 4)
+    S = np.around(V.dot(Q), 4)
+
     return S
```

### Comparing `multiSyncPy-0.1.0/multiSyncPy/visualisations.py` & `multiSyncPy-0.1.1/multiSyncPy/visualisations.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,477 +6,662 @@
  * plot_coherence - Calculates and visualises the coherence of a multivariate time series. 
  * plot_csd - Calculates and visualises the 'sum-normalized cross spectral density' of a multivariate time series. 
  * plot_rho - Calculates and visualises the cluster-phase 'rho' of a multivariate time series. 
  * plot_synchronyindex - Calculates and visualises the 'synchronization index' of a multivariate time series. 
 
 """
 
-import scipy 
-import numpy as np 
+import scipy
+import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 import matplotlib.ticker as ticker
-import multiSyncPy.synchrony_metrics as sm 
+import multiSyncPy.synchrony_metrics as sm
 
 
-def plot_entropy(data, window_length, step=None, figsize=None, custom_cols=None, gradient=False):  
+def plot_entropy(
+    data, window_length, step=None, figsize=None, custom_cols=None, gradient=False
+):
     """
-    Plots the windowed group entropy over a heatmap of the individual signals' tercile patterns.  
-    
+    Plots the windowed group entropy over a heatmap of the individual signals' tercile patterns.
+
     Parameters
     ----------
     data: ndarray
         An array containing the multivariate time series with shape (number_signals, duration).
     window_length: int
         The number of time steps to be included in a window.
     step: int
-        The number of time steps by which to move forward in order to obtain the next window. 
+        The number of time steps by which to move forward in order to obtain the next window.
     figsize: tuple
-        The width and height of the figure in inches, respectively. Default is (8,4). 
-    custom_cols: tuple 
-        The heatmap colormap/colors and line color to use for the plots. Default is (['#D4ECFC', '#FCF49C', '#FCC4AC'], 'black'). 
-    gradient: bool 
-        Determines whether the heatmap is displayed as a gradient, or matches the window and step size of the group metric. Default is False. 
-    
+        The width and height of the figure in inches, respectively. Default is (8,4).
+    custom_cols: tuple
+        The heatmap colormap/colors and line color to use for the plots. Default is (['#D4ECFC', '#FCF49C', '#FCC4AC'], 'black').
+    gradient: bool
+        Determines whether the heatmap is displayed as a gradient, or matches the window and step size of the group metric. Default is False.
+
     Returns
     -------
     figure: figure
         A figure containing the windowed group entropy and the individual signals' tercile patterns, along with axes labels and a colorbar.
     """
     if step is None:
-        step = window_length 
-    
+        step = window_length
+
     def windowed_view(data, window_length, step):
         dim_0 = 1 + (data.shape[1] - window_length) // step
         dim_1 = data.shape[0]
         dim_2 = window_length
-        
+
         if step is None:
             step = dim_2
         stride_0, stride_1 = data.strides
-        
-        return np.lib.stride_tricks.as_strided(data, shape=(dim_0,dim_1,dim_2), strides=(stride_1 * step, stride_0, stride_1))
 
-    if gradient == True: 
-        windowed_signals = (windowed_view(data, window_length=window_length, step=5)) # step size of 5 for the gradient 
-    else: 
-        windowed_signals = (windowed_view(data, window_length=window_length, step=step))
-        
-    yticks = [] # obtaining y tick labels from the number of windowed_signals 
-    for i in range(windowed_signals.shape[1]): 
-        yticks.append(i+1)
-
-    data_terciles = np.apply_along_axis(sm.convert_to_terciles, 1, windowed_signals).mean(axis=2).T
-
-    windowed_entropy =  sm.apply_windowed(data, sm.symbolic_entropy, window_length=window_length, step=step)
-
-    if figsize is None: 
-        figsize = (8,4)    
-    if custom_cols is None: 
-        custom_cols = (['#D4ECFC', '#FCF49C', '#FCC4AC'] , 'black')
-    
-    # Plotting 
-    figure, (ax1, cax) = plt.subplots(nrows=2, figsize=figsize,  gridspec_kw={"height_ratios":[1, 0.05]})
+        return np.lib.stride_tricks.as_strided(
+            data,
+            shape=(dim_0, dim_1, dim_2),
+            strides=(stride_1 * step, stride_0, stride_1),
+        )
+
+    if gradient == True:
+        windowed_signals = windowed_view(
+            data, window_length=window_length, step=5
+        )  # step size of 5 for the gradient
+    else:
+        windowed_signals = windowed_view(data, window_length=window_length, step=step)
+
+    yticks = []  # obtaining y tick labels from the number of windowed_signals
+    for i in range(windowed_signals.shape[1]):
+        yticks.append(i + 1)
+
+    data_terciles = (
+        np.apply_along_axis(sm.convert_to_terciles, 1, windowed_signals).mean(axis=2).T
+    )
+
+    windowed_entropy = sm.apply_windowed(
+        data, sm.symbolic_entropy, window_length=window_length, step=step
+    )
+
+    if figsize is None:
+        figsize = (8, 4)
+    if custom_cols is None:
+        custom_cols = (["#D4ECFC", "#FCF49C", "#FCC4AC"], "black")
+
+    # Plotting
+    figure, (ax1, cax) = plt.subplots(
+        nrows=2, figsize=figsize, gridspec_kw={"height_ratios": [1, 0.05]}
+    )
     figure.subplots_adjust(hspace=0.5)
-    gs = gridspec.GridSpec(2, 1, height_ratios=[1, 0.05]) # adding a second grid ontop of the subplots to overlay the group metric line onto the heatmap 
+    gs = gridspec.GridSpec(
+        2, 1, height_ratios=[1, 0.05]
+    )  # adding a second grid ontop of the subplots to overlay the group metric line onto the heatmap
     ax2 = figure.add_subplot(gs[0], frame_on=False)
-    ax1.set_xlim(0, data_terciles.shape[0]) # manually setting the x axis limits to ensure ticks of both plots are aligned 
+    ax1.set_xlim(
+        0, data_terciles.shape[0]
+    )  # manually setting the x axis limits to ensure ticks of both plots are aligned
     ax2.set_xlim(0, windowed_entropy.shape[0])
-    # plotting the heatmap 
-    cbar_kws = {'ticks': [0, 1, 2], 'label':'Individual pattern: 0=low, 1=medium, 2=high', 
-                'orientation':'horizontal'} 
-    sns.heatmap(data_terciles, linewidth=0, cmap=custom_cols[0], cbar_kws=cbar_kws, cbar_ax=cax, ax=ax1, yticklabels=yticks, vmin=0, vmax=2) 
-    # plotting the group metric 
+    # plotting the heatmap
+    cbar_kws = {
+        "ticks": [0, 1, 2],
+        "label": "Individual pattern: 0=low, 1=medium, 2=high",
+        "orientation": "horizontal",
+    }
+    sns.heatmap(
+        data_terciles,
+        linewidth=0,
+        cmap=custom_cols[0],
+        cbar_kws=cbar_kws,
+        cbar_ax=cax,
+        ax=ax1,
+        yticklabels=yticks,
+        vmin=0,
+        vmax=2,
+    )
+    # plotting the group metric
     ax2.plot(windowed_entropy, color=custom_cols[1], linewidth=1)
-    # editing axes labels and parameters 
-    ax1.tick_params(labelrotation=0) 
-    ax1.set(ylabel='Individual pattern')
+    # editing axes labels and parameters
+    ax1.tick_params(labelrotation=0)
+    ax1.set(ylabel="Individual pattern")
     ax1.get_xaxis().set_visible(False)
-    ax2.yaxis.tick_right()  
-    ax2.set(ylabel='Symbolic Entropy', xlabel=f'Time (window_length={window_length}, step={step})') 
-    ax2.yaxis.set_label_position('right')
-    
+    ax2.yaxis.tick_right()
+    ax2.set(
+        ylabel="Symbolic Entropy",
+        xlabel=f"Time (window_length={window_length}, step={step})",
+    )
+    ax2.yaxis.set_label_position("right")
+
     return figure
-    
 
-def plot_coherence(data, window_length, step=None, gradient=False, figsize=None, custom_cols=None, bounded_yaxis=True):
+
+def plot_coherence(
+    data,
+    window_length,
+    step=None,
+    gradient=False,
+    figsize=None,
+    custom_cols=None,
+    bounded_yaxis=True,
+):
     """
-    Plots the windowed group coherence over a heatmap of the pairwise signal coherence.  
-    
+    Plots the windowed group coherence over a heatmap of the pairwise signal coherence.
+
     Parameters
     ----------
     data: ndarray
         An array containing the multivariate time series with shape (number_signals, duration).
     window_length: int
         The number of time steps to be included in a window.
     step: int
-        The number of time steps by which to move forward in order to obtain the next window. 
-    gradient: bool 
-        Determines whether the heatmap is displayed as a gradient, or matches the window and step size of the group metric. Default is False. 
+        The number of time steps by which to move forward in order to obtain the next window.
+    gradient: bool
+        Determines whether the heatmap is displayed as a gradient, or matches the window and step size of the group metric. Default is False.
     figsize: tuple
-        The width and height of the figure in inches, respectively. Default is (8,4). 
-    custom_cols: tuple 
-        The heatmap colormap/colors and line color to use for the plots. Default is ('YlOrRd', 'black'). 
+        The width and height of the figure in inches, respectively. Default is (8,4).
+    custom_cols: tuple
+        The heatmap colormap/colors and line color to use for the plots. Default is ('YlOrRd', 'black').
     bounded_yaxis: bool
-        Determines whether the y-axis limits of the group metric are bounded to their range. Default is True. 
-        
+        Determines whether the y-axis limits of the group metric are bounded to their range. Default is True.
+
     Returns
     -------
     figure: figure
         A figure containing the windowed group coherence and the pairwise coherence, along with axes labels and a colorbar.
     """
-    if step is None: 
-        step = window_length 
-        
+    if step is None:
+        step = window_length
+
     def windowed_view(data, window_length, step):
         dim_0 = 1 + (data.shape[1] - window_length) // step
         dim_1 = data.shape[0]
         dim_2 = window_length
-        
+
         if step is None:
             step = dim_2
         stride_0, stride_1 = data.strides
-        
-        return np.lib.stride_tricks.as_strided(data, shape=(dim_0,dim_1,dim_2), strides=(stride_1 * step, stride_0, stride_1))
-    
-    if gradient == True: 
-        windowed_signals = (windowed_view(data, window_length=window_length, step=5)) # step size of 5 for the gradient 
-    else: 
-        windowed_signals = (windowed_view(data, window_length=window_length, step=step))
 
-    nperseg = None 
+        return np.lib.stride_tricks.as_strided(
+            data,
+            shape=(dim_0, dim_1, dim_2),
+            strides=(stride_1 * step, stride_0, stride_1),
+        )
+
+    if gradient == True:
+        windowed_signals = windowed_view(
+            data, window_length=window_length, step=5
+        )  # step size of 5 for the gradient
+    else:
+        windowed_signals = windowed_view(data, window_length=window_length, step=step)
+
+    nperseg = None
     if nperseg is None:
-        if (windowed_signals.shape[2] // 256) < 4:  ## Default value is 256 
+        if (windowed_signals.shape[2] // 256) < 4:  ## Default value is 256
             nperseg = windowed_signals.shape[2] // 4
-    
+
     paired_coherence = []
-    
+
     for dim in range(windowed_signals.shape[0]):
         temp_list = []
         signal_pairs = []
         for i, x in enumerate(windowed_signals[dim, :, :]):
             for j, y in enumerate(windowed_signals[dim, :, :]):
                 if i < j:
-                    temp_list.append(scipy.signal.coherence(x, y, nperseg=nperseg)[1].mean()) ## Actually we should just use the scipy coherence function
-                    signal_pairs.append(str(i+1)+'-'+str(j+1))
+                    temp_list.append(
+                        scipy.signal.coherence(x, y, nperseg=nperseg)[1].mean()
+                    )  ## Actually we should just use the scipy coherence function
+                    signal_pairs.append(str(i + 1) + "-" + str(j + 1))
         paired_coherence.append(temp_list)
-    
+
     paired_coherence = np.array(paired_coherence)
-    
-    windowed_coherence = sm.apply_windowed(data, sm.coherence_team, window_length=window_length, step=step)
 
-    if figsize is None: 
-        figsize = (8,4)
-    if custom_cols is None: 
-        custom_cols = ('YlOrRd', 'black')
-        
-    # Plotting 
-    figure, (ax1, cax) = plt.subplots(nrows=2, figsize=figsize,  gridspec_kw={"height_ratios":[1, 0.05]})
+    windowed_coherence = sm.apply_windowed(
+        data, sm.coherence_team, window_length=window_length, step=step
+    )
+
+    if figsize is None:
+        figsize = (8, 4)
+    if custom_cols is None:
+        custom_cols = ("YlOrRd", "black")
+
+    # Plotting
+    figure, (ax1, cax) = plt.subplots(
+        nrows=2, figsize=figsize, gridspec_kw={"height_ratios": [1, 0.05]}
+    )
     figure.subplots_adjust(hspace=0.5)
-    gs = gridspec.GridSpec(2, 1, height_ratios=[1, 0.05]) # adding a second grid ontop of the subplots to overlay the group metric line onto the heatmap 
+    gs = gridspec.GridSpec(
+        2, 1, height_ratios=[1, 0.05]
+    )  # adding a second grid ontop of the subplots to overlay the group metric line onto the heatmap
     ax2 = figure.add_subplot(gs[0], frame_on=False)
-    ax1.set_xlim(0, paired_coherence.shape[0]) # manually setting the x axis limits to ensure ticks of both plots are aligned 
+    ax1.set_xlim(
+        0, paired_coherence.shape[0]
+    )  # manually setting the x axis limits to ensure ticks of both plots are aligned
     ax2.set_xlim(0, windowed_coherence.shape[0])
-    # plotting the heatmap 
-    cbar_kws = {'label':'Coherence', 'orientation':'horizontal'}
-    sns.heatmap(paired_coherence.T, linewidth=0, cmap=custom_cols[0], cbar_kws=cbar_kws, cbar_ax=cax, ax=ax1, yticklabels=signal_pairs, vmin=0, vmax=1) 
+    # plotting the heatmap
+    cbar_kws = {"label": "Coherence", "orientation": "horizontal"}
+    sns.heatmap(
+        paired_coherence.T,
+        linewidth=0,
+        cmap=custom_cols[0],
+        cbar_kws=cbar_kws,
+        cbar_ax=cax,
+        ax=ax1,
+        yticklabels=signal_pairs,
+        vmin=0,
+        vmax=1,
+    )
     # plotting the group metric
     ax2.plot(windowed_coherence, color=custom_cols[1], linewidth=1)
-    # editing axes labels and parameters 
-    ax1.tick_params(labelrotation=0) 
-    ax1.set(ylabel='Pairwise Coherence')
+    # editing axes labels and parameters
+    ax1.tick_params(labelrotation=0)
+    ax1.set(ylabel="Pairwise Coherence")
     ax1.get_xaxis().set_visible(False)
     ax2.yaxis.tick_right()
-    ax2.set(ylabel='Group Coherence', xlabel=f'Time (window_length={window_length}, step={step})') 
-    ax2.yaxis.set_label_position('right')
-    if bounded_yaxis is True: 
+    ax2.set(
+        ylabel="Group Coherence",
+        xlabel=f"Time (window_length={window_length}, step={step})",
+    )
+    ax2.yaxis.set_label_position("right")
+    if bounded_yaxis is True:
         ax2.set_ylim(0, 1)
-    
-    return figure    
-    
 
-def plot_csd(data, window_length, step=None, gradient=False, figsize=None, custom_cols=None, bounded_yaxis=True):
+    return figure
+
+
+def plot_csd(
+    data,
+    window_length,
+    step=None,
+    gradient=False,
+    figsize=None,
+    custom_cols=None,
+    bounded_yaxis=True,
+):
     """
-    Plots the windowed group sum-normalized CSD over a heatmap of the pairwise sum-normalized CSD.  
-    
+    Plots the windowed group sum-normalized CSD over a heatmap of the pairwise sum-normalized CSD.
+
     Parameters
     ----------
     data: ndarray
         An array containing the multivariate time series with shape (number_signals, duration).
     window_length: int
         The number of time steps to be included in a window.
     step: int
-        The number of time steps by which to move forward in order to obtain the next window. 
-    gradient: bool 
-        Determines whether the heatmap is displayed as a gradient, or matches the window and step size of the group metric. Default is False. 
+        The number of time steps by which to move forward in order to obtain the next window.
+    gradient: bool
+        Determines whether the heatmap is displayed as a gradient, or matches the window and step size of the group metric. Default is False.
     figsize: tuple
-        The width and height of the figure in inches, respectively. Default is (8,4). 
-    custom_cols: tuple 
-        The heatmap colormap/colors and line color to use for the plots. Default is ('YlOrRd', 'black').  
+        The width and height of the figure in inches, respectively. Default is (8,4).
+    custom_cols: tuple
+        The heatmap colormap/colors and line color to use for the plots. Default is ('YlOrRd', 'black').
     bounded_yaxis: bool
-        Determines whether the y-axis limits of the group metric are bounded to their range. Default is True. 
-        
+        Determines whether the y-axis limits of the group metric are bounded to their range. Default is True.
+
     Returns
     -------
     figure: figure
         A figure containing the windowed group sum-normalized CSD and the pairwise sum-normalized CSD, along with axes labels and a colorbar.
     """
-    if step is None: 
-        step=window_length 
+    if step is None:
+        step = window_length
 
     def windowed_view(data, window_length, step):
         dim_0 = 1 + (data.shape[1] - window_length) // step
         dim_1 = data.shape[0]
         dim_2 = window_length
-        
+
         if step is None:
             step = dim_2
         stride_0, stride_1 = data.strides
-        
-        return np.lib.stride_tricks.as_strided(data, shape=(dim_0,dim_1,dim_2), strides=(stride_1 * step, stride_0, stride_1))
-    
-    if gradient == True: 
-        windowed_signals = (windowed_view(data, window_length=window_length, step=5)) # step size of 5 for the gradient 
-    else: 
-        windowed_signals = (windowed_view(data, window_length=window_length, step=step))
-        
-    if windowed_signals.shape[2] // 256 < 4: ## Default value is 256
+
+        return np.lib.stride_tricks.as_strided(
+            data,
+            shape=(dim_0, dim_1, dim_2),
+            strides=(stride_1 * step, stride_0, stride_1),
+        )
+
+    if gradient == True:
+        windowed_signals = windowed_view(
+            data, window_length=window_length, step=5
+        )  # step size of 5 for the gradient
+    else:
+        windowed_signals = windowed_view(data, window_length=window_length, step=step)
+
+    if windowed_signals.shape[2] // 256 < 4:  ## Default value is 256
         nperseg = windowed_signals.shape[2] // 4
     else:
-        nperseg = None ## Let scipy set it to default value
-    
+        nperseg = None  ## Let scipy set it to default value
+
     paired_sum_normalized_csd = []
-    
+
     for dim in range(windowed_signals.shape[0]):
         temp_list = []
         signal_pairs = []
         for i, x in enumerate(windowed_signals[dim, :, :]):
             for j, y in enumerate(windowed_signals[dim, :, :]):
                 if i < j:
                     temp_list.append(
-                    (np.abs(scipy.signal.csd(x, y, nperseg=nperseg)[1]) ** 2).sum() / (scipy.signal.csd(x, x, nperseg=nperseg)[1] * scipy.signal.csd(y, y, nperseg=nperseg)[1]).sum()
+                        (np.abs(scipy.signal.csd(x, y, nperseg=nperseg)[1]) ** 2).sum()
+                        / (
+                            scipy.signal.csd(x, x, nperseg=nperseg)[1]
+                            * scipy.signal.csd(y, y, nperseg=nperseg)[1]
+                        ).sum()
                     )
-                    signal_pairs.append(str(i+1)+'-'+str(j+1))
+                    signal_pairs.append(str(i + 1) + "-" + str(j + 1))
         paired_sum_normalized_csd.append(temp_list)
 
     paired_sum_normalized_csd = np.array(paired_sum_normalized_csd)
 
-    windowed_sum_normalized_csd = sm.apply_windowed(data, sm.sum_normalized_csd, window_length=window_length, step=step)
-    
-    if figsize is None: 
-        figsize = (8,4)
-    if custom_cols is None: 
-        custom_cols = ('YlOrRd', 'black')
-        
-    # Plotting 
-    figure, (ax1, cax) = plt.subplots(nrows=2, figsize=figsize,  gridspec_kw={"height_ratios":[1, 0.05]})
+    windowed_sum_normalized_csd = sm.apply_windowed(
+        data, sm.sum_normalized_csd, window_length=window_length, step=step
+    )
+
+    if figsize is None:
+        figsize = (8, 4)
+    if custom_cols is None:
+        custom_cols = ("YlOrRd", "black")
+
+    # Plotting
+    figure, (ax1, cax) = plt.subplots(
+        nrows=2, figsize=figsize, gridspec_kw={"height_ratios": [1, 0.05]}
+    )
     figure.subplots_adjust(hspace=0.5)
-    gs = gridspec.GridSpec(2, 1, height_ratios=[1, 0.05]) # adding a second grid ontop of the subplots to overlay the group metric line onto the heatmap 
+    gs = gridspec.GridSpec(
+        2, 1, height_ratios=[1, 0.05]
+    )  # adding a second grid ontop of the subplots to overlay the group metric line onto the heatmap
     ax2 = figure.add_subplot(gs[0], frame_on=False)
-    ax1.set_xlim(0, paired_sum_normalized_csd.shape[0]) # manually setting the x axis limits to ensure ticks of both plots are aligned 
+    ax1.set_xlim(
+        0, paired_sum_normalized_csd.shape[0]
+    )  # manually setting the x axis limits to ensure ticks of both plots are aligned
     ax2.set_xlim(0, windowed_sum_normalized_csd.shape[0])
-    # plotting the heatmap 
-    cbar_kws = {'label':'Sum-normalized CSD', 'orientation':'horizontal'}
-    sns.heatmap(paired_sum_normalized_csd.T, linewidth=0, cmap=custom_cols[0], cbar_kws=cbar_kws, cbar_ax=cax, ax=ax1, yticklabels=signal_pairs, vmin=0, vmax=1) 
+    # plotting the heatmap
+    cbar_kws = {"label": "Sum-normalized CSD", "orientation": "horizontal"}
+    sns.heatmap(
+        paired_sum_normalized_csd.T,
+        linewidth=0,
+        cmap=custom_cols[0],
+        cbar_kws=cbar_kws,
+        cbar_ax=cax,
+        ax=ax1,
+        yticklabels=signal_pairs,
+        vmin=0,
+        vmax=1,
+    )
     # plotting the group metric
     ax2.plot(windowed_sum_normalized_csd, color=custom_cols[1], linewidth=1)
-    # editing axes labels and parameters 
-    ax1.tick_params(labelrotation=0) 
-    ax1.set(ylabel='Pairwise CSD')
+    # editing axes labels and parameters
+    ax1.tick_params(labelrotation=0)
+    ax1.set(ylabel="Pairwise CSD")
     ax1.get_xaxis().set_visible(False)
     ax2.yaxis.tick_right()
-    ax2.set(ylabel='Group CSD', xlabel=f'Time (window_length={window_length}, step={step})') 
-    ax2.yaxis.set_label_position('right')
-    if bounded_yaxis is True: 
+    ax2.set(
+        ylabel="Group CSD", xlabel=f"Time (window_length={window_length}, step={step})"
+    )
+    ax2.yaxis.set_label_position("right")
+    if bounded_yaxis is True:
         ax2.set_ylim(0, 1)
-    
+
     return figure
 
 
-def plot_rho(phases, relative_phases=False, start=None, end=None, gradient=False, figsize=None, custom_cols=None, bounded_yaxis=True):
+def plot_rho(
+    phases,
+    relative_phases=False,
+    start=None,
+    end=None,
+    gradient=False,
+    figsize=None,
+    custom_cols=None,
+    bounded_yaxis=True,
+):
     """
-    Plots the group rho over a heatmap of the relative individual rho by default, and relative phase values of individual signals by choice.  
-    
+    Plots the group rho over a heatmap of the relative individual rho by default, and relative phase values of individual signals by choice.
+
     Parameters
     ----------
     data: ndarray
         An array containing the multivariate time series with shape (number_signals, duration).
-    relative_phases: bool 
-        Determines whether the individual relative phases (if True) or the individual rho values (if False) are plotted in the heatmap. Default is False, to plot the individual rho. 
+    relative_phases: bool
+        Determines whether the individual relative phases (if True) or the individual rho values (if False) are plotted in the heatmap. Default is False, to plot the individual rho.
     start: int
-        The starting point of the plot. Default is the first timestep of the signals' duration. 
+        The starting point of the plot. Default is the first timestep of the signals' duration.
     end: int
-        The ending point of the plot. Default is the last timestep of the signals' duration. 		
-    gradient: bool 
-        Determines whether the heatmap is displayed as a gradient, or matches the window and step size of the group metric. Default is False. 
+        The ending point of the plot. Default is the last timestep of the signals' duration.
+    gradient: bool
+        Determines whether the heatmap is displayed as a gradient, or matches the window and step size of the group metric. Default is False.
     figsize: tuple
-        The width and height of the figure in inches, respectively. Default is (8,4). 
-    custom_cols: tuple 
-        The colors and line color to use for the plots. Default is ('YlOrRd', 'black'). 
+        The width and height of the figure in inches, respectively. Default is (8,4).
+    custom_cols: tuple
+        The colors and line color to use for the plots. Default is ('YlOrRd', 'black').
     bounded_yaxis: bool
-        Determines whether the y-axis limits of the group metric are bounded to their range. Default is True. 
-        
+        Determines whether the y-axis limits of the group metric are bounded to their range. Default is True.
+
     Returns
     -------
     figure: figure
         A figure containing the time-varying group rho and individual rho, along with axes labels and a colorbar.
     """
     q_dash = np.exp(phases * 1j).mean(axis=0)
     q = np.arctan2(q_dash.imag, q_dash.real)
     phi = phases - q
     phi_bar_dash = np.exp(phi * 1j).mean(axis=1)
 
     phi_bar = np.arctan2(phi_bar_dash.imag, phi_bar_dash.real)
-    rho_individual = np.real(np.exp((phi - phi_bar[:,None]) * 1j))
+    rho_individual = np.real(np.exp((phi - phi_bar[:, None]) * 1j))
 
     time_varying_rho, mean_rho = sm.rho(phases)
 
-    if figsize is None: 
-        figsize = (8,4)
-    if custom_cols is None: 
-        custom_cols = ('YlOrRd', 'black')
+    if figsize is None:
+        figsize = (8, 4)
+    if custom_cols is None:
+        custom_cols = ("YlOrRd", "black")
     yticks = []
-    for i in range(phases.shape[0]): 
-        yticks.append(i+1)
-    
-    # Plotting 
-    figure, (ax1, cax) = plt.subplots(nrows=2, figsize=figsize,  gridspec_kw={"height_ratios":[1, 0.05]})
+    for i in range(phases.shape[0]):
+        yticks.append(i + 1)
+
+    # Plotting
+    figure, (ax1, cax) = plt.subplots(
+        nrows=2, figsize=figsize, gridspec_kw={"height_ratios": [1, 0.05]}
+    )
     figure.subplots_adjust(hspace=0.5)
-    gs = gridspec.GridSpec(2, 1, height_ratios=[1, 0.05]) # adding a second grid ontop of the subplots to overlay the group metric line onto the heatmap 
+    gs = gridspec.GridSpec(
+        2, 1, height_ratios=[1, 0.05]
+    )  # adding a second grid ontop of the subplots to overlay the group metric line onto the heatmap
     ax2 = figure.add_subplot(gs[0], frame_on=False)
-    if start is None: 
+    if start is None:
         start = 0
-    if end is None: 
+    if end is None:
         end = phases.shape[1]
-    ax1.set_xlim(start, end) # manually setting the x axis limits to ensure ticks of both plots are aligned 
+    ax1.set_xlim(
+        start, end
+    )  # manually setting the x axis limits to ensure ticks of both plots are aligned
     ax2.set_xlim(start, end)
-    # plotting the heatmap 
-    cbar_kws = {'label':'Cluster-phase Rho', 'orientation':'horizontal'}
-    sns.heatmap(rho_individual, linewidth=0, cmap=custom_cols[0], cbar_kws=cbar_kws, cbar_ax=cax, ax=ax1, yticklabels=yticks, vmin=0, vmax=1) 
+    # plotting the heatmap
+    cbar_kws = {"label": "Cluster-phase Rho", "orientation": "horizontal"}
+    sns.heatmap(
+        rho_individual,
+        linewidth=0,
+        cmap=custom_cols[0],
+        cbar_kws=cbar_kws,
+        cbar_ax=cax,
+        ax=ax1,
+        yticklabels=yticks,
+        vmin=0,
+        vmax=1,
+    )
     # plotting the group metric
     ax2.plot(time_varying_rho, color=custom_cols[1], linewidth=1)
-    
-    # editing axes labels and parameters 
-    ax1.tick_params(labelrotation=0) 
-    ax1.set(ylabel='Individual Rho')
+
+    # editing axes labels and parameters
+    ax1.tick_params(labelrotation=0)
+    ax1.set(ylabel="Individual Rho")
     ax1.get_xaxis().set_visible(False)
     ax2.yaxis.tick_right()
-    #ax2.xaxis.set_major_locator(ticker.MultipleLocator(5))
-    ax2.set(ylabel='Group Rho', xlabel='Time') 
-    ax2.yaxis.set_label_position('right')
-    if bounded_yaxis is True: 
+    # ax2.xaxis.set_major_locator(ticker.MultipleLocator(5))
+    ax2.set(ylabel="Group Rho", xlabel="Time")
+    ax2.yaxis.set_label_position("right")
+    if bounded_yaxis is True:
         ax2.set_ylim(0, 1)
-    
+
     return figure
 
 
-def plot_synchronyindex(data, window_length, step=None, driver=True, lag_length=10, gradient=False, figsize=None, custom_cols=None): 
+def plot_synchronyindex(
+    data,
+    window_length,
+    step=None,
+    driver=True,
+    lag_length=10,
+    gradient=False,
+    figsize=None,
+    custom_cols=None,
+):
     """
-    Plots the windowed synchrony index over a heatmap of either the drivers or empaths of synchrony. 
-    
+    Plots the windowed synchrony index over a heatmap of either the drivers or empaths of synchrony.
+
     Parameters
     ----------
     data: ndarray
         An array containing the multivariate time series with shape (number_signals, duration).
     window_length: int
         The number of time steps to be included in a window.
     step: int
-        The number of time steps by which to move forward in order to obtain the next window. 
+        The number of time steps by which to move forward in order to obtain the next window.
     driver: bool
-        Determines whether the drivers (if True) or the empaths (if False) are plotted in the heatmap. Default is True, to plot the drivers. 
+        Determines whether the drivers (if True) or the empaths (if False) are plotted in the heatmap. Default is True, to plot the drivers.
     lag_length: int
         The number of samples for lag length - used by the synchrony metric, default = 10.
-    gradient: bool 
-        Determines whether the heatmap is displayed as a gradient, or matches the window and step size of the group metric. Default is False. 
+    gradient: bool
+        Determines whether the heatmap is displayed as a gradient, or matches the window and step size of the group metric. Default is False.
     figsize: tuple
-        The width and height of the figure in inches, respectively. Default is (8,4). 
-    custom_cols: tuple 
-        The colors and line color to use for the plots. Default is ('YlOrRd', 'black'). 
+        The width and height of the figure in inches, respectively. Default is (8,4).
+    custom_cols: tuple
+        The colors and line color to use for the plots. Default is ('YlOrRd', 'black').
 
     Returns
     -------
     figure: figure
         A figure containing the windowed group synchrony index and the windowed driver or empath scores for each signal, along with axes labels and a colorbar.
-    """    
-    if step is None: 
-        step = window_length 
+    """
+    if step is None:
+        step = window_length
 
     synchrony_index = sm.apply_windowed(
-        data, 
-        lambda x: sm.get_sync_index(x, lag_length=lag_length), 
-        window_length=window_length, 
-        step=step)
-        
-    if figsize is None:  
-        figsize = (8,4)  
-    if custom_cols is None: 
-        custom_cols = ('YlOrRd', 'black')
+        data,
+        lambda x: sm.get_sync_index(x, lag_length=lag_length),
+        window_length=window_length,
+        step=step,
+    )
+
+    if figsize is None:
+        figsize = (8, 4)
+    if custom_cols is None:
+        custom_cols = ("YlOrRd", "black")
     yticks = []
-    for i in range(data.shape[0]): 
-        yticks.append(i+1)
-    
+    for i in range(data.shape[0]):
+        yticks.append(i + 1)
+
     # Plotting
-    figure, (ax1, cax) = plt.subplots(nrows=2, figsize=figsize,  gridspec_kw={"height_ratios":[1, 0.05]})
+    figure, (ax1, cax) = plt.subplots(
+        nrows=2, figsize=figsize, gridspec_kw={"height_ratios": [1, 0.05]}
+    )
     figure.subplots_adjust(hspace=0.5)
-    gs = gridspec.GridSpec(2, 1, height_ratios=[1, 0.05]) # adding a second grid ontop of the subplots to overlay the group metric line onto the heatmap 
+    gs = gridspec.GridSpec(
+        2, 1, height_ratios=[1, 0.05]
+    )  # adding a second grid ontop of the subplots to overlay the group metric line onto the heatmap
     ax2 = figure.add_subplot(gs[0], frame_on=False)
     # Driver visualization
-    if driver == True:   
-        if gradient == True: 
+    if driver == True:
+        if gradient == True:
             w_data = sm.apply_windowed(
-                data, 
-                lambda x: sm.get_driver_scores(x, lag_length=lag_length), 
-                window_length=window_length, 
-                step=5) # step size of 5 for the gradient
-        else: 
+                data,
+                lambda x: sm.get_driver_scores(x, lag_length=lag_length),
+                window_length=window_length,
+                step=5,
+            )  # step size of 5 for the gradient
+        else:
             w_data = sm.apply_windowed(
-                data, 
-                lambda x: sm.get_driver_scores(x, lag_length=lag_length), 
-                window_length=window_length, 
-                step=step)
-            
+                data,
+                lambda x: sm.get_driver_scores(x, lag_length=lag_length),
+                window_length=window_length,
+                step=step,
+            )
+
         norm_w_data = []
-        for window in range( len( w_data[ : , 0 ] ) ):
-            norm_w_data.append((w_data[ window ] - np.amin(w_data[ window ])) / (np.max(w_data[ window ]) - np.min(w_data[ window ])))
+        for window in range(len(w_data[:, 0])):
+            norm_w_data.append(
+                (w_data[window] - np.amin(w_data[window]))
+                / (np.max(w_data[window]) - np.min(w_data[window]))
+            )
         norm_w_data = np.array(norm_w_data).T
-        
-        cbar_kws = {'label':'Driver score', 'orientation':'horizontal'}
-        sns.heatmap(norm_w_data, linewidth=0, cmap=custom_cols[0], cbar_kws=cbar_kws, cbar_ax=cax, ax=ax1, yticklabels=yticks, vmin=0, vmax=1) 
-        ax1.set(ylabel='Individual Driver Scores')
-        ax2.plot(synchrony_index, color=custom_cols[1], linewidth=1)  
-        ax1.set_xlim(0, norm_w_data.shape[1]) # manually setting the x axis limits to ensure ticks of both plots are aligned 
+
+        cbar_kws = {"label": "Driver score", "orientation": "horizontal"}
+        sns.heatmap(
+            norm_w_data,
+            linewidth=0,
+            cmap=custom_cols[0],
+            cbar_kws=cbar_kws,
+            cbar_ax=cax,
+            ax=ax1,
+            yticklabels=yticks,
+            vmin=0,
+            vmax=1,
+        )
+        ax1.set(ylabel="Individual Driver Scores")
+        ax2.plot(synchrony_index, color=custom_cols[1], linewidth=1)
+        ax1.set_xlim(
+            0, norm_w_data.shape[1]
+        )  # manually setting the x axis limits to ensure ticks of both plots are aligned
         ax2.set_xlim(0, len(synchrony_index))
     # Empath visualization
-    else:   
-        if gradient == True: 
+    else:
+        if gradient == True:
             w_data = sm.apply_windowed(
-                data, 
-                lambda x: sm.get_empath_scores(x, lag_length=lag_length), 
-                window_length=window_length, 
-                step=5) # step size of 5 for the gradient
-        else: 
+                data,
+                lambda x: sm.get_empath_scores(x, lag_length=lag_length),
+                window_length=window_length,
+                step=5,
+            )  # step size of 5 for the gradient
+        else:
             w_data = sm.apply_windowed(
-                data, 
-                lambda x: sm.get_empath_scores(x, lag_length=lag_length), 
-                window_length=window_length, 
-                step=step)
-            
+                data,
+                lambda x: sm.get_empath_scores(x, lag_length=lag_length),
+                window_length=window_length,
+                step=step,
+            )
+
         norm_w_data = []
-        for window in range( len( w_data[ : , 0 ] ) ):
-            norm_w_data.append((w_data[ window ] - np.amin(w_data[ window ])) / (np.max(w_data[ window ]) - np.min(w_data[ window ])))
+        for window in range(len(w_data[:, 0])):
+            norm_w_data.append(
+                (w_data[window] - np.amin(w_data[window]))
+                / (np.max(w_data[window]) - np.min(w_data[window]))
+            )
         norm_w_data = np.array(norm_w_data).T
-        
-        cbar_kws = {'label':'Driver score', 'orientation':'horizontal'}
-        sns.heatmap(norm_w_data, linewidth=0, cmap=custom_cols[0], cbar_kws=cbar_kws, cbar_ax=cax, ax=ax1, yticklabels=yticks, vmin=0, vmax=1) 
-        ax1.set(ylabel='Individual Empath Scores')
-        ax2.plot(synchrony_index, color=custom_cols[1], linewidth=1)  
-        ax1.set_xlim(0, norm_w_data.shape[1]) # manually setting the x axis limits to ensure ticks of both plots are aligned 
+
+        cbar_kws = {"label": "Driver score", "orientation": "horizontal"}
+        sns.heatmap(
+            norm_w_data,
+            linewidth=0,
+            cmap=custom_cols[0],
+            cbar_kws=cbar_kws,
+            cbar_ax=cax,
+            ax=ax1,
+            yticklabels=yticks,
+            vmin=0,
+            vmax=1,
+        )
+        ax1.set(ylabel="Individual Empath Scores")
+        ax2.plot(synchrony_index, color=custom_cols[1], linewidth=1)
+        ax1.set_xlim(
+            0, norm_w_data.shape[1]
+        )  # manually setting the x axis limits to ensure ticks of both plots are aligned
         ax2.set_xlim(0, len(synchrony_index))
-    # editing axes labels and parameters 
-    ax1.tick_params(labelrotation=0) 
+    # editing axes labels and parameters
+    ax1.tick_params(labelrotation=0)
     ax1.get_xaxis().set_visible(False)
     ax2.yaxis.tick_right()
-    ax2.set(ylabel='Group Synchrony Index', xlabel=f'Time (window_length={window_length}, step={step})') 
-    ax2.yaxis.set_label_position('right')
+    ax2.set(
+        ylabel="Group Synchrony Index",
+        xlabel=f"Time (window_length={window_length}, step={step})",
+    )
+    ax2.yaxis.set_label_position("right")
 
-    return figure
+    return figure
```

### Comparing `multiSyncPy-0.1.0/multiSyncPy.egg-info/PKG-INFO` & `multiSyncPy-0.1.1/multiSyncPy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: multiSyncPy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functions to quantify multivariate synchrony
 Home-page: https://github.com/cslab-hub/multiSyncPy
 Author: Dan Hudson
 Author-email: daniel.dominic.hudson@uni-osnabrueck.de
 License: GNU LGPL
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-**Important announcement** - *There is an issue with the calculation of determinism in version 0.0.3 and below; update to version 0.0.4 or above to receive the fix (pip install --upgrade multiSyncPy). Thanks to @mrrezaie for spotting the issue. Please inform anyone you know who might be using multiSyncPy.*
+**Important announcement** - *There is a new version of multiSyncPy (0.1.0) that includes a new multivariate synchronization measures as well as some visualiation functions.*
 
 # multiSyncPy
 
-multiSyncPy is a Python package for quantifying multivariate synchrony. Our package supports the burgeoning field of research into synchrony, making accessible a set of methods for studying group-level rather than dyadic constructs of synchrony and/or coordination. We offer a range of metrics for estimating mulivariate synchrony based on a collection of those used in recent literature.
+multiSyncPy is a Python package for quantifying multivariate synchrony. Our package supports the burgeoning field of research into synchrony, making accessible a set of methods for studying group-level rather than dyadic constructs of synchrony and/or coordination. We offer a range of metrics for estimating multivariate synchrony based on a collection of those used in recent literature.
 
 The main methods of this package are functions to calculate:
 
  * symbolic entropy, 
  * multidimensional recurrence quantification, 
  * coherence (and a related 'sum-normalized CSD' metric),
  * the cluster-phase 'Rho' metric
- * the synchronization coefficient metric, and 
- * a statistical test based on the Kuramoto order parameter
+ * the synchronization coefficient metric,
+ * a statistical test based on the Kuramoto order parameter, and
+ * driver-empath model with synchrony index
 
 We also include functions for two surrogation techniques to compare the observed coordination dynamics with chance levels.
 
+Additionally, we include a set of functions to visualize the time-varying coordination metrics as well as the individual or pair-wise contributions to the multivariate measure (depending on the particular method).
+
 multiSyncPy is freely available under the LGPL license. The source code is maintained at <https://github.com/cslab-hub/multiSyncPy>, which also includes examples of usage of the package. Documentation can be accessed through `help()` or accessed at <https://cslab-hub.github.io/multiSyncPy/>. 
 
-Further details of the package and case studies of its use on real-world data are described in our paper 
+Further details of the package and case studies of its use on real-world data are described in our paper. 
 
 Hudson, D., Wiltshire, T.J. & Atzmueller, M. multiSyncPy: A Python package for assessing multivariate coordination dynamics. *Behav Res* (2022). <https://doi.org/10.3758/s13428-022-01855-y>. 
 
 Please cite this paper if you use multiSyncPy in your research.
```

### Comparing `multiSyncPy-0.1.0/setup.py` & `multiSyncPy-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="multiSyncPy",
-    version="0.1.0",
+    version="0.1.1",
     description="Functions to quantify multivariate synchrony",
-    long_description=README,
     long_description_content_type="text/markdown",
+    long_description=README,
     url="https://github.com/cslab-hub/multiSyncPy",
     author="Dan Hudson",
     author_email="daniel.dominic.hudson@uni-osnabrueck.de",
     license="GNU LGPL",
     classifiers=[
         "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
     ],
     packages=["multiSyncPy"],
     ##include_package_data=True,
-    install_requires=["numpy", "scipy", "sklearn", "seaborn", "matplotlib"]
+    install_requires=["numpy", "scipy", "scikit-learn", "seaborn", "matplotlib"],
 )
```

