# Comparing `tmp/git_remote_oracle-0.0.2.tar.gz` & `tmp/git_remote_oracle-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_remote_oracle-0.0.2.tar", last modified: Wed Jul  5 15:02:02 2023, max compression
+gzip compressed data, was "git_remote_oracle-0.0.3.tar", last modified: Thu Jul  6 16:53:04 2023, max compression
```

## Comparing `git_remote_oracle-0.0.2.tar` & `git_remote_oracle-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:02:02.713360 git_remote_oracle-0.0.2/
--rwxr-xr-x   0 root         (0) root         (0)     1066 2023-06-24 07:23:36.000000 git_remote_oracle-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-05 15:02:02.713360 git_remote_oracle-0.0.2/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      233 2023-07-02 09:48:14.000000 git_remote_oracle-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:02:02.713360 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)      764 2023-07-05 14:58:34.000000 git_remote_oracle-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 15:02:02.713360 git_remote_oracle-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:02:02.703360 git_remote_oracle-0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:02:02.713360 git_remote_oracle-0.0.2/src/git_remote_oracle/
--rwxr-xr-x   0 root         (0) root         (0)      113 2023-07-02 13:25:58.000000 git_remote_oracle-0.0.2/src/git_remote_oracle/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7868 2023-07-03 15:40:27.000000 git_remote_oracle-0.0.2/src/git_remote_oracle/git_remote_oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/
+-rwxr-xr-x   0 root         (0) root         (0)     1066 2023-06-24 07:23:36.000000 git_remote_oracle-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      233 2023-07-02 09:48:14.000000 git_remote_oracle-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 16:53:04.000000 git_remote_oracle-0.0.3/git_remote_oracle.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)      764 2023-07-06 16:41:24.000000 git_remote_oracle-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:53:04.062074 git_remote_oracle-0.0.3/src/git_remote_oracle/
+-rwxr-xr-x   0 root         (0) root         (0)      113 2023-07-02 13:25:58.000000 git_remote_oracle-0.0.3/src/git_remote_oracle/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7866 2023-07-06 16:39:42.000000 git_remote_oracle-0.0.3/src/git_remote_oracle/git_remote_oracle.py
```

### Comparing `git_remote_oracle-0.0.2/LICENSE` & `git_remote_oracle-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `git_remote_oracle-0.0.2/PKG-INFO` & `git_remote_oracle-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_remote_oracle
-Version: 0.0.2
+Version: 0.0.3
 Summary: A git remote helper to pull package source from oracle database.
 Author-email: CrazyT <crazyt2019+gro@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/git-remote-oracle
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/git-remote-oracle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `git_remote_oracle-0.0.2/git_remote_oracle.egg-info/PKG-INFO` & `git_remote_oracle-0.0.3/git_remote_oracle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-remote-oracle
-Version: 0.0.2
+Version: 0.0.3
 Summary: A git remote helper to pull package source from oracle database.
 Author-email: CrazyT <crazyt2019+gro@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/git-remote-oracle
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/git-remote-oracle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `git_remote_oracle-0.0.2/pyproject.toml` & `git_remote_oracle-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61"]
 
 [project]
 name = "git_remote_oracle"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="CrazyT", email="crazyt2019+gro@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `git_remote_oracle-0.0.2/src/git_remote_oracle/git_remote_oracle.py` & `git_remote_oracle-0.0.3/src/git_remote_oracle/git_remote_oracle.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
       AND last_ddl_time > :3
       AND generated = 'N'
       AND temporary = 'N'
       AND oracle_maintained = 'N'
     ORDER BY object_id
     """
   dbg(f"qry: {qry}")
-  for object_id, object_name, owner, object_type, ddl in cursor.execute(qry, [schema, username, last_ddl_time]):
+  for object_id, object_name, owner, object_type, ddl in cursor.execute(qry, [schema, schema, last_ddl_time]):
     #print(object_name)
     #print(ddl)
     ddl_str = ddl.read()
     dbg(f"object_name: {object_name}")
     print_fl(f"blob")
     print_fl(f"mark :{object_id}")
     print_fl(f"data {len(ddl_str)}")
```

