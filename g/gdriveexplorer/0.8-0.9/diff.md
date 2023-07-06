# Comparing `tmp/gdriveexplorer-0.8.tar.gz` & `tmp/gdriveexplorer-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdriveexplorer-0.8.tar", last modified: Tue Jan 17 12:19:46 2023, max compression
+gzip compressed data, was "gdriveexplorer-0.9.tar", last modified: Tue Jan 17 12:24:29 2023, max compression
```

## Comparing `gdriveexplorer-0.8.tar` & `gdriveexplorer-0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-01-17 12:19:46.581864 gdriveexplorer-0.8/
--rw-rw-rw-   0        0        0      836 2023-01-17 12:19:46.582601 gdriveexplorer-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-17 12:19:46.581602 gdriveexplorer-0.8/gdriveexplorer/
--rw-rw-rw-   0        0        0       56 2023-01-16 21:54:43.839301 gdriveexplorer-0.8/gdriveexplorer/__init__.py
--rw-rw-rw-   0        0        0     7570 2023-01-17 12:16:13.407568 gdriveexplorer-0.8/gdriveexplorer/gdriveexplorer.py
--rw-rw-rw-   0        0        0       39 2023-01-12 11:04:42.685736 gdriveexplorer-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1806 2023-01-17 12:17:36.369192 gdriveexplorer-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-17 12:24:29.001962 gdriveexplorer-0.9/
+-rw-rw-rw-   0        0        0      836 2023-01-17 12:24:29.002568 gdriveexplorer-0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-01-17 12:24:29.001194 gdriveexplorer-0.9/gdriveexplorer/
+-rw-rw-rw-   0        0        0       56 2023-01-16 21:54:43.839301 gdriveexplorer-0.9/gdriveexplorer/__init__.py
+-rw-rw-rw-   0        0        0     7569 2023-01-17 12:23:29.476875 gdriveexplorer-0.9/gdriveexplorer/gdriveexplorer.py
+-rw-rw-rw-   0        0        0       39 2023-01-12 11:04:42.685736 gdriveexplorer-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1806 2023-01-17 12:23:44.865188 gdriveexplorer-0.9/setup.py
```

### Comparing `gdriveexplorer-0.8/PKG-INFO` & `gdriveexplorer-0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: gdriveexplorer
-Version: 0.8
+Version: 0.9
 Summary: Class to help managing google drive files
 Home-page: https://github.com/sunep12/gdriveexplorer
 Author: Sunep
 Author-email: your.email@domain.com
 License: GPLv3+
-Download-URL: https://github.com/sunep12/gdriveexplorer/archive/refs/tags/v_08.tar.gz
+Download-URL: https://github.com/sunep12/gdriveexplorer/archive/refs/tags/v_09.tar.gz
 Description: UNKNOWN
 Keywords: GOOGLE DRIVE,API,WRAPPER
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `gdriveexplorer-0.8/gdriveexplorer/gdriveexplorer.py` & `gdriveexplorer-0.9/gdriveexplorer/gdriveexplorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
             os.remove('temp.csv')
 
             return df_
 
         else:
 
-            return pd.read_csv(io.StringIO(get_file_from_path(path_from_base, base).decode(decode)), **kwargs)
+            return pd.read_csv(io.StringIO(self.get_file_from_path(path_from_base).decode(decode)), **kwargs)
 
     def read_excel(self, path_from_base, **kwargs):
 
         return pd.read_excel(self.get_file_from_path(path_from_base), **kwargs)
 
     def create_or_update_file(self, path_from_base, base):
```

### Comparing `gdriveexplorer-0.8/setup.py` & `gdriveexplorer-0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'gdriveexplorer',         # How you named your package folder (MyLib)
   packages = ['gdriveexplorer'],   # Chose the same as "name"
-  version = '0.8',      # Start with a small number and increase it with every change you make
+  version = '0.9',      # Start with a small number and increase it with every change you make
   license='GPLv3+',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Class to help managing google drive files',   # Give a short description about your library
   author = 'Sunep',                   # Type in your name
   author_email = 'your.email@domain.com',      # Type in your E-Mail
   url = 'https://github.com/sunep12/gdriveexplorer',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/sunep12/gdriveexplorer/archive/refs/tags/v_08.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/sunep12/gdriveexplorer/archive/refs/tags/v_09.tar.gz',    # I explain this later on
   keywords = ['GOOGLE DRIVE', 'API', 'WRAPPER'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'PyDrive',
           'google.colab',
           'oauth2client',
           'google-api-python-client',
           'pandas'
```

