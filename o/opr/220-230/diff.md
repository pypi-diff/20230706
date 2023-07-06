# Comparing `tmp/opr-220.tar.gz` & `tmp/opr-230.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opr-220.tar", last modified: Tue Jul  4 14:57:11 2023, max compression
+gzip compressed data, was "opr-230.tar", last modified: Thu Jul  6 00:56:23 2023, max compression
```

## Comparing `opr-220.tar` & `opr-230.tar`

### file list

```diff
@@ -1,46 +1,36 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 14:57:11.079510 opr-220/
--rw-r--r--   0 bart      (1000) bart      (1000)     2487 2023-07-04 14:57:11.079510 opr-220/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1923 2023-07-04 14:13:27.000000 opr-220/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 14:57:11.079510 opr-220/opr/
--rw-r--r--   0 bart      (1000) bart      (1000)     1914 2023-07-04 11:49:32.000000 opr-220/opr/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      134 2023-07-03 12:59:17.000000 opr-220/opr/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     8946 2023-07-03 12:53:54.000000 opr-220/opr/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)      535 2023-07-03 12:35:01.000000 opr-220/opr/loggers.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 14:57:11.079510 opr-220/opr/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      361 2023-07-04 13:24:11.000000 opr-220/opr/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      937 2023-07-03 11:41:20.000000 opr-220/opr/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    20759 2023-07-03 12:52:48.000000 opr-220/opr/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      826 2023-07-03 00:19:09.000000 opr-220/opr/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4225 2023-07-03 11:59:03.000000 opr-220/opr/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17810 2023-07-03 12:57:45.000000 opr-220/opr/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2354 2023-07-01 05:55:02.000000 opr-220/opr/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)     8130 2023-07-03 11:42:24.000000 opr-220/opr/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1039 2023-07-03 00:19:36.000000 opr-220/opr/modules/shp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1065 2023-07-03 00:20:30.000000 opr-220/opr/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2934 2023-07-03 11:58:30.000000 opr-220/opr/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5691 2023-07-01 05:55:02.000000 opr-220/opr/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7012 2023-07-04 11:52:44.000000 opr-220/opr/objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5121 2023-07-03 14:25:17.000000 opr-220/opr/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1429 2023-07-03 12:41:32.000000 opr-220/opr/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7803 2023-07-04 14:10:29.000000 opr-220/opr/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2372 2023-07-03 12:33:25.000000 opr-220/opr/threads.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1978 2023-07-03 12:42:29.000000 opr-220/opr/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 14:57:11.079510 opr-220/opr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2487 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      756 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       41 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-04 14:57:11.000000 opr-220/opr.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      900 2023-07-04 14:56:37.000000 opr-220/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-04 14:57:11.079510 opr-220/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-07-01 10:59:30.000000 opr-220/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 14:57:11.079510 opr-220/test/
--rw-r--r--   0 bart      (1000) bart      (1000)      675 2023-07-01 05:55:02.000000 opr-220/test/test_composite.py
--rw-r--r--   0 bart      (1000) bart      (1000)      442 2023-07-03 12:00:09.000000 opr-220/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      370 2023-07-03 12:00:20.000000 opr-220/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      935 2023-07-01 05:55:02.000000 opr-220/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4382 2023-07-04 02:35:41.000000 opr-220/test/test_objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)      642 2023-07-03 13:43:53.000000 opr-220/test/test_recursive.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1232 2023-07-03 01:04:57.000000 opr-220/test/test_storage.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-06 00:56:23.530040 opr-230/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2487 2023-07-06 00:56:23.530040 opr-230/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1923 2023-07-04 14:13:27.000000 opr-230/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-06 00:56:23.526040 opr-230/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     6288 2023-07-05 21:49:59.000000 opr-230/bin/opr
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-06 00:56:23.526040 opr-230/opr/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1914 2023-07-04 11:49:32.000000 opr-230/opr/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    10722 2023-07-06 00:51:15.000000 opr-230/opr/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      535 2023-07-03 12:35:01.000000 opr-230/opr/loggers.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-06 00:56:23.530040 opr-230/opr/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      361 2023-07-04 13:24:11.000000 opr-230/opr/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      937 2023-07-03 11:41:20.000000 opr-230/opr/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    20964 2023-07-05 19:45:40.000000 opr-230/opr/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      826 2023-07-03 00:19:09.000000 opr-230/opr/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4225 2023-07-03 11:59:03.000000 opr-230/opr/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17831 2023-07-05 10:51:26.000000 opr-230/opr/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2354 2023-07-01 05:55:02.000000 opr-230/opr/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     8151 2023-07-05 10:51:10.000000 opr-230/opr/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1039 2023-07-03 00:19:36.000000 opr-230/opr/modules/shp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1065 2023-07-03 00:20:30.000000 opr-230/opr/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2934 2023-07-03 11:58:30.000000 opr-230/opr/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5691 2023-07-01 05:55:02.000000 opr-230/opr/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7012 2023-07-04 11:52:44.000000 opr-230/opr/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5121 2023-07-03 14:25:17.000000 opr-230/opr/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1429 2023-07-03 12:41:32.000000 opr-230/opr/repeats.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2372 2023-07-03 12:33:25.000000 opr-230/opr/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1978 2023-07-03 12:42:29.000000 opr-230/opr/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-06 00:56:23.530040 opr-230/opr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2487 2023-07-06 00:56:23.000000 opr-230/opr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      530 2023-07-06 00:56:23.000000 opr-230/opr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-06 00:56:23.000000 opr-230/opr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-06 00:56:23.000000 opr-230/opr.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-07-06 00:56:23.000000 opr-230/opr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)     1025 2023-07-06 00:55:50.000000 opr-230/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-06 00:56:23.530040 opr-230/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-07-01 10:59:30.000000 opr-230/setup.py
```

### Comparing `opr-220/PKG-INFO` & `opr-230/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opr
-Version: 220
+Version: 230
 Summary: Object Programming Runtime
 Author-email: Bart Thate <programmingobject@gmail.com>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/opr
 Project-URL: bugs, https://github.com/bthate/opr/issues
 Project-URL: source, https://github.com/bthate/opr
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `opr-220/README.rst` & `opr-230/README.rst`

 * *Files identical despite different names*

### Comparing `opr-220/opr/__init__.py` & `opr-230/opr/__init__.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/handler.py` & `opr-230/opr/handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 "handler"
 
 
 # IMPORTS
 
 
 import inspect
+import io
+import os
 import queue
 import ssl
 import sys
 import threading
+import traceback
 
 
 from opr.loggers import Logging
-from opr.objects import Default, Object, copy, keys
+from opr.objects import Default, Object, copy, keys, update
 from opr.threads import launch
 from opr.utility import spl
 
 
 # DEFINES
 
 
@@ -28,23 +31,28 @@
             'Bus',
             'Cfg',
             'Commands',
             'Errors',
             'Event',
             'Handler',
             "dispatch",
-            "parse"
+            "parse",
+            'parse_cli',
+            'waiter'
            )
 
 
 MODNAMES = {
            }
 
 
 Cfg = Default()
+Cfg.debug = False
+Cfg.mod = ""
+Cfg.verbose = False
 
 
 # CLASSES
 
 
 class Errors(Object):
 
@@ -293,26 +301,83 @@
         "stop loop'n"
         self.stopped.set()
         self.queue.put_nowait(None)
 
 
 # UTILITY
 
+def command(cli, txt) -> Event:
+    "run a command on a cli"
+    evt = cli.event(txt)
+    Commands.handle(evt)
+    evt.ready()
+    return evt
+
 
 def dispatch(func, evt) -> None:
     # pylint: disable=W0718
     "basic dispatcher"
     try:
         func(evt)
     except Exception as ex:
         exc = ex.with_traceback(ex.__traceback__)
         Errors.errors.append(exc)
         evt.ready()
 
 
+def parse_cli(txt) -> Cfg:
+    "parse commad line interface"
+    evt = Event()
+    evt.parse(txt)
+    update(Cfg, evt, False)
+    Cfg.mod += evt.mods
+    return Cfg
+
+
+def scanstr(pkg, mods, init=None, doall=False, wait=False) -> None:
+    "scan a package for list of modules"
+    res = []
+    path = pkg.__path__[0]
+    if doall:
+        modlist = [x[:-3] for x in os.listdir(path) if x.endswith(".py") and x != "__init__.py"]
+        mods = ",".join(sorted(modlist))
+    threads = []
+    for modname in spl(mods):
+        module = getattr(pkg, modname, None)
+        if module:
+            if not init:
+                Commands.scan(module)
+        if init and "start" in dir(module):
+            threads.append(launch(module.start))
+        res.append(module)
+    if wait:
+        for thread in threads:
+            thread.join()
+    return res
+
+
+def waiter(clear=True):
+    "poll for errors"
+    got = []
+    for ex in Errors.errors:
+        stream = io.StringIO(
+                             traceback.print_exception(
+                                                       type(ex),
+                                                       ex,
+                                                       ex.__traceback__
+                                                      )
+                            )
+        for line in stream.readlines():
+            Logging.debug(line)
+        got.append(ex)
+    if clear:
+        for exc in got:
+            Errors.errors.remove(exc)
+
+
 # METHODS
 
 
 def parsequal(obj, word):
     "check for qualness"
     try:
         key, value = word.split('==')
@@ -328,15 +393,15 @@
     except ValueError:
         return False
 
 
 def parseassign(obj, word):
     "check for assign"
     try:
-        key, value = word.split('=')
+        key, value = word.split('=', maxsplit=1)
         if key == "mod":
             if not obj.mod:
                 obj.mod = ""
             for val in spl(value):
                 if val not in obj.mods:
                     obj.mods += f",{val}"
             return True
```

### Comparing `opr-220/opr/loggers.py` & `opr-230/opr/loggers.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/modules/fnd.py` & `opr-230/opr/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/modules/irc.py` & `opr-230/opr/modules/irc.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from opr.objects import Default, Object, copy, edit, keys, prt, update
 from opr.persist import find, fntime, last, write
 from opr.threads import launch
 from opr.utility import elapsed
 
 
 NAME = "opr"
-
+VERSION = "221"
 
 saylock = _thread.allocate_lock()
 
 
 def start():
     "start a irc bot"
     irc = IRC()
@@ -66,14 +66,15 @@
     sasl = False
     server = 'localhost'
     servermodes = ''
     sleep = 60
     username = NAME
     users = False
     verbose = False
+    version = VERSION
 
     def __init__(self):
         Default.__init__(self)
         self.channel = Config.channel
         self.nick = Config.nick
         self.port = Config.port
         self.realname = Config.realname
@@ -240,19 +241,21 @@
         "connect to server"
         self.state.nrconnect += 1
         self.events.connected.clear()
         Logging.debug(f"connecting to {server}:{port}")
         if self.cfg.password:
             Logging.debug("using SASL")
             self.cfg.sasl = True
+            self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
             ctx.check_hostname = False
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
             self.sock.connect((server, port))
+            time.sleep(1.0)
             self.command('CAP LS 302')
         else:
             addr = socket.getaddrinfo(server, port, socket.AF_INET)[-1][-1]
             self.sock = socket.create_connection(addr)
             self.events.authed.set()
         if self.sock:
             os.set_inheritable(self.sock.fileno(), os.O_RDWR)
@@ -260,14 +263,15 @@
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
         "send direct text"
+        time.sleep(1.0)
         Logging.debug(txt)
         self.sock.send(bytes(txt.rstrip()+'\r\n', 'utf-8'))
 
     def disconnect(self):
         "disconnect from server"
         try:
             self.sock.shutdown(2)
@@ -334,14 +338,15 @@
         for channel in self.channels:
             self.command('JOIN', channel)
 
     def keep(self):
         "keep alive loop"
         while 1:
             self.events.connected.wait()
+            self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.command('PING', self.cfg.server)
             if self.state.pongcheck:
                 Logging.debug("failed pongcheck, restarting")
                 self.state.pongcheck = False
@@ -352,16 +357,16 @@
                 break
 
     def logon(self, server, nck):
         "logon to server"
         self.events.connected.wait()
         self.events.authed.wait()
         nck = self.cfg.username
-        self.direct(f'NICK {nck}')
-        self.direct(f'USER {nck} {server} {server} {nck}')
+        self.command(f'NICK {nck}')
+        self.command(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
         # pylint: disable=R0912,R0915
         "parse text"
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
@@ -436,14 +441,15 @@
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
                 Errors.errors.append(ex)
                 self.stop()
                 Logging.debug("handler stopped")
+                return self.event(str(ex))
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
@@ -556,23 +562,23 @@
     Logging.debug(evt.txt)
 
 
 def cb_h903(evt):
     "capabilities end"
     assert evt
     bot = evt.bot()
-    bot.command('CAP END')
+    bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_h904(evt):
     "capabilities end"
     assert evt
     bot = evt.bot()
-    bot.command('CAP END')
+    bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_kill(evt):
     "got killed"
```

### Comparing `opr-220/opr/modules/log.py` & `opr-230/opr/modules/log.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/modules/mbx.py` & `opr-230/opr/modules/mbx.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/modules/mdl.py` & `opr-230/opr/modules/mdl.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         'mdl',
         'now',
         'start'
     )
 
 
 def start():
+    time.sleep(60.0)
     for key in keys(oorzaken):
         val = getattr(oorzaken, key, None)
         if val and int(val) > 10000:
             evt = Event()
             evt.txt = ""
             evt.rest = key
             sec = seconds(val)
```

### Comparing `opr-220/opr/modules/req.py` & `opr-230/opr/modules/req.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/modules/rss.py` & `opr-230/opr/modules/rss.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from opr.repeats import Repeater
 from opr.threads import launch, threaded
 from opr.utility import elapsed, spl
 
 
 def start():
     "start a fetcher"
+    time.sleep(60.0)
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
 
 
 fetchlock = _thread.allocate_lock()
```

### Comparing `opr-220/opr/modules/shp.py` & `opr-230/opr/modules/shp.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/modules/tdo.py` & `opr-230/opr/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/modules/udp.py` & `opr-230/opr/modules/udp.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/modules/wsd.py` & `opr-230/opr/modules/wsd.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/objects.py` & `opr-230/opr/objects.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/persist.py` & `opr-230/opr/persist.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/repeats.py` & `opr-230/opr/repeats.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/runtime.py` & `opr-230/bin/opr`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+#!/usr/bin/env python3
 # This file is placed in the Public Domain.
+#
+# pylint: disable=E0001
 
 
-"runtime"
+"object programming runtime"
 
 
 # IMPORTS
 
 
 import io
 import os
@@ -13,43 +16,38 @@
 import sys
 import termios
 import threading
 import time
 import traceback
 
 
-from opr.handler import Bus, Commands, Errors, Event, Handler
+sys.path.insert(0, os.getcwd())
+
+
+from opr.handler import Bus, Cfg, Commands, Errors, Event, Handler
+from opr.handler import command, parse_cli, scanstr, waiter
 from opr.loggers import Logging
 from opr.objects import Default, Object, keys, kind, prt, update
 from opr.persist import Persist
-from opr.threads import launch
+from opr.threads import launch, name
 from opr.utility import elapsed, spl
 
 
 import opr.modules
 
 
 # DEFINES
 
 
 DATE = time.ctime(time.time()).replace("  ", " ")
-NAME = __file__.split(os.sep)[-2]
+NAME = sys.argv[0].split(os.sep)[-1]
 STARTTIME = time.time()
 
 
-Persist.workdir = os.path.expanduser("~/.{NAME}")
-
-
-Cfg = Default()
-Cfg.debug = False
-Cfg.mod = ""
-Cfg.verbose = False
-
-
-readline.redisplay()
+Persist.workdir = os.path.expanduser(f"~/.{NAME}")
 
 
 # CLASSES
 
 
 class CLI(Handler):
 
@@ -82,85 +80,28 @@
 
 def banner():
     "print banner"
     print(f"{NAME.upper()} started {DATE}")
     sys.stdout.flush()
 
 
-def command(cli, txt) -> Event:
-    "run a command on a cli"
-    evt = cli.event(txt)
-    Commands.handle(evt)
-    evt.ready()
-    return evt
-
-
 def daemon():
     "fork to the background"
     pid = os.fork()
+    print(f"forking {pid}")
     if pid:
-        os.setsid()
-        os.umask(0)
-        with open('/dev/null', 'r', encoding="utf-8") as sis:
-            os.dup2(sis.fileno(), sys.stdin.fileno())
-        with open('/dev/null', 'a+', encoding="utf-8") as sos:
-            os.dup2(sos.fileno(), sys.stdout.fileno())
-        with open('/dev/null', 'a+', encoding="utf-8") as ses:
-            os.dup2(ses.fileno(), sys.stderr.fileno())
-
-
-def parse_cli(txt) -> Cfg:
-    "parse commad line interface"
-    evt = Event()
-    evt.parse(txt)
-    update(Cfg, evt, False)
-    Cfg.mod += evt.mods
-    return Cfg
-
-
-def scanstr(pkg, mods, init=None, doall=False, wait=False) -> None:
-    "scan a package for list of modules"
-    res = []
-    path = pkg.__path__[0]
-    if doall:
-        modlist = [x[:-3] for x in os.listdir(path) if x.endswith(".py") and x != "__init__.py"]
-        mods = ",".join(sorted(modlist))
-    threads = []
-    for modname in spl(mods):
-        module = getattr(pkg, modname, None)
-        if module:
-            if not init:
-                Commands.scan(module)
-        if init and "start" in dir(module):
-            threads.append(launch(module.start))
-        res.append(module)
-    if wait:
-        for thread in threads:
-            thread.join()
-    return res
-
-
-def waiter(clear=True):
-    "poll for errors"
-    got = []
-    for ex in Errors.errors:
-        stream = io.StringIO(
-                             traceback.print_exception(
-                                                       type(ex),
-                                                       ex,
-                                                       ex.__traceback__
-                                                      )
-                            )
-        for line in stream.readlines():
-            Logging.debug(line)
-        got.append(ex)
-    if clear:
-        for exc in got:
-            Errors.errors.remove(exc)
-
+        os._exit(0)
+    #os.setsid()
+    os.umask(0)
+    with open('/dev/null', 'r', encoding="utf-8") as sis:
+        os.dup2(sis.fileno(), sys.stdin.fileno())
+    with open('/dev/null', 'a+', encoding="utf-8") as sos:
+        os.dup2(sos.fileno(), sys.stdout.fileno())
+    with open('/dev/null', 'a+', encoding="utf-8") as ses:
+        os.dup2(ses.fileno(), sys.stderr.fileno())
 
 
 def wrap(func):
     "wrap function"
     fds = sys.stdin.fileno()
     gotterm = True
     try:
@@ -207,15 +148,15 @@
     "show listeners"
     try:
         index = int(event.args[0])
         event.reply(prt(Bus.objs[index]))
         return
     except (KeyError, TypeError, IndexError, ValueError):
         pass
-    event.reply(' | '.join([kind(obj) for obj in Bus.objs]))
+    event.reply(' | '.join([name(obj) for obj in Bus.objs]))
 
 
 def mod(event):
     "show list of available modules"
     path = opr.modules.__path__[0]
     modlist = [x[:-3] for x in os.listdir(path) if x.endswith(".py") and x != "__init__.py"]
     mods = ",".join(sorted(modlist))
@@ -231,33 +172,33 @@
     for modname in spl(modnames):
         mods = getattr(opr.modules, modname)
         if not mods:
             event.reply(f"{modname} is not available")
             continue
         Commands.scan(mods)
         if "start" in dir(mods):
-            launch(mods.start)
+            thr = launch(mods.start)
         event.reply(f"reloaded {modname}")
 
 
 def sts(event):
     "print status"
     nmr = 0
     for bot in Bus.objs:
         if 'state' in dir(bot):
             event.reply(prt(bot.state, skip='lastline'))
             nmr += 1
-    if nmr:
+    if not nmr:
         event.reply("no status")
 
 
 def thr(event):
     "show list of running threads"
     result = []
-    for thread in sorted(threading.enumerate(), key=lambda x: x.getName()):
+    for thread in sorted(threading.enumerate(), key=lambda x: x.name):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
             uptime = obj.sleep - int(time.time() - obj.state.latest)
         elif getattr(obj, 'starttime', None):
@@ -324,15 +265,15 @@
     if "c" in Cfg.opts:
         dowait = True
     if dowait:
         banner()
         if 'c' in Cfg.opts and "d" not in Cfg.opts:
             csl = Console()
             csl.start()
-        scanstr(opr.modules, Cfg.mod, True, wait=True)
+        scanstr(opr.modules, Cfg.mod, True, wait=False)
         while 1:
             time.sleep(1.0)
             waiter()
 
 
 if __name__ == "__main__":
     wrap(main)
```

### Comparing `opr-220/opr/threads.py` & `opr-230/opr/threads.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr/utility.py` & `opr-230/opr/utility.py`

 * *Files identical despite different names*

### Comparing `opr-220/opr.egg-info/PKG-INFO` & `opr-230/opr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opr
-Version: 220
+Version: 230
 Summary: Object Programming Runtime
 Author-email: Bart Thate <programmingobject@gmail.com>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/opr
 Project-URL: bugs, https://github.com/bthate/opr/issues
 Project-URL: source, https://github.com/bthate/opr
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `opr-220/pyproject.toml` & `opr-230/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
+[options]
+zip_safe = true
+include_package_data = true
+
+
 [project]
 name = "opr"
 description = "Object Programming Runtime"
-version = "220"
+version = "230"
 authors = [
     {name = "Bart Thate", email = "programmingobject@gmail.com" },
 ]
 readme = "README.rst"
 license = { text="Public Domain"}
-classifiers=[
-             'Development Status :: 3 - Alpha',
-             'License :: Public Domain',
-             'Operating System :: Unix',
-             'Programming Language :: Python',
-             'Topic :: Utilities'
-            ]
+classifiers = [ 
+               'Development Status :: 3 - Alpha',
+               'License :: Public Domain',
+               'Operating System :: Unix',
+               'Programming Language :: Python',
+               'Topic :: Utilities'
+              ]
 
 
 [project.urls]
 "home" = "https://pypi.org/project/opr"
 "bugs" = "https://github.com/bthate/opr/issues"
 "source" = "https://github.com/bthate/opr"
 
 
-[project.scripts]
-opr = "opr.runtime:main"
-
-
 [project.optional-dependencies]
 dev = []
 
 [tool.setuptools]
-packages = [
-            "opr",
-            "opr.modules"
-           ]
-zip-safe = true
+script-files = ["bin/opr"]
+
+[tool.setuptools.packages.find]
+where = ["."]
+include = ["opr*"]
+exclude = ["tests*",]
+namespaces = false
+
+
+[tool.setuptools.package-data]
+"*" = ["bin/opr*"]
```

