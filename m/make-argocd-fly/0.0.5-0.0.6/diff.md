# Comparing `tmp/make_argocd_fly-0.0.5.tar.gz` & `tmp/make_argocd_fly-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make_argocd_fly-0.0.5.tar", last modified: Wed Jul  5 19:59:00 2023, max compression
+gzip compressed data, was "make_argocd_fly-0.0.6.tar", last modified: Thu Jul  6 05:25:42 2023, max compression
```

## Comparing `make_argocd_fly-0.0.5.tar` & `make_argocd_fly-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-05 19:59:00.213299 make_argocd_fly-0.0.5/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.5/LICENSE
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.5/MANIFEST.in
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2657 2023-07-05 19:59:00.213299 make_argocd_fly-0.0.5/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2303 2023-07-05 19:52:03.000000 make_argocd_fly-0.0.5/README.md
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-05 19:59:00.203298 make_argocd_fly-0.0.5/make_argocd_fly/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.5/make_argocd_fly/__init__.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.5/make_argocd_fly/config.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.5/make_argocd_fly/log_config.yml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5535 2023-07-04 20:47:34.000000 make_argocd_fly-0.0.5/make_argocd_fly/pipeline.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4243 2023-07-04 20:45:25.000000 make_argocd_fly-0.0.5/make_argocd_fly/resource.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      856 2023-07-04 20:39:27.000000 make_argocd_fly-0.0.5/make_argocd_fly/utils.py
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-05 19:59:00.213299 make_argocd_fly-0.0.5/make_argocd_fly.egg-info/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2657 2023-07-05 19:59:00.000000 make_argocd_fly-0.0.5/make_argocd_fly.egg-info/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      463 2023-07-05 19:59:00.000000 make_argocd_fly-0.0.5/make_argocd_fly.egg-info/SOURCES.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-05 19:59:00.000000 make_argocd_fly-0.0.5/make_argocd_fly.egg-info/dependency_links.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-05 19:59:00.000000 make_argocd_fly-0.0.5/make_argocd_fly.egg-info/entry_points.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-05 19:59:00.000000 make_argocd_fly-0.0.5/make_argocd_fly.egg-info/requires.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-05 19:59:00.000000 make_argocd_fly-0.0.5/make_argocd_fly.egg-info/top_level.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      724 2023-07-05 19:58:51.000000 make_argocd_fly-0.0.5/pyproject.toml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.5/requirements.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-05 19:59:00.213299 make_argocd_fly-0.0.5/setup.cfg
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-06 05:25:42.458487 make_argocd_fly-0.0.6/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.6/LICENSE
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.6/MANIFEST.in
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2657 2023-07-06 05:25:42.458487 make_argocd_fly-0.0.6/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2303 2023-07-06 05:25:22.000000 make_argocd_fly-0.0.6/README.md
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-06 05:25:42.458487 make_argocd_fly-0.0.6/make_argocd_fly/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.6/make_argocd_fly/__init__.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.6/make_argocd_fly/config.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.6/make_argocd_fly/log_config.yml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5535 2023-07-04 20:47:34.000000 make_argocd_fly-0.0.6/make_argocd_fly/pipeline.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4243 2023-07-04 20:45:25.000000 make_argocd_fly-0.0.6/make_argocd_fly/resource.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      856 2023-07-04 20:39:27.000000 make_argocd_fly-0.0.6/make_argocd_fly/utils.py
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-06 05:25:42.458487 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2657 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      463 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/SOURCES.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/dependency_links.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/entry_points.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/requires.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-06 05:25:42.000000 make_argocd_fly-0.0.6/make_argocd_fly.egg-info/top_level.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      724 2023-07-06 05:21:09.000000 make_argocd_fly-0.0.6/pyproject.toml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.6/requirements.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-06 05:25:42.458487 make_argocd_fly-0.0.6/setup.cfg
```

### Comparing `make_argocd_fly-0.0.5/LICENSE` & `make_argocd_fly-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.5/PKG-INFO` & `make_argocd_fly-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make_argocd_fly
-Version: 0.0.5
+Version: 0.0.6
 Summary: A project to generate ArgoCD application resources
 Author-email: Andrei Lapin <karandash8@gmail.com>
 License: GPLv3+
 Keywords: argocd,kustomize,jinja2
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -38,44 +38,41 @@
 
 vars:
   var_1:
     var_2: value_2
   var_3: value_3
 ```
 
+With such configuration file you can have kustomize overlays for `dev/stage/prod` and jinja2 variables like `{{ var_1.var_2 }} and {{ var_3 }}` in your source files.
+
 ## Caveats
 ### Currently supported directory structure
 ```
 repo
   source
     app_1
       base
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
       dev
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
       stage
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
       prod
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
     app_2
-      yaml.yml
-      kustomization.yml
+      yaml.yml(.j2)
+      kustomization.yml(.j2)
     app_3
-      yaml.yml.j2
-      kustomization.yml.j2
-    app_4
-      yaml.yml
+      yaml.yml(.j2)
 ```
 
-With such configuration file you can have kustomize overlays for `dev/stage/prod` and jinja2 variables like `{{ var_1.var_2 }} and {{ var_3 }}` in your source files.
-
 ### kustomization.yml
 Files referenced in the `resources` section shall be named after Kubernetes resource types with lower case letters as a single word. Example:
 
 ```
 resources:
   - deployment.yml
   - serviceaccount.yml
```

### Comparing `make_argocd_fly-0.0.5/README.md` & `make_argocd_fly-0.0.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -26,44 +26,41 @@
 
 vars:
   var_1:
     var_2: value_2
   var_3: value_3
 ```
 
+With such configuration file you can have kustomize overlays for `dev/stage/prod` and jinja2 variables like `{{ var_1.var_2 }} and {{ var_3 }}` in your source files.
+
 ## Caveats
 ### Currently supported directory structure
 ```
 repo
   source
     app_1
       base
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
       dev
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
       stage
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
       prod
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
     app_2
-      yaml.yml
-      kustomization.yml
+      yaml.yml(.j2)
+      kustomization.yml(.j2)
     app_3
-      yaml.yml.j2
-      kustomization.yml.j2
-    app_4
-      yaml.yml
+      yaml.yml(.j2)
 ```
 
-With such configuration file you can have kustomize overlays for `dev/stage/prod` and jinja2 variables like `{{ var_1.var_2 }} and {{ var_3 }}` in your source files.
-
 ### kustomization.yml
 Files referenced in the `resources` section shall be named after Kubernetes resource types with lower case letters as a single word. Example:
 
 ```
 resources:
   - deployment.yml
   - serviceaccount.yml
```

### Comparing `make_argocd_fly-0.0.5/make_argocd_fly/config.py` & `make_argocd_fly-0.0.6/make_argocd_fly/config.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.5/make_argocd_fly/pipeline.py` & `make_argocd_fly-0.0.6/make_argocd_fly/pipeline.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.5/make_argocd_fly/resource.py` & `make_argocd_fly-0.0.6/make_argocd_fly/resource.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.5/make_argocd_fly/utils.py` & `make_argocd_fly-0.0.6/make_argocd_fly/utils.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.5/make_argocd_fly.egg-info/PKG-INFO` & `make_argocd_fly-0.0.6/make_argocd_fly.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make-argocd-fly
-Version: 0.0.5
+Version: 0.0.6
 Summary: A project to generate ArgoCD application resources
 Author-email: Andrei Lapin <karandash8@gmail.com>
 License: GPLv3+
 Keywords: argocd,kustomize,jinja2
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -38,44 +38,41 @@
 
 vars:
   var_1:
     var_2: value_2
   var_3: value_3
 ```
 
+With such configuration file you can have kustomize overlays for `dev/stage/prod` and jinja2 variables like `{{ var_1.var_2 }} and {{ var_3 }}` in your source files.
+
 ## Caveats
 ### Currently supported directory structure
 ```
 repo
   source
     app_1
       base
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
       dev
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
       stage
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
       prod
-        yaml.yml
-        kustomization.yml
+        yaml.yml(.j2)
+        kustomization.yml(.j2)
     app_2
-      yaml.yml
-      kustomization.yml
+      yaml.yml(.j2)
+      kustomization.yml(.j2)
     app_3
-      yaml.yml.j2
-      kustomization.yml.j2
-    app_4
-      yaml.yml
+      yaml.yml(.j2)
 ```
 
-With such configuration file you can have kustomize overlays for `dev/stage/prod` and jinja2 variables like `{{ var_1.var_2 }} and {{ var_3 }}` in your source files.
-
 ### kustomization.yml
 Files referenced in the `resources` section shall be named after Kubernetes resource types with lower case letters as a single word. Example:
 
 ```
 resources:
   - deployment.yml
   - serviceaccount.yml
```

### Comparing `make_argocd_fly-0.0.5/pyproject.toml` & `make_argocd_fly-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "make_argocd_fly"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name = "Andrei Lapin", email = "karandash8@gmail.com"},
 ]
 description = "A project to generate ArgoCD application resources"
 requires-python = ">=3.10"
 keywords = ["argocd", "kustomize", "jinja2"]
 license = {text = "GPLv3+"}
```

