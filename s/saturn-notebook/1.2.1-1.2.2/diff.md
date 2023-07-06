# Comparing `tmp/saturn_notebook-1.2.1.tar.gz` & `tmp/saturn_notebook-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saturn_notebook-1.2.1.tar", max compression
+gzip compressed data, was "saturn_notebook-1.2.2.tar", max compression
```

## Comparing `saturn_notebook-1.2.1.tar` & `saturn_notebook-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2416 2020-08-13 16:16:46.619603 saturn_notebook-1.2.1/LICENSE.txt
--rw-r--r--   0        0        0     8090 2023-03-24 19:37:41.000000 saturn_notebook-1.2.1/README.md
--rw-r--r--   0        0        0      878 2023-03-24 22:22:56.067663 saturn_notebook-1.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2020-07-05 20:07:51.160472 saturn_notebook-1.2.1/saturn_notebook/__init__.py
--rwxr-xr-x   0        0        0    16222 2023-03-24 19:37:41.000000 saturn_notebook-1.2.1/saturn_notebook/__main__.py
--rw-r--r--   0        0        0    14772 2023-01-25 04:33:07.343325 saturn_notebook-1.2.1/saturn_notebook/cells.py
--rw-r--r--   0        0        0     1195 2020-07-05 21:53:06.049968 saturn_notebook-1.2.1/saturn_notebook/evaluate.py
--rw-r--r--   0        0        0     1423 2023-01-12 21:24:48.516804 saturn_notebook-1.2.1/saturn_notebook/image.py
--rw-r--r--   0        0        0      672 2022-11-21 16:46:07.487684 saturn_notebook-1.2.1/saturn_notebook/mpl.py
--rw-r--r--   0        0        0     8991 2023-03-24 19:37:41.000000 saturn_notebook-1.2.1/saturn_notebook/notebook.py
--rw-r--r--   0        0        0     1219 2023-01-24 22:09:57.765684 saturn_notebook-1.2.1/saturn_notebook/repl.py
--rw-r--r--   0        0        0      299 2022-12-04 20:55:31.206438 saturn_notebook-1.2.1/saturn_notebook/theme.py
--rw-r--r--   0        0        0     3718 2022-12-04 22:40:18.571225 saturn_notebook-1.2.1/saturn_notebook/traceback.py
--rw-r--r--   0        0        0     1805 2022-12-04 20:42:24.776804 saturn_notebook-1.2.1/saturn_notebook/utils.py
--rw-r--r--   0        0        0     9265 1970-01-01 00:00:00.000000 saturn_notebook-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2416 2020-08-13 16:16:46.619603 saturn_notebook-1.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     8129 2023-04-30 16:12:49.229582 saturn_notebook-1.2.2/README.md
+-rw-r--r--   0        0        0     1312 2023-07-06 01:55:46.476951 saturn_notebook-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-07-05 20:07:51.160472 saturn_notebook-1.2.2/saturn_notebook/__init__.py
+-rwxr-xr-x   0        0        0    17204 2023-04-30 16:11:51.681863 saturn_notebook-1.2.2/saturn_notebook/__main__.py
+-rw-r--r--   0        0        0    14779 2023-04-02 19:02:34.296085 saturn_notebook-1.2.2/saturn_notebook/cells.py
+-rw-r--r--   0        0        0     1195 2020-07-05 21:53:06.049968 saturn_notebook-1.2.2/saturn_notebook/evaluate.py
+-rw-r--r--   0        0        0     1423 2023-01-12 21:24:48.516804 saturn_notebook-1.2.2/saturn_notebook/image.py
+-rw-r--r--   0        0        0      672 2022-11-21 16:46:07.487684 saturn_notebook-1.2.2/saturn_notebook/mpl.py
+-rw-r--r--   0        0        0     8991 2023-03-28 20:37:32.230642 saturn_notebook-1.2.2/saturn_notebook/notebook.py
+-rw-r--r--   0        0        0     1219 2023-01-24 22:09:57.765684 saturn_notebook-1.2.2/saturn_notebook/repl.py
+-rw-r--r--   0        0        0      299 2022-12-04 20:55:31.206438 saturn_notebook-1.2.2/saturn_notebook/theme.py
+-rw-r--r--   0        0        0     3718 2022-12-04 22:40:18.571225 saturn_notebook-1.2.2/saturn_notebook/traceback.py
+-rw-r--r--   0        0        0     1805 2022-12-04 20:42:24.776804 saturn_notebook-1.2.2/saturn_notebook/utils.py
+-rw-r--r--   0        0        0     9304 1970-01-01 00:00:00.000000 saturn_notebook-1.2.2/PKG-INFO
```

### Comparing `saturn_notebook-1.2.1/LICENSE.txt` & `saturn_notebook-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `saturn_notebook-1.2.1/README.md` & `saturn_notebook-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
   * `-c, --clean`: run from scratch, ignoring the checkpoints.
   * `-a, --auto-capture`: automatically capture matplotlib figures, without `show()`.
   * `-i`, `--interactive`:
     drop into REPL (using [ptpython](https://github.com/prompt-toolkit/ptpython))
     after all the cells are processed; the results of the REPL interaction will
     be added to the notebook.
+  * `--no-mpi`: disable MPI awareness.
   * `-n, --dry-run`: don't save the result.
   * `--only-root-output`: under MPI, suppress output from all ranks other than 0.
   * `-e`, `--external notebook.zip`: use external zip archive `notebook.zip`
     to store binary content (instead of embedding it inline).
 
   Any arguments passed after `--` will be passed as `sys.argv` to the notebook.
```

### Comparing `saturn_notebook-1.2.1/saturn_notebook/__main__.py` & `saturn_notebook-1.2.2/saturn_notebook/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,16 @@
 
 from    contextlib import nullcontext
 
 from    .           import cells as c, notebook
 from    .repl       import PythonReplWithExecute
 from    .image      import show_png
 
-try:
-    from mpi4py import MPI
-    root = MPI.COMM_WORLD.Get_rank() == 0
-    using_mpi = MPI.COMM_WORLD.Get_size() > 1
-except ImportError:
-    root = True
-    using_mpi = False
+root = True
+using_mpi = False
 
 skip_repl = False
 
 # workaround for a bug in OpenMPI (or anything else that screws up the terminal size);
 # see https://github.com/willmcgugan/rich/issues/127
 import  shutil
 width = None if shutil.get_terminal_size().columns != 0 else 80
@@ -118,26 +113,40 @@
 
     if html:
         f_html.write('</body>\n')
         f_html.write('</html>\n')
 
 @argh.arg('infn', nargs='?')
 @argh.arg('outfn', nargs='?')
+@argh.arg('--no-mpi')
 @argh.arg('-n', '--dry-run')
 @argh.arg('-i', '--interactive')
 def run(infn: "input notebook",
         outfn: "output notebook (if empty, input modified in place)",
         clean: "run from scratch, ignoring checkpoints" = False,
         auto_capture: "automatically capture images" = False,
         external: "external zip archive with binary content" = '',
         debug: "show debugging information" = False,
+        no_mpi: "disable MPI awareness" = False,
         dry_run: "don't save the processed notebook" = False,
         only_root_output: "suppress output everywhere but rank 0 (for MPI)" = False,
         interactive: "run REPL after the notebook is processed" = False):
     """Run the notebook."""
+
+    global using_mpi
+    global root
+
+    if not no_mpi:
+        try:
+            from mpi4py import MPI
+            root = MPI.COMM_WORLD.Get_rank() == 0
+            using_mpi = MPI.COMM_WORLD.Get_size() > 1
+        except:
+            pass
+
     if infn and os.path.exists(infn):
         with open(infn) as f:
             cells = c.parse(f, external, info=info)
     else:
         cells = []
         if outfn and not dry_run:
             warn(f"Input file [error]{infn}[/error] doesn't exist, but given an output file [cyan]{outfn}[/cyan]; forcing [affirm]--dry-run[/affirm]")
@@ -162,14 +171,15 @@
         checkpoint = nb.find_checkpoint()
         if checkpoint is not None:
             info(f"Skipping to checkpoint {checkpoint}", style='magenta')
             nb.skip(checkpoint, output)
             info('Resuming', style="magenta")
 
     try:
+        sys.path.insert(0, os.path.dirname(infn))
         nb.process_all(output,
                        repl=lambda: run_repl(nb, output, debug=debug,
                                              prefix = [c.Blanks.create(1)], suffix = [c.Blanks.create(1), c.BreakCell.create()]),
                        force=interactive, info=info, debug=debug)
 
         if interactive:
             result = run_repl(nb, output, debug=debug)
@@ -189,14 +199,15 @@
 def run_repl(nb, output, debug = False,
              prefix = [c.Blanks.create(1), c.BreakCell.create(), c.Blanks.create(1)],
              suffix = []):
     if skip_repl:
         return
 
     if using_mpi:
+        from mpi4py import MPI
         comm = MPI.COMM_WORLD
 
     def execute_line(line):
         line += '\n'
         if using_mpi and root:
             line = comm.bcast(line, root = 0)
         cells = []
@@ -327,15 +338,15 @@
                     f.write(x)
 
             count += 1
 
 def version():
     """Show version of Saturn and its dependencies."""
     from importlib_metadata import version as ver
-    print(f"Saturn {ver('saturn_notebook')}")
+    print(f"Saturn {ver('saturn_notebook')} (Python {sys.version})")
     for dep in ['wurlitzer', 'rich', 'ptpython',
                 'dill', 'markdown', 'atomicwrites',
                 'pygments', 'more_itertools', 'matplotlib', 'nbformat']:
         print(f"   {dep} {ver(dep)}")
 
 @argh.arg('outfn', nargs='?')
 def convert(infn: "Jupyter notebook",
@@ -446,17 +457,34 @@
 
     nb = notebook.Notebook(name = infn)
     nb.add(cells)
     nb.move_all_incoming()
 
     nb.save(outfn, '')      # write without external
 
+@argh.arg('--no-mpi')
+@argh.arg('-n', '--dry-run')
+def _run(clean: "run from scratch, ignoring checkpoints" = False,
+        auto_capture: "automatically capture images" = False,
+        external: "external zip archive with binary content" = '',
+        debug: "show debugging information" = False,
+        no_mpi: "disable MPI awareness" = False,
+        dry_run: "don't save the processed notebook" = False,
+        only_root_output: "suppress output everywhere but rank 0 (for MPI)" = False):
+    """Launch Saturn REPL."""
+    run('', '', clean, auto_capture, external, debug, no_mpi, dry_run, only_root_output, True)
+
 def main():
     global argv
+
+    parser = argh.ArghParser()
+    parser.set_default_command(_run)
+
     if '--' in sys.argv:
         idx = sys.argv.index('--')
         argv = sys.argv[idx+1:]
         sys.argv = sys.argv[:idx]
-    argh.dispatch_commands([show, run, clean, image, version, convert, rehash, extract, embed])
+    parser.add_commands([show, run, clean, image, version, convert, rehash, extract, embed])
+    parser.dispatch()
 
 if __name__ == '__main__':
     main()
```

### Comparing `saturn_notebook-1.2.1/saturn_notebook/cells.py` & `saturn_notebook-1.2.2/saturn_notebook/cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     def empty(self):
         return self.composite_.empty()
 
     def show_console(self, console):
         for x in self.composite_:
             if type(x) is io.StringIO:
                 if x.getvalue():
-                    console.print(Text(x.getvalue()))
+                    console.print(Text(x.getvalue()), end='')
             elif type(x) is bytes:
                 image.show_png(x)
             elif isinstance(x,RichRenderable):
                 console.print(x)
             else:
                 console.print(Rule("[error]didn't recognize cell type[/error]"))
 
@@ -373,23 +373,20 @@
         return [self.header()]
 
 # Captures blank lines between cells
 class Blanks(Cell):
     _prefix = ''
 
     def show_console(self, console):
-        pass
+        for line in self.lines_:
+            console.print(line, end='')
 
     def show_html(self, f):
         pass
 
-    @classmethod
-    def display(cls):
-        return False
-
     @staticmethod
     def create(n):
         cell = Blanks()
         cell.lines_ = ['\n']*n
         return cell
 
 cell_types = [MarkdownCell, OutputCell, BreakCell, CheckpointCell, VariableCell, REPLCell, SaturnCell]
```

### Comparing `saturn_notebook-1.2.1/saturn_notebook/evaluate.py` & `saturn_notebook-1.2.2/saturn_notebook/evaluate.py`

 * *Files identical despite different names*

### Comparing `saturn_notebook-1.2.1/saturn_notebook/image.py` & `saturn_notebook-1.2.2/saturn_notebook/image.py`

 * *Files identical despite different names*

### Comparing `saturn_notebook-1.2.1/saturn_notebook/mpl.py` & `saturn_notebook-1.2.2/saturn_notebook/mpl.py`

 * *Files identical despite different names*

### Comparing `saturn_notebook-1.2.1/saturn_notebook/notebook.py` & `saturn_notebook-1.2.2/saturn_notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `saturn_notebook-1.2.1/saturn_notebook/repl.py` & `saturn_notebook-1.2.2/saturn_notebook/repl.py`

 * *Files identical despite different names*

### Comparing `saturn_notebook-1.2.1/saturn_notebook/traceback.py` & `saturn_notebook-1.2.2/saturn_notebook/traceback.py`

 * *Files identical despite different names*

### Comparing `saturn_notebook-1.2.1/saturn_notebook/utils.py` & `saturn_notebook-1.2.2/saturn_notebook/utils.py`

 * *Files identical despite different names*

### Comparing `saturn_notebook-1.2.1/PKG-INFO` & `saturn_notebook-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saturn-notebook
-Version: 1.2.1
+Version: 1.2.2
 Summary: Plain-text Python notebooks with checkpointing
 Home-page: https://github.com/mrzv/saturn
 License: BSD-3-Clause-LBNL
 Author: Dmitriy Morozov
 Author-email: dmitriy@mrzv.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -78,14 +78,15 @@
 
   * `-c, --clean`: run from scratch, ignoring the checkpoints.
   * `-a, --auto-capture`: automatically capture matplotlib figures, without `show()`.
   * `-i`, `--interactive`:
     drop into REPL (using [ptpython](https://github.com/prompt-toolkit/ptpython))
     after all the cells are processed; the results of the REPL interaction will
     be added to the notebook.
+  * `--no-mpi`: disable MPI awareness.
   * `-n, --dry-run`: don't save the result.
   * `--only-root-output`: under MPI, suppress output from all ranks other than 0.
   * `-e`, `--external notebook.zip`: use external zip archive `notebook.zip`
     to store binary content (instead of embedding it inline).
 
   Any arguments passed after `--` will be passed as `sys.argv` to the notebook.
```

