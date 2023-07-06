# Comparing `tmp/BLACKFORGE2-0.2.5.tar.gz` & `tmp/BLACKFORGE2-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLACKFORGE2-0.2.5.tar", last modified: Tue Jun 27 04:59:03 2023, max compression
+gzip compressed data, was "BLACKFORGE2-0.2.6.tar", last modified: Thu Jul  6 10:24:43 2023, max compression
```

## Comparing `BLACKFORGE2-0.2.5.tar` & `BLACKFORGE2-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 04:59:03.289899 BLACKFORGE2-0.2.5/
-drwxrwxrwx   0        0        0        0 2023-06-27 04:59:03.276735 BLACKFORGE2-0.2.5/BLACKFORGE2/
--rw-rw-rw-   0        0        0    14640 2023-06-27 04:58:33.000000 BLACKFORGE2-0.2.5/BLACKFORGE2/FORGE.py
--rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.2.5/BLACKFORGE2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 04:59:03.287890 BLACKFORGE2-0.2.5/BLACKFORGE2.egg-info/
--rw-rw-rw-   0        0        0      312 2023-06-27 04:59:03.000000 BLACKFORGE2-0.2.5/BLACKFORGE2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-27 04:59:03.000000 BLACKFORGE2-0.2.5/BLACKFORGE2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 04:59:03.000000 BLACKFORGE2-0.2.5/BLACKFORGE2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-27 04:59:03.000000 BLACKFORGE2-0.2.5/BLACKFORGE2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-27 04:59:03.000000 BLACKFORGE2-0.2.5/BLACKFORGE2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      312 2023-06-27 04:59:03.288900 BLACKFORGE2-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     8967 2023-06-16 21:39:12.000000 BLACKFORGE2-0.2.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-27 04:59:03.289899 BLACKFORGE2-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-06-27 04:58:51.000000 BLACKFORGE2-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:24:43.312932 BLACKFORGE2-0.2.6/
+drwxrwxrwx   0        0        0        0 2023-07-06 10:24:43.298944 BLACKFORGE2-0.2.6/BLACKFORGE2/
+-rw-rw-rw-   0        0        0    14607 2023-07-06 10:22:14.000000 BLACKFORGE2-0.2.6/BLACKFORGE2/FORGE.py
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.2.6/BLACKFORGE2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:24:43.309939 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/
+-rw-rw-rw-   0        0        0      312 2023-07-06 10:24:43.000000 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-06 10:24:43.000000 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:24:43.000000 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 10:24:43.000000 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-06 10:24:43.000000 BLACKFORGE2-0.2.6/BLACKFORGE2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      312 2023-07-06 10:24:43.311935 BLACKFORGE2-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8967 2023-06-16 21:39:12.000000 BLACKFORGE2-0.2.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-06 10:24:43.312932 BLACKFORGE2-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-07-06 10:24:24.000000 BLACKFORGE2-0.2.6/setup.py
```

### Comparing `BLACKFORGE2-0.2.5/BLACKFORGE2/FORGE.py` & `BLACKFORGE2-0.2.6/BLACKFORGE2/FORGE.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 			self.base = pygame.Rect(base)
 			self.rect = self.base.copy()
 			self.surf = pygame.Surface((base[2], base[3]), pygame.SRCALPHA)
 			self.base_func = self.draw_rect
 		self.center = self.surf.get_rect().center
 
 		if isinstance(hovered, str):
-			self.hovered = pygame.transform.scale(get_image('../assets/ui/buttons/button_plate2.png'), (128,64))
+			self.hovered = pygame.transform.scale(get_image(hovered), (128,64))
 			self.hover_func = self.draw_image
 		else:
 			self.hovered = pygame.Rect(hovered)
 			self.hover_func = self.draw_rect
 
 		self.rect.center = self.position
 		self.text_color = text_color
```

### Comparing `BLACKFORGE2-0.2.5/LICENSE` & `BLACKFORGE2-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `BLACKFORGE2-0.2.5/README.rst` & `BLACKFORGE2-0.2.6/README.rst`

 * *Files identical despite different names*

