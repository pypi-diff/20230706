# Comparing `tmp/ldst_monitor-1.0.2.tar.gz` & `tmp/ldst_monitor-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldst_monitor-1.0.2.tar", last modified: Thu Jul  6 15:50:29 2023, max compression
+gzip compressed data, was "ldst_monitor-1.0.3.tar", last modified: Thu Jul  6 16:01:48 2023, max compression
```

## Comparing `ldst_monitor-1.0.2.tar` & `ldst_monitor-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 15:50:29.983492 ldst_monitor-1.0.2/
--rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-06 15:50:29.983050 ldst_monitor-1.0.2/PKG-INFO
--rwxrwxrwx   0 happy     (1000) happy     (1000)      435 2023-07-06 15:48:55.000000 ldst_monitor-1.0.2/pyproject.toml
--rwxrwxrwx   0 happy     (1000) happy     (1000)       38 2023-07-06 15:50:29.983645 ldst_monitor-1.0.2/setup.cfg
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 15:50:29.969088 ldst_monitor-1.0.2/src/
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 15:50:29.975538 ldst_monitor-1.0.2/src/ldst_monitor/
--rwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 14:33:12.000000 ldst_monitor-1.0.2/src/ldst_monitor/__init__.py
--rwxrwxrwx   0 happy     (1000) happy     (1000)     1321 2023-07-06 14:55:29.000000 ldst_monitor-1.0.2/src/ldst_monitor/ding.py
--rwxrwxrwx   0 happy     (1000) happy     (1000)      987 2023-07-06 14:55:51.000000 ldst_monitor-1.0.2/src/ldst_monitor/main.py
--rwxrwxrwx   0 happy     (1000) happy     (1000)     2657 2023-07-06 11:55:20.000000 ldst_monitor-1.0.2/src/ldst_monitor/monitor.py
-drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 15:50:29.981454 ldst_monitor-1.0.2/src/ldst_monitor.egg-info/
--rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-06 15:50:29.000000 ldst_monitor-1.0.2/src/ldst_monitor.egg-info/PKG-INFO
--rwxrwxrwx   0 happy     (1000) happy     (1000)      281 2023-07-06 15:50:29.000000 ldst_monitor-1.0.2/src/ldst_monitor.egg-info/SOURCES.txt
--rwxrwxrwx   0 happy     (1000) happy     (1000)        1 2023-07-06 15:50:29.000000 ldst_monitor-1.0.2/src/ldst_monitor.egg-info/dependency_links.txt
--rwxrwxrwx   0 happy     (1000) happy     (1000)       13 2023-07-06 15:50:29.000000 ldst_monitor-1.0.2/src/ldst_monitor.egg-info/top_level.txt
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 16:01:48.685607 ldst_monitor-1.0.3/
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-06 16:01:48.685191 ldst_monitor-1.0.3/PKG-INFO
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      438 2023-07-06 16:01:30.000000 ldst_monitor-1.0.3/pyproject.toml
+-rwxrwxrwx   0 happy     (1000) happy     (1000)       38 2023-07-06 16:01:48.685754 ldst_monitor-1.0.3/setup.cfg
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 16:01:48.672563 ldst_monitor-1.0.3/src/
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 16:01:48.679158 ldst_monitor-1.0.3/src/ldst_monitor/
+-rwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 14:33:12.000000 ldst_monitor-1.0.3/src/ldst_monitor/__init__.py
+-rwxrwxrwx   0 happy     (1000) happy     (1000)     1321 2023-07-06 14:55:29.000000 ldst_monitor-1.0.3/src/ldst_monitor/ding.py
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      987 2023-07-06 14:55:51.000000 ldst_monitor-1.0.3/src/ldst_monitor/main.py
+-rwxrwxrwx   0 happy     (1000) happy     (1000)     2653 2023-07-06 16:01:17.000000 ldst_monitor-1.0.3/src/ldst_monitor/monitor.py
+drwxrwxrwx   0 happy     (1000) happy     (1000)        0 2023-07-06 16:01:48.683975 ldst_monitor-1.0.3/src/ldst_monitor.egg-info/
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      339 2023-07-06 16:01:48.000000 ldst_monitor-1.0.3/src/ldst_monitor.egg-info/PKG-INFO
+-rwxrwxrwx   0 happy     (1000) happy     (1000)      281 2023-07-06 16:01:48.000000 ldst_monitor-1.0.3/src/ldst_monitor.egg-info/SOURCES.txt
+-rwxrwxrwx   0 happy     (1000) happy     (1000)        1 2023-07-06 16:01:48.000000 ldst_monitor-1.0.3/src/ldst_monitor.egg-info/dependency_links.txt
+-rwxrwxrwx   0 happy     (1000) happy     (1000)       13 2023-07-06 16:01:48.000000 ldst_monitor-1.0.3/src/ldst_monitor.egg-info/top_level.txt
```

### Comparing `ldst_monitor-1.0.2/src/ldst_monitor/ding.py` & `ldst_monitor-1.0.3/src/ldst_monitor/ding.py`

 * *Files identical despite different names*

### Comparing `ldst_monitor-1.0.2/src/ldst_monitor/main.py` & `ldst_monitor-1.0.3/src/ldst_monitor/main.py`

 * *Files identical despite different names*

### Comparing `ldst_monitor-1.0.2/src/ldst_monitor/monitor.py` & `ldst_monitor-1.0.3/src/ldst_monitor/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
             self.status.update({"mysql": True})
 
     def nginx(self):
         nginx_shell = '/etc/init.d/nginx'
         process = subprocess.run([nginx_shell, "status"], capture_output=True)
         if process.stdout.decode("utf8").find("running") == -1:
             self.status.update({"nginx": False})
-            # process = subprocess.run([nginx_shell, 'start'])
-            # print(process.stdout)
+            process = subprocess.run([nginx_shell, 'start'])
+            print(process.stdout)
         else:
             self.status.update({"nginx": True})
 
     def memcached(self):
         process = subprocess.run(["pgrep", "-x", "memcached"], capture_output=True)
         if process.returncode != 0:
             self.status.update({"memcached": False})
```

