# Comparing `tmp/red-connector-ssh-1.2.tar.gz` & `tmp/red-connector-ssh-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red-connector-ssh-1.2.tar", last modified: Tue Nov  5 11:19:02 2019, max compression
+gzip compressed data, was "red-connector-ssh-1.3.tar", max compression
```

## Comparing `red-connector-ssh-1.2.tar` & `red-connector-ssh-1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    34523 2019-03-26 11:07:42.910330 red-connector-ssh-1.2/LICENSE
--rw-r--r--   0        0        0      657 2019-03-26 11:07:42.910330 red-connector-ssh-1.2/README.md
--rw-r--r--   0        0        0      708 2019-11-05 11:17:11.845073 red-connector-ssh-1.2/pyproject.toml
--rw-r--r--   0        0        0       69 2019-03-26 11:07:42.912330 red-connector-ssh-1.2/red_connector_ssh/__init__.py
--rw-r--r--   0        0        0       79 2019-03-26 11:07:42.912330 red-connector-ssh-1.2/red_connector_ssh/__main__.py
--rw-r--r--   0        0        0      809 2019-03-26 11:07:42.912330 red-connector-ssh-1.2/red_connector_ssh/cli_modes.py
--rw-r--r--   0        0        0        0 2019-03-26 11:07:42.912330 red-connector-ssh-1.2/red_connector_ssh/convert_ssh_key/__init__.py
--rw-r--r--   0        0        0       95 2019-03-26 11:07:42.912330 red-connector-ssh-1.2/red_connector_ssh/convert_ssh_key/__main__.py
--rw-r--r--   0        0        0     3310 2019-10-15 12:47:26.306963 red-connector-ssh-1.2/red_connector_ssh/convert_ssh_key/main.py
--rw-r--r--   0        0        0    10904 2019-11-05 11:17:59.652655 red-connector-ssh-1.2/red_connector_ssh/helpers.py
--rw-r--r--   0        0        0     2399 2019-08-22 13:52:18.933921 red-connector-ssh-1.2/red_connector_ssh/main.py
--rw-r--r--   0        0        0    12592 2019-11-05 11:16:47.040289 red-connector-ssh-1.2/red_connector_ssh/mount_dir.py
--rw-r--r--   0        0        0     2500 2019-11-05 11:17:59.652655 red-connector-ssh-1.2/red_connector_ssh/schemas.py
--rw-r--r--   0        0        0     6628 2019-10-15 12:47:26.307963 red-connector-ssh-1.2/red_connector_ssh/send_receive_dir.py
--rw-r--r--   0        0        0     5296 2019-10-15 12:47:26.308963 red-connector-ssh-1.2/red_connector_ssh/send_receive_file.py
--rw-r--r--   0        0        0       16 2019-11-05 11:17:11.854073 red-connector-ssh-1.2/red_connector_ssh/version.py
--rw-r--r--   0        0        0     1672 1970-01-01 00:00:00.000000 red-connector-ssh-1.2/setup.py
--rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 red-connector-ssh-1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/LICENSE
+-rw-r--r--   0        0        0      657 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/README.md
+-rw-r--r--   0        0        0      708 2023-07-06 10:12:56.421639 red-connector-ssh-1.3/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/__main__.py
+-rw-r--r--   0        0        0      809 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/cli_modes.py
+-rw-r--r--   0        0        0        0 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/convert_ssh_key/__init__.py
+-rw-r--r--   0        0        0       95 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/convert_ssh_key/__main__.py
+-rw-r--r--   0        0        0     3310 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/convert_ssh_key/main.py
+-rw-r--r--   0        0        0    11692 2023-07-06 10:12:56.421639 red-connector-ssh-1.3/red_connector_ssh/helpers.py
+-rw-r--r--   0        0        0     2399 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/main.py
+-rw-r--r--   0        0        0    12592 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/mount_dir.py
+-rw-r--r--   0        0        0     2626 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/schemas.py
+-rw-r--r--   0        0        0     7327 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/send_receive_dir.py
+-rw-r--r--   0        0        0     6175 2023-07-04 11:36:43.818381 red-connector-ssh-1.3/red_connector_ssh/send_receive_file.py
+-rw-r--r--   0        0        0       16 2023-07-06 10:12:56.421639 red-connector-ssh-1.3/red_connector_ssh/version.py
+-rw-r--r--   0        0        0     1722 2023-07-06 10:19:15.154155 red-connector-ssh-1.3/setup.py
+-rw-r--r--   0        0        0     1600 2023-07-06 10:19:15.154343 red-connector-ssh-1.3/PKG-INFO
```

### Comparing `red-connector-ssh-1.2/LICENSE` & `red-connector-ssh-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `red-connector-ssh-1.2/README.md` & `red-connector-ssh-1.3/README.md`

 * *Files identical despite different names*

### Comparing `red-connector-ssh-1.2/red_connector_ssh/cli_modes.py` & `red-connector-ssh-1.3/red_connector_ssh/cli_modes.py`

 * *Files identical despite different names*

### Comparing `red-connector-ssh-1.2/red_connector_ssh/convert_ssh_key/main.py` & `red-connector-ssh-1.3/red_connector_ssh/convert_ssh_key/main.py`

 * *Files identical despite different names*

### Comparing `red-connector-ssh-1.2/red_connector_ssh/helpers.py` & `red-connector-ssh-1.3/red_connector_ssh/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from functools import wraps
 from shutil import which
 
 from paramiko import SSHClient, AutoAddPolicy, RSAKey, SFTPClient, AuthenticationException, SSHException
 from scp import SCPException
 
 DEFAULT_PORT = 22
+DEFAULT_BANNER_TIMEOUT = 60
+DEFAULT_TIMEOUT = 120
+DEFAULT_AUTH_TIMEOUT = 60
 
 
 def graceful_error(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
@@ -107,42 +110,50 @@
     except IOError:
         dirname, basename = os.path.split(os.path.normpath(dir_path))
         _ssh_mkdir_recursive(sftp, dirname)
         sftp.mkdir(basename)
         sftp.chdir(basename)
 
 
-def create_ssh_client(host, port, username, password, private_key, passphrase):
+def create_ssh_client(host, port, username, password, private_key, passphrase, timeout=DEFAULT_TIMEOUT,
+                      auth_timeout=DEFAULT_AUTH_TIMEOUT, banner_timeout=DEFAULT_BANNER_TIMEOUT):
     """
     Creates and returns a connected SSHClient.
     If a password is supplied the connection is created using this password.
     If no password is supplied a valid private key must be present. If this private key is encrypted the associated
     passphrase must be supplied.
 
     :param host: The host to connect to
     :param username: The username which is used to connect to the ssh host
     :param port: The port number to connect to
     :param password: The password to authenticate
     :param private_key: A valid private RSA key as string
     :param passphrase: A passphrase to decrypt the private key, if the private key is encrypted
+    :param timeout: The timeout for the tcp connection. Defaults to 120.
+    :param auth_timeout: The authentication timeout in seconds. Defaults to 60.
+    :param banner_timeout: The banner timeout for the client in seconds. Defaults to 60.
 
     :return: A connected paramiko.SSHClient
 
     :raise ConnectionError: If the connection to the remote host failed or if neither password nor pkey are specified
     :raise InvalidAuthenticationError: If the authentication to the remote host failed
     """
     client = SSHClient()
     client.set_missing_host_key_policy(AutoAddPolicy())
+
     if password is not None:
         try:
             client.connect(
                 host,
                 port=port,
                 username=username,
-                password=password
+                password=password,
+                timeout=timeout,
+                auth_timeout=auth_timeout,
+                banner_timeout=banner_timeout
             )
         except socket.gaierror:
             raise ConnectionError('Could not connect to remote host "{}"'.format(host))
         except AuthenticationException:
             raise InvalidAuthenticationError(
                 'Could not connect to remote host "{}". Invalid username/password.'.format(host)
             )
@@ -150,15 +161,15 @@
         with create_temp_file(private_key) as key_file:
             try:
                 pkey = RSAKey.from_private_key(key_file, password=passphrase)
             except SSHException:
                 raise InvalidAuthenticationError('Could not connect to remote host "{}". Invalid key.'.format(host))
 
         try:
-            client.connect(host, username=username, pkey=pkey)
+            client.connect(host, port=port, username=username, pkey=pkey)
         except socket.gaierror:
             raise ConnectionError('Could not connect to remote host "{}"'.format(host))
     else:
         raise ConnectionError('At least password or private_key must be present.')
 
     return client
 
@@ -260,15 +271,18 @@
 
     with create_ssh_client(
             host=access['host'],
             port=access.get('port', DEFAULT_PORT),
             username=auth['username'],
             password=auth.get('password'),
             private_key=auth.get('privateKey'),
-            passphrase=auth.get('passphrase')
+            passphrase=auth.get('passphrase'),
+            timeout=access.get('timeout', DEFAULT_TIMEOUT),
+            auth_timeout=access.get('authTimeout', DEFAULT_AUTH_TIMEOUT),
+            banner_timeout=access.get('bannerTimeout', DEFAULT_BANNER_TIMEOUT)
     ) as client:
         with client.open_sftp() as sftp:
             try:
                 sftp.listdir(remote_dir_path)
             except FileNotFoundError:
                 raise FileNotFoundError('Could not find remote directory "{}"'.format(remote_dir_path))
```

### Comparing `red-connector-ssh-1.2/red_connector_ssh/main.py` & `red-connector-ssh-1.3/red_connector_ssh/main.py`

 * *Files identical despite different names*

### Comparing `red-connector-ssh-1.2/red_connector_ssh/mount_dir.py` & `red-connector-ssh-1.3/red_connector_ssh/mount_dir.py`

 * *Files identical despite different names*

### Comparing `red-connector-ssh-1.2/red_connector_ssh/schemas.py` & `red-connector-ssh-1.3/red_connector_ssh/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 
 _BASE_SCHEMA = {
     'type': 'object',
     'properties': {
         'host': {'type': 'string'},
         'port': {'type': 'integer'},
         'auth': _AUTH_SCHEMA,
+        'timeout': {'type': 'number'},
+        'authTimeout': {'type': 'number'},
+        'bannerTimeout': {'type': 'number'}
     },
     'additionalProperties': False,
     'required': ['host', 'auth']
 }
 
 
 FILE_SCHEMA = deepcopy(_BASE_SCHEMA)
```

### Comparing `red-connector-ssh-1.2/red_connector_ssh/send_receive_dir.py` & `red-connector-ssh-1.3/red_connector_ssh/send_receive_dir.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from argparse import ArgumentParser
 
 import jsonschema
 from scp import SCPClient, SCPException
 
 from red_connector_ssh.schemas import DIR_SCHEMA, LISTING_SCHEMA
 from red_connector_ssh.helpers import create_ssh_client, fetch_directory, DEFAULT_PORT, graceful_error, \
-    send_directory, ssh_mkdir, cut_remote_user_dir, check_remote_dir_available
+    send_directory, ssh_mkdir, cut_remote_user_dir, check_remote_dir_available, DEFAULT_BANNER_TIMEOUT, DEFAULT_TIMEOUT, \
+    DEFAULT_AUTH_TIMEOUT
 
 RECEIVE_DIR_DESCRIPTION = 'Receive input dir from SSH server.'
 RECEIVE_DIR_VALIDATE_DESCRIPTION = 'Validate access data for receive-dir.'
 
 SEND_DIR_DESCRIPTION = 'Send output dir to SSH server.'
 SEND_DIR_VALIDATE_DESCRIPTION = 'Validate access data for send-dir.'
 
@@ -40,15 +41,18 @@
 
     with create_ssh_client(
         host=access['host'],
         port=access.get('port', DEFAULT_PORT),
         username=auth['username'],
         password=auth.get('password'),
         private_key=auth.get('privateKey'),
-        passphrase=auth.get('passphrase')
+        passphrase=auth.get('passphrase'),
+        timeout=access.get('timeout', DEFAULT_TIMEOUT),
+        auth_timeout=access.get('authTimeout', DEFAULT_AUTH_TIMEOUT),
+        banner_timeout=access.get('bannerTimeout', DEFAULT_BANNER_TIMEOUT)
     ) as client:
         with SCPClient(client.get_transport()) as scp_client:
             if listing:
                 try:
                     os.mkdir(local_dir_path)
                 except FileExistsError:
                     pass
@@ -82,15 +86,18 @@
 
     with create_ssh_client(
             host=access['host'],
             port=access.get('port', DEFAULT_PORT),
             username=auth['username'],
             password=auth.get('password'),
             private_key=auth.get('privateKey'),
-            passphrase=auth.get('passphrase')
+            passphrase=auth.get('passphrase'),
+            timeout=access.get('timeout', DEFAULT_TIMEOUT),
+            auth_timeout=access.get('authTimeout', DEFAULT_AUTH_TIMEOUT),
+            banner_timeout=access.get('bannerTimeout', DEFAULT_BANNER_TIMEOUT)
     ) as ssh_client:
         if listing:
             with ssh_client.open_sftp() as sftp_client:
                 ssh_mkdir(sftp_client, remote_dir_path)
                 send_directory(listing, sftp_client, local_dir_path, remote_dir_path)
         else:
             with ssh_client.open_sftp() as sftp_client:
@@ -111,15 +118,18 @@
     auth = access['auth']
     with create_ssh_client(
             host=access['host'],
             port=access.get('port', DEFAULT_PORT),
             username=auth['username'],
             password=auth.get('password'),
             private_key=auth.get('privateKey'),
-            passphrase=auth.get('passphrase')
+            passphrase=auth.get('passphrase'),
+            timeout=access.get('timeout', DEFAULT_TIMEOUT),
+            auth_timeout=access.get('authTimeout', DEFAULT_AUTH_TIMEOUT),
+            banner_timeout=access.get('bannerTimeout', DEFAULT_BANNER_TIMEOUT)
     ):
         pass
 
 
 @graceful_error
 def receive_dir():
     parser = ArgumentParser(description=RECEIVE_DIR_DESCRIPTION)
```

### Comparing `red-connector-ssh-1.2/setup.py` & `red-connector-ssh-1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # -*- coding: utf-8 -*-
-from distutils.core import setup
+from setuptools import setup
 
 packages = \
 ['red_connector_ssh', 'red_connector_ssh.convert_ssh_key']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['jsonschema>=3.0,<4.0',
- 'paramiko>=2.5,<3.0',
+ 'paramiko>=3.0,<4.0',
  'pexpect>=4.7.0,<5.0.0',
  'scp>=0.13.0,<0.14.0']
 
 entry_points = \
 {'console_scripts': ['red-connector-ssh = red_connector_ssh.main:main',
                      'red-convert-ssh-key = '
                      'red_connector_ssh.convert_ssh_key.main:main']}
 
 setup_kwargs = {
     'name': 'red-connector-ssh',
-    'version': '1.2',
+    'version': '1.3',
     'description': 'RED Connector SSH is part of the Curious Containers project.',
     'long_description': '# RED Connector SSH\n\nRED Connector SSH is part of the Curious Containers project.\n\nFor more information please refer to the Curious Containers [documentation](https://www.curious-containers.cc/).\n\n## Acknowledgements\n\nThe Curious Containers software is developed at [CBMI](https://cbmi.htw-berlin.de/) (HTW Berlin - University of Applied Sciences). The work is supported by the German Federal Ministry of Economic Affairs and Energy (ZIM project BeCRF, grant number KF3470401BZ4), the German Federal Ministry of Education and Research (project deep.TEACHING, grant number 01IS17056 and project deep.HEALTH, grant number 13FH770IX6) and HTW Berlin Booster.\n\n',
     'author': 'Christoph Jansen',
     'author_email': 'Christoph.Jansen@htw-berlin.de',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://www.curious-containers.cc/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.4,<4.0',
+    'python_requires': '>=3.6,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `red-connector-ssh-1.2/PKG-INFO` & `red-connector-ssh-1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: red-connector-ssh
-Version: 1.2
+Version: 1.3
 Summary: RED Connector SSH is part of the Curious Containers project.
 Home-page: https://www.curious-containers.cc/
 License: AGPL-3.0
 Author: Christoph Jansen
 Author-email: Christoph.Jansen@htw-berlin.de
-Requires-Python: >=3.4,<4.0
+Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: jsonschema (>=3.0,<4.0)
-Requires-Dist: paramiko (>=2.5,<3.0)
+Requires-Dist: paramiko (>=3.0,<4.0)
 Requires-Dist: pexpect (>=4.7.0,<5.0.0)
 Requires-Dist: scp (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/curious-containers/red-connector-ssh
 Description-Content-Type: text/markdown
 
 # RED Connector SSH
```

