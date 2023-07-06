# Comparing `tmp/signe-0.1.2.tar.gz` & `tmp/signe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signe-0.1.2.tar", last modified: Tue Jun 27 15:44:53 2023, max compression
+gzip compressed data, was "signe-0.1.3.tar", last modified: Thu Jul  6 05:26:27 2023, max compression
```

## Comparing `signe-0.1.2.tar` & `signe-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 15:44:53.069589 signe-0.1.2/
--rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      469 2023-06-27 15:44:53.068592 signe-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 15:44:53.069589 signe-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:44:53.041797 signe-0.1.2/signe/
--rw-rw-rw-   0        0        0      160 2023-06-27 15:44:38.000000 signe-0.1.2/signe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:44:53.063721 signe-0.1.2/signe/core/
--rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.2/signe/core/__init__.py
--rw-rw-rw-   0        0        0      537 2023-06-25 12:24:57.000000 signe-0.1.2/signe/core/collections.py
--rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.2/signe/core/consts.py
--rw-rw-rw-   0        0        0     4309 2023-06-26 14:25:04.000000 signe-0.1.2/signe/core/effect.py
--rw-rw-rw-   0        0        0     2493 2023-06-25 12:24:57.000000 signe-0.1.2/signe/core/runtime.py
--rw-rw-rw-   0        0        0     2737 2023-06-25 12:24:57.000000 signe-0.1.2/signe/core/signal.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:44:53.066728 signe-0.1.2/signe/reactive/
--rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.2/signe/reactive/__init__.py
--rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.2/signe/reactive/proxy.py
--rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.2/signe/types.py
--rw-rw-rw-   0        0        0     1571 2023-06-26 14:13:09.000000 signe-0.1.2/signe/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:44:53.051753 signe-0.1.2/signe.egg-info/
--rw-rw-rw-   0        0        0      469 2023-06-27 15:44:52.000000 signe-0.1.2/signe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-06-27 15:44:53.000000 signe-0.1.2/signe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 15:44:52.000000 signe-0.1.2/signe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-27 15:44:52.000000 signe-0.1.2/signe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-06-27 15:44:52.000000 signe-0.1.2/signe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 05:26:26.996710 signe-0.1.3/
+-rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      469 2023-07-06 05:26:26.995712 signe-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 05:26:26.997229 signe-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 05:26:26.969414 signe-0.1.3/signe/
+-rw-rw-rw-   0        0        0      164 2023-07-06 05:26:07.000000 signe-0.1.3/signe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 05:26:26.989725 signe-0.1.3/signe/core/
+-rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.3/signe/core/__init__.py
+-rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.3/signe/core/collections.py
+-rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.3/signe/core/consts.py
+-rw-rw-rw-   0        0        0     4309 2023-06-26 14:25:04.000000 signe-0.1.3/signe/core/effect.py
+-rw-rw-rw-   0        0        0     2493 2023-06-25 12:24:57.000000 signe-0.1.3/signe/core/runtime.py
+-rw-rw-rw-   0        0        0     2737 2023-06-25 12:24:57.000000 signe-0.1.3/signe/core/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-06 05:26:26.993719 signe-0.1.3/signe/reactive/
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.3/signe/reactive/__init__.py
+-rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.3/signe/reactive/proxy.py
+-rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.3/signe/types.py
+-rw-rw-rw-   0        0        0     3062 2023-07-06 05:25:51.000000 signe-0.1.3/signe/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 05:26:26.978713 signe-0.1.3/signe.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-07-06 05:26:26.000000 signe-0.1.3/signe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-06 05:26:26.000000 signe-0.1.3/signe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 05:26:26.000000 signe-0.1.3/signe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 05:26:26.000000 signe-0.1.3/signe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-06 05:26:26.000000 signe-0.1.3/signe.egg-info/top_level.txt
```

### Comparing `signe-0.1.2/LICENSE` & `signe-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `signe-0.1.2/README.md` & `signe-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `signe-0.1.2/setup.py` & `signe-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.2/signe/core/collections.py` & `signe-0.1.3/signe/core/collections.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,15 +11,18 @@
     def set_current(self, obj: T):
         self.__stack.append(obj)
 
     def is_current(self, obj: T):
         return self.get_current() is obj
 
     def reset_current(self):
-        self.__stack.pop()
+        return self.__stack.pop()
+
+    def __len__(self):
+        return len(self.__stack)
 
     def get_current(
         self,
     ):
         if len(self.__stack) <= 0:
             return None
```

### Comparing `signe-0.1.2/signe/core/effect.py` & `signe-0.1.3/signe/core/effect.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.2/signe/core/runtime.py` & `signe-0.1.3/signe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.2/signe/core/signal.py` & `signe-0.1.3/signe/core/signal.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.2/signe/reactive/proxy.py` & `signe-0.1.3/signe/reactive/proxy.py`

 * *Files identical despite different names*

