# Comparing `tmp/adapter-client-1.1.0.tar.gz` & `tmp/adapter-client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapter-client-1.1.0.tar", last modified: Mon Apr 17 05:19:00 2023, max compression
+gzip compressed data, was "adapter-client-1.2.0.tar", last modified: Thu Jul  6 12:44:45 2023, max compression
```

## Comparing `adapter-client-1.1.0.tar` & `adapter-client-1.2.0.tar`

### file list

```diff
@@ -1,54 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.784935 adapter-client-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      290 2022-07-22 09:13:24.000000 adapter-client-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4146 2023-04-17 05:19:00.784935 adapter-client-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3243 2022-07-22 09:13:24.000000 adapter-client-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.761935 adapter-client-1.1.0/requirements/
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-17 05:18:46.000000 adapter-client-1.1.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-22 09:13:24.000000 adapter-client-1.1.0/requirements/prod.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 05:19:00.784935 adapter-client-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2431 2022-07-22 09:13:24.000000 adapter-client-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.758935 adapter-client-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.764935 adapter-client-1.1.0/src/adapter_client/
--rw-r--r--   0 root         (0) root         (0)       70 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.766935 adapter-client-1.1.0/src/adapter_client/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3709 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/base.py
--rw-r--r--   0 root         (0) root         (0)     9914 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.768935 adapter-client-1.1.0/src/adapter_client/adapters/smev/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8563 2023-04-17 05:18:46.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.770935 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/
--rw-r--r--   0 root         (0) root         (0)       95 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1621 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.771935 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12607 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.774935 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/
--rw-r--r--   0 root         (0) root         (0)     8513 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl
--rw-r--r--   0 root         (0) root         (0)     4627 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd
--rw-r--r--   0 root         (0) root         (0)    56967 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.777935 adapter-client-1.1.0/src/adapter_client/adapters/smev/services/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      301 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/services/base.py
--rw-r--r--   0 root         (0) root         (0)     1501 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/adapters/smev/services/registry.py
--rw-r--r--   0 root         (0) root         (0)     3606 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/apps.py
--rw-r--r--   0 root         (0) root         (0)      961 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.781935 adapter-client-1.1.0/src/adapter_client/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.781935 adapter-client-1.1.0/src/adapter_client/core/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/core/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7973 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/core/domain/model.py
--rw-r--r--   0 root         (0) root         (0)      286 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/core/services.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.783935 adapter-client-1.1.0/src/adapter_client/migrations/
--rw-r--r--   0 root         (0) root         (0)     7165 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.1.0/src/adapter_client/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6597 2023-04-17 05:18:46.000000 adapter-client-1.1.0/src/adapter_client/models.py
--rw-r--r--   0 root         (0) root         (0)     4899 2023-04-17 05:18:46.000000 adapter-client-1.1.0/src/adapter_client/tasks.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-04-17 05:18:46.000000 adapter-client-1.1.0/src/adapter_client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:19:00.765935 adapter-client-1.1.0/src/adapter_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4146 2023-04-17 05:19:00.000000 adapter-client-1.1.0/src/adapter_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1543 2023-04-17 05:19:00.000000 adapter-client-1.1.0/src/adapter_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-17 05:19:00.000000 adapter-client-1.1.0/src/adapter_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-17 05:19:00.000000 adapter-client-1.1.0/src/adapter_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-17 05:19:00.000000 adapter-client-1.1.0/src/adapter_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      450 2023-04-17 05:19:00.000000 adapter-client-1.1.0/version.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.354353 adapter-client-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      290 2022-07-22 09:13:24.000000 adapter-client-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4353 2023-07-06 12:44:45.354353 adapter-client-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3243 2022-07-22 09:13:24.000000 adapter-client-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.330353 adapter-client-1.2.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-06 12:44:32.000000 adapter-client-1.2.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-07-22 09:13:24.000000 adapter-client-1.2.0/requirements/prod.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 12:44:45.354353 adapter-client-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-07-06 12:44:32.000000 adapter-client-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.325353 adapter-client-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.334353 adapter-client-1.2.0/src/adapter_client/
+-rw-r--r--   0 root         (0) root         (0)       70 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.336353 adapter-client-1.2.0/src/adapter_client/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/adapters/base.py
+-rw-r--r--   0 root         (0) root         (0)     9914 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.339353 adapter-client-1.2.0/src/adapter_client/adapters/smev/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8563 2023-04-17 05:18:46.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.341353 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/
+-rw-r--r--   0 root         (0) root         (0)       95 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.341353 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12607 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.345353 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/
+-rw-r--r--   0 root         (0) root         (0)     8513 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl
+-rw-r--r--   0 root         (0) root         (0)     4627 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd
+-rw-r--r--   0 root         (0) root         (0)    56967 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.347353 adapter-client-1.2.0/src/adapter_client/adapters/smev/logging/
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/logging/opensearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.349353 adapter-client-1.2.0/src/adapter_client/adapters/smev/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      301 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/services/base.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/services/registry.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/apps.py
+-rw-r--r--   0 root         (0) root         (0)      961 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.350353 adapter-client-1.2.0/src/adapter_client/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.351353 adapter-client-1.2.0/src/adapter_client/core/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/core/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9067 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/core/domain/model.py
+-rw-r--r--   0 root         (0) root         (0)      286 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/core/services.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.353353 adapter-client-1.2.0/src/adapter_client/migrations/
+-rw-r--r--   0 root         (0) root         (0)     7165 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7821 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/models.py
+-rw-r--r--   0 root         (0) root         (0)     5004 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/tasks.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-04-17 05:18:46.000000 adapter-client-1.2.0/src/adapter_client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.335353 adapter-client-1.2.0/src/adapter_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4353 2023-07-06 12:44:45.000000 adapter-client-1.2.0/src/adapter_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-07-06 12:44:45.000000 adapter-client-1.2.0/src/adapter_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-06 12:44:45.000000 adapter-client-1.2.0/src/adapter_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-06 12:44:45.000000 adapter-client-1.2.0/src/adapter_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 12:44:45.000000 adapter-client-1.2.0/src/adapter_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-06 12:44:45.000000 adapter-client-1.2.0/version.conf
```

### Comparing `adapter-client-1.1.0/PKG-INFO` & `adapter-client-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: adapter-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
+Provides-Extra: opensearch
 
 # Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 ## Подключение
 settings:
 
     INSTALLED_APPS = [
         'adapter_client'
```

### Comparing `adapter-client-1.1.0/README.md` & `adapter-client-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/setup.py` & `adapter-client-1.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,21 +55,30 @@
         'Environment :: Web Environment',
         'Natural Language :: Russian',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Development Status :: 5 - Production/Stable',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
+    extras_require={
+        'opensearch': (
+            'opensearch-logger==1.2.2',
+        ),
+    },
     dependency_links=(
         'https://pypi.bars-open.ru/simple/m3-builder',
     ),
     setup_requires=(
         'm3-builder>=1.2,<2',
     ),
     set_build_info=Path(__file__).parent,
```

### Comparing `adapter-client-1.1.0/src/adapter_client/adapters/base.py` & `adapter-client-1.2.0/src/adapter_client/adapters/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 # coding: utf-8
 from abc import ABC
 from abc import abstractmethod
-from datetime import datetime
 from typing import Generator
-from typing import Iterable
-from typing import Optional
-from typing import Union
 
+from adapter_client.adapters.smev.logging import AbstractJournal  # noqa - обратная совместимость
 from adapter_client.core.domain import model
 
-from .smev.interfaces.base import ExchangeResult
-
 
 class AbstractConfigRepository(ABC):
 
     @abstractmethod
     def load_config(self) -> model.Config:
         """Загрузить кофигурацию адаптера."""
 
@@ -69,40 +64,7 @@
         """Обновить входящее сообщение."""
 
     @abstractmethod
     def get_pending_messages(self) -> Generator[
         model.IncomingMessage, None, None
     ]:
         """Получить входящие сообщения ожидающие обработки в РИС."""
-
-
-class AbstractJournal(ABC):
-
-    """Абстрактный журнал обмена сообщениями."""
-
-    def __init__(self, config: model.Config) -> None:
-        assert isinstance(config, model.Config)
-        self._config = config
-
-    @abstractmethod
-    def log_exchange_result(
-        self,
-        exchange_result: ExchangeResult
-    ) -> model.JournalEntry:
-        """Записывает результат обмена в журнал и возвращает запись журнала."""
-
-    @abstractmethod
-    def get_entries(
-        self,
-        offset: int = 0,
-        limit: int = 25,
-        sort_fields: Optional[Iterable[str]] = None,
-        client_id: Optional[str] = None,
-        request_types: Optional[Iterable[model.RequestType]] = None,
-        timestamp_from: Optional[datetime] = None,
-        timestamp_to: Optional[datetime] = None,
-    ) -> Generator[model.JournalEntry, None, None]:
-        """Возвращает генератор с записями журнала."""
-
-    @abstractmethod
-    def get_entry_by_id(self, _id: Union[str, int]) -> model.JournalEntry:
-        """Возвращает одну запись по id."""
```

### Comparing `adapter-client-1.1.0/src/adapter_client/adapters/db.py` & `adapter-client-1.2.0/src/adapter_client/adapters/db.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/src/adapter_client/adapters/smev/adapter.py` & `adapter-client-1.2.0/src/adapter_client/adapters/smev/adapter.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/base.py` & `adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     from pydantic.dataclasses import dataclass  # noqa
 
 
 @dataclass
 class ExchangeResult:
 
     """Результат выполнения запроса."""
+
     request_type: model.RequestType
     message_metadata: Optional[model.MessageMetadataInterface] = None
     request: Any = None
     response: Any = None
     error: Any = None
     result: Any = None
     address: str = None
```

### Comparing `adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py` & `adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl` & `adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd` & `adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd` & `adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/src/adapter_client/adapters/smev/services/registry.py` & `adapter-client-1.2.0/src/adapter_client/adapters/smev/services/registry.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/src/adapter_client/apps.py` & `adapter-client-1.2.0/src/adapter_client/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                         if isinstance(self_object, command):
                             return True
 
                         if isinstance(self_object, ManagementUtility):
                             # Срабатывает при использовании функции в AppConfig
                             if 'subcommand' in frame.f_locals:
                                 subcommand = frame.f_locals['subcommand']
-                                return subcommand in ['migrate', 'test']
+                                return subcommand in ['makemigrations', 'migrate', 'test']
 
                     frame = frame.f_back
 
             modules = (
                 'django.core.management.commands.migrate',
                 'django.core.management.commands.makemigrations',
                 'django.core.management.commands.sqlmigrate',
```

### Comparing `adapter-client-1.1.0/src/adapter_client/config.py` & `adapter-client-1.2.0/src/adapter_client/config.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/src/adapter_client/core/domain/model.py` & `adapter-client-1.2.0/src/adapter_client/core/domain/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # coding: utf-8
 from abc import ABC
 from datetime import datetime
 from enum import Enum
 from typing import TYPE_CHECKING
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import TypeVar
 from typing import Union
 from uuid import uuid4
 
 from pydantic.fields import Field
+from pydantic.types import Json
 
 
 if TYPE_CHECKING:
     from dataclasses import dataclass  # noqa
 else:
     from pydantic.dataclasses import dataclass  # noqa
 
@@ -69,32 +71,42 @@
     # Настройки поиска сообщения
     find_request_retry_time: int = Field(
         title='Период опроса Адаптера на наличие ответов СМЭВ',
         default=30
     )
 
     # Настройки интерфейсов
-    request_timeout_sec: int = 10
+    request_timeout_sec: int = Field(
+        title='Таймаут запроса',
+        default=10
+    )
 
     # Используемые компоненты адаптера
     adapter_interface: str = Field(
+        title='Используемый интерфейс',
         default=(
             'adapter_client.adapters.smev.interfaces.soap.interface.Interface'
         )
     )
     outgoing_message_repository: str = Field(
+        title='Репозиторий исходящих сообщений',
         default='adapter_client.adapters.db.OutgoingMessageRepository'
     )
     incoming_message_repository: str = Field(
+        title='Репозиторий входящих сообщений',
         default='adapter_client.adapters.db.IncomingMessageRepository'
     )
-
     journal: str = Field(
+        title='Журнал обмена',
         default='adapter_client.adapters.db.Journal'
     )
+    journal_config: Optional[Dict] = Field(
+        title='Конфигурация журнала обмена',
+        default=None
+    )
 
     id: int = 1
 
     def validate(self):
         errors = []
 
         for field_name in (
@@ -103,14 +115,23 @@
         ):
             if not getattr(self, field_name):
                 errors.append(
                     'Не заполнено поле '
                     f'"{getattr(type(self), field_name).title}"'
                 )
 
+        if (
+            self.journal == 'adapter_client.adapters.smev.logging.opensearch.OpenSearchJournal' and
+            not all((
+                self.journal_config.get('opensearch_address'), self.journal_config.get('opensearch_index_name'),
+                self.journal_config.get('opensearch_username'), self.journal_config.get('opensearch_password')
+            ))
+        ):
+            errors.append('Не произведена настройка OpenSearch')
+
         if errors:
             raise ConfigNotValid('\n'.join(errors), self)
 
 
 class NamedIntEnum(Enum):
     def __init__(self, id_: int, verbose: str) -> None:
         self.id = id_
@@ -250,14 +271,15 @@
 class JournalEntry:
     address: str = Field(
         title='Адрес запроса',
         default=None,
     )
     timestamp: datetime = Field(
         title='Дата отправки',
+        default_factory=lambda: datetime.now().astimezone()
     )
     type: RequestType = Field(
         title='Тип запроса'
     )
     request: str = Field(
         title='Запрос',
         default=None,
@@ -270,10 +292,11 @@
         title='Ошибка',
         default=None,
     )
     message: Message = Field(
         title='Сообщение',
         default=None,
     )
-    id: str = Field(
+    id: Optional[str] = Field(
         title='Идентификатор записи журнала',
+        default=None
     )
```

### Comparing `adapter-client-1.1.0/src/adapter_client/migrations/0001_initial.py` & `adapter-client-1.2.0/src/adapter_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/src/adapter_client/models.py` & `adapter-client-1.2.0/src/adapter_client/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,14 +70,47 @@
             MinValueValidator(1),
             MaxValueValidator(6000)
         ],
         default=30,
         help_text='сек',
         null=True, blank=True
     )
+    request_timeout_sec = models.IntegerField(
+        verbose_name=model.Config.request_timeout_sec.title,
+        default=model.Config.request_timeout_sec.default,
+        null=True, blank=True
+    )
+    adapter_interface = models.CharField(
+        verbose_name=model.Config.adapter_interface.title,
+        default=model.Config.adapter_interface.default,
+        max_length=200,
+        null=True, blank=True
+    )
+    incoming_message_repository = models.CharField(
+        verbose_name=model.Config.incoming_message_repository.title,
+        default=model.Config.incoming_message_repository.default,
+        max_length=200,
+        null=True, blank=True
+    )
+    outgoing_message_repository = models.CharField(
+        verbose_name=model.Config.outgoing_message_repository.title,
+        default=model.Config.outgoing_message_repository.default,
+        max_length=200,
+        null=True, blank=True
+    )
+    journal = models.CharField(
+        verbose_name=model.Config.journal.title,
+        default=model.Config.journal.default,
+        max_length=200,
+        null=True, blank=True
+    )
+    journal_config = JSONField(
+        verbose_name=model.Config.journal_config.title,
+        null=True, blank=True
+    )
 
 
 class Message(models.Model):
 
     class Meta:
         verbose_name = 'Сообщение'
         verbose_name_plural = 'Сообщения'
```

### Comparing `adapter-client-1.1.0/src/adapter_client/tasks.py` & `adapter-client-1.2.0/src/adapter_client/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,27 +76,33 @@
 class GetTask(task_base):
 
     description = 'Обработка сообщений в РИС (Get)'
 
     def run(self, *args, **kwargs):
         super().run(*args, **kwargs)
         success_count = fail_count = 0
-        for res in adapter.get_pending():
-            if res.status is model.IncomingStatus.processed:
-                success_count += 1
-            else:
-                fail_count += 1
+
+        res = adapter.get_pending()
+
+        if (
+            res.message_metadata and
+            res.message_metadata.status is model.IncomingStatus.processed
+        ):
+            success_count += 1
+        else:
+            fail_count += 1
+
         logger.info(
             'Обработано сообщений в РИС: успешно %d, c ошибкой %d',
             success_count,
             fail_count,
         )
 
 
-process_task = register_task(GetTask())
+get_task = register_task(GetTask())
 
 
 class FindTask(task_base):
 
     description = 'Получение ответов на сообщения от Адаптера СМЭВ'
 
     def run(self, *args, **kwargs):
@@ -143,14 +149,15 @@
     """Настройка фоновых задач."""
 
     logger.info('Configuring periodic tasks...')
 
     config = config or services.load_config()
 
     for task_cls, retry_time in (
+        (GetTask, config.get_request_retry_time),
         (SendTask, config.send_request_retry_time),
         (FindTask, config.find_request_retry_time),
         (ProcessTask, config.find_request_retry_time),
     ):
         schedule, _ = IntervalSchedule.objects.get_or_create(
             every=retry_time,
             period=IntervalSchedule.SECONDS,
```

### Comparing `adapter-client-1.1.0/src/adapter_client/utils.py` & `adapter-client-1.2.0/src/adapter_client/utils.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.1.0/src/adapter_client.egg-info/PKG-INFO` & `adapter-client-1.2.0/src/adapter_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: adapter-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
+Provides-Extra: opensearch
 
 # Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 ## Подключение
 settings:
 
     INSTALLED_APPS = [
         'adapter_client'
```

### Comparing `adapter-client-1.1.0/src/adapter_client.egg-info/SOURCES.txt` & `adapter-client-1.2.0/src/adapter_client.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,19 @@
 src/adapter_client/adapters/smev/interfaces/__init__.py
 src/adapter_client/adapters/smev/interfaces/base.py
 src/adapter_client/adapters/smev/interfaces/soap/__init__.py
 src/adapter_client/adapters/smev/interfaces/soap/interface.py
 src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl
 src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd
 src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd
+src/adapter_client/adapters/smev/logging/__init__.py
+src/adapter_client/adapters/smev/logging/opensearch.py
 src/adapter_client/adapters/smev/services/__init__.py
 src/adapter_client/adapters/smev/services/base.py
 src/adapter_client/adapters/smev/services/registry.py
 src/adapter_client/core/__init__.py
 src/adapter_client/core/services.py
 src/adapter_client/core/domain/__init__.py
 src/adapter_client/core/domain/model.py
 src/adapter_client/migrations/0001_initial.py
+src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py
 src/adapter_client/migrations/__init__.py
```

