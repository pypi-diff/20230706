# Comparing `tmp/empack-3.0.0.tar.gz` & `tmp/empack-3.0.1.tar.gz`

## Comparing `empack-3.0.0.tar` & `empack-3.0.1.tar`

### file list

```diff
@@ -1,37 +1,33 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 empack-3.0.0/.DS_Store
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 empack-3.0.0/.bumpversion.cfg
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 empack-3.0.0/.flake8
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 empack-3.0.0/.isort.cfg
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 empack-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 empack-3.0.0/Makefile
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 empack-3.0.0/ci_env.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 empack-3.0.0/setup.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 empack-3.0.0/config/empack_config.yaml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 empack-3.0.0/empack/__init__.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 empack-3.0.0/empack/file_patterns.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 empack-3.0.0/empack/filter_env.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 empack-3.0.0/empack/micromamba_wrapper.py
--rw-r--r--   0        0        0     8252 2020-02-02 00:00:00.000000 empack-3.0.0/empack/pack.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 empack-3.0.0/empack/repodata.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 empack-3.0.0/empack/tar_utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 empack-3.0.0/empack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.0.0/empack/cli/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 empack-3.0.0/empack/cli/app.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 empack-3.0.0/empack/cli/err.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 empack-3.0.0/empack/cli/main.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 empack-3.0.0/empack/cli/pack.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 empack-3.0.0/empack/cli/repodata.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 empack-3.0.0/empack/cli/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.0.0/tests/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 empack-3.0.0/tests/conftest.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 empack-3.0.0/tests/empack_test_config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 empack-3.0.0/tests/empack_test_extra_config.yaml
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 empack-3.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 empack-3.0.0/tests/test_filter.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 empack-3.0.0/tests/test_integration.py
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 empack-3.0.0/tests/test_pack.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 empack-3.0.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 empack-3.0.0/LICENSE
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 empack-3.0.0/README.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 empack-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 empack-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 empack-3.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 empack-3.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 empack-3.0.1/ci_env.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 empack-3.0.1/setup.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 empack-3.0.1/config/empack_config.yaml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 empack-3.0.1/empack/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 empack-3.0.1/empack/file_patterns.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 empack-3.0.1/empack/filter_env.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 empack-3.0.1/empack/micromamba_wrapper.py
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 empack-3.0.1/empack/pack.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 empack-3.0.1/empack/repodata.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 empack-3.0.1/empack/tar_utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 empack-3.0.1/empack/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/app.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/err.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/main.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/pack.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/repodata.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 empack-3.0.1/empack/cli/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 empack-3.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 empack-3.0.1/tests/empack_test_config.yaml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 empack-3.0.1/tests/empack_test_extra_config.yaml
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 empack-3.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 empack-3.0.1/tests/test_filter.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 empack-3.0.1/tests/test_integration.py
+-rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 empack-3.0.1/tests/test_pack.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 empack-3.0.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 empack-3.0.1/LICENSE
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 empack-3.0.1/README.md
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 empack-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 empack-3.0.1/PKG-INFO
```

### Comparing `empack-3.0.0/config/empack_config.yaml` & `empack-3.0.1/config/empack_config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,19 @@
       - pattern: '**/tests/**/*.so'
       - pattern: '**/tests/*.py'
       - pattern: '**/tests/*.so'
       - pattern: '**/tzdata/zoneinfo/**/*.pyc'
   zlib:
     exclude_patterns:
       - pattern: '**/so'
+  itables:
+    include_patterns:
+      - pattern: '*.py'
+      - pattern: 'html/**'
+      - pattern: 'external/**'
 default:
   include_patterns:
     - pattern: '*.so'
     - pattern: '*.py'
     - pattern: '*.json'
     - pattern: 'share/zoneinfo/**'
   exclude_patterns:
```

### Comparing `empack-3.0.0/empack/file_patterns.py` & `empack-3.0.1/empack/file_patterns.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import fnmatch
 import re
-from typing import Dict, List, Optional, Union
+from typing import Optional
 
 import yaml
-from pydantic import BaseModel, Extra, Field, PrivateAttr
+from pydantic import BaseModel, Field, PrivateAttr, RootModel
 
-import warnings
 
-class FilePatternsModelBase(BaseModel, extra=Extra.forbid):
+class FilePatternsModelBase(BaseModel, extra="forbid"):
     pass
 
 
 # match based on a regex
 class RegexPattern(FilePatternsModelBase):
     regex: str
     _pattern: str = PrivateAttr()
@@ -27,74 +26,71 @@
 class UnixPattern(FilePatternsModelBase):
     pattern: str
 
     def match(self, path):
         return fnmatch.fnmatch(path, self.pattern)
 
 
-class FilePattern(BaseModel, extra=Extra.forbid):
-    __root__: Union[RegexPattern, UnixPattern]
+class FilePattern(RootModel, extra="forbid"):
+    root: RegexPattern | UnixPattern
 
     def match(self, path):
-        return self.__root__.match(path)
+        return self.root.match(path)
 
 
-class FileFilter(BaseModel, extra=Extra.forbid):
-
-    include_patterns: List[FilePattern] = Field(default_factory=list)
-    exclude_patterns: List[FilePattern] = Field(default_factory=list)
+class FileFilter(BaseModel, extra="forbid"):
+    include_patterns: list[FilePattern] = Field(default_factory=list)
+    exclude_patterns: list[FilePattern] = Field(default_factory=list)
 
     def match(self, path):
         include = False
         for ip in self.include_patterns:
             if ip.match(path):
                 include = True
         if include:
             for ep in self.exclude_patterns:
                 if ep.match(path):
                     return False
 
         return include
 
 
-class PkgFileFilter(BaseModel, extra=Extra.forbid):
-    packages: Dict[str, Union[FileFilter, List[FileFilter]]]
+class PkgFileFilter(BaseModel, extra="forbid"):
+    packages: dict[str, FileFilter | list[FileFilter]]
     default: FileFilter
 
-
     def get_filter_for_pkg(self, pkg_name):
         return self.packages.get(pkg_name, self.default)
 
     def get_filters_for_pkg(self, pkg_name):
         matchers = self.get_filter_for_pkg(pkg_name)
         if not isinstance(matchers, list):
             matchers = [matchers]
         return matchers
-    
+
     def merge(self, *others):
         for other in others:
             if other.default is not None:
                 self.default = other.default
 
             for pkg_name, filters in other.packages.items():
                 self.packages[pkg_name] = filters
 
 
 # when multiple config files are provided, the default
 # must be optional for the additional configs, otherwise
 # the would always overwrite the main default config
-class AdditionalPkgFileFilter(BaseModel, extra=Extra.forbid):
-    packages: Dict[str, Union[FileFilter, List[FileFilter]]]
-    default: Optional[FileFilter]
+class AdditionalPkgFileFilter(BaseModel, extra="forbid"):
+    packages: dict[str, FileFilter | list[FileFilter]]
+    default: Optional[FileFilter] = None
 
 
 def pkg_file_filter_from_yaml(path, *extra_path):
-
-    with open(path, "r") as pack_config_file:
+    with open(path) as pack_config_file:
         pack_config = yaml.safe_load(pack_config_file)
-        pkg_file_filter = PkgFileFilter.parse_obj(pack_config)
+        pkg_file_filter = PkgFileFilter.model_validate(pack_config)
 
     for path in extra_path:
-        with open(path, "r") as pack_config_file:
+        with open(path) as pack_config_file:
             pack_config = yaml.safe_load(pack_config_file)
-            pkg_file_filter.merge(AdditionalPkgFileFilter.parse_obj(pack_config))
+            pkg_file_filter.merge(AdditionalPkgFileFilter.model_validate(pack_config))
     return pkg_file_filter
```

### Comparing `empack-3.0.0/empack/filter_env.py` & `empack-3.0.1/empack/filter_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 
 def iterate_env_pkg_meta(env_prefix):
     meta_dir = os.path.join(env_prefix, "conda-meta")
     pkg_meta_files = glob.glob(os.path.join(meta_dir, "*.json"))
     for p in pkg_meta_files:
-        with open(p, "r") as pkg_meta_file:
+        with open(p) as pkg_meta_file:
             pkg_meta = json.load(pkg_meta_file)
             yield pkg_meta
 
 
 def write_minimal_conda_meta(pkg_meta, env_prefix):
     content = {k: pkg_meta[k] for k in ["name", "version", "build", "build_number"]}
     conda_meta_dir = Path(env_prefix) / "conda-meta"
@@ -23,22 +23,19 @@
     path = conda_meta_dir / filename
     with open(path, "w") as f:
         json.dump(content, f)
     return path
 
 
 def filter_pkg(env_prefix, pkg_meta, target_dir, matchers):
-
     included = []
     env_path = Path(env_prefix)
     files = pkg_meta["files"]
     for file in files:
-
-        for i, matcher in enumerate(matchers):
-
+        for _i, matcher in enumerate(matchers):
             include = matcher.match(path=file)
             if include:
                 included.append(file)
                 path = env_path / file
                 if path.is_symlink() and not path.exists():
                     continue
 
@@ -47,30 +44,27 @@
                 shutil.copy(os.path.join(env_prefix, file), dest_fpath)
                 break
     path = write_minimal_conda_meta(pkg_meta=pkg_meta, env_prefix=target_dir)
     included.append(path.relative_to(target_dir))
     return included
 
 
-
 def filter_env(env_prefix, target_dir, pkg_file_filter, verbose=0):
     if os.path.isdir(target_dir):
         shutil.rmtree(target_dir)
         os.makedirs(target_dir)
-    any_file = False
 
     per_pkg_included_files = {}
     for pkg_meta in iterate_env_pkg_meta(env_prefix):
-
         if verbose > 0:
             print(f"filtering {pkg_meta['name']}")
         file_filter = pkg_file_filter.get_filters_for_pkg(pkg_name=pkg_meta["name"])
 
         included_files = filter_pkg(
             env_prefix=env_prefix,
             pkg_meta=pkg_meta,
             target_dir=target_dir,
             matchers=file_filter,
         )
         per_pkg_included_files[pkg_meta["name"]] = included_files
-    
+
     return per_pkg_included_files
```

### Comparing `empack-3.0.0/empack/micromamba_wrapper.py` & `empack-3.0.1/empack/micromamba_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 import subprocess
-from pathlib import Path
 
-import subprocess
 
-def create_environment(prefix, channels=None, packages=None, platform=None, no_deps=False, relocate_prefix=None, dry_run=False, micromamba_exe=None, supress_stdout=True):
-    """
-    Creates a new environment using Micromamba.
+def create_environment(
+    prefix,
+    channels=None,
+    packages=None,
+    platform=None,
+    no_deps=False,
+    relocate_prefix=None,
+    dry_run=False,
+    micromamba_exe=None,
+    supress_stdout=True,
+):
+    """Creates a new environment using Micromamba.
 
-    Parameters:
+    Parameters
+    ----------
     prefix (str): The path to the prefix directory in which to create the environment. Defaults to None.
     channels (list[str], optional): A list of additional channels to use when searching for packages. Defaults to None.
     packages (list[str], optional): A list of packages to install in the new environment. Defaults to None.
     platform (str, optional): The platform for which to create the environment (e.g. linux-64, osx-64, win-64). Defaults to None.
     no_deps (bool, optional): Whether to skip the installation of package dependencies. Defaults to False.
     dry_run (bool, optional): Whether to perform a dry run (i.e. print the Micromamba command that would be run) without actually running the command. Defaults to False.
     micromamba_exe (str, optional): The path to the micromamba executable. Defaults to "micromamba".
     supress_stdout (bool, optional): Whether to supress the output of the Micromamba command. Defaults to True.
-    Returns:
+
+
+    Returns
+    -------
     None
     """
     if micromamba_exe is None:
         micromamba_exe = "micromamba"
     micromamba_command = [str(micromamba_exe), "create", "-y"]
 
     if prefix:
         micromamba_command += ["-p", str(prefix)]
-    
+
     if relocate_prefix:
         micromamba_command += ["--relocate-prefix", str(relocate_prefix)]
 
     if platform:
         micromamba_command += ["--platform", platform]
 
     if no_deps:
         micromamba_command += ["--no-deps"]
 
     if channels:
         for channel in channels:
-
             micromamba_command += ["-c", str(channel)]
-            
 
     if packages:
         micromamba_command += packages
 
     if dry_run:
         print("Dry run: Micromamba command that would be run:")
         print(" ".join(micromamba_command))
-    else:
-        try:
-            extra_kwargs = {}
-            if supress_stdout:
-                extra_kwargs["stdout"] = subprocess.DEVNULL
-            subprocess.run(micromamba_command, check=True, **extra_kwargs)
-        except subprocess.CalledProcessError as e:
-            raise Exception(f"Error: Micromamba command failed with return code {e.returncode}") from e
+        return
+
+    try:
+        extra_kwargs = {}
+        if supress_stdout:
+            extra_kwargs["stdout"] = subprocess.DEVNULL
+        subprocess.run(micromamba_command, check=True, **extra_kwargs)  # noqa:  #  noqa: S603
+    except subprocess.CalledProcessError as e:
+        error_message = f"Error: Micromamba command failed with return code {e.returncode}"
+        raise Exception(error_message) from e
```

### Comparing `empack-3.0.0/empack/pack.py` & `empack-3.0.1/empack/pack.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from .micromamba_wrapper import create_environment
-from .filter_env import filter_pkg, filter_env, iterate_env_pkg_meta
-from tempfile import TemporaryDirectory
-from pathlib import Path, PosixPath
-import tarfile
-import os.path
 import json
+import os
+import os.path
 import shutil
-from appdirs import user_cache_dir
 import sys
-import os
-import stat
-from .tar_utils import save_as_tarfile, ALLOWED_FORMATS
+from pathlib import Path, PosixPath
+from tempfile import TemporaryDirectory
 
+from appdirs import user_cache_dir
+
+from .filter_env import filter_env, filter_pkg, iterate_env_pkg_meta
+from .micromamba_wrapper import create_environment
+from .tar_utils import ALLOWED_FORMATS, save_as_tarfile
 
 EMPACK_CACHE_DIR = Path(user_cache_dir("empack"))
 PACKED_PACKAGES_CACHE_DIR = EMPACK_CACHE_DIR / "packed_packages_cache"
 PACKED_PACKAGES_CACHE_DIR.mkdir(parents=True, exist_ok=True)
 DEFAULT_CONFIG_PATH = Path(sys.prefix) / "share" / "empack" / "empack_config.yaml"
 
 
@@ -39,24 +38,20 @@
     outdir=None,
 ):
     if cache_dir is None:
         cache_dir = PACKED_PACKAGES_CACHE_DIR
     fname_core = f"{filename_base_from_meta(pkg_meta)}.tar.{compression_format}"
     cache_file = cache_dir / fname_core
 
-    if outdir is not None:
-        fname = os.path.join(outdir, fname_core)
-    else:
-        fname = fname_core
-
-    if use_cache:
-        if cache_file.exists():
-            if outdir is not None:
-                shutil.copy(cache_file, fname)
-            return fname_core, True
+    fname = os.path.join(outdir, fname_core) if outdir is not None else fname_core
+
+    if use_cache and cache_file.exists():
+        if outdir is not None:
+            shutil.copy(cache_file, fname)
+        return fname_core, True
 
     conda_meta_filename = f"{filename_base_from_meta(pkg_meta)}.json"
     with open(filtered_prefix / "conda-meta" / conda_meta_filename, "w") as f:
         json.dump(pkg_meta, f)
 
     # make included files absolute
     filenames = [os.path.join(filtered_prefix, f) for f in included_files]
@@ -147,16 +142,14 @@
         filtered_prefix = Path(tmp_dir) / "filtered_env"
         included_files = filter_env(
             env_prefix=env_prefix,
             target_dir=filtered_prefix,
             pkg_file_filter=file_filters,
         )
 
-        package_filenames = []
-
         packages_info = []
         for pkg_meta in iterate_env_pkg_meta(filtered_prefix):
             pack_pkg_impl(
                 included_files=included_files[pkg_meta["name"]],
                 filtered_prefix=filtered_prefix,
                 relocate_prefix=relocate_prefix,
                 pkg_meta=pkg_meta,
@@ -196,34 +189,36 @@
     outname,
     compression_format=ALLOWED_FORMATS[0],
     compresslevel=9,
     outdir=None,
 ):
     host_dir = Path(host_dir)
     if not host_dir.is_dir():
-        raise RuntimeError(f"host_dir must be a directory: {host_dir=}")
-    if outdir is not None:
-        output_filename = Path(outdir) / outname
-    else:
-        output_filename = outname
+        error = f"host_dir must be a directory: {host_dir}"
+        raise RuntimeError(error)
+    output_filename = Path(outdir) / outname if outdir is not None else outname
 
     mount_dir = PosixPath(mount_dir)
     if not mount_dir.is_absolute() or mount_dir.parts[0] != "/":
-        raise RuntimeError(
-            f'mount_dir must be an absolute path starting with "/" eg "/usr/local" or "/foo/bar" but is: {mount_dir}'
+        error_message = (
+            'mount_dir must be an absolute path starting with "/" eg "/usr/local" or "/foo/bar"'
+            f" but is: {mount_dir}"
         )
+        raise RuntimeError(error_message)
 
     # remove first part from mount_dir
     mount_dir = PosixPath(*mount_dir.parts[1:])
-    assert mount_dir.is_absolute() == False
+    if mount_dir.is_absolute():
+        error_message = f"{mount_dir} should not be absolute"
+        raise RuntimeError(error_message)
 
     # iterate over all files in host_dir and store in list
     filenames = []
     arcnames = []
-    for root, dirs, files in os.walk(host_dir):
+    for root, _dirs, files in os.walk(host_dir):
         for file in files:
             abs_path = os.path.join(root, file)
             rel_path = os.path.relpath(abs_path, host_dir)
             filenames.append(os.path.join(root, file))
             if mount_dir == PosixPath("."):
                 arcnames.append(rel_path)
             else:
@@ -244,30 +239,30 @@
     outname,
     compression_format=ALLOWED_FORMATS[0],
     outdir=None,
     compresslevel=9,
 ):
     host_file = Path(host_file)
     if not host_file.is_file():
-        raise RuntimeError(f"File {host_file} is not a file")
+        error = f"File {host_file} is not a file"
+        raise RuntimeError(error)
 
     mount_dir = PosixPath(mount_dir)
     if not mount_dir.is_absolute() or mount_dir.parts[0] != "/":
         raise RuntimeError(
             'mount_dir must be an absolute path starting with "/" eg "/usr/local" or "/foo/bar"'
         )
 
-    if outdir is not None:
-        output_filename = Path(outdir) / outname
-    else:
-        output_filename = outname
+    output_filename = Path(outdir) / outname if outdir is not None else outname
 
     # remove first part from mount_dir
     mount_dir = PosixPath(*mount_dir.parts[1:])
-    assert mount_dir.is_absolute() == False
+    if mount_dir.is_absolute() is True:
+        error = f"{mount_dir} is an absolute path"
+        raise Exception(error)
 
     save_as_tarfile(
         output_filename=output_filename,
         filenames=[host_file],
         arcnames=[mount_dir / host_file.name],
         compression_format=compression_format,
         compresslevel=compresslevel,
```

### Comparing `empack-3.0.0/empack/repodata.py` & `empack-3.0.1/empack/repodata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-import requests
 import bz2
 import io
 import json
-from pathlib import Path
 import os
+from pathlib import Path
+
+import requests
 
 
 def get_pkg_names(repodata):
     pkg_names = set()
-    for k, v in repodata.items():
-        for pkg_key, meta in v["packages"].items():
+    for _k, v in repodata.items():
+        for _pkg_key, meta in v["packages"].items():
             pkg_names.add(meta["name"])
-    # print("#",len(pkg_names))
     return pkg_names
 
 
 def pkg_name_from_dependency_str(s):
     if " " in s:
         return s.split(" ")[0]
     else:
         return s
 
 
 def remove_non_available(repodata):
-
     noarch_pkgs = repodata["noarch"]["packages"]
 
     i = 0
     while True:
         pkg_names = get_pkg_names(repodata)
         removed_one = False
         i += 1
@@ -41,17 +40,16 @@
                     removed_one = True
                     break
         if not removed_one:
             break
 
 
 def hack_fields(repodata):
-    for k, v in repodata.items():
-        for pkg_key, meta in v["packages"].items():
-
+    for _k, v in repodata.items():
+        for _pkg_key, meta in v["packages"].items():
             # fmt: off
 
             meta['md5'] = "00000000000000000000000000000000"
             meta['sha256'] = "0000000000000000000000000000000000000000000000000000000000000000"
             meta['size'] = 1
             meta['timestamp'] = 1
             meta['time_modified'] = 1
@@ -63,24 +61,21 @@
         outdir = os.getcwd()
     outdir = Path(outdir)
     outdir.mkdir(exist_ok=True, parents=True)
 
     if "arch" not in repodata_urls or "noarch" not in repodata_urls:
         raise RuntimeError("need'arch' / 'noarch' keys in repodata_urls")
 
-    # print("download")
     # download
     repodata_urls[
         "arch"
     ] = "https://beta.mamba.pm/get/emscripten-forge/emscripten-32/repodata.json.bz2"
 
-    repodata_urls[
-        "noarch"
-    ] = "https://beta.mamba.pm/get/conda-forge/noarch/repodata.json.bz2"
-    repodata_response = {k: requests.get(url) for k, url in repodata_urls.items()}
+    repodata_urls["noarch"] = "https://beta.mamba.pm/get/conda-forge/noarch/repodata.json.bz2"
+    repodata_response = {k: requests.get(url, timeout=10) for k, url in repodata_urls.items()}
     [r.raise_for_status() for r in repodata_response.values()]
 
     # unzip
     repodata = dict()
     for k, response in repodata_response.items():
         with bz2.BZ2File(io.BytesIO(response.content)) as f:
             repodata[k] = json.load(f)
@@ -99,14 +94,13 @@
             json.dump(v, fp, indent=4)
         tarbz2contents = bz2.compress(json.dumps(v).encode(), 9)
         with open(outdir / f"{k}_picomamba.bz2", "wb") as f:
             f.write(tarbz2contents)
 
 
 if __name__ == "__main__":
-
     repodata_urls = {
         "arch": "https://beta.mamba.pm/get/emscripten-forge/emscripten-32/repodata.json.bz2",
         "noarch": "https://beta.mamba.pm/get/conda-forge/noarch/repodata.json.bz2",
     }
 
     download_and_shrink_repodata(repodata_urls)
```

### Comparing `empack-3.0.0/empack/tar_utils.py` & `empack-3.0.1/empack/tar_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-import tarfile 
-import os
+import tarfile
 from pathlib import Path
 
 ALLOWED_FORMATS = ["gz"]
 
 
-def save_as_tarfile(output_filename, filenames, arcnames,  compression_format=ALLOWED_FORMATS[0], compresslevel=9):
-    
+def save_as_tarfile(
+    output_filename,
+    filenames,
+    arcnames,
+    compression_format=ALLOWED_FORMATS[0],
+    compresslevel=9,
+):
     if compression_format not in ALLOWED_FORMATS:
-        raise RuntimeError(
-            f"Compression format {compression_format} not supported, only {ALLOWED_FORMATS} are supported."
+        error_message = (
+            f"Compression format {compression_format} not supported, only {ALLOWED_FORMATS} are"
+            " supported."
         )
+        raise RuntimeError(error_message)
 
     if not Path(output_filename).parts[-1].endswith(f".tar.{compression_format}"):
-        raise RuntimeError(
+        error_message = (
             f"Output filename {output_filename} does not end with .tar.{compression_format}"
         )
+        raise RuntimeError(error_message)
 
-    with tarfile.open(output_filename, f"w:{compression_format}", compresslevel=compresslevel) as tar:
-        for file,arcname in zip(filenames, arcnames):
-            tar.add(file, arcname=arcname)
+    with tarfile.open(
+        output_filename, f"w:{compression_format}", compresslevel=compresslevel
+    ) as tar:
+        for file, arcname in zip(filenames, arcnames):
+            tar.add(file, arcname=arcname)
```

### Comparing `empack-3.0.0/empack/cli/pack.py` & `empack-3.0.1/empack/cli/pack.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from pathlib import Path
-from typing import List, Optional
+from typing import Optional
+
 import typer
-import sys
 
-from .app import app
-from .err import exit_with_err
+from empack.file_patterns import pkg_file_filter_from_yaml
+from empack.pack import DEFAULT_CONFIG_PATH, pack_env
 
-from ..pack import pack_pkg, pack_env,DEFAULT_CONFIG_PATH
-from ..file_patterns import pkg_file_filter_from_yaml
+from .app import app
 
 # packaging
 pack_app = typer.Typer()
 app.add_typer(pack_app, name="pack")
 
 
-
 @pack_app.command(
     name="env",
     help="""Pack an environment into a multiple tarballs:
-This will pack and exisiting enviroment into multiple tarballs 
+This will pack and exisiting enviroment into multiple tarballs
 and a json file with a list of package filenmmes.
 """,
 )
 def pack_env_cli(
     env_prefix: str = typer.Option(  # noqa: B008
         ...,
         "--env-prefix",
@@ -31,15 +29,15 @@
     ),
     relocate_prefix: str = typer.Option(  # noqa: B008
         "/",
         "--relocate-prefix",
         "-r",
         help="path of the env in the the virtual filesystem",
     ),
-    config: List[Path] = typer.Option(  # noqa: B008
+    config: list[Path] = typer.Option(  # noqa: B008
         [DEFAULT_CONFIG_PATH],
         "--config",
         "-c",
         help="path to a .yaml file with the empack config",
     ),
     use_cache: Optional[bool] = typer.Option(  # noqa: B008
         True,
@@ -54,21 +52,17 @@
     outdir: Optional[str] = typer.Option(  # noqa: B008
         None,
         "--outdir",
         "-o",
         help="if no output directory is specified the current workdir is used",
     ),
     compresslevel: Optional[int] = typer.Option(  # noqa: B008
-        9,
-        "--compresslevel",
-        "-l",
-        help="compression level"
+        9, "--compresslevel", "-l", help="compression level"
     ),
 ):
-
     file_filters = pkg_file_filter_from_yaml(*config)
 
     pack_env(
         env_prefix=env_prefix,
         relocate_prefix=relocate_prefix,
         file_filters=file_filters,
         outdir=outdir,
```

### Comparing `empack-3.0.0/empack/cli/repodata.py` & `empack-3.0.1/empack/cli/repodata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-import os
 from pathlib import Path
-from typing import List, Optional
-import json
+
 import typer
 
-from ..repodata import download_and_shrink_repodata
+from empack.repodata import download_and_shrink_repodata
 
 from .app import app
-from .err import exit_with_err
 
 # packaging
 repodata_app = typer.Typer()
 app.add_typer(repodata_app, name="repodata")
 
 
 @repodata_app.command()
 def shrink(
     arch: str = typer.Option(  # noqa: B008
-        "https://beta.mamba.pm/get/emscripten-forge/emscripten-32/repodata.json.bz2"
-        "--arch",
+        "https://beta.mamba.pm/get/emscripten-forge/emscripten-32/repodata.json.bz2--arch",
         "-a",
         help="arch / emscripten-32 repodata",
     ),
     no_arch: str = typer.Option(  # noqa: B008
         "https://beta.mamba.pm/get/conda-forge/noarch/repodata.json.bz2",
         "--no-arch",
         "-n",
```

### Comparing `empack-3.0.0/tests/empack_test_config.yaml` & `empack-3.0.1/tests/empack_test_config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.0.0/tests/test_cli.py` & `empack-3.0.1/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 import pytest
-from .conftest import CHANNELS
-
 from typer.testing import CliRunner
 
 from empack.cli.main import app
 from empack.micromamba_wrapper import create_environment
 
+from .conftest import CHANNELS
 
 runner = CliRunner()
 
 
-class TestCLI(object):
-
+class TestCLI:
     def test_help(self):
         result = runner.invoke(app, ["--help"])
         assert result.exit_code == 0
         assert "Usage" in result.stdout
 
     @pytest.mark.parametrize("use_cache", [False, True])
     def test_pack_env(self, tmp_path, use_cache):
-
         prefix = tmp_path / "env"
-        create_environment(prefix=prefix, packages=["numpy"], channels=CHANNELS,
-                 relocate_prefix="/", platform="emscripten-32")
-        
+        create_environment(
+            prefix=prefix,
+            packages=["numpy"],
+            channels=CHANNELS,
+            relocate_prefix="/",
+            platform="emscripten-32",
+        )
+
         use_cache_arg = "--use-cache" if use_cache else "--no-use-cache"
 
-        args = ["pack","env", "--env-prefix", str(prefix), "--relocate-prefix","/","--outdir", str(tmp_path),use_cache_arg,  "--compresslevel", "1"]
+        args = [
+            "pack",
+            "env",
+            "--env-prefix",
+            str(prefix),
+            "--relocate-prefix",
+            "/",
+            "--outdir",
+            str(tmp_path),
+            use_cache_arg,
+            "--compresslevel",
+            "1",
+        ]
 
         result = runner.invoke(app, args)
         assert result.exit_code == 0
-
```

### Comparing `empack-3.0.0/tests/test_filter.py` & `empack-3.0.1/tests/test_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 from empack.file_patterns import FileFilter, FilePattern, pkg_file_filter_from_yaml
 
 
 def test_regex_pattern():
-    fp = FilePattern.parse_obj(
+    fp = FilePattern.model_validate(
         {
             "regex": R"^(?!.*\/tests\/).*((.*.\.py$)|(.*.\.so$))|(.*dateutil-zoneinfo\.tar\.gz$)",
         }
     )
     assert fp.match("/home/fu/bar.py")
     assert fp.match("/home/fu/bar.so")
     assert not fp.match("/home/tests/fu/bar.py")
     assert not fp.match("/home/tests/fu/bar.so")
     assert fp.match("/hometests/fu/bar.py")
     assert fp.match("/hometests/fu/bar.so")
 
 
 def test_unix_pattern():
-    fp = FilePattern.parse_obj({"pattern": "*.py"})
+    fp = FilePattern.model_validate({"pattern": "*.py"})
     assert fp.match("/home/fu/bar.py")
     assert not fp.match("/hometests/fu/bar.pyc")
 
-    fp = FilePattern.parse_obj({"pattern": "**/tests/*"})
+    fp = FilePattern.model_validate({"pattern": "**/tests/*"})
     assert fp.match("/home/tests/bar")
     assert not fp.match("/home/fu/bar")
 
 
 def test_file_filter():
-    fp = FileFilter.parse_obj(
+    fp = FileFilter.model_validate(
         {
             "include_patterns": [
                 {"pattern": "*.py"},
                 {"pattern": "*.so"},
                 {"pattern": "*matplotlibrc"},
             ],
             "exclude_patterns": [{"pattern": "**/tests/*"}],
         }
     )
     assert fp.match(
-        "/tmp/xeus-python-kernel/envs/xeus-python-kernel/lib/python3.10/"
+        "/tmp/xeus-python-kernel/envs/xeus-python-kernel/lib/python3.10/"  # noqa: S108
         "site-packages/matplotlib/mpl-data/matplotlibrc"
     )
     assert fp.match("/home/fu/bar.py")
     assert fp.match("/home/fu/bar.so")
     assert not fp.match("/home/tests/fu/bar.py")
     assert not fp.match("/home/tests/fu/bar.so")
     assert fp.match("/hometests/fu/bar.py")
     assert fp.match("/hometests/fu/bar.so")
 
 
 def test_empty_file_filter():
-
-    fp = FileFilter.parse_obj({"include_patterns": [], "exclude_patterns": []})
+    fp = FileFilter.model_validate({"include_patterns": [], "exclude_patterns": []})
     assert not fp.match("/home/fu/bar.py")
     assert not fp.match("/home/fu/bar.so")
     assert not fp.match("/home/tests/fu/bar.py")
     assert not fp.match("/home/tests/fu/bar.so")
     assert not fp.match("/hometests/fu/bar.py")
     assert not fp.match("/hometests/fu/bar.so")
 
 
 def test_dataset_filter():
-
-    fp = FileFilter.parse_obj(
+    fp = FileFilter.model_validate(
         {
             "include_patterns": [{"pattern": "**/sklearn/datasets/**"}],
             "exclude_patterns": [],
         }
     )
     assert fp.match("/home/fu/sklearn/datasets/some/folder.txt")
     assert fp.match("/home/fu/sklearn/datasets/some/folder.py")
@@ -75,20 +73,16 @@
 def test_from_yaml():
     import os
 
     dn = os.path.dirname(os.path.realpath(__file__))
     config_path = os.path.join(dn, "empack_test_config.yaml")
     pkg_file_filter = pkg_file_filter_from_yaml(config_path)
 
-    assert pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(
-        path="/home/fu/bar.py"
-    )
-    assert pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(
-        path="/home/fu/bar.so"
-    )
+    assert pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(path="/home/fu/bar.py")
+    assert pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(path="/home/fu/bar.so")
     assert not pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(
         path="/home/tests/fu/bar.py"
     )
     assert not pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(
         path="/home/tests/fu/bar.so"
     )
     assert pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(
@@ -109,20 +103,16 @@
     import os
 
     dn = os.path.dirname(os.path.realpath(__file__))
     config_path = os.path.join(dn, "empack_test_config.yaml")
     extra_config_path = os.path.join(dn, "empack_test_extra_config.yaml")
     pkg_file_filter = pkg_file_filter_from_yaml(config_path, extra_config_path)
 
-    assert pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(
-        path="/home/fu/bar.py"
-    )
-    assert pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(
-        path="/home/fu/bar.so"
-    )
+    assert pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(path="/home/fu/bar.py")
+    assert pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(path="/home/fu/bar.so")
     assert not pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(
         path="/home/tests/fu/bar.py"
     )
     assert not pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(
         path="/home/tests/fu/bar.so"
     )
     assert pkg_file_filter.get_filters_for_pkg(pkg_name="fubar")[0].match(
```

### Comparing `empack-3.0.0/tests/test_integration.py` & `empack-3.0.1/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import pytest
 import textwrap
-from .conftest import CHANNELS
-
-from empack.micromamba_wrapper import create_environment
 
+import pytest
 from pyjs_code_runner.run import run
 
+from empack.micromamba_wrapper import create_environment
+
+from .conftest import CHANNELS
 
 PYJS_VERSION = "1.0.0"
 PYJS_SPEC = f"pyjs>={PYJS_VERSION}"
 
 
 @pytest.mark.parametrize("backend_type", ["browser-main", "browser-worker"])
 def test_integration(tmp_path, tmp_path_module, free_port, backend_type):
@@ -25,15 +25,14 @@
         platform="emscripten-32",
     )
 
     script_dir = tmp_path / "scripts"
     script_dir.mkdir()
     script_path = script_dir / "main.py"
 
-
     py_main = """
 import scipy
 import numpy as np
 print(np.__version__)
 print(scipy.__version__)
 from scipy.linalg import lapack
 print(lapack.dlamch("Epsilon-Machine"))
```

### Comparing `empack-3.0.0/tests/test_pack.py` & `empack-3.0.1/tests/test_pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import pytest
-from .conftest import FILE_FILTERS, CHANNELS
-import os
-from pathlib import Path
-import sys
 import json
+import os
+import tarfile
+
+import pytest
 
 from empack.file_patterns import FileFilter
-from empack.pack import pack_pkg, pack_env, pack_directory, pack_file
 from empack.micromamba_wrapper import create_environment
-import tarfile
+from empack.pack import pack_directory, pack_env, pack_file, pack_pkg
+
+from .conftest import CHANNELS, FILE_FILTERS
 
 
 # we use the python 3.10 package twice since we want
 # to test if the caching code path is working
 @pytest.mark.parametrize("pkg_spec", ["python=3.10", "numpy", "python=3.10"])
 @pytest.mark.parametrize("use_cache", [False, True])
 def test_pack_pkg(tmp_path, tmp_path_module, use_cache, pkg_spec):
@@ -76,32 +76,30 @@
     )
 
     # check that there is a json with all the packages
     env_metadata_json_path = tmp_path / "empack_env_meta.json"
     assert env_metadata_json_path.exists()
 
     # check that json file contains all packages
-    with open(env_metadata_json_path, "r") as f:
+    with open(env_metadata_json_path) as f:
         env_metadata = json.load(f)
         packages_metadata = env_metadata["packages"]
         prefix = env_metadata["prefix"]
         assert prefix == relocate_prefix
         assert len(packages_metadata) >= len(packages)
 
         for pkg in packages:
             pkg_name = pkg.split("=")[0]
 
             found = False
             for pkg_meta in packages_metadata:
                 if pkg_meta["name"] == pkg_name:
                     found = True
                     break
-            assert found, "Could not find package {} in {}".format(
-                pkg, packages_metadata
-            )
+            assert found, f"Could not find package {pkg} in {packages_metadata}"
 
     # check that there is a tar.gz file for each package
     for pkg_info in packages_metadata:
         assert pkg_info["filename"].endswith(".tar.gz")
         fname = tmp_path / pkg_info["filename"]
         assert fname.exists()
 
@@ -154,17 +152,15 @@
         file = tar.extractfile(os.path.join(mount_dir[1:], "file1.txt"))
         assert file.read().decode("utf-8") == "file1"
 
         file = tar.extractfile(os.path.join(mount_dir[1:], "file2.txt"))
         assert file.read().decode("utf-8") == "file2"
 
         file = tar.extractfile(
-            os.path.join(
-                mount_dir[1:], "nested_dir_a", "nested_dir_b", "nested_file.txt"
-            )
+            os.path.join(mount_dir[1:], "nested_dir_a", "nested_dir_b", "nested_file.txt")
         )
         assert file.read().decode("utf-8") == "nested_file"
 
 
 @pytest.mark.parametrize("mount_dir", ["/some", "/some/", "/some/nested", "/"])
 def test_pack_file(tmp_path, mount_dir):
     # create a directory with some files
```

### Comparing `empack-3.0.0/.gitignore` & `empack-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `empack-3.0.0/LICENSE` & `empack-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `empack-3.0.0/PKG-INFO` & `empack-3.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empack
-Version: 3.0.0
+Version: 3.0.1
 Summary: empack emscripten+boa
 Project-URL: Homepage, https://github.com/emscripten-forge/empack
 Author-email: Thorsten Beier <derthorstenbeier@gmail.com>
 License: 
         MIT License
         
         Copyright (c) 2022, Thorsten Beier
@@ -26,25 +26,28 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Keywords: empack
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs
 Requires-Dist: networkx
-Requires-Dist: pydantic
+Requires-Dist: pydantic<3,>=2
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: typer
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: ruff==0.0.262; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # empack
 
 Pack a mamba environment with emsdk
 
 ## Installation
@@ -60,12 +63,20 @@
 ```
 
 ## Usage
 
 You can pack the  environment (located at `/path/to/env`) with the following command:
 
 ```bash
-empack pack env --env-prefix /path/to/env --outname python_data  --config /path/to/config.yaml
+empack pack env --env-prefix /path/to/env
 ```
 
-This will generate two files `python_data.js` and `python_data.data` that you can use in the browser.
-A sample config is located in [`tests/empack_test_config.yaml`](https://github.com/emscripten-forge/empack/blob/main/tests/empack_test_config.yaml)
+This will generate a few `.tag.gz` files that correspond to the packages in the environment located at `/path/to/env`.
+
+You can also provide a custom config with the `--config` flag. A sample config is located in [`tests/empack_test_config.yaml`](https://github.com/emscripten-forge/empack/blob/main/tests/empack_test_config.yaml)
+
+
+Run the following command for more information about the other CLI parameters:
+
+```bash
+empack pack env --help
+```
```

