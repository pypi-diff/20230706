# Comparing `tmp/scriptime-0.1.2.tar.gz` & `tmp/scriptime-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptime-0.1.2.tar", last modified: Thu Jul  6 20:06:37 2023, max compression
+gzip compressed data, was "scriptime-0.1.3.tar", last modified: Thu Jul  6 20:12:20 2023, max compression
```

## Comparing `scriptime-0.1.2.tar` & `scriptime-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:06:37.596033 scriptime-0.1.2/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       64 2023-07-06 20:05:31.000000 scriptime-0.1.2/MANIFEST.in
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 20:06:37.595886 scriptime-0.1.2/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)     4943 2023-07-06 19:42:35.000000 scriptime-0.1.2/README.md
--rw-r--r--   0 jakestrasler   (501) staff       (20)     4927 2023-07-06 20:05:24.000000 scriptime-0.1.2/README.rst
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:06:37.594875 scriptime-0.1.2/scriptime/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.1.2/scriptime/__init__.py
--rw-r--r--   0 jakestrasler   (501) staff       (20)   701148 2023-07-05 22:10:39.000000 scriptime-0.1.2/scriptime/alert.wav
--rw-r--r--   0 jakestrasler   (501) staff       (20)     9874 2023-07-06 19:55:45.000000 scriptime-0.1.2/scriptime/main.py
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:06:37.595622 scriptime-0.1.2/scriptime.egg-info/
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 20:06:37.000000 scriptime-0.1.2/scriptime.egg-info/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      265 2023-07-06 20:06:37.000000 scriptime-0.1.2/scriptime.egg-info/SOURCES.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 20:06:37.000000 scriptime-0.1.2/scriptime.egg-info/dependency_links.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       30 2023-07-06 20:06:37.000000 scriptime-0.1.2/scriptime.egg-info/requires.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 20:06:37.000000 scriptime-0.1.2/scriptime.egg-info/top_level.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 20:06:37.596089 scriptime-0.1.2/setup.cfg
--rw-r--r--   0 jakestrasler   (501) staff       (20)      476 2023-07-06 20:06:09.000000 scriptime-0.1.2/setup.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:12:20.072816 scriptime-0.1.3/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       64 2023-07-06 20:05:31.000000 scriptime-0.1.3/MANIFEST.in
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5231 2023-07-06 20:12:20.072679 scriptime-0.1.3/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     4943 2023-07-06 19:42:35.000000 scriptime-0.1.3/README.md
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:12:20.071633 scriptime-0.1.3/scriptime/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.1.3/scriptime/__init__.py
+-rw-r--r--   0 jakestrasler   (501) staff       (20)   701148 2023-07-05 22:10:39.000000 scriptime-0.1.3/scriptime/alert.wav
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     9874 2023-07-06 19:55:45.000000 scriptime-0.1.3/scriptime/main.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:12:20.072471 scriptime-0.1.3/scriptime.egg-info/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5231 2023-07-06 20:12:20.000000 scriptime-0.1.3/scriptime.egg-info/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      254 2023-07-06 20:12:20.000000 scriptime-0.1.3/scriptime.egg-info/SOURCES.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 20:12:20.000000 scriptime-0.1.3/scriptime.egg-info/dependency_links.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       30 2023-07-06 20:12:20.000000 scriptime-0.1.3/scriptime.egg-info/requires.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 20:12:20.000000 scriptime-0.1.3/scriptime.egg-info/top_level.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 20:12:20.072854 scriptime-0.1.3/setup.cfg
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      694 2023-07-06 20:12:13.000000 scriptime-0.1.3/setup.py
```

### Comparing `scriptime-0.1.2/README.md` & `scriptime-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.2/README.rst` & `scriptime-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,138 +1,139 @@
-scriptime
-=========
+Metadata-Version: 2.1
+Name: scriptime
+Version: 0.1.3
+Summary: A Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
+Author: Jake Strasler
+Author-email: jstr36@gmail.com
+Description-Content-Type: text/markdown
 
-Python library to notify when a script has finished running and
-providing insights such as run time, CPU and RAM usage, and more.
+# scriptime
+Python library to notify when a script has finished running and providing insights such as run time, CPU and RAM usage, and more.
 
--  `scriptime <#scriptime>`__
 
-   -  `About <#about>`__
-   -  `Getting Started <#getting-started>`__
-   -  `Using scriptimer <#using-scriptimer>`__
-   -  `Output <#output>`__
-
-About
------
-
-This project will send you an email or text message notifying you when a
-script has completed running. Configurable thorugh a config file,
-environment variables, or hardcoding the email credentials, this project
-has little overhead to get started.
-
-Getting Started
----------------
-
-The first step to using scriptime is setting up the email that will be
-sending the notifications. scriptime uses the built-in Python SMTP to
-send emails which requires an email address, said email’s password, and
-an SMTP SSL server and port. Therfore,
+- [scriptime](#scriptime)
+  - [About](#about)
+  - [Getting Started](#getting-started)
+  - [Using scriptimer](#using-scriptimer)
+  - [Output](#output)
 
-1. Choose how you will pass your email credential into scriptime:
-
-   1. **JSON config file** To set up, create a .json file with the
-      following contents:
-      ``{          "scriptime_email": "example@email.com",          "scriptime_password": "superSecure1",          "scriptime_server": "smtp.email.com"          "scriptime_port": 123>      }``
-
-   2. **Environment variables** *Recommended – if you plan to use
-      scriptime more than once this will be the simplest method over
-      time.* Set the following environment variales:
-      ``SCRIPTIME_EMAIL=example@email.com``
-      ``SCRIPTIME_PASSWORD=superSecure1``
-      ``SCRIPTIME_SERVER=smtp.email.com`` ``SCRIPTIME_PORT=123``
-
-   3. **Hard coding** If you choose to go the hard code route, when
-      creating the ``Timer`` object, you will need to pass in extra
-      arguments. Your constructor call should look something like:
-      ``python      timer = Timer(method="hardcode", email="example@email.com", password="superSecure1", server="smtp.email.com", port=123)``
-
-         Note that if you are using Gmail, you may have to create an
-         `app
-         password <https://support.google.com/accounts/answer/185833?hl=en>`__.
-         Your normal password will likely not work. Other email services
-         may have similar catches.
-
-Using scriptimer
-----------------
+## About
 
-The use of scriptimer is very straightforward:
-
-1. In a terminal, ``pip install scriptime``
+This project will send you an email or text message notifying you when a script has completed running. Configurable thorugh a config file, environment variables, or hardcoding the email credentials, this project has little overhead to get started.
 
-2. In a Python (.py) or Jupyter Notebook (.ipynb) file, add
-   ``python     from scriptime import Timer`` to your imports.
+## Getting Started
 
-3. Create an instance of a timer, which could be done in three ways
-   dependant on what you did in `Getting Started <#getting-started>`__:
+The first step to using scriptime is setting up the email that will be sending the notifications. scriptime uses the built-in Python SMTP to send emails which requires an email address, said email's password, and an SMTP SSL server and port. Therfore,
 
+1. Choose how you will pass your email credential into scriptime:
    1. **JSON config file**
-      ``python      timer = Timer(method="json", config_file="path/to/config.json")``
-
-   2. **Environment variables**
-      ``python      timer = Timer(method="env")``
-
-   3. **Hard coding** (This may look famiiliar):
-      ``python      timer = Timer(method="hardcode", email="example@email.com", password="superSecure1", server="smtp.email.com", port=123)``
-
-4. Start the timer
+        To set up, create a .json file with the following contents:
+        ```
+        {
+            "scriptime_email": "example@email.com",
+            "scriptime_password": "superSecure1",
+            "scriptime_server": "smtp.email.com"
+            "scriptime_port": 123>
+        }
+        ```
+    2. **Environment variables**
+        *Recommended -- if you plan to use scriptime more than once this will be the simplest method over time.*
+        Set the following environment variales:
+        `SCRIPTIME_EMAIL=example@email.com`
+        `SCRIPTIME_PASSWORD=superSecure1`
+        `SCRIPTIME_SERVER=smtp.email.com`
+        `SCRIPTIME_PORT=123`
+    3. **Hard coding**
+        If you choose to go the hard code route, when creating the `Timer` object, you will need to pass in extra arguments. Your constructor call should look something like:
+        ```python
+        timer = Timer(method="hardcode", email="example@email.com", password="superSecure1", server="smtp.email.com", port=123)
+        ```
 
-   .. code:: python
+        > Note that if you are using Gmail, you may have to create an [app password](https://support.google.com/accounts/answer/185833?hl=en). Your normal password will likely not work. Other email services may have similar catches.
 
-      timer.start()
 
-5. Then, at the end of the script (or wherever you would like a
-   notification), add one of or both of the following:
+## Using scriptimer
 
-   1. **Email notification** To get an email notification, simply call
-      the send_email function:
-      ``python      timer.send_email("receiver@email.com")``
-
-      You can also send a text using your carrier’s email-to-SMS
-      address. You can find your carrier at: `list of carrier SMS
-      emails <https://avtech.com/articles/138/list-of-email-to-sms-addresses/>`__
-      ``python   timer.send_email("0123456789@text.att.net")``
-
-      Multiple email addresses, phone numbers, or any combination
-      thereof can be passed in as a list:
-      ``python   timer.send_email(["receiver@email.com", "0123456789@text.att.net"])``
+The use of scriptimer is very straightforward:
 
-      Lastly, if you would like to see the output of the body in order
-      to have the statistics persistent or just because you’re curious,
-      simply use the ``print_body`` flag:
-      ``python   timer.send_email("receiver@email.com", print_body=True)``
+1. In a terminal, `pip install scriptime`
+2. In a Python (.py) or Jupyter Notebook (.ipynb) file, add
+    ```python
+    from scriptime import Timer
+    ``` 
+    to your imports.
+4. Create an instance of a timer, which could be done in three ways dependant on what you did in [Getting Started](#getting-started):
+   1. **JSON config file**
+        ```python
+        timer = Timer(method="json", config_file="path/to/config.json")
+        ```
 
-   2. **Play sound** If you would like an audible notification that your
-      script has finished, simply: ``python      timer.play_sound()`` >
-      If the time measurement aspect of this program is important to
-      you, be sure to run the play sound after sending the email (if you
-      are sending the email at the end of the script) as it takes ~5
-      seconds to play the sound.
+   2. **Environment variables**
+        ```python
+        timer = Timer(method="env")
+        ```
+   3. **Hard coding**
+        (This may look famiiliar):
+        ```python
+        timer = Timer(method="hardcode", email="example@email.com", password="superSecure1", server="smtp.email.com", port=123)
+        ```
+5. Start the timer
+   ```python
+   timer.start()
+   ```
+
+6. Then, at the end of the script (or wherever you would like a notification), add one of or both of the following:
+   1. **Email notification**
+        To get an email notification, simply call the send_email function:
+        ```python
+        timer.send_email("receiver@email.com")
+        ```
+
+        You can also send a text using your carrier's email-to-SMS address. You can find your carrier at: [list of carrier SMS emails](https://avtech.com/articles/138/list-of-email-to-sms-addresses/)
+        ```python
+        timer.send_email("0123456789@text.att.net")
+        ```
+
+        Multiple email addresses, phone numbers, or any combination thereof can be passed in as a list:
+        ```python
+        timer.send_email(["receiver@email.com", "0123456789@text.att.net"])
+        ```
+
+        Lastly, if you would like to see the output of the body in order to have the statistics persistent or just because you're curious, simply use the `print_body` flag:
+        ```python
+        timer.send_email("receiver@email.com", print_body=True)
+        ```
+   2. **Play sound**
+        If you would like an audible notification that your script has finished, simply:
+        ```python
+        timer.play_sound()
+        ```
+        > If the time measurement aspect of this program is important to you, be sure to run the play sound after sending the email (if you are sending the email at the end of the script) as it takes ~5 seconds to play the sound.
 
-Output
-------
+## Output
 
 The subject of the email will be:
 
-::
-
-   [MM-DD-YYYY HH:MM:SS] <name of file> Finished
+```
+[MM-DD-YYYY HH:MM:SS] <name of file> Finished
+```
 
 The email/text body will look like the following:
 
-::
-
-   Your script has finished.
-
-   Elapsed Time: 00:00:01
-
-   Max RAM Usage: 74.00%
-   Max CPU Usage: 40.90%
-   Remaining RAM Available: 2.08 GB
+```
+Your script has finished.
 
-   System information: Darwin
-   Processor: arm
-   Python Version: 3.11.4
+Elapsed Time: 00:00:01
 
-   Packages Used:
-   Package: numpy, Version: 1.24.2
-   Package: scikit-learn, Version: 1.2.2
-   ...
+Max RAM Usage: 74.00%
+Max CPU Usage: 40.90%
+Remaining RAM Available: 2.08 GB
+
+System information: Darwin
+Processor: arm
+Python Version: 3.11.4
+
+Packages Used:
+Package: numpy, Version: 1.24.2
+Package: scikit-learn, Version: 1.2.2
+...
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scriptime-0.1.2/scriptime/alert.wav` & `scriptime-0.1.3/scriptime/alert.wav`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.2/scriptime/main.py` & `scriptime-0.1.3/scriptime/main.py`

 * *Files identical despite different names*

