# Comparing `tmp/cici-tools-0.2.5.tar.gz` & `tmp/cici-tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cici-tools-0.2.5.tar", last modified: Sun Jul  2 22:15:39 2023, max compression
+gzip compressed data, was "cici-tools-0.3.0.tar", last modified: Thu Jul  6 05:19:26 2023, max compression
```

## Comparing `cici-tools-0.2.5.tar` & `cici-tools-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.244760 cici-tools-0.2.5/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-02 22:15:36.000000 cici-tools-0.2.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-02 22:15:36.000000 cici-tools-0.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2689 2023-07-02 22:15:39.244760 cici-tools-0.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1856 2023-07-02 22:15:36.000000 cici-tools-0.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.240760 cici-tools-0.2.5/cici/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.241760 cici-tools-0.2.5/cici/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/cli/_build.py
--rwxrwxrwx   0 root         (0) root         (0)     3088 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/cli/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/cli/fmt.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/cli/update.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.241760 cici-tools-0.2.5/cici/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.242760 cici-tools-0.2.5/cici/providers/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     5760 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/converter.py
--rw-rw-rw-   0 root         (0) root         (0)     6415 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3091 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.243760 cici-tools-0.2.5/cici/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/schema/LICENSE.gitlab
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    70638 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/schema/gitlab-ci.json
--rw-rw-rw-   0 root         (0) root         (0)     1829 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.244760 cici-tools-0.2.5/cici_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2689 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      753 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-02 22:15:39.245760 cici-tools-0.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1360 2023-07-02 22:15:36.000000 cici-tools-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 05:19:26.762578 cici-tools-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-06 05:19:24.000000 cici-tools-0.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-06 05:19:24.000000 cici-tools-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-07-06 05:19:26.762578 cici-tools-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-07-06 05:19:24.000000 cici-tools-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 05:19:26.759578 cici-tools-0.3.0/cici/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 05:19:26.759578 cici-tools-0.3.0/cici/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/cli/_build.py
+-rwxrwxrwx   0 root         (0) root         (0)     1973 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/cli/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/cli/fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/cli/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 05:19:26.760578 cici-tools-0.3.0/cici/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 05:19:26.760578 cici-tools-0.3.0/cici/providers/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/providers/gitlab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/providers/gitlab/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     5760 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/providers/gitlab/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/providers/gitlab/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3091 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/providers/gitlab/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/providers/gitlab/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 05:19:26.761578 cici-tools-0.3.0/cici/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/schema/LICENSE.gitlab
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70638 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/schema/gitlab-ci.json
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-07-06 05:19:24.000000 cici-tools-0.3.0/cici/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 05:19:26.762578 cici-tools-0.3.0/cici_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-07-06 05:19:26.000000 cici-tools-0.3.0/cici_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      753 2023-07-06 05:19:26.000000 cici-tools-0.3.0/cici_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 05:19:26.000000 cici-tools-0.3.0/cici_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-06 05:19:26.000000 cici-tools-0.3.0/cici_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-06 05:19:26.000000 cici-tools-0.3.0/cici_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-06 05:19:26.000000 cici-tools-0.3.0/cici_tools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-06 05:19:26.763578 cici-tools-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1360 2023-07-06 05:19:24.000000 cici-tools-0.3.0/setup.py
```

### Comparing `cici-tools-0.2.5/LICENSE` & `cici-tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/PKG-INFO` & `cici-tools-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici-tools
-Version: 0.2.5
+Version: 0.3.0
 Summary: Power tools for CI/CD.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
```

### Comparing `cici-tools-0.2.5/README.md` & `cici-tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/cli/_build.py` & `cici-tools-0.3.0/cici/cli/_build.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/cli/bundle.py` & `cici-tools-0.3.0/cici/cli/bundle.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,51 @@
 import copy
 import logging
+import re
 from importlib import import_module
 from pathlib import Path
-from typing import Optional
 
 from termcolor import colored
 
+from .._version import __version__
 from ..constants import CONFIG_DIR_NAME, DEFAULT_PROVIDER
 
 
-def get_job_prefix(pipeline_name: str, job_name: str) -> Optional[str]:
-    if job_name.startswith("."):
-        return None
-    return f"{pipeline_name}-"
-
-
-def parse_groups(name, file, groups):
-    if groups:
-        groups = [group.strip() for group in groups.split(",")]
-
-    if not groups:
-        group_names = set()
-        for job_name in file.jobs.keys():
-            if job_name.startswith("."):
-                continue
-            group_name = job_name[len(f"{name}-") :]
-            group_name = group_name.split("-")[0]
-            group_names.add(group_name)
-        groups = sorted(list(group_names))
-    return groups
+def get_bundle_name(text):
+    return re.sub(r"[-_ ]+", "-", text.casefold())
 
 
 def bundle_command(parser, args):
     logging.basicConfig(level=logging.INFO, format="[%(levelname)s] %(message)s")
-    print(colored("pipeline name:", color="yellow"), args.pipeline_name)
 
     provider = import_module(f".{DEFAULT_PROVIDER}", "cici.providers")
 
     ci_file_path = args.config_path / provider.CI_FILE
 
     if not Path(ci_file_path).exists():
         parser.error(f"file not found: {ci_file_path}")
 
     file = provider.load(ci_file_path)
 
     args.output_path = Path(args.output_path)
-    args.groups = parse_groups(args.pipeline_name, file, args.groups)
-    print(colored("bundle names:", color="yellow"), args.groups)
 
-    for bundle_name in args.groups:
-        pattern = f"{args.pipeline_name}-{bundle_name}"
+    for job_name, job in file.jobs.items():
+        if job_name.startswith("."):
+            continue
 
         bundle = copy.deepcopy(file)
         bundle.jobs = {}
+        bundle.jobs[job_name] = job
 
-        for job_name, job in file.jobs.items():
-            job_prefix = get_job_prefix(
-                pipeline_name=args.pipeline_name,
-                job_name=job_name,
-            )
-            if not job_prefix:
-                continue
-            assert job_name.startswith(job_prefix)
-            if job_name.startswith(pattern):
-                bundle.jobs[job_name] = job
-
-        bundle_filename = args.output_path / f"{bundle_name}.yml"
+        bundle_filename = args.output_path / f"{get_bundle_name(job_name)}.yml"
 
         with open(bundle_filename, "w") as stream:
+            stream.write(f"#\n")
+            stream.write(f"# This bundle is auto-generated with cici {__version__}\n")
+            stream.write(f"#\n")
             provider.dump(bundle, stream)
         print(colored("created", "magenta"), bundle_filename.name)
 
 
 def bundle_parser(subparsers):
     parser = subparsers.add_parser(
         "bundle", help="bundle CI jobs with dependencies into standalone distributions"
@@ -88,17 +62,9 @@
         "-o",
         "--output",
         metavar="DIR",
         dest="output_path",
         type=Path,
         default=Path.cwd().absolute(),
     )
-    parser.add_argument(
-        "-n",
-        "--name",
-        metavar="DIR",
-        dest="pipeline_name",
-        default=str(Path.cwd().name),
-        help="the name of the pipeline",
-    )
     parser.set_defaults(func=bundle_command)
     return parser
```

### Comparing `cici-tools-0.2.5/cici/cli/fmt.py` & `cici-tools-0.3.0/cici/cli/fmt.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         if not Path(filename).exists():
             parser.error(f"file not found: {filename}")
 
     for filename in args.filenames:
         file = provider.load(filename)
         with open(filename, "w") as stream:
             provider.dump(file, stream)
-        print(colored(filename, "magenta"), "formatted")
+        print(colored("formatted", "magenta"), filename)
 
 
 def fmt_parser(subparsers):
     parser = subparsers.add_parser("fmt", help="format CI files")
     parser.add_argument("filenames", metavar="FILE", nargs="*")
     parser.set_defaults(func=fmt_command)
     return parser
```

### Comparing `cici-tools-0.2.5/cici/cli/update.py` & `cici-tools-0.3.0/cici/cli/update.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,49 +39,43 @@
 
 def get_latest_release(project_id):
     return get_apiv4_url(
         f"/projects/{to_fragment(project_id)}/releases/permalink/latest"
     )
 
 
-def cproject(project_name):
-    return colored(project_name, "magenta")
-
-
-def ctag(tag_name):
-    return colored(tag_name, "yellow", attrs=["bold"])
-
-
 def update_include(include):
     if any(key not in include for key in ("project", "file")):
         return include
 
     project = get_project(include["project"])
     project_name = project["path_with_namespace"]
 
     latest_release = get_latest_release(project["id"])
     if latest_release:
         latest_tag = latest_release["tag_name"]
         current_tag = include.get("ref", None)
         if current_tag:
             if current_tag != latest_tag:
                 print(
-                    colored(project_name, "red", attrs=["bold"]),
-                    "updated from {current} to {latest}".format(
-                        current=ctag(current_tag),
-                        latest=ctag(latest_tag),
-                    ),
+                    colored("updated", "magenta"),
+                    project_name,
+                    colored("from", "magenta"),
+                    current_tag,
+                    colored("to", "magenta"),
+                    latest_tag,
                 )
-            else:
-                print(cproject(project_name), "is the latest at", ctag(current_tag))
         elif not current_tag:
-            print(cproject(project_name), "pinned to", ctag(latest_tag))
+            print(
+                colored("updated", "magenta"),
+                project_name,
+                colored("to", "magenta"),
+                latest_tag,
+            )
         include["ref"] = latest_tag
-    else:
-        print(cproject(project_name), "has no releases")
     newinclude = {}
     newinclude["project"] = include["project"]
     if "ref" in include:
         newinclude["ref"] = include["ref"]
     newinclude["file"] = include["file"]
     return newinclude
```

### Comparing `cici-tools-0.2.5/cici/constants.py` & `cici-tools-0.3.0/cici/constants.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/main.py` & `cici-tools-0.3.0/cici/main.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/providers/gitlab/constants.py` & `cici-tools-0.3.0/cici/providers/gitlab/constants.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/providers/gitlab/converter.py` & `cici-tools-0.3.0/cici/providers/gitlab/converter.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/providers/gitlab/models.py` & `cici-tools-0.3.0/cici/providers/gitlab/models.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/providers/gitlab/serializers.py` & `cici-tools-0.3.0/cici/providers/gitlab/serializers.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/providers/gitlab/utils.py` & `cici-tools-0.3.0/cici/providers/gitlab/utils.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/schema/LICENSE.gitlab` & `cici-tools-0.3.0/cici/schema/LICENSE.gitlab`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/schema/gitlab-ci.json` & `cici-tools-0.3.0/cici/schema/gitlab-ci.json`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici/utils.py` & `cici-tools-0.3.0/cici/utils.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/cici_tools.egg-info/PKG-INFO` & `cici-tools-0.3.0/cici_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici-tools
-Version: 0.2.5
+Version: 0.3.0
 Summary: Power tools for CI/CD.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
```

### Comparing `cici-tools-0.2.5/cici_tools.egg-info/SOURCES.txt` & `cici-tools-0.3.0/cici_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.5/setup.py` & `cici-tools-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.2.5"
+__version__ = "0.3.0"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```

