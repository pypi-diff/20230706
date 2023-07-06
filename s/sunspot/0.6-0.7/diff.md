# Comparing `tmp/sunspot-0.6.tar.gz` & `tmp/sunspot-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunspot-0.6.tar", last modified: Mon Jun 26 12:10:47 2023, max compression
+gzip compressed data, was "sunspot-0.7.tar", last modified: Thu Jul  6 02:23:25 2023, max compression
```

## Comparing `sunspot-0.6.tar` & `sunspot-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-26 12:10:47.769705 sunspot-0.6/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12028 2023-06-26 12:10:47.769430 sunspot-0.6/PKG-INFO
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    10997 2023-06-25 19:24:10.000000 sunspot-0.6/README.md
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     1104 2023-06-26 12:10:32.000000 sunspot-0.6/pyproject.toml
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       38 2023-06-26 12:10:47.769750 sunspot-0.6/setup.cfg
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-26 12:10:47.768523 sunspot-0.6/src/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      868 2023-06-22 01:07:07.000000 sunspot-0.6/src/foobar.py
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-26 12:10:47.769247 sunspot-0.6/src/sunspot.egg-info/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12028 2023-06-26 12:10:47.000000 sunspot-0.6/src/sunspot.egg-info/PKG-INFO
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      205 2023-06-26 12:10:47.000000 sunspot-0.6/src/sunspot.egg-info/SOURCES.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)        1 2023-06-26 12:10:47.000000 sunspot-0.6/src/sunspot.egg-info/dependency_links.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       20 2023-06-26 12:10:47.000000 sunspot-0.6/src/sunspot.egg-info/top_level.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    18189 2023-06-25 15:03:29.000000 sunspot-0.6/src/sunspot.py
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     8456 2023-06-25 00:40:27.000000 sunspot-0.6/src/test.py
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-07-06 02:23:25.819115 sunspot-0.7/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12021 2023-07-06 02:23:25.818938 sunspot-0.7/PKG-INFO
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    10990 2023-07-05 02:45:39.000000 sunspot-0.7/README.md
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     1104 2023-07-06 02:23:06.000000 sunspot-0.7/pyproject.toml
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       38 2023-07-06 02:23:25.819151 sunspot-0.7/setup.cfg
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-07-06 02:23:25.818248 sunspot-0.7/src/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      921 2023-07-06 02:13:09.000000 sunspot-0.7/src/foobar.py
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-07-06 02:23:25.818771 sunspot-0.7/src/sunspot.egg-info/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12021 2023-07-06 02:23:25.000000 sunspot-0.7/src/sunspot.egg-info/PKG-INFO
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      205 2023-07-06 02:23:25.000000 sunspot-0.7/src/sunspot.egg-info/SOURCES.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)        1 2023-07-06 02:23:25.000000 sunspot-0.7/src/sunspot.egg-info/dependency_links.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       20 2023-07-06 02:23:25.000000 sunspot-0.7/src/sunspot.egg-info/top_level.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    18364 2023-07-06 02:18:43.000000 sunspot-0.7/src/sunspot.py
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     8456 2023-06-25 00:40:27.000000 sunspot-0.7/src/test.py
```

### Comparing `sunspot-0.6/PKG-INFO` & `sunspot-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunspot
-Version: 0.6
+Version: 0.7
 Summary: Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any Target Body available through the JPL Horizons App. Also provides real-time tracking of those data for the duration of an ephemeris.
 Author-email: Phillip Curtsmith <phillip.curtsmith@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/sunspot/
 Project-URL: Bug Tracker, https://github.com/phillipcurtsmith/sunspot-issues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -46,15 +46,15 @@
 >>> titles
 ['Date__(UT)__HR:MN:SS', 'Azimuth_(a-app)', 'Elevation_(a-app)']
 ```
 And one can simply view a list of those data:
 ```python
 >>> azimuth = titles[1]
 >>> e.get_ephemeris_data( azimuth )
-['252.781222419', '253.019121568', ... , '252.896492970', '253.133817632']]
+['252.781222419', '253.019121568', ... , '252.896492970', '253.133817632']
 ```
 For each data point in every list, there is a corresponding time stamp. One can use the convenience method to view the time stamps:
 ```python
 >>> e.dates()
 ['2023-06-18 19:26:00', '2023-06-18 19:27:00', ... , '2023-06-21 19:27:00', '2023-06-21 19:28:00']
 ```
 Each list is always in chronological order such that the nth ````azimuth```` entry corresponds to the nth ````e.dates()```` entry.
@@ -95,15 +95,15 @@
     ...
 
 def after( args: list ):
     # method executes after Ephemeris entry, 
     # e.g., do 'clean-up' stuff here
     ...
 ```
-User-defined functions **must** accept a list of strings. This list corresponds to the _Observer Quantities_ for a given Ephemeris entry. For the example Ephemeris above, Tracker methods will be called with a list of two strings, where the first string is ```'Azimuth_(a-app)'``` and the second is ```'Elevation_(a-app)'```. The order of the arguments in the list are the same order as ````e.DATA_TITLES````.
+User-defined functions **must** accept a list of strings. This list corresponds to the _Observer Quantities_ for a given Ephemeris entry. For the example Ephemeris above, Tracker methods will be called with a list of three strings: ```'Date__(UT)__HR:MN:SS'```,  ```'Azimuth_(a-app)'```, and ```'Elevation_(a-app)'```. The order of the arguments in the list are the same order as ````e.DATA_TITLES````.
 
 Tracker has a simple constructor to begin tracking:
 
 ```python
 >>> t = sunspot.Tracker(    e,                                  # an Ephemeris object
                             track_before_method = before,       # user-generated method runs BEFORE Ephemeris event
                             track_on_time_method = on_time,     # user-generated method runs AT Ephemeris event
```

### Comparing `sunspot-0.6/README.md` & `sunspot-0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 >>> titles
 ['Date__(UT)__HR:MN:SS', 'Azimuth_(a-app)', 'Elevation_(a-app)']
 ```
 And one can simply view a list of those data:
 ```python
 >>> azimuth = titles[1]
 >>> e.get_ephemeris_data( azimuth )
-['252.781222419', '253.019121568', ... , '252.896492970', '253.133817632']]
+['252.781222419', '253.019121568', ... , '252.896492970', '253.133817632']
 ```
 For each data point in every list, there is a corresponding time stamp. One can use the convenience method to view the time stamps:
 ```python
 >>> e.dates()
 ['2023-06-18 19:26:00', '2023-06-18 19:27:00', ... , '2023-06-21 19:27:00', '2023-06-21 19:28:00']
 ```
 Each list is always in chronological order such that the nth ````azimuth```` entry corresponds to the nth ````e.dates()```` entry.
@@ -77,15 +77,15 @@
     ...
 
 def after( args: list ):
     # method executes after Ephemeris entry, 
     # e.g., do 'clean-up' stuff here
     ...
 ```
-User-defined functions **must** accept a list of strings. This list corresponds to the _Observer Quantities_ for a given Ephemeris entry. For the example Ephemeris above, Tracker methods will be called with a list of two strings, where the first string is ```'Azimuth_(a-app)'``` and the second is ```'Elevation_(a-app)'```. The order of the arguments in the list are the same order as ````e.DATA_TITLES````.
+User-defined functions **must** accept a list of strings. This list corresponds to the _Observer Quantities_ for a given Ephemeris entry. For the example Ephemeris above, Tracker methods will be called with a list of three strings: ```'Date__(UT)__HR:MN:SS'```,  ```'Azimuth_(a-app)'```, and ```'Elevation_(a-app)'```. The order of the arguments in the list are the same order as ````e.DATA_TITLES````.
 
 Tracker has a simple constructor to begin tracking:
 
 ```python
 >>> t = sunspot.Tracker(    e,                                  # an Ephemeris object
                             track_before_method = before,       # user-generated method runs BEFORE Ephemeris event
                             track_on_time_method = on_time,     # user-generated method runs AT Ephemeris event
```

### Comparing `sunspot-0.6/pyproject.toml` & `sunspot-0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sunspot"
-version = "0.6"
+version = "0.7"
 description = "Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any Target Body available through the JPL Horizons App. Also provides real-time tracking of those data for the duration of an ephemeris."
 readme = "README.md"
 authors = [{ name = "Phillip Curtsmith", email = "phillip.curtsmith@gmail.com" }]
 dependencies = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `sunspot-0.6/src/sunspot.egg-info/PKG-INFO` & `sunspot-0.7/src/sunspot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunspot
-Version: 0.6
+Version: 0.7
 Summary: Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any Target Body available through the JPL Horizons App. Also provides real-time tracking of those data for the duration of an ephemeris.
 Author-email: Phillip Curtsmith <phillip.curtsmith@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/sunspot/
 Project-URL: Bug Tracker, https://github.com/phillipcurtsmith/sunspot-issues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -46,15 +46,15 @@
 >>> titles
 ['Date__(UT)__HR:MN:SS', 'Azimuth_(a-app)', 'Elevation_(a-app)']
 ```
 And one can simply view a list of those data:
 ```python
 >>> azimuth = titles[1]
 >>> e.get_ephemeris_data( azimuth )
-['252.781222419', '253.019121568', ... , '252.896492970', '253.133817632']]
+['252.781222419', '253.019121568', ... , '252.896492970', '253.133817632']
 ```
 For each data point in every list, there is a corresponding time stamp. One can use the convenience method to view the time stamps:
 ```python
 >>> e.dates()
 ['2023-06-18 19:26:00', '2023-06-18 19:27:00', ... , '2023-06-21 19:27:00', '2023-06-21 19:28:00']
 ```
 Each list is always in chronological order such that the nth ````azimuth```` entry corresponds to the nth ````e.dates()```` entry.
@@ -95,15 +95,15 @@
     ...
 
 def after( args: list ):
     # method executes after Ephemeris entry, 
     # e.g., do 'clean-up' stuff here
     ...
 ```
-User-defined functions **must** accept a list of strings. This list corresponds to the _Observer Quantities_ for a given Ephemeris entry. For the example Ephemeris above, Tracker methods will be called with a list of two strings, where the first string is ```'Azimuth_(a-app)'``` and the second is ```'Elevation_(a-app)'```. The order of the arguments in the list are the same order as ````e.DATA_TITLES````.
+User-defined functions **must** accept a list of strings. This list corresponds to the _Observer Quantities_ for a given Ephemeris entry. For the example Ephemeris above, Tracker methods will be called with a list of three strings: ```'Date__(UT)__HR:MN:SS'```,  ```'Azimuth_(a-app)'```, and ```'Elevation_(a-app)'```. The order of the arguments in the list are the same order as ````e.DATA_TITLES````.
 
 Tracker has a simple constructor to begin tracking:
 
 ```python
 >>> t = sunspot.Tracker(    e,                                  # an Ephemeris object
                             track_before_method = before,       # user-generated method runs BEFORE Ephemeris event
                             track_on_time_method = on_time,     # user-generated method runs AT Ephemeris event
```

### Comparing `sunspot-0.6/src/sunspot.py` & `sunspot-0.7/src/sunspot.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         """
         Terminate tracking for a current Tracker object.
         :return: None
         """
         self.exit_event_trigger.set()
 
     def user_cancelled_tracking( self ) -> bool:
-        if not self.exit_event_trigger:
+        if self.exit_event_trigger.is_set():
             if self.verbose:
                 print( "SUNSPOT#TRACKER: Tracking cancelled by user." )
             return True
         return False
 
     def track( self, before_method, on_time_method, after_method, starting_index ):
         from datetime import datetime
@@ -210,23 +210,25 @@
         dates = e.dates()
         for i in dates:
             if datetime.now().timestamp() < datetime.strptime( i, DATA_FORMAT ).timestamp():
                 return dates.index( i )
         return None
 
 
-def sleep_time( future ) -> float:
+def sleep_time( future, verbose ) -> float:
     """
     :return: The difference, in seconds, between the moment this function is called and the (future) datetime passed as argument.
     If return value is negative (e.g., an event presumed to be in the future is actually in the past), throws exception.
     """
     from datetime import datetime
+    if verbose:
+        print( "SUNSPOT#TRACKER: Delay event initiated at [" + f'{datetime.now():%Y-%m-%d %H:%M:%S%z}' + "] for future time [" + future + "]." )
     delay = datetime.strptime( future, DATA_FORMAT ).timestamp() - datetime.now().timestamp()
     if delay < 0:
-        raise SystemError( "Tracker timing error: attempting to track object at time [" + future + "] indicates this time has already passed. Possibly the result of a long-running user process delaying thread execution." )
+        raise SystemError( "Tracker timing error. attempting to track object at time [" + future + "] indicates this time has already passed. Possibly the result of a long-running user process delaying thread execution." )
     return delay
 
 
 def convert_numeric_month( r ) -> str:
     return r.replace( "Jan", "01" ).replace( "Feb", "02" ).replace( "Mar", "03" ).replace( "Apr", "04" ).replace( "May", "05" ).replace( "Jun", "06" ).replace( "Jul", "07" ).replace( "Aug", "08" ).replace( "Sep", "09" ).replace( "Oct", "10" ).replace( "Nov", "11" ).replace( "Dec", "12" )
```

### Comparing `sunspot-0.6/src/test.py` & `sunspot-0.7/src/test.py`

 * *Files identical despite different names*

