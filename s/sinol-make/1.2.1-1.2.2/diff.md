# Comparing `tmp/sinol-make-1.2.1.tar.gz` & `tmp/sinol-make-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol-make-1.2.1.tar", last modified: Wed Jul  5 10:58:09 2023, max compression
+gzip compressed data, was "sinol-make-1.2.2.tar", last modified: Thu Jul  6 11:56:22 2023, max compression
```

## Comparing `sinol-make-1.2.1.tar` & `sinol-make-1.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.447265 sinol-make-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-05 10:57:56.000000 sinol-make-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-05 10:58:09.443264 sinol-make-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-05 10:57:56.000000 sinol-make-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 10:57:56.000000 sinol-make-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:58:09.447265 sinol-make-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.439264 sinol-make-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.439264 sinol-make-1.2.1/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.439264 sinol-make-1.2.1/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.443264 sinol-make-1.2.1/src/sinol_make/commands/inwer/
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/commands/inwer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/commands/inwer/inwer_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/commands/inwer/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.443264 sinol-make-1.2.1/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    34845 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/commands/run/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.443264 sinol-make-1.2.1/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/helpers/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/helpers/package_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/helpers/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.443264 sinol-make-1.2.1/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.443264 sinol-make-1.2.1/src/sinol_make/structs/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/structs/compiler_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-05 10:57:56.000000 sinol-make-1.2.1/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.443264 sinol-make-1.2.1/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-05 10:58:09.000000 sinol-make-1.2.1/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-05 10:58:09.000000 sinol-make-1.2.1/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:58:09.000000 sinol-make-1.2.1/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 10:58:09.000000 sinol-make-1.2.1/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-05 10:58:09.000000 sinol-make-1.2.1/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 10:58:09.000000 sinol-make-1.2.1/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:58:09.443264 sinol-make-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-05 10:57:56.000000 sinol-make-1.2.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.930280 sinol-make-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-06 11:56:12.000000 sinol-make-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-06 11:56:22.930280 sinol-make-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-06 11:56:12.000000 sinol-make-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-06 11:56:12.000000 sinol-make-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:56:22.930280 sinol-make-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.926280 sinol-make-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.926280 sinol-make-1.2.2/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.926280 sinol-make-1.2.2/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.926280 sinol-make-1.2.2/src/sinol_make/commands/inwer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/commands/inwer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/commands/inwer/inwer_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/commands/inwer/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.926280 sinol-make-1.2.2/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    36255 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/commands/run/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.930280 sinol-make-1.2.2/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/helpers/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/helpers/package_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/helpers/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.930280 sinol-make-1.2.2/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.930280 sinol-make-1.2.2/src/sinol_make/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/structs/compiler_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-07-06 11:56:12.000000 sinol-make-1.2.2/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.926280 sinol-make-1.2.2/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-06 11:56:22.000000 sinol-make-1.2.2/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-06 11:56:22.000000 sinol-make-1.2.2/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:56:22.000000 sinol-make-1.2.2/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 11:56:22.000000 sinol-make-1.2.2/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-06 11:56:22.000000 sinol-make-1.2.2/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 11:56:22.000000 sinol-make-1.2.2/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:56:22.930280 sinol-make-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-06 11:56:12.000000 sinol-make-1.2.2/tests/test_util.py
```

### Comparing `sinol-make-1.2.1/LICENSE` & `sinol-make-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol-make-1.2.1/PKG-INFO` & `sinol-make-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.2.1
+Version: 1.2.2
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sinol-make-1.2.1/README.md` & `sinol-make-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sinol-make-1.2.1/pyproject.toml` & `sinol-make-1.2.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 	"PyYAML",
 	"dictdiffer"
 ]
 
 [project.optional-dependencies]
 tests = [
   "pytest",
-  "pytest-cov"
+  "pytest-cov",
+  "requests-mock",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sio2project/sinol-make"
 "Bug Tracker" = "https://github.com/sio2project/sinol-make/issues"
 
 [project.scripts]
```

### Comparing `sinol-make-1.2.1/src/sinol_make/__init__.py` & `sinol-make-1.2.2/src/sinol_make/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import sys
 
 from sinol_make import util
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 def configure_parsers():
     parser = argparse.ArgumentParser(
         prog='sinol-make',
         description='Tool for creating and testing sio2 tasks',
     )
     parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __version__)
@@ -28,14 +28,19 @@
 def main():
     parser = configure_parsers()
     commands = util.get_commands()
     args = parser.parse_args()
 
     for command in commands:
         if command.get_name() == args.command:
+            new_version = util.check_for_updates(__version__)
+            if new_version is not None:
+                print(util.warning(f'New version of sinol-make is available (your version: {__version__}, available version: {new_version}).\n'
+                                   f' You can update it by running `pip3 install sinol-make --upgrade`.'))
+
             if sys.platform == 'linux' and not util.check_oiejq():
                 print(util.warning('`oiejq` in `~/.local/bin/` not detected, installing now...'))
 
                 try:
                     if util.install_oiejq():
                         print(util.info('`oiejq` was successfully installed.'))
                     else:
```

### Comparing `sinol-make-1.2.1/src/sinol_make/commands/inwer/__init__.py` & `sinol-make-1.2.2/src/sinol_make/commands/inwer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,18 @@
     def verify_test(execution: InwerExecution) -> VerificationResult:
         """
         Verifies a test and returns the result of inwer on this test.
         """
         output_dir = os.path.join(os.getcwd(), 'cache', 'executions', execution.test_name)
         os.makedirs(output_dir, exist_ok=True)
 
-        command = f'{execution.inwer_exe_path} < {execution.test_path}'
-        process = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-        process.wait()
+        command = [execution.inwer_exe_path]
+        with open(execution.test_path, 'r') as test:
+            process = subprocess.Popen(command, stdin=test, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+            process.wait()
         exit_code = process.returncode
         out, _ = process.communicate()
 
         return VerificationResult(
             execution.test_path,
             exit_code == 0,
             out.decode('utf-8')
```

### Comparing `sinol-make-1.2.1/src/sinol_make/commands/inwer/inwer_util.py` & `sinol-make-1.2.2/src/sinol_make/commands/inwer/inwer_util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.2.1/src/sinol_make/commands/inwer/structs.py` & `sinol-make-1.2.2/src/sinol_make/commands/inwer/structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.2.1/src/sinol_make/commands/run/__init__.py` & `sinol-make-1.2.2/src/sinol_make/commands/run/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Modified version of https://sinol3.dasie.mimuw.edu.pl/oij/jury/package/-/blob/master/runner.py
 # Author of the original code: Bartosz Kostka <kostka@oij.edu.pl>
 # Version 0.6 (2021-08-29)
+import subprocess
 
 from sinol_make.commands.run.structs import ExecutionResult, ResultChange, ValidationResult, ExecutionData
 from sinol_make.helpers.parsers import add_compilation_arguments
 from sinol_make.interfaces.BaseCommand import BaseCommand
 from sinol_make.interfaces.Errors import CompilationError
 from sinol_make.helpers import compile, compiler, package_util
 import sinol_make.util as util
@@ -156,16 +157,14 @@
 
     def compile_solutions(self, solutions):
         os.makedirs(self.COMPILATION_DIR, exist_ok=True)
         os.makedirs(self.EXECUTABLES_DIR, exist_ok=True)
         print("Compiling %d solutions..." % len(solutions))
         with mp.Pool(self.cpus) as pool:
             compilation_results = pool.map(self.compile, solutions)
-        if not all(compilation_results):
-            util.exit_with_error("\nCompilation failed.")
         return compilation_results
 
 
     def compile(self, solution):
         compile_log_file = os.path.join(
             self.COMPILATION_DIR, "%s.compile_log" % package_util.get_file_name(solution))
         source_file = os.path.join(os.getcwd(), "prog", self.get_solution_from_exe(solution))
@@ -180,56 +179,72 @@
         except CompilationError as e:
             print(util.error("Compilation of file %s was unsuccessful."
                              % package_util.get_file_name(solution)))
             compile.print_compile_log(compile_log_file)
             return False
 
 
-    def execute_oiejq(self, command, result_file, output_file, answer_file, time_limit, memory_limit):
-        timeout_exit_code = os.system(command)
+    def execute_oiejq(self, command, input_file_path, answer_file_path,
+                      time_limit, memory_limit):
+        env = os.environ.copy()
+        env["MEM_LIMIT"] = f'{memory_limit}K'
+        env["MEASURE_MEM"] = "1"
+        with open(input_file_path, "r") as input_file:
+            process = subprocess.Popen(command, shell=True, stdin=input_file, stdout=subprocess.PIPE, stderr=subprocess.PIPE, env=env)
+            process.wait()
+        timeout_exit_code = process.returncode
+        lines = process.stderr.read().decode("utf-8").splitlines()
+        output = process.stdout.read().decode("utf-8").splitlines()
+
         result = ExecutionResult(None, None, None)
-        with open(result_file) as r:
-            for line in r:
-                line = line.strip()
-                if ": " in line:
-                    (key, value) = line.split(": ")[:2]
-                    if key == "Time":
-                        result.Time = self.parse_time(value)
-                    elif key == "Memory":
-                        result.Memory = self.parse_memory(value)
-                    else:
-                        setattr(result, key, value)
 
-        if timeout_exit_code == 35072:
+        for line in lines:
+            line = line.strip()
+            if ": " in line:
+                (key, value) = line.split(": ")[:2]
+                if key == "Time":
+                    result.Time = self.parse_time(value)
+                elif key == "Memory":
+                    result.Memory = self.parse_memory(value)
+                else:
+                    setattr(result, key, value)
+
+        # If timeout kills the process, the exit code should be 137.
+        # But on Arch Linux it returns the negative value of the signal that killed the process.
+        if timeout_exit_code == 137 or timeout_exit_code == -9:
             result.Status = "TL"
         elif getattr(result, "Time") is not None and result.Time > time_limit:
             result.Status = "TL"
         elif getattr(result, "Memory") is not None and result.Memory > memory_limit:
             result.Status = "ML"
         elif getattr(result, "Status") is None:
             result.Status = "RE"
         elif result.Status == "OK":
             if result.Time > time_limit:
                 result.Status = "TL"
             elif result.Memory > memory_limit:
                 result.Status = "ML"
-            elif os.system("diff -q -Z %s %s >/dev/null"
-                           % (output_file, answer_file)):
+            elif not util.lines_diff(output, open(answer_file_path).readlines()):
                 result.Status = "WA"
         else:
             result.Status = result.Status[:2]
 
         return result
 
 
-    def execute_time(self, command, result_file, output_file, answer_file, time_limit, memory_limit):
-        timeout_exit_code = os.system(command)
+    def execute_time(self, command, result_file_path, input_file_path, answer_file_path,
+                     time_limit, memory_limit):
+        with open(input_file_path, "r") as input_file:
+            process = subprocess.Popen(command, stdin=input_file, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL)
+            process.wait()
+        timeout_exit_code = process.returncode
+        output = process.stdout.read().decode("utf-8").splitlines()
 
         result = ExecutionResult(None, None, None)
-        lines = open(result_file).readlines()
+        lines = open(result_file_path).readlines()
         program_exit_code = None
         if len(lines) == 3:
             """
             If programs runs successfully, the output looks like this:
              - first line is CPU time in seconds
              - second line is memory in KB
              - third line is exit code
@@ -250,53 +265,49 @@
             result.Status = "RE"
         elif timeout_exit_code != 0:
             result.Status = "TL"
         elif result.Time > time_limit:
             result.Status = "TL"
         elif result.Memory > memory_limit:
             result.Status = "ML"
-        elif os.system("diff -q -Z %s %s >/dev/null" % (output_file, answer_file)):
+        elif not util.lines_diff(output, open(answer_file_path).readlines()):
             result.Status = "WA"
         else:
             result.Status = "OK"
 
         return result
 
 
     def run_solution(self, data_for_execution: ExecutionData):
         """
         Run an execution and return the result as ExecutionResult object.
         """
 
         (name, executable, test, time_limit, memory_limit, timetool_path) = data_for_execution
         file_no_ext = os.path.join(self.EXECUTIONS_DIR, name, self.extract_test_id(test))
-        output_file = file_no_ext + ".out"
         result_file = file_no_ext + ".res"
         hard_time_limit_in_s = math.ceil(2 * time_limit / 1000.0)
 
         if self.args.time_tool == 'oiejq':
-            command = "MEM_LIMIT=%sK MEASURE_MEM=true timeout -k %ds -s SIGKILL %ds %s %s <%s >%s 2>%s" \
-                      % (memory_limit, hard_time_limit_in_s,
-                         hard_time_limit_in_s, timetool_path,
-                         executable, test, output_file, result_file)
+            command = f'timeout -k {hard_time_limit_in_s}s -s SIGKILL {hard_time_limit_in_s}s "{timetool_path}" "{executable}"'
 
-            return self.execute_oiejq(command, result_file, output_file, self.get_output_file(test), time_limit, memory_limit)
+            return self.execute_oiejq(command, test, self.get_output_file(test), time_limit, memory_limit)
         elif self.args.time_tool == 'time':
             if sys.platform == 'darwin':
                 timeout_name = 'gtimeout'
                 time_name = 'gtime'
             elif sys.platform == 'linux':
                 timeout_name = 'timeout'
                 time_name = 'time'
             elif sys.platform == 'win32' or sys.platform == 'cygwin':
                 raise Exception("Measuring time with GNU time on Windows is not supported.")
 
-            command = f'{timeout_name} -k {hard_time_limit_in_s}s {hard_time_limit_in_s}s ' \
-                      f'{time_name} -f "%U\\n%M\\n%x" -o {result_file} {executable} <{test} >{output_file} 2>/dev/null'
-            return self.execute_time(command, result_file, output_file, self.get_output_file(test), time_limit, memory_limit)
+            command = [f'{timeout_name}', '-k', f'{hard_time_limit_in_s}s', f'{hard_time_limit_in_s}s',
+                       f'{time_name}', '-f', '%U\\n%M\\n%x', '-o', result_file, executable]
+            return self.execute_time(command, result_file, test, self.get_output_file(test), time_limit, memory_limit)
 
 
     def update_group_status(self, group_status, new_status):
         order = ["TL", "ML", "RE", "WA", "OK"]
         if order.index(new_status) < order.index(group_status):
             return new_status
         return group_status
@@ -456,20 +467,28 @@
             if result == "OK" and group != 0:
                 points += self.scores[group]
         return points
 
 
     def compile_and_run(self, solutions):
         compilation_results = self.compile_solutions(solutions)
+        compiled_solutions = []
+        for i in range(len(solutions)):
+            if compilation_results[i]:
+                compiled_solutions.append(solutions[i])
+            else:
+                self.failed_compilations.append(solutions[i])
+        compilation_results = [result for result in compilation_results if result]
+
         os.makedirs(self.EXECUTIONS_DIR, exist_ok=True)
         executables = [os.path.join(self.EXECUTABLES_DIR, package_util.get_executable(solution))
-                       for solution in solutions]
-        compiled_commands = zip(solutions, executables, compilation_results)
-        names = solutions
-        return self.run_solutions(compiled_commands, names, solutions, self.args.solutions_report)
+                       for solution in compiled_solutions]
+        compiled_commands = zip(compiled_solutions, executables, compilation_results)
+        names = compiled_solutions
+        return self.run_solutions(compiled_commands, names, compiled_solutions, self.args.solutions_report)
 
 
     def print_expected_scores(self, expected_scores):
         yaml_dict = { "sinol_expected_scores": expected_scores }
         print(yaml.dump(yaml_dict, default_flow_style=None))
 
 
@@ -482,14 +501,19 @@
                 "points": self.calculate_points(results[solution])
             }
 
         config_expected_scores = self.config.get("sinol_expected_scores", {})
         used_solutions = results.keys()
         if self.args.solutions == None and config_expected_scores: # If no solutions were specified, use all solutions from config
             used_solutions = config_expected_scores.keys()
+        used_solutions = list(used_solutions)
+
+        for solution in self.failed_compilations:
+            if solution in used_solutions:
+                used_solutions.remove(solution)
 
         used_groups = set()
         if self.args.tests == None and config_expected_scores: # If no groups were specified, use all groups from config
             for solution in config_expected_scores.keys():
                 for group in config_expected_scores[solution]["expected"]:
                     used_groups.add(group)
         else:
@@ -643,14 +667,19 @@
         elif args.time_tool == 'time':
             if sys.platform == 'win32' or sys.platform == 'cygwin':
                 util.exit_with_error('Measuring with `time` is not supported on Windows.')
             timetool_path = 'time'
 
         return compilers, timetool_path
 
+    def exit(self):
+        if len(self.failed_compilations) > 0:
+            util.exit_with_error('Compilation failed for {cnt} solution{letter}.'.format(
+                cnt=len(self.failed_compilations), letter='' if len(self.failed_compilations) == 1 else 's'))
+
     def set_scores(self):
         self.tests = package_util.get_tests(self.args.tests)
         self.groups = list(sorted(set([self.get_group(test) for test in self.tests])))
         self.scores = collections.defaultdict(int)
 
         if 'scores' not in self.config.keys():
             print(util.warning('Scores are not defined in config.yml. Points will be assigned equally to all groups.'))
@@ -733,11 +762,13 @@
 
             example_tests = [test for test in self.tests if self.get_group(test) == 0]
             if len(example_tests) == len(self.tests):
                 print(util.warning('Running only on example tests.'))
         else:
             print(util.warning('There are no tests to run.'))
 
+        self.failed_compilations = []
         solutions = self.get_solutions(self.args.solutions)
         results = self.compile_and_run(solutions)
         validation_results = self.validate_expected_scores(results)
         self.print_expected_scores_diff(validation_results)
+        self.exit()
```

### Comparing `sinol-make-1.2.1/src/sinol_make/commands/run/structs.py` & `sinol-make-1.2.2/src/sinol_make/commands/run/structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.2.1/src/sinol_make/helpers/compile.py` & `sinol-make-1.2.2/src/sinol_make/helpers/compile.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.2.1/src/sinol_make/helpers/compiler.py` & `sinol-make-1.2.2/src/sinol_make/helpers/compiler.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.2.1/src/sinol_make/helpers/package_util.py` & `sinol-make-1.2.2/src/sinol_make/helpers/package_util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.2.1/src/sinol_make/helpers/parsers.py` & `sinol-make-1.2.2/src/sinol_make/helpers/parsers.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.2.1/src/sinol_make/structs/compiler_structs.py` & `sinol-make-1.2.2/src/sinol_make/structs/compiler_structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.2.1/src/sinol_make.egg-info/PKG-INFO` & `sinol-make-1.2.2/src/sinol_make.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.2.1
+Version: 1.2.2
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sinol-make-1.2.1/src/sinol_make.egg-info/SOURCES.txt` & `sinol-make-1.2.2/src/sinol_make.egg-info/SOURCES.txt`

 * *Files identical despite different names*

