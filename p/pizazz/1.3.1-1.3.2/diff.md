# Comparing `tmp/pizazz-1.3.1.tar.gz` & `tmp/pizazz-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizazz-1.3.1.tar", last modified: Fri Apr 21 13:55:53 2023, max compression
+gzip compressed data, was "pizazz-1.3.2.tar", last modified: Thu Jul  6 06:10:35 2023, max compression
```

## Comparing `pizazz-1.3.1.tar` & `pizazz-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 13:55:53.484700 pizazz-1.3.1/
--rw-rw-rw-   0        0        0      157 2023-04-18 15:26:46.000000 pizazz-1.3.1/AUTHORS.md
--rw-rw-rw-   0        0        0     1283 2023-04-21 13:55:39.000000 pizazz-1.3.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2022-05-22 14:38:29.000000 pizazz-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      203 2022-05-22 14:38:29.000000 pizazz-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11450 2023-04-21 13:55:53.484700 pizazz-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    10217 2023-04-19 22:06:08.000000 pizazz-1.3.1/README.md
--rw-rw-rw-   0        0        0     2215 2022-10-08 16:54:54.000000 pizazz-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     1473 2023-04-21 13:55:53.484700 pizazz-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      115 2023-04-21 12:33:15.000000 pizazz-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:55:53.400021 pizazz-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 13:55:53.469066 pizazz-1.3.1/src/pizazz/
--rw-rw-rw-   0        0        0      356 2023-04-21 13:55:39.000000 pizazz-1.3.1/src/pizazz/__init__.py
--rw-rw-rw-   0        0        0     8109 2023-04-21 12:33:15.000000 pizazz-1.3.1/src/pizazz/pizazz.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:55:53.484700 pizazz-1.3.1/src/pizazz.egg-info/
--rw-rw-rw-   0        0        0    11450 2023-04-21 13:55:53.000000 pizazz-1.3.1/src/pizazz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-21 13:55:53.000000 pizazz-1.3.1/src/pizazz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 13:55:53.000000 pizazz-1.3.1/src/pizazz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-21 13:55:53.000000 pizazz-1.3.1/src/pizazz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 13:55:53.000000 pizazz-1.3.1/src/pizazz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 06:10:35.725914 pizazz-1.3.2/
+-rw-rw-rw-   0        0        0      157 2023-04-18 15:26:46.000000 pizazz-1.3.2/AUTHORS.md
+-rw-rw-rw-   0        0        0     1587 2023-07-06 06:10:20.000000 pizazz-1.3.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2022-05-22 14:38:29.000000 pizazz-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      203 2022-05-22 14:38:29.000000 pizazz-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    11730 2023-07-06 06:10:35.725914 pizazz-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10493 2023-07-06 05:59:48.000000 pizazz-1.3.2/README.md
+-rw-rw-rw-   0        0        0     2215 2022-10-08 16:54:54.000000 pizazz-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1473 2023-07-06 06:10:35.725914 pizazz-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      115 2023-04-21 12:33:15.000000 pizazz-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:10:35.694112 pizazz-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 06:10:35.710255 pizazz-1.3.2/src/pizazz/
+-rw-rw-rw-   0        0        0      356 2023-07-06 06:10:20.000000 pizazz-1.3.2/src/pizazz/__init__.py
+-rw-rw-rw-   0        0        0     8109 2023-04-21 12:33:15.000000 pizazz-1.3.2/src/pizazz/pizazz.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:10:35.725914 pizazz-1.3.2/src/pizazz.egg-info/
+-rw-rw-rw-   0        0        0    11730 2023-07-06 06:10:35.000000 pizazz-1.3.2/src/pizazz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-07-06 06:10:35.000000 pizazz-1.3.2/src/pizazz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:10:35.000000 pizazz-1.3.2/src/pizazz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-06 06:10:35.000000 pizazz-1.3.2/src/pizazz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 06:10:35.000000 pizazz-1.3.2/src/pizazz.egg-info/top_level.txt
```

### Comparing `pizazz-1.3.1/CHANGELOG.md` & `pizazz-1.3.2/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.2 (2023-07-06)
+### Documentation
+* Update hyperlinks ([`bc1fa76`](https://github.com/Stephen-RA-King/pizazz/commit/bc1fa7627be96cff136eaaa27aa002c26db17aed))
+* Minor update to markdown ([`5273d0f`](https://github.com/Stephen-RA-King/pizazz/commit/5273d0f9cdfd5cad5d631a96449ed67e379f6bc0))
+
 ## v1.3.1 (2023-04-21)
 ### Fix
 * Shebang for version 3 env ([`3202092`](https://github.com/Stephen-RA-King/pizazz/commit/320209290e0782ae20229d88227989543bda2978))
 
 ### Documentation
 * Update email links ([`c726e4e`](https://github.com/Stephen-RA-King/pizazz/commit/c726e4e8ae8d0fd6d449b3833cc3c3b39c0ec270))
 * Rename base cookiecutter name ([`8aa5b0f`](https://github.com/Stephen-RA-King/pizazz/commit/8aa5b0f6ead9683900f453fda03506caaff69676))
```

### Comparing `pizazz-1.3.1/LICENSE` & `pizazz-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.1/PKG-INFO` & `pizazz-1.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizazz
-Version: 1.3.1
+Version: 1.3.2
 Summary: Easy configuration and control of 74HC595 Shift Registers on a Raspberry Pi
 Home-page: https://github.com/stephen-ra-king/pizazz
 Download-URL: 
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -23,15 +23,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # Pizazz
 
-\_**A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.**-
+**A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.**
 
 [![PyPI version](https://badge.fury.io/py/pizazz.svg)](https://badge.fury.io/py/pizazz)
 [![Documentation Status](https://readthedocs.org/projects/pizazz/badge/?version=latest)](https://pizazz.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/personalized-badge/pizazz?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pizazz)
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -237,22 +237,24 @@
 ## Meta
 
 ---
 
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/github.png)](https://github.com/Stephen-RA-King/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pizazz)
-[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/www.png)](https://www.justpython.tech)
+[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/www.png)](https://stephen-ra-king.github.io/justpython/)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/email.png)](mailto:sking.github@gmail.com)
 
 Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
+Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.2.1
+
+Digital object identifier: [![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
 
 <!-- Markdown link & img dfn's -->
 
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
 [rpi-gpio-url]: https://pypi.org/project/RPi.GPIO/
 [status-board-url]: https://thepihut.com/products/status-board-pro
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
@@ -265,8 +267,10 @@
 [bandit-url]: https://github.com/PyCQA/bandit
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [license-image]: https://img.shields.io/pypi/l/pizazz
 [license-url]: https://github.com/Stephen-RA-King/pizazz/blob/main/LICENSE
 [mit-license-image]: https://img.shields.io/badge/license-MIT-blue
 [mit-license-url]: https://choosealicense.com/licenses/mit/
+[pydough-image]: https://img.shields.io/badge/pydough-2023-orange
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [wiki]: https://github.com/stephen-ra-king/pizazz/wiki
```

### Comparing `pizazz-1.3.1/README.md` & `pizazz-1.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Pizazz
 
-\_**A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.**-
+**A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.**
 
 [![PyPI version](https://badge.fury.io/py/pizazz.svg)](https://badge.fury.io/py/pizazz)
 [![Documentation Status](https://readthedocs.org/projects/pizazz/badge/?version=latest)](https://pizazz.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/personalized-badge/pizazz?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pizazz)
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -210,22 +210,24 @@
 ## Meta
 
 ---
 
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/github.png)](https://github.com/Stephen-RA-King/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pizazz)
-[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/www.png)](https://www.justpython.tech)
+[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/www.png)](https://stephen-ra-king.github.io/justpython/)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/email.png)](mailto:sking.github@gmail.com)
 
 Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
+Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.2.1
+
+Digital object identifier: [![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
 
 <!-- Markdown link & img dfn's -->
 
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
 [rpi-gpio-url]: https://pypi.org/project/RPi.GPIO/
 [status-board-url]: https://thepihut.com/products/status-board-pro
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
@@ -238,8 +240,10 @@
 [bandit-url]: https://github.com/PyCQA/bandit
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [license-image]: https://img.shields.io/pypi/l/pizazz
 [license-url]: https://github.com/Stephen-RA-King/pizazz/blob/main/LICENSE
 [mit-license-image]: https://img.shields.io/badge/license-MIT-blue
 [mit-license-url]: https://choosealicense.com/licenses/mit/
+[pydough-image]: https://img.shields.io/badge/pydough-2023-orange
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [wiki]: https://github.com/stephen-ra-king/pizazz/wiki
```

### Comparing `pizazz-1.3.1/pyproject.toml` & `pizazz-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.1/setup.cfg` & `pizazz-1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.1/src/pizazz/pizazz.py` & `pizazz-1.3.2/src/pizazz/pizazz.py`

 * *Files identical despite different names*

### Comparing `pizazz-1.3.1/src/pizazz.egg-info/PKG-INFO` & `pizazz-1.3.2/src/pizazz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizazz
-Version: 1.3.1
+Version: 1.3.2
 Summary: Easy configuration and control of 74HC595 Shift Registers on a Raspberry Pi
 Home-page: https://github.com/stephen-ra-king/pizazz
 Download-URL: 
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -23,15 +23,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # Pizazz
 
-\_**A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.**-
+**A utility class to leverage 74HC595 shift register chips with a Raspberry Pi.**
 
 [![PyPI version](https://badge.fury.io/py/pizazz.svg)](https://badge.fury.io/py/pizazz)
 [![Documentation Status](https://readthedocs.org/projects/pizazz/badge/?version=latest)](https://pizazz.readthedocs.io/en/latest/?badge=latest)
 [![Downloads](https://static.pepy.tech/personalized-badge/pizazz?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pizazz)
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -237,22 +237,24 @@
 ## Meta
 
 ---
 
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/github.png)](https://github.com/Stephen-RA-King/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pizazz)
-[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/www.png)](https://www.justpython.tech)
+[![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/www.png)](https://stephen-ra-king.github.io/justpython/)
 [![](https://github.com/Stephen-RA-King/pizazz/raw/main/assets/email.png)](mailto:sking.github@gmail.com)
 
 Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
+Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.2.1
+
+Digital object identifier: [![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
 
 <!-- Markdown link & img dfn's -->
 
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
 [rpi-gpio-url]: https://pypi.org/project/RPi.GPIO/
 [status-board-url]: https://thepihut.com/products/status-board-pro
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
@@ -265,8 +267,10 @@
 [bandit-url]: https://github.com/PyCQA/bandit
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [license-image]: https://img.shields.io/pypi/l/pizazz
 [license-url]: https://github.com/Stephen-RA-King/pizazz/blob/main/LICENSE
 [mit-license-image]: https://img.shields.io/badge/license-MIT-blue
 [mit-license-url]: https://choosealicense.com/licenses/mit/
+[pydough-image]: https://img.shields.io/badge/pydough-2023-orange
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [wiki]: https://github.com/stephen-ra-king/pizazz/wiki
```

