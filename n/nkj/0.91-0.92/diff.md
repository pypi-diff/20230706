# Comparing `tmp/nkj-0.91.tar.gz` & `tmp/nkj-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkj-0.91.tar", last modified: Thu Jul  6 10:21:13 2023, max compression
+gzip compressed data, was "nkj-0.92.tar", last modified: Thu Jul  6 10:20:47 2023, max compression
```

## Comparing `nkj-0.91.tar` & `nkj-0.92.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-06 10:21:13.565808 nkj-0.91/
--rw-r--r--   0 nakajima   (501) staff       (20)      151 2023-07-06 10:21:13.565692 nkj-0.91/PKG-INFO
-drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-06 10:21:13.564927 nkj-0.91/nkj/
--rw-r--r--   0 nakajima   (501) staff       (20)      190 2023-05-22 09:16:20.000000 nkj-0.91/nkj/__init__.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1760 2023-05-02 17:38:40.000000 nkj-0.91/nkj/arg.py
--rw-r--r--   0 nakajima   (501) staff       (20)    16357 2023-07-04 12:22:38.000000 nkj-0.91/nkj/cam.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1232 2023-05-03 06:08:21.000000 nkj-0.91/nkj/core.py
--rw-r--r--   0 nakajima   (501) staff       (20)     6795 2023-06-12 14:04:44.000000 nkj-0.91/nkj/curvefit.py
--rw-r--r--   0 nakajima   (501) staff       (20)     3593 2023-05-02 18:05:13.000000 nkj-0.91/nkj/cv.py
--rw-r--r--   0 nakajima   (501) staff       (20)    23284 2023-06-08 08:47:20.000000 nkj-0.91/nkj/cwt.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2284 2023-06-19 16:47:05.000000 nkj-0.91/nkj/ea.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2393 2023-05-02 17:46:49.000000 nkj-0.91/nkj/fa.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2325 2023-05-02 17:50:02.000000 nkj-0.91/nkj/file.py
--rw-r--r--   0 nakajima   (501) staff       (20)     3857 2023-05-19 07:00:21.000000 nkj-0.91/nkj/filter.py
--rw-r--r--   0 nakajima   (501) staff       (20)    13595 2023-06-20 02:11:43.000000 nkj-0.91/nkj/func.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1150 2023-05-02 17:34:25.000000 nkj-0.91/nkj/json.py
--rw-r--r--   0 nakajima   (501) staff       (20)    80728 2023-07-06 02:01:51.000000 nkj-0.91/nkj/math.py
--rw-r--r--   0 nakajima   (501) staff       (20)      502 2023-05-02 15:36:15.000000 nkj-0.91/nkj/np.py
--rw-r--r--   0 nakajima   (501) staff       (20)     1638 2023-05-02 17:37:18.000000 nkj-0.91/nkj/os.py
--rw-r--r--   0 nakajima   (501) staff       (20)     2149 2023-05-02 15:36:15.000000 nkj-0.91/nkj/plot.py
--rw-r--r--   0 nakajima   (501) staff       (20)      701 2023-05-02 17:17:27.000000 nkj-0.91/nkj/prob.py
--rw-r--r--   0 nakajima   (501) staff       (20)     3326 2023-05-03 03:21:09.000000 nkj-0.91/nkj/pygame.py
--rw-r--r--   0 nakajima   (501) staff       (20)     9145 2023-05-03 03:23:05.000000 nkj-0.91/nkj/serial.py
--rw-r--r--   0 nakajima   (501) staff       (20)      186 2023-05-02 17:55:10.000000 nkj-0.91/nkj/socket.py
--rw-r--r--   0 nakajima   (501) staff       (20)     5356 2023-05-02 17:41:44.000000 nkj-0.91/nkj/stat.py
--rw-r--r--   0 nakajima   (501) staff       (20)     5941 2023-06-27 07:05:16.000000 nkj-0.91/nkj/str.py
-drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-06 10:21:13.565539 nkj-0.91/nkj.egg-info/
--rw-r--r--   0 nakajima   (501) staff       (20)      151 2023-07-06 10:21:13.000000 nkj-0.91/nkj.egg-info/PKG-INFO
--rw-r--r--   0 nakajima   (501) staff       (20)      394 2023-07-06 10:21:13.000000 nkj-0.91/nkj.egg-info/SOURCES.txt
--rw-r--r--   0 nakajima   (501) staff       (20)        1 2023-07-06 10:21:13.000000 nkj-0.91/nkj.egg-info/dependency_links.txt
--rw-r--r--   0 nakajima   (501) staff       (20)        4 2023-07-06 10:21:13.000000 nkj-0.91/nkj.egg-info/top_level.txt
--rw-r--r--   0 nakajima   (501) staff       (20)       38 2023-07-06 10:21:13.565849 nkj-0.91/setup.cfg
--rw-r--r--   0 nakajima   (501) staff       (20)      285 2023-07-06 10:21:07.000000 nkj-0.91/setup.py
+drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-06 10:20:47.208821 nkj-0.92/
+-rw-r--r--   0 nakajima   (501) staff       (20)      151 2023-07-06 10:20:47.208695 nkj-0.92/PKG-INFO
+drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-06 10:20:47.207840 nkj-0.92/nkj/
+-rw-r--r--   0 nakajima   (501) staff       (20)      190 2023-05-22 09:16:20.000000 nkj-0.92/nkj/__init__.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1760 2023-05-02 17:38:40.000000 nkj-0.92/nkj/arg.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    16357 2023-07-04 12:22:38.000000 nkj-0.92/nkj/cam.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1232 2023-05-03 06:08:21.000000 nkj-0.92/nkj/core.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     6795 2023-06-12 14:04:44.000000 nkj-0.92/nkj/curvefit.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     3593 2023-05-02 18:05:13.000000 nkj-0.92/nkj/cv.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    23284 2023-06-08 08:47:20.000000 nkj-0.92/nkj/cwt.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2284 2023-06-19 16:47:05.000000 nkj-0.92/nkj/ea.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2393 2023-05-02 17:46:49.000000 nkj-0.92/nkj/fa.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2325 2023-05-02 17:50:02.000000 nkj-0.92/nkj/file.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     3857 2023-05-19 07:00:21.000000 nkj-0.92/nkj/filter.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    13595 2023-06-20 02:11:43.000000 nkj-0.92/nkj/func.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1150 2023-05-02 17:34:25.000000 nkj-0.92/nkj/json.py
+-rw-r--r--   0 nakajima   (501) staff       (20)    80728 2023-07-06 02:01:51.000000 nkj-0.92/nkj/math.py
+-rw-r--r--   0 nakajima   (501) staff       (20)      502 2023-05-02 15:36:15.000000 nkj-0.92/nkj/np.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     1638 2023-05-02 17:37:18.000000 nkj-0.92/nkj/os.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     2149 2023-05-02 15:36:15.000000 nkj-0.92/nkj/plot.py
+-rw-r--r--   0 nakajima   (501) staff       (20)      701 2023-05-02 17:17:27.000000 nkj-0.92/nkj/prob.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     3326 2023-05-03 03:21:09.000000 nkj-0.92/nkj/pygame.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     9145 2023-05-03 03:23:05.000000 nkj-0.92/nkj/serial.py
+-rw-r--r--   0 nakajima   (501) staff       (20)      186 2023-05-02 17:55:10.000000 nkj-0.92/nkj/socket.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     5356 2023-05-02 17:41:44.000000 nkj-0.92/nkj/stat.py
+-rw-r--r--   0 nakajima   (501) staff       (20)     5941 2023-06-27 07:05:16.000000 nkj-0.92/nkj/str.py
+drwxr-xr-x   0 nakajima   (501) staff       (20)        0 2023-07-06 10:20:47.208526 nkj-0.92/nkj.egg-info/
+-rw-r--r--   0 nakajima   (501) staff       (20)      151 2023-07-06 10:20:47.000000 nkj-0.92/nkj.egg-info/PKG-INFO
+-rw-r--r--   0 nakajima   (501) staff       (20)      394 2023-07-06 10:20:47.000000 nkj-0.92/nkj.egg-info/SOURCES.txt
+-rw-r--r--   0 nakajima   (501) staff       (20)        1 2023-07-06 10:20:47.000000 nkj-0.92/nkj.egg-info/dependency_links.txt
+-rw-r--r--   0 nakajima   (501) staff       (20)        4 2023-07-06 10:20:47.000000 nkj-0.92/nkj.egg-info/top_level.txt
+-rw-r--r--   0 nakajima   (501) staff       (20)       38 2023-07-06 10:20:47.208869 nkj-0.92/setup.cfg
+-rw-r--r--   0 nakajima   (501) staff       (20)      285 2023-07-06 10:19:56.000000 nkj-0.92/setup.py
```

### Comparing `nkj-0.91/nkj/arg.py` & `nkj-0.92/nkj/arg.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/cam.py` & `nkj-0.92/nkj/cam.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/core.py` & `nkj-0.92/nkj/core.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/curvefit.py` & `nkj-0.92/nkj/curvefit.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/cv.py` & `nkj-0.92/nkj/cv.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/cwt.py` & `nkj-0.92/nkj/cwt.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/ea.py` & `nkj-0.92/nkj/ea.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/fa.py` & `nkj-0.92/nkj/fa.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/file.py` & `nkj-0.92/nkj/file.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/filter.py` & `nkj-0.92/nkj/filter.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/func.py` & `nkj-0.92/nkj/func.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/json.py` & `nkj-0.92/nkj/json.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/math.py` & `nkj-0.92/nkj/math.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/os.py` & `nkj-0.92/nkj/os.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/plot.py` & `nkj-0.92/nkj/plot.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/prob.py` & `nkj-0.92/nkj/prob.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/pygame.py` & `nkj-0.92/nkj/pygame.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/serial.py` & `nkj-0.92/nkj/serial.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/stat.py` & `nkj-0.92/nkj/stat.py`

 * *Files identical despite different names*

### Comparing `nkj-0.91/nkj/str.py` & `nkj-0.92/nkj/str.py`

 * *Files identical despite different names*

