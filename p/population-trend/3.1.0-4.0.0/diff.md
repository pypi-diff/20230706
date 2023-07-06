# Comparing `tmp/population_trend-3.1.0.tar.gz` & `tmp/population_trend-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "population_trend-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "population_trend-4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `population_trend-3.1.0.tar` & `population_trend-4.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1037 2023-07-04 23:17:38.042354 population_trend-3.1.0/README.md
--rw-r--r--   0        0        0      251 2023-07-04 23:17:38.042354 population_trend-3.1.0/population_trend/__init__.py
--rw-r--r--   0        0        0     6901 2023-07-04 23:17:38.042354 population_trend-3.1.0/population_trend/calculate_growth_rates.py
--rw-r--r--   0        0        0     1894 2023-07-04 23:17:38.042354 population_trend-3.1.0/population_trend/cli.py
--rw-r--r--   0        0        0      403 2023-07-04 23:17:38.042354 population_trend-3.1.0/population_trend/filter_data.py
--rw-r--r--   0        0        0     4361 2023-07-04 23:17:38.042354 population_trend-3.1.0/population_trend/population_growth_model.py
--rw-r--r--   0        0        0      495 2023-07-04 23:17:38.042354 population_trend-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1037 2023-07-06 17:37:44.730400 population_trend-4.0.0/README.md
+-rw-r--r--   0        0        0      251 2023-07-06 17:37:44.730400 population_trend-4.0.0/population_trend/__init__.py
+-rw-r--r--   0        0        0     6901 2023-07-06 17:37:44.730400 population_trend-4.0.0/population_trend/calculate_growth_rates.py
+-rw-r--r--   0        0        0     2627 2023-07-06 17:37:44.730400 population_trend-4.0.0/population_trend/cli.py
+-rw-r--r--   0        0        0      403 2023-07-06 17:37:44.730400 population_trend-4.0.0/population_trend/filter_data.py
+-rw-r--r--   0        0        0     4732 2023-07-06 17:37:44.730400 population_trend-4.0.0/population_trend/population_growth_model.py
+-rw-r--r--   0        0        0      495 2023-07-06 17:37:44.730400 population_trend-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-4.0.0/PKG-INFO
```

### Comparing `population_trend-3.1.0/README.md` & `population_trend-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `population_trend-3.1.0/population_trend/calculate_growth_rates.py` & `population_trend-4.0.0/population_trend/calculate_growth_rates.py`

 * *Files identical despite different names*

### Comparing `population_trend-3.1.0/population_trend/population_growth_model.py` & `population_trend-4.0.0/population_trend/population_growth_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 
 class Population_Trend_Model:
     def __init__(self, fit_data, intervals, interest_variable):
         self.intervals = intervals
         self.model_domain = calculate_model_domain(fit_data)
         self.initial_population = lambda_calculator(
             fit_data["Temporada"], fit_data[interest_variable]
-        )[1]
+        )
 
     @property
     def model_min(self):
-        return power_law(self.model_domain, self.intervals[0], self.initial_population)
+        return power_law(self.model_domain, self.intervals[0][0], self.intervals[0][1])
 
     @property
     def model_med(self):
-        return power_law(self.model_domain, self.intervals[1], self.initial_population)
+        return power_law(self.model_domain, self.intervals[1][0], self.intervals[1][1])
 
     @property
     def model_max(self):
-        return power_law(self.model_domain, self.intervals[2], self.initial_population)
+        return power_law(self.model_domain, self.intervals[2][0], self.intervals[2][1])
 
 
 class Plotter_Population_Trend_Model:
     def __init__(self, data):
         self.fig, self.ax = geci_plot()
         self.data = data
         self.plot_seasons = self.data["Temporada"][:] - self.data["Temporada"].iloc[0] + 1
@@ -53,18 +53,29 @@
         self.ticks_positions = ticks_positions_array(self.ticks_text)
         self.plot_domain = np.linspace(self.ticks_positions.min(), self.ticks_positions.max(), 100)
 
     def plot_smooth(self, Population_Trend_Model):
         self.ax.fill_between(
             self.plot_domain,
             Population_Trend_Model.model_min,
-            Population_Trend_Model.model_max,
-            alpha=0.2,
+            Population_Trend_Model.model_med,
             label="Confidence zone",
-            color="b",
+            color="powderblue",
+        )
+        self.ax.fill_between(
+            self.plot_domain,
+            Population_Trend_Model.model_med,
+            Population_Trend_Model.model_max,
+            color="powderblue",
+        )
+        self.ax.fill_between(
+            self.plot_domain,
+            Population_Trend_Model.model_min,
+            Population_Trend_Model.model_max,
+            color="powderblue",
         )
 
     def plot_model(self, Population_Trend_Model):
         plt.plot(
             self.plot_domain,
             Population_Trend_Model.model_med,
             label="Population growth model",
```

### Comparing `population_trend-3.1.0/PKG-INFO` & `population_trend-4.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: population_trend
-Version: 3.1.0
+Version: 4.0.0
 Summary: A template Python module
 Home-page: https://github.com/IslasGECI/population_trend
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Dist: bootstrapping-tools==2.0.0
+Requires-Dist: bootstrapping-tools==3.0.0
 Requires-Dist: geci-plots
 Requires-Dist: typer
 
 <a href="https://www.islas.org.mx/"><img src="https://www.islas.org.mx/img/logo.svg" align="right" width="256" /></a>
 # Dummy Transformations
 
 Para usar este repo como plantilla debemos hacer lo siguiente:
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: population_trend Version: 3.1.0 Summary: A template
+Metadata-Version: 2.1 Name: population_trend Version: 4.0.0 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/population_trend Author:
 Ciencia de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-
 Python: >=3.9 Description-Content-Type: text/markdown Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
-bootstrapping-tools==2.0.0 Requires-Dist: geci-plots Requires-Dist: typer
+bootstrapping-tools==3.0.0 Requires-Dist: geci-plots Requires-Dist: typer
 [https://www.islas.org.mx/img/logo.svg] # Dummy Transformations Para usar este
 repo como plantilla debemos hacer lo siguiente: 1. Presiona el botÃ³n verde que
 dice _Use this template_ 1. Selecciona como dueÃ±o a la organizaciÃ³n IslasGECI
 1. Agrega el nombre del nuevo mÃ³dulo de python 1. Presiona el botÃ³n _Create
 repository from template_ 1. Reemplaza `dummy_transformations` por el nombre
 del nuevo mÃ³dulo en: - `Makefile` - `pyproject.toml` -
 `tests\test_transformations.py` 1. Renombra el archivo
```

