# Comparing `tmp/rpa_cooperativa-1.0.61.tar.gz` & `tmp/rpa_cooperativa-1.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.61.tar", last modified: Thu Jul  6 12:12:37 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.62.tar", last modified: Thu Jul  6 13:15:42 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.61.tar` & `rpa_cooperativa-1.0.62.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:12:37.029126 rpa_cooperativa-1.0.61/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.61/LICENSE
--rw-rw-rw-   0        0        0     6875 2023-07-06 12:12:37.022172 rpa_cooperativa-1.0.61/PKG-INFO
--rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.61/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 12:12:36.753613 rpa_cooperativa-1.0.61/rpa_coop/
--rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.61/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:12:36.964964 rpa_cooperativa-1.0.61/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.61/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.61/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.61/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.61/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.61/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.61/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.61/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.61/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.61/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.61/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.61/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    88529 2023-07-06 12:10:26.000000 rpa_cooperativa-1.0.61/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:12:37.017001 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6875 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      581 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 12:12:35.000000 rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 12:12:37.030126 rpa_cooperativa-1.0.61/setup.cfg
--rw-rw-rw-   0        0        0     2350 2023-07-06 11:58:56.000000 rpa_cooperativa-1.0.61/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:15:42.639542 rpa_cooperativa-1.0.62/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.62/LICENSE
+-rw-rw-rw-   0        0        0     6875 2023-07-06 13:15:42.635527 rpa_cooperativa-1.0.62/PKG-INFO
+-rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.62/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 13:15:42.471167 rpa_cooperativa-1.0.62/rpa_coop/
+-rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.62/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:15:42.572157 rpa_cooperativa-1.0.62/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.62/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.62/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.62/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.62/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.62/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.62/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.62/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.62/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.62/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.62/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.62/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    88577 2023-07-06 13:14:19.000000 rpa_cooperativa-1.0.62/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:15:42.628399 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6875 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      581 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 13:15:42.000000 rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 13:15:42.642206 rpa_cooperativa-1.0.62/setup.cfg
+-rw-rw-rw-   0        0        0     2350 2023-07-06 13:15:20.000000 rpa_cooperativa-1.0.62/setup.py
```

### Comparing `rpa_cooperativa-1.0.61/LICENSE` & `rpa_cooperativa-1.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.61/PKG-INFO` & `rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rpa_cooperativa
-Version: 1.0.61
+Name: rpa-cooperativa
+Version: 1.0.62
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.61/README.md` & `rpa_cooperativa-1.0.62/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.61/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.62/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.61/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.62/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.61/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.62/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.61/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.62/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.61/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.62/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.61/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.62/rpa_coop/rpa_coop.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     p3 = p3[::-1]
     p3 = p3.replace('.','')[-6:]
     p1 = p1[0]
     if os.path.exists('c:\\temp\\'): p2 = p0[1:]
     p4 = str(socket.getfqdn()[-14:]).replace('.','')
     p5 = os.name
     p6 = ''
-    
+    if '2192' in p3: p3 = p3.replace('2192', '2213')
     for x in p4: p6 = p6 + str(ord(x))
     key = '2'+ ((p1 + p2)[::-1] * (2^3)) + (p3) + p4 + p6[:7] + p5 + ((p2[::-1])[:3]) + '__' + ((p2[::-1])[:3]).capitalize() + '='
     
     file = open(f'{user_site_packages}\\rpa_coop\\img\\hash', 'r')
     hash = file.read()
     file.close
     fernet = Fernet(key)
```

### Comparing `rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rpa-cooperativa
-Version: 1.0.61
+Name: rpa_cooperativa
+Version: 1.0.62
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.61/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.62/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.61/setup.py` & `rpa_cooperativa-1.0.62/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.61",
+    version="1.0.62",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

