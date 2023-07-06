# Comparing `tmp/micropython_magic-0.3.1.tar.gz` & `tmp/micropython_magic-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_magic-0.3.1.tar", max compression
+gzip compressed data, was "micropython_magic-0.4.0.tar", max compression
```

## Comparing `micropython_magic-0.3.1.tar` & `micropython_magic-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1090 2023-04-13 20:20:40.063549 micropython_magic-0.3.1/LICENSE
--rw-r--r--   0        0        0     1424 2023-06-29 18:52:04.239019 micropython_magic-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6364 2023-06-29 18:39:42.591892 micropython_magic-0.3.1/readme.md
--rw-r--r--   0        0        0      875 2023-06-29 18:39:42.635353 micropython_magic-0.3.1/src/micropython_magic/__init__.py
--rw-r--r--   0        0        0     3611 2023-06-29 18:39:42.637353 micropython_magic-0.3.1/src/micropython_magic/interactive.py
--rw-r--r--   0        0        0      773 2023-06-29 18:39:42.638770 micropython_magic-0.3.1/src/micropython_magic/magic_transformer.py
--rw-r--r--   0        0        0    26107 2023-06-29 18:51:41.327067 micropython_magic-0.3.1/src/micropython_magic/memoryinfo.py
--rw-r--r--   0        0        0     4816 2023-06-29 18:39:42.640926 micropython_magic-0.3.1/src/micropython_magic/mpr.py
--rw-r--r--   0        0        0    11949 2023-06-29 18:39:42.643280 micropython_magic-0.3.1/src/micropython_magic/octarine.py
--rw-r--r--   0        0        0      488 2023-06-07 09:44:35.636682 micropython_magic-0.3.1/src/micropython_magic/param_fixup.py
--rw-r--r--   0        0        0     2928 2023-06-29 18:39:42.645270 micropython_magic-0.3.1/src/micropython_magic/test_magics.py
--rw-r--r--   0        0        0     7111 1970-01-01 00:00:00.000000 micropython_magic-0.3.1/setup.py
--rw-r--r--   0        0        0     6890 1970-01-01 00:00:00.000000 micropython_magic-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-13 20:20:40.063549 micropython_magic-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1492 2023-07-06 14:02:07.913898 micropython_magic-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6364 2023-06-29 18:39:42.591892 micropython_magic-0.4.0/readme.md
+-rw-r--r--   0        0        0      877 2023-07-06 14:02:07.933922 micropython_magic-0.4.0/src/micropython_magic/__init__.py
+-rw-r--r--   0        0        0     5497 2023-07-06 12:34:39.272049 micropython_magic-0.4.0/src/micropython_magic/interactive.py
+-rw-r--r--   0        0        0      773 2023-06-29 18:39:42.638770 micropython_magic-0.4.0/src/micropython_magic/magic_transformer.py
+-rw-r--r--   0        0        0    26107 2023-06-29 18:51:41.327067 micropython_magic-0.4.0/src/micropython_magic/memoryinfo.py
+-rw-r--r--   0        0        0     5093 2023-07-06 10:21:54.314700 micropython_magic-0.4.0/src/micropython_magic/mpr.py
+-rw-r--r--   0        0        0    12264 2023-07-06 12:54:55.520197 micropython_magic-0.4.0/src/micropython_magic/octarine.py
+-rw-r--r--   0        0        0      488 2023-06-07 09:44:35.636682 micropython_magic-0.4.0/src/micropython_magic/param_fixup.py
+-rw-r--r--   0        0        0     4105 2023-07-06 11:01:06.908674 micropython_magic-0.4.0/src/micropython_magic/scripts/fw_info.py
+-rw-r--r--   0        0        0     2928 2023-06-29 18:39:42.645270 micropython_magic-0.4.0/src/micropython_magic/test_magics.py
+-rw-r--r--   0        0        0     7140 1970-01-01 00:00:00.000000 micropython_magic-0.4.0/setup.py
+-rw-r--r--   0        0        0     6890 1970-01-01 00:00:00.000000 micropython_magic-0.4.0/PKG-INFO
```

### Comparing `micropython_magic-0.3.1/LICENSE` & `micropython_magic-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.1/pyproject.toml` & `micropython_magic-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-magic"
-version = "0.3.1"
+version = "0.4.0"
 description = "MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs"
 keywords = [
     "MicroPython",
     "stubs",
     "Jupyter",
     "notebooks",
     "Jupyter Labs",
@@ -38,14 +38,15 @@
 pylance = "^0.4.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.poetry_bumpversion.file."src/micropython_magic/__init__.py"]
 # configuration for Black.
 
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
```

### Comparing `micropython_magic-0.3.1/readme.md` & `micropython_magic-0.4.0/readme.md`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.1/src/micropython_magic/__init__.py` & `micropython_magic-0.4.0/src/micropython_magic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """MicroPython magics for Jupyter Notebooks and JupyterLabs"""
-__version__ = "0.2.0"
+__version__ = "0.4.0"
 __author__ = "Jos Verlinde"
 
 
 from IPython.core.interactiveshell import InteractiveShell
 from loguru import logger as log
 
 from .magic_transformer import comment_magic_transformer
@@ -12,15 +12,15 @@
 
 
 def load_ipython_extension(ipython: InteractiveShell):
     # register the input transformer to allow %%cell_magics in comments
     ipython.input_transformers_cleanup.append(comment_magic_transformer)
     # register the magics
     ipython.register_magics(MpyMagics)
-    ipython.register_magics(TestMagics)
+    # ipython.register_magics(TestMagics)
 
 
 def unload_ipython_extension(ipython: InteractiveShell):
     # unregister the magics, allows to unload / reload the extension
     # ipython.magics_manager.magics["cell"].pop("mpy", None)
     # TODO
     pass
```

### Comparing `micropython_magic-0.3.1/src/micropython_magic/interactive.py` & `micropython_magic-0.4.0/src/micropython_magic/interactive.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,138 @@
 import asyncio
 import subprocess
+from dataclasses import dataclass
 from threading import Timer
-from typing import List, Tuple, Union
+from typing import List, Union
 
 from IPython.core.getipython import get_ipython
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.utils.text import SList
 from loguru import logger as log
 
 TIMEOUT = 300
 from .memoryinfo import RE_ALL
 
 
+@dataclass
+class LogTags:
+    reset_tags: List[str]
+    error_tags: List[str]
+    warning_tags: List[str]
+    success_tags: List[str]
+    ignore_tags: List[str]
+
+
+DEFAULT_LOG_TAGS = LogTags(
+    reset_tags=["rst cause:1, boot mode:"],
+    error_tags=["Error: ", "Exception: ", "ERROR :", "CRIT  :"],  # "Traceback ",
+    warning_tags=["WARNING:", "WARN  :"],
+    success_tags=["SUCCESS", "SUCCESS~"],
+    ignore_tags=['  File "<stdin>",'],
+)
+
+
 def ipython_run(
-    cmd: Union[List[str], str],
+    cmd: Union[list[str], str],
     stream_out=True,
     timeout: Union[int, float] = TIMEOUT,
     shell: bool = False,
     hide_meminfo: bool = False,
     store_output: bool = True,
+    log_errors: bool = True,
+    tags: LogTags = DEFAULT_LOG_TAGS,
 ) -> SList:
     """Run an external command stream the output back to the Ipython console.
     args:
         cmd: the command to run, as a list of strings or a single string
         stream_out: stream the output back to the console as it is received (per line)
-        timeout: the timeout in seconds, defaults to 300 seconds
+        timeout: the timeout in seconds, defaults to 300 seconds (5 mins)
         shell: run the command in a shell
         hide_meminfo: hide the output of  micropython.mem_info() from the console ( it will still be available in the execution value)
         store_output: store the output of the command in the ipython kernel namespace
 
     returns:
         (exit_code:int, output:List[str])
         a tuple of the exit code of the command and the output of the command
     """
     # Only implement line based reading and parsing for now
     # it is, faster, easier to implement and more useful for parsing regexes
     line_based = True
+    forever = timeout == 0
+    timeout = abs(timeout)
+
     all_out = []
     # if stream_out:
     #     # InteractiveShell.ast_node_interactivity = "all"
     #     pass
     log.trace(f"per char , with timeout of {timeout} seconds")
-    assert timeout > 0
+    # assert timeout > 0
     try:
         process = subprocess.Popen(
             cmd, shell=shell, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )  # ,  universal_newlines=True)
     except FileNotFoundError as e:
         raise FileNotFoundError(f"Failed to start {cmd[0]}") from e
 
     assert process.stdout is not None
 
-    def timed_out():
-        process.kill()
-        log.warning(f"Command {cmd} timed out after {timeout} seconds")
-
-    process_timer = Timer(interval=timeout, function=timed_out)
-    process_timer.start()
-    while True:
-        # await asyncio.sleep(0.1)
-        if line_based:
-            output = process.stdout.readline()
-            output = output.decode("utf-8", errors="ignore")
-
-            if hide_meminfo and output and any(re.match(output) for re in RE_ALL):
+    process_timer = None
+    try:
+        if not forever:
+            # only if a timeout was specified start a timer to kill the process
+            def timed_out():
+                process.kill()
+                log.warning(f"Command {cmd} timed out after {timeout} seconds")
+
+            process_timer = Timer(interval=timeout, function=timed_out)
+            process_timer.start()
+        while forever or (process_timer and process_timer.is_alive()):
+            if line_based:
+                output = process.stdout.readline()
+                output = output.decode("utf-8", errors="ignore")
+                # detect board reset
+                if any(tag in output for tag in tags.reset_tags):
+                    raise RuntimeError(f"Board reset detected : {output}")
+                # detect errors
+                if log_errors and any(tag in output for tag in tags.error_tags):
+                    log.error(output)
+                # detect warnings
+                if any(tag in output for tag in tags.warning_tags):
+                    log.warning(output)
+                # detect success
+                if any(tag in output for tag in tags.success_tags):
+                    log.success(output)
+                # ignore some tags
+                if any(tag in output for tag in tags.ignore_tags):
+                    continue
                 # do not output the line that matched a meminfo regex
-                continue
-        else:
-            output = process.stdout.read(1)
-            output = output.decode("utf-8", errors="ignore")
-            # ToDo # swallow the output if it matches a regex
-
-        if output == "" and process.poll() is not None:
-            # process has finished, read the rest of the output before breaking out of the loop
-            break
-        if output:
-            all_out.append(output)
-            if stream_out:
-                print(output, end="")
-
-    process_timer.cancel()
-    # rearrange the output to be a list of lines
-    all_out = SList("".join(all_out).splitlines())
-    if store_output:
-        # update the ipython kernel namespace with the output of the command
-        # this is useful for storing the output of a command in a variable
-        # Normally the output of a command is not stored in the kernel namespace
-        ipy: InteractiveShell = get_ipython()  # type: ignore
-        ipy.displayhook.fill_exec_result(all_out)
-        ipy.displayhook.update_user_ns(all_out)
-    return all_out
+                if hide_meminfo and output and any(re.match(output) for re in RE_ALL):
+                    continue
+            else:
+                output = process.stdout.read(1)
+                output = output.decode("utf-8", errors="ignore")
+                # ToDo # swallow the output if it matches a regex
+
+            if output == "" and process.poll() is not None:
+                # process has finished, read the rest of the output before breaking out of the loop
+                break
+            if output:
+                all_out.append(output)
+                if stream_out:
+                    print(output, end="")
+
+        # rearrange the output to be a list of lines
+        all_out = SList("".join(all_out).splitlines())
+        if store_output:
+            # update the ipython kernel namespace with the output of the command
+            # this is useful for storing the output of a command in a variable
+            # Normally the output of a command is not stored in the kernel namespace
+            ipy: InteractiveShell = get_ipython()  # type: ignore
+            ipy.displayhook.fill_exec_result(all_out)
+            ipy.displayhook.update_user_ns(all_out)
+        return all_out
+    finally:
+        if process.stderr and log_errors:
+            for line in process.stderr:
+                log.warning(line)
+        if process_timer and process_timer.is_alive():
+            process_timer.cancel()
```

### Comparing `micropython_magic-0.3.1/src/micropython_magic/magic_transformer.py` & `micropython_magic-0.4.0/src/micropython_magic/magic_transformer.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.1/src/micropython_magic/memoryinfo.py` & `micropython_magic-0.4.0/src/micropython_magic/memoryinfo.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.1/src/micropython_magic/mpr.py` & `micropython_magic-0.4.0/src/micropython_magic/mpr.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,81 +3,92 @@
 
 import contextlib
 import json
 import tempfile
 from pathlib import Path
 from typing import List, Optional, Union
 
-import IPython
-from colorama import Style
 from IPython.core.interactiveshell import InteractiveShell
-from IPython.utils.text import LSString, SList
 from loguru import logger as log
 
 from .interactive import ipython_run
 
 JSON_START = "<json~"
 JSON_END = "~json>"
 DONT_KNOW = "<~?~>"
 
 from .interactive import TIMEOUT
 
 
 class MPRemote2:
-    def __init__(self, shell: InteractiveShell, port: str = "auto", resume: bool = True):
+    def __init__(self, shell: InteractiveShell, port: str = "auto", resume: bool = True,):
         self.shell: InteractiveShell = shell
-        self.port: str = "auto"  # by default connect to the first device
+        self.port: str = port  # by default connect to the first device
         self.resume = resume  # by default resume the device to maintain state
         self.timeout = TIMEOUT
 
     @property
     def cmd_prefix(self):
         """mpremote command prefix including port and resume according to options"""
         return f"mpremote {self.connect_to}{'resume' if self.resume else ''} "
 
     @property
     def connect_to(self):
         "Creates mpremote 'connect to string' if port is specified."
         return f"connect {self.port} " if self.port else ""
 
-    def run_cmd(self, cmd: str, *, auto_connect: bool = True, stream_out: bool = True, shell=True, timeout=0):
+    def run_cmd(
+        self,
+        cmd: Union[str, List[str]],
+        *,
+        auto_connect: bool = True,
+        stream_out: bool = True,
+        shell=True,
+        timeout: Union[int, float] = 0,
+    ):
         """run a command on the device and return the output"""
         if auto_connect:
-            cmd = f"""{self.cmd_prefix} {cmd}"""
+            if isinstance(cmd, str):
+                cmd = f"""{self.cmd_prefix} {cmd}"""
+            else:
+                log.warning(f"cmd is not a string: {cmd}")
         log.debug(cmd)
         return ipython_run(cmd, stream_out=stream_out, shell=shell, timeout=timeout or self.timeout)
 
         # output = self.shell.getoutput(cmd, split=True)
         # assert isinstance(output, SList)
         # if len(output) > 0 and output[0].strip() == "no device found":
         #     raise ConnectionError("no device found")
         # return output
 
-    def select_device(self, line: Optional[str]):
+    def select_device(self, port: Optional[str], verify: bool = False):
         """try to select the device to connect to by specifying the serial port name."""
-        _port = line.strip() if line else "auto"
-        cmd = f"""eval \"'Checking connection to MCU on port {_port}.'\""""
+        _port = port.strip() if port else "auto"
+        if not verify:
+            self.port = _port
+            return _port
+        cmd = f"""eval \"'{_port}'\""""
         try:
             output = self.run_cmd(cmd)
             self.port = _port
         except Exception as e:
             output = e
         return output
 
-    def run_cell(self, cell: str):
+    def run_cell(self, cell: str, *, timeout: Union[int, float] = TIMEOUT):
         """run a codeblock on the device and return the output"""
         #     # TODO: if the cell is small enough, concat the cell with \n an use exec instead of copy
         #     # - may need escaping quotes and newlines
         # copy the cell to a file on the device
         self.cell_to_mcu_file(cell, "__magic.py")
         # run the transferred cell/file
-        result = self.run_mcu_file("__magic.py", stream_out=True)
+        result = self.run_mcu_file("__magic.py", stream_out=True, timeout=timeout)
         return
 
-    def run_mcu_file(self, filename: str, stream_out: bool = True, timeout: int = 0):
+    def run_mcu_file(self, filename: str, stream_out: bool = True, timeout: Union[int, float] = 0):
         exec_cmd = f"exec \"exec( open('{filename}').read() , globals() )\""
         return self.run_cmd(exec_cmd, stream_out=stream_out, timeout=timeout)
 
     def cell_to_mcu_file(self, cell, filename):
         with tempfile.NamedTemporaryFile(mode="w", suffix=".py", delete=False) as f:
             f.write("# Jupyter cell\n")  # add a line to replace the cell magic to keep the line numbers aligned
             f.write(cell)
```

### Comparing `micropython_magic-0.3.1/src/micropython_magic/octarine.py` & `micropython_magic-0.4.0/src/micropython_magic/octarine.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 """
 
 import argparse
 import re
 import sys
 from typing import List, Optional
 
+import pkg_resources
 from colorama import Style
 from IPython.core.error import UsageError
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.core.magic import Magics, cell_magic, line_magic, magics_class, output_can_be_silenced
 from IPython.core.magic_arguments import argument, argument_group, magic_arguments, parse_argstring
 from IPython.utils.text import LSString, SList
 from loguru import logger as log
 
+from micropython_magic.interactive import TIMEOUT
 from micropython_magic.param_fixup import get_code
 
 from .mpr import DONT_KNOW, JSON_END, JSON_START, MPRemote2
 
 # https://ipython.readthedocs.io/en/stable/config/custommagics.html
 # https://ipython.readthedocs.io/en/stable/api/generated/IPython.core.magic.html#IPython.core.magic.Magics
 # https://nbviewer.org/github/rossant/ipython-minibook/blob/master/chapter6/602-cpp.ipynb
@@ -54,25 +56,14 @@
 
     def __repr__(self):
         return repr(self.data)
 
     def _str_(self):
         return "\n".join(self.data.list)
 
-    # def _repr_pretty_(self, pp, cycle):
-    #     timefmt = "%a %b %d %H:%M:%S %Y %Z"
-    #     text = "Software versions\n"
-    #     text += "-----------------\n"
-    #     text += "Python %s\n" % sys.version
-    #     # for name, version in self.packages:
-    #     #     text += "%s %s\n" % (name, version)
-    #     text += "IPython %s\n" % IPython.__version__
-    #     text += "Timestamp %s\n" % time.strftime(timefmt)
-    #     pp.text(text)S
-
     def _repr_json_(self):
         return self.data
         # return json.dumps(self.data, indent=2)
 
 
 def just_text(output) -> str:
     """returns the text output of the command"""
@@ -113,14 +104,15 @@
     @cell_magic("micropython")
     @cell_magic("mpy")
     @magic_arguments("%micropython")  # add additional % to display two %% in help
     @argument_group("Code execution")
     @argument("--writefile", "--save", "-wf", type=str, help="MCU [path/]filename to write to", metavar="PATH/FILE.PY")
     @argument("--readfile", "--load", "-rf", type=str, help="MCU [path/]filename to read from", metavar="PATH/FILE.PY")
     @argument("--new", action="store_true", help="new cell is added after the current cell instead of replacing it")
+    @argument("--timeout", default=TIMEOUT, help="maximum timeout for the cell to run")
     # #
     @argument_group("Devices")
     @argument("--select", nargs="+", help="serial port to connect to", metavar="PORT")
     @argument("--reset", "--soft-reset", action="store_true", help="Reset device (before running cell).")
     @argument("--hard-reset", action="store_true", help="reset device.")
     def micropython(self, line: str, cell: str = ""):
         """
@@ -163,36 +155,35 @@
                 self.shell.set_next_input(code, replace=False)
             else:
                 self.shell.set_next_input(code, replace=True)
             return
 
         if not cell:
             raise UsageError("Please specify some MicroPython code to execute")
-        output = self.MCU.run_cell(cell)
+        output = self.MCU.run_cell(cell, timeout=float(args.timeout))
         # return PrettyOutput(output)
 
     # -------------------------------------------------------------------------
     # line magics
     # -------------------------------------------------------------------------
 
     @line_magic("micropython")
     @line_magic("mpy")
     @magic_arguments("mpy")
     @argument_group("Code execution")
     @argument("statement", nargs="*", help="Micropython code to run.", metavar="STATEMENT(S)")
     @argument("--eval", "-e", nargs="*", help="Expression to evaluate", metavar="EXPRESSION")
-    # @argument("--run", nargs=1, help="file to run on the MCU", metavar="PATH/FILE.PY")
-    # --follow / --no-follow switch
-    # @argument("--follow",  action=argparse.BooleanOptionalAction, help="follow the output of the MCU")
-    #
+    @argument("--timeout", default=TIMEOUT, help="maximum timeout for the cell to run")
+    @argument("--stream", action="store_true", help="stream each line of output as it is received")
     @argument_group("Devices")
     @argument("--list", "--devs", "-l", action="store_true", help="List available devices.")
     @argument("--select", "-s", nargs="+", help="serial port to connect to", metavar="PORT")
     @argument("--reset", "--soft-reset", action="store_true", help="reset device.")
     @argument("--hard-reset", action="store_true", help="reset device.")
+    @argument("--info", action="store_true", help="get boardinfo from device")
     @output_can_be_silenced
     def mpy_line(self, line: str):
         """
         Run Micropython code on an attached device using mpremote.
 
         - can be silenced with a trailing semicolon when used as a line magic
         """
@@ -220,46 +211,59 @@
             self.hard_reset()
         elif args.reset:
             self.soft_reset()
 
         # processing
         if args.list:
             return self.list_devices()
+        elif args.info:
+            #  load datafile  from installed package
+            script_path = pkg_resources.resource_filename("micropython_magic", "scripts/fw_info.py")
+            cmd = ["run", script_path]
+            if out := self.MCU.run_cmd(" ".join(cmd), stream_out=False, timeout=TIMEOUT):
+                if not out[0].startswith("{"):
+                    return out
+                r = eval(out[0])
+                r["serial_port"] = self.MCU.port
+                return r
         elif args.eval:
             return self.eval(args.eval)
 
         elif args.statement:
             # Assemble the command to run
             statement = "\n".join(args.statement)
             cmd = f'exec "{statement}"'
             log.debug(f"{cmd=}")
 
-            output = self.MCU.run_cmd(cmd, stream_out=False)
-            return output
+            return self.MCU.run_cmd(
+                cmd,
+                stream_out=bool(args.stream),
+                timeout=float(args.timeout),
+            )
 
     # -------------------------------------------------------------------------
     # worker mothods - these are called by the magics
     # -------------------------------------------------------------------------
 
     def list_devices(self) -> list:
         """
         Return a SList or list of the Micropython devices connected to the computer through serial ports or USB.
         """
         cmd = "mpremote connect list"
         # output = self.shell.getoutput(cmd)
         output = self.MCU.run_cmd(cmd, auto_connect=False, stream_out=False)
         return output
 
-    def select(self, line: Optional[str]):
+    def select(self, port: Optional[str]):
         """
         Select the device to connect to by specifying the serial port name.
         """
-        device = line.strip() if line else "auto"
+        device = port.strip() if port else "auto"
         output = self.MCU.select_device(device)
-        return just_text(output)
+        return output
 
     def eval(self, line: str):
         """
         Run a Micropython expression on an attached device using mpremote.
         Note that the expression
          * can only be a single expression
          * it cannot contain  comments or newlines.
@@ -296,8 +300,8 @@
 
     def hard_reset(self):
         """
         Perform a hard-reset on the current Micropython device.
         """
         output = self.MCU.run_cmd("reset")
         self.output = output
-        return just_text(output)
+        return output
```

### Comparing `micropython_magic-0.3.1/src/micropython_magic/test_magics.py` & `micropython_magic-0.4.0/src/micropython_magic/test_magics.py`

 * *Files identical despite different names*

### Comparing `micropython_magic-0.3.1/setup.py` & `micropython_magic-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['micropython_magic']
+['micropython_magic', 'micropython_magic.scripts']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['mpremote==1.20.0']
 
 setup_kwargs = {
     'name': 'micropython-magic',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': 'MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs',
     'long_description': '# micropython-magic\n\nThese magic methods allow MicroPython to be used from within any Jupyter Notebook or JupyterLab (formerly IPython Notebook)\nThe magics make use of the [mpremote tool](https://github.com/micropython/micropython/blob/master/tools/mpremote/README.md) to enable communication with the MCUs \n\n\nIt allows \n * Mixing of Host and MCU Code ( and languages if you wish)\n * Creating graphs of the data captured by MCU sensors \n * create re-uasable sequences ( download/compile firmware - flash firmware - uploade code - run expiriment - same outcome) \n * create and execute tests that require orchestration across multiple MCUs and hosts \n * Rapid Prototyping \n * Capturing the results and outputs in a consistent way\n * Mixing documentation with code  \n\n\n## Samples \n\n<table>\n\n<tr>\n<td>\nPlot cpu temperature  \n\n<img src="docs/cpu_plot.gif" width="300" />\n</td>\n<td>\nVisualize the memory map of the MCU\n\n<img src="docs/memory_map.gif" width="300" />\n</td>\n</tr>\n\n<tr>\n<td>\n</td>\n<td>\nMemory allocation of the MCU over time\n\n<img src="docs/memory_map_sequence.gif" width="300" />\n</td>\n</tr>\n</table>\n\nFor the source please refer to the samples folder\n## Installation\n- create and activate a venv `python3 -m venv .venv`\n - [ ] `pip install -U "micropython-magic"`\n\n- or install directly into your notbook environment/kernel using the \'%pip\' magic by running\n  - [ ] `%pip install -U "micropython-magic"`\n\nRecommended : install stubs for your MCU of choice\n- [ ] Install stubs for MicroPython syntax checking `pip install micropython-rp2-stubs` (or your port of choise)\n\n## Usage\n\n**1) Create a notebook**\n- install your desired notebook environment:\n  - [VScode and the **Juypyter extension**](https://code.visualstudio.com/docs/languages/python#_jupyter-notebooks) ,\n  - [Jupyter Notebook](https://jupyter.org/install#jupyter-notebook) \n  - [JupyterLab ](https://jupyter.org/install)\n\n- create a new notebook \n\n**2) Load the magic**\n```python\n%load_ext micropython_magic\n```\nThis can also be configured once to always load automatically ( see below)\n\n\n**3) add a cell with some code to run on the MCU**\n```python\n# %%micropython  \nfrom machine import Pin\nled = Pin(25, Pin.OUT)\nled.value(1)\n```\nThe `%%micropython` cell magic will instruct Jupyter to run the code on the connected MCU\n\n**4) enable code highlighting for MicroPython**\n```python\n%pip install micropython-esp32-stubs==1.20.0.*\n# installs the stubs for MicroPython syntax checking (one time install per environment) \n```\n\n```python\n# %%micropython  \nfrom machine import Pin\nled = Pin(25, Pin.OUT)\nled.value(1)\n```\nThis allows for syntax highlighting and code completion of MicroPython code.\nTested in VSCode with\n- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) extension\n- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension\n\n\n## Advanced \nList the connected devices \n```python\n%mpy --list\n```\n\n## Automatically load the magic on startup\n\nIn order to automatically load the magic on startup, you can add the following to your `ipython_config.py` file:\n\n- create a ipython profile \n  - `ipython profile create`\n  - add the following to the configuration file (`.../.ipython/profile_default/ipython_config.py`)\n\n    ```python\n    c = get_config()  #noqa\n\n    c.InteractiveShellApp.extensions = [\n        \'micropython_magic\'\n    ]\n    ```\n\n# initial \n\n - [x] run a code cell on a MCU \n - [ ] mpremote primitives\n   - [x] list connected boards and loop through them \n   - [x] switch the active MCU\n   - [x] avoid resetting MCU between cells ( use `resume`)\n   - [x] soft-reset a MCU\n   - [/] hard-reset a MCU\n       - only works on non-rp2040 devices \n       - report / fix hardware reset  issue on rp2040 `machine.reset()` ?\n   - all mpremote commands are possible using `!mpremote`\n   - [ ] mip install \n   - [ ] direct - copy file / files to / from \n   - [ ] mount folder \n   - [ ] ls and other file operations \n   - [ ] recursive delete wipe files from MCU - as a built-in magic ? / wait for / create PR for mpremote update ?\n   - [ ] cellmagic to copy cell content to specific files on the MCS \n       - [ ] %%micropython --writefile main.py\n       - [ ] %%micropython --readfile boot.py\n- [ ] Notebook essentials\n   - [x] load magics from `%pip install micropython-magic`\n   - [x] get the output from the MCU into a python variable `local = %eval remote`\n         - eval is not quite the same as mpremote\n         - retain type through json ?\n         - [?] can this be done with repr(insted) of json ?\n   - [x] plot data from a MCU\n            - [x] using bqplot ( > pyplot > vscode-Jupyter) \n            - [/] add documentation / sample\n-   \n   - [ ] copy/echo MCU global vars to local vars ( sync_from / sync_to)?\n   - [ ] get a data series onto the notebook and plot the outcome \n       - [x] loop one by one and update plot\n       - [ ] get larger series \n   - [ ] loop and update plot \n         https://ipywidgets.readthedocs.io/en/7.x/examples/Widget%20Asynchronous.html#Updating-a-widget-in-the-background\n   - [ ] long running via mqtt / async / folder mount ?\n - [ ] is there a way to avoid needing to set %%micropython on all cells ?\n       this could be done via an input_transformer - but keeping the state between cells may be quuite hard / confusing\n - [ ] %timeit / %%timeit for micropython code to avoid measuring the mpremote startup overhead \n\nSamples\n   - [x] Install\n   - [x] basic board control\n   - [x] blink\n   - [x] list connected boards and loop through them \n   - [~] read sensor and build series ( file / list / plot)\n   - [ ] flash a mcu with new firmware ( sample per port )\n   - [ ] mip install \n   - [ ] upload a repo / folder to a MCU\n\n## development\n## Testing \n\n- using Pytest\n- using testbook for testing notebooks\n  - located in the `./tests/` folder\n  - tests are paired with notebooks that contain the cells and magic commands to be tested\n  - tests have not been mocked - and therefore require a connected MCU to run ( rp2040 )\n\n- TODO: add tests for (remote) kernels \n  - [x] Local (on windows)\n  - [ ] on windows \n  - [ ] on linux\n  - [ ] jupyter notebook\n  - [ ] jupyter labs \n\n',
     'author': 'Jos Verlinde',
     'author_email': 'jos_verlinde@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `micropython_magic-0.3.1/PKG-INFO` & `micropython_magic-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-magic
-Version: 0.3.1
+Version: 0.4.0
 Summary: MicroPython Magic commands for use with Jupyter notebooks and Jupyter Labs
 License: MIT
 Keywords: MicroPython,stubs,Jupyter,notebooks,Jupyter Labs,vscode
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

