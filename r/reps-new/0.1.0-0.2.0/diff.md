# Comparing `tmp/reps_new-0.1.0.tar.gz` & `tmp/reps_new-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reps_new-0.1.0.tar", max compression
+gzip compressed data, was "reps_new-0.2.0.tar", max compression
```

## Comparing `reps_new-0.1.0.tar` & `reps_new-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,44 @@
--rw-r--r--   0        0        0    16725 2023-06-26 14:32:18.742202 reps_new-0.1.0/LICENSE
--rw-r--r--   0        0        0      878 2023-06-28 15:28:34.307375 reps_new-0.1.0/README.md
--rw-r--r--   0        0        0      528 2023-06-28 15:59:13.776862 reps_new-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 14:40:53.482059 reps_new-0.1.0/reps/__init__.py
--rw-r--r--   0        0        0     1561 2023-06-28 15:28:34.307375 reps_new-0.1.0/reps/console.py
--rw-r--r--   0        0        0     2663 2023-06-27 20:05:58.083480 reps_new-0.1.0/reps/hooks.py
--rw-r--r--   0        0        0      446 2023-06-27 15:15:55.197097 reps_new-0.1.0/reps/templates/base/cookiecutter.json
--rw-r--r--   0        0        0       88 2023-06-27 14:22:18.958542 reps_new-0.1.0/reps/templates/base/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-06-26 17:22:22.013700 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/.codespell-ignore-words.txt
--rw-r--r--   0        0        0      105 2023-06-26 18:33:35.852510 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/CODEOWNERS
--rw-r--r--   0        0        0     2788 2023-06-26 18:38:23.842430 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      980 2023-06-26 17:25:52.613642 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2023-06-26 17:21:43.703711 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/.yamllint.yml
--rw-r--r--   0        0        0      493 2023-06-26 17:18:54.383758 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    16725 2023-06-26 17:19:01.503756 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE
--rw-r--r--   0        0        0      723 2023-06-27 15:07:50.494974 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile
--rw-r--r--   0        0        0      958 2023-06-26 18:17:31.402780 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/README.md
--rw-r--r--   0        0        0       18 2023-06-27 15:37:41.811689 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/concepts/index.rst
--rw-r--r--   0        0        0     1732 2023-06-27 15:07:07.525755 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py
--rw-r--r--   0        0        0       28 2023-06-27 15:37:27.161828 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/howto/index.rst
--rw-r--r--   0        0        0      255 2023-06-27 15:33:11.684251 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/index.rst
--rw-r--r--   0        0        0       20 2023-06-27 15:37:52.271590 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/reference/index.rst
--rw-r--r--   0        0        0       20 2023-06-27 15:38:02.821490 reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/tutorials/index.rst
--rw-r--r--   0        0        0      742 2023-06-27 20:05:58.083480 reps_new-0.1.0/reps/templates/python/cookiecutter.json
--rw-r--r--   0        0        0      129 2023-06-27 20:05:58.083480 reps_new-0.1.0/reps/templates/python/hooks/post_gen_project.py
--rw-r--r--   0        0        0      113 2023-06-27 20:05:58.083480 reps_new-0.1.0/reps/templates/python/hooks/pre_gen_project.py
--rw-r--r--   0        0        0    14684 2023-06-27 20:05:58.083480 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml
--rw-r--r--   0        0        0      918 2023-06-27 20:05:58.083480 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml
--rw-r--r--   0        0        0     1192 2023-06-27 20:12:17.263374 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml
--rw-r--r--   0        0        0      713 2023-06-27 20:05:58.083480 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml
--rw-r--r--   0        0        0      555 2023-06-27 20:07:42.663451 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml
--rw-r--r--   0        0        0      743 2023-06-27 20:05:58.083480 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml
--rw-r--r--   0        0        0     1243 2023-06-27 20:05:58.083480 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml
--rw-r--r--   0        0        0      713 2023-06-27 20:16:13.963308 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/codecov-upload.py
--rw-r--r--   0        0        0      635 2023-06-27 20:14:20.693340 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup
--rw-r--r--   0        0        0      345 2023-06-27 15:00:30.932961 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/test/conftest.py
--rw-r--r--   0        0        0       60 2023-06-27 14:59:09.804436 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/test/test_{{cookiecutter.__package_name}}.py
--rw-r--r--   0        0        0      956 2023-06-27 20:05:58.083480 reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/tox.ini
--rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 reps_new-0.1.0/setup.py
--rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 reps_new-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-06-26 14:32:18.742202 reps_new-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1008 2023-07-06 19:30:10.728667 reps_new-0.2.0/README.md
+-rw-r--r--   0        0        0      550 2023-07-06 20:48:57.587349 reps_new-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 14:40:53.482059 reps_new-0.2.0/reps/__init__.py
+-rw-r--r--   0        0        0     1556 2023-07-06 19:29:55.318671 reps_new-0.2.0/reps/console.py
+-rw-r--r--   0        0        0     2915 2023-07-06 19:29:55.318671 reps_new-0.2.0/reps/hooks.py
+-rw-r--r--   0        0        0      446 2023-06-27 15:15:55.197097 reps_new-0.2.0/reps/templates/base/cookiecutter.json
+-rw-r--r--   0        0        0       88 2023-06-27 14:22:18.958542 reps_new-0.2.0/reps/templates/base/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-06-26 17:22:22.013700 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.codespell-ignore-words.txt
+-rw-r--r--   0        0        0      105 2023-06-26 18:33:35.852510 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/CODEOWNERS
+-rw-r--r--   0        0        0     2788 2023-06-26 18:38:23.842430 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      980 2023-06-26 17:25:52.613642 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2023-06-26 17:21:43.703711 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.yamllint.yml
+-rw-r--r--   0        0        0      493 2023-06-26 17:18:54.383758 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    16725 2023-06-26 17:19:01.503756 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE
+-rw-r--r--   0        0        0      723 2023-06-27 15:07:50.494974 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile
+-rw-r--r--   0        0        0      958 2023-07-06 14:55:10.046283 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/README.md
+-rw-r--r--   0        0        0       18 2023-06-27 15:37:41.811689 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/concepts/index.rst
+-rw-r--r--   0        0        0     1732 2023-06-27 15:07:07.525755 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py
+-rw-r--r--   0        0        0       28 2023-06-27 15:37:27.161828 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/howto/index.rst
+-rw-r--r--   0        0        0      255 2023-06-27 15:33:11.684251 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/index.rst
+-rw-r--r--   0        0        0       20 2023-06-27 15:37:52.271590 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/reference/index.rst
+-rw-r--r--   0        0        0       20 2023-06-27 15:38:02.821490 reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/tutorials/index.rst
+-rw-r--r--   0        0        0     1120 2023-07-06 19:29:54.578671 reps_new-0.2.0/reps/templates/python/cookiecutter.json
+-rw-r--r--   0        0        0      129 2023-06-27 20:05:58.083480 reps_new-0.2.0/reps/templates/python/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      113 2023-06-27 20:05:58.083480 reps_new-0.2.0/reps/templates/python/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0    16185 2023-07-06 19:30:10.728667 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml
+-rw-r--r--   0        0        0      918 2023-06-27 20:05:58.083480 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 20:18:22.754371 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/src/{{cookiecutter.__package_name}}/__init__.py
+-rw-r--r--   0        0        0     1175 2023-07-06 20:25:24.507743 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml
+-rw-r--r--   0        0        0      570 2023-07-05 13:50:01.939464 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml
+-rw-r--r--   0        0        0      512 2023-07-06 19:29:54.578671 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml
+-rw-r--r--   0        0        0      743 2023-06-27 20:05:58.083480 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml
+-rw-r--r--   0        0        0      993 2023-07-06 20:28:44.257688 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml
+-rw-r--r--   0        0        0      518 2023-07-04 19:06:10.348905 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/fetch/Dockerfile
+-rw-r--r--   0        0        0     1306 2023-07-06 20:23:53.167770 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/docker/python/Dockerfile
+-rw-r--r--   0        0        0       22 2023-07-04 19:26:34.218564 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/requirements.in
+-rw-r--r--   0        0        0      701 2023-07-06 19:29:55.318671 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/codecov-upload.py
+-rwxr-xr-x   0        0        0      179 2023-07-06 19:29:56.058671 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/poetry-setup
+-rwxr-xr-x   0        0        0      658 2023-07-06 20:36:16.647561 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup
+-rw-r--r--   0        0        0      345 2023-06-27 15:00:30.932961 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/test/conftest.py
+-rw-r--r--   0        0        0      164 2023-07-06 19:29:55.318671 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/test/test_{{cookiecutter.__package_name}}.py
+-rw-r--r--   0        0        0      957 2023-07-06 19:30:10.738667 reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/tox.ini
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 reps_new-0.2.0/PKG-INFO
```

### Comparing `reps_new-0.1.0/LICENSE` & `reps_new-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reps_new-0.1.0/README.md` & `reps_new-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 This repository:
 
 1. Defines the standard tools and workflows that Mozilla Release Engineering
    endeavours to use across its projects.
 2. Implements a `reps` binary that can be used to bootstrap new projects based
    on the defined standard.
 
+## Project Standard
+
+Please see
+[STANDARD.md](https://github.com/mozilla-releng/reps/blob/main/STANDARD.md) for
+the REPS definition.
+
 ## Usage
 
 The `reps` tool can be used to bootstrap new projects that conform to this
 standard. It is recommended to install and run it with
 [pipx](https://github.com/pypa/pipx) (so the most up to date version is always
 used):
 
@@ -22,8 +28,8 @@
 You may optionally specify a different template to use with the `-t/--template` flag:
 
 ```bash
 pipx run reps-new -t base
 ```
 
 Available templates can be found in the
-[templates directory](https://github.com/mozilla-releng/reps/tree/main/src/reps/templates).
+[templates directory](https://github.com/mozilla-releng/reps/tree/main/reps/templates).
```

### Comparing `reps_new-0.1.0/pyproject.toml` & `reps_new-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "reps-new"
-version = "0.1.0"
+version = "0.2.0"
 description = "Mozilla Release Engineering Project Standard"
 authors = ["Mozilla Release Engineering <release@mozilla.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 packages = [{ include = "reps" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 cookiecutter = "^2.1.1"
 pre-commit = "^3.3.3"
 taskcluster-taskgraph = "^5.4.0"
 pyyaml = "^6.0"
+pip-tools = "^6.14.0"
 
 [tool.poetry.scripts]
 reps-new = "reps.console:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `reps_new-0.1.0/reps/console.py` & `reps_new-0.2.0/reps/console.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,31 +20,27 @@
     if template != "base":
         # The 'base' template will be generated first, and non-base templates
         # then get merged into it. So unless the 'base' template was explicitly
         # specified, ensure we don't error out when the project already exists.
         cookiecutter_args.setdefault("overwrite_if_exists", False)
 
     template = TEMPLATE_DIR / template
-    context = {"project_name": name}
+    cookiecutter_args.setdefault("extra_context", {}).setdefault("project_name", name)
 
     # Generate the project.
     cookiecutter(
         str(template),
-        extra_context=context,
         **cookiecutter_args,
     )
 
 
 def run(args=sys.argv[1:]):
     parser = ArgumentParser()
     parser.add_argument(
-        "name",
-        nargs="?",
-        default=None,
-        help="Name of the project to create."
+        "name", nargs="?", default=None, help="Name of the project to create."
     )
     parser.add_argument(
         "-t",
         "--template",
         default="python",
         choices=available_templates(),
         help="Project template to initialize.",
```

### Comparing `reps_new-0.1.0/reps/hooks.py` & `reps_new-0.2.0/reps/hooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,18 +28,21 @@
     kwargs.setdefault("check", True)
     subprocess.run(cmd, **kwargs)
 
 
 @hook("pre-gen-py")
 def base_init(items):
     """Generate the 'base' template first."""
+    if "_copy_without_render" in items:
+        del items["_copy_without_render"]
+
     command_new(
         items["__project_slug"],
         template="base",
-        default_config=items,
+        extra_context=items,
         no_input=True,
         output_dir=str(Path.cwd().parent),
         accept_hooks=False,
         overwrite_if_exists=True,
     )
 
 
@@ -103,23 +106,29 @@
     run(["git", "checkout", "-b", "main"])
     run(
         [
             "git",
             "remote",
             "add",
             "origin",
-            f"https://github.com/{items['github_slug']}",
+            f"git@github.com:{items['github_slug']}.git",
         ]
     )
 
 
 @hook("post-gen-py")
 @hook("post-gen-base")
 def pre_commit_autoupdate(items):
     run(["pre-commit", "autoupdate"])
 
 
+@hook("post-gen-py")
+@hook("post-gen-base")
+def lock_taskgraph_requirements(items):
+    run(["pip-compile", "requirements.in", "--generate-hashes"], cwd="taskcluster")
+
+
 @hook("post-gen-base")
 def taskgraph_init(items):
     run(["taskgraph", "init"])
```

### Comparing `reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml` & `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml` & `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE` & `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile` & `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/README.md` & `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `reps_new-0.1.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py` & `reps_new-0.2.0/reps/templates/base/{{cookiecutter.__project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reps_new-0.1.0/reps/templates/python/cookiecutter.json` & `reps_new-0.2.0/reps/templates/python/cookiecutter.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'__github_project'": '"{{cookiecutter.github_slug[cookiecutter.github_slug.find(\'/\')+1:]}}"',*

 * * "'__max_tox_python_version'": '"{{cookiecutter._max_python_version.replace(\'.\', \'\')}}"',*

 * * "'__secrets_path'": "'project/releng/{{cookiecutter.trust_domain}}/{{cookiecutter.trust_project}}/build/level-{{cookiecutter.level}}/ci'",*

 * * "'_max_python_version'": "'3.11'",*

 * * "'trust_project'": "'{{cookiecutter.__github_project}}'",*

 * * 'delete': "['_max_tox_python_version']"}*

```diff
@@ -1,17 +1,21 @@
 {
     "__github_org": "{{cookiecutter.github_slug[:cookiecutter.github_slug.find('/')]}}",
+    "__github_project": "{{cookiecutter.github_slug[cookiecutter.github_slug.find('/')+1:]}}",
+    "__max_tox_python_version": "{{cookiecutter._max_python_version.replace('.', '')}}",
     "__min_tox_python_version": "{{cookiecutter.min_python_version.replace('.', '')}}",
     "__package_name": "{{cookiecutter.project_name|lower|replace(' ', '_')}}",
     "__project_slug": "{{cookiecutter.project_name|lower|replace(' ', '-')}}",
+    "__secrets_path": "project/releng/{{cookiecutter.trust_domain}}/{{cookiecutter.trust_project}}/build/level-{{cookiecutter.level}}/ci",
     "_copy_without_render": [
         ".github/workflows/codeql-analysis.yml"
     ],
-    "_max_tox_python_version": "311",
+    "_max_python_version": "3.11",
     "author": "Mozilla Release Engineering <release@mozilla.com>",
     "github_slug": "mozilla-releng/{{cookiecutter.__project_slug}}",
     "level": "1",
     "min_python_version": "3.7",
     "project_name": "My Project",
     "short_description": "",
-    "trust_domain": "mozilla"
+    "trust_domain": "mozilla",
+    "trust_project": "{{cookiecutter.__github_project}}"
 }
```

### Comparing `reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml` & `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/.taskcluster.yml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 version: 1
 reporting: checks-v1
 policy:
     pullRequests: public
 tasks:
     - $let:
           trustDomain: "{{cookiecutter.trust_domain}}"
-          level: "{{cookiecutter.level}}"
           ownerEmail:
               $switch:
                   'tasks_for == "github-push"': '${event.pusher.email}'
                   'tasks_for[:19] == "github-pull-request"': '${event.pull_request.user.login}@users.noreply.github.com'
                   'tasks_for in ["cron", "action"]': '${tasks_for}@noreply.mozilla.org'
           baseRepoUrl:
               $switch:
@@ -66,206 +65,227 @@
           pullRequestAction:
               $switch:
                   'tasks_for[:19] == "github-pull-request"': ${event.action}
                   $default: 'UNDEFINED'
           isPullRequest:
               $eval: 'tasks_for[:19] == "github-pull-request"'
       in:
-          $if: >
-              tasks_for in ["action", "cron"]
-              || (tasks_for == "github-push" && head_branch == "refs/heads/main")
-              || (isPullRequest && pullRequestAction in ["opened", "reopened", "synchronize"])
-          then:
-              taskId: {$if: 'tasks_for != "action"', then: '${ownTaskId}'}
-              taskGroupId:
-                  $if: 'tasks_for == "action"'
-                  then:
-                      '${action.taskGroupId}'
-                  else:
-                      '${ownTaskId}'  # same as taskId; this is how automation identifies a decision task
-              schedulerId: '${trustDomain}-level-${level}'
-              created: {$fromNow: ''}
-              deadline: {$fromNow: '1 day'}
-              expires: {$fromNow: '1 year 1 second'}  # 1 second so artifacts expire first
-              metadata:
-                  $merge:
-                      - owner: "${ownerEmail}"
-                        source: "${repoUrl}/raw/${head_sha}/.taskcluster.yml"
-                      - $switch:
-                            'tasks_for == "github-push" || isPullRequest':
-                                name: "Decision Task"
-                                description: 'The task that creates all of the other tasks in the task graph'
-                            'tasks_for == "action"':
-                                name: "Action: ${action.title}"
-                                description: |
-                                    ${action.description}
-
-                                    Action triggered by clientID `${clientId}`
-                            $default:
-                                name: "Decision Task for cron job ${cron.job_name}"
-                                description: 'Created by a [cron task](https://firefox-ci-tc.services.mozilla.com/tasks/${cron.task_id})'
-
-              provisionerId: "${trustDomain}-${level}"
-              workerType: "decision-gcp"
-
-              tags:
-                  $switch:
-                      'tasks_for == "github-push" || isPullRequest':
-                          createdForUser: "${ownerEmail}"
-                          kind: decision-task
-                      'tasks_for == "action"':
-                          createdForUser: '${ownerEmail}'
-                          kind: 'action-callback'
-                      'tasks_for == "cron"':
-                          kind: cron-task
-
-              routes:
-                  $flatten:
-                      - checks
-                      - $switch:
-                            'tasks_for == "github-push"':
-                                - "index.${trustDomain}.v2.${project}.latest.taskgraph.decision"
-                                - "index.${trustDomain}.v2.${project}.revision.${head_sha}.taskgraph.decision"
-                            'tasks_for == "action"':
-                                - "index.${trustDomain}.v2.${project}.revision.${head_sha}.taskgraph.actions.${ownTaskId}"
-                            'tasks_for == "cron"':
-                                - "index.${trustDomain}.v2.${project}.latest.taskgraph.decision-${cron.job_name}"
-                                - "index.${trustDomain}.v2.${project}.revision.${head_sha}.taskgraph.decision-${cron.job_name}"
-                                # list each cron task on this revision, so actions can find them
-                                - 'index.${trustDomain}.v2.${project}.revision.${head_sha}.cron.${ownTaskId}'
-                            $default: []
-
-              scopes:
-                  $switch:
-                      'tasks_for in ["github-push"]':
-                          $let:
-                              short_head_ref:
-                                  $if: 'head_ref[:10] == "refs/tags/"'
-                                  then: {$eval: 'head_ref[10:]'}
-                                  else:
-                                      $if: 'head_ref[:11] == "refs/heads/"'
-                                      then: {$eval: 'head_ref[11:]'}
-                                      else: ${head_ref}
-                          in:
-                              - 'assume:repo:${repoUrl[8:]}:branch:${short_head_ref}'
-                      'isPullRequest':
-                          - 'assume:repo:github.com/${event.pull_request.base.repo.full_name}:${tasks_for[7:]}'
-                      'tasks_for == "action"':
-                          - 'assume:repo:${repoUrl[8:]}:action:${action.action_perm}'
-                      $default:
-                          - 'assume:repo:${repoUrl[8:]}:cron:${cron.job_name}'
-
-              dependencies: []
-              requires: all-completed
-
-              priority:
-                  $switch:
-                      'tasks_for == "cron"': low
-                      'tasks_for == "github-push"|| isPullRequest': very-low
-                      $default: lowest  # tasks_for == 'action'
-              retries: 5
-
-              payload:
-                  $let:
-                      normProject:
-                          $eval: 'join(split(project, "-"), "_")'
-                      normProjectUpper:
-                          $eval: 'uppercase(join(split(project, "-"), "_"))'
-                  in:
-                      env:
-                          # run-task uses these to check out the source; the inputs to
-                          # `taskgraph decision` are all on the command line.
-                          $merge:
-                              - ${normProjectUpper}_BASE_REPOSITORY: '${baseRepoUrl}'
-                                ${normProjectUpper}_BASE_REF: '${base_ref}'
-                                ${normProjectUpper}_BASE_REV: '${base_sha}'
-                                ${normProjectUpper}_HEAD_REPOSITORY: '${repoUrl}'
-                                ${normProjectUpper}_HEAD_REF: '${head_ref}'
-                                ${normProjectUpper}_HEAD_REV: '${head_sha}'
-                                ${normProjectUpper}_REPOSITORY_TYPE: git
-                                ${normProjectUpper}_PIP_REQUIREMENTS: taskcluster/requirements.txt
-                                REPOSITORIES:
-                                    $json:
-                                        ${normProject}: ${normProject}
-                              - $if: 'isPullRequest'
-                                then:
-                                    ${normProjectUpper}_PULL_REQUEST_NUMBER: '${event.pull_request.number}'
-                              - $if: 'tasks_for == "action"'
-                                then:
-                                    ACTION_TASK_GROUP_ID: '${action.taskGroupId}'  # taskGroupId of the target task
-                                    ACTION_TASK_ID: {$json: {$eval: 'taskId'}}  # taskId of the target task (JSON-encoded)
-                                    ACTION_INPUT: {$json: {$eval: 'input'}}
-                                    ACTION_CALLBACK: '${action.cb_name}'
-
-                      cache:
-                          "${trustDomain}-level-${level}-checkouts-sparse-v2": /builds/worker/checkouts
-
-                      features:
-                          taskclusterProxy: true
-
-                      image: mozillareleases/taskgraph:decision-10378fde0bf12adbd64e74313bf72ea3c6caf311ad6af23e2bff1d8f1232a221@sha256:7518c410bdf91142b0e26455d26ddaf861202cfbb3c35d0b1ef85d1ed577a5bd
-                      maxRunTime: 1800
-
-                      command:
-                          - run-task
-                          - '--${normProject}-checkout=/builds/worker/checkouts/src'
-                          - '--'
-                          - bash
-                          - -cx
-                          - $let:
-                                extraArgs: {$if: 'tasks_for == "cron"', then: '${cron.quoted_args}', else: ''}
-                            in:
-                                $if: 'tasks_for == "action"'
-                                then: >
-                                    cd /builds/worker/checkouts/src &&
-                                    ln -s /builds/worker/artifacts artifacts &&
-                                    pip3 install -r requirements/base.txt &&
-                                    ~/.local/bin/taskgraph action-callback
-                                else: >
-                                    cd /builds/worker/checkouts/src &&
-                                    ln -s /builds/worker/artifacts artifacts &&
-                                    ~/.local/bin/taskgraph decision
-                                    --pushlog-id='0'
-                                    --pushdate='0'
-                                    --project='${project}'
-                                    --owner='${ownerEmail}'
-                                    --level='${level}'
-                                    --repository-type=git
-                                    --tasks-for='${tasks_for}'
-                                    --base-repository='${baseRepoUrl}'
-                                    --base-ref='${base_ref}'
-                                    --base-rev='${base_sha}'
-                                    --head-repository='${repoUrl}'
-                                    --head-ref='${head_ref}'
-                                    --head-rev='${head_sha}'
-                                    ${extraArgs}
-
-                      artifacts:
-                          'public':
-                              type: 'directory'
-                              path: '/builds/worker/artifacts'
-                              expires: {$fromNow: '1 year'}
-                          'public/docker-contexts':
-                              type: 'directory'
-                              path: '/builds/worker/checkouts/src/docker-contexts'
-                              # This needs to be at least the deadline of the
-                              # decision task + the docker-image task deadlines.
-                              # It is set to a week to allow for some time for
-                              # debugging, but they are not useful long-term.
-                              expires: {$fromNow: '7 day'}
-
-                      extra:
-                          $merge:
-                              - $if: 'tasks_for == "action"'
-                                then:
-                                    parent: '${action.taskGroupId}'
-                                    action:
-                                        name: '${action.name}'
-                                        context:
-                                            taskGroupId: '${action.taskGroupId}'
-                                            taskId: {$eval: 'taskId'}
-                                            input: {$eval: 'input'}
-                                            clientId: {$eval: 'clientId'}
-                              - $if: 'tasks_for == "cron"'
-                                then:
-                                    cron: {$json: {$eval: 'cron'}}
-                              - tasks_for: '${tasks_for}'
+          $let:
+              short_base_ref:
+                  $if: 'base_ref[:11] == "refs/heads/"'
+                  then: {$eval: 'base_ref[11:]'}
+                  else: ${base_ref}
+
+              short_head_ref:
+                  $if: 'head_ref[:11] == "refs/heads/"'
+                  then: {$eval: 'head_ref[11:]'}
+                  else: ${head_ref}
+              {%- if cookiecutter.level == "1" %}
+              level: 1
+              {% else %}
+              level:
+                  $if: >
+                      repoUrl == "https://github.com/{{cookiecutter.github_slug}}" && (
+                      tasks_for in [""cron", "action"] ||
+                      (tasks_for == "github-push" && head_branch == "refs/head/main"))
+                  then: {{cookiecutter.level}}
+                  else: 1
+              {%- endif %}
+          in:
+              $if: >
+                  tasks_for in ["action", "cron", "github-push"]
+                  || (isPullRequest && pullRequestAction in ["opened", "reopened", "synchronize"])
+              then:
+                  taskId: {$if: 'tasks_for != "action"', then: '${ownTaskId}'}
+                  taskGroupId:
+                      $if: 'tasks_for == "action"'
+                      then:
+                          '${action.taskGroupId}'
+                      else:
+                          '${ownTaskId}'  # same as taskId; this is how automation identifies a decision task
+                  schedulerId: '${trustDomain}-level-${level}'
+                  created: {$fromNow: ''}
+                  deadline: {$fromNow: '1 day'}
+                  expires: {$fromNow: '1 year 1 second'}  # 1 second so artifacts expire first
+                  metadata:
+                      $merge:
+                          - owner: "${ownerEmail}"
+                            source: "${repoUrl}/raw/${head_sha}/.taskcluster.yml"
+                          - $switch:
+                                'tasks_for == "github-push" || isPullRequest':
+                                    name: "Decision Task"
+                                    description: 'The task that creates all of the other tasks in the task graph'
+                                'tasks_for == "action"':
+                                    name: "Action: ${action.title}"
+                                    description: |
+                                        ${action.description}
+
+                                        Action triggered by clientID `${clientId}`
+                                $default:
+                                    name: "Decision Task for cron job ${cron.job_name}"
+                                    description: 'Created by a [cron task](https://firefox-ci-tc.services.mozilla.com/tasks/${cron.task_id})'
+
+                  provisionerId: "${trustDomain}-${level}"
+                  workerType: "decision-gcp"
+
+                  tags:
+                      $switch:
+                          'tasks_for == "github-push" || isPullRequest':
+                              createdForUser: "${ownerEmail}"
+                              kind: decision-task
+                          'tasks_for == "action"':
+                              createdForUser: '${ownerEmail}'
+                              kind: 'action-callback'
+                          'tasks_for == "cron"':
+                              kind: cron-task
+
+                  routes:
+                      $flatten:
+                          - checks
+                          - $switch:
+                                'tasks_for == "github-push"':
+                                    - "index.${trustDomain}.v2.${project}.latest.taskgraph.decision"
+                                    - "index.${trustDomain}.v2.${project}.revision.${head_sha}.taskgraph.decision"
+                                'tasks_for == "action"':
+                                    - "index.${trustDomain}.v2.${project}.revision.${head_sha}.taskgraph.actions.${ownTaskId}"
+                                'tasks_for == "cron"':
+                                    - "index.${trustDomain}.v2.${project}.latest.taskgraph.decision-${cron.job_name}"
+                                    - "index.${trustDomain}.v2.${project}.revision.${head_sha}.taskgraph.decision-${cron.job_name}"
+                                    # list each cron task on this revision, so actions can find them
+                                    - 'index.${trustDomain}.v2.${project}.revision.${head_sha}.cron.${ownTaskId}'
+                                $default: []
+
+                  scopes:
+                      $switch:
+                          'tasks_for in ["github-push"]':
+                              $let:
+                                  short_head_ref:
+                                      $if: 'head_ref[:10] == "refs/tags/"'
+                                      then: {$eval: 'head_ref[10:]'}
+                                      else:
+                                          $if: 'head_ref[:11] == "refs/heads/"'
+                                          then: {$eval: 'head_ref[11:]'}
+                                          else: ${head_ref}
+                              in:
+                                  - 'assume:repo:${repoUrl[8:]}:branch:${short_head_ref}'
+                          'isPullRequest':
+                              - 'assume:repo:github.com/${event.pull_request.base.repo.full_name}:${tasks_for[7:]}'
+                          'tasks_for == "action"':
+                              - 'assume:repo:${repoUrl[8:]}:action:${action.action_perm}'
+                          $default:
+                              - 'assume:repo:${repoUrl[8:]}:cron:${cron.job_name}'
+
+                  dependencies: []
+                  requires: all-completed
+
+                  priority:
+                      $switch:
+                          'tasks_for == "cron"': low
+                          'tasks_for == "github-push"|| isPullRequest': very-low
+                          $default: lowest  # tasks_for == 'action'
+                  retries: 5
+
+                  payload:
+                      $let:
+                          normProject:
+                              $eval: 'join(split(project, "-"), "_")'
+                          normProjectUpper:
+                              $eval: 'uppercase(join(split(project, "-"), "_"))'
+                      in:
+                          env:
+                              # run-task uses these to check out the source; the inputs to
+                              # `taskgraph decision` are all on the command line.
+                              $merge:
+                                  - ${normProjectUpper}_BASE_REPOSITORY: '${baseRepoUrl}'
+                                    ${normProjectUpper}_BASE_REF: '${short_base_ref}'
+                                    ${normProjectUpper}_BASE_REV: '${base_sha}'
+                                    ${normProjectUpper}_HEAD_REPOSITORY: '${repoUrl}'
+                                    ${normProjectUpper}_HEAD_REF: '${short_head_ref}'
+                                    ${normProjectUpper}_HEAD_REV: '${head_sha}'
+                                    ${normProjectUpper}_REPOSITORY_TYPE: git
+                                    ${normProjectUpper}_PIP_REQUIREMENTS: taskcluster/requirements.txt
+                                    REPOSITORIES:
+                                        $json:
+                                            ${normProject}: ${normProject}
+                                  - $if: 'isPullRequest'
+                                    then:
+                                        ${normProjectUpper}_PULL_REQUEST_NUMBER: '${event.pull_request.number}'
+                                  - $if: 'tasks_for == "action"'
+                                    then:
+                                        ACTION_TASK_GROUP_ID: '${action.taskGroupId}'  # taskGroupId of the target task
+                                        ACTION_TASK_ID: {$json: {$eval: 'taskId'}}  # taskId of the target task (JSON-encoded)
+                                        ACTION_INPUT: {$json: {$eval: 'input'}}
+                                        ACTION_CALLBACK: '${action.cb_name}'
+
+                          cache:
+                              "${trustDomain}-level-${level}-checkouts-sparse-v2": /builds/worker/checkouts
+
+                          features:
+                              taskclusterProxy: true
+
+                          image: mozillareleases/taskgraph:decision-f19bfa3ae9dbc19190149445bfc38ad966b713336e44342c7643b3f7f1e0b023@sha256:ddcc7348db272885e8ea32825f698bfafa4727401099531cd8239d3d458b39aa
+                          maxRunTime: 1800
+
+                          command:
+                              - run-task
+                              - '--${normProject}-checkout=/builds/worker/checkouts/src'
+                              - '--'
+                              - bash
+                              - -cx
+                              - $let:
+                                    extraArgs: {$if: 'tasks_for == "cron"', then: '${cron.quoted_args}', else: ''}
+                                in:
+                                    $if: 'tasks_for == "action"'
+                                    then: >
+                                        cd /builds/worker/checkouts/src &&
+                                        ln -s /builds/worker/artifacts artifacts &&
+                                        pip3 install -r requirements/base.txt &&
+                                        ~/.local/bin/taskgraph action-callback
+                                    else: >
+                                        cd /builds/worker/checkouts/src &&
+                                        ln -s /builds/worker/artifacts artifacts &&
+                                        ~/.local/bin/taskgraph decision
+                                        --pushlog-id='0'
+                                        --pushdate='0'
+                                        --project='${project}'
+                                        --owner='${ownerEmail}'
+                                        --level='${level}'
+                                        --repository-type=git
+                                        --tasks-for='${tasks_for}'
+                                        --base-repository='${baseRepoUrl}'
+                                        --base-ref='${short_base_ref}'
+                                        --base-rev='${base_sha}'
+                                        --head-repository='${repoUrl}'
+                                        --head-ref='${short_head_ref}'
+                                        --head-rev='${head_sha}'
+                                        ${extraArgs}
+
+                          artifacts:
+                              'public':
+                                  type: 'directory'
+                                  path: '/builds/worker/artifacts'
+                                  expires: {$fromNow: '1 year'}
+                              'public/docker-contexts':
+                                  type: 'directory'
+                                  path: '/builds/worker/checkouts/src/docker-contexts'
+                                  # This needs to be at least the deadline of the
+                                  # decision task + the docker-image task deadlines.
+                                  # It is set to a week to allow for some time for
+                                  # debugging, but they are not useful long-term.
+                                  expires: {$fromNow: '7 day'}
+
+                          extra:
+                              $merge:
+                                  - $if: 'tasks_for == "action"'
+                                    then:
+                                        parent: '${action.taskGroupId}'
+                                        action:
+                                            name: '${action.name}'
+                                            context:
+                                                taskGroupId: '${action.taskGroupId}'
+                                                taskId: {$eval: 'taskId'}
+                                                input: {$eval: 'input'}
+                                                clientId: {$eval: 'clientId'}
+                                  - $if: 'tasks_for == "cron"'
+                                    then:
+                                        cron: {$json: {$eval: 'cron'}}
+                                  - tasks_for: '${tasks_for}'
```

### Comparing `reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml` & `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml` & `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/codecov/kind.yml`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 kind-dependencies:
     - fetch
     - test
 
 tasks:
     upload:
         description: "Upload coverage.xml to codecov.io"
-        worker-type: t-linux
+        worker-type: linux
         worker:
             docker-image: {in-tree: python}
             max-run-time: 600
             env:
                 MOZ_FETCHES_DIR: /builds/worker/fetches
         scopes:
-            - secrets:get:project/releng/{{cookiecutter.__project_slug}}/ci
+            - secrets:get:{{cookiecutter.__secrets_path}}
         dependencies:
             test: test-unit
         fetches:
             fetch:
                 - codecov-uploader
             test:
                 - coverage.xml
         run-on-tasks-for: ["github-push", "github-pull-request"]
         run:
             using: run-task
             cwd: '{checkout}'
             command: >-
-                poetry install --only test
+                poetry install --only test &&
                 poetry run python taskcluster/scripts/codecov-upload.py
```

### Comparing `reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml` & `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/config.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 ---
 trust-domain: "{{cookiecutter.trust_domain}}"
 task-priority: low
 
 taskgraph:
-  cached-task-prefix: "{{cookiecutter.trust_domain}}.v2.{{cookiecutter.__project_slug}}"
+  cached-task-prefix: "{{cookiecutter.trust_domain}}.v2.{{cookiecutter.trust_project}}"
   repositories:
     {{cookiecutter.__package_name}}:
       name: "{{cookiecutter.project_name}}"
 
 workers:
   aliases:
-    b-linux:
-      provisioner: '{trust-domain}-{level}'
-      implementation: docker-worker
-      os: linux
-      worker-type: '{alias}-gcp'
     images:
       provisioner: '{trust-domain}-{level}'
       implementation: docker-worker
       os: linux
       worker-type: '{alias}-gcp'
-    t-linux-large:
+    linux:
       provisioner: '{trust-domain}-t'
       implementation: docker-worker
       os: linux
-      worker-type: '{alias}-gcp'
+      worker-type: 't-{alias}-large-gcp'
```

### Comparing `reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml` & `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/docker-image/kind.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 {%- set pylist -%}
-{%- for i in range(cookiecutter._max_tox_python_version[1:]|int, cookiecutter.__min_tox_python_version[1:]|int - 1, -1) -%}
+{%- for i in range(cookiecutter.__max_tox_python_version[1:]|int, cookiecutter.__min_tox_python_version[1:]|int - 1, -1) -%}
 3.{{i}}
 {%- if not loop.last %},{% endif -%}
 {%- endfor -%}
 {%- endset -%}
 ---
 loader: taskgraph.loader.transform:loader
 
 transforms:
     - taskgraph.transforms.docker_image:transforms
     - taskgraph.transforms.cached_tasks:transforms
     - taskgraph.transforms.task:transforms
 
 tasks:
-    fetch:
-        symbol: I(fetch)
+    fetch: {}
     python:
-        symbol: I(py)
         args:
             PYENV_VERSIONS: "{{pylist}}"
```

### Comparing `reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml` & `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/fetch/kind.yml`

 * *Files identical despite different names*

### Comparing `reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml` & `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/ci/test/kind.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,36 @@
-{%- set pylist -%}
-{%- for i in range(cookiecutter._max_tox_python_version[1:]|int, cookiecutter.__min_tox_python_version[1:]|int - 1, -1) -%}
-3.{{i}}
-{%- if not loop.last %} {% endif -%}
-{%- endfor -%}
-{%- endset -%}
 ---
 loader: taskgraph.loader.transform:loader
 
 transforms:
     - taskgraph.transforms.job:transforms
     - taskgraph.transforms.task:transforms
 
 task-defaults:
     attributes:
         retrigger: true
-    worker-type: t-linux
+    worker-type: linux
     worker:
         docker-image: {in-tree: python}
         max-run-time: 3600
     run:
         using: run-task
         cwd: '{checkout}'
         cache-dotcache: true
 
 tasks:
     unit:
         description: "Run `unit tests` to validate the latest changes"
-        treeherder:
-            symbol: unit
         attributes:
             artifact_prefix: public
         worker:
             artifacts:
                 - type: file
                   path: /builds/worker/artifacts/coverage.xml
                   name: public/coverage.xml
             env:
                 COVERAGE_REPORT_COMMAND: "coverage xml -o /builds/worker/artifacts/coverage.xml"
                 TOX_PARALLEL_NO_SPINNER: "1"
         run:
             command: >-
-                pyenv local {{pylist}} &&
-                tox --parallel
+                poetry install --only test &&
+                poetry run tox --parallel
```

### Comparing `reps_new-0.1.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup` & `reps_new-0.2.0/reps/templates/python/{{cookiecutter.__project_slug}}/taskcluster/scripts/pyenv-setup`

 * *Files 14% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 for i in ${1//,/ }
 do
     version=$(pyenv latest --known $i)
     pyenv install $version
 done
 chmod 777 /builds/worker/.pyenv/shims
 pyenv rehash
+pyenv global ${1//,/ }
```

### Comparing `reps_new-0.1.0/PKG-INFO` & `reps_new-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: reps-new
-Version: 0.1.0
+Version: 0.2.0
 Summary: Mozilla Release Engineering Project Standard
 License: MPL-2.0
 Author: Mozilla Release Engineering
 Author-email: release@mozilla.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
+Requires-Dist: pip-tools (>=6.14.0,<7.0.0)
 Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: taskcluster-taskgraph (>=5.4.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Release Engineering Project Standard
 
 This repository:
 
 1. Defines the standard tools and workflows that Mozilla Release Engineering
    endeavours to use across its projects.
 2. Implements a `reps` binary that can be used to bootstrap new projects based
    on the defined standard.
 
+## Project Standard
+
+Please see
+[STANDARD.md](https://github.com/mozilla-releng/reps/blob/main/STANDARD.md) for
+the REPS definition.
+
 ## Usage
 
 The `reps` tool can be used to bootstrap new projects that conform to this
 standard. It is recommended to install and run it with
 [pipx](https://github.com/pypa/pipx) (so the most up to date version is always
 used):
 
@@ -40,9 +47,9 @@
 You may optionally specify a different template to use with the `-t/--template` flag:
 
 ```bash
 pipx run reps-new -t base
 ```
 
 Available templates can be found in the
-[templates directory](https://github.com/mozilla-releng/reps/tree/main/src/reps/templates).
+[templates directory](https://github.com/mozilla-releng/reps/tree/main/reps/templates).
```

