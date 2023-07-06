# Comparing `tmp/scriptime-0.0.8.tar.gz` & `tmp/scriptime-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptime-0.0.8.tar", last modified: Thu Jul  6 13:24:15 2023, max compression
+gzip compressed data, was "scriptime-0.0.9.tar", last modified: Thu Jul  6 13:33:13 2023, max compression
```

## Comparing `scriptime-0.0.8.tar` & `scriptime-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 13:24:15.686227 scriptime-0.0.8/
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 13:24:15.686078 scriptime-0.0.8/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      142 2023-07-05 21:03:13.000000 scriptime-0.0.8/README.md
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 13:24:15.684801 scriptime-0.0.8/scriptime/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.0.8/scriptime/__init__.py
--rw-r--r--   0 jakestrasler   (501) staff       (20)     5210 2023-07-06 13:21:33.000000 scriptime-0.0.8/scriptime/main.py
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 13:24:15.685856 scriptime-0.0.8/scriptime.egg-info/
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 13:24:15.000000 scriptime-0.0.8/scriptime.egg-info/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      222 2023-07-06 13:24:15.000000 scriptime-0.0.8/scriptime.egg-info/SOURCES.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 13:24:15.000000 scriptime-0.0.8/scriptime.egg-info/dependency_links.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       19 2023-07-06 13:24:15.000000 scriptime-0.0.8/scriptime.egg-info/requires.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 13:24:15.000000 scriptime-0.0.8/scriptime.egg-info/top_level.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 13:24:15.686272 scriptime-0.0.8/setup.cfg
--rw-r--r--   0 jakestrasler   (501) staff       (20)      397 2023-07-06 13:22:13.000000 scriptime-0.0.8/setup.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 13:33:13.942324 scriptime-0.0.9/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 13:33:13.942197 scriptime-0.0.9/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      142 2023-07-05 21:03:13.000000 scriptime-0.0.9/README.md
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 13:33:13.941277 scriptime-0.0.9/scriptime/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.0.9/scriptime/__init__.py
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5209 2023-07-06 13:28:00.000000 scriptime-0.0.9/scriptime/main.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 13:33:13.942022 scriptime-0.0.9/scriptime.egg-info/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 13:33:13.000000 scriptime-0.0.9/scriptime.egg-info/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      222 2023-07-06 13:33:13.000000 scriptime-0.0.9/scriptime.egg-info/SOURCES.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 13:33:13.000000 scriptime-0.0.9/scriptime.egg-info/dependency_links.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       19 2023-07-06 13:33:13.000000 scriptime-0.0.9/scriptime.egg-info/requires.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 13:33:13.000000 scriptime-0.0.9/scriptime.egg-info/top_level.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 13:33:13.942390 scriptime-0.0.9/setup.cfg
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      454 2023-07-06 13:33:11.000000 scriptime-0.0.9/setup.py
```

### Comparing `scriptime-0.0.8/scriptime/main.py` & `scriptime-0.0.9/scriptime/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         email_body += f"Elapsed Time: {elapsed_time_str}\n\n"
         email_body += f"Max RAM Usage: {ram_usage:.2f}%\n"
         email_body += f"Max CPU Usage: {cpu_usage:.2f}%\n"
         email_body += f"Max RAM Available: {ram_available:.2f} GB\n\n"
         email_body += f"System information: {system_info}\n"
         email_body += f"Processor: {processor}\n"
         email_body += f"Python Version: {python_version}\n\n"
-        email_body += f"Packages Used: {self.pkgs}\n"
+        email_body += f"Packages Used:\n{self.pkgs}"
 
         try:
             with smtplib.SMTP(self.server, self.port) as smtp:
                 smtp.starttls()
                 smtp.login(self.sender_email, self.sender_password)
                 if isinstance(target, str):
                     smtp.sendmail(self.sender_email, target, email_body)
```

