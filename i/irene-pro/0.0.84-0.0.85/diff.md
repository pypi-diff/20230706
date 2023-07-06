# Comparing `tmp/irene_pro-0.0.84.tar.gz` & `tmp/irene_pro-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.84.tar", last modified: Wed Jul  5 14:02:35 2023, max compression
+gzip compressed data, was "irene_pro-0.0.85.tar", last modified: Thu Jul  6 13:55:36 2023, max compression
```

## Comparing `irene_pro-0.0.84.tar` & `irene_pro-0.0.85.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 14:02:35.483549 irene_pro-0.0.84/
--rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.84/LICENSE
--rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.84/MANIFEST.in
--rw-rw-rw-   0        0        0     1280 2023-07-05 14:02:35.482551 irene_pro-0.0.84/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.84/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 14:02:35.466593 irene_pro-0.0.84/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.84/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     8171 2023-07-05 12:28:28.000000 irene_pro-0.0.84/irene_pro/logics.py
--rw-rw-rw-   0        0        0    35895 2023-07-05 14:01:23.000000 irene_pro-0.0.84/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:02:35.479562 irene_pro-0.0.84/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1280 2023-07-05 14:02:35.000000 irene_pro-0.0.84/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-05 14:02:35.000000 irene_pro-0.0.84/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 14:02:35.000000 irene_pro-0.0.84/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-05 14:02:35.000000 irene_pro-0.0.84/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 14:02:35.000000 irene_pro-0.0.84/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 14:02:35.483549 irene_pro-0.0.84/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-07-05 14:01:54.000000 irene_pro-0.0.84/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:55:36.436880 irene_pro-0.0.85/
+-rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.85/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.85/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-07-06 13:55:36.433913 irene_pro-0.0.85/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.85/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 13:55:36.393463 irene_pro-0.0.85/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.85/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     8186 2023-07-06 13:52:26.000000 irene_pro-0.0.85/irene_pro/logics.py
+-rw-rw-rw-   0        0        0    35895 2023-07-06 13:53:43.000000 irene_pro-0.0.85/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:55:36.426376 irene_pro-0.0.85/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-07-06 13:55:36.000000 irene_pro-0.0.85/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-06 13:55:36.000000 irene_pro-0.0.85/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:55:36.000000 irene_pro-0.0.85/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-06 13:55:36.000000 irene_pro-0.0.85/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 13:55:36.000000 irene_pro-0.0.85/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 13:55:36.437874 irene_pro-0.0.85/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-07-06 13:54:11.000000 irene_pro-0.0.85/setup.py
```

### Comparing `irene_pro-0.0.84/PKG-INFO` & `irene_pro-0.0.85/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.84
+Version: 0.0.85
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.84/README.md` & `irene_pro-0.0.85/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.84/irene_pro/logics.py` & `irene_pro-0.0.85/irene_pro/logics.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 class DateTime:
     def __init__(self, week = datetime.today().isocalendar()[1], day = strftime("%Y-%m-%d"), 
                  month = strftime("%Y-%m"), year = strftime("%Y"), current_weeks = None, combined = int(strftime("%Y%m%d%H%M")),
                    combined_date = None) -> None:
         self.week = week
         self.day = day
         self.month = month
-        self.year = year
-        self.current_weeks = current_weeks
+        self.year = int(year)
+        self.current_weeks = int(current_weeks)
         self.current_weeks = str(week) + str(year)
-        self.combined = combined
+        self.combined = int(combined)
         self.combined_date = combined_date
 
     def datedelta(self, start, end):
         date1 = datetime.strptime(start, "%Y-%m-%d %H:%M:%S")
         date2 = datetime.strptime(end, "%Y-%m-%d %H:%M:%S")
         delta = date2 - date1
         return delta
```

### Comparing `irene_pro-0.0.84/irene_pro/widgets.py` & `irene_pro-0.0.85/irene_pro/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 
         if " all" in str(self['text']).lower():
             self.config(image = image)
         
         if " id" in str(self['text']).lower():
             self.config(image = image)
         
-        self.bind('<Enter>', lambda e: self.config(bg = '#39ff13'))
+        self.bind('<Enter>', lambda e: self.config(bg = '#FF78C4'))
         self.bind('<Leave>', lambda e: self.config(bg = prev_color))
     
 
 class Display_image:
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `irene_pro-0.0.84/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.85/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.84
+Version: 0.0.85
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.84/setup.py` & `irene_pro-0.0.85/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3834 270d 0a44 4553 4352   '0.0.84'..DESCR
+00000100: 2027 302e 302e 3835 270d 0a44 4553 4352   '0.0.85'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

