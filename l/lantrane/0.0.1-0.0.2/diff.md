# Comparing `tmp/lantrane-0.0.1.tar.gz` & `tmp/lantrane-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lantrane-0.0.1.tar", last modified: Sun Jul  2 00:00:36 2023, max compression
+gzip compressed data, was "lantrane-0.0.2.tar", last modified: Thu Jul  6 02:54:26 2023, max compression
```

## Comparing `lantrane-0.0.1.tar` & `lantrane-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-02 00:00:36.057294 lantrane-0.0.1/
--rw-rw-r--   0 ace       (1000) ace       (1000)    35149 2023-07-01 23:09:40.000000 lantrane-0.0.1/LICENSE.md
--rw-rw-r--   0 ace       (1000) ace       (1000)     1137 2023-07-02 00:00:36.057294 lantrane-0.0.1/PKG-INFO
--rw-rw-r--   0 ace       (1000) ace       (1000)      682 2023-07-01 23:59:44.000000 lantrane-0.0.1/README.md
-drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-02 00:00:36.057294 lantrane-0.0.1/lantrane/
--rw-rw-r--   0 ace       (1000) ace       (1000)       60 2023-07-01 23:54:37.000000 lantrane-0.0.1/lantrane/__init__.py
--rw-rw-r--   0 ace       (1000) ace       (1000)      911 2023-07-01 23:22:02.000000 lantrane-0.0.1/lantrane/data.py
--rw-rw-r--   0 ace       (1000) ace       (1000)      567 2023-07-01 23:54:27.000000 lantrane-0.0.1/lantrane/lantrane.py
-drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-02 00:00:36.057294 lantrane-0.0.1/lantrane.egg-info/
--rw-rw-r--   0 ace       (1000) ace       (1000)     1137 2023-07-02 00:00:35.000000 lantrane-0.0.1/lantrane.egg-info/PKG-INFO
--rw-rw-r--   0 ace       (1000) ace       (1000)      216 2023-07-02 00:00:35.000000 lantrane-0.0.1/lantrane.egg-info/SOURCES.txt
--rw-rw-r--   0 ace       (1000) ace       (1000)        1 2023-07-02 00:00:35.000000 lantrane-0.0.1/lantrane.egg-info/dependency_links.txt
--rw-rw-r--   0 ace       (1000) ace       (1000)        9 2023-07-02 00:00:35.000000 lantrane-0.0.1/lantrane.egg-info/top_level.txt
--rw-rw-r--   0 ace       (1000) ace       (1000)       38 2023-07-02 00:00:36.057294 lantrane-0.0.1/setup.cfg
--rw-rw-r--   0 ace       (1000) ace       (1000)     1488 2023-07-01 23:45:52.000000 lantrane-0.0.1/setup.py
+drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-06 02:54:26.313043 lantrane-0.0.2/
+-rw-rw-r--   0 ace       (1000) ace       (1000)    35149 2023-07-01 23:09:40.000000 lantrane-0.0.2/LICENSE.md
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1127 2023-07-06 02:54:26.313043 lantrane-0.0.2/PKG-INFO
+-rw-rw-r--   0 ace       (1000) ace       (1000)      672 2023-07-06 01:14:46.000000 lantrane-0.0.2/README.md
+drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-06 02:54:26.313043 lantrane-0.0.2/lantrane/
+-rw-rw-r--   0 ace       (1000) ace       (1000)       60 2023-07-01 23:54:37.000000 lantrane-0.0.2/lantrane/__init__.py
+-rw-rw-r--   0 ace       (1000) ace       (1000)      911 2023-07-01 23:22:02.000000 lantrane-0.0.2/lantrane/data.py
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1218 2023-07-06 02:53:39.000000 lantrane-0.0.2/lantrane/lantrane.py
+drwxrwxr-x   0 ace       (1000) ace       (1000)        0 2023-07-06 02:54:26.313043 lantrane-0.0.2/lantrane.egg-info/
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1127 2023-07-06 02:54:26.000000 lantrane-0.0.2/lantrane.egg-info/PKG-INFO
+-rw-rw-r--   0 ace       (1000) ace       (1000)      216 2023-07-06 02:54:26.000000 lantrane-0.0.2/lantrane.egg-info/SOURCES.txt
+-rw-rw-r--   0 ace       (1000) ace       (1000)        1 2023-07-06 02:54:26.000000 lantrane-0.0.2/lantrane.egg-info/dependency_links.txt
+-rw-rw-r--   0 ace       (1000) ace       (1000)        9 2023-07-06 02:54:26.000000 lantrane-0.0.2/lantrane.egg-info/top_level.txt
+-rw-rw-r--   0 ace       (1000) ace       (1000)       38 2023-07-06 02:54:26.313043 lantrane-0.0.2/setup.cfg
+-rw-rw-r--   0 ace       (1000) ace       (1000)     1488 2023-07-06 02:54:10.000000 lantrane-0.0.2/setup.py
```

### Comparing `lantrane-0.0.1/LICENSE.md` & `lantrane-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lantrane-0.0.1/PKG-INFO` & `lantrane-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lantrane
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for interacting with Trane thermostats locally.
 Home-page: https://github.com/MoralCode/lantrane
 Author: Adrian Edwards
 Author-email: adrian@adriancedwards.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 
 ## Usage Example
 Your thermostat for communicating, variable speed heat pump systems might have a port open that emits data every time the compressor speed changes if you can find the right port via nmap and telnet (usually port 30,000 or so), this example will listen on that port and give you data. The port may change when the device is updated though.
 
 ```python
 from lantrane import Trane
 
-for data in Trane().listen(host=args.ip, port=args.port):
+for data in Trane(args.ip, args.port).listen():
 	print(data)
 
 ```
 
 
 
 ## Distribution
```

### Comparing `lantrane-0.0.1/README.md` & `lantrane-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ## Usage Example
 Your thermostat for communicating, variable speed heat pump systems might have a port open that emits data every time the compressor speed changes if you can find the right port via nmap and telnet (usually port 30,000 or so), this example will listen on that port and give you data. The port may change when the device is updated though.
 
 ```python
 from lantrane import Trane
 
-for data in Trane().listen(host=args.ip, port=args.port):
+for data in Trane(args.ip, args.port).listen():
 	print(data)
 
 ```
 
 
 
 ## Distribution
```

### Comparing `lantrane-0.0.1/lantrane/data.py` & `lantrane-0.0.2/lantrane/data.py`

 * *Files identical despite different names*

### Comparing `lantrane-0.0.1/lantrane.egg-info/PKG-INFO` & `lantrane-0.0.2/lantrane.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lantrane
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for interacting with Trane thermostats locally.
 Home-page: https://github.com/MoralCode/lantrane
 Author: Adrian Edwards
 Author-email: adrian@adriancedwards.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 
 ## Usage Example
 Your thermostat for communicating, variable speed heat pump systems might have a port open that emits data every time the compressor speed changes if you can find the right port via nmap and telnet (usually port 30,000 or so), this example will listen on that port and give you data. The port may change when the device is updated though.
 
 ```python
 from lantrane import Trane
 
-for data in Trane().listen(host=args.ip, port=args.port):
+for data in Trane(args.ip, args.port).listen():
 	print(data)
 
 ```
 
 
 
 ## Distribution
```

### Comparing `lantrane-0.0.1/setup.py` & `lantrane-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Configurations
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=[],      								  # Dependencies
      python_requires='>=3',                                   # Minimum Python version
      name='lantrane',                                  # Package name
-     version="0.0.1",                                     # Version
+     version="0.0.2",                                     # Version
      author="Adrian Edwards",                                 # Author name
      author_email="adrian@adriancedwards.com",                           # Author mail
      description="Python package for interacting with Trane thermostats locally.",    # Short package description
      long_description=long_description,                       # Long package description
      long_description_content_type="text/markdown",
      url="https://github.com/MoralCode/lantrane",       # Url to your Git Repo
     #  download_url = 'https://github.com/MoralCode/lantrane/archive/'+new_version+'.tar.gz',
```

