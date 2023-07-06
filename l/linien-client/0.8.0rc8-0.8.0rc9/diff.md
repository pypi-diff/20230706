# Comparing `tmp/linien-client-0.8.0rc8.tar.gz` & `tmp/linien-client-0.8.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-client-0.8.0rc8.tar", last modified: Wed Jul  5 09:24:09 2023, max compression
+gzip compressed data, was "linien-client-0.8.0rc9.tar", last modified: Wed Jul  5 12:53:07 2023, max compression
```

## Comparing `linien-client-0.8.0rc8.tar` & `linien-client-0.8.0rc9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:24:09.254231 linien-client-0.8.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-05 09:24:09.254231 linien-client-0.8.0rc8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:24:09.254231 linien-client-0.8.0rc8/linien_client/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/linien_client/remote_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:24:09.254231 linien-client-0.8.0rc8/linien_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-05 09:24:09.000000 linien-client-0.8.0rc8/linien_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-05 09:24:09.000000 linien-client-0.8.0rc8/linien_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:24:09.000000 linien-client-0.8.0rc8/linien_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 09:24:09.000000 linien-client-0.8.0rc8/linien_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 09:24:09.000000 linien-client-0.8.0rc8/linien_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:24:09.254231 linien-client-0.8.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-05 09:23:25.000000 linien-client-0.8.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:53:07.928321 linien-client-0.8.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-05 12:53:07.928321 linien-client-0.8.0rc9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:53:07.928321 linien-client-0.8.0rc9/linien_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 12:52:27.000000 linien-client-0.8.0rc9/linien_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-05 12:52:27.000000 linien-client-0.8.0rc9/linien_client/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-05 12:52:27.000000 linien-client-0.8.0rc9/linien_client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-05 12:52:27.000000 linien-client-0.8.0rc9/linien_client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-05 12:52:27.000000 linien-client-0.8.0rc9/linien_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-05 12:52:27.000000 linien-client-0.8.0rc9/linien_client/remote_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:53:07.928321 linien-client-0.8.0rc9/linien_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-05 12:53:07.000000 linien-client-0.8.0rc9/linien_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-05 12:53:07.000000 linien-client-0.8.0rc9/linien_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:53:07.000000 linien-client-0.8.0rc9/linien_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 12:53:07.000000 linien-client-0.8.0rc9/linien_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 12:53:07.000000 linien-client-0.8.0rc9/linien_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:53:07.928321 linien-client-0.8.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-05 12:52:27.000000 linien-client-0.8.0rc9/setup.py
```

### Comparing `linien-client-0.8.0rc8/PKG-INFO` & `linien-client-0.8.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 0.8.0rc8
+Version: 0.8.0rc9
 Summary: Client components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien/
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-client-0.8.0rc8/linien_client/communication.py` & `linien-client-0.8.0rc9/linien_client/communication.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc8/linien_client/connection.py` & `linien-client-0.8.0rc9/linien_client/connection.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc8/linien_client/deploy.py` & `linien-client-0.8.0rc9/linien_client/deploy.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc8/linien_client/exceptions.py` & `linien-client-0.8.0rc9/linien_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc8/linien_client/remote_parameters.py` & `linien-client-0.8.0rc9/linien_client/remote_parameters.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc8/linien_client.egg-info/PKG-INFO` & `linien-client-0.8.0rc9/linien_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 0.8.0rc8
+Version: 0.8.0rc9
 Summary: Client components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien/
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-client-0.8.0rc8/setup.py` & `linien-client-0.8.0rc9/setup.py`

 * *Files 1% similar despite different names*

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
     name="linien-client",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
```

