# Comparing `tmp/linien-server-0.8.0rc8.tar.gz` & `tmp/linien-server-0.8.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-server-0.8.0rc8.tar", last modified: Wed Jul  5 09:23:53 2023, max compression
+gzip compressed data, was "linien-server-0.8.0rc9.tar", last modified: Wed Jul  5 12:52:53 2023, max compression
```

## Comparing `linien-server-0.8.0rc8.tar` & `linien-server-0.8.0rc9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/linien_server/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/acquisition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/linien_server/autolock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/algorithm_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/autolock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/robust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/csr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/csrmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/iir_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)  2083740 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/linien.bin
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/linien_install_requirements.sh
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/linien_start_server.sh
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/linien_stop_server.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/linien_server/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/approach_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/linien_server/pid_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/pid_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/pid_optimization/pid_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/linien_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:52:53.300067 linien-server-0.8.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 12:52:53.300067 linien-server-0.8.0rc9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:52:53.296067 linien-server-0.8.0rc9/linien_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/acquisition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:52:53.296067 linien-server-0.8.0rc9/linien_server/autolock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/autolock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/autolock/algorithm_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/autolock/autolock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/autolock/fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/autolock/robust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/autolock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/csrmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/iir_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2083740 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/linien.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/linien_install_requirements.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/linien_start_server.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/linien_stop_server.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:52:53.296067 linien-server-0.8.0rc9/linien_server/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/optimization/approach_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/optimization/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/optimization/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/optimization/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:52:53.296067 linien-server-0.8.0rc9/linien_server/pid_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/pid_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/pid_optimization/pid_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/linien_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:52:53.296067 linien-server-0.8.0rc9/linien_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 12:52:53.000000 linien-server-0.8.0rc9/linien_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-05 12:52:53.000000 linien-server-0.8.0rc9/linien_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:52:53.000000 linien-server-0.8.0rc9/linien_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 12:52:53.000000 linien-server-0.8.0rc9/linien_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-05 12:52:53.000000 linien-server-0.8.0rc9/linien_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 12:52:53.000000 linien-server-0.8.0rc9/linien_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:52:53.300067 linien-server-0.8.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-05 12:52:27.000000 linien-server-0.8.0rc9/setup.py
```

### Comparing `linien-server-0.8.0rc8/PKG-INFO` & `linien-server-0.8.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-server
-Version: 0.8.0rc8
+Version: 0.8.0rc9
 Summary: Server components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-server-0.8.0rc8/linien_server/acquisition.py` & `linien-server-0.8.0rc9/linien_server/acquisition.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/autolock/algorithm_selection.py` & `linien-server-0.8.0rc9/linien_server/autolock/algorithm_selection.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/autolock/autolock.py` & `linien-server-0.8.0rc9/linien_server/autolock/autolock.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/autolock/fast.py` & `linien-server-0.8.0rc9/linien_server/autolock/fast.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/autolock/robust.py` & `linien-server-0.8.0rc9/linien_server/autolock/robust.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/autolock/utils.py` & `linien-server-0.8.0rc9/linien_server/autolock/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/csr.py` & `linien-server-0.8.0rc9/linien_server/csr.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/csrmap.py` & `linien-server-0.8.0rc9/linien_server/csrmap.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/iir_coeffs.py` & `linien-server-0.8.0rc9/linien_server/iir_coeffs.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/influxdb.py` & `linien-server-0.8.0rc9/linien_server/influxdb.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/linien.bin` & `linien-server-0.8.0rc9/linien_server/linien.bin`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/linien_start_server.sh` & `linien-server-0.8.0rc9/linien_server/linien_start_server.sh`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/optimization/approach_line.py` & `linien-server-0.8.0rc9/linien_server/optimization/approach_line.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/optimization/engine.py` & `linien-server-0.8.0rc9/linien_server/optimization/engine.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/optimization/general.py` & `linien-server-0.8.0rc9/linien_server/optimization/general.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/optimization/optimization.py` & `linien-server-0.8.0rc9/linien_server/optimization/optimization.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/optimization/utils.py` & `linien-server-0.8.0rc9/linien_server/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/parameters.py` & `linien-server-0.8.0rc9/linien_server/parameters.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/pid_optimization/pid_optimization.py` & `linien-server-0.8.0rc9/linien_server/pid_optimization/pid_optimization.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/registers.py` & `linien-server-0.8.0rc9/linien_server/registers.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server/server.py` & `linien-server-0.8.0rc9/linien_server/server.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/linien_server.egg-info/PKG-INFO` & `linien-server-0.8.0rc9/linien_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-server
-Version: 0.8.0rc8
+Version: 0.8.0rc9
 Summary: Server components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-server-0.8.0rc8/linien_server.egg-info/SOURCES.txt` & `linien-server-0.8.0rc9/linien_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc8/setup.py` & `linien-server-0.8.0rc9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
-version = "0.8.0rc8"
+version = "0.8.0rc9"
 
 setup(
     name="linien-server",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
@@ -41,15 +41,15 @@
     python_requires=">=3.5",
     install_requires=[
         "appdirs>=1.4.4",
         "certifi==2021.10.8;python_version<'3.10'",  # pinned because of bug in pip 9.0.1, see #339 # noqa: E501
         "click>=7.1.2",
         "cma>=3.0.3",
         "pylpsd>=0.1.4",
-        "pyrp3>=1.1.0;platform_machine=='armv7l'",  # only install on RedPitaya
+        "pyrp3>=1.1.0,<2.0;platform_machine=='armv7l'",  # only install on RedPitaya
         "requests==2.25.1;python_version<'3.10'",  # pinned because of bug in pip 9.0.1, see #339 # noqa: E501
         "requests>=2.25.1;python_version>='3.10'",
         "linien-common=={}".format(version),
     ],
     scripts=[
         "linien_server/linien_start_server.sh",
         "linien_server/linien_stop_server.sh",
```

