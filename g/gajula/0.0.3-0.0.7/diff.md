# Comparing `tmp/gajula-0.0.3.tar.gz` & `tmp/gajula-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gajula-0.0.3.tar", last modified: Wed Jul  5 09:16:59 2023, max compression
+gzip compressed data, was "gajula-0.0.7.tar", last modified: Wed Jul  5 10:07:23 2023, max compression
```

## Comparing `gajula-0.0.3.tar` & `gajula-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 09:16:59.781710 gajula-0.0.3/
--rw-rw-rw-   0        0        0     1096 2023-07-05 07:25:55.000000 gajula-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      474 2023-07-05 09:16:59.780710 gajula-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-05 09:16:59.760711 gajula-0.0.3/gajula/
-drwxrwxrwx   0        0        0        0 2023-07-05 09:16:59.778709 gajula-0.0.3/gajula/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 09:16:59.776735 gajula-0.0.3/gajula/src/gajula.egg-info/
--rw-rw-rw-   0        0        0      474 2023-07-05 09:16:59.000000 gajula-0.0.3/gajula/src/gajula.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-07-05 09:16:59.000000 gajula-0.0.3/gajula/src/gajula.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 09:16:59.000000 gajula-0.0.3/gajula/src/gajula.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-05 09:16:59.000000 gajula-0.0.3/gajula/src/gajula.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2718 2023-07-05 09:15:11.000000 gajula-0.0.3/gajula/src/gajula.py
--rw-rw-rw-   0        0        0       42 2023-07-05 09:16:59.782712 gajula-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1314 2023-07-05 09:16:53.000000 gajula-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:23.874891 gajula-0.0.7/
+-rw-rw-rw-   0        0        0     1096 2023-07-05 07:25:55.000000 gajula-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      474 2023-07-05 10:07:23.872892 gajula-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:23.851895 gajula-0.0.7/gajula/
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:23.869893 gajula-0.0.7/gajula/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 10:07:23.866892 gajula-0.0.7/gajula/src/gajula.egg-info/
+-rw-rw-rw-   0        0        0      474 2023-07-05 10:07:23.000000 gajula-0.0.7/gajula/src/gajula.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-07-05 10:07:23.000000 gajula-0.0.7/gajula/src/gajula.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 10:07:23.000000 gajula-0.0.7/gajula/src/gajula.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 10:07:23.000000 gajula-0.0.7/gajula/src/gajula.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2873 2023-07-05 09:25:20.000000 gajula-0.0.7/gajula/src/gajula.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 10:07:23.874891 gajula-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1519 2023-07-05 10:06:54.000000 gajula-0.0.7/setup.py
```

### Comparing `gajula-0.0.3/LICENSE` & `gajula-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gajula-0.0.3/gajula/src/gajula.py` & `gajula-0.0.7/gajula/src/gajula.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,34 +15,36 @@
     def time_now(self,timezone='Universal',format='default'):
         '''
         returns time in desired timezone in desired format. 
         '''
         if timezone not in self.all_timezones:
             raise ValueError("Time zone is not valid")
         if format == 'object':
-            return datetime.now(pytz.timezone('timezone'))
+            return datetime.now(pytz.timezone(timezone))
         if format == 'unix':
-            dt =  datetime.now(pytz.timezone('timezone'))
+            dt =  datetime.now(pytz.timezone(timezone))
             return int( time.mktime(dt.timetuple()) )
         if format == 'default':
-            return datetime.now(pytz.timezone('timezone')).strftime('%Y-%m-%d %H:%M:%S')
+            return datetime.now(pytz.timezone(timezone)).strftime('%Y-%m-%d %H:%M:%S')
         else:
-            return datetime.now(pytz.timezone('timezone')).strftime(format)
+            return datetime.now(pytz.timezone(timezone)).strftime(format)
 
-    def utc_now(self,type='datetime'):
+    def utc_now(self,format='datetime'):
         '''
         returns UTC time now
         types = datetime, unix
         '''
-        if type=='datetime':
+        if format not in ['datetime','default','unix']:
+            return datetime.utcnow().strftime(format)
+        if format =='datetime':
             return datetime.utcnow()
-        if type=='unix':
+        if format =='default':
+            return datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')
+        if format =='unix':
             return int( time.mktime(datetime.utcnow().timetuple()) )
-        else:
-            return "Unknown type passed"
     
     def random_date(self,future=True)->datetime:
         '''
         returns a random date and time in the next 365 days. 
         future is true if passed false will give random date and time in past. 
         '''
         r_days = random.randint(0,7)
```

### Comparing `gajula-0.0.3/setup.py` & `gajula-0.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import setuptools
+import pickle
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+version = open('version', 'rb')
+ver = pickle.load(version)
+version.close()
+
+
+version = open('version', 'wb')
+pickle.dump(ver + 1,version)                     
+version.close()
+
 setuptools.setup(
     name="gajula",                     # This is the name of the package
-    version="0.0.3",                        # The initial release version
+    version=f"0.0.{ver}",                        # The initial release version
     author="Jagadeesh Gajula",                     # Full name of the author
     description="Gajula Package consists of useful utilites and functions",
     long_description="Gajula Package is developed for public use, it contains generic functions and utilities",      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

