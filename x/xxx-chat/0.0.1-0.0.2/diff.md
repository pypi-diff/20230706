# Comparing `tmp/xxx-chat-0.0.1.tar.gz` & `tmp/xxx-chat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xxx-chat-0.0.1.tar", last modified: Wed Jul  5 09:52:57 2023, max compression
+gzip compressed data, was "xxx-chat-0.0.2.tar", last modified: Thu Jul  6 03:06:43 2023, max compression
```

## Comparing `xxx-chat-0.0.1.tar` & `xxx-chat-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-05 09:52:57.119119 xxx-chat-0.0.1/
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1062 2023-04-12 09:19:49.000000 xxx-chat-0.0.1/LICENSE
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1064 2023-07-05 09:52:57.118757 xxx-chat-0.0.1/PKG-INFO
--rw-r--r--   0 taofoxtel   (503) staff       (20)      665 2023-07-05 09:36:04.000000 xxx-chat-0.0.1/README.md
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-05 09:52:57.110230 xxx-chat-0.0.1/command/
--rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.1/command/__init__.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1108 2023-07-05 09:36:04.000000 xxx-chat-0.0.1/command/__main__.py
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-05 09:52:57.111276 xxx-chat-0.0.1/commons/
--rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.1/commons/__init__.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)     2557 2023-07-05 08:08:08.000000 xxx-chat-0.0.1/commons/config.py
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-05 09:52:57.112393 xxx-chat-0.0.1/configuration/
--rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.1/configuration/__init__.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1213 2023-04-12 09:19:49.000000 xxx-chat-0.0.1/configuration/profile_config.py
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-05 09:52:57.113755 xxx-chat-0.0.1/occ/
--rw-r--r--   0 taofoxtel   (503) staff       (20)     2840 2023-07-05 09:33:41.000000 xxx-chat-0.0.1/occ/CommandChat.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.1/occ/__init__.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)       38 2023-07-05 09:52:57.119223 xxx-chat-0.0.1/setup.cfg
--rw-r--r--   0 taofoxtel   (503) staff       (20)      780 2023-07-05 09:36:04.000000 xxx-chat-0.0.1/setup.py
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-05 09:52:57.115052 xxx-chat-0.0.1/utils/
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1223 2023-04-12 09:55:10.000000 xxx-chat-0.0.1/utils/CommonUtil.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.1/utils/__init__.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1533 2023-04-12 09:19:49.000000 xxx-chat-0.0.1/utils/logger.py
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-05 09:52:57.118178 xxx-chat-0.0.1/xxx_chat.egg-info/
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1064 2023-07-05 09:52:57.000000 xxx-chat-0.0.1/xxx_chat.egg-info/PKG-INFO
--rw-r--r--   0 taofoxtel   (503) staff       (20)      445 2023-07-05 09:52:57.000000 xxx-chat-0.0.1/xxx_chat.egg-info/SOURCES.txt
--rw-r--r--   0 taofoxtel   (503) staff       (20)        1 2023-07-05 09:52:57.000000 xxx-chat-0.0.1/xxx_chat.egg-info/dependency_links.txt
--rw-r--r--   0 taofoxtel   (503) staff       (20)       46 2023-07-05 09:52:57.000000 xxx-chat-0.0.1/xxx_chat.egg-info/entry_points.txt
--rw-r--r--   0 taofoxtel   (503) staff       (20)        6 2023-07-05 09:52:57.000000 xxx-chat-0.0.1/xxx_chat.egg-info/requires.txt
--rw-r--r--   0 taofoxtel   (503) staff       (20)       40 2023-07-05 09:52:57.000000 xxx-chat-0.0.1/xxx_chat.egg-info/top_level.txt
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.760973 xxx-chat-0.0.2/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1062 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/LICENSE
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1064 2023-07-06 03:06:43.760724 xxx-chat-0.0.2/PKG-INFO
+-rw-r--r--   0 taofoxtel   (503) staff       (20)      665 2023-07-05 09:36:04.000000 xxx-chat-0.0.2/README.md
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.756036 xxx-chat-0.0.2/command/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/command/__init__.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1107 2023-07-06 03:00:54.000000 xxx-chat-0.0.2/command/__main__.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.756589 xxx-chat-0.0.2/commons/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/commons/__init__.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     2506 2023-07-06 03:03:46.000000 xxx-chat-0.0.2/commons/config.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.757143 xxx-chat-0.0.2/configuration/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/configuration/__init__.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1213 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/configuration/profile_config.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)       38 2023-07-06 03:06:43.761055 xxx-chat-0.0.2/setup.cfg
+-rw-r--r--   0 taofoxtel   (503) staff       (20)      811 2023-07-06 03:04:22.000000 xxx-chat-0.0.2/setup.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.757998 xxx-chat-0.0.2/utils/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)      772 2023-07-06 01:29:12.000000 xxx-chat-0.0.2/utils/CommonUtil.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/utils/__init__.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1506 2023-07-06 03:00:54.000000 xxx-chat-0.0.2/utils/logger.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.758595 xxx-chat-0.0.2/xxx/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     2527 2023-07-06 03:00:54.000000 xxx-chat-0.0.2/xxx/CommandChat.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/xxx/__init__.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.760347 xxx-chat-0.0.2/xxx_chat.egg-info/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1064 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/PKG-INFO
+-rw-r--r--   0 taofoxtel   (503) staff       (20)      445 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        1 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 taofoxtel   (503) staff       (20)       46 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/entry_points.txt
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        6 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/requires.txt
+-rw-r--r--   0 taofoxtel   (503) staff       (20)       40 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/top_level.txt
```

### Comparing `xxx-chat-0.0.1/LICENSE` & `xxx-chat-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xxx-chat-0.0.1/PKG-INFO` & `xxx-chat-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xxx-chat
-Version: 0.0.1
+Version: 0.0.2
 Summary: use command to chat with openai models, for :bear:
 Home-page: https://github.com/
 Author: xoto
 Author-email: xxx.tao.c@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xxx-chat-0.0.1/README.md` & `xxx-chat-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xxx-chat-0.0.1/command/__main__.py` & `xxx-chat-0.0.2/command/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import absolute_import
 
 import click
 import pkg_resources
 
 import utils.logger as logger
 from configuration.profile_config import add_profile, add_default_profile
-from occ.CommandChat import CommandChat
 from utils.CommonUtil import waiting_stop
-
+from xxx.CommandChat import CommandChat
 
 VERSION = pkg_resources.require("xxx-chat")[0].version
 
 
 @click.group()
 @click.version_option(version=VERSION, prog_name='xxx-chat')
 def commandchat_operator():
```

### Comparing `xxx-chat-0.0.1/commons/config.py` & `xxx-chat-0.0.2/commons/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     if not homedir:
         logger.log_r("Home Directory Not found!! Set Envirnoment `HOME` ")
         exit()
     logger.debug("Home Directory : " + homedir)
     config_file_temp = os.path.join(homedir + "/.xxx/config")
     logger.debug("Config File Location : " + config_file_temp)
     if not os.path.exists(config_file_temp):
-        logger.log_r("ERROR: No Config file present. \n 你可以先使用 `xxx configure` 来进行配置")
+        logger.log_r("ERROR: No Config file present. \n")
         try:
             os.makedirs(os.path.dirname(config_file_temp))
         except OSError as exc:  # Guard against race condition
             logger.log_r("Directory found! but not config file")
 
         logger.debug("Creating config file")
         file = open(config_file_temp, "w")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xxx-chat-0.0.1/configuration/profile_config.py` & `xxx-chat-0.0.2/configuration/profile_config.py`

 * *Files identical despite different names*

### Comparing `xxx-chat-0.0.1/occ/CommandChat.py` & `xxx-chat-0.0.2/xxx/CommandChat.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-
+import http.client
 import json
-from commons.config import get_env
 import os
-import http.client
 
+import utils.logger as logger
+from commons.config import get_env
 from utils.CommonUtil import waiting_start, waiting_stop
 
 
 def get_home_path():
     homedir = os.environ.get('HOME', None)
     if os.name == 'nt':
         homedir = os.path.expanduser('~')
     return homedir
 
-class CommandChat:
 
+class CommandChat:
     DEFAULT_PROFILE = "default"
     DEFAULT_CHAT_LOG_ID = "chat-1"
 
     def __init__(self, profile=None, chat_log_id=None):
         self.api_key = get_env(profile or self.DEFAULT_PROFILE, "api_key")
         self.limit_history = int(get_env(profile or self.DEFAULT_PROFILE, "limit_history") or 4)
         self.chat_log_id = chat_log_id or self.DEFAULT_CHAT_LOG_ID
@@ -29,48 +29,34 @@
             open(self.file_name, 'w').close()
         self.messages = [json.loads(line) for line in (line.strip() for line in open(self.file_name)) if line.strip()]
 
     def chat(self, message):
         message = {"role": "user", "content": message}
         self.messages.append(message)
         waiting_start()
-        
-        conn = http.client.HTTPSConnection("3gxj2qqbul.execute-api.ap-southeast-1.amazonaws.com")
-        payload = ''
-        headers = {
+
+        connection = http.client.HTTPSConnection("3gxj2qqbul.execute-api.ap-southeast-1.amazonaws.com")
+        htp_headers = {
             'x-api-key': self.api_key,
             'x-message': json.dumps(message)
         }
-        conn.request("GET", "/default/gateway", payload, headers)
-        res = conn.getresponse()
-        data = res.read().decode('unicode_escape')
-        output_data = data[1:-1]
+        connection.request("GET", "/default/gateway", '', htp_headers)
+        response = connection.getresponse()
+        output_data = response.read().decode('unicode_escape')[1:-1]
 
-        waiting_stop()   
-        print(output_data)
+        waiting_stop()
+        logger.log_cy(output_data)
         print("\n")
         self.record_chat_logs(message, {"role": "assistant", "content": output_data})
 
     def record_chat_logs(self, content, completion_text):
         with open(self.file_name, 'r+') as f:
             lines = f.readlines()
             if len(lines) >= self.limit_history:
                 with open(os.path.join(self.folder_path, self.chat_log_id + '_history.log'), 'a+') as hf:
-                    hf.writelines(lines[:(self.limit_history)])
-                lines = lines[(self.limit_history):]
-            lines.append('\n{}\n{}'.format(json.dumps(content, ensure_ascii=False), json.dumps(completion_text, ensure_ascii=False)))
+                    hf.writelines(lines[:self.limit_history])
+                lines = lines[self.limit_history:]
+            lines.append('\n{}\n{}'.format(json.dumps(content, ensure_ascii=False),
+                                           json.dumps(completion_text, ensure_ascii=False)))
             f.seek(0)
             f.truncate()
             f.writelines(lines)
-
-
-if __name__ == '__main__':
-    conn = http.client.HTTPSConnection("3gxj2qqbul.execute-api.ap-southeast-1.amazonaws.com")
-    payload = ''
-    headers = {
-    'x-api-key': 'inlDSY1cPZ9eE60Vj72Hz5b0MCfXGvFAajZTVrtS'
-    }
-    conn.request("GET", "/default/gateway", payload, headers)
-    res = conn.getresponse()
-    data = res.read()
-    print(data.decode("utf-8"))
-
```

### Comparing `xxx-chat-0.0.1/setup.py` & `xxx-chat-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='xxx-chat',
-    version='0.0.1',
+    version='0.0.2',
     entry_points={
         'console_scripts': [
             'xxx = command.__main__:main'
         ]
     },
     author="xoto",
     author_email="xxx.tao.c@gmail.com",
     description="use command to chat with openai models, for :bear:",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     packages=setuptools.find_packages(),
+    include_package_data=True,
     install_requires=[
         'click'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `xxx-chat-0.0.1/utils/logger.py` & `xxx-chat-0.0.2/utils/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 
 debug_logging = False;
 
 all_colors = 'black', 'red', 'green', 'yellow', 'blue', 'magenta', \
-             'cyan', 'white', 'bright_black', 'bright_red', \
-             'bright_green', 'bright_yellow', 'bright_blue', \
-             'bright_magenta', 'bright_cyan', 'bright_white'
+    'cyan', 'white', 'bright_black', 'bright_red', \
+    'bright_green', 'bright_yellow', 'bright_blue', \
+    'bright_magenta', 'bright_cyan', 'bright_white'
 
 
 def log_c(*argv):
     if len(argv) == 1:
         click.echo(click.style(argv[0], fg='magenta', bold=True))
     if len(argv) == 2:
         click.secho(argv[0], nl=False)
```

### Comparing `xxx-chat-0.0.1/xxx_chat.egg-info/PKG-INFO` & `xxx-chat-0.0.2/xxx_chat.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xxx-chat
-Version: 0.0.1
+Version: 0.0.2
 Summary: use command to chat with openai models, for :bear:
 Home-page: https://github.com/
 Author: xoto
 Author-email: xxx.tao.c@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

