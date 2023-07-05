# Comparing `tmp/pyirecovery-0.1.4.tar.gz` & `tmp/pyirecovery-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyirecovery-0.1.4.tar", max compression
+gzip compressed data, was "pyirecovery-0.1.5.tar", max compression
```

## Comparing `pyirecovery-0.1.4.tar` & `pyirecovery-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-06-16 17:10:08.642664 pyirecovery-0.1.4/LICENSE
--rw-r--r--   0        0        0      451 2023-06-16 17:10:08.642921 pyirecovery-0.1.4/README.md
--rw-r--r--   0        0        0      233 2023-06-16 17:10:08.644459 pyirecovery-0.1.4/pyirecovery/__init__.py
--rw-r--r--   0        0        0     7869 2023-06-17 05:22:56.364189 pyirecovery-0.1.4/pyirecovery/__main__.py
--rw-r--r--   0        0        0     2900 2023-06-16 17:58:15.900281 pyirecovery-0.1.4/pyirecovery/no_backend_fix.py
--rw-r--r--   0        0        0      471 2023-06-17 05:23:22.334739 pyirecovery-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 pyirecovery-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-16 17:10:08.642664 pyirecovery-0.1.5/LICENSE
+-rw-r--r--   0        0        0      451 2023-06-16 17:10:08.642921 pyirecovery-0.1.5/README.md
+-rw-r--r--   0        0        0      233 2023-06-16 17:10:08.644459 pyirecovery-0.1.5/pyirecovery/__init__.py
+-rw-r--r--   0        0        0     7870 2023-06-18 14:11:29.167114 pyirecovery-0.1.5/pyirecovery/__main__.py
+-rw-r--r--   0        0        0     2927 2023-07-01 23:47:57.391127 pyirecovery-0.1.5/pyirecovery/no_backend_fix.py
+-rw-r--r--   0        0        0      470 2023-07-05 22:06:24.669999 pyirecovery-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 pyirecovery-0.1.5/PKG-INFO
```

### Comparing `pyirecovery-0.1.4/LICENSE` & `pyirecovery-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyirecovery-0.1.4/pyirecovery/__main__.py` & `pyirecovery-0.1.5/pyirecovery/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         click.echo('NONC: N/A')
     try:
         sep_nonce = binascii.hexlify(client.sep_nonce)
         click.echo(f'SNON: {sep_nonce.decode()}')
     except:
         click.echo('SNON: N/A')
     try:
-        pwned = (client._device_info['PWND']).replace('[', '')
+        pwned = (client._device_info['PWND']).replace('[', ']')
         pwned = pwned.replace(']', '')
         click.echo(f'PWND: {pwned}')
     except:
         pass
 
     click.echo(f'MODE: {mode_to_str(client.mode)}')
     for device in irecv_devices.IRECV_DEVICES:
```

### Comparing `pyirecovery-0.1.4/pyirecovery/no_backend_fix.py` & `pyirecovery-0.1.5/pyirecovery/no_backend_fix.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
                 #print("Didn't find {}\nin\n{}\nat line\n{}\nMoving on to next patch...".format(
                     #stockString, filepath, stringLine))
                 return -1
     else:
         #print("Couldn't find file at {}\nMoving on to next patch...".format(filepath))
         return -1
 
+# from m1stadev's Inferius
 def _get_backend():  # Attempt to find a libusb 1.0 library to use as pyusb's backend, exit if one isn't found.
     directories = (
         '/usr/local/lib',
         '/opt/procursus/lib',
         '/usr/lib',
         '/opt/homebrew/lib' # this works on my M2 Mac, tell me to add more if libusb is in a different path on your computer
     )  # Common library directories to search
```

### Comparing `pyirecovery-0.1.4/PKG-INFO` & `pyirecovery-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pyirecovery
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI wrapper of pymobiledevice3 that interacts with Recovery/DFU Apple devices
 License: GPL-3.0-only
 Author: Mini-Exploit
 Author-email: miniexploitttt@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pymobiledevice3 (>=1.36.2,<2.0.0)
+Requires-Dist: pymobiledevice3 (>=2.0.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## pyirecovery
 A CLI wrapper of pymobiledevice3 that interacts with Recovery/DFU Apple devices
 # Installation
 * Install with PIP:
 ```
```

