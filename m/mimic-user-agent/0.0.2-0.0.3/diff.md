# Comparing `tmp/mimic_user_agent-0.0.2.tar.gz` & `tmp/mimic_user_agent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimic_user_agent-0.0.2.tar", last modified: Thu Jul  6 17:31:58 2023, max compression
+gzip compressed data, was "mimic_user_agent-0.0.3.tar", last modified: Thu Jul  6 18:43:14 2023, max compression
```

## Comparing `mimic_user_agent-0.0.2.tar` & `mimic_user_agent-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-06 17:31:58.057201 mimic_user_agent-0.0.2/
--rw-r--r--   0 tomas     (1000) tomas     (1000)    35149 2023-07-06 17:10:37.000000 mimic_user_agent-0.0.2/LICENSE
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1082 2023-07-06 17:31:58.057201 mimic_user_agent-0.0.2/PKG-INFO
--rw-r--r--   0 tomas     (1000) tomas     (1000)      565 2023-07-06 17:27:28.000000 mimic_user_agent-0.0.2/README.md
--rw-r--r--   0 tomas     (1000) tomas     (1000)      503 2023-07-06 17:31:36.000000 mimic_user_agent-0.0.2/pyproject.toml
--rw-r--r--   0 tomas     (1000) tomas     (1000)       38 2023-07-06 17:31:58.057201 mimic_user_agent-0.0.2/setup.cfg
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-06 17:31:58.056200 mimic_user_agent-0.0.2/src/
--rw-r--r--   0 tomas     (1000) tomas     (1000)        0 2023-06-17 15:51:41.000000 mimic_user_agent-0.0.2/src/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2237 2023-07-06 16:57:00.000000 mimic_user_agent-0.0.2/src/mimicUserAgent.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-06 17:31:58.056200 mimic_user_agent-0.0.2/src/mimic_user_agent.egg-info/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1082 2023-07-06 17:31:58.000000 mimic_user_agent-0.0.2/src/mimic_user_agent.egg-info/PKG-INFO
--rw-r--r--   0 tomas     (1000) tomas     (1000)      275 2023-07-06 17:31:58.000000 mimic_user_agent-0.0.2/src/mimic_user_agent.egg-info/SOURCES.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2023-07-06 17:31:58.000000 mimic_user_agent-0.0.2/src/mimic_user_agent.egg-info/dependency_links.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       24 2023-07-06 17:31:58.000000 mimic_user_agent-0.0.2/src/mimic_user_agent.egg-info/top_level.txt
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-06 17:31:58.057201 mimic_user_agent-0.0.2/tests/
--rw-r--r--   0 tomas     (1000) tomas     (1000)      408 2023-07-06 16:58:20.000000 mimic_user_agent-0.0.2/tests/test_mimicUserAgent.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-06 18:43:14.069952 mimic_user_agent-0.0.3/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    35149 2023-07-06 17:10:37.000000 mimic_user_agent-0.0.3/LICENSE
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1082 2023-07-06 18:43:14.069952 mimic_user_agent-0.0.3/PKG-INFO
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      565 2023-07-06 17:27:28.000000 mimic_user_agent-0.0.3/README.md
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      591 2023-07-06 18:42:47.000000 mimic_user_agent-0.0.3/pyproject.toml
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       38 2023-07-06 18:43:14.069952 mimic_user_agent-0.0.3/setup.cfg
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-06 18:43:14.067952 mimic_user_agent-0.0.3/src/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        0 2023-06-17 15:51:41.000000 mimic_user_agent-0.0.3/src/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2237 2023-07-06 16:57:00.000000 mimic_user_agent-0.0.3/src/mimicUserAgent.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-06 18:43:14.068951 mimic_user_agent-0.0.3/src/mimic_user_agent.egg-info/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1082 2023-07-06 18:43:14.000000 mimic_user_agent-0.0.3/src/mimic_user_agent.egg-info/PKG-INFO
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      275 2023-07-06 18:43:14.000000 mimic_user_agent-0.0.3/src/mimic_user_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2023-07-06 18:43:14.000000 mimic_user_agent-0.0.3/src/mimic_user_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       24 2023-07-06 18:43:14.000000 mimic_user_agent-0.0.3/src/mimic_user_agent.egg-info/top_level.txt
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-06 18:43:14.068951 mimic_user_agent-0.0.3/tests/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      408 2023-07-06 16:58:20.000000 mimic_user_agent-0.0.3/tests/test_mimicUserAgent.py
```

### Comparing `mimic_user_agent-0.0.2/LICENSE` & `mimic_user_agent-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mimic_user_agent-0.0.2/PKG-INFO` & `mimic_user_agent-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimic_user_agent
-Version: 0.0.2
+Version: 0.0.3
 Summary: simple user-agent generator.
 Author-email: kurotom <author@example.com>
 Project-URL: Homepage, https://github.com/kurotom/mimic_user_agent
 Project-URL: Bug Tracker, https://github.com/kurotom/mimic_user_agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mimic_user_agent-0.0.2/README.md` & `mimic_user_agent-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mimic_user_agent-0.0.2/src/mimicUserAgent.py` & `mimic_user_agent-0.0.3/src/mimicUserAgent.py`

 * *Files identical despite different names*

### Comparing `mimic_user_agent-0.0.2/src/mimic_user_agent.egg-info/PKG-INFO` & `mimic_user_agent-0.0.3/src/mimic_user_agent.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimic-user-agent
-Version: 0.0.2
+Version: 0.0.3
 Summary: simple user-agent generator.
 Author-email: kurotom <author@example.com>
 Project-URL: Homepage, https://github.com/kurotom/mimic_user_agent
 Project-URL: Bug Tracker, https://github.com/kurotom/mimic_user_agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

