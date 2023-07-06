# Comparing `tmp/simfwp-0.0.1.tar.gz` & `tmp/simfwp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfwp-0.0.1.tar", last modified: Thu Jul  6 04:00:39 2023, max compression
+gzip compressed data, was "simfwp-0.0.2.tar", last modified: Thu Jul  6 04:39:48 2023, max compression
```

## Comparing `simfwp-0.0.1.tar` & `simfwp-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 04:00:39.246883 simfwp-0.0.1/
--rw-rw-rw-   0        0        0       66 2023-07-06 03:12:24.000000 simfwp-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0      597 2023-07-06 03:15:36.000000 simfwp-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-07-06 03:15:38.000000 simfwp-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      970 2023-07-06 04:00:39.245883 simfwp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-07-06 03:40:45.000000 simfwp-0.0.1/README.md
--rw-rw-rw-   0        0        0      351 2023-07-06 03:07:40.000000 simfwp-0.0.1/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-06 04:00:39.246883 simfwp-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-07-06 03:57:40.000000 simfwp-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 04:00:39.242882 simfwp-0.0.1/simfwp.egg-info/
--rw-rw-rw-   0        0        0      970 2023-07-06 04:00:39.000000 simfwp-0.0.1/simfwp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-06 04:00:39.000000 simfwp-0.0.1/simfwp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 04:00:39.000000 simfwp-0.0.1/simfwp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 04:00:39.000000 simfwp-0.0.1/simfwp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 04:39:48.861901 simfwp-0.0.2/
+-rw-rw-rw-   0        0        0       66 2023-07-06 04:33:49.000000 simfwp-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0      597 2023-07-06 03:15:36.000000 simfwp-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-07-06 03:15:38.000000 simfwp-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      770 2023-07-06 04:39:48.860900 simfwp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-07-06 03:40:45.000000 simfwp-0.0.2/README.md
+-rw-rw-rw-   0        0        0      351 2023-07-06 03:07:40.000000 simfwp-0.0.2/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 04:39:48.862900 simfwp-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-07-06 04:33:49.000000 simfwp-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 04:39:48.858900 simfwp-0.0.2/simfwp.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-07-06 04:39:48.000000 simfwp-0.0.2/simfwp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-06 04:39:48.000000 simfwp-0.0.2/simfwp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 04:39:48.000000 simfwp-0.0.2/simfwp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 04:39:48.000000 simfwp-0.0.2/simfwp.egg-info/top_level.txt
```

### Comparing `simfwp-0.0.1/LICENCE.txt` & `simfwp-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `simfwp-0.0.1/setup.py` & `simfwp-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from setuptools import setup, find_packages
 
 setup(
     name="simfwp",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     install_requires=[
         # List your project dependencies here, e.g.
         # "numpy>=1.0",
         # "pandas>=1.0",
     ],
     entry_points={
         "console_scripts": [
             # If your project has command-line scripts, add their entry points here, e.g.
             # "my_script=my_package.my_module:main",
         ],
     },
-    python_requires=">=3.6",
+    python_requires=">=3.11",
     # Add metadata about your project
     author="Jacob Meyers",
     author_email="jakejem@outlook.com",
     description="Makes Reading, Writing, Adding to files easier.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
+		"Programming Language :: Python :: 3.11",
     ],
 )
```

