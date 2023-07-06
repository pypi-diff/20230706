# Comparing `tmp/lean_dojo-1.1.1.tar.gz` & `tmp/lean_dojo-1.1.2.tar.gz`

## Comparing `lean_dojo-1.1.1.tar` & `lean_dojo-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/mypy.ini
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/__init__.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/constants.py
--rw-r--r--   0        0        0    11641 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/container.py
--rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/utils.py
--rw-r--r--   0        0        0    17589 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/0001-Modify-Lean-for-proof-recording.patch
--rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/ExtractData.lean
--rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/build_lean3_repo.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/build_lean4_repo.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/cache.py
--rw-r--r--   0        0        0    17785 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/lean.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/trace.py
--rw-r--r--   0        0        0    47904 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/traced_data.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/ast/lean3/ast_utils.py
--rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/ast/lean3/expr.py
--rw-r--r--   0        0        0    74077 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/ast/lean3/node.py
--rw-r--r--   0        0        0    26808 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/data_extraction/ast/lean4/node.py
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/interaction/Lean4Repl.lean
--rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/interaction/dojo.py
--rw-r--r--   0        0        0    20967 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/src/lean_dojo/interaction/lean3_repl.lean
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/tests/data_extraction/test_trace.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/tests/interaction/test_env.py
--rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/tests/interaction/test_examples.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/tests/interaction/test_init_errors.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/tests/interaction/test_sorry.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/tests/interaction/test_timeout.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/tests/interaction/test_unexpected_errors.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/LICENSE
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/README.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 lean_dojo-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/mypy.ini
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/__init__.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/constants.py
+-rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/container.py
+-rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/utils.py
+-rw-r--r--   0        0        0    17589 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/0001-Modify-Lean-for-proof-recording.patch
+-rw-r--r--   0        0        0    12360 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/ExtractData.lean
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/build_lean3_repo.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/build_lean4_repo.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/cache.py
+-rw-r--r--   0        0        0    17785 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/lean.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/trace.py
+-rw-r--r--   0        0        0    47904 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/traced_data.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/ast/lean3/ast_utils.py
+-rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/ast/lean3/expr.py
+-rw-r--r--   0        0        0    74077 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/ast/lean3/node.py
+-rw-r--r--   0        0        0    26808 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/data_extraction/ast/lean4/node.py
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/interaction/Lean4Repl.lean
+-rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/interaction/dojo.py
+-rw-r--r--   0        0        0    20967 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/src/lean_dojo/interaction/lean3_repl.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/tests/data_extraction/test_trace.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/tests/interaction/test_env.py
+-rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/tests/interaction/test_examples.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/tests/interaction/test_init_errors.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/tests/interaction/test_sorry.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/tests/interaction/test_timeout.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/tests/interaction/test_unexpected_errors.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/LICENSE
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 lean_dojo-1.1.2/PKG-INFO
```

### Comparing `lean_dojo-1.1.1/.readthedocs.yaml` & `lean_dojo-1.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/__init__.py` & `lean_dojo-1.1.2/src/lean_dojo/__init__.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/constants.py` & `lean_dojo-1.1.2/src/lean_dojo/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Many of them are configurable via :ref:`environment-variables`.
 """
 import os
 import multiprocessing
 from pathlib import Path
 
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 CACHE_DIR = (
     Path(os.environ["CACHE_DIR"])
     if "CACHE_DIR" in os.environ
     else Path.home() / ".cache/lean_dojo"
 )
 """Cache directory for storing traced repos (see :ref:`caching`).
@@ -69,13 +69,13 @@
 DOCKER_AVAILABLE = os.system("docker version 1>/dev/null 2>/dev/null") == 0
 
 DOCKER_TAG = "yangky11/lean-dojo"
 
 if CONTAINER == "docker":
     assert (
         DOCKER_AVAILABLE
-    ), "Failed to access Docker. Please make sure Docker is running and you have access. Alternatively, you can try to run without Docker by setting the `CONTAINER` environment variable to `native`."
+    ), "Failed to access Docker. Please make sure Docker is running and you have access. Alternatively, you can try to run without Docker by setting the `CONTAINER` environment variable to `native` (see https://leandojo.readthedocs.io/en/latest/user-guide.html#advanced-running-without-docker)."
     os.system(f"docker pull {DOCKER_TAG} 1>/dev/null 2>/dev/null")
 
 MIN_LEAN3_VERSION = "v3.42.1"
 """The minimum version of Lean 3 that LeanDojo supports.
 """
```

### Comparing `lean_dojo-1.1.1/src/lean_dojo/container.py` & `lean_dojo-1.1.2/src/lean_dojo/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,19 @@
                     with report_critical_failure(
                         f"Failed to override the directory {src}"
                     ):
                         shutil.rmtree(src)
                         shutil.move(dst, src)
 
             for path in dst.parents:
-                if path.is_relative_to(cwd) and len(list(path.glob("**/*"))) == 0:
+                if (
+                    path.exists()
+                    and path.is_relative_to(cwd)
+                    and len(list(path.glob("**/*"))) == 0
+                ):
                     path.rmdir()
 
     def _build_native_command(self, command: str, envs: Dict[str, str]) -> str:
         if len(envs) == 0:
             return command
         else:
             return " ".join(f"{k}={v}" for k, v in envs.items()) + " " + command
```

### Comparing `lean_dojo-1.1.1/src/lean_dojo/utils.py` & `lean_dojo-1.1.2/src/lean_dojo/utils.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/0001-Modify-Lean-for-proof-recording.patch` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/0001-Modify-Lean-for-proof-recording.patch`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/ExtractData.lean` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/ExtractData.lean`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 namespace Pp
 
 
 private def addLine (s : String) : String :=
   if s.isEmpty then s else s ++ "\n"
 
 
--- Similar to `Meta.ppGoal` but use String instead of Format to make sure local declarations are separted by "\n".
+-- Similar to `Meta.ppGoal` but use String instead of Format to make sure local declarations are separated by "\n".
 private def ppGoal (mvarId : MVarId) : MetaM String := do
   match (← getMCtx).findDecl? mvarId with
   | none          => return "unknown goal"
   | some mvarDecl =>
     let indent         := 2
     let lctx           := mvarDecl.lctx
     let lctx           := lctx.sanitizeNames.run' { options := (← getOptions) }
@@ -142,15 +142,15 @@
 private def trim (path : FilePath) : FilePath :=
   assert! path.isRelative
   match path.components with
   | "." :: tl => mkFilePath tl
   | _ => path
 
 
-def toBuildDir (subDir: String) (path : FilePath) (ext : String) : Option FilePath :=
+def toBuildDir (subDir : String) (path : FilePath) (ext : String) : Option FilePath :=
   let path' := (trim path).withExtension ext
   match relativeTo path' "lake-packages/lean4/src" with
   | some p => some $ "lake-packages/lean4/lib" / p
   | none => match relativeTo path' "lake-packages" with
     | some p =>
       match p.components with
       | [] => none
@@ -175,14 +175,20 @@
     let comps := path'.components
       assert! comps[0]! == "build"
       match comps with
       | _ :: _ :: tl => mkFilePath tl
       | _ => "invalid path"
 
 
+-- Create all parent directories of `p` if they don't exist.
+def makeParentDirs (p : FilePath) : IO Unit := do
+  let some parent := p.parent | throw $ IO.userError s!"Unable to get the parent of {p}"
+  IO.FS.createDirAll parent
+
+
 end Path
 
 
 namespace Traversal
 
 
 private def visitTacticInfo (ctx : ContextInfo) (ti : TacticInfo) (parent : InfoTree) : TraceM Unit := do
@@ -281,14 +287,15 @@
   let some relativePath := Path.relativeTo path cwd | throw $ IO.userError s!"Invalid path: {path}"
   let json_path := (
     if is_lean then
       mkFilePath $ "lib" :: (relativePath.withExtension "ast.json").components.tail!
     else
       (Path.toBuildDir "ir" relativePath "ast.json").get!
   )
+  Path.makeParentDirs json_path
   IO.FS.writeFile json_path (toJson trace).pretty
 
   -- Print imports, similar to `lean --deps` in Lean 3.
   let mut s := ""
   for dep in headerToImports header do
     let oleanPath ← findOLean dep.module
     if oleanPath.isRelative then
@@ -309,14 +316,15 @@
 
   let dep_path := (
     if is_lean then
       mkFilePath $ "lib" :: (relativePath.withExtension "dep_paths").components.tail!
     else
       (Path.toBuildDir "ir" relativePath "dep_paths").get!
   )
+  Path.makeParentDirs dep_path
   IO.FS.writeFile dep_path s.trim
 
 
 end LeanDojo
 
 open LeanDojo
```

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/build_lean3_repo.py` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/build_lean3_repo.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import itertools
 import subprocess
 from tqdm import tqdm
 from loguru import logger
 from time import sleep, monotonic
 from pathlib import Path, PurePath
 from multiprocessing import Process
-from typing import Union, List, Optional
+from contextlib import contextmanager
+from typing import Union, List, Optional, Generator
 
 
 def run_cmd(cmd: Union[str, List[str]], capture_output: bool = False) -> Optional[str]:
     """Run a shell command.
 
     Args:
         cmd (Union[str, List[str]]): A command or a list of commands.
@@ -74,21 +75,24 @@
                 sleep(_PROGRESSBAR_UPDATE_INTERNAL - time_elapsed)
             pbar.update(num_done - pbar.n)
             if num_done >= num_total:
                 break
     print("")
 
 
-def launch_progressbar(paths: List[Union[str, Path]]) -> None:
+@contextmanager
+def launch_progressbar(paths: List[Union[str, Path]]) -> Generator[None, None, None]:
     """Launch an async progressbar to monitor the progress of tracing the repo."""
     paths = [Path(p) for p in paths]
     lean_files = list(itertools.chain.from_iterable(p.glob("**/*.lean") for p in paths))
     num_total = len(lean_files)
     p = Process(target=_monitor, args=(paths, num_total), daemon=True)
     p.start()
+    yield
+    p.kill()
 
 
 def main() -> None:
     num_procs = int(os.environ["NUM_PROCS"])
     repo_name = sys.argv[1]
     traced_repo_root = Path.cwd() / repo_name
     if repo_name == "lean":
@@ -141,19 +145,19 @@
             record_paths(dep_src_dir, traced_repo_root, modifed_lean_bin)
 
     logger.info(f"Tracing {repo_name}")
     remove_files(modifed_lean_lib, ".olean")
     modified_lean = f"{modifed_lean_bin} --ast --tsast --tspp --recursive --make --threads={num_procs}"
     io_path = modifed_lean_lib / "system/io.lean"
     run_cmd(f"{modified_lean} {io_path}", capture_output=True)
-    launch_progressbar(["_target/deps", src_dir])
-    try:
-        run_cmd(f"{modified_lean} {src_dir}", capture_output=True)
-    except subprocess.CalledProcessError as ex:
-        logger.error(ex)
-        logger.error("Please check if the repo can be built with `leanpkg build`.")
+    with launch_progressbar(["_target/deps", src_dir]):
+        try:
+            run_cmd(f"{modified_lean} {src_dir}", capture_output=True)
+        except subprocess.CalledProcessError as ex:
+            logger.error(ex)
+            logger.error("Please check if the repo can be built with `leanpkg build`.")
     record_paths(src_dir, traced_repo_root, modifed_lean_bin)
     os.chdir("..")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/build_lean4_repo.py` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/build_lean4_repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import subprocess
 from glob import glob
 from tqdm import tqdm
 from loguru import logger
 from time import sleep, monotonic
 from pathlib import Path, PurePath
 from multiprocessing import Process
-from typing import Union, List, Optional
+from contextlib import contextmanager
+from typing import Union, List, Optional, Generator
 
 
 def run_cmd(cmd: Union[str, List[str]], capture_output: bool = False) -> Optional[str]:
     """Run a shell command.
 
     Args:
         cmd (Union[str, List[str]]): A command or a list of commands.
@@ -75,23 +76,26 @@
                 sleep(_PROGRESSBAR_UPDATE_INTERNAL - time_elapsed)
             pbar.update(num_done - pbar.n)
             if num_done >= num_total:
                 break
     print("")
 
 
-def launch_progressbar(paths: List[Union[str, Path]]) -> None:
+@contextmanager
+def launch_progressbar(paths: List[Union[str, Path]]) -> Generator[None, None, None]:
     """Launch an async progressbar to monitor the progress of tracing the repo."""
     paths = [Path(p) for p in paths]
     olean_files = list(
         itertools.chain.from_iterable(p.glob("**/*.olean") for p in paths)
     )
     num_total = len(olean_files)
     p = Process(target=_monitor, args=(paths, num_total), daemon=True)
     p.start()
+    yield
+    p.kill()
 
 
 def main() -> None:
     num_procs = int(os.environ["NUM_PROCS"])
     repo_name = sys.argv[1]
     os.chdir(repo_name)
 
@@ -109,35 +113,35 @@
                 "rm build/release/stage0/src/lean",  # Remove symbolic link.
                 "mkdir lib && cp -r build/release/stage1/lib/lean lib/lean",
                 "mv src src_tmp && mkdir src && mv src_tmp src/lean",
             ]
         )
 
         logger.info(f"Tracing {repo_name}")
-        launch_progressbar(["lib"])
-        run_cmd(
-            f"./build/release/stage1/bin/lean --threads {num_procs} --run ExtractData.lean",
-            capture_output=True,
-        )
+        with launch_progressbar(["lib"]):
+            run_cmd(
+                f"./build/release/stage1/bin/lean --threads {num_procs} --run ExtractData.lean",
+                capture_output=True,
+            )
 
     else:
         # Build the repo using lake.
         run_cmd(f"lake build")
 
         # Copy the Lean 4 stdlib into lake-packages.
         lean_prefix = run_cmd(f"lean --print-prefix", capture_output=True).strip()
         shutil.copytree(lean_prefix, "lake-packages/lean4")
 
         # Run ExtractData.lean to extract ASTs and tactic states.
         logger.info(f"Tracing {repo_name}")
-        launch_progressbar(["build"])
-        run_cmd(
-            f"lake env lean --threads {num_procs} --run ExtractData.lean",
-            capture_output=True,
-        )
+        with launch_progressbar(["build", "lake-packages"]):
+            run_cmd(
+                f"lake env lean --threads {num_procs} --run ExtractData.lean",
+                capture_output=True,
+            )
 
         num_json = len(glob("build/ir/**/*.ast.json", recursive=True))
         num_dep = len(glob("build/ir/**/*.dep_paths", recursive=True))
         num_c = len(glob("build/ir/**/*.c", recursive=True))
         assert num_json == num_dep == num_c, f"{num_json} {num_dep} {num_c}"
```

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/cache.py` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/cache.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/lean.py` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/lean.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/trace.py` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/trace.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/traced_data.py` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/traced_data.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/ast/lean3/expr.py` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/ast/lean3/expr.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/ast/lean3/node.py` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/ast/lean3/node.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/data_extraction/ast/lean4/node.py` & `lean_dojo-1.1.2/src/lean_dojo/data_extraction/ast/lean4/node.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/interaction/Lean4Repl.lean` & `lean_dojo-1.1.2/src/lean_dojo/interaction/Lean4Repl.lean`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/interaction/dojo.py` & `lean_dojo-1.1.2/src/lean_dojo/interaction/dojo.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/src/lean_dojo/interaction/lean3_repl.lean` & `lean_dojo-1.1.2/src/lean_dojo/interaction/lean3_repl.lean`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/tests/conftest.py` & `lean_dojo-1.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/tests/interaction/test_env.py` & `lean_dojo-1.1.2/tests/interaction/test_env.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/tests/interaction/test_examples.py` & `lean_dojo-1.1.2/tests/interaction/test_examples.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/tests/interaction/test_init_errors.py` & `lean_dojo-1.1.2/tests/interaction/test_init_errors.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/tests/interaction/test_sorry.py` & `lean_dojo-1.1.2/tests/interaction/test_sorry.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/tests/interaction/test_timeout.py` & `lean_dojo-1.1.2/tests/interaction/test_timeout.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/tests/interaction/test_unexpected_errors.py` & `lean_dojo-1.1.2/tests/interaction/test_unexpected_errors.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/.gitignore` & `lean_dojo-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/LICENSE` & `lean_dojo-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.1.1/pyproject.toml` & `lean_dojo-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "/docs",
   "/images",
   "/scripts",
 ]
 
 [project]
 name = "lean-dojo"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Kaiyu Yang", email="kaiyuy@caltech.edu" },
 ]
 description = "LeanDojo: Machine Learning for Theorem Proving in Lean"
 keywords = ["theorem proving", "machine learning", "Lean"]
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `lean_dojo-1.1.1/PKG-INFO` & `lean_dojo-1.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lean-dojo
-Version: 1.1.1
+Version: 1.1.2
 Summary: LeanDojo: Machine Learning for Theorem Proving in Lean
 Project-URL: Homepage, https://leandojo.org/
 Project-URL: Bug Tracker, https://github.com/lean-dojo/LeanDojo/issues
 Author-email: Kaiyu Yang <kaiyuy@caltech.edu>
 License: MIT License
         
         Copyright (c) 2023 LeanDojo Team
@@ -77,17 +77,18 @@
 
 [![Documentation Status](https://readthedocs.org/projects/leandojo/badge/?version=latest)](https://leandojo.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/lean-dojo)](https://pypi.org/project/lean-dojo/) [![GitHub license](https://img.shields.io/github/license/MineDojo/MineDojo)](https://github.com/MineDojo/MineDojo/blob/main/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
 
 ______________________________________________________________________
 
 ## Requirements
 
-* Linux or macOS
+* Supported platforms: Linux, Windows (WSL), and macOS (:warning: experimental for Apple silicon)
 * Git >= 2.25
-* Python >= 3.9
+* 3.9 <= Python <= 3.10
+* wget
 * Docker strongly recommended
 
 
 ## Installation
 
 LeanDojo is available on [PyPI](https://pypi.org/project/lean-dojo/) and can be installed via pip:
 ```bash
@@ -95,40 +96,41 @@
 ```
 
 It can also be installed locally from the Git repo:
 ```bash
 pip install .
 ```
 
+:warning: **Known issue**: If you encounter errors related to `ray` and `pydantic`, see this temporary workaround: https://github.com/ray-project/ray/issues/37019. The error will be fixed when Ray 2.6 is released.
 
 ## Documentation
 
 * [Getting Started](https://leandojo.readthedocs.io/en/latest/getting-started.html)
 * [Demo](https://github.com/lean-dojo/LeanDojo/blob/main/scripts/demo.ipynb)
 * [Full documentation](https://leandojo.readthedocs.io/en/latest/index.html)
 
 
 ## Questions and Bugs
 
 * For general questions and discussions, please use [GitHub Discussions](https://github.com/lean-dojo/LeanDojo/discussions).  
-* To report a potential bug, please open an issue.
+* To report a potential bug, please open an issue. In the issue, please include your OS information, the exact steps to reproduce the error, and complete logs in debug mode (setting the environment variable `VERBOSE` to 1). The more details you provide, the better we will be able to help you. 
 
 
 ## Related Links
 
 * [LeanDojo Website](https://leandojo.org/): The official website of LeanDojo.
 * [LeanDojo Benchmark](https://zenodo.org/record/8016386) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8016386.svg)](https://doi.org/10.5281/zenodo.8016386): The dataset used in our paper, consisting of 96,962 theorems and proofs extracted from [mathlib](https://github.com/leanprover-community/mathlib/commits/8c1b484d6a214e059531e22f1be9898ed6c1fd47) by [generate-benchmark-lean3.ipynb](./scripts/generate-benchmark-lean3.ipynb). 
 * [LeanDojo Benchmark 4](https://zenodo.org/record/8040110) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8040110.svg)](https://doi.org/10.5281/zenodo.8040110): The Lean 4 version of LeanDojo Benchmark, consisting of 91,766 theorems and proofs extracted from [mathlib4](https://github.com/leanprover-community/mathlib4/commit/5a919533f110b7d76410134a237ee374f24eaaad) by [generate-benchmark-lean4.ipynb](./scripts/generate-benchmark-lean4.ipynb).
 * [ReProver](https://github.com/lean-dojo/ReProver): The ReProver (Retrieval-Augmented Prover) model in our paper.
 * [LeanDojo ChatGPT Plugin](https://github.com/lean-dojo/LeanDojoChatGPT)
 
 
 ## Citation
 
-[LeanDojo: Theorem Proving with Retrieval-Augmented Language Models](https://arxiv.org/abs/xxxx.xxxxx)      
+[LeanDojo: Theorem Proving with Retrieval-Augmented Language Models](https://leandojo.org/)      
 Under review, NeurIPS (Datasets and Benchmarks Track), 2023  
 [Kaiyu Yang](https://yangky11.github.io/), [Aidan Swope](https://aidanswope.com/about), [Alex Gu](https://minimario.github.io/), [Rahul Chalamala](https://rchalamala.github.io/),  
 [Peiyang Song](https://www.linkedin.com/in/peiyang-song-3279b3251/), [Shixing Yu](https://billysx.github.io/), [Saad Godil](https://www.linkedin.com/in/saad-godil-9728353/), [Ryan Prenger](https://www.linkedin.com/in/ryan-prenger-18797ba1/), [Anima Anandkumar](http://tensorlab.cms.caltech.edu/users/anima/)
 
 ```bibtex
 @article{yang2023leandojo,
   title={{LeanDojo}: Theorem Proving with Retrieval-Augmented Language Models},
```

