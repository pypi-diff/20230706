# Comparing `tmp/vps-deploy-1.0.0.tar.gz` & `tmp/vps-deploy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vps-deploy-1.0.0.tar", last modified: Wed Apr 12 00:07:46 2023, max compression
+gzip compressed data, was "vps-deploy-1.1.0.tar", last modified: Thu Jul  6 01:10:07 2023, max compression
```

## Comparing `vps-deploy-1.0.0.tar` & `vps-deploy-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ben       (1000) users      (998)        0 2023-04-12 00:07:46.754970 vps-deploy-1.0.0/
--rw-r--r--   0 ben       (1000) users      (998)    35061 2017-10-16 01:30:57.000000 vps-deploy-1.0.0/COPYING
--rw-r--r--   0 ben       (1000) users      (998)     2985 2023-04-12 00:04:29.000000 vps-deploy-1.0.0/HISTORY.rst
--rw-r--r--   0 ben       (1000) users      (998)     7370 2023-04-12 00:07:46.754970 vps-deploy-1.0.0/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (998)     3842 2020-08-10 04:24:14.000000 vps-deploy-1.0.0/README.rst
--rw-r--r--   0 ben       (1000) users      (998)      103 2021-09-20 12:04:15.000000 vps-deploy-1.0.0/pyproject.toml
--rw-r--r--   0 ben       (1000) users      (998)      697 2023-04-12 00:07:46.754970 vps-deploy-1.0.0/setup.cfg
--rw-r--r--   0 ben       (1000) users      (998)       38 2021-09-20 12:04:37.000000 vps-deploy-1.0.0/setup.py
-drwxr-xr-x   0 ben       (1000) users      (998)        0 2023-04-12 00:07:46.754970 vps-deploy-1.0.0/vps_deploy/
--rw-r--r--   0 ben       (1000) users      (998)        0 2017-10-16 01:30:57.000000 vps-deploy-1.0.0/vps_deploy/__init__.py
--rw-r--r--   0 ben       (1000) users      (998)    12564 2023-03-08 23:51:43.000000 vps-deploy-1.0.0/vps_deploy/django_fabric2.py
-drwxr-xr-x   0 ben       (1000) users      (998)        0 2023-04-12 00:07:46.754970 vps-deploy-1.0.0/vps_deploy.egg-info/
--rw-r--r--   0 ben       (1000) users      (998)     7370 2023-04-12 00:07:46.000000 vps-deploy-1.0.0/vps_deploy.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (998)      285 2023-04-12 00:07:46.000000 vps-deploy-1.0.0/vps_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) users      (998)        1 2023-04-12 00:07:46.000000 vps-deploy-1.0.0/vps_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) users      (998)       74 2023-04-12 00:07:46.000000 vps-deploy-1.0.0/vps_deploy.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) users      (998)       11 2023-04-12 00:07:46.000000 vps-deploy-1.0.0/vps_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1000) users      (998)        0 2023-07-06 01:10:07.688919 vps-deploy-1.1.0/
+-rw-r--r--   0 ben       (1000) users      (998)    35061 2017-10-16 01:30:57.000000 vps-deploy-1.1.0/COPYING
+-rw-r--r--   0 ben       (1000) users      (998)     3161 2023-07-06 01:07:27.000000 vps-deploy-1.1.0/HISTORY.rst
+-rw-r--r--   0 ben       (1000) users      (998)     6855 2023-07-06 01:10:07.688919 vps-deploy-1.1.0/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (998)     3151 2023-07-06 00:05:06.000000 vps-deploy-1.1.0/README.rst
+-rw-r--r--   0 ben       (1000) users      (998)      103 2021-09-20 12:04:15.000000 vps-deploy-1.1.0/pyproject.toml
+-rw-r--r--   0 ben       (1000) users      (998)      679 2023-07-06 01:10:07.692919 vps-deploy-1.1.0/setup.cfg
+-rw-r--r--   0 ben       (1000) users      (998)       38 2021-09-20 12:04:37.000000 vps-deploy-1.1.0/setup.py
+drwxr-xr-x   0 ben       (1000) users      (998)        0 2023-07-06 01:10:07.688919 vps-deploy-1.1.0/vps_deploy/
+-rw-r--r--   0 ben       (1000) users      (998)        0 2017-10-16 01:30:57.000000 vps-deploy-1.1.0/vps_deploy/__init__.py
+-rw-r--r--   0 ben       (1000) users      (998)    12551 2023-07-06 01:08:47.000000 vps-deploy-1.1.0/vps_deploy/django_fabric2.py
+drwxr-xr-x   0 ben       (1000) users      (998)        0 2023-07-06 01:10:07.688919 vps-deploy-1.1.0/vps_deploy.egg-info/
+-rw-r--r--   0 ben       (1000) users      (998)     6855 2023-07-06 01:10:07.000000 vps-deploy-1.1.0/vps_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (998)      285 2023-07-06 01:10:07.000000 vps-deploy-1.1.0/vps_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) users      (998)        1 2023-07-06 01:10:07.000000 vps-deploy-1.1.0/vps_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) users      (998)       57 2023-07-06 01:10:07.000000 vps-deploy-1.1.0/vps_deploy.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) users      (998)       11 2023-07-06 01:10:07.000000 vps-deploy-1.1.0/vps_deploy.egg-info/top_level.txt
```

### Comparing `vps-deploy-1.0.0/COPYING` & `vps-deploy-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `vps-deploy-1.0.0/HISTORY.rst` & `vps-deploy-1.1.0/HISTORY.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Release History
 ---------------
 
+1.1.0 (2023-07-06)
+++++++++++++++++++
+
+ - drop dependency on patchwork due to version conflict with Python
+   3.11-compatible version of invoke
+ - remove docs about Fabric 1
+
+
 1.0.0 (2023-04-12)
 ++++++++++++++++++
 
  - remove Python 2 support
  - also look for ``breakpoint`` (Python 3.7) when checking for debugger calls
  - make ``sudo_upload_template`` function part of public API
  - use ``mktemp`` instead of deprecated ``tempfile``
```

### Comparing `vps-deploy-1.0.0/PKG-INFO` & `vps-deploy-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vps-deploy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Common commands for deployment on a VPS.
 Home-page: https://gitlab.com/sturm/vps-deploy
 Author: Ben Sturmfels
 Author-email: ben@sturm.com.au
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -13,17 +13,16 @@
 Requires-Python: >=3.6
 License-File: COPYING
 
 ==========
 VPS Deploy
 ==========
 
-This is a base set of Fabric deployment functions for projects based on Django,
-Nginx, uWSGI Emperor, Memcached and PostgreSQL. Both Fabric 2 and legacy Fabric
-1 systems are supported.
+This is a base set of Fabric 2 deployment functions for projects based on
+Django, Nginx, uWSGI Emperor, Memcached and PostgreSQL.
 
 Fabric is a handy tool for automating deployment processes. Unlike Salt or
 Ansible, you're writing code from the beginning rather than diving into a Turing
 Tarpit of templated YAML. Also unlike Salt, Ansible or shell scripts, Fabric
 neatly coordinates both local and remote SSH tasks. While Fabric may not be your
 best choice for provisioning, it works well as a simple and flexible tool for
 automatic custom workflows.
@@ -38,34 +37,14 @@
   $ pip install --user vps-deploy
 
 Otherwise::
 
   $ pip install --user fabric invoke vps-deploy
 
 
-Legacy installation for Fabric 1.*
-----------------------------------
-
-Fabric 1.* is recommended only for supporting existing projects. For new
-projects, use Fabric 2.*.
-
-Since Fabric 1.* is Python 2-only and you're probably using a Python 3 virtual
-env, you'll need to install Fabric and VPS Deploy as a `--user` package::
-
-  # System package for Fabric, user package for vps-deploy:
-  $ sudo apt install fabric
-  $ pip install --user vps-deploy
-
-  # All in user packages:
-  $ pip install --user fabric~=1.14 vps-deploy
-
-Alternately, while Fabric 1.* remains available for some operating systems, you
-could also install it that way.
-
-
 Getting started
 ---------------
 
 To get started, create a `fabfile.py` in your top-level project directory. It
 might look something like this:
 
 .. code:: python
@@ -140,14 +119,22 @@
 server and having the server-site software and accounts set up. Those tend to to
 be better handled with configuration management tools like Salt or Ansible (and
 potentially triggered by Fabric!).
 
 Release History
 ---------------
 
+1.1.0 (2023-07-06)
+++++++++++++++++++
+
+ - drop dependency on patchwork due to version conflict with Python
+   3.11-compatible version of invoke
+ - remove docs about Fabric 1
+
+
 1.0.0 (2023-04-12)
 ++++++++++++++++++
 
  - remove Python 2 support
  - also look for ``breakpoint`` (Python 3.7) when checking for debugger calls
  - make ``sudo_upload_template`` function part of public API
  - use ``mktemp`` instead of deprecated ``tempfile``
```

### Comparing `vps-deploy-1.0.0/README.rst` & `vps-deploy-1.1.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 ==========
 VPS Deploy
 ==========
 
-This is a base set of Fabric deployment functions for projects based on Django,
-Nginx, uWSGI Emperor, Memcached and PostgreSQL. Both Fabric 2 and legacy Fabric
-1 systems are supported.
+This is a base set of Fabric 2 deployment functions for projects based on
+Django, Nginx, uWSGI Emperor, Memcached and PostgreSQL.
 
 Fabric is a handy tool for automating deployment processes. Unlike Salt or
 Ansible, you're writing code from the beginning rather than diving into a Turing
 Tarpit of templated YAML. Also unlike Salt, Ansible or shell scripts, Fabric
 neatly coordinates both local and remote SSH tasks. While Fabric may not be your
 best choice for provisioning, it works well as a simple and flexible tool for
 automatic custom workflows.
@@ -23,34 +22,14 @@
   $ pip install --user vps-deploy
 
 Otherwise::
 
   $ pip install --user fabric invoke vps-deploy
 
 
-Legacy installation for Fabric 1.*
-----------------------------------
-
-Fabric 1.* is recommended only for supporting existing projects. For new
-projects, use Fabric 2.*.
-
-Since Fabric 1.* is Python 2-only and you're probably using a Python 3 virtual
-env, you'll need to install Fabric and VPS Deploy as a `--user` package::
-
-  # System package for Fabric, user package for vps-deploy:
-  $ sudo apt install fabric
-  $ pip install --user vps-deploy
-
-  # All in user packages:
-  $ pip install --user fabric~=1.14 vps-deploy
-
-Alternately, while Fabric 1.* remains available for some operating systems, you
-could also install it that way.
-
-
 Getting started
 ---------------
 
 To get started, create a `fabfile.py` in your top-level project directory. It
 might look something like this:
 
 .. code:: python
```

### Comparing `vps-deploy-1.0.0/vps_deploy/django_fabric2.py` & `vps-deploy-1.1.0/vps_deploy/django_fabric2.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 import datetime
 import io
 import sys
 import os
 
 import invoke
 from jinja2 import Template
-from patchwork.files import exists
 
 
 def transfer_files_git(c, push_to_origin=True):
     if push_to_origin:
         c.local(f'git push origin {c.env.branch}')
     c.sudo(f'mkdir -p {c.env.project_dir}')
     c.sudo(f'chown {c.user} {c.env.project_dir}')
@@ -63,25 +62,25 @@
         c.run('git config receive.denyCurrentBranch ignore')
         c.run(f'git fetch origin {c.env.branch}')
         c.run(f'git reset --hard origin/{c.env.branch}')
 
 
 def init(c):
     """Misc first-time run things."""
-    if not exists(c, f'{c.env.project_dir}/env'):
+    if not c.run(f'test -e {c.env.project_dir}/env'):
         c.run(f'touch {c.env.project_dir}/env')
     media_dir = os.path.join(c.env.project_dir, c.env.media_dir)
-    if not exists(c, media_dir):
+    if not c.run(f'test -e {media_dir}'):
         c.run(f'mkdir -p {media_dir}')
 
 
 def prepare_virtualenv(c, pip_install_options=''):
     """Initialise a virtualenv and install required Python modules."""
 
-    if not exists(c, c.env.virtualenv):
+    if not c.run(f'test -e {c.env.virtualenv}'):
         c.sudo(f"mkdir -p $(dirname {c.env.virtualenv})")
         c.sudo(f'chown {c.user} $(dirname {c.env.virtualenv})')
 
         c.run("{env.python} -m venv --system-site-packages {env.virtualenv}".format(env=c.env))
     with c.cd(c.env.project_dir):
         c.run("{env.virtualenv}/bin/python -m pip install -r {env.requirements} {pip_install_options}".format(
             env=c.env, pip_install_options=pip_install_options))
```

### Comparing `vps-deploy-1.0.0/vps_deploy.egg-info/PKG-INFO` & `vps-deploy-1.1.0/vps_deploy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vps-deploy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Common commands for deployment on a VPS.
 Home-page: https://gitlab.com/sturm/vps-deploy
 Author: Ben Sturmfels
 Author-email: ben@sturm.com.au
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -13,17 +13,16 @@
 Requires-Python: >=3.6
 License-File: COPYING
 
 ==========
 VPS Deploy
 ==========
 
-This is a base set of Fabric deployment functions for projects based on Django,
-Nginx, uWSGI Emperor, Memcached and PostgreSQL. Both Fabric 2 and legacy Fabric
-1 systems are supported.
+This is a base set of Fabric 2 deployment functions for projects based on
+Django, Nginx, uWSGI Emperor, Memcached and PostgreSQL.
 
 Fabric is a handy tool for automating deployment processes. Unlike Salt or
 Ansible, you're writing code from the beginning rather than diving into a Turing
 Tarpit of templated YAML. Also unlike Salt, Ansible or shell scripts, Fabric
 neatly coordinates both local and remote SSH tasks. While Fabric may not be your
 best choice for provisioning, it works well as a simple and flexible tool for
 automatic custom workflows.
@@ -38,34 +37,14 @@
   $ pip install --user vps-deploy
 
 Otherwise::
 
   $ pip install --user fabric invoke vps-deploy
 
 
-Legacy installation for Fabric 1.*
-----------------------------------
-
-Fabric 1.* is recommended only for supporting existing projects. For new
-projects, use Fabric 2.*.
-
-Since Fabric 1.* is Python 2-only and you're probably using a Python 3 virtual
-env, you'll need to install Fabric and VPS Deploy as a `--user` package::
-
-  # System package for Fabric, user package for vps-deploy:
-  $ sudo apt install fabric
-  $ pip install --user vps-deploy
-
-  # All in user packages:
-  $ pip install --user fabric~=1.14 vps-deploy
-
-Alternately, while Fabric 1.* remains available for some operating systems, you
-could also install it that way.
-
-
 Getting started
 ---------------
 
 To get started, create a `fabfile.py` in your top-level project directory. It
 might look something like this:
 
 .. code:: python
@@ -140,14 +119,22 @@
 server and having the server-site software and accounts set up. Those tend to to
 be better handled with configuration management tools like Salt or Ansible (and
 potentially triggered by Fabric!).
 
 Release History
 ---------------
 
+1.1.0 (2023-07-06)
+++++++++++++++++++
+
+ - drop dependency on patchwork due to version conflict with Python
+   3.11-compatible version of invoke
+ - remove docs about Fabric 1
+
+
 1.0.0 (2023-04-12)
 ++++++++++++++++++
 
  - remove Python 2 support
  - also look for ``breakpoint`` (Python 3.7) when checking for debugger calls
  - make ``sudo_upload_template`` function part of public API
  - use ``mktemp`` instead of deprecated ``tempfile``
```

