# Comparing `tmp/xpath-localizer-1.0.3.tar.gz` & `tmp/xpath-localizer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpath-localizer-1.0.3.tar", last modified: Sat Feb 18 13:11:45 2023, max compression
+gzip compressed data, was "xpath-localizer-1.0.4.tar", last modified: Thu Jul  6 13:27:16 2023, max compression
```

## Comparing `xpath-localizer-1.0.3.tar` & `xpath-localizer-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 skayano    (501) staff       (20)        0 2023-02-18 13:11:45.484316 xpath-localizer-1.0.3/
--rw-r--r--   0 skayano    (501) staff       (20)     1064 2022-08-27 13:26:59.000000 xpath-localizer-1.0.3/LICENSE
--rw-r--r--   0 skayano    (501) staff       (20)     6882 2023-02-18 13:11:45.483942 xpath-localizer-1.0.3/PKG-INFO
--rw-r--r--   0 skayano    (501) staff       (20)     6154 2023-02-18 13:09:29.000000 xpath-localizer-1.0.3/README.rst
-drwxr-xr-x   0 skayano    (501) staff       (20)        0 2023-02-18 13:11:45.478020 xpath-localizer-1.0.3/listener/
--rw-r--r--   0 skayano    (501) staff       (20)     1136 2022-09-23 11:35:40.000000 xpath-localizer-1.0.3/listener/__init__.py
-drwxr-xr-x   0 skayano    (501) staff       (20)        0 2023-02-18 13:11:45.478431 xpath-localizer-1.0.3/robotLocalization/
--rw-r--r--   0 skayano    (501) staff       (20)    14130 2023-02-18 09:43:19.000000 xpath-localizer-1.0.3/robotLocalization/__init__.py
--rw-r--r--   0 skayano    (501) staff       (20)       38 2023-02-18 13:11:45.484447 xpath-localizer-1.0.3/setup.cfg
--rw-r--r--   0 skayano    (501) staff       (20)     1530 2023-02-18 13:11:21.000000 xpath-localizer-1.0.3/setup.py
-drwxr-xr-x   0 skayano    (501) staff       (20)        0 2023-02-18 13:11:45.480764 xpath-localizer-1.0.3/xpath_localizer.egg-info/
--rw-r--r--   0 skayano    (501) staff       (20)     6882 2023-02-18 13:11:44.000000 xpath-localizer-1.0.3/xpath_localizer.egg-info/PKG-INFO
--rw-r--r--   0 skayano    (501) staff       (20)      412 2023-02-18 13:11:45.000000 xpath-localizer-1.0.3/xpath_localizer.egg-info/SOURCES.txt
--rw-r--r--   0 skayano    (501) staff       (20)        1 2023-02-18 13:11:44.000000 xpath-localizer-1.0.3/xpath_localizer.egg-info/dependency_links.txt
--rw-r--r--   0 skayano    (501) staff       (20)       92 2023-02-18 13:11:44.000000 xpath-localizer-1.0.3/xpath_localizer.egg-info/entry_points.txt
--rw-r--r--   0 skayano    (501) staff       (20)      192 2023-02-18 13:11:45.000000 xpath-localizer-1.0.3/xpath_localizer.egg-info/requires.txt
--rw-r--r--   0 skayano    (501) staff       (20)       33 2023-02-18 13:11:45.000000 xpath-localizer-1.0.3/xpath_localizer.egg-info/top_level.txt
-drwxr-xr-x   0 skayano    (501) staff       (20)        0 2023-02-18 13:11:45.483385 xpath-localizer-1.0.3/xploc/
--rw-r--r--   0 skayano    (501) staff       (20)        0 2023-02-18 09:43:19.000000 xpath-localizer-1.0.3/xploc/__init__.py
--rw-r--r--   0 skayano    (501) staff       (20)     8166 2023-02-18 09:43:19.000000 xpath-localizer-1.0.3/xploc/analyze.py
--rw-r--r--   0 skayano    (501) staff       (20)    25884 2023-02-18 09:43:19.000000 xpath-localizer-1.0.3/xploc/api.py
--rw-r--r--   0 skayano    (501) staff       (20)     6247 2023-02-18 09:43:19.000000 xpath-localizer-1.0.3/xploc/loader.py
--rw-r--r--   0 skayano    (501) staff       (20)     2552 2023-02-18 09:43:19.000000 xpath-localizer-1.0.3/xploc/loader_xml.py
--rw-r--r--   0 skayano    (501) staff       (20)     7152 2023-02-18 09:43:19.000000 xpath-localizer-1.0.3/xploc/util.py
+drwxr-xr-x   0 skayano    (501) staff       (20)        0 2023-07-06 13:27:16.921417 xpath-localizer-1.0.4/
+-rw-r--r--   0 skayano    (501) staff       (20)     1064 2022-08-27 13:26:59.000000 xpath-localizer-1.0.4/LICENSE
+-rw-r--r--   0 skayano    (501) staff       (20)     7337 2023-07-06 13:27:16.921075 xpath-localizer-1.0.4/PKG-INFO
+-rw-r--r--   0 skayano    (501) staff       (20)     6500 2023-03-04 15:48:31.000000 xpath-localizer-1.0.4/README.rst
+drwxr-xr-x   0 skayano    (501) staff       (20)        0 2023-07-06 13:27:16.915446 xpath-localizer-1.0.4/listener/
+-rw-r--r--   0 skayano    (501) staff       (20)     1136 2022-09-23 11:35:40.000000 xpath-localizer-1.0.4/listener/__init__.py
+drwxr-xr-x   0 skayano    (501) staff       (20)        0 2023-07-06 13:27:16.915829 xpath-localizer-1.0.4/robotLocalization/
+-rw-r--r--   0 skayano    (501) staff       (20)    14130 2023-02-18 09:43:19.000000 xpath-localizer-1.0.4/robotLocalization/__init__.py
+-rw-r--r--   0 skayano    (501) staff       (20)       38 2023-07-06 13:27:16.921547 xpath-localizer-1.0.4/setup.cfg
+-rw-r--r--   0 skayano    (501) staff       (20)     1638 2023-07-06 13:27:11.000000 xpath-localizer-1.0.4/setup.py
+drwxr-xr-x   0 skayano    (501) staff       (20)        0 2023-07-06 13:27:16.918208 xpath-localizer-1.0.4/xpath_localizer.egg-info/
+-rw-r--r--   0 skayano    (501) staff       (20)     7337 2023-07-06 13:27:16.000000 xpath-localizer-1.0.4/xpath_localizer.egg-info/PKG-INFO
+-rw-r--r--   0 skayano    (501) staff       (20)      412 2023-07-06 13:27:16.000000 xpath-localizer-1.0.4/xpath_localizer.egg-info/SOURCES.txt
+-rw-r--r--   0 skayano    (501) staff       (20)        1 2023-07-06 13:27:16.000000 xpath-localizer-1.0.4/xpath_localizer.egg-info/dependency_links.txt
+-rw-r--r--   0 skayano    (501) staff       (20)       92 2023-07-06 13:27:16.000000 xpath-localizer-1.0.4/xpath_localizer.egg-info/entry_points.txt
+-rw-r--r--   0 skayano    (501) staff       (20)      192 2023-07-06 13:27:16.000000 xpath-localizer-1.0.4/xpath_localizer.egg-info/requires.txt
+-rw-r--r--   0 skayano    (501) staff       (20)       33 2023-07-06 13:27:16.000000 xpath-localizer-1.0.4/xpath_localizer.egg-info/top_level.txt
+drwxr-xr-x   0 skayano    (501) staff       (20)        0 2023-07-06 13:27:16.920526 xpath-localizer-1.0.4/xploc/
+-rw-r--r--   0 skayano    (501) staff       (20)        0 2023-02-18 09:43:19.000000 xpath-localizer-1.0.4/xploc/__init__.py
+-rw-r--r--   0 skayano    (501) staff       (20)     8166 2023-02-18 09:43:19.000000 xpath-localizer-1.0.4/xploc/analyze.py
+-rw-r--r--   0 skayano    (501) staff       (20)    25884 2023-02-18 09:43:19.000000 xpath-localizer-1.0.4/xploc/api.py
+-rw-r--r--   0 skayano    (501) staff       (20)     6247 2023-02-18 09:43:19.000000 xpath-localizer-1.0.4/xploc/loader.py
+-rw-r--r--   0 skayano    (501) staff       (20)     2552 2023-02-18 09:43:19.000000 xpath-localizer-1.0.4/xploc/loader_xml.py
+-rw-r--r--   0 skayano    (501) staff       (20)     7152 2023-02-18 09:43:19.000000 xpath-localizer-1.0.4/xploc/util.py
```

### Comparing `xpath-localizer-1.0.3/LICENSE` & `xpath-localizer-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xpath-localizer-1.0.3/PKG-INFO` & `xpath-localizer-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: xpath-localizer
-Version: 1.0.3
+Version: 1.0.4
 Summary: XPATH internationalization and localization helper
 Author: Shinichiro Kayano
 License: MIT
-Keywords: localization cicd test automation
+Keywords: automation cicd internationalization localization playwright robot test xpath
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Robot Framework :: Tool
+Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Provides-Extra: dev
 Provides-Extra: optional
 License-File: LICENSE
 
 ###################################################
 xpath-localizer (a.k.a robotframework-localization)
@@ -25,21 +26,31 @@
 |license|
 |Conventional Commits|
 
 *************************************************************
 Xpath Localizer Package
 *************************************************************
 
-xpath localizer contains the following tools which can be used to internationalize
+xpath localizer contains the following tools which help you to internationalize
 various web UI automation frameworks such as robotFramework and playwright, or any 
 automation tools that use the XPATH for the web element locator.
 
+xploc command
+    - ``xploc``` command 
+    - this is a test
+
+robotLocalization 
+    ``robotLocalization`` command is to be used with Variabes statement in the robot frame work.
+    It provides ``get_variables`` function and loads variables from specified properties files.
+
+
 - A python command (xploc) to localize properties files containing XPATH specification. 
-- A python library (xploc) to load localized strings and implement a language fallback.
-- A python command (robotLocalization) is used to load **variables** from localized properties files.
+- A python library (xploc) to load localized strings using a BCP-47 compliant language fallback.
+- A python command (robotLocalization) to load **variables** from localized properties files 
+  with the robot Variables statement.
 
 ============
 Installation
 ============
 robotLocalization can be installed with pip/pipenv:
 
 .. code:: bash
@@ -47,29 +58,29 @@
     pip install xpath-localizer
     pipenv install xpath-localizer
 
 =======================
 Usage in robotFramework
 =======================
 
-robotLocalization is used to provide a get_variables function in the robot framework.
+robotLocalization is used to provide a ``get_variables`` function in the robotFramework.
 The get_variables function can be used in the robot test case to load strings from
 properties files by providing a language fallback mechanism. 
 
-.. code:: java
+.. code-block:: properties
 
     # resources/sample.properties
     msg = Hello, World!
 
-.. code:: java
+.. code-block:: properties
 
     # resources/sample_ja.properties
     msg = みなさん、こんにちは!
 
-.. code:: robotFramework
+.. code-block:: robotframework
 
     #   sample.robot
     # 
     #   $ robot --variable language:en sample.robot
     #   $ robot --variable language:ja sample.robot
     #   
     *** Settings ***
@@ -84,15 +95,15 @@
         [Documentation]    robotLocalization Sample
         Log To Console     ${msg}
         Log Variables
 
 Getting variables from get_variables function
 ***********************************************
 
-robotLocalization provides get_variabes function which can be specified 
+robotLocalization provides ``get_variabes`` function which can be specified 
 in the robot Variables statement. 
 
 Syntax in robot test
 --------------------
 
 Variables   **robotLocalization**   *localeId*   *path or file list* *pathOptions*
 
@@ -131,22 +142,22 @@
     xploc [*path list()] --analyze [*robot_file*]
 
 \--analyze
 ^^^^^^^^^^^
 Specifies a robot test case.  Typically, this robot file contains Xpath specifications
 with UI elements or robot variable specifications used in other keywords. 
 
-Extract Mode (robot framework)
+Extract Mode (robotFramework)
 ------------------------------
 
 The extract mode is used to extract strings from a specified robot file.  
 It also generates internationalized robot files by replacing localizable strings
 with variables references. 
 
-\--extract (robot framework)
+\--extract (robotFramework)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 Specifies a robot test case to extract strings. 
 
 \--output_bundle | --outb
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Specifies a bundle file that can be used to store product properties into a single file. 
@@ -178,15 +189,15 @@
 and checks the multiple translations.   If a variant translation is found, it extends the xpath expression 
 to use "OR" condition to check against all of the variant translations. 
 
 \--playwright (robotFramework)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 \--playwright option checks the xpath specification for Playwright when externalizing the robot
-variables.  This option is useful when a robot Framework is used with the Playwright for Python. 
+variables.  This option is useful when a robotFramework is used with the Playwright for Python. 
 
 \--xpath (playwright|pytest)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 \--xpath options specified that the specified files contain XPATH strings only.  This option is useful
 to create a properties file from an XPATH file.  The XPATH file is usually generated by using a 
 test automation framework that uses XPATH expression when locating web elements.
```

### Comparing `xpath-localizer-1.0.3/README.rst` & `xpath-localizer-1.0.4/xpath_localizer.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,56 @@
+Metadata-Version: 2.1
+Name: xpath-localizer
+Version: 1.0.4
+Summary: XPATH internationalization and localization helper
+Author: Shinichiro Kayano
+License: MIT
+Keywords: automation cicd internationalization localization playwright robot test xpath
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Robot Framework :: Tool
+Classifier: Topic :: Software Development :: Internationalization
+Classifier: Topic :: Software Development :: Localization
+Provides-Extra: dev
+Provides-Extra: optional
+License-File: LICENSE
+
 ###################################################
 xpath-localizer (a.k.a robotframework-localization)
 ###################################################
 |license|
 |Conventional Commits|
 
 *************************************************************
 Xpath Localizer Package
 *************************************************************
 
-xpath localizer contains the following tools which can be used to internationalize
+xpath localizer contains the following tools which help you to internationalize
 various web UI automation frameworks such as robotFramework and playwright, or any 
 automation tools that use the XPATH for the web element locator.
 
+xploc command
+    - ``xploc``` command 
+    - this is a test
+
+robotLocalization 
+    ``robotLocalization`` command is to be used with Variabes statement in the robot frame work.
+    It provides ``get_variables`` function and loads variables from specified properties files.
+
+
 - A python command (xploc) to localize properties files containing XPATH specification. 
-- A python library (xploc) to load localized strings and implement a language fallback.
-- A python command (robotLocalization) is used to load **variables** from localized properties files.
+- A python library (xploc) to load localized strings using a BCP-47 compliant language fallback.
+- A python command (robotLocalization) to load **variables** from localized properties files 
+  with the robot Variables statement.
 
 ============
 Installation
 ============
 robotLocalization can be installed with pip/pipenv:
 
 .. code:: bash
@@ -26,29 +58,29 @@
     pip install xpath-localizer
     pipenv install xpath-localizer
 
 =======================
 Usage in robotFramework
 =======================
 
-robotLocalization is used to provide a get_variables function in the robot framework.
+robotLocalization is used to provide a ``get_variables`` function in the robotFramework.
 The get_variables function can be used in the robot test case to load strings from
 properties files by providing a language fallback mechanism. 
 
-.. code:: java
+.. code-block:: properties
 
     # resources/sample.properties
     msg = Hello, World!
 
-.. code:: java
+.. code-block:: properties
 
     # resources/sample_ja.properties
     msg = みなさん、こんにちは!
 
-.. code:: robotFramework
+.. code-block:: robotframework
 
     #   sample.robot
     # 
     #   $ robot --variable language:en sample.robot
     #   $ robot --variable language:ja sample.robot
     #   
     *** Settings ***
@@ -63,15 +95,15 @@
         [Documentation]    robotLocalization Sample
         Log To Console     ${msg}
         Log Variables
 
 Getting variables from get_variables function
 ***********************************************
 
-robotLocalization provides get_variabes function which can be specified 
+robotLocalization provides ``get_variabes`` function which can be specified 
 in the robot Variables statement. 
 
 Syntax in robot test
 --------------------
 
 Variables   **robotLocalization**   *localeId*   *path or file list* *pathOptions*
 
@@ -110,22 +142,22 @@
     xploc [*path list()] --analyze [*robot_file*]
 
 \--analyze
 ^^^^^^^^^^^
 Specifies a robot test case.  Typically, this robot file contains Xpath specifications
 with UI elements or robot variable specifications used in other keywords. 
 
-Extract Mode (robot framework)
+Extract Mode (robotFramework)
 ------------------------------
 
 The extract mode is used to extract strings from a specified robot file.  
 It also generates internationalized robot files by replacing localizable strings
 with variables references. 
 
-\--extract (robot framework)
+\--extract (robotFramework)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 Specifies a robot test case to extract strings. 
 
 \--output_bundle | --outb
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Specifies a bundle file that can be used to store product properties into a single file. 
@@ -157,15 +189,15 @@
 and checks the multiple translations.   If a variant translation is found, it extends the xpath expression 
 to use "OR" condition to check against all of the variant translations. 
 
 \--playwright (robotFramework)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 \--playwright option checks the xpath specification for Playwright when externalizing the robot
-variables.  This option is useful when a robot Framework is used with the Playwright for Python. 
+variables.  This option is useful when a robotFramework is used with the Playwright for Python. 
 
 \--xpath (playwright|pytest)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 \--xpath options specified that the specified files contain XPATH strings only.  This option is useful
 to create a properties file from an XPATH file.  The XPATH file is usually generated by using a 
 test automation framework that uses XPATH expression when locating web elements. 
@@ -180,7 +212,9 @@
 
 
 .. |license| image:: https://img.shields.io/badge/license-MIT-blue.svg
 .. |robotLocalization_icon| image:: robotLocalization.png
 .. |Conventional Commits| image:: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 
 
+
+
```

### Comparing `xpath-localizer-1.0.3/listener/__init__.py` & `xpath-localizer-1.0.4/listener/__init__.py`

 * *Files identical despite different names*

### Comparing `xpath-localizer-1.0.3/robotLocalization/__init__.py` & `xpath-localizer-1.0.4/robotLocalization/__init__.py`

 * *Files identical despite different names*

### Comparing `xpath-localizer-1.0.3/setup.py` & `xpath-localizer-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='xpath-localizer',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     license='MIT',
     author='Shinichiro Kayano',
     description='XPATH internationalization and localization helper',
     long_description=long_description,
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Environment :: Console',
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Framework :: Robot Framework :: Tool',
+        'Topic :: Software Development :: Internationalization',
         'Topic :: Software Development :: Localization'
     ],
-    install_requires=['jproperties>=2.1.1', 'requests>=2.22.0'],
+    install_requires=['jproperties>=2.1.1', 'requests>=2.31.0'],
     extras_require={
         'dev': ["pytest", "docutils", "pygments"],
         'optional': ["robotframework", "robotframework-seleniumlibrary" ,
             "robotframework-autorecorder", "robotframework-requests" , "opencv-python"],
     },
-    keywords="localization cicd test automation",
+    keywords="automation cicd internationalization localization playwright robot test xpath",
     entry_points={
         'console_scripts': [
             'robotLocalization=robotLocalization:main',
             'xploc=robotLocalization:main',
         ],
     },
```

### Comparing `xpath-localizer-1.0.3/xploc/analyze.py` & `xpath-localizer-1.0.4/xploc/analyze.py`

 * *Files identical despite different names*

### Comparing `xpath-localizer-1.0.3/xploc/api.py` & `xpath-localizer-1.0.4/xploc/api.py`

 * *Files identical despite different names*

### Comparing `xpath-localizer-1.0.3/xploc/loader.py` & `xpath-localizer-1.0.4/xploc/loader.py`

 * *Files identical despite different names*

### Comparing `xpath-localizer-1.0.3/xploc/loader_xml.py` & `xpath-localizer-1.0.4/xploc/loader_xml.py`

 * *Files identical despite different names*

### Comparing `xpath-localizer-1.0.3/xploc/util.py` & `xpath-localizer-1.0.4/xploc/util.py`

 * *Files identical despite different names*

