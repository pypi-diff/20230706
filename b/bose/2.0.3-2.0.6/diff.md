# Comparing `tmp/bose-2.0.3.tar.gz` & `tmp/bose-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-2.0.3.tar", last modified: Wed Jul  5 01:36:20 2023, max compression
+gzip compressed data, was "bose-2.0.6.tar", last modified: Thu Jul  6 12:05:39 2023, max compression
```

## Comparing `bose-2.0.3.tar` & `bose-2.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 01:36:20.736947 bose-2.0.3/
--rw-rw-rw-   0        0        0    14240 2023-07-05 01:36:20.736947 bose-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-2.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 01:36:20.736947 bose-2.0.3/bose/
--rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.3/bose/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.3/bose/account_generator.py
--rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.3/bose/analytics.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.3/bose/base_data.py
--rw-rw-rw-   0        0        0     8287 2023-07-01 12:32:35.823549 bose-2.0.3/bose/base_task.py
--rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.3/bose/beep_utils.py
--rw-rw-rw-   0        0        0    10014 2023-07-01 15:53:31.955272 bose-2.0.3/bose/bose_driver.py
--rw-rw-rw-   0        0        0    10026 2023-07-01 15:54:08.464721 bose-2.0.3/bose/bose_undetected_driver.py
--rw-rw-rw-   0        0        0     7884 2023-07-01 17:18:08.107702 bose-2.0.3/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.3/bose/download_driver.py
--rw-rw-rw-   0        0        0      948 2023-06-30 07:55:50.167685 bose-2.0.3/bose/ip_utils.py
--rw-rw-rw-   0        0        0     2995 2023-07-01 18:25:25.812969 bose-2.0.3/bose/launch_tasks.py
--rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.3/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.3/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.3/bose/opponent.py
--rw-rw-rw-   0        0        0     2510 2023-07-01 09:16:40.175639 bose-2.0.3/bose/output.py
--rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.3/bose/profile.py
--rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.3/bose/schedule_utils.py
--rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.3/bose/task_config.py
--rw-rw-rw-   0        0        0     1375 2023-07-01 09:14:29.721606 bose-2.0.3/bose/task_info.py
--rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.3/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7480 2023-07-03 07:28:55.309830 bose-2.0.3/bose/user_agent.py
--rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.3/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.3/bose/wait.py
--rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.675976 bose-2.0.3/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2312 2023-07-05 01:36:00.489143 bose-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:05:39.350177 bose-2.0.6/
+-rw-rw-rw-   0        0        0    14120 2023-07-06 12:05:39.389114 bose-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10357 2023-07-06 11:59:35.580609 bose-2.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 12:05:39.350177 bose-2.0.6/bose/
+-rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.6/bose/__init__.py
+-rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.6/bose/account_generator.py
+-rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.6/bose/analytics.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.6/bose/base_data.py
+-rw-rw-rw-   0        0        0     8287 2023-07-01 12:32:35.823549 bose-2.0.6/bose/base_task.py
+-rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.6/bose/beep_utils.py
+-rw-rw-rw-   0        0        0    10372 2023-07-06 11:45:35.506166 bose-2.0.6/bose/bose_driver.py
+-rw-rw-rw-   0        0        0    10384 2023-07-06 11:56:35.717259 bose-2.0.6/bose/bose_undetected_driver.py
+-rw-rw-rw-   0        0        0     7884 2023-07-01 17:18:08.107702 bose-2.0.6/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.6/bose/download_driver.py
+-rw-rw-rw-   0        0        0      993 2023-07-06 10:42:02.261172 bose-2.0.6/bose/ip_utils.py
+-rw-rw-rw-   0        0        0     2995 2023-07-01 18:25:25.812969 bose-2.0.6/bose/launch_tasks.py
+-rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.6/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.6/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.6/bose/opponent.py
+-rw-rw-rw-   0        0        0     2558 2023-07-05 08:58:01.580924 bose-2.0.6/bose/output.py
+-rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.6/bose/profile.py
+-rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.6/bose/schedule_utils.py
+-rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.6/bose/task_config.py
+-rw-rw-rw-   0        0        0     1375 2023-07-01 09:14:29.721606 bose-2.0.6/bose/task_info.py
+-rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.6/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7480 2023-07-03 07:28:55.309830 bose-2.0.6/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.6/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.6/bose/wait.py
+-rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.675976 bose-2.0.6/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2023-07-06 12:00:05.333647 bose-2.0.6/setup.py
```

### Comparing `bose-2.0.3/PKG-INFO` & `bose-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 2.0.3
+Version: 2.0.6
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: 🚀 Introducing ✨ Bose Framework - The Swiss Army Knife for Bot Developers 🤖
         =============================================================================
         
-        .. figure:: https://www.omkar.cloud/bose/assets/images/featured-0bacb14445a1b4cf367c10cd01454000.jpg
-        
         Bot Development is Tough.
         
         Bot Detectors like Cloudflare are ready to defend websites from our
         Bots. Configuring Selenium with ChromeOptions to specify the driver
         path, profile, user agent, and window size is Cumbersome and a nightmare
         in windows. Debugging Bot Crashes via logs is hard. How do you solve
         these pain points without sacrificing speed and handy development?
```

### Comparing `bose-2.0.3/README.rst` & `bose-2.0.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 🚀 Introducing ✨ Bose Framework - The Swiss Army Knife for Bot Developers 🤖
 =============================================================================
 
-.. figure:: https://www.omkar.cloud/bose/assets/images/featured-0bacb14445a1b4cf367c10cd01454000.jpg
-
 Bot Development is Tough.
 
 Bot Detectors like Cloudflare are ready to defend websites from our
 Bots. Configuring Selenium with ChromeOptions to specify the driver
 path, profile, user agent, and window size is Cumbersome and a nightmare
 in windows. Debugging Bot Crashes via logs is hard. How do you solve
 these pain points without sacrificing speed and handy development?
```

### Comparing `bose-2.0.3/bose/account_generator.py` & `bose-2.0.6/bose/account_generator.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/analytics.py` & `bose-2.0.6/bose/analytics.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/base_data.py` & `bose-2.0.6/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/base_task.py` & `bose-2.0.6/bose/base_task.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/bose_driver.py` & `bose-2.0.6/bose/bose_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,20 +273,30 @@
                 f'{self.task_path}/{filename}', 0)
             self.get_screenshot_as_file(
                 saving_screenshot_at)
         except:
             traceback.print_exc()
             print('Failed to save screenshot')
 
-    def prompt_to_solve_captcha(self):
+    def prompt_to_solve_captcha(self, more_rules = []):
         print('')
         print('   __ _ _ _    _                          _       _           ')
         print('  / _(_) | |  (_)                        | |     | |          ')
         print(' | |_ _| | |   _ _ __      ___ __ _ _ __ | |_ ___| |__   __ _ ')
         print(' |  _| | | |  | | `_ \    / __/ _` | `_ \| __/ __| `_ \ / _` |') 
         print(' | | | | | |  | | | | |  | (_| (_| | |_) | || (__| | | | (_| |')   # Tells user to solve captcha
         print(' |_| |_|_|_|  |_|_| |_|   \___\__,_| .__/ \__\___|_| |_|\__,_|')
         print('                                   | |                        ')
         print('                                   |_|                        ')
         print('')
 
-        return beep_input('Press fill in the captcha and press enter to continue ...', self.beep)
+        print('General Rules of Captcha Solving')
+        print(' - Solve it Fast')
+
+        for t in more_rules:
+            print(t)
+        # print('- Solve it Fast')
+        # print('1. If')
+
+        return beep_input('Press fill in the captcha, the faster the less detectable, then press enter to continue ...', self.beep)
+
+        # return beep_input('Press fill in the captcha and press enter to continue ...', self.beep)
```

### Comparing `bose-2.0.3/bose/bose_undetected_driver.py` & `bose-2.0.6/bose/bose_undetected_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,20 +273,30 @@
                 f'{self.task_path}/{filename}', 0)
             self.get_screenshot_as_file(
                 saving_screenshot_at)
         except:
             traceback.print_exc()
             print('Failed to save screenshot')
 
-    def prompt_to_solve_captcha(self):
+    def prompt_to_solve_captcha(self, more_rules = []):
         print('')
         print('   __ _ _ _    _                          _       _           ')
         print('  / _(_) | |  (_)                        | |     | |          ')
         print(' | |_ _| | |   _ _ __      ___ __ _ _ __ | |_ ___| |__   __ _ ')
         print(' |  _| | | |  | | `_ \    / __/ _` | `_ \| __/ __| `_ \ / _` |') 
         print(' | | | | | |  | | | | |  | (_| (_| | |_) | || (__| | | | (_| |')   # Tells user to solve captcha
         print(' |_| |_|_|_|  |_|_| |_|   \___\__,_| .__/ \__\___|_| |_|\__,_|')
         print('                                   | |                        ')
         print('                                   |_|                        ')
         print('')
 
-        return beep_input('Press fill in the captcha and press enter to continue ...', self.beep)
+        print('General Rules of Captcha Solving')
+        print(' - Solve it Fast')
+
+        for t in more_rules:
+            print(t)
+        # print('- Solve it Fast')
+        # print('1. If')
+
+        return beep_input('Press fill in the captcha, the faster the less detectable, then press enter to continue ...', self.beep)
+
+        # return beep_input('Press fill in the captcha and press enter to continue ...', self.beep)
```

### Comparing `bose-2.0.3/bose/create_driver.py` & `bose-2.0.6/bose/create_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/download_driver.py` & `bose-2.0.6/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/ip_utils.py` & `bose-2.0.6/bose/ip_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,16 @@
         response = requests.get(url, timeout=10)
         data =  (response.json())
 
         if "readme" in data:
            del data["readme"]
         return data
     except ReadTimeout:
-        return None
+        print('Refetching IP')
+        return find_ip_details()
     except Exception:
         traceback.print_exc()
         return None
     
 
 def find_ip():
     url = 'https://checkip.amazonaws.com/'
```

### Comparing `bose-2.0.3/bose/launch_tasks.py` & `bose-2.0.6/bose/launch_tasks.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/local_storage.py` & `bose-2.0.6/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/local_storage_driver.py` & `bose-2.0.6/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/output.py` & `bose-2.0.6/bose/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,12 +70,14 @@
     
         response = requests.get(url)
         if response.status_code == 200:
             # Extract the filename from the URL
             output_dir = "output"
 
             # Save the image in the output directory
+            path = f'{output_dir}/{filename}'
             with open(relative_path(
-                f'{output_dir}/{filename}', 0), "wb") as f:
+                path, 0), "wb") as f:
                 f.write(response.content)
         else:
             print("Failed to download the image.")
+            return path
```

### Comparing `bose-2.0.3/bose/profile.py` & `bose-2.0.6/bose/profile.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/schedule_utils.py` & `bose-2.0.6/bose/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/task_info.py` & `bose-2.0.6/bose/task_info.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/temp_mail.py` & `bose-2.0.6/bose/temp_mail.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/user_agent.py` & `bose-2.0.6/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/utils.py` & `bose-2.0.6/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/bose/window_size.py` & `bose-2.0.6/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.3/setup.py` & `bose-2.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     except:
       return None
     
             
 setup(
     name='bose',
     packages=['bose'],
-    version='2.0.3',
+    version='2.0.6',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/",
         "Source": "https://github.com/omkarcloud/bose",
         "Tracker": "https://github.com/omkarcloud/bose/issues",
     },
```

