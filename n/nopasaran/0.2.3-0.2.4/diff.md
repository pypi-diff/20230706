# Comparing `tmp/nopasaran-0.2.3.tar.gz` & `tmp/nopasaran-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.2.3.tar", last modified: Wed Jul  5 13:02:55 2023, max compression
+gzip compressed data, was "nopasaran-0.2.4.tar", last modified: Thu Jul  6 03:58:49 2023, max compression
```

## Comparing `nopasaran-0.2.3.tar` & `nopasaran-0.2.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.693757 nopasaran-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 13:02:47.000000 nopasaran-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-05 13:02:55.689757 nopasaran-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-05 13:02:47.000000 nopasaran-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/controllers/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/controllers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/controllers/protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/definitions/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/definitions/control_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/definitions/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/definitions/transitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/interpreters/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/interpreters/action_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/interpreters/condition_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2131 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/interpreters/interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/ipsec_tunnels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/machines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/machines/action_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/machines/state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/parsers/interpreter_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/parsers/state_machine_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/primitives/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14684 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/primitives/action_primitives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1025 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/primitives/condition_primitives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      406 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/primitives/transition_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran/sniffers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/sniffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-05 13:02:47.000000 nopasaran-0.2.3/nopasaran/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/nopasaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 13:02:55.000000 nopasaran-0.2.3/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 13:02:55.693757 nopasaran-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 13:02:54.000000 nopasaran-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:55.689757 nopasaran-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:02:47.000000 nopasaran-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 03:58:41.000000 nopasaran-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-06 03:58:49.582018 nopasaran-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-06 03:58:41.000000 nopasaran-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/controllers/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/controllers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/controllers/protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/definitions/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/definitions/control_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/definitions/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/definitions/transitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/interpreters/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/interpreters/action_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/interpreters/condition_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2131 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/interpreters/interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/nopasaran/machines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/machines/action_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/machines/state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/nopasaran/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/parsers/interpreter_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/parsers/state_machine_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/nopasaran/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14684 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/primitives/action_primitives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1025 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/primitives/condition_primitives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      406 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/primitives/transition_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/nopasaran/sniffers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-06 03:58:41.000000 nopasaran-0.2.4/nopasaran/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.578018 nopasaran-0.2.4/nopasaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 03:58:49.000000 nopasaran-0.2.4/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 03:58:49.582018 nopasaran-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-06 03:58:49.000000 nopasaran-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:49.582018 nopasaran-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:58:41.000000 nopasaran-0.2.4/tests/__init__.py
```

### Comparing `nopasaran-0.2.3/LICENSE` & `nopasaran-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/PKG-INFO` & `nopasaran-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.3
+Version: 0.2.4
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.3/README.md` & `nopasaran-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/__main__.py` & `nopasaran-0.2.4/nopasaran/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,8 +82,9 @@
             deferToThread(machine.start).addBoth(lambda _: reactor.stop())
             reactor.run()
         except Exception as e:
             logging.error(f'[Main] Error starting the machine: {str(e)}')
 
     logging.info('[Main] Application finished')
 
-main()
+if __name__ == "__main__":
+    main()
```

### Comparing `nopasaran-0.2.3/nopasaran/controllers/controller.py` & `nopasaran-0.2.4/nopasaran/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/controllers/factory.py` & `nopasaran-0.2.4/nopasaran/controllers/factory.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/controllers/protocol.py` & `nopasaran-0.2.4/nopasaran/controllers/protocol.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/decorators.py` & `nopasaran-0.2.4/nopasaran/decorators.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/definitions/control_channel.py` & `nopasaran-0.2.4/nopasaran/definitions/control_channel.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/interpreters/action_interpreter.py` & `nopasaran-0.2.4/nopasaran/interpreters/action_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/interpreters/condition_interpreter.py` & `nopasaran-0.2.4/nopasaran/interpreters/condition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/interpreters/interpreter.py` & `nopasaran-0.2.4/nopasaran/interpreters/interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/interpreters/transition_interpreter.py` & `nopasaran-0.2.4/nopasaran/interpreters/transition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.2.4/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/machines/action_queue.py` & `nopasaran-0.2.4/nopasaran/machines/action_queue.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/machines/state_machine.py` & `nopasaran-0.2.4/nopasaran/machines/state_machine.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/parsers/interpreter_parser.py` & `nopasaran-0.2.4/nopasaran/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/parsers/state_machine_parser.py` & `nopasaran-0.2.4/nopasaran/parsers/state_machine_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/primitives/action_primitives.py` & `nopasaran-0.2.4/nopasaran/primitives/action_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/primitives/condition_primitives.py` & `nopasaran-0.2.4/nopasaran/primitives/condition_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/sniffers/sniffer.py` & `nopasaran-0.2.4/nopasaran/sniffers/sniffer.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran/utils.py` & `nopasaran-0.2.4/nopasaran/utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.2.4/nopasaran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.3
+Version: 0.2.4
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.3/nopasaran.egg-info/SOURCES.txt` & `nopasaran-0.2.4/nopasaran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.3/setup.py` & `nopasaran-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 # Version will automatically be updated when pushed on the main branch
 setup(
     name="nopasaran",
-    version='0.2.3',
+    version='0.2.4',
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
```

