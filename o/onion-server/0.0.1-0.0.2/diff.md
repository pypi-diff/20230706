# Comparing `tmp/onion-server-0.0.1.tar.gz` & `tmp/onion-server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion-server-0.0.1.tar", last modified: Tue Jun 13 04:19:22 2023, max compression
+gzip compressed data, was "onion-server-0.0.2.tar", last modified: Thu Jul  6 14:23:42 2023, max compression
```

## Comparing `onion-server-0.0.1.tar` & `onion-server-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-06-13 04:19:22.114739 onion-server-0.0.1/
--rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)      104 2023-06-13 01:23:57.000000 onion-server-0.0.1/CHANGELOG.md
--rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)     1065 2023-06-13 01:15:27.000000 onion-server-0.0.1/LICENCE.txt
--rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)       31 2023-06-13 01:16:12.000000 onion-server-0.0.1/MANIFEST.in
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1024 2023-06-13 04:19:22.114739 onion-server-0.0.1/PKG-INFO
--rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)      395 2023-06-13 04:17:25.000000 onion-server-0.0.1/README.md
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15773 2023-06-13 03:17:52.000000 onion-server-0.0.1/__init__.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-06-13 04:19:22.114739 onion-server-0.0.1/onion_server.egg-info/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1024 2023-06-13 04:19:21.000000 onion-server-0.0.1/onion_server.egg-info/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      301 2023-06-13 04:19:21.000000 onion-server-0.0.1/onion_server.egg-info/SOURCES.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-06-13 04:19:21.000000 onion-server-0.0.1/onion_server.egg-info/dependency_links.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       44 2023-06-13 04:19:21.000000 onion-server-0.0.1/onion_server.egg-info/entry_points.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        9 2023-06-13 04:19:21.000000 onion-server-0.0.1/onion_server.egg-info/requires.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       13 2023-06-13 04:19:21.000000 onion-server-0.0.1/onion_server.egg-info/top_level.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15773 2023-06-13 04:15:30.000000 onion-server-0.0.1/onion_server.py
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-06-13 04:19:22.114739 onion-server-0.0.1/setup.cfg
--rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)     1220 2023-06-13 04:18:50.000000 onion-server-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:23:42.703410 onion-server-0.0.2/
+-rwxr-xr-x   0 root         (0) root         (0)      306 2023-07-06 13:46:22.000000 onion-server-0.0.2/CHANGELOG.md
+-rwxr-xr-x   0 root         (0) root         (0)     1065 2023-06-13 01:15:27.000000 onion-server-0.0.2/LICENCE.txt
+-rwxr-xr-x   0 root         (0) root         (0)       31 2023-06-13 01:16:12.000000 onion-server-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-07-06 14:23:42.691411 onion-server-0.0.2/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     1364 2023-07-06 14:19:56.000000 onion-server-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      169 2023-07-06 14:21:43.000000 onion-server-0.0.2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:23:42.691411 onion-server-0.0.2/onion_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 14:23:41.000000 onion-server-0.0.2/onion_server.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    16920 2023-07-06 13:46:05.000000 onion-server-0.0.2/onion_server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 14:23:42.703410 onion-server-0.0.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1220 2023-07-06 14:20:43.000000 onion-server-0.0.2/setup.py
```

### Comparing `onion-server-0.0.1/LICENCE.txt` & `onion-server-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `onion-server-0.0.1/__init__.py` & `onion-server-0.0.2/onion_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,20 @@
     BOX_INFO = 'SERVER'
 
     TASK_LIST = {}
 
 
     def change_hostname(new_hostname):
         sp.getoutput(f'hostname {new_hostname}')
-
+    
+    def init_config_file():
+        if path.isfile(f'{DIR_NAME}/config.ini') == False:
+            with open(f'{DIR_NAME}/config.ini', 'w') as config_file:
+                DEFAULT_CONFIG.write(config_file)
+    
     class Settings:
         def __init__(self, filename):
             self.config = ConfigParser()
             self.filename = filename
             self.config_dict = dict()
 
 
@@ -83,22 +88,32 @@
                 if VALUE == 'True':
                     section[KEY] = True
                 elif VALUE == 'False':
                     section[KEY] = False
                 elif VALUE == 'None':
                     section[KEY] = None
 
+        
+
         def make_config(self, section):
             for KEY in section:
                 VALUE = section[KEY]
                 if VALUE == None:
                     section[KEY] = 'None'
             
 
-
+    def make_process_stop():
+        processes = [TOR_SERVICE, HTTP_SERVER]
+        for i in range(2):
+            try:
+                stop(processes[i-1])
+            except:
+                ...
+            
+        change_hostname(SYSTEM_HOSTNAME)
 
 
     def kill_task(_type: str = HTTP_SERVER):
         server = 'python3 -m http.server --bind 127.0.0.1 8080'
         pid = []
 
         def kill(task):
@@ -169,14 +184,25 @@
         except:
             ...
 
         kill_task(name)
 
         process.terminate()
 
+    def reset(name):
+        KEY =  name + '_status'
+        CONFIG = settings.get('MAIN')
+
+        try:
+            CONFIG[KEY] = False
+            settings.update()
+        except:
+            ...
+
+        kill_task(name)
 
 
     def init_torrc():
         with open('/etc/tor/torrc', 'r') as file:
             file = file.readlines()
             SECTION_MARKER = "## This section is just for relays ##"
 
@@ -263,26 +289,38 @@
                     stop(processes[i-1])
                 except:
                     ...
             
         elif action == 'scan':
             update_server()
 
+        elif cmd == 'reboot' or cmd == 'restart':
+            make_process_stop()
+            return 'reboot'
+
 
     def handle_cmd(cmd):
         if cmd == 'exit':
+            make_process_stop()
+            exit()
+            
+        elif cmd == 'reset':
             processes = [TOR_SERVICE, HTTP_SERVER]
             for i in range(2):
-                try:
-                    stop(processes[i-1])
-                except:
-                    ...
-            
-            change_hostname(SYSTEM_HOSTNAME)
-            exit()
+                reset(processes[i-1])
+        
+        elif 'config' in cmd:
+            command = cmd.split('.')
+            action = command[1]
+
+            if action == 'del' or action == 'remove' or action == 'delete':
+                sp.getoutput(f'rm -r {DIR_NAME}/config.ini')
+            else:
+                init_config_file()
+                
         elif 'tor' in cmd:
             command = cmd.split('.')
             action = command[1]
             GET = settings.get('MAIN')
 
             if action == 'start':
                 if GET['tor_service_status'] != True:
@@ -428,18 +466,15 @@
     uname_section = f'{Fore.WHITE}┌──({Fore.RED + Style.BRIGHT + USERNAME}'
     host_section = f'㉿{HOSTNAME + Fore.WHITE + Style.NORMAL})-['
     input_section = f'{Fore.WHITE}└─{Fore.RED + Style.BRIGHT}${Style.RESET_ALL}'
 
     # __main__ code
     DIR_NAME = f'{path.dirname(__file__)}'
 
-    if path.isfile(f'{DIR_NAME}/config.ini') == False:
-        with open(f'{DIR_NAME}/config.ini', 'w') as config_file:
-            DEFAULT_CONFIG.write(config_file)
-            
+    init_config_file()
     settings = Settings(f'{DIR_NAME}/config.ini')
     init_torrc()
 
     if USERNAME != 'root':
         print(f'\n  [{Fore.YELLOW + Style.BRIGHT} MESSAGE {Style.RESET_ALL}]  {Fore.RED + Style.BRIGHT}Run as Root!{Style.RESET_ALL}')
     else:
         change_hostname('onion')
@@ -453,13 +488,22 @@
                 else:
                     BOX_INFO = FILE_DIR.removesuffix("/")
 
                 info_section = f'{Fore.LIGHTBLUE_EX + Style.BRIGHT + BOX_INFO + Fore.WHITE + Style.NORMAL}]\n'
 
                 print(f'''\n{uname_section + host_section + info_section + input_section} ''', end="")
                 handle_cmd(input())
-        except KeyboardInterrupt:
+        except SystemExit:
+            ...
+        except:
             change_hostname(SYSTEM_HOSTNAME)
+            print(f'\n\n  [{Fore.RED + Style.BRIGHT} ERROR {Style.RESET_ALL}]  An Error Occured... e0x00')
+
 
 
 if __name__ == '__main__':
-    main()
+    # main()
+    while True:
+        action = main()
+        if action != 'reboot':
+            break
+
```

### Comparing `onion-server-0.0.1/setup.py` & `onion-server-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     with codecs.open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as changelog:
         LONG_DESCRIPTION = readme.read() + '\n\n\n' + changelog.read()
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Dot-Onion Services Manager Client'
 KEYWORDS = ['tor', 'hosting', 'onion', 'hidden', 'services', 'server']
 
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
```

