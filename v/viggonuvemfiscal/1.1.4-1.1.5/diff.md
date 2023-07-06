# Comparing `tmp/viggonuvemfiscal-1.1.4.tar.gz` & `tmp/viggonuvemfiscal-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggonuvemfiscal-1.1.4.tar", last modified: Wed Jul  5 16:47:31 2023, max compression
+gzip compressed data, was "viggonuvemfiscal-1.1.5.tar", last modified: Thu Jul  6 18:38:00 2023, max compression
```

## Comparing `viggonuvemfiscal-1.1.4.tar` & `viggonuvemfiscal-1.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:31.323510 viggonuvemfiscal-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-05 16:47:31.323510 viggonuvemfiscal-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:47:31.323510 viggonuvemfiscal-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:31.319510 viggonuvemfiscal-1.1.4/viggonuvemfiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:31.319510 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:31.319510 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:31.319510 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:31.323510 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    19322 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-05 16:46:39.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:31.319510 viggonuvemfiscal-1.1.4/viggonuvemfiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-05 16:47:31.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-05 16:47:31.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:47:31.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-05 16:47:31.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 16:47:31.000000 viggonuvemfiscal-1.1.4/viggonuvemfiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:38:00.101575 viggonuvemfiscal-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-06 18:38:00.101575 viggonuvemfiscal-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:38:00.101575 viggonuvemfiscal-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:38:00.101575 viggonuvemfiscal-1.1.5/viggonuvemfiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:38:00.101575 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:38:00.101575 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:38:00.101575 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:38:00.101575 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19329 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-06 18:37:10.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:38:00.101575 viggonuvemfiscal-1.1.5/viggonuvemfiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-06 18:38:00.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-06 18:38:00.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:38:00.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 18:38:00.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 18:38:00.000000 viggonuvemfiscal-1.1.5/viggonuvemfiscal.egg-info/top_level.txt
```

### Comparing `viggonuvemfiscal-1.1.4/viggonuvemfiscal/__init__.py` & `viggonuvemfiscal-1.1.5/viggonuvemfiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.4/viggonuvemfiscal/resources.py` & `viggonuvemfiscal-1.1.5/viggonuvemfiscal/resources.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py` & `viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py` & `viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py` & `viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,16 +296,16 @@
         return self.manager.executar_requisicao('GET', url, ambiente=ambiente)
 
 
 class BaixarXmlNfce(operation.List):
 
     def do(self, session, **kwargs):
         ambiente = kwargs.pop('api_fiscal', cnf_tipo.HOMOLOGACAO)
-        nfe_id = self.manager.get_nfe_id(**kwargs)
-        url = self.manager.get_endpoint(f'/nfe/{nfe_id}/xml/nota', ambiente)
+        nfce_id = self.manager.get_nfce_id(**kwargs)
+        url = self.manager.get_endpoint(f'/nfce/{nfce_id}/xml/nota', ambiente)
         return self.manager.executar_requisicao('GET', url, ambiente=ambiente)
 
 
 class BaixarXmlNotaNfce(operation.List):
 
     def do(self, session, **kwargs):
         ambiente = kwargs.pop('api_fiscal', cnf_tipo.HOMOLOGACAO)
@@ -326,34 +326,34 @@
         return self.manager.executar_requisicao('GET', url, ambiente=ambiente)
 
 
 class ConsultarCancelamentoNfce(operation.List):
 
     def do(self, session, **kwargs):
         ambiente = kwargs.pop('api_fiscal', cnf_tipo.HOMOLOGACAO)
-        nfce_id = self.manager.get_nfe_id(**kwargs)
+        nfce_id = self.manager.get_nfce_id(**kwargs)
         url = self.manager.get_endpoint(
             f'/nfce/{nfce_id}/cancelamento', ambiente)
         return self.manager.executar_requisicao('GET', url, ambiente=ambiente)
 
 
 class BaixarXmlCancelamentoNfce(operation.List):
     def do(self, session, **kwargs):
         ambiente = kwargs.pop('api_fiscal', cnf_tipo.HOMOLOGACAO)
-        nfce_id = self.manager.get_nfe_id(**kwargs)
+        nfce_id = self.manager.get_nfce_id(**kwargs)
         url = self.manager.get_endpoint(
             f'/nfce/{nfce_id}/cancelamento/xml', ambiente)
         return self.manager.executar_requisicao('GET', url, ambiente=ambiente)
 
 
 class CancelarNfceAutorizada(operation.List):
 
     def do(self, session, **kwargs):
         ambiente = kwargs.pop('api_fiscal', cnf_tipo.HOMOLOGACAO)
-        nfce_id = self.manager.get_nfe_id(**kwargs)
+        nfce_id = self.manager.get_nfce_id(**kwargs)
         url = self.manager.get_endpoint(
             f'/nfce/{nfce_id}/cancelamento', ambiente)
         kwargs.pop('nfce_id')
         return self.manager.executar_requisicao(
             'POST', url, json=kwargs, ambiente=ambiente)
```

### Comparing `viggonuvemfiscal-1.1.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py` & `viggonuvemfiscal-1.1.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.4/viggonuvemfiscal.egg-info/SOURCES.txt` & `viggonuvemfiscal-1.1.5/viggonuvemfiscal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

