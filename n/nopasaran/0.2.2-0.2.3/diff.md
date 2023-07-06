# Comparing `tmp/nopasaran-0.2.2.tar.gz` & `tmp/nopasaran-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.2.2.tar", last modified: Sat Jul  1 13:05:38 2023, max compression
+gzip compressed data, was "nopasaran-0.2.3.tar", last modified: Wed Jul  5 13:02:55 2023, max compression
```

## Comparing `nopasaran-0.2.2.tar` & `nopasaran-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.731066 nopasaran-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 13:05:29.000000 nopasaran-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-01 13:05:38.727066 nopasaran-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-01 13:05:29.000000 nopasaran-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.723066 nopasaran-0.2.2/nopasaran/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/controllers/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/controllers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/controllers/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/controllers/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/interpreters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/interpreters/action_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/interpreters/condition_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/ipsec_tunnels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/machines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/machines/machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/parsers/interpreter_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/sniffers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/sniffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 13:05:38.731066 nopasaran-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-01 13:05:37.000000 nopasaran-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.693757 nopasaran-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 13:02:47.000000 nopasaran-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-05 13:02:55.689757 nopasaran-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-05 13:02:47.000000 nopasaran-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/controllers/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/controllers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/controllers/protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/definitions/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/definitions/control_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/definitions/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/definitions/transitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/interpreters/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/interpreters/action_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/interpreters/condition_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2131 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/interpreters/interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/machines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/machines/action_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/machines/state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/parsers/interpreter_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/parsers/state_machine_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14684 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/primitives/action_primitives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1025 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/primitives/condition_primitives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      406 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/primitives/transition_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/sniffers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 13:02:55.693757 nopasaran-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 13:02:54.000000 nopasaran-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/tests/__init__.py
```

### Comparing `nopasaran-0.2.2/LICENSE` & `nopasaran-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.2/PKG-INFO` & `nopasaran-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.2
+Version: 0.2.3
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
         
@@ -123,15 +123,15 @@
         
         ### Additional Options
         
         You can further customize the behavior of NoPASARAN with the following options:
         
         - `--verbose` or `-v`: Enable verbose output.
         - `--log=<path-to-log-file>` or `-l=<path-to-log-file>`: Specify the path to the log file (default is "conf.log").
-        - `--log-level=<log-level>` or `-ll=<log-level>`: Specify the log level for output. Valid choices are "info", "warning", and "error".
+        - `--log-level=<log-level>` or `-ll=<log-level>`: Specify the log level for output. Valid choices are "debug", "info", "warning", and "error".
         
         Replace `<path-to-json-scenario-file>` with the path to your actual JSON scenario file.
         
         For any further assistance, use the `--help` argument with any command for additional information.
         
         ## Docker
```

### Comparing `nopasaran-0.2.2/README.md` & `nopasaran-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
 ### Additional Options
 
 You can further customize the behavior of NoPASARAN with the following options:
 
 - `--verbose` or `-v`: Enable verbose output.
 - `--log=<path-to-log-file>` or `-l=<path-to-log-file>`: Specify the path to the log file (default is "conf.log").
-- `--log-level=<log-level>` or `-ll=<log-level>`: Specify the log level for output. Valid choices are "info", "warning", and "error".
+- `--log-level=<log-level>` or `-ll=<log-level>`: Specify the log level for output. Valid choices are "debug", "info", "warning", and "error".
 
 Replace `<path-to-json-scenario-file>` with the path to your actual JSON scenario file.
 
 For any further assistance, use the `--help` argument with any command for additional information.
 
 ## Docker
```

### Comparing `nopasaran-0.2.2/nopasaran/__main__.py` & `nopasaran-0.2.3/nopasaran/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import json
 import logging
 import sys
 from twisted.internet.threads import deferToThread
 from twisted.internet import reactor
-from nopasaran.machines.machine import Machine
+from nopasaran.machines.state_machine import StateMachine
 
 def main():
     # Set up argument parser
     parser = argparse.ArgumentParser(
         prog='ROLE',
         description='NoPASARAN: Internet Route Testing Framework for Network Middleboxes',
         epilog="See '<command> --help' for more information on a command."
@@ -16,15 +16,15 @@
 
     # Set up base parser
     base_parser = argparse.ArgumentParser(add_help=False)
     base_parser.add_argument("-v", "--verbose", action="store_true", help="Enable verbose output")
 
     # Add -l and -ll options as shorter names for --log and --log-level
     base_parser.add_argument("-l", "--log", dest="log_file", default="conf.log", help="Path to the log file (default: %(default)s)")
-    base_parser.add_argument("-ll", "--log-level", choices=["info", "warning", "error"], help="Log level for output")
+    base_parser.add_argument("-ll", "--log-level", choices=["debug", "info", "warning", "error"], help="Log level for output")
 
     # Create subparsers for the role
     subparsers = parser.add_subparsers(dest='role', help='Define the role for the machine in the architecture')
 
     # Parser for WORKER role
     worker_parser = subparsers.add_parser("WORKER", help="The Worker performs a test campaign to evaluate network middleboxes. It can be either the client machine that tests its connection path to another endpoint or a trusted machine registered in the network.", parents=[base_parser])
     worker_parser.add_argument("-s", "--scenario", required=True, help="JSON scenario file for the state machine indicating the test campaign the Worker has to run")
@@ -62,28 +62,28 @@
 
     # If role is WORKER, load JSON file and start the machine
     if args.role == 'WORKER':
         if not args.scenario:
             parser.error("The 'WORKER' role requires the '--scenario' argument.")
             return
 
-        logging.info('Loading JSON scenario file...')
+        logging.info('[Main] Loading JSON scenario file...')
         try:
             with open(args.scenario) as f:
-                xstate_json = json.load(f)
+                state_json = json.load(f)
         except Exception as e:
-            logging.error(f'Error loading JSON scenario file: {str(e)}')
+            logging.error(f'[Main] Error loading JSON scenario file: {str(e)}')
             return
 
-        logging.info('JSON scenario file loaded')
-        machine = Machine(xstate_json=xstate_json)
+        logging.info('[Main] JSON scenario file loaded')
+        machine = StateMachine(state_json=state_json)
 
-        logging.info('Starting the machine')
+        logging.info('[Main] Starting the root machine')
         try:
-            deferToThread(machine.start).addCallback(lambda _: reactor.stop())
+            deferToThread(machine.start).addBoth(lambda _: reactor.stop())
             reactor.run()
         except Exception as e:
-            logging.error(f'Error starting the machine: {str(e)}')
+            logging.error(f'[Main] Error starting the machine: {str(e)}')
 
-    logging.info('Application finished')
+    logging.info('[Main] Application finished')
 
 main()
```

### Comparing `nopasaran-0.2.2/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.2.3/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.2/nopasaran/sniffers/sniffer.py` & `nopasaran-0.2.3/nopasaran/sniffers/sniffer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,91 @@
+import logging
 from nopasaran.utils import *
 from scapy.all import AsyncSniffer, Ether, sniff
 
+
 class Sniffer(AsyncSniffer):
     """
     Custom Sniffer class inheriting from the AsyncSniffer of Scapy.
     """
+
     def __init__(self, machine, filter=''):
         """
-        Initializer for the Sniffer class.
+        Initialize the Sniffer.
+        
         Args:
             machine (str): A string defining the machine to sniff.
             filter (str): A string defining the filter for packets.
         """
         super().__init__(prn=self.__handle_sniffer(), lfilter=lambda pkt: self.__filter_packet(pkt))
-        self.machine = machine 
+        self.machine = machine
         self.__filter = filter
         self.queue = None
-        
+        logging.debug('[Sniffer] Machine ID: {}: Sniffer initialized'.format(machine.machine_id))
+
     def __handle_sniffer(self):
         """
-        Internal method to handle the sniffer. A callback for packets sniffed.
+        Handle the sniffer callback.
+        
         Returns:
-            pkt_callback (func): Function to execute when a packet is sniffed.
+            function: The callback function to execute when a packet is sniffed.
         """
         def pkt_callback(packet):
-            if self.queue != None:
+            """
+            Callback function for sniffed packets.
+            
+            Args:
+                packet: The sniffed packet.
+            """
+            if self.queue is not None:
                 self.queue.append(packet)
         return pkt_callback
-    
+
     def __filter_packet(self, packet):
         """
-        Internal method to filter the packets.
+        Filter the packets.
+        
         Args:
-            packet (Packet): Packet to filter.
+            packet: The packet to filter.
+        
         Returns:
             bool: True if the packet is accepted, False otherwise.
         """
         if 'Ether' in packet:
-            if (packet[Ether].src != Ether().src):
+            if packet[Ether].src != Ether().src:
                 filtered_packets = sniff(offline=packet, filter=self.__filter)
                 if packet in filtered_packets:
+                    logging.debug("[Sniffer] Packet passed the filter: %s", packet)
                     return True
         return False
-    
+
     def set_filter(self, filter):
         """
-        Method to set a new filter.
+        Set a new filter.
+        
         Args:
-            filter (str): String defining the new filter.
+            filter (str): The new filter string.
         """
         self.__filter = filter
-    
+        logging.debug("[Sniffer] Filter set to: %s", filter)
+
     def get_packet_layers(self, packet):
         """
-        Method to get all the layers in a packet.
+        Get all the layers in a packet.
+        
         Args:
-            packet (Packet): Packet to analyze.
+            packet: The packet to analyze.
+        
         Returns:
             list: List of layers in the packet.
         """
         layers = []
         counter = 0
         while True:
             layer = packet.getlayer(counter)
             if layer is None:
                 break
             else:
                 layers.append(layer)
             counter += 1
+        logging.debug("[Sniffer] Packet layers: %s", layers)
         return layers
```

### Comparing `nopasaran-0.2.2/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.2.3/nopasaran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.2
+Version: 0.2.3
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
         
@@ -123,15 +123,15 @@
         
         ### Additional Options
         
         You can further customize the behavior of NoPASARAN with the following options:
         
         - `--verbose` or `-v`: Enable verbose output.
         - `--log=<path-to-log-file>` or `-l=<path-to-log-file>`: Specify the path to the log file (default is "conf.log").
-        - `--log-level=<log-level>` or `-ll=<log-level>`: Specify the log level for output. Valid choices are "info", "warning", and "error".
+        - `--log-level=<log-level>` or `-ll=<log-level>`: Specify the log level for output. Valid choices are "debug", "info", "warning", and "error".
         
         Replace `<path-to-json-scenario-file>` with the path to your actual JSON scenario file.
         
         For any further assistance, use the `--help` argument with any command for additional information.
         
         ## Docker
```

### Comparing `nopasaran-0.2.2/nopasaran.egg-info/SOURCES.txt` & `nopasaran-0.2.3/nopasaran.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 LICENSE
 README.md
 setup.py
 nopasaran/__init__.py
 nopasaran/__main__.py
+nopasaran/decorators.py
 nopasaran/utils.py
 nopasaran.egg-info/PKG-INFO
 nopasaran.egg-info/SOURCES.txt
 nopasaran.egg-info/dependency_links.txt
 nopasaran.egg-info/entry_points.txt
 nopasaran.egg-info/requires.txt
 nopasaran.egg-info/top_level.txt
 nopasaran/controllers/__init__.py
 nopasaran/controllers/controller.py
 nopasaran/controllers/factory.py
-nopasaran/controllers/messages.py
 nopasaran/controllers/protocol.py
+nopasaran/definitions/__init__.py
+nopasaran/definitions/commands.py
+nopasaran/definitions/control_channel.py
+nopasaran/definitions/events.py
+nopasaran/definitions/transitions.py
 nopasaran/interpreters/__init__.py
 nopasaran/interpreters/action_interpreter.py
 nopasaran/interpreters/condition_interpreter.py
+nopasaran/interpreters/interpreter.py
 nopasaran/interpreters/transition_interpreter.py
 nopasaran/ipsec_tunnels/__init__.py
 nopasaran/ipsec_tunnels/ipsec_conf.py
 nopasaran/machines/__init__.py
-nopasaran/machines/machine.py
+nopasaran/machines/action_queue.py
+nopasaran/machines/state_machine.py
 nopasaran/parsers/__init__.py
 nopasaran/parsers/interpreter_parser.py
+nopasaran/parsers/state_machine_parser.py
+nopasaran/primitives/__init__.py
+nopasaran/primitives/action_primitives.py
+nopasaran/primitives/condition_primitives.py
+nopasaran/primitives/transition_primitives.py
 nopasaran/sniffers/__init__.py
 nopasaran/sniffers/sniffer.py
 tests/__init__.py
```

### Comparing `nopasaran-0.2.2/setup.py` & `nopasaran-0.2.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 # Version will automatically be updated when pushed on the main branch
 setup(
     name="nopasaran",
-    version='0.2.2',
+    version='0.2.3',
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
```

