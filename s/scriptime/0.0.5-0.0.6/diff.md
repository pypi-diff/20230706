# Comparing `tmp/scriptime-0.0.5.tar.gz` & `tmp/scriptime-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptime-0.0.5.tar", last modified: Thu Jul  6 02:44:59 2023, max compression
+gzip compressed data, was "scriptime-0.0.6.tar", last modified: Thu Jul  6 02:51:44 2023, max compression
```

## Comparing `scriptime-0.0.5.tar` & `scriptime-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 02:44:59.927643 scriptime-0.0.5/
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 02:44:59.927508 scriptime-0.0.5/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      142 2023-07-05 21:03:13.000000 scriptime-0.0.5/README.md
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 02:44:59.926593 scriptime-0.0.5/scriptime/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.0.5/scriptime/__init__.py
--rw-r--r--   0 jakestrasler   (501) staff       (20)     5007 2023-07-06 02:42:34.000000 scriptime-0.0.5/scriptime/main.py
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 02:44:59.927328 scriptime-0.0.5/scriptime.egg-info/
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 02:44:59.000000 scriptime-0.0.5/scriptime.egg-info/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      222 2023-07-06 02:44:59.000000 scriptime-0.0.5/scriptime.egg-info/SOURCES.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 02:44:59.000000 scriptime-0.0.5/scriptime.egg-info/dependency_links.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       19 2023-07-06 02:44:59.000000 scriptime-0.0.5/scriptime.egg-info/requires.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 02:44:59.000000 scriptime-0.0.5/scriptime.egg-info/top_level.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 02:44:59.927680 scriptime-0.0.5/setup.cfg
--rw-r--r--   0 jakestrasler   (501) staff       (20)      397 2023-07-06 02:43:37.000000 scriptime-0.0.5/setup.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 02:51:44.721733 scriptime-0.0.6/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 02:51:44.721590 scriptime-0.0.6/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      142 2023-07-05 21:03:13.000000 scriptime-0.0.6/README.md
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 02:51:44.720631 scriptime-0.0.6/scriptime/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.0.6/scriptime/__init__.py
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     4859 2023-07-06 02:51:26.000000 scriptime-0.0.6/scriptime/main.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 02:51:44.721399 scriptime-0.0.6/scriptime.egg-info/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 02:51:44.000000 scriptime-0.0.6/scriptime.egg-info/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      222 2023-07-06 02:51:44.000000 scriptime-0.0.6/scriptime.egg-info/SOURCES.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 02:51:44.000000 scriptime-0.0.6/scriptime.egg-info/dependency_links.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       19 2023-07-06 02:51:44.000000 scriptime-0.0.6/scriptime.egg-info/requires.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 02:51:44.000000 scriptime-0.0.6/scriptime.egg-info/top_level.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 02:51:44.721773 scriptime-0.0.6/setup.cfg
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      397 2023-07-06 02:51:32.000000 scriptime-0.0.6/setup.py
```

### Comparing `scriptime-0.0.5/scriptime/main.py` & `scriptime-0.0.6/scriptime/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,25 +101,22 @@
         email_body += f"Max CPU Usage: {cpu_usage:.2f}%\n"
         email_body += f"Max RAM Available: {ram_available:.2f}\n\n"
         email_body += f"System information: {system_info}\n"
         email_body += f"Processor: {processor}\n"
         email_body += f"Python Version: {python_version}\n"
         email_body += f"Packages Used: {self.pkgs}"
 
-        try:
-            with smtplib.SMTP(self.server, self.port) as smtp:
-                smtp.starttls()
-                smtp.login(self.sender_email, self.sender_password)
-                if isinstance(target, str):
-                    smtp.sendmail(self.sender_email, target, email_body)
-                elif isinstance(target, list):
-                    for email in target:
-                        smtp.sendmail(self.sender_email, email, email_body)
-        except Exception as e:
-            raise Exception(f"An error occurred sending an email: {e}")
+        with smtplib.SMTP(self.server, self.port) as smtp:
+            smtp.starttls()
+            smtp.login(self.sender_email, self.sender_password)
+            if isinstance(target, str):
+                smtp.sendmail(self.sender_email, target, email_body)
+            elif isinstance(target, list):
+                for email in target:
+                    smtp.sendmail(self.sender_email, email, email_body)
 
     def play_sound(self):
         wave_obj = sa.WaveObject.from_wave_file("resources/alert.wav")
         play_obj = wave_obj.play()
         play_obj.wait_done()
 
     def _get_pkgs(self):
```

