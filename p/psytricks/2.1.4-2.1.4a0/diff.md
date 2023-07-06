# Comparing `tmp/psytricks-2.1.4.tar.gz` & `tmp/psytricks-2.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psytricks-2.1.4.tar", max compression
+gzip compressed data, was "psytricks-2.1.4a0.tar", max compression
```

## Comparing `psytricks-2.1.4.tar` & `psytricks-2.1.4a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.4/LICENSE
--rw-r--r--   0        0        0     7868 2023-06-07 09:29:33.837553 psytricks-2.1.4/README.md
--rw-r--r--   0        0        0     1112 2023-07-06 10:58:41.583719 psytricks-2.1.4/pyproject.toml
--rw-r--r--   0        0        0       93 2023-07-06 10:58:41.583719 psytricks-2.1.4/src/psytricks/__init__.py
--rw-r--r--   0        0        0     6146 2023-07-06 10:58:41.583719 psytricks-2.1.4/src/psytricks/__ps1__/psytricks-lib.ps1
--rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.4/src/psytricks/__ps1__/psytricks-wrapper.ps1
--rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.4/src/psytricks/__ps1__/restricks-server.example.xml
--rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.4/src/psytricks/__ps1__/restricks-server.ps1
--rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.4/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
--rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.4/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
--rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.4/src/psytricks/__ps1__/sampledata/GetSessions.json
--rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.4/src/psytricks/cli.py
--rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.4/src/psytricks/decoder.py
--rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.4/src/psytricks/literals.py
--rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.4/src/psytricks/mappings.py
--rw-r--r--   0        0        0    24278 2023-07-06 10:55:44.342051 psytricks-2.1.4/src/psytricks/wrapper.py
--rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 psytricks-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.4a0/LICENSE
+-rw-r--r--   0        0        0     7868 2023-06-07 09:29:33.837553 psytricks-2.1.4a0/README.md
+-rw-r--r--   0        0        0     1116 2023-06-14 14:00:52.880002 psytricks-2.1.4a0/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-06-14 14:00:52.880002 psytricks-2.1.4a0/src/psytricks/__init__.py
+-rw-r--r--   0        0        0     6150 2023-06-14 14:00:52.884002 psytricks-2.1.4a0/src/psytricks/__ps1__/psytricks-lib.ps1
+-rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/__ps1__/psytricks-wrapper.ps1
+-rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/__ps1__/restricks-server.example.xml
+-rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.4a0/src/psytricks/__ps1__/restricks-server.ps1
+-rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
+-rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
+-rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetSessions.json
+-rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.4a0/src/psytricks/cli.py
+-rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.4a0/src/psytricks/decoder.py
+-rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.4a0/src/psytricks/literals.py
+-rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.4a0/src/psytricks/mappings.py
+-rw-r--r--   0        0        0    24280 2023-06-14 13:59:13.038825 psytricks-2.1.4a0/src/psytricks/wrapper.py
+-rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 psytricks-2.1.4a0/PKG-INFO
```

### Comparing `psytricks-2.1.4/LICENSE` & `psytricks-2.1.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/README.md` & `psytricks-2.1.4a0/README.md`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/pyproject.toml` & `psytricks-2.1.4a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>"]
 description = "PowerShell Python Citrix Tricks."
 documentation = "https://imcf.one/apidocs/psytricks/psytricks.html"
 license = "GPL-3.0-or-later"
 name = "psytricks"
 readme = "README.md"
-version = "2.1.4"
+version = "2.1.4-a.0"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/imcf/psytricks/blob/main/CHANGELOG.md"
 "Organisation Homepage" = "https://imcf.one/"
 "Twitter" = "https://twitter.com/imcf_basel"
 
 [tool.poetry.dependencies]
```

### Comparing `psytricks-2.1.4/src/psytricks/__ps1__/psytricks-lib.ps1` & `psytricks-2.1.4a0/src/psytricks/__ps1__/psytricks-lib.ps1`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <#
 
 Collection of functions and other definitions to be sourced by other scripts.
 
 #>
 
 # the version variable will be filled by poetry at build time:
-$Version = "2.1.4"
+$Version = "2.1.4-a.0"
 
 
 #region properties-selectors
 
 $MachineProperties = @(
     "AgentVersion",
     "AssociatedUserUPNs",
```

### Comparing `psytricks-2.1.4/src/psytricks/__ps1__/psytricks-wrapper.ps1` & `psytricks-2.1.4a0/src/psytricks/__ps1__/psytricks-wrapper.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/src/psytricks/__ps1__/restricks-server.example.xml` & `psytricks-2.1.4a0/src/psytricks/__ps1__/restricks-server.example.xml`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/src/psytricks/__ps1__/restricks-server.ps1` & `psytricks-2.1.4a0/src/psytricks/__ps1__/restricks-server.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/src/psytricks/__ps1__/sampledata/GetAccessUsers.json` & `psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/src/psytricks/__ps1__/sampledata/GetMachineStatus.json` & `psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/src/psytricks/__ps1__/sampledata/GetSessions.json` & `psytricks-2.1.4a0/src/psytricks/__ps1__/sampledata/GetSessions.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/src/psytricks/cli.py` & `psytricks-2.1.4a0/src/psytricks/cli.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/src/psytricks/decoder.py` & `psytricks-2.1.4a0/src/psytricks/decoder.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/src/psytricks/literals.py` & `psytricks-2.1.4a0/src/psytricks/literals.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/src/psytricks/mappings.py` & `psytricks-2.1.4a0/src/psytricks/mappings.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.4/src/psytricks/wrapper.py` & `psytricks-2.1.4a0/src/psytricks/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,16 +373,16 @@
     def validate_version(self, server_ver):
         """Validate the server version against the local module.
 
         Parse the version strings of the local module and the server response
         and compare them for equality (ignoring the 4th component, which may
         denote a pre- or development-release).
 
-        If the 3rd component (PATCH level) is differing a message will be issued
-        to the debug log but the method will still return True.
+        If the 3rd component (PATCH level) is differing a warning message will
+        be issued to the log but the method will still return True.
 
         Parameters
         ----------
         server_ver : dict
             The dict parsed from the JSON response when sending a `version` GET
             request to the server.
```

### Comparing `psytricks-2.1.4/PKG-INFO` & `psytricks-2.1.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psytricks
-Version: 2.1.4
+Version: 2.1.4a0
 Summary: PowerShell Python Citrix Tricks.
 License: GPL-3.0-or-later
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

