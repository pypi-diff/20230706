# Comparing `tmp/estratega-utils-0.0.1.tar.gz` & `tmp/estratega-utils-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estratega-utils-0.0.1.tar", last modified: Thu Jul  6 14:23:26 2023, max compression
+gzip compressed data, was "estratega-utils-1.1.tar", last modified: Thu Jul  6 15:04:32 2023, max compression
```

## Comparing `estratega-utils-0.0.1.tar` & `estratega-utils-1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 14:23:26.700587 estratega-utils-0.0.1/
--rw-rw-rw-   0        0        0      580 2023-07-06 14:23:26.699587 estratega-utils-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 14:23:26.693603 estratega-utils-0.0.1/estratega_utils.egg-info/
--rw-rw-rw-   0        0        0      580 2023-07-06 14:23:26.000000 estratega-utils-0.0.1/estratega_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-06 14:23:26.000000 estratega-utils-0.0.1/estratega_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 14:23:26.000000 estratega-utils-0.0.1/estratega_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-06 14:23:26.000000 estratega-utils-0.0.1/estratega_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 14:23:26.000000 estratega-utils-0.0.1/estratega_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 14:23:26.700587 estratega-utils-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-07-06 13:48:55.000000 estratega-utils-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 14:23:26.698591 estratega-utils-0.0.1/utils/
--rw-rw-rw-   0        0        0       25 2023-07-06 13:43:15.000000 estratega-utils-0.0.1/utils/__init__.py
--rw-rw-rw-   0        0        0      822 2023-07-06 13:42:40.000000 estratega-utils-0.0.1/utils/objetos.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:04:32.843763 estratega-utils-1.1/
+-rw-rw-rw-   0        0        0      578 2023-07-06 15:04:32.843763 estratega-utils-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 15:04:32.821823 estratega-utils-1.1/estratega_utils.egg-info/
+-rw-rw-rw-   0        0        0      578 2023-07-06 15:04:32.000000 estratega-utils-1.1/estratega_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-07-06 15:04:32.000000 estratega-utils-1.1/estratega_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:04:32.000000 estratega-utils-1.1/estratega_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 15:04:32.000000 estratega-utils-1.1/estratega_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 15:04:32.000000 estratega-utils-1.1/estratega_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:04:32.844761 estratega-utils-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2023-07-06 14:50:13.000000 estratega-utils-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:04:32.841770 estratega-utils-1.1/utils/
+-rw-rw-rw-   0        0        0       78 2023-07-06 15:01:30.000000 estratega-utils-1.1/utils/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-07-06 13:42:40.000000 estratega-utils-1.1/utils/objetos.py
+-rw-rw-rw-   0        0        0      403 2023-07-06 14:57:10.000000 estratega-utils-1.1/utils/strings.py
```

### Comparing `estratega-utils-0.0.1/PKG-INFO` & `estratega-utils-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estratega-utils
-Version: 0.0.1
+Version: 1.1
 Summary: Utilidades varias
 Author: Ivan Sayavedra
 Author-email: <isayavedra@estrategasoftware.com.ar>
 Keywords: python,estratega utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `estratega-utils-0.0.1/estratega_utils.egg-info/PKG-INFO` & `estratega-utils-1.1/estratega_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estratega-utils
-Version: 0.0.1
+Version: 1.1
 Summary: Utilidades varias
 Author: Ivan Sayavedra
 Author-email: <isayavedra@estrategasoftware.com.ar>
 Keywords: python,estratega utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `estratega-utils-0.0.1/setup.py` & `estratega-utils-1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '1.1'
 DESCRIPTION = 'Utilidades varias'
 LONG_DESCRIPTION = 'Funciones y clases con utiliddades para agilizar y optimizar la escritura de código'
 
 # Configurando
 setup(
     # el nombre debe coincidir con el nombre de la carpeta
     # 'modulomuysimple'
@@ -12,15 +12,15 @@
     version=VERSION,
     author="Ivan Sayavedra",
     author_email="<isayavedra@estrategasoftware.com.ar>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     # añade cualquier paquete adicional que debe ser
-    install_requires=['typing', 'devtools', 'pydantic'],
+    install_requires=['pydantic'],
     # instalado junto con tu paquete. Ej: 'caer'
 
     keywords=['python', 'estratega utils'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 2",
```

### Comparing `estratega-utils-0.0.1/utils/objetos.py` & `estratega-utils-1.1/utils/objetos.py`

 * *Files identical despite different names*

