# Comparing `tmp/glean-cli-0.6.0.tar.gz` & `tmp/glean-cli-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glean-cli-0.6.0.tar", last modified: Fri Jun 23 20:04:33 2023, max compression
+gzip compressed data, was "glean-cli-0.6.1.tar", last modified: Thu Jul  6 15:36:28 2023, max compression
```

## Comparing `glean-cli-0.6.0.tar` & `glean-cli-0.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.280097 glean-cli-0.6.0/
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)    11357 2023-01-11 18:02:06.000000 glean-cli-0.6.0/LICENSE
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1283 2023-06-23 20:04:33.280162 glean-cli-0.6.0/PKG-INFO
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)      832 2023-06-23 20:03:49.000000 glean-cli-0.6.0/README.md
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)      103 2023-01-11 18:02:06.000000 glean-cli-0.6.0/pyproject.toml
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)      814 2023-06-23 20:04:33.280447 glean-cli-0.6.0/setup.cfg
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)       38 2023-01-11 18:02:06.000000 glean-cli-0.6.0/setup.py
-drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.275496 glean-cli-0.6.0/src/
-drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.277548 glean-cli-0.6.0/src/glean/
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)       18 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/__init__.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)    28983 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/cli.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1598 2023-01-11 18:02:06.000000 glean-cli-0.6.0/src/glean/credentials.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)     3904 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/filesystem.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)    13622 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/glean_api.py
-drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.278446 glean-cli-0.6.0/src/glean/utils/
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)        0 2023-01-11 18:02:06.000000 glean-cli-0.6.0/src/glean/utils/__init__.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)      509 2023-01-11 18:02:06.000000 glean-cli-0.6.0/src/glean/utils/cli.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)     2622 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/utils/grn.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1356 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/utils/resource.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1089 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/utils/validate_config.py
-drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.279199 glean-cli-0.6.0/src/glean_cli.egg-info/
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1283 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/PKG-INFO
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)      616 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)        1 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)       41 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/entry_points.txt
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)      102 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/requires.txt
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)        6 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/top_level.txt
-drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.279964 glean-cli-0.6.0/tests/
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)      309 2023-01-11 18:02:06.000000 glean-cli-0.6.0/tests/test_cli.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1652 2023-01-11 18:02:06.000000 glean-cli-0.6.0/tests/test_credentials.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)     4632 2023-06-23 20:04:07.000000 glean-cli-0.6.0/tests/test_filesystem.py
--rw-r--r--   0 nathanielstokoe   (501) staff       (20)      666 2023-01-11 18:02:06.000000 glean-cli-0.6.0/tests/test_glean_api.py
+drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.757036 glean-cli-0.6.1/
+-rw-r--r--   0 melody     (501) staff       (20)    11357 2022-02-18 21:50:06.000000 glean-cli-0.6.1/LICENSE
+-rw-r--r--   0 melody     (501) staff       (20)     1283 2023-07-06 15:36:28.757102 glean-cli-0.6.1/PKG-INFO
+-rw-r--r--   0 melody     (501) staff       (20)      832 2023-01-03 15:16:58.000000 glean-cli-0.6.1/README.md
+-rw-r--r--   0 melody     (501) staff       (20)      103 2022-02-18 21:50:06.000000 glean-cli-0.6.1/pyproject.toml
+-rw-r--r--   0 melody     (501) staff       (20)      831 2023-07-06 15:36:28.757345 glean-cli-0.6.1/setup.cfg
+-rw-r--r--   0 melody     (501) staff       (20)       38 2022-02-18 21:50:06.000000 glean-cli-0.6.1/setup.py
+drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.752625 glean-cli-0.6.1/src/
+drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.754459 glean-cli-0.6.1/src/glean/
+-rw-r--r--   0 melody     (501) staff       (20)       18 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/__init__.py
+-rw-r--r--   0 melody     (501) staff       (20)    31870 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/cli.py
+-rw-r--r--   0 melody     (501) staff       (20)     1598 2023-01-03 15:16:58.000000 glean-cli-0.6.1/src/glean/credentials.py
+-rw-r--r--   0 melody     (501) staff       (20)     3904 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/filesystem.py
+-rw-r--r--   0 melody     (501) staff       (20)    14250 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/glean_api.py
+drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.755148 glean-cli-0.6.1/src/glean/utils/
+-rw-r--r--   0 melody     (501) staff       (20)        0 2023-01-03 15:16:58.000000 glean-cli-0.6.1/src/glean/utils/__init__.py
+-rw-r--r--   0 melody     (501) staff       (20)      509 2023-01-03 15:16:58.000000 glean-cli-0.6.1/src/glean/utils/cli.py
+-rw-r--r--   0 melody     (501) staff       (20)     2622 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/utils/grn.py
+-rw-r--r--   0 melody     (501) staff       (20)     1356 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/utils/resource.py
+-rw-r--r--   0 melody     (501) staff       (20)     1089 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/utils/validate_config.py
+drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.755877 glean-cli-0.6.1/src/glean_cli.egg-info/
+-rw-r--r--   0 melody     (501) staff       (20)     1283 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/PKG-INFO
+-rw-r--r--   0 melody     (501) staff       (20)      616 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 melody     (501) staff       (20)        1 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 melody     (501) staff       (20)       41 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/entry_points.txt
+-rw-r--r--   0 melody     (501) staff       (20)      116 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/requires.txt
+-rw-r--r--   0 melody     (501) staff       (20)        6 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/top_level.txt
+drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.756695 glean-cli-0.6.1/tests/
+-rw-r--r--   0 melody     (501) staff       (20)      309 2023-01-03 15:16:58.000000 glean-cli-0.6.1/tests/test_cli.py
+-rw-r--r--   0 melody     (501) staff       (20)     1652 2023-01-03 15:16:58.000000 glean-cli-0.6.1/tests/test_credentials.py
+-rw-r--r--   0 melody     (501) staff       (20)     4632 2023-07-06 15:35:54.000000 glean-cli-0.6.1/tests/test_filesystem.py
+-rw-r--r--   0 melody     (501) staff       (20)      666 2023-01-12 21:30:33.000000 glean-cli-0.6.1/tests/test_glean_api.py
```

### Comparing `glean-cli-0.6.0/LICENSE` & `glean-cli-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.0/PKG-INFO` & `glean-cli-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.6.0
+Version: 0.6.1
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.6.0/README.md` & `glean-cli-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.0/setup.cfg` & `glean-cli-0.6.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 install_requires = 
 	Click >= 8.0
 	pyyaml >= 6.0
 	requests >= 2.0
 	ruamel.yaml >= 0.17
 	yaspin >= 2.1.0
 	GitPython >= 3.1.30
+	semver >= 3.0.1
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	glean = glean.cli:main
```

### Comparing `glean-cli-0.6.0/src/glean/cli.py` & `glean-cli-0.6.1/src/glean/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from contextlib import suppress
 from itertools import count
 import logging
 import os
 import string
+import subprocess
 from typing import Optional, List
 from uuid import UUID, uuid3
 import webbrowser
 from pathlib import Path, PurePath, PurePosixPath
 
 import click
 import git
@@ -45,15 +46,15 @@
 MAX_COLUMN_REGEX_LENGTH = 30
 MAX_COLUMN_FILTER_CHARS = 1000
 
 
 def main():
     with cli_error_boundary(debug=GLEAN_DEBUG):
         if not _check_version():
-            logging.warn(
+            logging.warning(
                 "There is a newer version of the Glean CLI available on PyPI. Upgrade your glean-cli package for the latest features.\n"
             )
 
         cli()
 
 
 git_revision_option = click.option(
@@ -79,97 +80,131 @@
     "dbt_manifest_path",
     required=False,
     # TODO(meyer): unhide when feature is stable
     hidden=True,
     help="Path to dbt manifest JSON file (if using Glean dbt integration).",
     type=click.Path(exists=True, readable=True, file_okay=True, dir_okay=False),
 )
+run_dbt_parse_option = click.option(
+    "--dbt",
+    "run_dbt_parse",
+    required=False,
+    hidden=True,
+    help="If specified, runs `dbt parse` and uses the resulting manifest.",
+    is_flag=True,
+    default=False
+)
+dbt_parse_flags_argument = click.argument(
+    "DBT_FLAGS",
+    type=click.STRING,
+    nargs=-1,
+)
 local_path_argument = click.argument(
     "filepath", type=click.Path(exists=True), default="."
 )
+allow_dangerous_empty_build_option = click.option(
+    "--allow-dangerous-empty-build",
+    "allow_dangerous_empty_build",
+    is_flag=True,
+    default=False,
+    help="Allow builds with no config files. WARNING: this will allow a build to delete all of your resources, including non-dataops resources that depend on your dataops resources!",
+)
 
 
 @click.group(context_settings=dict(max_content_width=130))
 @click.version_option(version=VERSION, prog_name="Glean")
 @click.option(
     "--credentials-filepath",
     type=str,
     default="~/.glean/glean_access_key.json",
     show_default=True,
     help="Path to your Glean access key credentials. You can also control this by setting a "
     "GLEAN_CREDENTIALS_FILEPATH environment variable.",
     envvar="GLEAN_CREDENTIALS_FILEPATH",
 )
-@click.option(
-    "--allow-dangerous-empty-build",
-    is_flag=True,
-    default=False,
-    help="Allow builds with no config files. WARNING: this will allow a build to delete all of your resources, including non-dataops resources that depend on your dataops resources!",
-)
 @click.pass_context
-def cli(ctx, credentials_filepath, allow_dangerous_empty_build=False):
+def cli(ctx, credentials_filepath):
     """A command-line interface for interacting with Glean."""
     if GLEAN_DEBUG or GLEAN_VERBOSE_DEBUG_UNSAFE:
         _enable_http_logging()
 
     ctx.ensure_object(dict)
-    ctx.obj["allow_dangerous_empty_build"] = allow_dangerous_empty_build
     ctx.obj["credentials"] = get_credentials(os.path.expanduser(credentials_filepath))
 
 
-@cli.command()
+@cli.command(
+    "preview",
+    context_settings=dict(
+        ignore_unknown_options=True,
+    ),
+)
+@allow_dangerous_empty_build_option
 @git_revision_option
 @git_path_option
 @dbt_manifest_option
+@run_dbt_parse_option
 @local_path_argument
+@dbt_parse_flags_argument
 @click.pass_context
-def preview(ctx, git_revision, git_path, dbt_manifest_path, filepath):
+def preview(ctx, git_revision, git_path, dbt_manifest_path, filepath, run_dbt_parse, dbt_flags, allow_dangerous_empty_build):
     """Validates resource configurations and generates a preview link."""
+    dbt_manifest_path = _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags)
+
     click.echo("🏗️  Creating preview build...")
     build_results = _create_build_using_options(
         ctx,
         filepath,
         git_revision=git_revision,
         git_path=git_path,
         deploy=False,
         dbt_manifest_path=dbt_manifest_path,
+        allow_dangerous_empty_build=allow_dangerous_empty_build,
     )
     _echo_build_results(build_results, False)
 
 
 @cli.command()
+@allow_dangerous_empty_build_option
 @git_revision_option
 @git_path_option
 @dbt_manifest_option
+@run_dbt_parse_option
 @local_path_argument
+@dbt_parse_flags_argument
 @click.option(
     "--preview / --no-preview",
     default=True,
     help="Whether to generate a Preview Build before deploying.",
 )
 @click.pass_context
 def deploy(
     ctx: click.Context,
     git_revision: Optional[str],
     git_path: Optional[str],
     dbt_manifest_path: Optional[PurePath],
+    run_dbt_parse: bool,
     filepath: str,
     preview: bool,
+    dbt_flags,
+    allow_dangerous_empty_build: bool,
 ):
     """Validates and deploys resource configurations to your project."""
 
+    dbt_manifest_path = _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags)
+
     if preview:
         click.echo("🏗️  Creating preview build...")
         build_results = _create_build_using_options(
             ctx,
             filepath,
             git_revision=git_revision,
             git_path=git_path,
             deploy=False,
             dbt_manifest_path=dbt_manifest_path,
+            allow_dangerous_empty_build=allow_dangerous_empty_build,
         )
         _echo_build_results(build_results, False)
         click.echo("")
         if not click.confirm("Continue with deploy?"):
             exit(1)
 
     click.echo("🚀 Creating deploy build...")
@@ -519,14 +554,63 @@
     filename = model["name"]
     _save_config(config, filename, skip_confirmation=skip_confirmation)
 
     _echo_build_results(build_summary, False, query_name="modelPreviewBuildFromGleanDb")
     webbrowser.open(preview_model_uri(model["id"], build_summary))
 
 
+def _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags):
+    """Convenience wrapper for running `dbt parse` before `glean preview` or `glean deploy`.
+    Must be run from your Glean project directory.
+
+    Flags passed in after the Glean subcommand will be passed onwards to dbt.
+    """
+
+    if not run_dbt_parse:
+        return None
+
+    if dbt_manifest_path is not None:
+        click.echo()
+        click.echo("🚨 `--dbt-manifest` is redundant when running with `--dbt` and will be ignored.")
+        click.echo()
+    click.echo("🐇 Running `dbt parse` to generate a manifest file.")
+
+    click.echo()
+
+    dbt_flags = list(dbt_flags) or []
+    # find the dbt target dir (some manual flags parsing)
+    target_dir = Path("target")
+    with suppress(ValueError, IndexError):
+        flag_index = dbt_flags.index("--target-dir")
+        target_dir = Path(dbt_flags[flag_index + 1])
+    with suppress(StopIteration):
+        flag_index = next(
+            n for n, f in enumerate(dbt_flags) if f.startswith("--target-dir=")
+        )
+        if flag_index is not None:
+            target_dir = Path(dbt_flags[flag_index][len("--target-dir=") :])
+
+    dbt_command = (f"dbt parse " + " ".join(dbt_flags)).strip()
+    click.echo(f"$ {dbt_command}")
+    click.echo("--- dbt output ---")
+
+    ret_code = subprocess.Popen(dbt_command.split(" ")).wait()
+    click.echo("--- end of dbt output ---")
+    if ret_code != 0:
+        raise click.ClickException(f"dbt returned nonzero exit code ({ret_code})")
+
+    manifest_path = target_dir / "manifest.json"
+    if not manifest_path.is_file():
+        raise click.ClickException("⚠️ manifest file does not exist after `dbt parse` ran successfully.")
+
+    click.echo()
+    click.echo(f"✅ Using manifest file at {manifest_path}\n")
+    return manifest_path
+
+
 def _infer_if_sql(table: str) -> bool:
     """
     Guesses if the table input is a table or a SQL query.
     """
     return bool(table.count(" ") >= 3 and "select" in table.lower())
 
 
@@ -600,18 +684,18 @@
     ctx: click.Context,
     filepath: str,
     dbt_manifest_path: Optional[PurePath] = None,
     git_revision: Optional[str] = None,
     git_path: Optional[str] = None,
     deploy: bool = False,
     targets: Optional[set] = None,
+    allow_dangerous_empty_build: bool = False,
 ):
     s = Session()
     project_id = login(s, ctx.obj["credentials"])
-    allow_dangerous_empty_build = ctx.obj["allow_dangerous_empty_build"]
     if git_revision:
         return create_build_from_git_revision(
             s,
             project_id,
             git_revision,
             git_path,
             deploy,
@@ -734,31 +818,31 @@
         lines = item.split("\n")
         click.echo(click.style("*", fg=color) + "  " + lines[0])
         for line in lines[1:]:
             click.echo("   " + line)
 
 
 def _echo_resources_with_status(resources: dict, status: str, title: str):
-    models = resources[status]["models"]
+    model_bundles = resources[status]["modelBundles"]
     saved_views = resources[status]["savedViews"]
     dashboards = resources[status]["dashboards"]
     color_palettes = resources[status]["colorPalettes"]
     homepage_launchpads = resources[status]["homepageLaunchpads"]
 
     combinedResources = (
-        models + saved_views + dashboards + color_palettes + homepage_launchpads
+        model_bundles + saved_views + dashboards + color_palettes + homepage_launchpads
     )
 
     if combinedResources:
         click.echo(title)
         _echo_list(
             [
                 click.style("Model - ", fg="bright_black")
-                + click.style(r["name"], fg="white")
-                for r in models
+                + click.style(r["model"]["name"], fg="white")
+                for r in model_bundles
             ]
         )
         _echo_list(
             [
                 click.style("View - ", fg="bright_black")
                 + click.style(r["name"], fg="white")
                 for r in saved_views
@@ -815,14 +899,15 @@
     if GLEAN_VERBOSE_DEBUG_UNSAFE:
         HTTPConnection.debuglevel = 1
 
 
 def _check_version():
     from pathlib import Path
     import time, requests
+    import semver
 
     ttl = 24 * 60 * 60
     path = Path.home() / ".glean" / ".cache" / "version"
 
     try:
         os.makedirs(path.parent, exist_ok=True)
     except:
@@ -840,26 +925,26 @@
         try:
             path.unlink()  # missing_ok not available in Python 3.7
         except:
             pass
 
     try:
         with open(path, "r") as f:
-            return VERSION == f.readline().strip()
+            return semver.compare(VERSION, f.readline().strip()) >= 0
     except:
         pass
 
     # cache was stale or did not exist; fetch from pypi
     try:
         with open(path, "w+") as f:
             PACKAGE_JSON_URL = "https://pypi.org/pypi/glean-cli/json"
             resp = requests.get(PACKAGE_JSON_URL, timeout=1)
             data = resp.json()
             LATEST_VERSION: str = list(data["releases"].keys())[-1]
             f.write(LATEST_VERSION)
-            return VERSION == LATEST_VERSION
+            return semver.compare(VERSION, LATEST_VERSION) >= 0
     except Exception as e:
-        logging.warn(
+        logging.warning(
             f"Unable to check whether this is the latest version of the CLI: {e}."
         )
         # Unable to pull version information currently, just return true
         return True
```

### Comparing `glean-cli-0.6.0/src/glean/credentials.py` & `glean-cli-0.6.1/src/glean/credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.0/src/glean/filesystem.py` & `glean-cli-0.6.1/src/glean/filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.0/src/glean/glean_api.py` & `glean-cli-0.6.1/src/glean/glean_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,17 +157,16 @@
         """,
         {
             "projectId": project_id,
             "resourceType": resource_type,
             "resourceId": resource_id,
         },
     )["data"]["pullResource"]
-    res["configs"] =  [
-        Resource.from_dict(json.loads(string))
-        for string in res["configs"]
+    res["configs"] = [
+        Resource.from_dict(json.loads(string)) for string in res["configs"]
     ]
     return res
 
 
 def _parse_table_data(table_data: dict) -> Dict[str, Dict[str, str]]:
     """Formats table names for output, and returns tables names and schemas"""
     tables = table_data["data"]["getAvailableGleanDbTables"]
@@ -186,18 +185,18 @@
     return _graphql_query(
         session,
         """
         mutation CreateBuild($projectId: String!, $buildSpec: BuildSpecInput!, $deploy: Boolean!, $allowEmptyBuild: Boolean) {
             createBuild( projectId: $projectId, buildSpec: $buildSpec, deploy: $deploy, allowEmptyBuild: $allowEmptyBuild) {
                 id,
                 resources {
-                    added { models { name }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
-                    changed { models { name }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
-                    unchanged { models { name }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
-                    deleted { models { name }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
+                    added { modelBundles { model { name } }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
+                    changed { modelBundles { model { name } }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
+                    unchanged { modelBundles { model { name } }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
+                    deleted { modelBundles { model { name } }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
                 },
                 warnings,
                 errors
             }
         }
         """,
         {
@@ -284,15 +283,14 @@
                 columnsToInclude: $columnsToInclude,
                 columnsRegex: $columnsRegex,
                 addAllColumnsAsAttributes: $addAllColumnsAsAttributes,
                 ) {
                 id,
                 resources {
                     added {
-                        models { name, id }
                         modelBundles {
                             model {
                                 id,
                                 project,
                                 createdAt,
                                 updatedAt,
                                 name,
@@ -308,17 +306,17 @@
                             }
                         },
                         savedViews { name },
                         dashboards { name },
                         colorPalettes { name },
                         homepageLaunchpads { id }
                     }
-                    changed { models { name }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
-                    unchanged { models { name }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
-                    deleted { models { name }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
+                    changed { modelBundles { model { name } }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
+                    unchanged { modelBundles { model { name } }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
+                    deleted { modelBundles { model { name } }, savedViews { name }, dashboards { name }, colorPalettes { name }, homepageLaunchpads { id } }
                 },
                 warnings,
                 errors
             }
         }
         """,
         {
@@ -375,14 +373,21 @@
     graphql_exceptions = results.get("errors")
     if (
         graphql_exceptions
         and isinstance(graphql_exceptions[0], dict)
         and graphql_exceptions[0].get("message")
     ):
         error = graphql_exceptions[0]["message"]
+
+        # Must match error message in server code at glean/services/data_ops/build_management.py line #543 (as of 7/5/23).
+        if error == "No Glean config files were found, and empty builds were not enabled, so the build was aborted.":
+            error += "\n\tTo enable empty builds, use the --allow-dangerous-empty-builds flag.\n\tWARNING: This will remove all data-ops managed resources, and any resources that depend on them, from your project."
+            from glean.cli import _echo_build_errors_and_exit
+            _echo_build_errors_and_exit([error])
+
         raise ClickException(
             f"Unexpected error received from the Glean server:\n  {error}"
         )
 
     return results
```

### Comparing `glean-cli-0.6.0/src/glean/utils/grn.py` & `glean-cli-0.6.1/src/glean/utils/grn.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.0/src/glean/utils/resource.py` & `glean-cli-0.6.1/src/glean/utils/resource.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.0/src/glean/utils/validate_config.py` & `glean-cli-0.6.1/src/glean/utils/validate_config.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.0/src/glean_cli.egg-info/PKG-INFO` & `glean-cli-0.6.1/src/glean_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.6.0
+Version: 0.6.1
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.6.0/src/glean_cli.egg-info/SOURCES.txt` & `glean-cli-0.6.1/src/glean_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.0/tests/test_credentials.py` & `glean-cli-0.6.1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.0/tests/test_filesystem.py` & `glean-cli-0.6.1/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.0/tests/test_glean_api.py` & `glean-cli-0.6.1/tests/test_glean_api.py`

 * *Files identical despite different names*

