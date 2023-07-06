# Comparing `tmp/django_tailwind_cli-1.4.3.tar.gz` & `tmp/django_tailwind_cli-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwind_cli-1.4.3.tar", max compression
+gzip compressed data, was "django_tailwind_cli-1.5.0.tar", max compression
```

## Comparing `django_tailwind_cli-1.4.3.tar` & `django_tailwind_cli-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/LICENSE
--rw-r--r--   0        0        0     2836 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/README.md
--rw-r--r--   0        0        0     2725 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/pyproject.toml
--rw-r--r--   0        0        0       78 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0      168 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0     4712 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0       79 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/styles.css
--rw-r--r--   0        0        0      436 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/tailwind.config.js
--rw-r--r--   0        0        0      518 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      257 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      463 2023-04-10 14:22:18.821436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0     2961 2023-04-10 14:22:18.821436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 django_tailwind_cli-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2836 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/README.md
+-rw-r--r--   0        0        0     2725 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0     5736 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0       79 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/styles.css
+-rw-r--r--   0        0        0      436 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/tailwind.config.js
+-rw-r--r--   0        0        0      518 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      257 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      463 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0     2961 2023-07-06 11:39:40.665351 django_tailwind_cli-1.5.0/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 django_tailwind_cli-1.5.0/PKG-INFO
```

### Comparing `django_tailwind_cli-1.4.3/LICENSE` & `django_tailwind_cli-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-1.4.3/README.md` & `django_tailwind_cli-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-1.4.3/pyproject.toml` & `django_tailwind_cli-1.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-tailwind-cli"
-version = "1.4.3"
+version = "1.5.0"
 description = "Django and Tailwind integration based on the prebuilt Tailwind CSS CLI."
 license = "MIT"
 authors = ["Oliver Andrich <oliver@andrich.me>"]
 readme = "README.md"
 homepage = "https://oliverandrich.github.io/django-tailwind-cli/"
 repository = "https://github.com/oliverandrich/django-tailwind-cli"
 keywords = ["django", "tailwind", "css"]
```

### Comparing `django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/commands/tailwind.py` & `django_tailwind_cli-1.5.0/src/django_tailwind_cli/management/commands/tailwind.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 """`tailwind` management command."""
 
 import shutil
 import subprocess
+import sys
 from importlib.util import find_spec
+from multiprocessing import Process, Queue
 from pathlib import Path
-from typing import Any
+from typing import Any, Sequence
 
 from django.conf import settings
-
-# We need to import click and djclick to make pyright happy
 from django.core.management.base import CommandError, LabelCommand
 from django_rich.management import RichCommand
 
 from django_tailwind_cli.utils import (
     download_file,
     get_config,
     get_dist_css_path,
     get_download_url,
     get_executable_path,
     get_src_css_path,
     get_theme_app_path,
 )
 
 
+def _run_process(cmd: Sequence[str], queue: "Queue[str]") -> None:
+    with subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True) as process:
+        if process.stdout is not None:
+            for line in process.stdout:
+                if line:
+                    queue.put(line)
+
+
 class Command(RichCommand, LabelCommand):
     """Create and manage a Tailwind CSS theme."""
 
     def handle_label(self, label: str, **options: Any) -> None:
         """Perform the command's actions for ``label``, which will be the string as given on the command line."""
         if label == "installcli":
             self.installcli()
         elif label == "init":
             self.init_theme_app()
         elif label == "build":
             self.build()
         elif label == "watch":
             self.watch()
+        elif label == "runserver":
+            self.runserver()
         else:
             raise CommandError(f"Unsupported subcommand `{label}` called.")
 
     def installcli(self):
         """Install the Tailwind CSS cli in the version defined by TAILWIND_VERSION."""
 
         # build path for cli
@@ -128,7 +138,27 @@
                 "--output",
                 str(get_dist_css_path()),
                 "--watch",
             ],
             cwd=get_theme_app_path(),
             check=True,
         )
+
+    def runserver(self):
+        """Start the Django development server and the tailwind cli in watch mode."""
+
+        q: Queue[str] = Queue()
+
+        p1 = Process(target=_run_process, args=([sys.executable, "manage.py", "runserver", "--no-color"], q))
+        p1.start()
+        p2 = Process(target=_run_process, args=([sys.executable, "manage.py", "tailwind", "watch"], q))
+        p2.start()
+
+        while True:
+            line = q.get()
+            if line:
+                self.console.print(line.strip())
+            if not p1.is_alive() or not p2.is_alive():
+                break
+
+        p1.join()
+        p2.join()
```

### Comparing `django_tailwind_cli-1.4.3/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-1.5.0/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-1.4.3/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-1.5.0/src/django_tailwind_cli/utils.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-1.4.3/PKG-INFO` & `django_tailwind_cli-1.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tailwind-cli
-Version: 1.4.3
+Version: 1.5.0
 Summary: Django and Tailwind integration based on the prebuilt Tailwind CSS CLI.
 Home-page: https://oliverandrich.github.io/django-tailwind-cli/
 License: MIT
 Keywords: django,tailwind,css
 Author: Oliver Andrich
 Author-email: oliver@andrich.me
 Requires-Python: >=3.8.1,<4
@@ -17,18 +17,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Dist: certifi
 Requires-Dist: django (>=3.2,<5)
 Requires-Dist: django-rich (>=1.5.0,<2.0.0)
 Project-URL: Mastodon, https://2pxnl.de/@oliver
 Project-URL: Repository, https://github.com/oliverandrich/django-tailwind-cli
```

