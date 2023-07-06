# Comparing `tmp/tychos-0.0.2.tar.gz` & `tmp/tychos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tychos-0.0.2.tar", last modified: Fri Jun 30 20:18:24 2023, max compression
+gzip compressed data, was "tychos-0.0.3.tar", last modified: Thu Jul  6 14:11:48 2023, max compression
```

## Comparing `tychos-0.0.2.tar` & `tychos-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-30 20:18:24.844036 tychos-0.0.2/
--rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.2/LICENSE
--rw-r--r--   0 abe732     (501) staff       (20)       95 2023-06-30 20:18:24.843918 tychos-0.0.2/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)       19 2023-06-27 16:59:52.000000 tychos-0.0.2/README.md
--rw-r--r--   0 abe732     (501) staff       (20)       38 2023-06-30 20:18:24.844067 tychos-0.0.2/setup.cfg
--rw-r--r--   0 abe732     (501) staff       (20)      138 2023-06-30 20:16:58.000000 tychos-0.0.2/setup.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-30 20:18:24.842991 tychos-0.0.2/tychos/
--rw-r--r--   0 abe732     (501) staff       (20)       74 2023-06-30 15:48:02.000000 tychos-0.0.2/tychos/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-26 15:20:14.000000 tychos-0.0.2/tychos/api.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-30 20:18:24.843786 tychos-0.0.2/tychos/helpers/
--rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-30 14:56:23.000000 tychos-0.0.2/tychos/helpers/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1296 2023-06-30 20:02:27.000000 tychos-0.0.2/tychos/vector.py
--rw-r--r--   0 abe732     (501) staff       (20)      996 2023-06-30 20:02:19.000000 tychos-0.0.2/tychos/vector_data_store.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-30 20:18:24.843678 tychos-0.0.2/tychos.egg-info/
--rw-r--r--   0 abe732     (501) staff       (20)       95 2023-06-30 20:18:24.000000 tychos-0.0.2/tychos.egg-info/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)      280 2023-06-30 20:18:24.000000 tychos-0.0.2/tychos.egg-info/SOURCES.txt
--rw-r--r--   0 abe732     (501) staff       (20)        1 2023-06-30 20:18:24.000000 tychos-0.0.2/tychos.egg-info/dependency_links.txt
--rw-r--r--   0 abe732     (501) staff       (20)        9 2023-06-30 20:18:24.000000 tychos-0.0.2/tychos.egg-info/requires.txt
--rw-r--r--   0 abe732     (501) staff       (20)        7 2023-06-30 20:18:24.000000 tychos-0.0.2/tychos.egg-info/top_level.txt
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-06 14:11:48.542961 tychos-0.0.3/
+-rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.3/LICENSE
+-rw-r--r--   0 abe732     (501) staff       (20)       95 2023-07-06 14:11:48.542802 tychos-0.0.3/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)     2507 2023-07-05 22:42:39.000000 tychos-0.0.3/README.md
+-rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-06 14:11:48.543003 tychos-0.0.3/setup.cfg
+-rw-r--r--   0 abe732     (501) staff       (20)      246 2023-07-06 14:09:11.000000 tychos-0.0.3/setup.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-06 14:11:48.541137 tychos-0.0.3/tychos/
+-rw-r--r--   0 abe732     (501) staff       (20)       74 2023-06-30 15:48:02.000000 tychos-0.0.3/tychos/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1084 2023-07-05 20:35:35.000000 tychos-0.0.3/tychos/cli.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-06 14:11:48.542629 tychos-0.0.3/tychos/helpers/
+-rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-30 14:56:23.000000 tychos-0.0.3/tychos/helpers/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1296 2023-06-30 20:02:27.000000 tychos-0.0.3/tychos/vector.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1259 2023-07-05 22:43:42.000000 tychos-0.0.3/tychos/vector_data_store.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-06 14:11:48.542499 tychos-0.0.3/tychos.egg-info/
+-rw-r--r--   0 abe732     (501) staff       (20)       95 2023-07-06 14:11:48.000000 tychos-0.0.3/tychos.egg-info/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)      313 2023-07-06 14:11:48.000000 tychos-0.0.3/tychos.egg-info/SOURCES.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-06 14:11:48.000000 tychos-0.0.3/tychos.egg-info/dependency_links.txt
+-rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-06 14:11:48.000000 tychos-0.0.3/tychos.egg-info/entry_points.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-06 14:11:48.000000 tychos-0.0.3/tychos.egg-info/requires.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-06 14:11:48.000000 tychos-0.0.3/tychos.egg-info/top_level.txt
```

### Comparing `tychos-0.0.2/LICENSE` & `tychos-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tychos-0.0.2/tychos/vector.py` & `tychos-0.0.3/tychos/vector.py`

 * *Files identical despite different names*

### Comparing `tychos-0.0.2/tychos/vector_data_store.py` & `tychos-0.0.3/tychos/vector_data_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,8 +25,18 @@
                     'top': limit,
                 }
         response = requests.post(url=url, headers=headers, json=payload)
 
         # error handling
         response.raise_for_status()
 
+        return response.json()
+    
+    def list(self):
+        url = f'{self.base_url}/datasets'
+        headers = {'api_key': self.api_key}
+        response = requests.get(url=url, headers=headers)
+
+        # error handling
+        response.raise_for_status()
+
         return response.json()
```

